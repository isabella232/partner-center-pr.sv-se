---
title: Debiteringstyper i avstämningsfiler
ms.topic: article
ms.date: 06/05/2020
description: Identifiera typer av avgifter (till exempel licensbaserade, användningsbaserade och en-gång), krediter och rabatter i Partner Center-avstämningsfiler.
ms.service: partner-dashboard
ms.subservice: partnercenter-billing
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 8e41210f6eedbea36e72d5d4408fd102e7f7d3289f3f1a7c0ee635fe226aa427
ms.sourcegitcommit: 121f1b9cbd88faeba60dc9b475f9c0647cdc933c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/06/2021
ms.locfileid: "115688904"
---
# <a name="understand-the-different-charge-types-in-partner-center-reconciliation-files"></a>Förstå de olika avgiftstyperna i Avstämningsfiler för Partnercenter

**Gäller för:** Partner Center-| Partnercenter för Microsoft Cloud for US Government

**Lämpliga roller:** Administratörsagent | Faktureringsadministratörskonto | Global administratör

I den här artikeln beskrivs mappningarna mellan ett fakturaavsnitt och associerade avgiftstyper som kan finnas i avstämningsfilen. Din faktura innehåller en sammanfattning av avgifterna. Avstämningsfilen innehåller en detaljerad analys av radobjekttransaktioner, inklusive avgiftstyper. Mer information om avstämningsfiler finns i [använda avstämningsfiler](use-the-reconciliation-files.md).

Både [användningsbaserade avstämningsfiler](usage-based-recon-files.md) [och licensbaserade](license-based-recon-files.md) avstämningsfiler visar endast användningsrelaterade transaktioner och avgifter (förbrukade enheter och relaterade avgifter).

> [!NOTE]
> Krediter, rabatter eller återbetalningar som visas på fakturan som Justeringar visas inte i **avstämningsfilen.**

## <a name="map-charge-types-to-invoice-charges"></a>Mappa avgiftstyper till fakturaavgifter

Om du vill korsreferensa avgiftsbeloppen mellan din faktura och avstämningsfilen använder du filteralternativen i Microsoft Excel. Filtrera efter avgiftstyper i avstämningsfilen för att mappa fakturade avgifterna till en uppsättning uppdelningar av avgifter i avstämningsfilen.

## <a name="license-based-charges"></a>Licensbaserade avgifter

Om du vill mappa dessa licensbaserade avgifter till din faktura **summerar du** kolumnen Amount från den licensbaserade filen.

| Avgiftsbeskrivning (kolumnen ChargeType i avstämningsfilen) | Förklaring av avgifter |
| ------------------------------------------------------------- | ------------------ |
| Aktiveringsavgift | Det belopp som debiteras kunden när de använder prenumerationen efter köpet. |
| Avbokningsavgift | Prorerade avgifter återbetalas till kunden när associerade licenser ändras. |
| Avbryta instansprorate | Prorerade avgifter avbryts när en prenumeration har inaktiverats för en kund med en månadsprenumeration och associerade licenser har ändrats under samma månad. |
| Cykelavgift | Periodiska avgifter för en prenumeration. |
| Cykelinstansprorate | Taxerade avgifter som utvärderas från kunden när associerade licenser ändras. |
| Prorate fees when cancel ( Ställ in avgifter vid avbokning) | Återbetalas i procent för oanvänd del av tjänsten vid annullering. |
| Räkna ut avgifter när du konverterar bort från det aktuella erbjudandet | Prorerade avgifter efter att ha konverterat bort från den aktuella månadsprenumerationen till en årlig prenumeration. |
| Prorate fees when convert to a new offering (Prorate-avgifter vid konvertering till ett nytt erbjudande) | Prorated charges after converting a monthly subscription to a new annual subscription. |
| Prorate fees when purchase (Prorate-avgifter vid köp) | Avgiftstypen för en prenumeration när du använder både månads- eller årsfakturering. |
| Avgifter för prorate vid förnyelse | Prorerade avgifter vid prenumerationsförnyelse. |
| Förnya avgift | Avgift för att förnya en prenumeration |
| Prorate fees when activate (Prorate-avgifter vid aktivering) | Fakturerade avgifter från aktivering till slutet av faktureringsperioden. |

## <a name="one-time-charges"></a>Avgifter för en gång

Om du vill mappa dessa engångsavgifter till din faktura summerar **du kolumnen Amount** från den licensbaserade filen.

| Avgiftsbeskrivning (kolumnen ChargeType i avstämningsfilen) | Förklaring av avgifter |
| ------------------------------------------------------------- | ------------------ |
| ny | Används när ett nytt köp skapas. |
| förnya | Används när en prenumeration förnyas efter slutet av perioden. |
| addQuantity | Används i både återbetalningen av det ursprungliga köpet och den nya kvantiteten efter en ökning. |
| removeQuantity | Används i både återbetalningen av det ursprungliga köpet och den nya kvantiteten efter en minskning. |
| cancelImmediate | Används när en prenumeration avbryts. |
| omvandla | Används när en licens uppgraderas. |
| customerCredit | Används när krediter (t.ex. Azure, serviceavtal osv.) ges mot en transaktion. |

## <a name="usage-charges"></a>Avgifter för användning

Om du vill mappa dessa användningsavgifter till din faktura summerar du **kolumnen PretaxCharges** från den användningsbaserade filen.

| Avgiftsbeskrivning (kolumnen ChargeType i avstämningsfilen) | Förklaring av avgifter |
| ------------------------------------------------------------- | ------------------ |
| Utvärdera användningsavgiften när du avbryter | Åtkomstanvändningsavgift vid annullering för obetalt användning under den aktuella faktureringsperioden. |
| Utvärdera användningsavgiften för den aktuella cykeln | Åtkomstanvändningsavgift för den aktuella faktureringsperioden. |

### <a name="credits"></a>Krediter

Så här mappar du dessa krediter till din faktura:

- Summera **TotalForCustomer** från den licensbaserade filen.
- Summera **kolumnen PostTaxTotal** från den användningsbaserade filen.

| Avgiftsbeskrivning (kolumnen ChargeType i avstämningsfilen) | Förklaring av avgifter |
| ------------------------------------------------------------- | ------------------ |
| Förskjut ett radobjekt | Partiell eller hel återbetalning till ett radobjekt, inklusive skatter. |

### <a name="usage-based-discounts"></a>Användningsbaserade rabatter

Om du vill mappa dessa användningsbaserade rabatter till din faktura summerar du kolumnen **PretaxCharges** från den användningsbaserade filen.

| Avgiftsbeskrivning (kolumnen ChargeType i avstämningsfilen) | Förklaring av avgifter |
| ------------------------------------------------------------- | ------------------ |
| Aktiveringsrabatt | Rabatt som tillämpas när prenumerationen aktiveras. |
| Cykelrabatt | Rabatt som tillämpas på periodiska avgifter. |
| Förnya rabatt | Rabatt som tillämpas när prenumerationen förnyas. |
| Avbryta rabatt | Avgifter som tillämpas när rabatter avbryts. |

### <a name="license-based-discounts"></a>Licensbaserade rabatter

Om du vill mappa licensbaserade rabatter till din faktura summerar du **kolumnen TotalOtherDiscount** från den licensbaserade filen.

*Licensbaserade rabatter kan tillämpas på flera olika avgiftstyper.*
