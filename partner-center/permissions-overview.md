---
title: Tilldela roller och behörigheter till användare
ms.topic: article
ms.date: 09/27/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-account
description: Lär dig vilka roller som passar bäst för företagets användare som hanterar kommersiella transaktioner, hänvisningar, incitament eller MPN-medlemskap i Partnercenter.
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: high
ms.custom: SEOMAY.20, contperf-fy21q1
ms.openlocfilehash: 46d17de1ba7572c72162cfd38143ed9aa084c5c7
ms.sourcegitcommit: d731813da1d31519dc2dc583d17899e5cf4ec1b2
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/27/2021
ms.locfileid: "129075773"
---
# <a name="assign-roles-and-permissions-to-users"></a>Tilldela roller och behörigheter till användare

**Lämpliga roller:** Global | Administratörsbehörighet för användarhantering | MPN-partneradministratör

Du har ställt in din partnerprofil, inklusive juridiskt namn och adress, supportinformation, skattebefrielse för filer, bankinformation och den primära kontakten för ditt företag. Nästa steg är att konfigurera dina användare med lösenord och roller så att de kan börja arbeta i Partnercenter med dig.

## <a name="set-up-your-employees-to-work-in-partner-center"></a>Konfigurera dina anställda att arbeta i Partnercenter

Du avgör vilka typer av åtkomst dina användare har till Partnercenter efter de roller och behörigheter som du ger dem. Roller är relaterade till de program som din verksamhet ingår i. Om ditt företag till exempel är ett Molnlösningsleverantör-företag (CSP) har du inte bara standardrollerna för hantering av Azure Active Directory-klienter (Azure AD), till exempel global administratör, utan behöver roller som är specifika för CSP-programmet. Varje program har specifika roller.

> [!NOTE]
> Azure AD-klientroller omfattar rollerna global administratör, användaradministratör och CSP. Icke-Azure-AD-roller är de roller som inte hanterar klientorganisationen och de inkluderar MPN-partneradministratör (Microsoft Partner Network), företagsprofiladministratör, referensadministratör, incitamentadministratör och incitamentanvändare. 

### <a name="manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles"></a>Hantera kommersiella transaktioner i Partnercenter (Azure AD- och CSP-roller)

|**Role**|**Vad de kan göra**| **Arbetsyta** | **Läs mer**|
|----------------------------------|---|---|:---------------------------------|
|Global administratör|* Kan komma åt Microsoft-konto/tjänster med fullständig behörighet| Kontoinställningar | [Hantera ditt Partnercenter-konto](partner-center-account-setup.md) |
||* Skapa supportärenden för Partnercenter | Hjälp + support |
||* Visa partnersupportärenden som du skapar | Hjälp + support |
||* Visa avtal, prislistor och erbjudanden | Prissättning |
||* Visa, skapa och hantera partneranvändare | Kontoinställningar |
||  Visa, skapa och hantera fakturering, fakturor och rekognoseringsfiler | Fakturering |
| Administratör för användarhantering   | * Visa, skapa och hantera användare| Fördelar | [Hantera Microsoft Partner Network medlemsförmåner och erbjudanden i Partnercenter](manage-your-partner-network-benefits.md)
||* Visa alla partnerprofiler | Kunder |
||* Skapa supportärenden för Partnercenter | Hjälp + support |
||* Visa partnersupportärenden som du skapar | Hjälp + support |
|Faktureringsadministratör | – Visa, skapa och hantera fakturering, fakturor och rekognoseringsfiler| Fakturering | [Läsa fakturan](billing.md)
||* Visa priser | Fakturering |
||* Skapa supportärenden för Partnercenter | Hjälp + support |
||* Visa partnersupportärenden som du skapar | Hjälp + support |
|Standardanvändare|  Visa min profil   | Kontoinställningar | [Återställa lösenordet](reset-my-pasword.md)
|Administratörsagent | * Kundhantering| Kunder | [Få kontakt med dina kunder](connect-with-your-customers.md)
||* Lägg till enhetslista i Partnercenter | Kontoinställningar |
||* Skapa och tillämpa profiler på enheter | Kontoinställningar |
||* Prenumerationshantering | Kontoinställningar |
||* Tjänsthälsa och tjänstbegäranden för kunder | Hjälp + support |
||* Begära delegerade administratörsbehörigheter | Kontoinställningar |
||* Visa priser och erbjudanden | Prissättning |
||* Fakturering | Fakturering |
||* Administrera för en kunds räkning | Kontoinställningar |
||* Registrera en återförsäljare med mervärde | Kontoinställningar |
||* Skapa supportärenden för Partnercenter | Hjälp + support |
||* Visa partnersupportärenden som du skapar | Hjälp + support |
|Försäljningsagent | * Kundhantering| Fakturering | [Tillhandahålla faktureringssupport för dina kunder och hjälp med att besvara deras faktureringsfrågor](provide-billing-support.md)
||* Lägg till enhetslista i Partnercenter | Kontoinställningar |
||* Prenumerationshantering | Kontoinställningar |
||* Visa supportärenden | Hjälp + support |
||* Begära en relation med en kund | Kunder |
||* Visa priser och erbjudanden | Prissättning |
||* Hantera kund-leads | Referenser |
||* Visa kundavtalet | Kunder |
||* Registrera en återförsäljare med mervärde | Kontoinställningar |
||* Skapa supportärenden för Partnercenter | Hjälp + support |
||* Visa partnersupportärenden som du skapar | Hjälp + support |
|Supportagent| * Söka efter och visa en kund| Hjälp + support | [Eskalera problem till Microsoft och lär dig vilka problem som passar bättre för Microsoft-eskalering](escalate-problems-to-microsoft.md)
||* Redigera kundinformation  | Hjälp + support |
||* Hjälp med att lösa kundproblem med fakturerings- eller prenumerationshantering | Hjälp + support |
||* Begär support för kunders räkning | Hjälp + support |
||* Hantera prenumerationer och faktureringsproblem åt kunder | Fakturering |
||* Skapa supportärenden för Partnercenter | Hjälp + support |
||* Visa partnersupportärenden som du skapar  | Hjälp + support |

