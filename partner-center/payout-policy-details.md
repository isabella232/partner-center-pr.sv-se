---
title: Utbetalningsscheman och -processer
description: Lär dig mer om utbetalning och transaktioner, till exempel betalningsscheman och återbetalningsprocesser för den kommersiella marknadsplatsen och andra transaktioner.
ms.service: marketplace
ms.subservice: partnercenter-marketplace-publisher
ms.topic: conceptual
author: eunjkim520
ms.author: eunjkim
ms.date: 12/04/2020
ms.openlocfilehash: f2ba8132677eb0a0368021b6d7065f5202589f24
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 05/19/2021
ms.locfileid: "110146960"
---
# <a name="payout-schedules-and-processes"></a>Utbetalningsscheman och -processer

**Lämpliga roller:** Kontoadministratörsroller | Global administratör

Den här artikeln beskriver Microsofts betalningsschema, var du hittar status för en utbetalning och processen för att inte betala av kunden.

## <a name="payment-schedules"></a>Betalningsscheman

I följande avsnitt beskrivs vår utbetalningsprocess för **Enterprise-avtal** **och kreditkorts-/fakturatransaktioner.**

### <a name="enterprise-agreement-transactions"></a>Enterprise-avtalstransaktioner

När en kund köper en produkt från Microsoft AppSource eller Azure Marketplace med sitt befintliga Microsoft Enterprise-avtal för transaktioner, kommer vi att utfärda utbetalningar i nästa utbetalningscykel 30 dagar efter kundfakturan. Transaktioner där en kund använder ett kreditkort har en kvarhållningsperiod på 30 dagar före utbetalningen.

