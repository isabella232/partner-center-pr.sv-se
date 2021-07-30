---
title: Hantera uteblivna betalningar, bedrägeri eller missbruk
description: Lär dig mer om de olika riskerna med onlinetransaktioner och metodtips för att hantera och minska riskerna i Partnercenter.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-payouts
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 07/14/2020
ms.openlocfilehash: f74a1c091a4c5cd838f8856152c1498f3ecd9d2b
ms.sourcegitcommit: ad1af627f5ee6b6e3a70655f90927e932cf4c985
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 07/29/2021
ms.locfileid: "114836752"
---
# <a name="managing-non-payment-fraud-or-misuse-in-partner-center"></a>Hantera icke-betalning, bedrägeri eller missbruk i Partnercenter

**Gäller för:** Partner Center-| Partnercenter för Microsoft Cloud for US Government

**Lämpliga roller:** Globala | Administratörsbehörighet för | Administratörsagent | Faktureringsadministratör

Du är ekonomiskt ansvarig för bedrägliga köp av dina kunder och/eller kunders icke-betalning av köpta tjänster. Därför rekommenderar *vi starkt att du använder kontroller för bedrägeriskydd och identifiering av riskreducering.*

För att undvika och/eller åtgärda bedräglig aktivitet eller missbruk är det viktigt att förstå potentiella risker och utveckla principer och metoder som kan minska exponeringen.

## <a name="enforcement-of-microsoft-acceptable-use-policy"></a>Framtvingande av Microsofts policy för godtagbar användning

Om Microsoft upptäcker partner- eller kundaktivitet som vi bekräftar eller misstänker bryter mot principen för acceptabel användning, kommer vi att vidta tvingande åtgärder. Kunden kan omedelbart pausas. Microsoft kommer att meddela dig om tvingande åtgärder eller uppdatera dina begäranden.

## <a name="abuse-of-service-risks"></a>Missbruk av tjänstrisker

**Missbruk av tjänstrisker** innebär kunder som använder molntjänster i strid med Microsofts policy för acceptabel användning.

### <a name="examples-of-abuse-of-service"></a>Exempel på missbruk av tjänsten

Exempel på dessa överträdelser av Microsofts acceptable use policy kan vara:

- Spamming
- Hacking
- Distribuerade DDoS-attacker (Denial-of-Service)
- Bitcoin-utvinning
- Distribution av skadlig kod
- Omförsäljning av snedfördelade prenumerationer

## <a name="theft-of-service-risks"></a>Stöld av tjänstrisker

**Stöld av tjänstrisker** innebär kunder som inte har för avsikt att betala för förbrukade tjänster. Den här stölden kan handla om att använda stulna betalningsmedel, tillhandahålla falsk faktureringsinformation och/eller att betala utestående saldon som standard.

### <a name="examples-of-service-theft"></a>Exempel på tjänststöld

Exempel på dessa onlinetransaktionsrisker kan vara:

- Transaktioner som inte sker personligen ("kreditkortet finns inte" transaktioner)
- Felrepresenterade identiteter
- Tjänster som etablerats och används innan den första betalningen tas emot
- Nya marknader och/eller högriskregioner för online-bedrägeri
- Automatisera skapande och inköp av konton av dåliga aktörer

## <a name="managing-online-risk"></a>Hantera onlinerisker

Du kan använda följande rekommendationer för att utveckla principer och metoder för att minska din exponering för onlinetransaktionsrisker i livscykeln för dina kundrelationer.

### <a name="onboarding-new-customers"></a>Registrera nya kunder

Här är några förslag på hur du kan minska onlineriskerna när du ska registrera nya kunder:

- Upprätta personliga relationer med kunder när det är möjligt (till exempel kontakta kunder via telefon).
- Verifiera kundernas autentiseringsuppgifter och bakgrund med bättre metoder (till exempel genom att använda kreditkontor eller kommersiella företagsrapportkontor).
- Använd multifaktorautentisering (till exempel SMS-verifiering) under registrering för att minimera exponeringen för att skapa och köpa robotkonto.
- Hantera och spåra identiteter med hjälp av tjänster (till exempel digitala identitetstjänster).
- Utvärdera kundens ekonomiska styrka genom rigorösa system för identifiering av kreditkortsbedrägerier.
- Upprätta en princip för rensade samlingar. Beskriva dina samlingar och när åtkomsten till prenumerationer påverkas av utebliven betalning. (Du kan inaktivera åtkomst [eller inaktivera en kunds prenumerationer vid](create-a-new-subscription.md#suspend-a-subscription) utebliven betalning.)

### <a name="managing-customer-accounts"></a>Hantera kundkonton

Här är några förslag på hur du kan hantera kundkonton efter köpet:

- Implementera en process för att snabbt ta emot, granska, agera på och svara på Microsoft-meddelanden.
- Arbeta med kunder för att förstå sina affärsbehov för molnanvändning samtidigt som du kan se lämpliga tröskelvärden för övervakning. (Du kan till exempel ange [en månatlig Azure-utgiftsbudget](set-an-azure-spending-budget-for-your-customers.md) i Partnercenter. Den här förståelsen gör att du kan övervaka kundanvändningen under månaden och bli meddelad när kunderna är nära sin budget.)
- Övervaka [kundaktivitetsloggar](activity-logs.md) regelbundet för att upptäcka bedrägerier i ett tidigt skede.
- Vidta snabba åtgärder när misstänkta aktiviteter identifieras.
- Undvik att ge kunderna fullständig administrativ åtkomst till prenumerationer utan att först implementera riskreduceringskontroller.

### <a name="managing-customer-billing"></a>Hantera kundfakturering

Här är några förslag på hur du kan hantera kundfakturering efter köpet:

- Begär förskottsbetalningar före inledande transaktioner och fakturering.
- Acceptera inte betalningsmedel med hög risk (till exempel förbetalda kort eller lagrade värdekort).
- Övervaka kundbetalningar och äldre kundreskontra. Aggressivt framtvinga standardiserade dunningsprocesser för försenade betalningar eller utebliven betalning.

Mer detaljerade strategier för att minimera onlinerisk finns i [onlineguiden för transaktionsriskhantering.](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE4Bhtt)
