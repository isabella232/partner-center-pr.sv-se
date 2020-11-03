---
title: Lägg till ytterligare klienter till ditt partner Center-konto
ms.topic: article
ms.date: 07/30/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Lär dig hur du lägger till, konsoliderar eller hanterar flera Azure AD-klienter i ditt partner Center-konto. Lär dig också om några av de orsaker du kanske vill göra det.
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: b9379ce6b27a8ef6e5d6894a0630745794e04e04
ms.sourcegitcommit: 3c45a181ef86b3a4866e97fb50efeae8714ab3f7
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 10/19/2020
ms.locfileid: "92532028"
---
# <a name="add-and-manage-multiple-tenants-in-your-partner-center-account"></a>Lägga till och hantera flera klienter i ditt partner Center-konto

**Gäller för**

- Partnercenter

**Lämpliga roller**

- Global administratör

Med den här funktionen kan du hantera flera klientorganisationer i ditt företag och konsolidera dem till ditt Partner Center-konto. Det finns många orsaker till varför du kan behöva hantera flera Azure AD-klienter i ditt partner Center-konto. Exempel:

- Företaget kan köpa ett annat företag och du vill att de anställda i det nya företaget ska kunna använda Partner Center. Men du vill att de två företagen ska vara åtskilda. I det här fallet associerar du det nya företagets Azure AD-klient med ditt partner globala konto (PGA). Den här kopplingen gör det möjligt för användare i båda företagen att arbeta i Partner Center.

- Om du har fler än en klient för att köra företaget (t. ex. contoso.com, contoso.uk, contoso.in) kan du använda flera innehavare för att koppla ihop dem under samma PC-konto.

- Sammanslagningar och förvärv kräver att du arbetar med fler än en klient (t. ex. om contoso förvärvar Fabrikam måste du kunna använda både Constoso.com och Fabrikam.com respektive klienter).

- Användare från någon av klient organisationerna måste kunna:
    1.  Åtkomst till Partner Center för utbildning, digital hämtning, MCP-Association
    2.  Tilldelas Partner Center-roller som MPN-administratör, incitaments administratör osv.


## <a name="add-another-azure-ad-tenant-to-your-account"></a>Lägg till en annan Azure AD-klient i ditt konto

1. Logga in på [instrument panelen](https://partner.microsoft.com/dashboard)för partner Center som global administratör.
1. Från **inställnings** ikonen väljer du **konto inställningar** och väljer sedan **klienter** .
 
:::image type="content" source="images/merge-accounts/multitenantNew.png" alt-text="koppla klienter"::: 

3. Välj **associera en annan AD-klient** och ange den klient som du vill koppla.

1. Logga in på den klient som du vill associera och bekräfta associationen som global administratör. 

:::image type="content" source="images/merge-accounts/multitenantNew2.png" alt-text="koppla klienter"::: 

5. När **du har bekräftat visas ett meddelande** om detta.  Välj **återgå till klient organisations hantering** så visas den nyligen tillagda klienten i listan. 
 

>[!NOTE]
>Du kan inte koppla en klient till ett konto om det redan är kopplat till ett annat Partner Center-konto.

 
## <a name="next-steps"></a>Nästa steg

- [Lägg till användare](create-user-accounts-and-set-permissions.md)
