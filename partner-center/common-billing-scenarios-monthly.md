---
title: Vanliga scenarier för månadsfakturering
ms.topic: article
ms.date: 05/13/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-billing
description: Vanliga scenarier i Partnercenter när du använder månatlig fakturering – omfattar att lägga till nya prenumerationer, ändra licenskvantitet och pausa prenumerationer.
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: dad132f9ad749076dc52a45f1ce77f23839e8671
ms.sourcegitcommit: ad1af627f5ee6b6e3a70655f90927e932cf4c985
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 07/29/2021
ms.locfileid: "114840713"
---
# <a name="sample-monthly-billing-scenarios-for-new-subscriptions-changing-license-amounts-or-suspensions"></a>Exempel på månatliga faktureringsscenarier för nya prenumerationer, ändring av licensbelopp eller indragningar

**Lämpliga roller:** Administratörsagent | Faktureringsadministratörskonto | Supportagent | Försäljningsagent

Dessa exempel [på vanliga faktureringsscenarier](common-billing-scenarios.md) gäller om du använder månatlig fakturering i Partnercenter.

## <a name="new-monthly-subscription"></a>Ny månadsprenumeration

Faktureringsdatumet är den 15:e i varje månad. Den 13 januari köper du en ny prenumeration med en licens för 4 USD/månad och väljer månatlig fakturering. Den 15 januari licensbaserade avstämningsfilen innehåller följande faktureringsrader:

|Startdatum för avgift |Slutdatum för avgift |Avgiftstyp |Enhetspris |Kvantitet |Amount |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|1/13/2018         |2/12/2018    |Cykelavgift   |4,00       |1        |4,00 |

Licensbaserad avstämningsfil från 15 februari innehåller följande faktureringsrad:

|Startdatum för avgift |Slutdatum för avgift |Avgiftstyp |Enhetspris |Kvantitet |Amount |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|2/13/2018         |3/12/2018    |Cykelavgift   |4,00       |1        |4,00 |

## <a name="change-license-quantity"></a>Ändra licensantal

Faktureringsdatumet är den 15:e i varje månad. Den 13 januari köper du en ny prenumeration med en licens för 4 USD/månad och väljer månatlig fakturering. Den 15 januari licensbaserade avstämningsfilen innehåller följande faktureringsrader:

|Startdatum för avgift |Slutdatum för avgift |Avgiftstyp |Enhetspris |Kvantitet |Amount |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|1/13/2018         |2/12/2018    |Cykelavgift   |4,00       |1        |4,00    |

Den 1 februari ökar du din licenskvantitet från en till två. Licensbaserad avstämningsfil från 15 februari innehåller följande faktureringsrader:

|Startdatum för avgift |Slutdatum för avgift |Avgiftstyp |Enhetspris |Kvantitet |Amount |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
| 1/13/2018        |2/12/2018    |Cycle Instance Prorate   |-4.00       |1        |-4.00   |
|1/13/2018         |1/31/2018    | Cycle Instance Prorate   |2.45       |1        |2.45    |
|2/1/2018         |2/12/2018    | Cycle Instance Prorate   |1,55       |2        |3.10    |
|2/13/2018         |3/12/2018    | Cycle Instance Prorate   |4,00       |2        |8.00    |

Månadspriset är 4,00 och det finns 31 dagar i tjänstperioden 2018-13-13– 2018-02-12. Detta motsvarar ett dagligt pris på 0,129 (4/31).

Det finns 19 dagar i prorationsperioden 1/13/2018 – 2018-1-31.

Prorationsenhetspris = 2,451 = 19 x 0,129

Det finns 12 dagar i prorationsperioden 2018-02-12- 2018.

Pris på prorationsenhet = 1,54 = 12 x 0,129

## <a name="suspend-before-30-days"></a>Pausa före 30 dagar

Faktureringsdatumet är den 15:e i varje månad. Den 13 januari köper du en ny prenumeration med en licens för 4 USD/månad och väljer månatlig fakturering. Den 15 januari licensbaserade avstämningsfilen innehåller följande faktureringsrader:

|Startdatum för avgift |Slutdatum för avgift |Avgiftstyp |Enhetspris |Kvantitet |Amount |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|1/13/2018         |2/12/2018    |Cykelavgift   |4,00       |1        |4,00    |

Den 1 februari pausar du en prenumeration. Licensbaserad avstämningsfil från 15 februari innehåller följande faktureringsrad:

|Startdatum för avgift |Slutdatum för avgift |Avgiftstyp |Enhetspris |Kvantitet |Amount |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|2/12/2018|Avbryta avgift|-4.00|1|-4.00

## <a name="suspend-after-30-days"></a>Pausa efter 30 dagar

Faktureringsdatumet är den 15:e i varje månad. Den 13 januari köper du en ny prenumeration med en licens för 4 USD/månad och väljer månatlig fakturering. Den 15 januari licensbaserade avstämningsfilen innehåller följande faktureringsrader:

|Startdatum för avgift |Slutdatum för avgift |Avgiftstyp |Enhetspris |Kvantitet |Amount |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|2/12/2018|Cykelavgift|4,00|1|4,00

Licensbaserad avstämningsfil från 15 februari innehåller följande faktureringsrad:

|Startdatum för avgift |Slutdatum för avgift |Avgiftstyp |Enhetspris |Kvantitet |Amount |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
2/13/2018|3/12/2018|Cykelavgift|4,00|1|4,00

Den 1 mars pausar du prenumerationen. Licensbaserad avstämningsfil från den 15 mars innehåller följande faktureringsrad:

|Startdatum för avgift |Slutdatum för avgift |Avgiftstyp |Enhetspris |Kvantitet |Amount |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
3/1/2018|3/12/2018|Avbryta avgift|-1.72|1|-1.72

Månadspriset är 4,00 och det finns 28 dagar i tjänstperioden 2018-02-13– 2018-03-12. Detta motsvarar ett dagligt pris på 0,143 (4/28).

Enhetspris = dagar i tjänstperioden x dagligt pris x antal licenser.

Det finns 12 dagar i annulleringsperioden 3/1/2018 – 2018-03-12.

Därför är enhetspriset = -1,716 (12 x 0,143 x (-1)).

## <a name="next-steps"></a>Nästa steg

- [Faktureringsscenarier för engångsinköp och välj återkommande inköp](common-billing-scenarios-onetime-recurring.md)