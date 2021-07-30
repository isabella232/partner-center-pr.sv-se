---
title: Lägga till klientorganisationer i ditt Partnercenter-konto
ms.topic: article
ms.date: 01/11/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-enroll
description: Lär dig hur du lägger till, konsoliderar eller hanterar flera Azure AD-klienter i ditt Partnercenter-konto och lär dig varför du kanske vill göra det.
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 3917d431cb57a8b7555079e063726da3b1c60fab
ms.sourcegitcommit: ad1af627f5ee6b6e3a70655f90927e932cf4c985
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 07/29/2021
ms.locfileid: "114836854"
---
# <a name="add-and-manage-multiple-tenants-in-your-partner-center-account"></a>Lägga till och hantera flera klienter i ditt Partnercenter-konto


**Lämpliga roller:** Global | Kontoadministratör

Den här artikeln beskriver hur du konsoliderar flera Azure Active Directory-klienter (Azure AD) för ditt företag och sedan lägger till och hanterar dem i ditt Partnercenter-konto. Det finns många skäl att göra det. Till exempel:

- Anta att ditt företag, Contoso, har köpt ett annat företag, Fabrikam. Du vill att de två företagen ska vara åtskilda, men du vill att de nya medarbetarna ska kunna använda Partnercenter. I det här fallet associerar du det nya företagets Azure AD-klientorganisation med ditt globala partnerkonto (PGA). Den här associationen gör det möjligt för användare i båda företagen att arbeta i Partnercenter.

- Om du driver ditt företag med fler än en klientorganisation (till exempel *contoso.com*, *contoso.uk* och *contoso.in*) kan du använda flera klientorganisationen för att gruppera dem i samma datorkonto.

- Om riktlinjerna för sammanslagningar och förvärv kräver att du arbetar med klienter för båda företagen använder du både constoso.com *och* *fabrikam.com* klienter.

- Användare av någon av klienterna måste kunna:
    * Få åtkomst till Partnercenter för utbildning, digitala nedladdningar eller MICROSOFT Certified Professional-association (MCP).
    * Tilldelas Partner Center-roller som Microsoft Partner Network (MPN)-administratör eller incitamentsadministratör.

## <a name="add-an-azure-ad-tenant-to-your-account"></a>Lägga till en Azure AD-klientorganisation till ditt konto

1. Logga in som global administratör på [Microsoft Partner Center.](https://partner.microsoft.com/dashboard)

1. Längst upp till höger **väljer Inställningar** väljer **du Kontoinställningar** och sedan **Klienter.**
 
   :::image type="content" source="images/merge-accounts/multitenantNew.png" alt-text="Skärmbild av knappen Associera i fönstret Azure AD-profil."::: 

1. Välj **Associera** och ange sedan den klientorganisation som du vill associera.

1. Logga in som global administratör till den klientorganisation som du vill associera i prompten och välj sedan **Bekräfta**. 

   :::image type="content" source="images/merge-accounts/multitenantNew2.png" alt-text="Skärmbild av knappen Bekräfta i fönstret Bekräfta ny Azure AD-association."::: 

   När du har bekräftat associationen visas **meddelandet All set** .. Om du vill visa den nyligen tillagda klienten väljer **du Återgå till klientorganisationshantering.** 
 
>[!NOTE]
>Du kan inte associera en klientorganisation med ett konto om den redan är associerad med ett annat Partnercenter-konto.


## <a name="remove-a-tenant-from-your-account"></a>Ta bort en klientorganisation från ditt konto
 
1. Logga in som global administratör på [Microsoft Partner Center.](https://partner.microsoft.com/dashboard)

1. Längst upp till höger väljer du **Inställningar** och sedan **Kontoinställningar.**

1. I den vänstra rutan väljer **du Klienter.** Under **Hantera Azure AD-klienter** väljer du **fliken** Partner.
 
1. Välj **Ta** bort bredvid den klientorganisation vars association du vill ta bort.

   :::image type="content" source="images/disassociate.png" alt-text="Skärmbild av de aktuella klientorganisationsassociationer och deras Ta bort-länkar.":::

   Som du ser i föregående  skärmbild är länkarna Ta bort aktiverade för alla associerade klienter, förutom för den primära klienten och den klientorganisation som du är inloggad på. 

   > [!NOTE]   
   > När du tar bort en klientorganisation har användarna i den klientorganisationen inte längre åtkomst till Partnercenter-kontot och borttagningen kan påverka dina kompetenser. 

## <a name="next-steps"></a>Nästa steg

- [Skapa användarkonton](create-user-accounts-and-set-permissions.md)






