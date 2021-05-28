---
title: Återställa administratörsbehörigheter för Azure CSP
ms.topic: how-to
ms.date: 05/27/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Lär dig hur du hjälper kunder att återställa en partners administratörsbehörighet så att partnern kan hantera en kunds Azure CSP prenumerationer.
author: dhirajgandhi
ms.author: dhgandhi
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: ca4c8323562e6c6f1d762465cad86e7ae113eb19
ms.sourcegitcommit: beba696954b62ab5396a893d050d0c2c211aeafc
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 05/28/2021
ms.locfileid: "110601434"
---
# <a name="reinstate-admin-privileges-for-a-customers-azure-csp-subscriptions"></a>Återställa administratörsbehörigheter för en kunds Azure CSP prenumerationer  

**Lämpliga roller:** Globala | Administratörsagent

Som CSP-partner förväntar sig kunderna ofta att du hanterar deras Azure-användning och deras system åt dem. Du måste ha administratörsbehörighet för att göra det. Vissa behörigheter beviljas när din återförsäljarrelation med kunden upprättas. Andra beviljas till dig av din kund.

## <a name="admin-privileges-for-azure-in-csp"></a>Administratörsbehörighet för Azure i CSP

Det finns två nivåer av administratörsbehörighet för Azure i CSP.

- **Administratörsbehörighet på klientorganisationsnivå (delegerade administratörsbehörigheter):** CSP-partner får dessa behörigheter när de upprättar en CSP-återförsäljarrelation med kunder. Delegerade administratörsbehörigheter ger CSP-partner åtkomst till sina kunders klienter. Den här åtkomsten gör att de kan använda administrativa funktioner som att lägga till/hantera användare, återställa lösenord och hantera användarlicenser.
- **Administratörsbehörighet på prenumerationsnivå:** CSP-partner får dessa behörigheter när de skapar Azure CSP prenumerationer för sina kunder. Dessa behörigheter ger CSP-partner fullständig åtkomst till dessa prenumerationer, vilket gör att de kan etablera och hantera Azure-resurser.

## <a name="reinstate-csp-a-partners-admin-privileges"></a>Återställa CSP:ens administratörsbehörighet

Kunden kan skapa CSP-rolltilldelningen på nytt om du anger `object ID` för gruppen AdminAgents till kunden. För att återfå delegerade administratörsbehörigheter måste du arbeta med kunden genom följande steg.

1. Logga in på instrumentpanelen i Partnercenter.

2. På menyn i Partnercenter väljer du **Kunder.**

3. Välj den kund som du arbetar med och **begär en återförsäljarrelation.** Den här åtgärden genererar en länk till kunden som har administratörsrättigheter för klientorganisationen.

4. Kunden måste välja länken och godkänna begäran om återförsäljarrelation.

   :::image type="content" source="images/azure/revoke4.png" alt-text="E-postexempel för att skapa återförsäljarrelation":::

5. Du, partnern, måste ansluta till partnerklientorganisationen för att hämta objekt-ID för gruppen AdminAgents.
  
   ```powershell
   Connect-AzAccount -Tenant "Partner tenant"
   # Get Object ID of AdminAgents group
   Get-AzADGroup -DisplayName AdminAgents
   ```

6. Kunden måste sedan göra följande med antingen PowerShell eller Azure CLI. Kunden måste ha:

- Rollen som ägare **eller** **administratör för användaråtkomst** 
- Behörighet att skapa rolltilldelningar på prenumerationsnivå

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

I stället för att bevilja ägarbehörighet i prenumerationsomfånget kan du bevilja på resursgrupps- eller resursnivå. 

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

## <a name="next-steps"></a>Nästa steg

- [Hantera prenumerationer och resurser under Azure-planen](azure-plan-manage.md)
