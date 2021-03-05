---
title: Lägga till klienter till ditt partner Center-konto
ms.topic: article
ms.date: 01/11/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Lär dig hur du lägger till, konsoliderar eller hanterar flera Azure AD-klienter i ditt partner Center-konto och lär dig varför du kanske vill göra det.
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 2f3094489f65b7164b4a55804047f9a4ab5f11cb
ms.sourcegitcommit: 79d2f00c352db61252e523f45abf93fe2a2742a5
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/04/2021
ms.locfileid: "102124813"
---
# <a name="add-and-manage-multiple-tenants-in-your-partner-center-account"></a>Lägga till och hantera flera klienter i ditt partner Center-konto


**Lämpliga roller**

- Global administratör
- Kontoadministratör

Den här artikeln beskriver hur du konsoliderar flera Azure Active Directory (Azure AD)-klienter för företaget och sedan lägger till och hanterar dem i ditt partner Center-konto. Det finns många skäl att göra det. Exempel:

- Låt oss säga att ditt företag, contoso, har förvärvat ett annat företag, Fabrikam. Du vill att de två företagen ska vara åtskilda, men du vill att de nya anställda ska kunna använda Partner Center. I det här fallet associerar du det nya företagets Azure AD-klient med ditt partner globala konto (PGA). Den här kopplingen gör det möjligt för användare i båda företagen att arbeta i Partner Center.

- Om du kör din verksamhet med fler än en klient (till exempel *contoso.com*, *contoso.uk* och *contoso.in*) kan du använda flera innehavare för att gruppera dem i samma PC-konto.

- Om rikt linjerna för sammanslagning och förvärv kräver att du arbetar med klienter för båda företagen, använder du både *constoso.com* -och *fabrikam.com* -klienterna.

- Användare av någon av klienterna måste kunna:
    * Få åtkomst till Partner Center för utbildning, digital hämtning eller Microsoft Certified Professional (MCP)-Association.
    * Tilldelas Partner Center-roller som Microsoft Partner Network (MPN) admin eller incitaments administratör.

## <a name="add-an-azure-ad-tenant-to-your-account"></a>Lägg till en Azure AD-klient i ditt konto

1. Logga in som global administratör till [Microsoft Partner Center](https://partner.microsoft.com/dashboard).

1. I det övre högra hörnet väljer du **Inställningar**, sedan **konto inställningar** och väljer sedan **klienter**.
 
   :::image type="content" source="images/merge-accounts/multitenantNew.png" alt-text="Skärm bild av knappen associera i fönstret Azure AD-profil."::: 

1. Välj **associera** och ange den klient som du vill associera.

1. Vid prompten loggar du in som global administratör till den klient som du vill associera och väljer sedan **Bekräfta**. 

   :::image type="content" source="images/merge-accounts/multitenantNew2.png" alt-text="Skärm bild av knappen Bekräfta i fönstret Bekräfta nytt Azure AD-Association."::: 

   När du har bekräftat associationen visas ett meddelande om att **alla anges** . Om du vill visa den nyligen tillagda klienten väljer du **återgå till klient organisations hantering**. 
 
>[!NOTE]
>Du kan inte associera en klient med ett konto om det redan är kopplat till ett annat Partner Center-konto.


## <a name="remove-a-tenant-from-your-account"></a>Ta bort en klient från ditt konto
 
1. Logga in som global administratör till [Microsoft Partner Center](https://partner.microsoft.com/dashboard).

1. Klicka på ikonen **Inställningar** längst upp till höger och välj sedan **konto inställningar**.

1. Välj **innehavare** i det vänstra fönstret. Under **Hantera Azure AD-klienter** väljer du fliken **partner** .
 
1. Välj **ta bort** bredvid den klient vars Association du vill ta bort.

   :::image type="content" source="images/disassociate.png" alt-text="Skärm bild av de aktuella klient kopplingarna och deras borttagnings länkar.":::

   Som du ser i föregående skärm bild är **ta bort** länkar aktiverade för alla associerade klienter, förutom den primära klienten och klienten som du för närvarande är inloggad på. 

   > [!NOTE]   
   > När du tar bort en klient har användarna på den innehavaren inte längre åtkomst till Partner Center-kontot, och borttagningen kan påverka din kompetens. 

## <a name="next-steps"></a>Nästa steg

- [Skapa användarkonton](create-user-accounts-and-set-permissions.md)






