---
title: Tilldela roller & behörigheter till användare
ms.topic: article
ms.date: 10/30/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Lär dig vilka roller som passar bäst för ditt företags användare som hanterar affärs transaktioner, referenser, incitament eller MPN-medlemskap i Partner Center.
author: hemas
ms.author: hemas
ms.localizationpriority: high
ms.custom: SEOMAY.20, contperfq1
ms.openlocfilehash: 8ae4bed8536907c59f1b22e72896cfbe7f7aff9a
ms.sourcegitcommit: 445c7b70943f71cc4b2cb48a327b9dcc1814974d
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 11/17/2020
ms.locfileid: "94670158"
---
# <a name="assign-users-roles-and-permissions-for-a-companys-users-needing-to-work-in-partner-center"></a>Tilldela användare roller och behörigheter för ett företags användare som behöver arbeta i Partner Center

**Lämpliga roller**

- Global administratör
- Användaradministratör
- MPN-partner administratör

Du har konfigurerat din partner profil, inklusive juridiskt namn och adress, support information, fil skatte undantag, bank information och den primära kontakten för ditt företag. Nästa steg: få dina användare att konfigureras med lösen ord och roller så att de kan börja arbeta i Partner Center med dig.

## <a name="set-up-your-employees-to-work-in-partner-center"></a>Konfigurera dina anställda så att de arbetar i Partner Center

Du bestämmer vilka typer av åtkomst användarna har till Partner Center av de roller och behörigheter som du ger dem. Rollerna är relaterade till de program som din verksamhet är involverad i. Om ditt företag till exempel är en moln lösnings leverantör (CSP), så har du inte bara standard Azure Active Directory klient hanterings roller som global administratör, men behöver roller som är specifika för CSP-programmet. Varje program har roller som är just det.

>[!Note]
> Azure Active Directory klient rollerna är globala administratörer, användar administratör och CSP-roller. Icke-Azure-Active-Directory-roller är de roller som inte hanterar klienten, och de omfattar MPN-administratör, företags profil administratör, hänvisnings administratör, incitaments administratör och stimulans användare. 

### <a name="manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles"></a>Hantera affärs transaktioner i Partner Center (Azure AD och CSP-roller)

|**Role**|**Vad de kan göra**|**Läs mer**|
|----------------------------------|---|:---------------------------------|
|Global administratör|* Kan komma åt alla Microsoft-konto/tjänster med fullständig behörighet|[Hantera ditt Partnercenter-konto](partner-center-account-setup.md)
|      |* Skapa support biljetter för partner Center
||* Visa partner support biljetter som du skapar
||* Visa avtal, pris listor och erbjudanden
||* Visa, skapa och hantera partner användare|
||  Visa, skapa och hantera fakturerings-, fakturor-och rekognoseringar-filer
|Administratör för användar hantering   | * Visa, skapa och hantera användare|[Hantera dina Microsoft Partner Network medlemskaps förmåner och erbjudanden i Partner Center](manage-your-partner-network-benefits.md)
||* Visa alla partner profiler
||* Skapa support biljetter för partner Center
||* Visa partner support biljetter som du skapar
|Faktureringsadministratör | – Visa, skapa och hantera fakturerings-, fakturor-och rekognoseringar-filer|[Läsa fakturan](billing.md)
||* Visa priser
||* Skapa support biljetter för partner Center
||* Visa partner support biljetter som du skapar
|Standard användare|  Visa min profil   |[Återställa lösenordet](reset-my-pasword.md)
|Administratörs agent | * Kund hantering|[Få kontakt med dina kunder](connect-with-your-customers.md)
||* Lägg till enhets lista i partner centret
||* Skapa och tillämpa profiler på enheter
||* Prenumerations hantering
||* Tjänstens hälso-och tjänst begär Anden för kunder
||* Begär delegerad administratörs behörighet
||* Visa priser och erbjudanden
||* Fakturering
||* Administrera för en kunds räkning
||* Registrera ett värde för tillagd åter försäljare
||* Skapa support biljetter för partner Center
||* Visa partner support biljetter som du skapar|
|Försäljnings agent | * Kund hantering|[Ge fakturerings support för dina kunder och hjälp med att besvara sina fakturerings frågor](provide-billing-support.md)
||* Lägg till enhets lista i partner centret
||* Prenumerations hantering
||* Visa support biljetter
||* Begär en relation med en kund
||* Visa priser och erbjudanden
||* Hantera kund ledare
||* Visa kund avtalet
||* Registrera en åter försäljare som har lagts till
||* Skapa support biljetter för partner Center
||* Visa partner support biljetter som du skapar|
|Support agent| * Sök efter och visa en kund|[Eskalera problem till Microsoft och lär dig mer om vilka problem som är mer lämpliga för Microsoft-eskalering](escalate-problems-to-microsoft.md)
||* Redigera kund information
||* Hjälp till att lösa kund problem med fakturerings-eller prenumerations hantering
||* Begär support för kundernas räkning 
||* Hantera prenumerationer och fakturerings problem för kundernas räkning
||* Skapa support biljetter för partner Center
||* Visa partner support biljetter som du skapar| 

