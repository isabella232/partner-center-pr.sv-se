---
title: Det går inte att logga in på Partnercenter
ms.topic: troubleshooting
ms.date: 04/08/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-account
description: Felsök möjliga orsaker och lär dig mer om lösningar för när du inte kan logga in på Partnercenter – läs mer om att återställa lösenord, kontrollera roller och kontrollera autentiseringsuppgifter.
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: d084cbf4def33074cc0ca1aae556004cf67bf555
ms.sourcegitcommit: 1161d5bcb345e368348c535a7211f0d353c5a471
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/09/2021
ms.locfileid: "123960876"
---
# <a name="troubleshoot-sign-in-issues-for-partner-center"></a>Felsöka inloggningsproblem för Partnercenter

**Lämpliga roller:** Alla partner som är intresserade av Partnercenter

Den här artikeln innehåller lösningar på vanliga inloggningsproblem för Partnercenter.

## <a name="youve-forgotten-your-password-for-partner-center"></a>Du har glömt lösenordet för Partnercenter

Kontakta supporten om du har glömt ditt lösenord och inte kan logga in på Partnercenter. Du hittar lämplig kontakt på [Support för företagsprodukter.](/microsoft-365/admin/contact-support-for-business-products)

Om du är partner Microsoft Partner Network (MPN) ber du din globala administratör att skapa ett nytt lösenord åt dig. Om du är en indirekt återförsäljare Molnlösningsleverantör (CSP) ber du din indirekta leverantör att skapa en ny global administratör åt dig i din Azure Active Directory-klientorganisation (AD) eller skapa ett nytt lösenord för dig med hjälp av deras delegerade administratörsbehörigheter.

Mer information om hur du kan återställa lösenordet och återfå åtkomsten till ditt arbetskonto finns i Återställa ditt arbets- eller [skollösenord med hjälp av säkerhetsinformation.](/azure/active-directory/user-help/active-directory-passwords-update-your-own-password#how-to-change-your-password)

## <a name="you-cant-view-or-manage-the-expected-pages-or-capabilities-in-partner-center"></a>Du kan inte visa eller hantera förväntade sidor eller funktioner i Partnercenter

Åtkomsten till sidor i Partnercenter styrs av de roller som du har tilldelats. Om du vill kontrollera vilka roller du har tilldelats väljer du ikonen Inställningar Partnercenter, väljer Kontoinställningar och sedan Användarhantering i **Kontoinställningar.** I Sök skriver du ditt namn och visar sedan resultatet.

Om du inte kan visa eller hantera de kompetenser, kunder, incitament eller användare som du förväntar dig kan du prova följande lösningar:

- Kontakta din globala administratör eller kontoadministratör för att få åtkomst till funktionerna i MPN, CSP och referenser. Mer information om roller och de uppgifter som de aktiverar i Partnercenter finns i [Tilldela roller & behörigheter till användare.](permissions-overview.md)
- Om du vill ha åtkomst till funktionerna i Commercial Marketplace och Windows & Xbox, Office Store, Microsoft Edge och Program för maskinvaruutveckling kontaktar du personen i rollen Ägare eller Chef i din organisation. Mer information om roller och behörigheter finns i [Så här hanterar du ett konto på den kommersiella marknadsplatsen i Microsoft Partner Center.](/azure/marketplace/partner-center-portal/manage-account#define-user-roles-and-permissions)

## <a name="you-cant-see-your-offer-or-benefits-in-partner-center"></a>Du kan inte se ditt erbjudande eller dina förmåner i Partnercenter

Bekräfta att du använder rätt autentiseringsuppgifter för att logga in. Till exempel kan dina arbetskonton och personliga konton se likadana ut (till exempel ), men ett kan vara ett personligt konto som du har skapat och ett annat kan vara ett företagskonto som har ställts in för abc@contoso.com din räkning. Om du är inloggad men inte kan visa förväntade funktioner som rör MPN, CSP, Commercial Marketplace kan du i det här fallet prova att välja ditt arbetskonto.

## <a name="next-steps"></a>Nästa steg

- [Verifiera din kontoinformation](verification-responses.md)
- [Återställa mitt lösenord](reset-my-pasword.md)
- [Återställa ett användarlösenord](reset-a-user-password.md)