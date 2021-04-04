---
title: Hantera uteblivna betalningar, bedrägeri eller missbruk
description: Lär dig mer om de olika riskerna i onlinetransaktioner och de bästa metoderna för att hantera och minimera riskerna i Partner Center.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 07/14/2020
ms.openlocfilehash: 75881544097abdfac8d6f96bde37e9700eb28cf7
ms.sourcegitcommit: f24089cd27b1de6ecf6ddbefb6cbb2d340e144de
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/01/2021
ms.locfileid: "106132357"
---
# <a name="managing-non-payment-fraud-or-misuse-in-partner-center"></a>Hantera icke-betalning, bedrägeri eller missbruk i Partnercenter

Gäller för:

- Partner Center för Microsoft myndighets moln

**Lämpliga roller**

- Global administratör
- Administratör för användar hantering
- Administratörs agent
- Faktureringsadministratör

Du är ekonomiskt ansvarig för bedrägliga köp av dina kunder och/eller kunders utebliven betalning av köpta tjänster. Därför *rekommenderar vi starkt att du inför kontroller av bedrägeri skydd och identifiering av risker*.

För att undvika och/eller adressera bedräglig aktivitet eller missbruk är det viktigt att förstå potentiella risker och utveckla principer och metoder som kan minska exponeringen.

## <a name="enforcement-of-microsoft-acceptable-use-policy"></a>Tillämpning av Microsofts acceptabla användnings princip

Om Microsoft identifierar partner-eller kund aktivitet som vi bekräftar eller misstänker strider mot principen för godkänd användning, vidtar vi tillämpnings anvisningar. Kunden kan inaktive ras omedelbart. Du får ett meddelande om tvingande åtgärder eller uppdaterad på dina begär Anden från Microsoft.

## <a name="abuse-of-service-risks"></a>Missbruk av tjänste risker

**Missbruk av tjänste** risker innebär att kunder som använder moln tjänster strider mot Microsofts acceptabla användnings princip.

### <a name="examples-of-abuse-of-service"></a>Exempel på missbruk av tjänsten

Exempel på följande överträdelser av Microsofts acceptable use policy kan vara:

- Mass utskick
- Hackning
- DDoS-attacker (distributed denial-of-Service)
- Bitcoin-utvinning
- Distribution av skadlig kod
- Åter försäljning av piratkopierade prenumerationer

## <a name="theft-of-service-risks"></a>Stöld av tjänst risker

**Stöld av tjänste** risker innebär att kunder som inte har avsikt att betala för förbrukade tjänster. Den här stölden kan innebära att använda stulna betalnings instrument, tillhandahålla falsk fakturerings information och/eller standardvärden på utestående saldon.

### <a name="examples-of-service-theft"></a>Exempel på tjänst stöld

Exempel på sådana online transaktions risker kan vara:

- Transaktioner som inte inträffar personligen ("kredit kort finns inte"-transaktioner)
- Felvisade identiteter
- Tjänster som tillhandahålls och används före första betalningen tas emot
- Nya marknader och/eller hög risk regioner för bedrägerier online
- Automatisera konto skapande och köp av felaktiga aktörer

## <a name="managing-online-risk"></a>Hantera online-risk

Du kan använda följande rekommendationer för att hjälpa dig att utveckla principer och metoder för att minska exponeringen för transaktions risker online i livs cykeln för dina kund relationer.

### <a name="onboarding-new-customers"></a>Publicera nya kunder

Förslag på att minska antalet online-risker när du registrerar nya kunder är:

- Upprätta personliga relationer med kunder när det är möjligt (till exempel kontakta kunder via telefon).
- Verifiera kundernas autentiseringsuppgifter och bakgrund genom bättre metoder (t. ex. genom att använda kredit byråer eller affärsmässiga rapport byråer).
- Använd Multi-Factor Authentication (till exempel SMS-verifiering) under registreringen för att minimera exponeringen för att skapa och köpa automatiska konton.
- Hantera och spåra identiteter med hjälp av tjänster (t. ex. digitala identitets tjänster).
- Utvärdera kundens finansiella styrka genom rigorösa kredit korts identifierings system.
- Upprätta en princip för att rensa samlingar. Beskriv insamlings processen och när åtkomst till prenumerationer kommer att påverkas av utebliven betalning. (Du kan inaktivera åtkomst eller [pausa en kunds prenumerationer](create-a-new-subscription.md#suspend-a-subscription) för icke-betalning.)

### <a name="managing-customer-accounts"></a>Hantera kundkonton

Förslag på att hantera kund konton efter köpet är:

- Implementera en process för att snabbt få, granska, agera på och svara på Microsoft-meddelanden.
- Arbeta med kunder för att förstå deras behov av moln användnings verksamhet medan inställningarna är lämpliga för övervaknings trösklar. (Du kan till exempel [Ange en månatlig Azure utgifts budget](set-an-azure-spending-budget-for-your-customers.md) i Partner Center. Med den här överenskommelsen kan du övervaka kund användning under månaden och bli informerad när kunderna är nära sina budget.)
- Övervaka [kund aktivitets loggar](activity-logs.md) regelbundet för att hjälpa att upptäcka bedrägerier tidigt.
- Vidta snabb åtgärd när misstänkta aktiviteter identifieras.
- Undvik att ge kunderna fullständig administrativ åtkomst till prenumerationer utan att först implementera risk minsknings kontroller.

### <a name="managing-customer-billing"></a>Hantera kund fakturering

Förslag på hantering av kund fakturerings post-inköp inkluderar:

- Begär förskotts betalningar före första transaktioner och fakturering.
- Godkänn inte högrisk betalnings instrument (till exempel förbetalda kort eller lagrings värde kort).
- Övervaka kund betalningar och kund fordringar för ålders konton. Använd aggressivt standardiserade Dunning-processer för sena betalningar eller utebliven betalning.

Mer detaljerad information om hur du kan åtgärda online-risker finns i [hand boken för transaktions riskhantering.](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE4Bhtt)
