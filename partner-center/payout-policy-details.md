---
title: Utbetalnings scheman och princip information – Azure Marketplace
description: Läs mer om information som rör utbetalnings principer för kommersiella Marketplace, inklusive scheman och återkoppling.
ms.service: marketplace
ms.subservice: partnercenter-marketplace-publisher
ms.topic: conceptual
author: eunjkim520
ms.author: eunjkim
ms.date: 11/06/2020
ms.openlocfilehash: 9c03878ec69b9df06795054464ef7f76e038e780
ms.sourcegitcommit: cc30a06abe55b9da32177a24e74bfd6fc7d8bbb9
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 11/12/2020
ms.locfileid: "94531995"
---
# <a name="payout-schedules-and-policy-details"></a>Utbetalnings scheman och princip information

I den här artikeln beskrivs Microsofts utbetalnings process, ett utbetalnings schema, var du hittar status för en utbetalning och processen för kund utebliven betalning.

## <a name="payment-schedules"></a>Betalnings scheman

I följande avsnitt beskrivs vår utbetalnings process för **Enterprise-avtal** och **kredit kort/faktura** transaktioner.

### <a name="enterprise-agreement-transactions"></a>Enterprise-avtal transaktioner

När en kund köper en produkt från Microsoft AppSource eller Azure Marketplace med hjälp av sina befintliga Microsoft-Enterprise-avtal för transaktioner, kommer vi att utfärda utbetalningar i nästa utbetalnings cykel 30 dagar efter kund faktura. Transaktioner där en kund använder ett kredit kort har en 30-dagars företags period innan utbetalning.

