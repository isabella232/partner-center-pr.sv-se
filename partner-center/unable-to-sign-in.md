---
title: Det går inte att logga in på Partnercenter
ms.topic: troubleshooting
ms.date: 04/08/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Felsök möjliga orsaker och lär dig mer om lösningar för när du inte kan logga in på Partnercenter – läs mer om att återställa lösenord, kontrollera roller och kontrollera autentiseringsuppgifter.
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: f4af8c48e2bbe65f58549b542447c80b699332be
ms.sourcegitcommit: dc9438475ccc6298bec6a698bf5fc9bd5cf2aa81
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 05/12/2021
ms.locfileid: "109818804"
---
# <a name="troubleshoot-sign-in-issues-for-partner-center"></a>Felsöka inloggningsproblem för Partnercenter

**Lämpliga roller:** Alla partner som är intresserade av Partnercenter

Den här artikeln innehåller lösningar på vanliga inloggningsproblem för Partnercenter.

## <a name="youve-forgotten-your-password-for-partner-center"></a>Du har glömt lösenordet för Partnercenter

Kontakta supporten om du har glömt ditt lösenord och inte kan logga in på Partnercenter. Du hittar lämplig kontakt på [Support för företagsprodukter.](/microsoft-365/admin/contact-support-for-business-products)

Om du är MPN-partner kan du be din globala administratör att skapa ett nytt lösenord åt dig. Om du är en indirekt CSP-återförsäljare kan du be din indirekta leverantör att skapa en ny global administratör åt dig i din Azure AD-klient eller skapa ett nytt lösenord åt dig med hjälp av deras delegerade administratörsbehörigheter.

Mer information om hur du återställer ditt lösenord och återfår åtkomsten till ditt arbetskonto finns i Återställa ditt arbets- eller [skollösenord med hjälp av säkerhetsinformation.](/azure/active-directory/user-help/active-directory-passwords-update-your-own-password#how-to-change-your-password)

## <a name="you-cant-view-or-manage-the-expected-pages-or-capabilities-in-partner-center"></a>Du kan inte visa eller hantera förväntade sidor eller funktioner i Partnercenter

Åtkomsten till sidor i Partnercenter styrs av de roller som du har tilldelats. Kontrollera vilka roller du har tilldelats genom att i Partnercenter välja ikonen Inställningar, välja Kontoinställningar och sedan Användarhantering i **Kontoinställningar.** I Sök skriver du ditt namn och visar sedan resultatet.

Om du inte kan visa eller hantera kompetenser, kunder, incitament eller användare som du förväntar dig kan du prova följande lösningar:

- Kontakta din globala administratör eller kontoadministratör för att få åtkomst till funktionerna i MPN, CSP och referenser. Mer information om roller och de aktiviteter som de aktiverar i Partnercenter finns i [Tilldela roller & behörigheter till användare.](permissions-overview.md)
- Om du vill ha åtkomst till funktionerna i Den kommersiella marknadsplatsen och Windows & Xbox, Office Store, Microsoft Edge och maskinvaruutvecklingsprogram kontaktar du personen i rollen Ägare eller Ansvarig i din organisation. Mer information om roller och behörigheter finns i [Hantera ett konto på den kommersiella marknadsplatsen i Microsoft Partner Center.](/azure/marketplace/partner-center-portal/manage-account#define-user-roles-and-permissions)

## <a name="you-cant-see-your-offer-or-benefits-in-partner-center"></a>Du kan inte se ditt erbjudande eller dina förmåner i Partnercenter

Bekräfta att du använder rätt autentiseringsuppgifter för att logga in. Till exempel kan dina arbetskonton och personliga konton se likadana ut (till exempel ), men ett kan vara ett personligt konto som du har skapat och ett annat kan vara ett företagskonto som har ställts in för abc@contoso.com din räkning. Om du är inloggad men inte kan visa förväntade funktioner som rör MPN, CSP eller Kommersiell marknadsplats kan du i det här fallet prova att välja ditt arbetskonto.

## <a name="next-steps"></a>Nästa steg

- [Verifiera din kontoinformation](verification-responses.md)
- [Återställa mitt lösenord](reset-my-pasword.md)
- [Återställa ett användarlösenord](reset-a-user-password.md)