En utbetalning sker ofta innan Microsoft samlar in betalningar från kunden. Se [Process för kundens uteblivna betalning](#process-for-customer-non-payment) nedan för de åtgärder vi vidta om kunden inte betalar Microsoft men vi redan har utfärdat en utbetalning.

| Händelse | Description | Rapporteringssynlighet | Tidsinställning* |
| --- | --- | --- | --- |
| Användning eller transaktionsmånad | Kunden använder eller köper en tjänst. | [Instrumentpanel](/azure/marketplace/partner-center-portal/usage-dashboard) för [användning eller](/azure/marketplace/partner-center-portal/orders-dashboard) beställning | **Månad 1** |
| Microsoft beräknar faktureringsbeloppet | Fastställa total användning, totalt antal transaktioner | [Instrumentpanel](/azure/marketplace/partner-center-portal/usage-dashboard) för [användning eller](/azure/marketplace/partner-center-portal/orders-dashboard) beställning | **Månad 2** |
| Utbetalning som har publicerats | Fastställa myndighetsavgifter och utbetalningsintäkter | Markerat som Obearbetat i transaktionshistoriken på [utbetalningsutdraget](payout-statement.md) | **Månad 3 (första veckan)** |
| Förbereda utbetalning | Intäkter förbereds för månatlig betalning | Markerat som Kommande i transaktionshistoriken i [utbetalningsutdraget](payout-statement.md) | **Månad 3 (första veckan)** |
| **Utbetalningen har skickats** | **Betalningen skickas till utgivaren** | **Markerat som Skickat i transaktionshistoriken och i avsnittet Betalningar i [utbetalningsutdrag](payout-statement.md)** | **Månad 3 (senast den 15:e)** |
| Faktura som betalas av kunden | Microsoft samlar in betalning från kund | Ingen ändring | **Månad 4 till och med 12** |
|

\* Utbetalningsdatumet är i Pacific Standard Time (PST).

:::image type="content" source="images/payouts/timeline-enterprise.png" alt-text="Tidslinje för betalningar för Enterprise-avtalskunder.":::

### <a name="transactions-with-credit-card-or-invoice-checkwire"></a>Transaktioner med kreditkort eller faktura (check/banköverföring)

Alla inköp med kreditkort eller månadsfaktura har en 30-dagars kvarhållningsperiod för att säkerställa att medel samlas in från kunden.

| Händelse | Description | Rapporteringssynlighet | Tidsinställning* |
| --- | --- | --- | --- |
| Användning eller transaktionsmånad | Kunden använder eller köper en tjänst. | [Instrumentpanel](/azure/marketplace/partner-center-portal/usage-dashboard) för [användning eller](/azure/marketplace/partner-center-portal/orders-dashboard) beställning | **Månad 1** |
| Faktura som betalas av kunden | Fastställa total användning, totalt transaktionsvärde och kund betalar faktura | [Instrumentpanel](/azure/marketplace/partner-center-portal/usage-dashboard) för [användning eller](/azure/marketplace/partner-center-portal/orders-dashboard) beställning | **Månad 2** |
| Utsänd utbetalning | Fastställa myndighetsavgifter och utbetalningsintäkter | Markerat som Obearbetat i transaktionshistoriken på [utbetalningsutdraget](payout-statement.md) | **Månad 2** |
| 30-dagars innehavsperiod | Se till att medel, möjliga återbetalningar och återbetalningar görs | Markerat som Obearbetat i transaktionshistoriken på [utbetalningsutdraget](payout-statement.md) | **Månad 3** |
| Förbereda utbetalning | Intäkter förbereds för månatlig betalning | Markerat som Kommande i transaktionshistoriken i [utbetalningsutdraget](payout-statement.md) | **Månad 4 (första veckan)** |
| **Utbetalningen har skickats** | **Betalningen skickas till utgivaren** | **Markerat som Skickat i transaktionshistoriken och i avsnittet Betalningar i [utbetalningsutdrag](payout-statement.md)** | **Månad 4 (senast den 15:e)** |
|

\* Utbetalningsdatumet är i Pacific Standard Time (PST).

:::image type="content" source="images/payouts/timeline-credit-card-invoice.png" alt-text="Tidslinje för betalningar för kreditkorts- och fakturakunder.":::

## <a name="process-for-customer-non-payment"></a>Process för utebliven kundbetalning

I sällsynta fall kan Microsoft inte samla in betalningar från kunder för sina köp på den kommersiella marknadsplatsen. När en kund inte betalar Microsoft enligt sitt faktureringsschema påbörjar vi insamlingsprocessen. Den här processen tar cirka fyra månader och omfattar beständig kommunikation från Microsoft. Om betalningen inte tas emot i slutet av den här processen skriver Microsoft av beloppen som osamlade.

Enligt utbetalningsprocessen som formuleras här kanske Microsoft redan har betalat ut pengar till utgivare (du) som i slutänden inte går att samla in. Därför har vi en process för att stämma av dessa mängder. För att säkerställa att du har en varning om att din (redan mottagna) betalning kan stämmas av, får du ett meddelande när en kund är i samlingsprocessen och inköpen sannolikt skrivs av.

Microsoft kommer att få tillbaka alla utbetalningar som redan har betalats till dig med någon av följande metoder: (1) Microsoft kan subtrahera de obetalt beloppen från framtida utbetalningar; Om till exempel 1 000 USD i utbetalning betraktas som osamlade och skrivs av, kommer dina framtida utbetalningar att uppsnaftas tills de 1 000 USD har återställts eller (2) Microsoft kan begära en återbetalning eller fakturautgivare för eventuella oupptäckta belopp.

Följande schema är ett exempel:

| Händelse | Ungefärligt datum* | Partnersynlighet |
| --- | --- | --- |
| Exempel på utbetalningsdatum | 10/15/2020 | Markerat som **skickat i** transaktionshistoriken och i avsnittet Betalningar i utbetalningsinstrumentpanelen |
| <font color="red">Om kunden inte betalar Microsoft</font> | 12/2/2020 – 12/5/2020 | Ingen ändring, samma som ovan |
| Kunden får sin första e-postadress för försenad betalning | 12/6/2020 | Ingen |
| Kunden får regelbundna e-postmeddelanden om ökande angelägenhetsgrad | 12/7/2020 – 1/31/2021 | Ingen |
| Utgivaren meddelas om troligen en nedskrivning | 1/7/2021 | E-postmeddelande som skickas till utgivaren om att kunden ännu inte har skickat betalningen. Transaktions-ID och belopp i dollar ingår. |
| Kunden får ett meddelande om uppsägning | 2/1/2021 | Ingen |
| Insamlingsprocessen avslutas/medel skrivs av | 2/15/2021 | E-postmeddelande som skickats till utgivaren om att medel har skrivits av. Transaktions-ID och belopp i dollar ingår. |
| Utbetalning dras av | 3/1/2021 | Utgivaren ser en negativ transaktion i partnercentrets utbetalningsutdrag |
| Utbetalningen är indragen | 3/15/2021 | Framtida utbetalningar visas i partnercentrets utbetalningsutdrag. Utgivaren får ingen betalning förrän saldot inte längre är negativt.  |
|||

\* Utbetalningsdatumet är i Pacific Standard Time (PST).

## <a name="number-of-days-for-payments-to-reach-a-payout-account"></a>Antal dagar som betalningar ska nå ett utbetalningskonto

Vi skickar vanligtvis en betalning som förfaller under en viss månad den 15:e dagen i den månaden, men det tar en annan tid för betalningen att nå ditt konto. Antalet dagar beror på vilken betalningsmetod vi använder för ditt konto, enligt beskrivningen nedan.

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
