---
title: Det går inte att logga in på Partner Center
ms.topic: troubleshooting
ms.date: 04/08/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Felsök möjliga orsaker och lär dig mer om lösningar när du inte kan logga in på Partner Center – Läs mer om hur du återställer lösen ord, kontrollerar roller och kontrollerar autentiseringsuppgifter.
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 17087727afcaf3dbcf47801f8668388c370758e7
ms.sourcegitcommit: 9b04509f3830462628c1bb6af2ca41ed68b52619
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/09/2021
ms.locfileid: "107266579"
---
# <a name="troubleshoot-sign-in-issues-for-partner-center"></a>Felsöka inloggnings problem för partner Center

**Lämpliga roller**

- Alla partner som är intresserade av Partner Center

Den här artikeln innehåller lösningar för vanliga inloggnings problem för partner Center.

## <a name="youve-forgotten-your-password-for-partner-center"></a>Du har glömt ditt lösen ord för partner Center

Kontakta supporten om du har glömt ditt lösen ord och inte kan logga in på Partner Center. Hitta lämplig kontakt vid [Support för företags produkter](/microsoft-365/admin/contact-support-for-business-products).

Om du är en MPN-partner kan du be din globala administratör att skapa ett nytt lösen ord åt dig. Om du är en CSP-indirekt åter försäljare ber du din indirekta Provider att skapa en ny global administratör för dig på din Azure AD-klient eller skapa ett nytt lösen ord för dig med hjälp av deras delegerade administratörs behörighet.

Läs mer om hur du kan återställa ditt lösen ord och få åtkomst till ditt arbets konto genom att läsa [återställa ditt arbets-eller skol lösen ord med hjälp av säkerhets information](/azure/active-directory/user-help/active-directory-passwords-update-your-own-password#how-to-change-your-password).

## <a name="you-cant-view-or-manage-the-expected-pages-or-capabilities-in-partner-center"></a>Du kan inte Visa eller hantera förväntade sidor eller funktioner i Partner Center

Åtkomst till sidor i Partner Center styrs av de roller som du har tilldelat. Om du vill kontrol lera vilka roller som du har tilldelat väljer du ikonen Inställningar i Partner Center, väljer **konto inställningar** och väljer sedan **användar hantering** i konto inställningar. I Sök skriver du ditt namn och visar resultatet.

Om du inte kan visa eller hantera de kompetenser, kunder, incitament eller användare som du förväntar dig, kan du prova följande lösningar:

- Kontakta din globala administratör eller konto administratör om du vill ha åtkomst till funktionerna i MPN, CSP och referenser. Mer information om roller och de uppgifter som de aktiverar i Partner Center finns i [tilldela roller & behörigheter till användare](permissions-overview.md).
- Om du vill ha till gång till funktionerna i affärs marknads platsen och Windows & Xbox, Office Store, Microsoft Edge och program vara för utvecklare kontaktar du personen i ägaren eller chefs rollen i din organisation. Mer information om roller och behörigheter finns i [hantera ett kommersiellt marknads plats konto i Microsoft Partner Center](/azure/marketplace/partner-center-portal/manage-account#define-user-roles-and-permissions).

## <a name="you-cant-see-your-offer-or-benefits-in-partner-center"></a>Du kan inte se ditt erbjudande eller dina förmåner i Partner Center

Bekräfta att du använder rätt autentiseringsuppgifter för att logga in. Dina arbets-och personliga konton kan till exempel se likadant ut (till exempel abc@contoso.com ), men det kan vara ett personligt konto som du har skapat och ett annat kan vara ett företags konto som har kon figurer ATS för din räkning. I det här fallet, om du är inloggad, men inte kan visa förväntade funktioner relaterade till MPN, CSP, kommersiella marknads platser, kan du försöka välja ditt arbets konto.

## <a name="next-steps"></a>Nästa steg

- [Verifiera din kontoinformation](verification-responses.md)
- [Återställa mitt lösenord](reset-my-pasword.md)
- [Återställa ett användarlösenord](reset-a-user-password.md)