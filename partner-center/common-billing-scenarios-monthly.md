---
title: Vanliga månads fakturerings scenarier
ms.topic: article
ms.date: 05/13/2020
description: Vanliga scenarier i Partner Center när du använder månatlig fakturering – inkluderar att lägga till nya prenumerationer, ändra licens antal och pausa prenumerationer.
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 616f706ddb4613f927e0c2830dd794fa3db3944e
ms.sourcegitcommit: 7153f0b8c67efd35f58695ca2a7e00e70da1c5e9
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 07/17/2020
ms.locfileid: "92530988"
---
# <a name="sample-monthly-billing-scenarios-for-new-subscriptions-changing-license-amounts-or-suspensions"></a>Exempel på månatliga fakturerings scenarier för nya prenumerationer, ändring av licens belopp eller SUS pensioner

**Lämpliga roller**

- Administratörs agent
- Faktureringsadministratör
- Support agent
- Försäljnings agent

Dessa exempel på [vanliga fakturerings scenarier](common-billing-scenarios.md) är tillgängliga om du använder fakturering per månad i Partner Center.

## <a name="new-monthly-subscription"></a>Ny månatlig prenumeration

Ditt fakturerings datum är den 15: e i varje månad. Den 13 januari köper du en ny prenumeration med en licens i USD 4 per månad och väljer månatlig fakturering. Den 15 juli licensbaserade avstämnings filen innehåller följande fakturerings rader:

|Start datum för debitering |Debiterings slutdatum |Avgifts typ |Enhetspris |Kvantitet |Belopp |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|1/13/2018         |2/12/2018    |Cykel avgift   |4,00       |1        |4,00 |

Den 15 februari licensbaserade avstämnings filen innehåller följande fakturerings rad:

|Start datum för debitering |Debiterings slutdatum |Avgifts typ |Enhetspris |Kvantitet |Belopp |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|2/13/2018         |3/12/2018    |Cykel avgift   |4,00       |1        |4,00 |

## <a name="change-license-quantity"></a>Ändra licensantal

Ditt fakturerings datum är den 15: e i varje månad. Den 13 januari köper du en ny prenumeration med en licens i USD 4 per månad och väljer månatlig fakturering. Den 15 juli licensbaserade avstämnings filen innehåller följande fakturerings rader:

|Start datum för debitering |Debiterings slutdatum |Avgifts typ |Enhetspris |Kvantitet |Belopp |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|1/13/2018         |2/12/2018    |Cykel avgift   |4,00       |1        |4,00    |

Den 1 februari ökar du antalet licenser från en till två. Den 15 februari licensbaserade avstämnings filen innehåller följande fakturerings rader:

|Start datum för debitering |Debiterings slutdatum |Avgifts typ |Enhetspris |Kvantitet |Belopp |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
| 1/13/2018        |2/12/2018    |Prograder för cykel instans   |– 4,00       |1        |– 4,00   |
|1/13/2018         |1/31/2018    | Prograder för cykel instans   |2.45       |1        |2.45    |
|2/1/2018         |2/12/2018    | Prograder för cykel instans   |1,55       |2        |3,10    |
|2/13/2018         |3/12/2018    | Prograder för cykel instans   |4,00       |2        |8,00    |

Månads priset är 4,00 och det finns 31 dagar i service perioden 1/13/2018 – 2/12/2018. Detta motsvarar ett dagligt pris på 0,129 (4/31).

Det finns 19 dagar i proportions perioden 1/13/2018 – 1/31/2018.

Proportioner enhets pris = 2,451 = 19 x 0,129

Det finns 12 dagar i proportions perioden 2/1/2018 – 2/12/2018.

Proportioner enhets pris = 1,54 = 12 x 0,129

## <a name="suspend-before-30-days"></a>Pausa före 30 dagar

Ditt fakturerings datum är den 15: e i varje månad. Den 13 januari köper du en ny prenumeration med en licens i USD 4 per månad och väljer månatlig fakturering. Den 15 juli licensbaserade avstämnings filen innehåller följande fakturerings rader:

|Start datum för debitering |Debiterings slutdatum |Avgifts typ |Enhetspris |Kvantitet |Belopp |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|1/13/2018         |2/12/2018    |Cykel avgift   |4,00       |1        |4,00    |

Den 1 februari pausar du en prenumeration. Den 15 februari licensbaserade avstämnings filen innehåller följande fakturerings rad:

|Start datum för debitering |Debiterings slutdatum |Avgifts typ |Enhetspris |Kvantitet |Belopp |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|2/12/2018|Annullera avgift|– 4,00|1|– 4,00

## <a name="suspend-after-30-days"></a>Pausa efter 30 dagar

Ditt fakturerings datum är den 15: e i varje månad. Den 13 januari köper du en ny prenumeration med en licens i USD 4 per månad och väljer månatlig fakturering. Den 15 juli licensbaserade avstämnings filen innehåller följande fakturerings rader:

|Start datum för debitering |Debiterings slutdatum |Avgifts typ |Enhetspris |Kvantitet |Belopp |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|2/12/2018|Cykel avgift|4,00|1|4,00

Den 15 februari licensbaserade avstämnings filen innehåller följande fakturerings rad:

|Start datum för debitering |Debiterings slutdatum |Avgifts typ |Enhetspris |Kvantitet |Belopp |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
2/13/2018|3/12/2018|Cykel avgift|4,00|1|4,00

Den 1 mars du pausar prenumerationen. Den 15 mars-licensbaserade avstämnings filen innehåller följande fakturerings rad:

|Start datum för debitering |Debiterings slutdatum |Avgifts typ |Enhetspris |Kvantitet |Belopp |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
3/1/2018|3/12/2018|Annullera avgift|– 1,72|1|– 1,72

Månads priset är 4,00 och det finns 28 dagar i service perioden 2/13/2018 – 3/12/2018. Detta motsvarar ett dagligt pris på 0,143 (4/28).

Enhets pris = dagar i service perioden x det dagliga priset x antal licenser.

Det finns 12 dagar i annullerings perioden 3/1/2018 – 3/12/2018.

Därför är enhets priset =-1,716 (12 x 0,143 x (-1)).
