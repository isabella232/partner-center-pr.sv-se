---
title: Fakturering för engångsinköp & återkommande inköp
ms.topic: article
ms.date: 05/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Faktureringsexempel för Partnercenter för engångsköp och välj återkommande inköp – när du köper prenumerationer lägger du till fler prenumerationer, lägger till eller tar bort licenser.
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: a26b6e5299c5186959612e622808161ca0f7f7c2
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 05/19/2021
ms.locfileid: "110148626"
---
# <a name="partner-center-billing-scenarios-for-one-time-and-select-recurring-purchases"></a>Faktureringsscenarier i Partnercenter för engångsköp och välj återkommande inköp

**Lämpliga roller:** Administratörsagent | Faktureringsadministratörskonto | Supportagent för | Försäljningsagent

Det här är [vanliga faktureringsscenarier.](common-billing-scenarios.md) 

## <a name="purchase-a-subscription-and-add-a-license-on-the-same-day"></a>Köpa en prenumeration och lägga till en licens samma dag

I scenario 1 köper du en prenumeration den 11 juni till ett enhetspris på 4 USD. Senare samma dag köper du en annan av samma prenumeration till samma pris.

Rekognoseringsfilen innehåller följande:

- 4 USD för serviceperioden 10 juni – 9 juli.
- 4,00 USD fakturerade omfakturering för tjänstperioden 11 juni – 11 juni. Det här är den period då du hade en licens. Beräkning = (månadsvis pris/totalt antal dagar i tjänstperioden) x dagar i den prorated serviceperioden x antalet licenser = (4/30) x 30 x 1 = 4,00.
- 8,00 USD fakturerade omfakturering för tjänstperioden 10–9 juli. Det här är den period då du hade två licenser. Beräkning = (4/30) x 30 x 2 = 8,00.

|**Inköpsdatum**   |**Avgiftsstart** |**Avgiftsslut**  |**Enhetspris**  |**Kvantitet**  |**Amount** |**Kostnadstyp** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|6/11/2019      |6/10/2019   |7/09/2019         |4 USD                |1                 |4 USD            |Ny         |
|6/11/2019     | 6/10/2019    |7/09/2019        |4 USD        |1        | -$4       |addQuantity           |
|6/11/2019     | 6/10/2019    |7/09/2019        |4 USD        | 2      |8 USD         |addQuantity           |

## <a name="purchase-a-subscription-and-add-more-subscriptions-later"></a>Köpa en prenumeration och lägga till fler prenumerationer senare

I scenario 2 köper du en prenumeration den 11 juni till ett enhetspris på 4 USD, och den 12 juni köper du en annan prenumeration för samma produkt till samma pris.

Rekognoseringsfilen innehåller följande:

- 4 USD för serviceperioden 10 juni – 9 juli.
- 3,87 USD fakturerade omfakturering för tjänstperioden 11 juni – 12 juni. Det här är den period då du hade en licens. Beräkning = (månadsvis pris/totalt antal dagar i tjänstperioden) x dagar i den prorated serviceperioden x antalet licenser = (4/30) x 29 x 1 = 3,87.
- 7,74 USD fakturerade 7,74 USD för tjänsteperioden 12–9 juli. Det här är den period då du hade två licenser. Beräkning = (4/30) x 29 x 2 = 7,74.

|**Inköpsdatum**   |**Avgiftsstart** |**Avgiftsslut**  |**Enhetspris**  |**Kvantitet**  |**Amount** |**Kostnadstyp** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|2019-06-11 (du har en licens)     |6/10/2019   |7/09/2019         |4 USD         |1        |4 USD            |Ny         |
|6/12/2019     | 6/10/2019    |7/09/2019        |4 USD        |1        | -$3,87       |addQuantity           |
|6/12/2019     | 6/10/2019    |7/09/2019        |4 USD        | 2      |7,74 USD       |addQuantity           |

## <a name="purchase-a-subscription-and-remove-a-license-on-the-same-day"></a>Köpa en prenumeration och ta bort en licens samma dag

I scenario 3 köper du två prenumerationer för samma produkt den 11 juni till ett enhetspris på 4 USD. Senare samma dag tar du bort en av licenserna.  

Rekognoseringsfilen innehåller följande:

- Faktura på 8 USD för två licenser för tjänstperioden 10 juni – 9 juli.
- 8,00 USD fakturerade omfakturering för tjänstperioden 11 juni – 11 juni. Det här är den period då du hade två licenser. Beräkning = (månadsvis pris/totalt antal dagar i tjänstperioden) x dagar i den prorrerade serviceperioden x antalet licenser = (4/30) x 30 x 2 = 8,00.
- 4,00 USD fakturerade omfakturering för tjänstperioden 11 juni – 9 juli. Det här är den period då du hade en licens. Beräkning = (4/30) x 30 x 1 = 4,00.

|**Inköpsdatum**   |**Avgiftsstart** |**Avgiftsslut**  |**Enhetspris**  |**Kvantitet**  |**Amount** |**Kostnadstyp** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|6/11/2019      |6/10/2019   |7/09/2019         |4 USD                |2                 |8 USD            |Ny         |
|6/11/2019     | 6/10/2019    |7/09/2019        |4 USD        |2        | -$8       |removeQuantity           |
|6/11/2019     | 6/10/2019    |7/09/2019        |4 USD        | 1      |4 USD         |removeQuantity           |

## <a name="purchase-a-subscription-and-remove-licenses-later"></a>Köpa en prenumeration och ta bort licenser senare

I scenario 4 köper du två prenumerationer den 11 juni till ett enhetspris på 4 USD och den 12 juni tar du bort en av licenserna.

Rekognoseringsfilen innehåller följande:

- 8 USD för serviceperioden 10 juni – 9 juli.
- 7,74 USD fakturerade omfakturering i procent för tjänstperioden 11 juni – 12 juni. Det här är den period då du hade två licenser. Beräkning = (månadsvis pris/totalt antal dagar i tjänstperioden) x dagar i den prorerade tjänstperioden x antalet licenser = (4/30) x 29 x 2 = 7,74.
- 3,87 USD fakturerade omfakturering för tjänstperioden 12 juni – 9 juli. Det här är den period då du hade en licens. Beräkning = (4/30) x 29 x 1 = 3,87.

|**Inköpsdatum**   |**Avgiftsstart** |**Avgiftsslut**  |**Enhetspris**  |**Kvantitet**  |**Amount** |**Kostnadstyp** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|2019-06-11 (du har två licenser)     |6/10/2019   |7/09/2019         |4 USD         |2        |8 USD       |Ny       |
|6/12/2019     | 6/10/2019    |7/09/2019        |4 USD        |2        | -$7,74       |removeQuantity           |
|2019-06-12 (du har en licens)    | 6/10/2019    |7/09/2019   |4 USD    |1      |3,87 USD    |removeQuantity |

## <a name="next-steps"></a>Nästa steg

- [Exempel på månatliga faktureringsscenarier för nya prenumerationer, ändring av licensbelopp eller indragningar](common-billing-scenarios-monthly.md)