En utbetalning inträffar ofta innan Microsoft samlar in betalning från kunden. Se [processen för kund ej inbetalning](#process-for-customer-non-payment) nedan för de åtgärder som vi vidtar om kunden inte betalar Microsoft men vi redan har utfärdat en utbetalning.

| Händelse | Beskrivning | Rapporterings synlighet | Ordning |
| --- | --- | --- | --- |
| Användning eller månad för transaktion | Kunden använder eller köper en tjänst. | [Användnings](/azure/marketplace/partner-center-portal/usage-dashboard) -eller [order](/azure/marketplace/partner-center-portal/orders-dashboard) instrument panel | **Månad 1** |
| Inköps order skapas | Fastställ total användning, totalt antal transaktioner | [Användnings](/azure/marketplace/partner-center-portal/usage-dashboard) -eller [order](/azure/marketplace/partner-center-portal/orders-dashboard) instrument panel | **Månad 2** |
| ISV-betalning skapas | Fastställa utbetalnings avgiften och utbetalnings intäkterna | Markerade som obearbetade i transaktions historiken för utbetalnings instruktionen | **Månad 3 (1: e veckan)** |
| Förbered utbetalning | Intäkterna är för beredda för månatlig betalning | Markerat som kommande i transaktions historik i utbetalnings instruktionen | **Månad 3 (1: e veckan)** |
| **Utbetalnings datum** | **Betalningen skickas till utgivaren** | **Markerat som skickat i transaktions historik och i avsnittet betalningar i utbetalnings instruktionen** | **Månad 3 (senast den 15)** |
| Faktura betald per kund | Microsoft samlar in betalning från kunden | Ingen ändring | **Månad 4 till 12** |
|

\* Utbetalnings datumet är i Pacific, normal tid (PST).

### <a name="customers-who-pay-using-credit-card-or-invoice"></a>Kunder som betalar med kredit kort eller faktura

Alla inköp med ett kredit kort eller en månads faktura har en 30-dagars period för att säkerställa att fonder samlas in från kunden.

| Händelse | Beskrivning | Rapporterings synlighet | Ordning |
| --- | --- | --- | --- |
| Användning eller månad för transaktion | Kunden använder eller köper en tjänst. | [Användnings](/azure/marketplace/partner-center-portal/usage-dashboard) -eller [order](/azure/marketplace/partner-center-portal/orders-dashboard) instrument panel | **Månad 1** |
| Faktura betald per kund | Fastställer total användning, totalt transaktions värde och kund betalar faktura | [Användnings](/azure/marketplace/partner-center-portal/usage-dashboard) -eller [order](/azure/marketplace/partner-center-portal/orders-dashboard) instrument panel | **Månad 2** |
| ISV-betalning skapas | Fastställa utbetalnings avgiften och utbetalnings intäkterna | Markerade som obearbetade i transaktions historiken för utbetalnings instruktionen | **Månad 2** |
| 30 dagars anläggnings period | Se till att insamling av fonder, eventuell åter betalning och åter betalnings förfrågningar | Markerade som obearbetade i transaktions historiken för utbetalnings instruktionen | **Månad 3** |
| Förbered utbetalning | Intäkterna är för beredda för månatlig betalning | Markerat som kommande i transaktions historik i utbetalnings instruktionen | **Första veckan i månad 4** |
| **Utbetalnings datum** | **Betalningen skickas till utgivaren** | **Markerat som skickat i transaktions historik och i avsnittet betalningar i utbetalnings instruktionen** | **Månad 4 (senast den 15)** |
|

\* Utbetalnings datumet är i PST (Pacific, normal tid).

## <a name="process-for-customer-non-payment"></a>Process för ej betalnings kund

I sällsynta fall kan Microsoft inte samla in betalningar från kunder för sina kommersiella marknads marknads inköp. När en kund inte betalar Microsoft enligt deras fakturerings schema påbörjar vi samlings processen. Den här processen tar cirka fyra månader och inbegriper beständig kommunikation från Microsoft. Om betalningen inte tas emot i slutet av den här processen, skriver Microsoft ut medlen som ej insamlade.

Efter utbetalnings processen som har framställts här kan Microsoft redan betala ut pengar till utgivare (du) som slutligen inte kan samlas in. Därför har vi en process för att stämma av dessa belopp. För att se till att du har en varning om att din (redan inlevererad) betalning kan stämmas av får du ett meddelande när en kund befinner sig i Inkasso processen och köp kan förmodligen skrivas av.

Microsoft kommer att koppla tillbaka eventuella utbetalningar som redan betalats till dig med någon av följande metoder: (1) Microsoft kan subtrahera de obetalda beloppen från framtida utbetalningar. om till exempel $1 000 i utbetalningar betraktas som ej kan samlas in och skrivs av, kommer dina framtida utbetalningar att bli kvar tills $1 000 återställs eller (2) Microsoft kan begära en åter betalning eller faktura utgivare för alla insamlade belopp.

Följande är ett exempel schema:

| Händelse | Ungefärligt datum * | Partner synlighet |
| --- | --- | --- |
| Exempel på utbetalnings datum | 10/15/2020 | Markerat som **skickat** i transaktions historik och i avsnittet betalningar i instrument panelen för utbetalning |
| <font color="red">Om kunden inte betalar Microsoft</font> | 12/2/2020 – 12/5/2020 | Ingen ändring, samma som ovan |
| Kunden får ett e-postmeddelande om betalning för första sent | 12/6/2020 | Inget |
| Kunden får regelbundna e-postmeddelanden med ökande angelägenhets grad | 12/7/2020 – 1/31/2021 | Inget |
| Utgivaren har meddelats att skriva av är troligt vis | 1/7/2021 | E-postmeddelande som skickas till utgivaren om att deras kunder ännu inte har skickat någon betalning. Transaktions-ID och dollar belopp ingår. |
| Kund mottar uppsägnings meddelande | 2/1/2021 | Inget |
| Samlings processens slut/medel skrivs av | 2/15/2021 | E-postmeddelande som skickas till utgivare som fonder har skrivits av. Transaktions-ID och dollar belopp ingår. |
| Utbetalningen dras av | 3/1/2021 | I Publisher visas en negativ transaktion i Partner Center utbetalnings instruktion |
| Utbetalningen nekas | 3/15/2021 | Framtida utbetalningar visas i utbetalnings instruktionen för partner Center. Utgivare får ingen betalning förrän saldot inte längre är negativt.  |
|||

\* Utbetalnings datumet är i PST (Pacific, normal tid).

## <a name="number-of-days-for-payments-to-reach-a-payout-account"></a>Antal dagar för betalningar för att uppnå ett utbetalnings konto

Vi skickar vanligt vis ut alla betalningar som förfaller under en månad den 15: e dagen i månaden, men det tar ytterligare tid för betalningen att komma åt ditt konto. Antalet dagar beror på betalnings metoden som vi använder för ditt konto, enligt beskrivningen nedan.

> [!NOTE]
> De dagar som visas nedan är ungefärliga; alla betalningar kan ta längre eller kortare tid att komma åt ditt konto.

| Betalningsmetod     | Antal dagar för att uppnå utbetalnings konto     |
|--------------------|--------------------------------------------|
| PayPal             | 1 arbets dag                             |
| ACH/SEPA           | 2-3 arbets dagar                          |
| Överföring av överföring      | 7-10 arbets dagar                         |
|

## <a name="next-steps"></a>Nästa steg

Läs mer om [skatte information](tax-details-marketplace.md).