### <a name="control-panel-vendor-cpv-csp-role-and-non-azure-ad-role"></a>Kontroll panels leverantör (CPV). (CSP-roll och icke-Azure AD-roll)

CPVs utvecklar appar för användning av leverantörer av moln lösningar (CSP) så att de kan integrera sina system med API: er för partner Center. 

|**Role**   |**Det här kan du göra**|**Läs mer**|
|------------------------------|:----------------------------|----|
|Global administratör| Visa och hantera din CPV-profil|[Registrera dig som en kontroll panels leverantör för att integrera CSP-partnersystem med API: er för partner Center](enroll-as-cpv.md)
||Visa och hantera alla användare som behöver åtkomst till CPV-funktioner|

### <a name="guest-user-must-be-added-to-the-azure-active-directory-tenant"></a>Gäst användare (måste läggas till i Azure Active Directory klient organisationen)

|**Gäst användare**   | **Roller**|
|---------------------------|:--------------------|
||MPN-partner administratör|
||Företags profil administratör|
||Referens administratör|


## <a name="manage-mpn-membership-and-your-company"></a>Hantera MPN-medlemskap och ditt företag 

Dessa roller är inte Azure Active Directory roller. Dessa roller hanterar företagets verksamhet i stället för klient organisationen.

|**Role** | **Det här kan du göra**|**Läs mer**|
|----------------------------|:----------------------------|-----|
|MPN-partner administratör|* Visa, skapa och hantera partner tjänst begär Anden|[Köp eller förnya en Microsoft Action Pack-prenumeration eller silver- eller guldkompetens](mpn-get-action-pack.md)
||* Visa juridiska, företags-, företags-och MPN profiler
||* Visa användar information och deras kunskaps data
||* Visa kompetenser
||* Visa och hantera förmåner
||* Visa och Köp MPN-erbjudanden
||* Visa MPN för order historik och fakturor
||* Visa information om partner bidrags indikatorer
||* Kan användas i validerings verktyget för verifikationer|
||* Visa kund data analys
||* Visa andra användar roller inom företaget, men kan inte tilldela roller
||* Skapa support biljetter för partner Center
||* Visa partner support biljetter som du skapar
|Kontoadministratör| Lägg till platser|[Hantera platser](manage-locations.md)
|| Hantera profiler som är relaterade till de konton som du är administratör för 
||* Tilldela roller för användare i klient organisationen till icke-Azure-Active-Directory-roller 
||* Registrera platser i program
||* Skapa support biljetter för partner Center
||* Visa partner support biljetter som du skapar

## <a name="manage-referrals"></a>Hantera referenser

