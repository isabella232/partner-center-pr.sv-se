---
title: Återställa administratörs behörighet för Azure CSP
ms.topic: how-to
ms.date: 04/08/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Lär dig hur du kan hjälpa kunder att återställa en partners administratörs behörighet så att partnern kan hjälpa dig att hantera en kunds prenumeration på Azure CSP.
author: dhirajgandhi
ms.author: dhgandhi
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: f536d975d3c644a7afa29a95a3cb45608f6b2c9f
ms.sourcegitcommit: 89be77c9f35c77463d9558826293202afc6dec56
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/13/2021
ms.locfileid: "107315855"
---
# <a name="reinstate-admin-privileges-for-a-customers-azure-csp-subscriptions"></a>Återställa administratörs behörighet för en kunds Azure CSP-prenumeration  

**Tillämpliga roller**

- Global administratör
- Administratörs agent

Som CSP-partner förväntar sig kunderna ofta att du ska hantera sin Azure-användning och deras system. Om du gör det måste du ha administratörs behörighet. Vissa behörigheter beviljas när din åter försäljares relation med kunden har upprättats. Andra beviljas av kunden.

## <a name="admin-privileges-for-azure-in-csp"></a>Administratörs behörighet för Azure i CSP

Det finns två nivåer av administratörs behörighet för Azure i CSP.

**Administratörs behörighet för klient organisation** (**delegerad administratörs behörighet**) – CSP-partner får de här privilegierna när du skapar en CSP-återförsäljares relation med kunder. Delegerade administratörs privilegier ger CSP-partner åtkomst till sina kunders klienter, vilket gör att de kan utföra administrativa funktioner, till exempel lägga till/hantera användare, återställa lösen ord och hantera användar licenser.

**Administratörs behörighet på prenumerations nivå** – CSP-partners får de här behörigheterna när de skapar Azure CSP-prenumerationer för sina kunder. Med dessa behörigheter får CSP-partner fullständig åtkomst till dessa prenumerationer, vilket gör att de kan etablera och hantera Azure-resurser.

## <a name="reinstate-csp-partners-admin-privileges"></a>Återställ administratörs behörighet för CSP-partner

Kunden kan återskapa CSP-rollens tilldelning så länge du anger objekt-ID: t för AdminAgents-gruppen till din kund. Du måste arbeta med din kund för att återställa delegerade administratörs behörigheter.

1. Logga in på Partner Center-instrumentpanelen och välj **kunder** från menyn Partner Center.

2. Välj den kund som du arbetar med och **begär en åter försäljares relation.** Detta genererar en länk till kunden som har administratörs behörighet för innehavare.

3. Kunden måste välja länken och godkänna åter försäljarens Relations förfrågan.

   :::image type="content" source="images/azure/revoke4.png" alt-text="E-postexempel för skapa åter försäljarens relation":::

4. Du, partnern, måste ansluta till partner klienten för att hämta objekt-ID för AdminAgents-gruppen.

  
    ```powershell

    PS C:\WINDOWS\system32> Connect-AzAccount -Tenant "Partner tenant"
      Get Object ID of AdminAgents group
   
    

   S C:\WINDOWS\system32> Get-AzADGroup -DisplayName AdminAgents
    ```


5. Din kund som har rollen **ägare eller administratör för användar åtkomst** och har behörighet att skapa roll tilldelning på prenumerations nivån gör följande:


    1. Ansluter till den klient där CSP-prenumerationen finns.
      ```powershell
        PS C:\WINDOWS\system32> Connect-AzAccount -TenantID "Customer tenant"
      ```

    2. Ansluter till prenumerationen (endast tillämpligt om användaren har roll tilldelnings behörigheter över flera prenumerationer i klienten).
   
         PS C:\WINDOWS\system32> Set-AzContext-SubscriptionID prenumerations-ID för CSP ""


    3. Skapar roll tilldelningen
    
    ```powershell
      PS C:\WINDOWS\system32> New-AzRoleAssignment -ObjectID "Object ID of the Admin Agents group- needs to be provided by partner" -RoleDefinitionName "Owner" -Scope "/subscriptions/CSP subscription ID"
    ```


Om du vill ge ägar rollen behörighet på resurs grupps nivå eller resurs nivå i stället för prenumerations omfånget kan följande kommandon fungera:


```powershell
Grant owner role at resource group level

   New-AzRoleAssignment -ObjectID "Object ID that you got from step 3" -RoleDefinitionName Owner -Scope "/subscriptions/"SubscriptionID of CSP subscription"/resourceGroups/"Resource group name"

Grant owner role at resource level

   New-AzRoleAssignment -ObjectID <Object ID that you got from step 3> -RoleDefinitionName Owner -Scope "Resource URI"
```


## <a name="next-steps"></a>Nästa steg

- [Hantera prenumerationer och resurser under Azure-planen](azure-plan-manage.md)
