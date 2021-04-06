---
title: Årlig fakturering – vanliga scenarier
ms.topic: article
ms.date: 05/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Årlig fakturering för partner Center – när du lägger till nya prenumerationer lägger du till licenser före fakturerings datum, ändra licens antal eller inaktivera/återaktivera prenumerationer.
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 7494fd7cc003d1179c0ed959b21e1be2cbcc3255
ms.sourcegitcommit: 3d7d5064c5e021079ed7e6f93f03869cbf425a32
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/06/2021
ms.locfileid: "106502488"
---
# <a name="common-annual-billing-scenarios-in-partner-center"></a>Vanliga årliga fakturerings scenarier i Partner Center

**Lämpliga roller**

- Administratörs agent
- Faktureringsadministratör
- Support agent
- Försäljnings agent

Dessa exempel på [vanliga fakturerings scenarier](common-billing-scenarios.md) är tillämpliga om du använder årlig fakturering i Partner Center.

## <a name="new-annual-subscription"></a>Ny årlig prenumeration

Ditt fakturerings datum är den 15: e i varje månad. Den 13 januari köper du en ny prenumeration med en licens i USD 4 per månad och väljer årlig fakturering. Den 15 licensbaserade avstämnings filen för januari kommer att innehålla följande fakturerings rad:

|Start datum för debitering |Debiterings slutdatum |Avgifts typ |Enhetspris |Kvantitet |Amount |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|Betala avgifter vid köp|48,00|1|48,00

## <a name="add-license-after-subscription-anniversary-date-but-before-billing-date"></a>Lägg till licens efter prenumerations jubileums dag men före fakturerings datum

Du köper en ny prenumeration på 2/11/17 med en licens för $211.20/år. Prenumerations årsdagen anges som 11 i varje månad. Microsofts fakturerings system skapar följande fakturerings rader:

- $211,20-kostnad för perioden 2/11/17 – 2/10/18.

På 2/12/17 köper du en andra licens. Ditt fakturerings datum är 2/14/17. En faktura och en avstämnings fil skapas. Avstämnings filen innehåller följande fakturerings rader:

|Start datum för debitering  |Debiterings slutdatum  |Avgifts typ  |Enhetspris |Kvantitet | Amount |
|      :---:   |      :---:   |      :---:   |      :---:   |:---:   |:---:   |
|2/11/2017 |2/10/2018 |Betala avgifter vid köp |211,20 |1 | 211,20 |

På prenumerationens jubileums dag 3/11/17 skapar Microsoft fakturerings systemet följande fakturerings rader för licens ökningen den 2/12/17:

- $211,20 kredit för perioden 2/11/17 – 2/10/18.
- $0,58 Beräknad avgift per licens för en licens för perioden 2/11/17 – 2/11/17.
- $15,62 Beräknad avgift per licens för två licenser för perioden 2/12/17 – 3/10/2017.
- $195,00 Beräknad avgift per licens för två licenser för perioden 3/11/2017 – 2/10/2018.

På 2/11/17 köper du en prenumeration. På 2/12/17 lägger du till en licens. Ditt fakturerings datum är 2/14/17. Den 2/11/18 prenumerationen förnyas.

Nästa fakturerings datum är 3/14/17 och en faktura och en avstämnings fil skapas. Avstämnings filen innehåller följande fakturerings rader:

|Start datum för debitering  |Debiterings slutdatum  |Avgifts typ  |Enhetspris |Kvantitet | Amount |
|      :---:   |      :---:   |      :---:   |      :---:   |:---:   |:---:   |
|2/11/2017 |2/10/2018 |Prograder för cykel instans |– 211,20 |1 |– 211,20 |
|2/11/2017 |2/11/2017 |Prograder för cykel instans |0,58 |1 |0,58 |
|2/12/2017 |3/10/2017 |Prograder för cykel instans |15,62 |2 |31,25 |
|3/11/2017 |2/10/2018 |Prograder för cykel instans |195,00 |2 |390,00 |

Den 2/11/18 prenumerationen förnyas under en till tolv månaders period.

## <a name="change-license-quantity"></a>Ändra licensantal

Ditt fakturerings datum är den 15: e i varje månad. Den 13 januari köper du en ny prenumeration med en licens i USD 4 per månad och väljer årlig fakturering. Den 15 licensbaserade avstämnings filen för januari kommer att innehålla följande fakturerings rad:

|Start datum för debitering |Debiterings slutdatum |Avgifts typ |Enhetspris |Kvantitet |Amount |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|Betala avgifter vid köp|48,00|1|48,00

Den 1 februari ökar du licens antalet från en till två. Den 15 licensbaserade avstämnings filen från februari kommer att innehålla följande fakturerings rader:

|Start datum för debitering |Debiterings slutdatum |Avgifts typ |Enhetspris |Kvantitet |Amount |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|Prograder för cykel instans|– 48,00|1|– 48,00
1/13/2018|1/31/2018|Prograder för cykel instans|2,47|1|2,47
2/1/2018|1/12/2019|Prograder för cykel instans|44,98|2|89,96

Det årliga priset är 48,00 som motsvarar det dagliga priset för 0,13 (48.00/365).

Enhets pris = dagar i service perioden x det dagliga priset x antal licenser.

Det finns 19 dagar i service perioden 1/13/2018 – 1/31/2018.

Därför är enhets pris = 2,47 (19x 0.13 x1)

Det finns 346 dagar i service perioden 2/1/2018 – 1/12/2019.

Därför är enhets pris = 44,98 (346x 0.13 x2)

## <a name="suspend-before-30-days"></a>Pausa före 30 dagar

Ditt fakturerings datum är den 15: e i varje månad. Den 13 januari köper du en ny prenumeration med en licens i USD 4 per månad och väljer årlig fakturering. Den 15 licensbaserade avstämnings filen för januari kommer att innehålla följande fakturerings rad:

|Start datum för debitering |Debiterings slutdatum |Avgifts typ |Enhetspris |Kvantitet |Amount |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|Betala avgifter vid köp|48,00|1|48,00

Den 1 februari pausar du din prenumeration. Den 15 licensbaserade avstämnings filen från februari kommer att innehålla följande fakturerings rad:

|Start datum för debitering |Debiterings slutdatum |Avgifts typ |Enhetspris |Kvantitet |Amount |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|Annullera avgift|– 48,00|1|– 48,00

## <a name="suspend-after-30-days"></a>Pausa efter 30 dagar

Ditt fakturerings datum är den 15: e i varje månad. Den 13 januari köper du en ny prenumeration med en licens i USD 4 per månad och väljer årlig fakturering. Den 15 licensbaserade avstämnings filen för januari kommer att innehålla följande fakturerings rad:

|Start datum för debitering |Debiterings slutdatum |Avgifts typ |Enhetspris |Kvantitet |Amount |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|Betala avgifter vid köp|48,00|1|48,00

Den 15 licensbaserade avstämnings filen från februari kommer inte att innehålla några fakturerings rader för den här prenumerationen.
Den 1 mars pausar du din prenumeration. Den 15 mars-licensbaserade avstämnings filen innehåller följande fakturerings rad:

|Start datum för debitering |Debiterings slutdatum |Avgifts typ |Enhetspris |Kvantitet |Amount |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
3/1/2018|1/12/2019|Annullera avgift|– 41,34|1|– 41,34

Det årliga priset är 48,00 som motsvarar det dagliga priset för 0,13 (48.00/365).

Enhets pris = dagar i service perioden x det dagliga priset x antal licenser.

Det finns 318 dagar i service perioden 3/1/2018 – 1/12/2019.

Därför är enhets pris = 41,34 (318x 0.13 x1). Eftersom det här är en kredit är enhets priset-41,34.

## <a name="suspend-and-reactivate"></a>Pausa och återaktivera

Ditt fakturerings datum är den 15: e i varje månad. Den 13 januari köper du en ny prenumeration med en licens i USD 4 per månad och väljer årlig fakturering. Den 15 licensbaserade avstämnings filen för januari kommer att innehålla följande fakturerings rad:

|Start datum för debitering |Debiterings slutdatum |Avgifts typ |Enhetspris |Kvantitet |Amount |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|Betala avgifter vid köp|48,00|1|48,00

Den 1 februari pausar du din prenumeration. Den 15 licensbaserade avstämnings filen från februari kommer att innehålla följande fakturerings rad:

|Start datum för debitering |Debiterings slutdatum |Avgifts typ |Enhetspris |Kvantitet |Amount |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|Annullera avgift|– 48,00|1|– 48,00

Den 1 mars återaktiverar du din prenumeration. Den 15 mars-licensbaserade avstämnings filen innehåller följande fakturerings rad:

|Start datum för debitering |Debiterings slutdatum |Avgifts typ |Enhetspris |Kvantitet |Amount |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
3/1/2018|1/12/2019|Betala avgifter vid köp|41,34|1|41,34

Det årliga priset är 48,00 som motsvarar det dagliga priset för 0,13 (48.00/365).

Enhets pris = dagar i service perioden x det dagliga priset x antal licenser.

Det finns 318 dagar i service perioden 3/1/2018 – 1/12/2019.

Därför är enhets pris = 41,34 (318x 0.13 x1).
