---
title: Tilldela roller & behörigheter till användare
ms.topic: article
ms.date: 10/30/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-enroll
description: Lär dig vilka roller som passar bäst för företagets användare som hanterar kommersiella transaktioner, hänvisningar, incitament eller MPN-medlemskap i Partnercenter.
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: high
ms.custom: SEOMAY.20, contperf-fy21q1
ms.openlocfilehash: 7638a35b5aa583cd3a7c3b40833123402df7cb70
ms.sourcegitcommit: 9d155ff319ba2b2793bc9945d179ce1cb9c8f7c7
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/19/2021
ms.locfileid: "122453806"
---
# <a name="assign-users-roles-and-permissions-for-a-companys-users-needing-to-work-in-partner-center"></a>Tilldela användarroller och behörigheter för ett företags användare som behöver arbeta i Partnercenter

**Lämpliga roller:** Globala | Administratörsbehörighet för användarhantering | MPN-partneradministratör

Du har ställt in din partnerprofil, inklusive juridiskt namn och adress, supportinformation, skattebefrielse för filer, bankinformation och den primära kontakten för ditt företag. Nästa steg: Konfigurera dina användare med lösenord och roller så att de kan börja arbeta i Partnercenter med dig.

## <a name="set-up-your-employees-to-work-in-partner-center"></a>Konfigurera dina anställda att arbeta i Partnercenter

Du avgör vilka typer av åtkomst dina användare har till Partnercenter efter de roller och behörigheter som du ger dem. Roller är relaterade till de program som din verksamhet ingår i. Om ditt företag till exempel är ett Molnlösningsleverantör-företag (CSP) har du inte bara standardrollerna för Azure Active Directory-klientorganisation (Azure AD), till exempel global administratör, utan behöver roller som är specifika för CSP-programmet. Varje program har specifika roller.

>[!Note]
> Azure AD-klientroller omfattar rollerna global administratör, användaradministratör och CSP. Icke-Azure-AD-roller är de roller som inte hanterar klientorganisationen och de omfattar MPN-partneradministratör (Microsoft Partner Network), företagsprofiladministratör, referensadministratör, incitamentadministratör och incitamentanvändare. 

### <a name="manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles"></a>Hantera kommersiella transaktioner i Partnercenter (Azure AD- och CSP-roller)

|**Role**|**Vad de kan göra**|**Läs mer**|
|----------------------------------|---|:---------------------------------|
|Global administratör|* Kan komma åt Microsoft-konto/tjänster med fullständig behörighet|[Hantera ditt Partnercenter-konto](partner-center-account-setup.md)
|      |* Skapa supportärenden för Partnercenter
||* Visa partnersupportärenden som du skapar
||* Visa avtal, prislistor och erbjudanden
||* Visa, skapa och hantera partneranvändare|
||  Visa, skapa och hantera fakturering, fakturor och rekognoseringsfiler
|Administratör för användarhantering   | * Visa, skapa och hantera användare|[Hantera Microsoft Partner Network medlemskapsförmåner och erbjudanden i Partnercenter](manage-your-partner-network-benefits.md)
||* Visa alla partnerprofiler
||* Skapa supportärenden för Partnercenter
||* Visa partnersupportärenden som du skapar
|Faktureringsadministratör | – Visa, skapa och hantera fakturering, fakturor och rekognoseringsfiler|[Läsa fakturan](billing.md)
||* Visa priser
||* Skapa supportärenden för Partnercenter
||* Visa partnersupportärenden som du skapar
|Standardanvändare|  Visa Min profil   |[Återställa lösenordet](reset-my-pasword.md)
|Administratörsagent | * Kundhantering|[Få kontakt med dina kunder](connect-with-your-customers.md)
||* Lägg till enhetslista i Partnercenter
||* Skapa och tillämpa profiler på enheter
||* Prenumerationshantering
||* Tjänsthälsa och tjänstbegäranden för kunder
||* Begära delegerade administratörsbehörigheter
||* Visa priser och erbjudanden
||* Fakturering
||* Administrera för en kunds räkning
||* Registrera en återförsäljare med mervärde
||* Skapa supportärenden för Partnercenter
||* Visa partnersupportärenden som du skapar|
|Försäljningsagent | * Kundhantering|[Tillhandahålla faktureringssupport för dina kunder och hjälp med att besvara deras faktureringsfrågor](provide-billing-support.md)
||* Lägg till enhetslista i Partnercenter
||* Prenumerationshantering
||* Visa supportärenden
||* Begära en relation med en kund
||* Visa priser och erbjudanden
||* Hantera kund leads
||* Visa kundavtalet
||* Registrera en återförsäljare med mervärde
||* Skapa supportärenden för Partnercenter
||* Visa partnersupportärenden som du skapar|
|Supportagent| * Sök efter och visa en kund|[Eskalera problem till Microsoft och lär dig vilka problem som passar bättre för Microsoft-eskalering](escalate-problems-to-microsoft.md)
||* Redigera kundinformation
||* Hjälp till att lösa kundproblem med fakturerings- eller prenumerationshantering
||* Begär support för kunders räkning 
||* Hantera prenumerationer och faktureringsproblem åt kunder
||* Skapa supportärenden för Partnercenter
||* Visa partnersupportärenden som du skapar| 

