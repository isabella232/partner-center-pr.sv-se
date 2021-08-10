---
title: Återställa administratörsbehörighet för Azure CSP
ms.topic: how-to
ms.date: 05/27/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-customers
description: Lär dig hur du hjälper kunder att återställa en partners administratörsbehörighet så att partnern kan hjälpa till att hantera en kunds Azure Molnlösningsleverantör prenumerationer (CSP).
author: dhirajgandhi
ms.author: dhgandhi
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 53f9cf6533127231c152fbba0d7d7fbdadd6a897424f3d9383818fb45edf3465
ms.sourcegitcommit: 121f1b9cbd88faeba60dc9b475f9c0647cdc933c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/06/2021
ms.locfileid: "115682664"
---
# <a name="reinstate-admin-privileges-for-a-customers-azure-csp-subscriptions"></a>Återställa administratörsbehörigheter för en kunds Azure CSP prenumerationer  

**Lämpliga roller:** Global | Administratörsagent

Som CSP Molnlösningsleverantör partner förväntar sig kunderna ofta att du hanterar deras Azure-användning och deras system åt dem. Du måste ha administratörsbehörighet för att göra det. Vissa behörigheter beviljas när din återförsäljarrelation med kunden upprättas. Andra beviljas till dig av din kund.

## <a name="admin-privileges-for-azure-in-csp"></a>Administratörsbehörighet för Azure i CSP

Det finns två nivåer av administratörsbehörighet för Azure i CSP.

- **Administratörsbehörighet på klientorganisationsnivå (delegerade administratörsbehörigheter):** CSP-partner får dessa behörigheter när de upprättar en CSP-återförsäljarrelation med kunder. Delegerade administratörsbehörigheter ger CSP-partner åtkomst till sina kunders klienter. Med den här åtkomsten kan de använda administrativa funktioner som att lägga till/hantera användare, återställa lösenord och hantera användarlicenser.
- **Administratörsbehörighet på prenumerationsnivå:** CSP-partner får dessa behörigheter när de skapar Azure CSP prenumerationer för sina kunder. Med dessa behörigheter får CSP-partner fullständig åtkomst till dessa prenumerationer, vilket gör att de kan etablera och hantera Azure-resurser.

## <a name="reinstate-csp-a-partners-admin-privileges"></a>Återställa CSP:ens administratörsbehörighet

Kunden kan skapa CSP-rolltilldelningen på nytt om du anger `object ID` för gruppen AdminAgents till kunden. För att återfå delegerade administratörsbehörigheter måste du arbeta med kunden genom följande steg.

1. Logga in på instrumentpanelen i Partnercenter.

2. På menyn i Partnercenter väljer du **Kunder.**

3. Välj den kund som du arbetar med och **begär en återförsäljarrelation.** Den här åtgärden genererar en länk till kunden som har administratörsrättigheter för klientorganisationen.

4. Kunden måste välja länken och godkänna begäran om återförsäljarrelation.

   :::image type="content" source="images/azure/revoke4.png" alt-text="E-postexempel för att skapa återförsäljarrelation.":::

5. Du, partnern, måste ansluta till partnerklientorganisationen för att hämta objekt-ID för gruppen AdminAgents.
  
   ```powershell
   Connect-AzAccount -Tenant "Partner tenant"
   # Get Object ID of AdminAgents group
   Get-AzADGroup -DisplayName AdminAgents
   ```

6. Kunden måste sedan göra följande med antingen PowerShell eller Azure CLI. Kunden måste ha:

