---
title: Återställa administratörs behörighet för Azure CSP
ms.topic: how-to
ms.date: 07/28/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Lär dig hur du kan hjälpa kunder att återställa en partners administratörs behörighet så att partnern kan hjälpa dig att hantera en kunds prenumeration på Azure CSP.
author: dhirajgandhi
ms.author: dhgandhi
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 13fdeb01ecd73dc1a63d174a4ad5cb8e1bdc813a
ms.sourcegitcommit: 455894365fa488368f7572ac72312e84a267ef5e
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 12/10/2020
ms.locfileid: "97011510"
---
# <a name="reinstate-admin-privileges-for-a-customers-azure-csp-subscriptions"></a>Återställa administratörs behörighet för en kunds Azure CSP-prenumeration  

**Tillämpliga roller**

- Global administratör
- Administratörs agent

Som CSP-partner förväntar sig kunderna ofta att du ska hantera sin Azure-användning och deras system. Om du gör det måste du ha administratörs behörighet. Vissa behörigheter beviljas dessa när din åter försäljares relation med kunden har upprättats. Andra beviljas av kunden.

## <a name="admin-privileges-for-azure-in-csp"></a>Administratörs behörighet för Azure i CSP

Det finns två nivåer av administratörs behörighet för Azure i CSP.

**Administratörs behörighet för klient organisation** (**delegerad administratörs behörighet**) – CSP-partner får de här privilegierna när du skapar en CSP-återförsäljares relation med kunder. Detta ger CSP-partner åtkomst till sina kunders klienter, vilket gör att de kan utföra administrativa funktioner, till exempel lägga till/hantera användare, återställa lösen ord och hantera användar licenser.

**Administratörs behörighet på prenumerations nivå** – CSP-partners får de här behörigheterna när de skapar Azure CSP-prenumerationer för sina kunder. Med dessa behörigheter får CSP-partner fullständig åtkomst till dessa prenumerationer, vilket gör att de kan etablera och hantera Azure-resurser.

## <a name="reinstate-csp-partners-admin-privileges"></a>Återställ administratörs behörighet för CSP-partner

Du måste arbeta med din kund för att återställa delegerade administratörs behörigheter.

1. Logga in på instrument panelen för partner Center och välj **kunder** från menyn Partner Center.

2. Välj den kund som du arbetar med och **begär en åter försäljares relation.** Detta genererar en länk till kunden som har administratörs behörighet för innehavare.

3. Användaren måste välja länken och godkänna åter försäljarens Relations förfrågan.

   :::image type="content" source="images/azure/revoke4.png" alt-text="åter försäljarens relation":::

## <a name="adding-the-admin-agents-group-as-an-owner-for-the-azure-csp-subscription"></a>Lägga till gruppen admin agents som ägare för Azure CSP-prenumerationen

Kunden måste lägga till din administratörs agent grupp som ägare av en Azure CSP-prenumeration, en resurs grupp eller en resurs. 

1. Använd antingen PowerShell-konsolen eller PowerShell-integrering (Integrated Scripting Environment). Se till att AzureAD-moduler är installerade.

2. Anslut till din Azure AD-klient.

   ```powershell
   Connect-AzureAD
   ```

3. Hämta ObjectId för grupperna med administratörs agenter.

   ```powershell
   Get-AzureADGroup
   ```
   Följande steg utförs av användaren i kundens företag som har ägar åtkomst till Azure CSP-prenumerationen.

4. Användaren med ägar åtkomst till Azure CSP-prenumerationen loggar in på Azure med sina autentiseringsuppgifter.

   ```powershell
   Connect-AzureRmAccount
   ```

5. Hon kan sedan lägga till din administratörs agent grupp som ägare till CSP: n Azure-prenumeration, resurs grupp eller resurs genom att använda en korrekt resurs-URI i omfattnings parametern. 

    ```powershell
    # Grant owner role at subscription level
    New-AzureRmRoleAssignment -ObjectId <Object Id that you got from step 3> -RoleDefinitionName Owner -Scope "/subscriptions/<SubscriptionId of CSP subscription>"

    # Grant owner role at resource group level
    New-AzureRmRoleAssignment -ObjectId <Object Id that you got from step 3> -RoleDefinitionName Owner -Scope "/subscriptions/<SubscriptionId of CSP subscription>/resourceGroups/<Resource group name>"

    # Grant owner role at resource level
    New-AzureRmRoleAssignment -ObjectId <Object Id that you got from step 3> -RoleDefinitionName Owner -Scope "<Resource Uri>"
    ```

## <a name="next-steps"></a>Nästa steg

[Hantera prenumerationer och resurser under Azure-planen](azure-plan-manage.md)