### <a name="control-panel-vendor-cpv-csp-role-and-non-azure-ad-role"></a>Kontrollpanelen Vendor (CPV). (CSP-roll och icke-Azure AD-roll)

CPV:er utvecklar appar för användning av CSP-partner så att de kan integrera sina system med Partner Center-API:er. 

|**Role**   |**Det här kan du göra**|**Läs mer**|
|------------------------------|:----------------------------|----|
|Global administratör| Visa och hantera din Kontrollpanelen leverantörsprofil (CPV)|[Registrera dig som en Kontrollpanelen leverantör för att integrera CSP-partnersystem med Partner Center-API:er](enroll-as-cpv.md)
||Visa och hantera alla användare som behöver åtkomst till CPV-funktioner|

### <a name="guest-user-must-be-added-to-the-azure-ad-tenant"></a>Gästanvändare (måste läggas till i Azure AD-klientorganisationen)

|**Gästanvändare**   | **Roller**|
|---------------------------|:--------------------|
||MPN-partneradministratör|
||Företagsprofiladministratör|
||Referensadministratör|


## <a name="manage-mpn-membership-and-your-company"></a>Hantera MPN-medlemskap och ditt företag 

Dessa roller är inte Azure AD-roller. De här rollerna hanterar företagets verksamhet i stället för klientorganisationen.

|**Role** | **Det här kan du göra**|**Läs mer**|
|----------------------------|:----------------------------|-----|
|MPN-partneradministratör|* Visa, skapa och hantera partnertjänstbegäranden|[Köp eller förnya en Microsoft Action Pack-prenumeration eller silver- eller guldkompetens](mpn-get-action-pack.md)
||* Visa profiler för juridik, företag, företag och MPN
||* Visa användarinformation och deras kompetensdata
||* Visa kompetenser
||* Visa och hantera fördelar
||* Visa och köpa MPN-erbjudanden
||* Visa MPN-erbjudanden, orderhistorik och fakturor
||* Visa indikatordata för partnerbidrag
||* Kan fungera i valideringsverktyget för validering|
||* Visa kunddataanalys
||* Visa andra användarroller inom företaget, men kan inte tilldela roller
||* Skapa supportärenden för Partnercenter
||* Visa partnersupportärenden som du skapar
|Kontoadministratör| Lägg till platser|[Hantera platser](manage-locations.md)
|| Hantera profiler relaterade till de konton som du är administratör för 
||* Tilldela roller för användare i klientorganisationen till icke-Azure-AD-roller 
||* Registrera platser i program
||* Skapa supportärenden för Partnercenter
||* Visa partnersupportärenden som du skapar

## <a name="manage-referrals"></a>Hantera hänvisningar