- Rollen som ägare **eller** **administratör för användaråtkomst** 
- Behörigheter för att skapa rolltilldelningar på prenumerationsnivå

   a. Endast för PowerShell måste kunden uppdatera `Az.Resources` modulen.
   ```powershell
   Update-Module Az.Resources
   ```

   b. Kunden ansluter till den klientorganisation där CSP-prenumerationen finns.
   ```powershell
   Connect-AzAccount -TenantID "<Customer tenant>"
   ```
   ```azurecli
   az login --tenant <Customer tenant>
   ```

   c. Kunden ansluter till prenumerationen. Detta gäller *endast* om användaren har rolltilldelningsbehörigheter för flera prenumerationer i klientorganisationen.

   ```powershell
   Set-AzContext -SubscriptionID <"CSP Subscription ID">
   ```
   ```azurecli
   az account set --subscription <CSP Subscription ID>
   ```

   d. Kunden skapar sedan rolltilldelningen.
    
   ```powershell
   New-AzRoleAssignment -ObjectID "<Object ID of the Admin Agents group provided by partner>" -RoleDefinitionName "Owner" -Scope "/subscriptions/'<CSP subscription ID>'"
   ```
   ```azurecli
   az role assignment create --role "Owner" --assignee-object-id <Object Id of the Admin Agents group provided by partner> --scope "/subscriptions/<CSP Subscription Id>"
   ```

I stället för att bevilja ägarbehörigheter i prenumerationsomfånget kan du bevilja på resursgrupps- eller resursnivå. 

- På resursgruppsnivå

   ```powershell
   New-AzRoleAssignment -ObjectID "<Object ID from step 3>" -RoleDefinitionName Owner -Scope "/subscriptions/'SubscriptionID of CSP subscription'/resourceGroups/'Resource group name'"
   ```

   ```azurecli
   az role assignment create --role "Owner" --assignee-object-id <Object Id of the Admin Agents group provided by partner> --scope "/subscriptions/<CSP Subscription Id>//resourceGroups/<Resource group name>"
   ```

- På resursnivå

   ```powershell
   New-AzRoleAssignment -ObjectID "<Object ID from step 3>" -RoleDefinitionName Owner -Scope "<Resource URI>"
   ```

   ```azurecli
   az role assignment create --role "Owner" --assignee-object-id <Object Id of the Admin Agents group provided by partner> --scope "<Resource URI>"
   ```

Om ovanstående steg inte fungerar eller om du får felmeddelanden när du försöker utföra dem kan du prova följande "catch-all"-procedur för att återställa administratörsrättigheterna för din kund.

```powershell
Install-Module -Name Az.Resources -Force -Verbose
Import-Module -Name Az.Resources -Verbose -MinimumVersion 4.1.1
Connect-AzAccount -Tenant <customer tenant>
Set-AzContext -SubscriptionId <customer subscriptions>
New-AzRoleAssignment -ObjectId <principal ID> -RoleDefinitionName "Owner" -Scope "/subscriptions/<customer subscription>" -ObjectType "ForeignGroup"
```

### <a name="troubleshooting"></a>Felsökning

Om kunden inte kan slutföra steg 6 ovan kan kunden prova följande kommando:

```powershell
New-AzRoleAssignment -ObjectId <principal ID> -RoleDefinitionName "Owner" -Scope "/subscriptions/<costumer subscription>" -ObjectType "ForeignGroup" -Debug > newRoleAssignment.log
```

Ange den resulterande `newRoleAssignment.log` filen till Microsoft för ytterligare analys.

Om "catch-all"-proceduren misslyckas under `Import-Module` kan du prova följande steg:
- Om importen misslyckas på grund av att modulen används startar du om PowerShell-sessionen genom att stänga och öppna alla fönster igen.
- Kontrollera versionen av `Az.Resources` med `Get-Module Az.Resources -ListAvailable` .
- Om version 4.1.1 inte finns i den tillgängliga listan måste du använda `Update-Module Az.Resources -Force` .
- Om felet visar att `Az.Accounts` måste vara en specifik version uppdaterar du även den modulen och ersätter `Az.Resources` med `Az.Accounts` . Du måste sedan starta om PowerShell-sessionen.


## <a name="next-steps"></a>Nästa steg

- [Hantera prenumerationer och resurser under Azure-planen](azure-plan-manage.md)
