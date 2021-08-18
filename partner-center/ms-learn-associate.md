---
title: Länka Microsoft Learn MCP-ID till Partnercenter-konto
ms.topic: how-to
ms.date: 08/03/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-membership
description: Lär dig hur du associerar ditt MCP-ID till ditt Partnercenter-konto så att ditt företag kan se utbildningsvägarna som du har tagit mot kompetenser.
author: kbangalore
ms.author: kiranban
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: d78009e66f8a12779e96d08a16a2877a6e88fc5d
ms.sourcegitcommit: 815760499700bf2c947550524cbddd091622081f
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/13/2021
ms.locfileid: "121915412"
---
# <a name="link-or-unlink-a-microsoft-certification-profile-id-mcid-to-a-microsoft-partner-network-mpn-account"></a>Länka eller avlänka ett Microsoft-certifikatprofil-ID (MCID) till Microsoft Partner Network (MPN)-konto

**Lämpliga roller:** Alla Partner Center-användare

Den här artikeln beskriver hur kunder som har aktiva certifieringar i Microsofts certifieringsprogram kan länka eller avlänka sitt Microsoft-certifieringsprofil-ID (MCID) med en Microsoft Partner Network-organisation (MPN).

Du måste vara MPN-partneradministratör eller global administratör för att kunna granska kompetensstatus [(inloggning](https://partner.microsoft.com/pcv/partnership/competencies) krävs) för prov eller för att ladda ned kunskapsrapporter för att granska associerade prov. Partnerorganisationen uppfyller kompetenskraven genom att ha personer med länkade MCID:er som är kopplade till organisationen. Ett MCID kan bara länkas till ett enda MPN-medlemskap i taget.

## <a name="get-partner-university-access"></a>Få åtkomst till Partner University

För att kunna associera din Microsoft-certifiering måste du ha ett Partnercenter-konto (Active AD) associerat med din partnerorganisation. Medlemmar i MPN-partnerorganisationer bör använda sitt mpn-partnerorganisations användarnamn och lösenord (arbetskonto) för att logga in på Partnercenter.
Använd proceduren nedan för att få åtkomst till Partner University.

1. Logga in på [instrumentpanelen i Partnercenter](https://partner.microsoft.com/dashboard/).
2. Välj den blå **ikonen Min** profil i det övre högra hörnet
3. I fältet **Learning** väljer du **Get Partner University Access (Hämta åtkomst till Partner University).** Du måste ange autentiseringsuppgifterna för ditt Partner University-konto (inte ditt Partnercenter-konto) Ditt Partner University-konto kommer nu att associeras med ditt Partnercenter-användarkonto. Dina utvärderingar visas i partnercentrets användarkunskapsrapport inom 72 timmar.
4. Om du vill ta bort associationen väljer du **Ta bort åtkomst.**

## <a name="associate-a-microsoft-learning-account"></a>Associera ett Microsoft Learning konto

Använd följande procedur för att associera ett Microsoft Learning konto. 

1. Logga in på [instrumentpanelen i Partnercenter](https://partner.microsoft.com/dashboard/).
2. På din profilsida rullar du ned till **fältet Microsoft-prov** och certifieringar och väljer **Associera Microsoft Learning konto.**
3. När du uppmanas till det anger du de autentiseringsuppgifter som du använder för att logga in på din Microsoft-certifieringsprofil (din MCID).

>[!NOTE]
>Om Microsoft Learning-kontoautentiseringsuppgifterna är samma som autentiseringsuppgifterna för Partner University-kontot väljer du Använd för att associera **email@address mitt Microsoft Learning konto.**

## <a name="download-skills-report-microsoft-certification-list"></a>Ladda ned kunskapsrapport (Microsoft-certifieringslista)
Om du behöver information kan kunskapsrapporten nås och laddas ned av valfri global administratör eller MPN-partneradministratör från Partnercenter. Mer information finns [i](./mpn-skills-report.md#view-skills-report-data).


## <a name="frequently-asked-questions-about-linking-accounts"></a>Vanliga frågor och svar om att länka konton

### <a name="how-can-a-user-link-their-microsoft-certification-profile-id-mcid-with-the-microsoft-partner-network-mpn-organization-they-work-for"></a>Hur kan en användare länka sitt Microsoft-certifieringsprofil-ID (MCID) till den Microsoft Partner Network (MPN)-organisation som de arbetar för?

Användarna bör logga in på Partnercenter och gå **till Min profil** och sedan välja Skaffa **Partner University-konto** eller Associera Ett **Microsoft Learning konto** och ange sina autentiseringsuppgifter. För att associera till ett Microsoft Learning-konto måste användaren ange det användarnamn och lösenord som används för att logga in på sin Microsoft-certifieringsprofil (MCID). På grund av sekretessöverväganden måste användarna själva slutföra kontolänkningsprocessen.  

### <a name="how-can-a-user-unlink-their-mcid-from-the-mpn-organization-they-work-for"></a>Hur kan en användare avlänka sin MCID från den MPN-organisation som de arbetar för?

Logga in på Partnercenter, gå till **Min profil och** välj sedan Ta bort **åtkomst.** På grund av sekretessöverväganden måste användaren själva slutföra kontolänkningsprocessen.

### <a name="the-user-left-company-a-and-now-works-for-company-b-how-can-they-link-their-microsoft-certification-profile-id-mcid-with-company-b"></a>Användaren har lämnat Företag A och arbetar nu för Företag B. Hur kan de länka sitt Microsoft-certifieringsprofil-ID (MCID) till företag B?

Användaren måste länka sin MCID till företag B genom att följa proceduren ovan. När användaren länkar sin MCID till företag B tas de automatiskt bort från företag A.

### <a name="the-user-left-company-a-and-no-longer-has-access-to-partner-center-they-want-to-unlink-their-mcid-from-company-a-and-are-not-planning-to-link-it-with-another-mpn-organization-at-the-moment"></a>Användaren har lämnat Företag A och har inte längre åtkomst till Partnercenter. De vill avlänka sin MCID från företag A och planerar inte att länka den till en annan MPN-organisation för tillfället.

Användarens konto måste tas bort av den globala administratören när han eller hon lämnar företaget. Om användarens MCID fortfarande visas som länkad till företaget i kunskapsrapporten måste användaren begära att den globala administratören tar bort dem från rapporten.

### <a name="the-admin-provided-sign-in-details-for-a-work-email-account-to-a-user-and-they-have-had-no-response"></a>Administratören angav inloggningsinformation för ett arbets-e-postkonto till en användare och de har inte fått något svar.

Administratören bör först verifiera den e-postadress som användes och sedan kontakta användaren som kontoinformationen har angetts till.

### <a name="a-user-tries-to-associate-their-mcp-learning-account-to-their-profile-in-partner-center-and-receives-a-message-that-their-association-is-limited-for-example-you-have-attempted-to-associate-with-a-partner-organization-however-we-require-a-period-of-30-days-between-associations-your-next-available-date-for-a-subsequent-association-is-xxx"></a>En användare försöker associera sitt MCP Learning konto till sin profil i Partnercenter och får ett meddelande om att deras association är begränsad. Till exempel "Du har försökt associera med en partnerorganisation. Vi kräver dock en period på 30 dagar mellan associationer. Ditt nästa tillgängliga datum för en efterföljande association är XXX"

För att skydda mot missbruk har en MCP-individ ett begränsat antal 3 associationer som tillåts varje år och det finns en nedspolningsperiod på 30 dagar mellan varje association som börjar i början av associationen. Varje användare kan kontrollera datumet i sin profil för att se när de kan starta en ny association. Om användaren har problem med att associera efter det datumet bör de kontakta supporten.  

## <a name="how-to-get-support"></a>Hur du kan få support

För tekniska problem med länkning eller avlänkning av MCID:er med MPN-partnerorganisationer som inte behandlas i vanliga frågor och svar kan du öppna ett ärende hos Microsoft [Support.](https://partner.microsoft.com/support)

Om du har frågor om sammanslagningsprocessen för Microsoft-certifieringsprofiler (MCID) kontaktar du [Certifieringssupport.](https://aka.ms/mcpforum)

## <a name="next-steps"></a>Nästa steg

- [Användarroller och behörigheter](./permissions-overview.md)
- [Kompetenser](https://partner.microsoft.com/membership/competencies)
- [Rapporten Microsoft Learn analys visar status för elever i ditt företag](ms-learn-analytics.md)