### <a name="control-panel-vendor-cpv-csp-role-and-non-azure-ad-role"></a>Kontrollpanelen Leverantör (CPV). (CSP-roll och icke-Azure AD-roll)

CPV:er utvecklar appar för användning av CSP-partner så att de kan integrera sina system med Partner Center-API:er.

|**Role**                   | **Det här kan du göra**      | **Arbetsyta** | **Läs mer**|
|------------------------------|:----------------------------|---------------|---------------|
|Global administratör| Visa och hantera din Kontrollpanelen leverantörsprofil (CPV)|  | [Registrera dig som en Kontrollpanelen leverantör för att integrera CSP-partnersystem med Partner Center-API:er](enroll-as-cpv.md)
||Visa och hantera alla användare som behöver åtkomst till CPV-funktioner |  |

### <a name="guest-user-must-be-added-to-the-azure-ad-tenant"></a>Gästanvändare (måste läggas till i Azure AD-klientorganisationen)

| **Gästanvändare**    | **Roller**            |
|----------------------|:------------------------|
|                      | MPN-partneradministratör       |
|                      | Administratör för företagsprofil  |
|                      | Referensadministratör         |

## <a name="manage-mpn-membership-and-your-company"></a>Hantera MPN-medlemskap och ditt företag

Dessa roller är **inte** Azure AD-roller. De används för att hantera företagets verksamhet i stället för klientorganisationen.

| **Role** | **Det här kan du göra** | **Arbetsyta** | **Läs mer**|
|----------------------------|:----------------------------|-----|
|MPN-partneradministratör|* Visa, skapa och hantera partnertjänstbegäranden| Medlemskap | [Köp eller förnya en Microsoft Action Pack-prenumeration eller silver- eller guldkompetens](mpn-get-action-pack.md) |
| |* Visa profiler för juridik, företag, företag och MPN | Kontoinställningar |
| |* Visa användarinformation och deras kompetensdata | Medlemskap |
| |* Visa kompetenser | Medlemskap |
| |* Visa och hantera fördelar | Fördelar |
| |* Visa och köpa MPN-erbjudanden | Medlemskap |
| |* Visa ORDERHISTORIK och fakturor för MPN-erbjudanden | Medlemskap |
| |* Visa indikatordata för partnerbidrag | Medlemskap |
| |* Kan fungera i valideringsverktyget för validering av validering | Medlemskap |
| |* Visa kunddataanalys | Insikter |
| |* Visa andra användarroller i företaget, men kan inte tilldela roller | Kontoinställningar |
| |* Skapa supportärenden för Partnercenter | Hjälp + support |
| |* Visa partnersupportärenden som du skapar | Hjälp + support |
| Kontoadministratör| Lägg till platser| Kontoinställningar | [Hantera platser](manage-locations.md)
| |* Hantera profiler relaterade till de konton som du är administratör för | Kontoinställningar |
| |* Tilldela roller för användare i klientorganisationen till icke-Azure AD-roller | Kontoinställningar |
| |* Registrera platser i program |  |
| |* Skapa supportärenden för Partnercenter | Hjälp + support |
| |* Visa partnersupportärenden som du skapar | Hjälp + support |