|**Role** | **Det här kan du göra**|**Läs mer**
|------------------------------|:-------------------------|---|
|Referensadministratör|Skapa och hantera allt under fliken Referenser i Partnercenter|[Hantera möjligheter till säljsamarbete](manage-co-sell-opportunities.md)
||    Kan visa och redigera alla möjligheter till säljförsäljning och leads
||    Kan tilldela teammedlemmar för ett avtal
||    Kan visa och redigera företagsprofiler
||    Kan visa och registrera avtal för affärsmöjligheter som har markerats som vann och berättigade till avtalsregistrering
||    Kan skapa och visa supportärenden
|Referensanvändare|Skapa och hantera möjligheter till säljförsäljning endast om de ingår i teamet |[Hantera möjligheter till säljsamarbete](manage-co-sell-opportunities.md)
||    Kan skapa möjligheter till säljförsäljning för de platser där de tilldelas rollen.
||    Kan visa och registrera avtal för affärsmöjligheter som har markerats som vann och berättigade till avtalsregistrering om de är gruppmedlem.
||    Kan skapa och visa supportärenden
|Företagsprofiladministratör|Skapa och hantera företagsprofiler | [Hantera företagsprofiler](create-a-marketing-profile.md)
||    Kan skapa och visa supportärenden

Tillsammans med den nya referensanvändarrollen introducerar vi även platsomfånget för avtal. Tabellen nedan förklarar avtalsåtkomsten baserat på platsen.

|**Omfång** | **Det här kan du göra** |
|------------------------------|:-------------------------|
|Hela företaget | Både administratörer och användare har åtkomst till att skapa avtal för alla platser i företaget|
|| Referensadministratören har åtkomst till att visa och redigera alla avtal |
|| Hänvisningsanvändare har endast åtkomst till att visa och redigera alla avtal om de ingår i teamet |
|En eller flera platser | Både administratörer och användare har åtkomst till att skapa avtal för den tilldelade platsen i företaget|
|| Referensadministratören har åtkomst till att visa och redigera alla avtal som hör till de tilldelade platserna|
|| Hänvisningsanvändare har åtkomst till att visa och redigera alla avtal som hör till de tilldelade platserna om de ingår i teamet|

## <a name="manage-incentives"></a>Hantera incitament

|**Role** | **Det här kan du göra**|**Läs mer**
|------------------------------|:-------------------------|---|
|Incitamentsadministratör|* Initierar och hanterar incitament |[Använd de här resurserna för att komma igång med incitament](incentives-get-started-intro.md)
||* Kan visa och redigera alla aspekter av incitamentsprogram
||* Kan visa och redigera bank- och skatteinformation
||* Visa löner och co-op-intäkter
||* Åtkomststöd
||* Bestrida incitamentsbetalningar|
|Incitamentsanvändare|* Kan visa incitamentsprogram
||* Kan visa och initiera incitamentsanspråk
||* Visa löner och co-op-intäkter
||* Skapa supportärenden för Partnercenter
||* Visa partnersupportärenden som du skapar

## <a name="view-partner-center-insights-data"></a>Visa partnercenter för Insights data

|**Role** | **Det här kan du göra**|**Läs mer**|
|------------------------------|:-------------------------|---|
|Visningsprogram för chefsrapport|Åtkomst till alla rapportdatauppsättningar, skapa partnersupportärenden, visa partnersupportärenden som du skapar|[Översikt över instrumentpanelsrapporter som är tillgängliga i Partnercenter Insights](insights-overview-report.md)
|Rapportvisningsprogram|Åtkomst till datarapporter med undantag för intäkter och kund- och medarbetares personliga data, skapa partnersupportärenden, visa partnersupportärenden som du skapar|

## <a name="next-steps"></a>Nästa steg

- [Skapa användarkonton och tilldela roller och behörigheter](create-user-accounts-and-set-permissions.md)
- [Verifiera din kontoinformation när du registrerar dig i ett nytt Partnercenter-program](verification-responses.md)
