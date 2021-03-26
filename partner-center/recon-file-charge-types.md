---
title: Debiteringstyper i avstämningsfiler
ms.topic: article
ms.date: 06/05/2020
description: Identifiera typer av avgifter (till exempel licensbaserade, användnings och engångs), krediter och rabatter i filer för partner Center-avstämning.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: ba42ac5beb28a3cf819c54a86385fb79853cdcd0
ms.sourcegitcommit: 700150044ea4f1a0b96cb4caeb97d7197da29ef6
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/25/2021
ms.locfileid: "105549234"
---
# <a name="understand-the-different-charge-types-in-partner-center-reconciliation-files"></a>Förstå de olika debiterings typerna i filer för partner Center-avstämning

**Gäller för**

- Partner Center för Microsoft myndighets moln

**Lämpliga roller**

- Administratörs agent
- Faktureringsadministratör
- Global administratör

I den här artikeln beskrivs mappningarna mellan avsnittet faktura och tillhör ande avgifts typer som kan finnas i avstämnings filen. Fakturan innehåller en sammanfattning av avgifter. Din avstämnings fil innehåller en detaljerad uppdelning av rad artikel transaktioner, inklusive avgifts typer. Mer information om avstämnings filer finns i [så här använder du avstämnings filer](use-the-reconciliation-files.md).

Både [användnings avstämnings filer](usage-based-recon-files.md) och [licensbaserade avstämnings filer](license-based-recon-files.md) visar bara användnings-relaterade transaktioner och avgifter (förbrukade enheter och relaterade avgifter).

> [!NOTE]
> En eller flera krediter, rabatter eller åter betalningar som visas på fakturan när **justeringar** inte visas i avstämnings filen.

## <a name="map-charge-types-to-invoice-charges"></a>Mappa avgifts typer till faktura avgifter

Använd filter alternativen i Microsoft Excel för att välja mellan referenser mellan fakturor och avstämnings fil. Filtrera efter debiterings typer i avstämnings filen för att mappa faktura avgifterna till en uppsättning med debiterings nivåer i avstämnings filen.

## <a name="license-based-charges"></a>Licensbaserade avgifter

För att mappa dessa licensbaserade avgifter till din faktura, summerar du kolumnen **mängd** från den licensierade filen.

| Avgifts Beskrivning (ChargeType-kolumnen i avstämnings filen) | Avgifts förklaring |
| ------------------------------------------------------------- | ------------------ |
| Aktiverings avgift | Det belopp som debiteras kunden när de använder prenumerationen efter köpet. |
| Annullera avgift | Proportionella avgifter som återbetalas till kunden när tillhör ande licenser ändras. |
| Avbryt instans prograden | Proportionella avgifter annulleras när kunden med en månatlig prenumeration har inaktiverat prenumerationen och tillhör ande licenser har ändrats inom samma månad. |
| Cykel avgift | Periodiska avgifter för en prenumeration. |
| Prograder för cykel instans | Beräknad kostnad som bedöms från kunden när tillhör ande licenser ändras. |
| Betala avgifter när du avbryter | Proportionellt åter betalning för oanvänd del av tjänst vid annullering. |
| Prorate-avgifter vid omvandling bort från aktuellt erbjudande | Proportionella avgifter efter konvertering från den aktuella månads prenumerationen till en års prenumeration. |
| Protaxa-avgifter vid konvertering till ett nytt erbjudande | Proportionella avgifter efter konvertering av en månatlig prenumeration till en ny års prenumeration. |
| Betala avgifter vid köp | Avgifts typen för en prenumeration när du använder både månatlig eller årlig fakturering. |
| Protaxa-avgift vid förnyelse | Debiterade avgifter vid förnyelse av prenumerationen. |
| Förnya avgift | Avgift för att förnya en prenumeration |
| Taxa för avgifter vid aktivering | Debiteras avgifter från aktivering till slutet av fakturerings perioden. |

## <a name="one-time-charges"></a>Engångs kostnader

Om du vill mappa dessa engångs kostnader till din faktura, summerar du kolumnen **mängd** från den licensierade filen.

| Avgifts Beskrivning (ChargeType-kolumnen i avstämnings filen) | Avgifts förklaring |
| ------------------------------------------------------------- | ------------------ |
| Ny | Används när ett nytt inköp skapas. |
| addQuantity | Används både i åter betalningen av det ursprungliga köpet och den nya kvantiteten efter en ökning. |
| removeQuantity | Används både i åter betalningen av det ursprungliga köpet och den nya kvantiteten efter en minskning. |
| Avbryt | Används när en prenumeration avbryts. |
| Konvertera | Används när en licens uppgraderas men antalet licenser förblir oförändrat. |

## <a name="usage-charges"></a>Avgifter för användning

Om du vill mappa dessa användnings kostnader till din faktura, summerar du kolumnen **PretaxCharges** från den användnings filen.

| Avgifts Beskrivning (ChargeType-kolumnen i avstämnings filen) | Avgifts förklaring |
| ------------------------------------------------------------- | ------------------ |
| Utvärdera användnings avgiften när du avbryter | Åtkomst användnings avgift vid annullering för obetald användning under den aktuella fakturerings perioden. |
| Utvärdera användnings avgiften för den aktuella cykeln | Åtkomst användnings avgift för den aktuella fakturerings perioden. |

### <a name="credits"></a>Krediter

För att mappa dessa krediter till din faktura:

- Summera **TotalForCustomer** från den licensierade filen.
- Summera kolumnen **PostTaxTotal** från den Usage-baserade filen.

| Avgifts Beskrivning (ChargeType-kolumnen i avstämnings filen) | Avgifts förklaring |
| ------------------------------------------------------------- | ------------------ |
| Förskjut ett linje objekt | Delvis eller fullständig åter betalning till ett rad objekt, inklusive skatt. |

### <a name="usage-based-discounts"></a>Användnings rabatter

Om du vill mappa dessa användnings rabatter till din faktura, summerar du kolumnen **PretaxCharges** från den användnings filen.

| Avgifts Beskrivning (ChargeType-kolumnen i avstämnings filen) | Avgifts förklaring |
| ------------------------------------------------------------- | ------------------ |
| Aktiverings rabatt | Rabatt som tillämpas när prenumerationen aktive ras. |
| Cykel rabatt | Rabatt som tillämpas på periodiska kostnader. |
| Förnya rabatt | Rabatt som tillämpas när prenumerationen förnyas. |
| Avbryt rabatt | Avgifter som tillämpas när rabatter annulleras. |

### <a name="license-based-discounts"></a>Licensbaserade rabatter

Om du vill mappa licensbaserade rabatter till din faktura, summerar du kolumnen **TotalOtherDiscount** från den licensierade filen.

*Licensbaserade rabatter kan tillämpas på flera debiterings typer.*
