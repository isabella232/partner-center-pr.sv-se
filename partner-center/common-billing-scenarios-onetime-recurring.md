---
title: Fakturering för & återkommande inköp vid ett tillfälle
ms.topic: article
ms.date: 05/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Fakturerings exempel för partner Center för en gång och väljer återkommande inköp – när du köper prenumerationer lägger du till fler prenumerationer, lägger till eller tar bort licenser.
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 329675e10205755819a19710976073d22f73eb58
ms.sourcegitcommit: 3d7d5064c5e021079ed7e6f93f03869cbf425a32
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/06/2021
ms.locfileid: "106502539"
---
# <a name="partner-center-billing-scenarios-for-one-time-and-select-recurring-purchases"></a>Fakturerings scenarier för partner Center vid ett tillfälle och välj återkommande inköp

**Lämpliga roller**

- Administratörs agent
- Faktureringsadministratör
- Support agent
- Försäljnings agent

Detta är [vanliga fakturerings scenarier](common-billing-scenarios.md). 

## <a name="purchase-a-subscription-and-add-a-license-on-the-same-day"></a>Köp en prenumeration och Lägg till en licens på samma dag

I Scenario 1 köper du en prenumeration den 11 juni till ett enhets pris på $4. Senare samma dag köper du en annan av samma prenumeration till samma pris.

Rekognoseringar-filen kommer att innehålla följande:

- $4 faktureras för service perioden 10 – 9 juli.
- $-4,00 Beräknad omstrukturering för service perioden 11 – 11 juni. Det här är den period när du hade dem som licens. Beräkning = (månatligt pris/totalt antal dagar i service perioden) x dagar i Beräknad service period x antal licenser = (4/30) x 30 x 1 = 4,00.
- $8,00 Beräknad omstrukturering för service perioden den 10 – juli, 9 juni. Detta är perioden när du hade två licenser. Beräkning = (4/30) x 30 x 2 = 8,00.

|**Inköps datum**   |**Avgifts start** |**Debiterings slut**  |**Enhets pris**  |**Kvantitet**  |**Amount** |**Kostnadstyp** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|6/11/2019      |6/10/2019   |7/09/2019         |$4                |1                 |$4            |Ny         |
|6/11/2019     | 6/10/2019    |7/09/2019        |$4        |1        | – $4       |addQuantity           |
|6/11/2019     | 6/10/2019    |7/09/2019        |$4        | 2      |$8         |addQuantity           |

## <a name="purchase-a-subscription-and-add-more-subscriptions-later"></a>Köp en prenumeration och Lägg till fler prenumerationer senare

I scenario 2 köper du en prenumeration den 11 juni till ett enhets pris på $4 och den 12 juni köper du en annan prenumeration för samma produkt till samma pris.

Rekognoseringar-filen kommer att innehålla följande:

- $4 faktureras för service perioden 10 – 9 juli.
- $-3,87 Beräknad omstrukturering för service perioden 11 – 12 juni. Detta är perioden när du har en licens. Beräkning = (månatligt pris/totalt antal dagar i service perioden) x dagar i Beräknad service period x antal licenser = (4/30) x 29 x 1 = 3,87.
- $7,74 Beräknad omstrukturering för service perioden den 12 juni – 9 juli. Detta är perioden när du hade två licenser. Beräkning = (4/30) x 29 x 2 = 7,74.

|**Inköps datum**   |**Avgifts start** |**Debiterings slut**  |**Enhets pris**  |**Kvantitet**  |**Amount** |**Kostnadstyp** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|6/11/2019 (du har en licens)     |6/10/2019   |7/09/2019         |$4         |1        |$4            |Ny         |
|6/12/2019     | 6/10/2019    |7/09/2019        |$4        |1        | – $3,87       |addQuantity           |
|6/12/2019     | 6/10/2019    |7/09/2019        |$4        | 2      |$7,74       |addQuantity           |

## <a name="purchase-a-subscription-and-remove-a-license-on-the-same-day"></a>Köp en prenumeration och ta bort en licens på samma dag

I scenario 3 köper du två prenumerationer för samma produkt den 11 juni till ett enhets pris på $4. Senare samma dag tar du bort en av licenserna.  

Rekognoseringar-filen kommer att innehålla följande:

- $8 fakturera för två licenser för service perioden 10 – juli 9.
- $-8,00 Beräknad omstrukturering för service perioden 11 – 11 juni. Detta är perioden när du hade två licenser. Beräkning = (månatligt pris/totalt antal dagar i service perioden) x dagar i Beräknad service period x antal licenser = (4/30) x 30 x 2 = 8,00.
- $4,00 Beräknad Omfakturering för service perioden 11 – juli 9. Detta är perioden när du har en licens. Beräkning = (4/30) x 30 x 1 = 4,00.

|**Inköps datum**   |**Avgifts start** |**Debiterings slut**  |**Enhets pris**  |**Kvantitet**  |**Amount** |**Kostnadstyp** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|6/11/2019      |6/10/2019   |7/09/2019         |$4                |2                 |$8            |Ny         |
|6/11/2019     | 6/10/2019    |7/09/2019        |$4        |2        | – $8       |removeQuantity           |
|6/11/2019     | 6/10/2019    |7/09/2019        |$4        | 1      |$4         |removeQuantity           |

## <a name="purchase-a-subscription-and-remove-licenses-later"></a>Köp en prenumeration och ta bort licenser senare

I Scenario 4 köper du två prenumerationer den 11 juni till ett enhets pris på $4 och den 12 juni tar du bort en av licenserna.

Rekognoseringar-filen kommer att innehålla följande:

- $8 faktureras för service perioden 10 – 9 juli.
- $-7,74 Beräknad omstrukturering för service perioden 11 – 12 juni. Detta är perioden när du hade två licenser. Beräkning = (månatligt pris/totalt antal dagar i service perioden) x dagar i Beräknad service period x antal licenser = (4/30) x 29 x 2 = 7,74.
- $3,87 Beräknad omstrukturering för service perioden den 12 juni – 9 juli. Detta är perioden när du har en licens. Beräkning = (4/30) x 29 x 1 = 3,87.

|**Inköps datum**   |**Avgifts start** |**Debiterings slut**  |**Enhets pris**  |**Kvantitet**  |**Amount** |**Kostnadstyp** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|6/11/2019 (du har två licenser)     |6/10/2019   |7/09/2019         |$4         |2        |$8       |Ny       |
|6/12/2019     | 6/10/2019    |7/09/2019        |$4        |2        | – $7,74       |removeQuantity           |
|6/12/2019 (du har en licens)    | 6/10/2019    |7/09/2019   |$4    |1      |$3,87    |removeQuantity |

## <a name="next-steps"></a>Nästa steg

- [Exempel på månatliga fakturerings scenarier för nya prenumerationer, ändring av licens belopp eller SUS pensioner](common-billing-scenarios-monthly.md)