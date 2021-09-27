---
title: Återställ administratörsbehörigheter för Azure CSP
ms.topic: how-to
ms.date: 05/27/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-customers
description: Lär dig hur du hjälper kunder att återställa en partners administratörsbehörighet så att partnern kan hjälpa till att hantera en kunds Azure Molnlösningsleverantör prenumerationer (CSP).
author: dhirajgandhi
ms.author: dhgandhi
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: ea64a6030acbc41aec085b3a0a7927d8ed28cc88
ms.sourcegitcommit: d731813da1d31519dc2dc583d17899e5cf4ec1b2
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/27/2021
ms.locfileid: "129070174"
---
# <a name="reinstate-admin-privileges-for-a-customers-azure-csp-subscriptions"></a>Återställa administratörsbehörigheter för en kunds Azure CSP prenumerationer  

**Lämpliga roller:** Global | Administratörsagent

Som CSP Molnlösningsleverantör partner (CSP) förlitar sig dina kunder ofta på att du hanterar deras Azure-användning och deras system. Du behöver administratörsbehörighet för att hjälpa dem. Om du inte redan har administratörsbehörighet kan du samarbeta med kunden för att återställa dem.

## <a name="admin-privileges-for-azure-in-the-csp-program"></a>Administratörsbehörighet för Azure i CSP-programmet

Vissa administratörsbehörigheter beviljas automatiskt när du upprättar en återförsäljarrelation med kunden. Andra måste beviljas till dig av kunden. Det finns två nivåer av administratörsbehörighet för Azure i CSP.

- **Administratörsbehörigheter på klientorganisationsnivå (dvs. delegerade administratörsbehörigheter)** ger dig åtkomst till dina kunders klienter. Med den här åtkomsten kan du göra administrativa funktioner som att lägga till och hantera användare, återställa lösenord och hantera användarlicenser. Du får dessa behörigheter när du etablerar CSP-återförsäljarrelationer med kunder.
- **Administratörsbehörighet på prenumerationsnivå** ger dig fullständig åtkomst till dina kunders Azure CSP prenumerationer. Med den här åtkomsten kan du etablera och hantera deras Azure-resurser. Du får dessa behörigheter när du skapar Azure CSP prenumerationer för dina kunder.

## <a name="how-to-reinstate-your-csp-admin-privileges"></a>Återställa dina CSP-administratörsbehörigheter

Du kan arbeta med kunden för att återfå delegerade administratörsbehörigheter.

