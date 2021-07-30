---
title: Det går inte att logga in på Partnercenter
ms.topic: troubleshooting
ms.date: 04/08/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-enroll
description: Felsök möjliga orsaker och lär dig mer om lösningar för när du inte kan logga in på Partnercenter – läs mer om att återställa lösenord, kontrollera roller och kontrollera autentiseringsuppgifter.
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: d0a4583aa7b3ec6f51066dfa2c3dedcbcc18eb35
ms.sourcegitcommit: ad1af627f5ee6b6e3a70655f90927e932cf4c985
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 07/29/2021
ms.locfileid: "114836650"
---
# <a name="troubleshoot-sign-in-issues-for-partner-center"></a>Felsöka inloggningsproblem för Partnercenter

**Lämpliga roller:** Alla partner som är intresserade av Partnercenter

Den här artikeln innehåller lösningar på vanliga inloggningsproblem för Partnercenter.

## <a name="youve-forgotten-your-password-for-partner-center"></a>Du har glömt ditt lösenord för Partnercenter

Kontakta supporten om du har glömt ditt lösenord och inte kan logga in på Partnercenter. Du hittar lämplig kontakt på [Support för företagsprodukter.](/microsoft-365/admin/contact-support-for-business-products)

Om du är en partner Microsoft Partner Network (MPN) ber du din globala administratör att skapa ett nytt lösenord åt dig. Om du är en indirekt Molnlösningsleverantör-återförsäljare (CSP) ber du din indirekta leverantör att skapa en ny global administratör åt dig på din Azure Active Directory-klient (AD) eller skapa ett nytt lösenord för dig med hjälp av deras delegerade administratörsbehörigheter.

Mer information om hur du kan återställa lösenordet och återfå åtkomsten till ditt arbetskonto finns i Återställa ditt arbets- eller [skollösenord med hjälp av säkerhetsinformation.](/azure/active-directory/user-help/active-directory-passwords-update-your-own-password#how-to-change-your-password)

## <a name="you-cant-view-or-manage-the-expected-pages-or-capabilities-in-partner-center"></a>Du kan inte visa eller hantera förväntade sidor eller funktioner i Partnercenter

Åtkomsten till sidor i Partnercenter styrs av de roller som du har tilldelats. Du kan kontrollera vilka roller du har tilldelats genom att Inställningar i Partnercenter, välja Kontoinställningar och sedan Användarhantering i **Kontoinställningar.** I Sök skriver du ditt namn och visar sedan resultatet.

Om du inte kan visa eller hantera de kompetenser, kunder, incitament eller användare som du förväntar dig kan du prova följande lösningar:

- Kontakta din globala administratör eller kontoadministratör för att få åtkomst till funktionerna i MPN, CSP och referenser. Mer information om roller och de uppgifter som de aktiverar i Partnercenter finns i [Tilldela roller & behörigheter till användare](permissions-overview.md).
- Om du vill ha åtkomst till funktionerna i Den kommersiella marknadsplatsen och programmen för Windows & Xbox, Office Store, Microsoft Edge och maskinvaruutvecklare kontaktar du personen i rollen Ägare eller Ansvarig i din organisation. Mer information om roller och behörigheter finns i [Hantera ett konto på den kommersiella marknadsplatsen i Microsoft Partner Center.](/azure/marketplace/partner-center-portal/manage-account#define-user-roles-and-permissions)

## <a name="you-cant-see-your-offer-or-benefits-in-partner-center"></a>Du kan inte se ditt erbjudande eller dina förmåner i Partnercenter

Bekräfta att du använder rätt autentiseringsuppgifter för att logga in. Dina arbetskonton och personliga konton kan till exempel se likadana ut (till exempel ), men ett kan vara ett personligt konto som du har skapat och ett annat kan vara ett företagskonto som har ställts in för abc@contoso.com din räkning. Om du är inloggad men inte kan visa förväntade funktioner som rör MPN, CSP eller Kommersiell marknadsplats kan du i det här fallet prova att välja ditt arbetskonto.

## <a name="next-steps"></a>Nästa steg

- [Verifiera din kontoinformation](verification-responses.md)
- [Återställa mitt lösenord](reset-my-pasword.md)
- [Återställa ett användarlösenord](reset-a-user-password.md)