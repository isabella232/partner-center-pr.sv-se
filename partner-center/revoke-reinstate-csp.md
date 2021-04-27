---
title: Återställa administratörsbehörighet för Azure CSP
ms.topic: how-to
ms.date: 04/08/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Lär dig hur du hjälper kunder att återställa en partners administratörsbehörighet så att partnern kan hjälpa till att hantera en kunds Azure CSP prenumerationer.
author: dhirajgandhi
ms.author: dhgandhi
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 26768bdf33c03145a893fa445eab6ebf92ca9b1c
ms.sourcegitcommit: efd711b0e65c55f24ce5b9636abd7b5a8cc719fe
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/27/2021
ms.locfileid: "108018195"
---
# <a name="reinstate-admin-privileges-for-a-customers-azure-csp-subscriptions"></a>Återställa administratörsbehörigheter för en kunds Azure CSP prenumerationer  

**Lämpliga roller**

- Global administratör
- Administratörsagent

Som CSP-partner förväntar sig kunderna ofta att du hanterar deras Azure-användning och deras system åt dem. Om du gör det måste du ha administratörsbehörighet. Vissa behörigheter beviljas när din återförsäljarrelation med kunden upprättas. Andra beviljas till dig av din kund.

## <a name="admin-privileges-for-azure-in-csp"></a>Administratörsbehörighet för Azure i CSP

Det finns två nivåer av administratörsbehörighet för Azure i CSP.

**Administratörsbehörigheter på klientorganisationsnivå** **(delegerade administratörsbehörigheter)**– CSP-partner får dessa privilegier när de upprättar en CSP-återförsäljarrelation med kunder. Delegerade administratörsbehörigheter ger CSP-partner åtkomst till sina kunders klienter, vilket gör att de kan utföra administrativa funktioner som att lägga till/hantera användare, återställa lösenord och hantera användarlicenser.

**Administratörsbehörighet på prenumerationsnivå** – CSP-partner får dessa behörigheter när de skapar Azure CSP prenumerationer för sina kunder. Med dessa behörigheter får CSP-partner fullständig åtkomst till dessa prenumerationer, vilket gör att de kan etablera och hantera Azure-resurser.

## <a name="reinstate-csp-partners-admin-privileges"></a>Återställa CSP-partners administratörsbehörigheter

Kunden kan skapa CSP-rolltilldelningen på nytt så länge du anger objekt-ID:t för gruppen AdminAgents till kunden. Om du vill återfå delegerade administratörsbehörigheter måste du arbeta med kunden.

1. Logga in på instrumentpanelen i Partnercenter och välj Kunder i **Partnercenter-menyn.**

2. Välj den kund som du arbetar med och **begär en återförsäljarrelation.** Den här åtgärden genererar en länk till kunden som har administratörsrättigheter för klientorganisationen.

3. Kunden måste välja länken och godkänna begäran om återförsäljarrelation.

   :::image type="content" source="images/azure/revoke4.png" alt-text="E-postexempel för att skapa återförsäljarrelation":::

4. Du, partnern, måste ansluta till partnerklientorganisationen för att hämta objekt-ID för gruppen AdminAgents.

  
    ```powershell

    PS C:\WINDOWS\system32> Connect-AzAccount -Tenant "Partner tenant"
      Get Object ID of AdminAgents group
   
    

   S C:\WINDOWS\system32> Get-AzADGroup -DisplayName AdminAgents
    ```


5. Kunden som har rollen ägare eller administratör **för användaråtkomst** och har behörighet att skapa rolltilldelningar på prenumerationsnivå gör följande:


    1. Ansluter till den klientorganisation där CSP-prenumerationen finns.
      ```powershell
        PS C:\WINDOWS\system32> Connect-AzAccount -TenantID "Customer tenant"
      ```

    2. Ansluter till prenumerationen (gäller endast om användaren har rolltilldelningsbehörigheter över flera prenumerationer i klientorganisationen).
   
         PS C:\WINDOWS\system32> Set-AzContext -SubscriptionID "CSP Subscription ID"'


    3. Skapar rolltilldelningen
    
    ```powershell
      PS C:\WINDOWS\system32> New-AzRoleAssignment -ObjectID "Object ID of the Admin Agents group- needs to be provided by partner" -RoleDefinitionName "Owner" -Scope "/subscriptions/CSP subscription ID"
    ```


Om du vill ge ägarrollen behörighet på resursgruppsnivå eller resursnivå i stället för prenumerationsomfånget kan följande kommandon fungera:


```powershell
Grant owner role at resource group level

   New-AzRoleAssignment -ObjectID "Object ID that you got from step 3" -RoleDefinitionName Owner -Scope "/subscriptions/"SubscriptionID of CSP subscription"/resourceGroups/"Resource group name"

Grant owner role at resource level

   New-AzRoleAssignment -ObjectID <Object ID that you got from step 3> -RoleDefinitionName Owner -Scope "Resource URI"
```


## <a name="next-steps"></a>Nästa steg

- [Hantera prenumerationer och resurser under Azure-planen](azure-plan-manage.md)