## <a name="manage-referrals"></a>Hantera hänvisningar

|**Role** | **Det här kan du göra**| **Arbetsyta** | **Läs mer** |
|------------------------------|:---|-----------------------|---|
|Referensadministratör|Skapa och hantera allt under fliken Referenser i Partnercenter| Referenser | [Hantera möjligheter till säljsamarbete](manage-co-sell-opportunities.md)
||    Kan visa och redigera alla möjligheter till säljförsäljning och leads | Referenser |
||    Kan tilldela teammedlemmar för ett avtal | Referenser |
||    Kan visa och redigera företagsprofiler | Referenser |
||    Kan visa och registrera avtal för affärsmöjligheter som har markerats som vann och berättigade till avtalsregistrering | Referenser |
||    Kan skapa och visa supportärenden | Hjälp + support |
|Referensanvändare|Skapa och hantera möjligheter till säljförsäljning endast om de ingår i teamet | Referenser | [Hantera möjligheter till säljsamarbete](manage-co-sell-opportunities.md)
||    Kan skapa möjligheter till säljförsäljning för de platser där de tilldelas rollen. | Referenser |
||    Kan visa och registrera avtal för affärsmöjligheter som markerats som vann och berättigade till avtalsregistrering om de är gruppmedlem. | Referenser |
||    Kan skapa och visa supportärenden | Hjälp + support |
|Administratör för företagsprofil|Skapa och hantera företagsprofiler | Referenser | [Hantera företagsprofiler](create-a-marketing-profile.md)
||    Kan skapa och visa supportärenden | Hjälp + support |

Tillsammans med den nya referensanvändarrollen introducerar vi även platsomfånget för avtal. Tabellen nedan förklarar avtalsåtkomsten baserat på platsen.

|**Omfång** | **Det här kan du göra** | **Arbetsyta** |
|------------------------------|:-----------------|--------|
|Hela företaget | Både administratörer och användare har åtkomst till att skapa avtal för alla platser i företaget| Referenser |
|| Referensadministratören har åtkomst till att visa och redigera alla avtal | Referenser |
|| Hänvisningsanvändare har endast åtkomst till att visa och redigera alla avtal om de ingår i teamet | Referenser |
|En eller flera platser | Både administratörer och användare har åtkomst till att skapa avtal för den tilldelade platsen i sitt företag| Referenser |
|| Referensadministratören har åtkomst till att visa och redigera alla avtal som hör till de tilldelade platserna| Referenser |
|| Hänvisningsanvändare har åtkomst till att visa och redigera alla avtal som hör till de tilldelade platserna om de ingår i teamet| Referenser |

## <a name="manage-incentives"></a>Hantera incitament

|**Role** | **Det här kan du göra**| **Arbetsyta** | **Läs mer** |
|---------|:-------------------|---------------|----------------|
|Incitamentsadministratör|* Initierar och hanterar incitament | Incitament | [Använd de här resurserna för att komma igång med incitament](incentives-get-started-intro.md) |
||* Kan visa och redigera alla aspekter av incitamentsprogram | Incitament |
||* Kan visa och redigera bank- och skatteinformation | Incitament |
||* Visa löner och co-op-intäkter | Incitament |
||* Åtkomststöd | Hjälp + support |
||* Bestrid incitamentsbetalningar | Incitament |
|Incitamentsanvändare|* Kan visa incitamentsprogram | Incitament ||
||* Kan visa och initiera incitamentsanspråk | Incitament |
||* Visa löner och co-op-intäkter | Incitament |
||* Skapa supportärenden för Partnercenter | Hjälp + support |
||* Visa partnersupportärenden som du skapar | Hjälp + support |

## <a name="view-partner-center-insights-data"></a>Visa Insights partnercenter

|**Role** | **Det här kan du göra** | **Arbetsyta** | **Läs mer** |
|---------|:--------------------|---------------|----------------|
|Visningsprogram för exekutiv rapport|Åtkomst till alla rapportdatauppsättningar, skapa partnersupportärenden, visa partnersupportärenden som du skapar| Insikter | [Översikt över instrumentpanelsrapporter som är tillgängliga i Partnercenter-Insights](insights-overview-report.md) |
|Rapportvisningsprogram|Åtkomst till datarapporter med undantag för intäkter och personliga data för kunder och anställda, skapa partnersupportärenden, visa partnersupportärenden som du skapar | Insikter | |

## <a name="next-steps"></a>Nästa steg

- [Skapa användarkonton och tilldela roller och behörigheter](create-user-accounts-and-set-permissions.md)
- [Verifiera din kontoinformation när du registrerar dig i ett nytt Partnercenter-program](verification-responses.md)
