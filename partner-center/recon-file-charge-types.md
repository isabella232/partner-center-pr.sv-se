---
title: Debiteringstyper i avstämningsfiler
ms.topic: article
ms.date: 06/05/2020
description: Identifiera typer av avgifter (till exempel licensbaserade, användningsbaserade och en-gång), krediter och rabatter i Partner Center-avstämningsfiler.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 5a1f45de59fc9dac6a443bb8a14c3a80b36ba3f7
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 05/13/2021
ms.locfileid: "109855887"
---
# <a name="understand-the-different-charge-types-in-partner-center-reconciliation-files"></a>Förstå de olika avgiftstyperna i Avstämningsfiler för Partnercenter

**Gäller för:** Partner Center-| Partnercenter för Microsoft Cloud for US Government

**Lämpliga roller:** Administratörsagent | Faktureringsadministratörskonto | Global administratör

I den här artikeln beskrivs mappningarna mellan ett fakturaavsnitt och associerade avgiftstyper som kan finnas i avstämningsfilen. Din faktura innehåller en sammanfattning av avgifterna. Avstämningsfilen innehåller en detaljerad analys av radobjekttransaktioner, inklusive avgiftstyper. Mer information om avstämningsfiler finns i [använda avstämningsfiler](use-the-reconciliation-files.md).

Både [användningsbaserade avstämningsfiler](usage-based-recon-files.md) [och licensbaserade](license-based-recon-files.md) avstämningsfiler visar endast användningsrelaterade transaktioner och avgifter (förbrukade enheter och relaterade avgifter).

> [!NOTE]
> Krediter, rabatter eller återbetalningar som visas på fakturan som Justeringar visas inte i **avstämningsfilen.**

## <a name="map-charge-types-to-invoice-charges"></a>Mappa avgiftstyper till fakturaavgifter

Om du vill korsreferensa avgiftsbeloppen mellan din faktura och avstämningsfil använder du filteralternativen i Microsoft Excel. Filtrera efter avgiftstyper i avstämningsfilen för att mappa fakturade avgifterna till en uppsättning uppdelningar av avgifter i avstämningsfilen.

## <a name="license-based-charges"></a>Licensbaserade avgifter

Om du vill mappa dessa licensbaserade avgifter till din faktura summerar **du kolumnen Amount** från den licensbaserade filen.

| Avgiftsbeskrivning (kolumnen ChargeType i avstämningsfilen) | Förklaring av avgifter |
| ------------------------------------------------------------- | ------------------ |
| Aktiveringsavgift | Det belopp som debiteras kunden när de använder prenumerationen efter köpet. |
| Avbokningsavgift | Återbetalade avgifter till kunden när associerade licenser ändras. |
| Avbryta instansprorate | Avgiftsberäknade avgifter avbröts när en kund med månadsprenumeration pausade och associerade licenser ändrades under samma månad. |
| Cykelavgift | Periodiska avgifter för en prenumeration. |
| Cykelinstansprorate | Taxerade avgifter som utvärderas från kunden när associerade licenser ändras. |
| Betala avgifter när du avbryter | Återbetalas i procent för oanvänd del av tjänsten vid annullering. |
| Prorate fees when convert away from current offering (Prorate-avgifter när de konverteras bort från det aktuella erbjudandet) | Räknade avgifter efter att ha konverterat bort från den aktuella månadsprenumerationen till en årlig prenumeration. |
| Betala avgifter när du konverterar till ett nytt erbjudande | Prorerade avgifter efter konvertering av en månatlig prenumeration till en ny årsprenumeration. |
| Betala avgifter vid köp | Avgiftstypen för en prenumeration när du använder både månatlig eller årlig fakturering. |
| Betala avgifter vid förnyelse | Prorerade avgifter vid prenumerationsförnyelse. |
| Förnya avgift | Avgift för att förnya en prenumeration |
| Prorate fees when activate (Gå ut med avgifter när du aktiverar) | Fakturerade avgifter från aktivering till slutet av faktureringsperioden. |

## <a name="one-time-charges"></a>Avgifter för en gång

Om du vill mappa dessa engångsavgifter till din faktura summerar **du kolumnen Amount** från den licensbaserade filen.

| Avgiftsbeskrivning (kolumnen ChargeType i avstämningsfilen) | Förklaring av avgifter |
| ------------------------------------------------------------- | ------------------ |
| Ny | Används när ett nytt köp skapas. |
| addQuantity | Används i både återbetalningen av det ursprungliga köpet och den nya kvantiteten efter en ökning. |
| removeQuantity | Används i både återbetalningen av det ursprungliga köpet och den nya kvantiteten efter en minskning. |
| Avbryt | Används när en prenumeration avbryts. |
| Konvertera | Används när en licens uppgraderas men antalet licenser förblir oförändrat. |

## <a name="usage-charges"></a>Avgifter för användning

Om du vill mappa dessa användningsavgifter till din faktura summerar du kolumnen **PretaxCharges** från den användningsbaserade filen.

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

Om du vill mappa licensbaserade rabatter till din faktura **summerar du kolumnen TotalOtherDiscount** från den licensbaserade filen.

*Licensbaserade rabatter kan tillämpas på flera avgiftstyper.*
