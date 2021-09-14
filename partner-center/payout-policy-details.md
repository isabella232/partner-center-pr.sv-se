---
title: Utbetalningsscheman och -processer
description: Lär dig mer om utbetalning och transaktioner, till exempel betalningsscheman och återbetalningsprocesser för Azure Marketplace och andra transaktioner.
ms.service: partner-dashboard
ms.subservice: partnercenter-payouts
ms.topic: conceptual
author: eunjkim520
ms.author: eunjkim
ms.date: 05/25/2021
ms.openlocfilehash: d30dbc3db4727aac815c37406d36f416b4563f10
ms.sourcegitcommit: 37eac16c4339cb97831eb2a86d156c45bdf6a531
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/13/2021
ms.locfileid: "126247428"
---
# <a name="payout-schedules-and-processes"></a>Utbetalningsscheman och -processer

**Lämpliga roller:** Kontoadministratörsroller | Global administratör

Den här artikeln beskriver Microsofts betalningsschema, var du hittar status för en utbetalning och processen för icke-betalning från kunden.

## <a name="payment-schedules"></a>Betalningsscheman

I följande avsnitt beskrivs vår utbetalningsprocess för **företagsavtal** och **Microsoft-kundavtal CSP-transaktioner.**

### <a name="transactions-when-customer-has-an-enterprise-agreement"></a>Transaktioner när kunden har en företagsavtal

När en kund köper en produkt från Microsoft AppSource eller Azure Marketplace med hjälp av sin befintliga Microsoft företagsavtal för transaktioner, kommer vi att utfärda utbetalningar i nästa utbetalningscykel 30 dagar efter kundfakturan. Transaktioner där en kund använder ett kreditkort har en kvarhållningsperiod på 30 dagar före utbetalningen.