> [!NOTE]
> Förhandsversionsgränssnittet i Partnercenter ger en mer effektiv och produktiv användarupplevelse via logiskt grupperade arbetsytor. Mer information om arbetsytegränssnittet och hur du aktiverar det finns i [Getting around Partner Center (Ta sig runt i Partnercenter).](get-around-partner-center.md#turn-workspaces-on-and-off)

#### <a name="workspaces-view"></a>[Vy över arbetsytor](#tab/workspaces-view)

1. Logga in på [instrumentpanelen i Partnercenter](https://partner.microsoft.com/dashboard).

2. Välj **panelen** Kunder.

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

#### <a name="current-view"></a>[Aktuell vy](#tab/current-view)

1. Logga in på [instrumentpanelen i Partnercenter](https://partner.microsoft.com/dashboard).

2. I menyn i Partnercenter väljer du **Kunder.**

3. Välj den kund som du arbetar med och begär **en återförsäljarrelation.** Den här åtgärden skickar en länk till kunden via e-post.

   :::image type="content" source="images/azure/revoke4.png" alt-text="E-postexempel för att skapa återförsäljarrelation.":::

4. När kunden godkänner begäran om återförsäljarrelation via länken ansluter du till partnerklientorganisationen för att hämta för `object ID` gruppen AdminAgents.
  
   ```powershell
   Connect-AzAccount -Tenant "Partner tenant"
   # Get Object ID of AdminAgents group
   Get-AzADGroup -DisplayName AdminAgents
   ```

5. Kontrollera att kunden har:

   1. Rollen som ägare **eller** **administratör för användaråtkomst** 
   2. Behörigheter för att skapa rolltilldelningar på prenumerationsnivå

6. För att slutföra processen måste kunden göra följande med antingen PowerShell eller Azure CLI. 

   1. Om du använder PowerShell måste kunden uppdatera `Az.Resources` modulen.

       ```powershell
       Update-Module Az.Resources
       ```

   2. Kunden bör ansluta till den klientorganisation där CSP-prenumerationen finns.

      ```powershell
      Connect-AzAccount -TenantID "<Customer tenant>"
      ```

      ```azurecli
      az login --tenant <Customer tenant>
      ```

   3. Kunden bör nu ansluta till prenumerationen. Detta gäller *endast* om användaren har rolltilldelningsbehörigheter för flera prenumerationer i klientorganisationen.

      ```powershell
      Set-AzContext -SubscriptionID <"CSP Subscription ID">
      ```

      ```azurecli
      az account set --subscription <CSP Subscription ID>
      ```

   4. Kunden kan sedan skapa rolltilldelningen.

      ```powershell
      New-AzRoleAssignment -ObjectID "<Object ID of the AdminAgents group from step 4>" -RoleDefinitionName "Owner" -Scope "/subscriptions/'<CSP subscription ID>'"
      ```

      ```azurecli
      az role assignment create --role "Owner" --assignee-object-id <Object ID of the AdminAgents group from step 4> --scope "/subscriptions/<CSP Subscription Id>"
      ```

I stället för att bevilja ägarbehörighet på prenumerationsnivå kan du bevilja dem på resursgrupps- eller resursnivå: 

- På resursgruppsnivå

   ```powershell
   New-AzRoleAssignment -ObjectID "<Object ID of the AdminAgents group from step 4>" -RoleDefinitionName Owner -Scope "/subscriptions/'SubscriptionID of CSP subscription'/resourceGroups/'Resource group name'"
   ```

   ```azurecli
   az role assignment create --role "Owner" --assignee-object-id <Object ID of the AdminAgents group from step 4> --scope "/subscriptions/<CSP Subscription Id>//resourceGroups/<Resource group name>"
   ```

- På resursnivå

   ```powershell
   New-AzRoleAssignment -ObjectID "<Object ID of the AdminAgents group from step 4>" -RoleDefinitionName Owner -Scope "<Resource URI>"
   ```

   ```azurecli
   az role assignment create --role "Owner" --assignee-object-id <Object ID of the AdminAgents group from step 4> --scope "<Resource URI>"
   ```

Om ovanstående steg inte fungerar eller om du får fel när du försöker göra dem kan du prova följande "catch-all"-procedur för att återställa administratörsrättigheterna för din kund:

```powershell
Install-Module -Name Az.Resources -Force -Verbose
Import-Module -Name Az.Resources -Verbose -MinimumVersion 4.1.1
Connect-AzAccount -Tenant <customer tenant>
Set-AzContext -SubscriptionId <customer subscriptions>
New-AzRoleAssignment -ObjectId <principal ID> -RoleDefinitionName "Owner" -Scope "/subscriptions/<customer subscription>" -ObjectType "ForeignGroup"
```

* * *

### <a name="troubleshooting"></a>Felsökning
Om kunden inte kan slutföra steg 6 föreslår du följande kommando och anger den resulterande `newRoleAssignment.log` filen till Microsoft för ytterligare analys:

```powershell
New-AzRoleAssignment -ObjectId <principal ID> -RoleDefinitionName "Owner" -Scope "/subscriptions/<customer subscription>" -ObjectType "ForeignGroup" -Debug > newRoleAssignment.log
```

Om "catch-all"-proceduren misslyckas under `Import-Module` kan du prova följande steg:
- Om importen misslyckas på grund av att modulen används startar du om PowerShell-sessionen genom att stänga och öppna alla fönster igen.
- Kontrollera versionen av `Az.Resources` med `Get-Module Az.Resources -ListAvailable` .
- Om version 4.1.1 inte finns i den tillgängliga listan måste du använda `Update-Module Az.Resources -Force` .
- Om felet visar att `Az.Accounts` måste vara en specifik version uppdaterar du även den modulen och ersätter `Az.Resources` med `Az.Accounts` . Du måste sedan starta om PowerShell-sessionen.


## <a name="next-steps"></a>Nästa steg

- [Hantera prenumerationer och resurser under Azure-planen](azure-plan-manage.md)