> [!Note]
>Användar rollen nya hänvisningar kommer att vara tillgänglig från 18 november 2020. Befintliga hänvisnings administratörer behåller sin hänvisnings administratörs roll som är begränsad till hela företaget.

|**Role** | **Det här kan du göra**|**Läs mer**
|------------------------------|:-------------------------|---|
|Referens administratör|Skapa och hantera allt under fliken referenser i Partner Center|[Hantera säljsamarbete](manage-co-sell-opportunities.md)
||    Kan visa och redigera alla samförsäljnings möjligheter och leads
||    Kan tilldela team medlemmar för ett erbjudande
||    Kan visa och redigera affärs profiler
||    Kan visa och registrera erbjudanden för affärs möjligheter som marker ATS som vunna och berättigade för avtals registrering
||    Kan skapa och Visa support biljetter
|Referent användare|Skapa och hantera samförsäljnings möjligheter endast om de ingår i teamet |[Hantera säljsamarbete](manage-co-sell-opportunities.md)
||    Kan skapa samförsäljnings möjligheter för de platser där de tilldelas rollen.
||    Kan visa och registrera erbjudanden för affärs möjligheter som är markerade som vunna och berättigade till avtals registrering om de är team medlemmar.
||    Kan skapa och Visa support biljetter
|Företags profil administratör|Skapa och hantera affärs profiler | [Hantera affärs profiler](create-a-marketing-profile.md)
||    Kan skapa och Visa support biljetter

Tillsammans med användar rollen nya referenser presenterar vi också plats omfånget för avtal. I tabellen nedan förklaras hur du får åtkomst baserat på platsen.

|**Omfång** | **Det här kan du göra** |
|------------------------------|:-------------------------|
|Hela företaget | Både administratörer och användare har åtkomst till att skapa avtal för alla platser i företaget|
|| Referens administratören har åtkomst till att visa och redigera alla avtal |
|| Hänvisnings användare har behörighet att visa och redigera alla avtal endast om de ingår i teamet |
|En eller flera platser | Både administratörer och användare har åtkomst till att skapa avtal för den tilldelade platsen i företaget|
|| Referens administratören har åtkomst till att visa och redigera alla avtal som hör till tilldelade platser|
|| Hänvisnings användare har behörighet att visa och redigera alla avtal som hör till de tilldelade platserna, om de ingår i teamet|

## <a name="manage-incentives"></a>Hantera incitament

|**Role** | **Det här kan du göra**|**Läs mer**
|------------------------------|:-------------------------|---|
|Incitaments administratör|* Initierar och hanterar incitament |[Använd dessa resurser för att komma igång med incitament](incentives-get-started-intro.md)
||* Kan visa och redigera alla aspekter av incitaments program
||* Kan visa och redigera bank-och skatte information
||* Visa rabatt-och samop-intäkter
||* Åtkomst stöd
||* Betalnings åtgärder för tvister|
|Incitaments användare|* Kan visa incitaments program
||* Kan visa och initiera incitaments anspråk
||* Visa rabatt-och samop-intäkter
||* Skapa support biljetter för partner Center
||* Visa partner support biljetter som du skapar

## <a name="view-partner-center-insights-data"></a>Visa information om Partner Center Insights

|**Role** | **Det här kan du göra**|**Läs mer**|
|------------------------------|:-------------------------|---|
|Rapport visnings program för chefer|Åtkomst till alla data uppsättningar för rapportering, skapa partner support biljetter, Visa partner support biljetter som du skapar|[Översikt över instrument panels rapporter i Partner Center Insights](pci-overview-report.md)
|Rapport visnings program|Åtkomst till data rapporter med undantag för intäkter och kunders och anställdas personliga data, skapa partner support biljetter, Visa partner support biljetter som du skapar|

## <a name="next-steps"></a>Nästa steg

- [Skapa användarkonton och tilldela roller och behörigheter](create-user-accounts-and-set-permissions.md)
- [Verifiera din konto information när du registrerar dig i ett nytt Partner Center-program](verification-responses.md)