En utbetalning sker ofta innan Microsoft samlar in betalning från kunden. Se [Process för utebliven betalning av kund](#process-for-customer-non-payment) nedan för de åtgärder vi vidta om kunden inte betalar Microsoft, men vi redan har utfärdat en utbetalning.

| Händelse | Description | Rapporteringssynlighet | Tidsinställning* |
| --- | --- | --- | --- |
| Användning eller månad för transaktion | Kunden använder eller köper en tjänst. | [Instrumentpanel](/azure/marketplace/partner-center-portal/usage-dashboard) för [användning eller](/azure/marketplace/partner-center-portal/orders-dashboard) beställning | **Månad 1** |
| Microsoft beräknar faktureringsbeloppet | Fastställa total användning, totalt antal transaktioner | [Instrumentpanel](/azure/marketplace/partner-center-portal/usage-dashboard) för [användning eller](/azure/marketplace/partner-center-portal/orders-dashboard) beställning | **Månad 2** |
| Utbetalning som har publicerats | Fastställa myndighetsavgifter och utbetalningsintäkter | Markerat som Obearbetat i transaktionshistoriken på [utbetalningsutdraget](payout-statement.md) | **Månad 3 (första veckan)** |
| Förbereda utbetalning | Intäkter förbereds för månatlig betalning | Markerat som Kommande i transaktionshistoriken i [utbetalningsutdraget](payout-statement.md) | **Månad 3 (första veckan)** |
| **Utbetalningen har skickats** | **Betalningen skickas till utgivaren** | **Markerat som Skickat i transaktionshistoriken och i avsnittet Betalningar i [utbetalningsutdrag](payout-statement.md)** | **Månad 3 (senast den 15:e)** |
| Faktura som betalas av kunden | Microsoft samlar in betalning från kund | Ingen ändring | **Månad 4 till och med 12** |
|

\* Utbetalningsdatumet är i Pacific Standard Time (PST).

:::image type="content" source="images/payouts/timeline-enterprise.png" alt-text="Tidslinje för betalningar för Enterprise-avtalskunder.":::

### <a name="transactions-when-customer-has-a-microsoft-customer-agreement-or-csp"></a>Transaktioner när kunden har en Microsoft-kundavtal eller CSP

Alla inköp med kreditkort eller månadsfaktura har en 30-dagars kvarhållningsperiod för att säkerställa att medel samlas in från kunden.

| Händelse | Description | Rapporteringssynlighet | Tidsinställning* |
| --- | --- | --- | --- |
| Användning eller månad för transaktion | Kunden använder eller köper en tjänst. | [Instrumentpanel](/azure/marketplace/partner-center-portal/usage-dashboard) för [användning eller](/azure/marketplace/partner-center-portal/orders-dashboard) beställning | **Månad 1** |
| Faktura som betalas av kunden | Fastställa total användning, totalt transaktionsvärde och kundbetalningsfaktura | [Instrumentpanel](/azure/marketplace/partner-center-portal/usage-dashboard) för [användning eller](/azure/marketplace/partner-center-portal/orders-dashboard) beställning | **Månad 2** |
| Utbetalning som har publicerats | Fastställa myndighetsavgifter och utbetalningsintäkter | Markerat som Obearbetat i transaktionshistoriken på [utbetalningsutdraget](payout-statement.md) | **Månad 2** |
| 30-dagars kvarhållningsperiod | Se till att medel, möjliga återbetalningar och återbetalningar görs | Markerat som Obearbetat i transaktionshistoriken på [utbetalningsutdraget](payout-statement.md) | **Månad 3** |
| Förbereda utbetalning | Intäkter förbereds för månatlig betalning | Markerat som Kommande i transaktionshistoriken i [utbetalningsutdraget](payout-statement.md) | **Månad 4 (första veckan)** |
| **Utbetalningen har skickats** | **Betalningen skickas till utgivaren** | **Markerat som Skickat i transaktionshistoriken och i avsnittet Betalningar i [utbetalningsutdrag](payout-statement.md)** | **Månad 4 (senast den 15:e)** |
|

\* Utbetalningsdatumet är i Pacific Standard Time (PST).

:::image type="content" source="images/payouts/timeline-credit-card-invoice.png" alt-text="Tidslinje för betalningar för kreditkorts- och fakturakunder.":::

## <a name="process-for-customer-non-payment"></a>Process för utebliven betalning av kund

I sällsynta fall kan Microsoft inte samla in betalningar från kunder för sina köp på den kommersiella marknadsplatsen. När en kund inte betalar Microsoft enligt sitt faktureringsschema påbörjar vi insamlingsprocessen. Den här processen tar cirka fyra månader och omfattar beständig kommunikation från Microsoft. Om betalningen inte tas emot i slutet av den här processen skriver Microsoft av beloppen som osamlade.

Enligt utbetalningsprocessen som formuleras här kanske Microsoft redan har betalat ut pengar till utgivare (du) som i slutänden inte går att samla in. Därför har vi en process för att stämma av dessa mängder.

Microsoft kommer att få tillbaka alla utbetalningar som redan har betalats till dig med någon av följande metoder: (1) Microsoft kan subtrahera de obetalt beloppen från framtida utbetalningar; Om till exempel 1 000 USD i utbetalning betraktas som osamlade och skrivs av, kommer dina framtida utbetalningar att vara väntande tills de 1 000 USD har återställts eller (2) Microsoft kan begära en återbetalning eller fakturautgivare för eventuella oupptäckta belopp.

Följande schema är ett exempel:

| Händelse | Ungefärligt datum* | Partnersynlighet |
| --- | --- | --- |
| Exempel på utbetalningsdatum | 10/15/2020 | Markerat som **Skickat i** transaktionshistoriken och i avsnittet Betalningar i utbetalningsinstrumentpanelen |
| <font color="red">Om kunden inte betalar Microsoft</font> | 12/2/2020 – 12/5/2020 | Ingen ändring, samma som ovan |
| Kunden får sitt första e-postmeddelande med försenad betalning | 12/6/2020 | Ingen |
| Kunden får regelbundna e-postmeddelanden om ökande angelägenhetsgrad | 12/7/2020 – 1/31/2021 | Ingen |
| Publisher meddelas om avskrivning är sannolikt | 1/7/2021 | - |
| Kunden får ett meddelande om uppsägning | 2/1/2021 | Ingen |
| Insamlingsprocessen slutar/medel skrivs av | 2/15/2021 | E-postmeddelande som skickas till utgivaren om att medel har skrivits av. |
| Utbetalning dras av | 3/1/2021 | Publisher ser negativa transaktioner i partnercentrets utbetalningsutdrag |
| Utbetalningen är indragen | 3/15/2021 | Framtida utbetalningar visas i partnercentrets utbetalningsutdrag. Publisher får ingen betalning förrän saldot inte längre är negativt.  |
|||

\* Utbetalningsdatumet är i Pacific Standard Time (PST).

## <a name="number-of-days-for-payments-to-reach-a-payout-account"></a>Antal dagar som betalningar ska nå ett utbetalningskonto

Vanligtvis skickar vi en betalning som förfaller under en viss månad den 15:e dagen i den månaden, men det tar en annan tid för betalningen att nå ditt konto. Antalet dagar beror på vilken betalningsmetod vi använder för ditt konto, enligt beskrivningen nedan.

> [!NOTE]
> De dagar som visas nedan är ungefärliga; eventuell betalning kan ta mer eller mindre tid att nå ditt konto.

| Betalningsmetod     | Antal dagar som utbetalningskontot ska nås     |
|--------------------|--------------------------------------------|
| PayPal             | 1 arbetsdag                             |
| ACH/SEPA           | 2–3 arbetsdagar                          |
| Banköverföring      | 7–10 arbetsdagar                         |
|

## <a name="next-steps"></a>Nästa steg

- [Skatteinformation](tax-details-marketplace.md)
