---
title: Årlig fakturering – vanliga scenarier
ms.topic: article
ms.date: 05/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-billing
description: Årlig fakturering i Partnercenter – när du lägger till nya prenumerationer, lägger till licenser före faktureringsdatum, ändrar licensantal eller inaktiverar/återaktiverar prenumerationer.
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 2baab834c3d31639f1353a53fb8787da041aec1c1c59776df49bd590fb7452f0
ms.sourcegitcommit: 121f1b9cbd88faeba60dc9b475f9c0647cdc933c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/06/2021
ms.locfileid: "115682376"
---
# <a name="common-annual-billing-scenarios-in-partner-center"></a>Vanliga årliga faktureringsscenarier i Partnercenter

**Lämpliga roller:** Administratörsagent | Faktureringsadministratörskonto | Supportagent för | Försäljningsagent

Dessa exempel [på vanliga faktureringsscenarier](common-billing-scenarios.md) gäller om du använder årlig fakturering i Partnercenter.

## <a name="new-annual-subscription"></a>Ny årsprenumeration

Faktureringsdatumet är den 15:e i varje månad. Den 13 januari köper du en ny prenumeration med en licens för 4 USD/månad och väljer årlig fakturering. Den 15 januari licensbaserade avstämningsfilen innehåller följande faktureringsrad:

|Startdatum för avgift |Slutdatum för avgift |Avgiftstyp |Enhetspris |Kvantitet |Amount |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|Prorate fees when purchase (Prorate-avgifter vid köp)|48.00|1|48.00

## <a name="add-license-after-subscription-anniversary-date-but-before-billing-date"></a>Lägg till licens efter prenumerationens årsdag men före faktureringsdatum

Du köper en ny prenumeration 2017-02-11 med en licens för 211,20 USD/år. Din prenumerations årsdag anges till den 11:e i varje månad. Microsofts faktureringssystem skapar följande faktureringsrader:

- Avgift på 211,20 USD för perioden 2/11/17 – 2/10/18.

Den 17-12-17 köper du en andra licens. Faktureringsdatumet är 17-02-14. En faktura och avstämningsfil genereras. Avstämningsfilen innehåller följande faktureringsrader:

|Startdatum för avgift  |Slutdatum för avgift  |Avgiftstyp  |Enhetspris |Kvantitet | Amount |
|      :---:   |      :---:   |      :---:   |      :---:   |:---:   |:---:   |
|2/11/2017 |2/10/2018 |Prorate-avgifter vid köp |211.20 |1 | 211.20 |

På årsdagen för prenumerationen, 17-03-11, skapar Microsofts faktureringssystem följande faktureringsrader för licensökningen den 17-02-12:

- Kredit på 211,20 USD för perioden 2/11/17 – 2/10/18.
- 0,58 USD i prorated avgift per licens för en licens under perioden 2/11/17 – 2/11/17.
- 15,62 USD i prorated avgift per licens för två licenser under perioden 2017-02-12-10.
- 195,00 USD i prorated avgift per licens för två licenser för perioden 2017-03-11 – 2018-02-10.

Den 17-02-11 köper du en prenumeration. Den 17-12-17 lägger du till en licens. Faktureringsdatumet är 17-02-14. Den 18-11-18 förnyas din prenumeration.

Nästa faktureringsdatum är 17-03-14 och en faktura- och avstämningsfil genereras. Avstämningsfilen innehåller följande faktureringsrader:

|Startdatum för avgift  |Slutdatum för avgift  |Avgiftstyp  |Enhetspris |Kvantitet | Amount |
|      :---:   |      :---:   |      :---:   |      :---:   |:---:   |:---:   |
|2/11/2017 |2/10/2018 |Cycle Instance Prorate |-211.20 |1 |-211.20 |
|2/11/2017 |2/11/2017 |Cycle Instance Prorate |0.58 |1 |0.58 |
|2/12/2017 |3/10/2017 |Cycle Instance Prorate |15.62 |2 |31.25 |
|3/11/2017 |2/10/2018 |Cycle Instance Prorate |195.00 |2 |390.00 |

Den 18-11-18 förnyas prenumerationen med ytterligare en period på 12 månader.

## <a name="change-license-quantity"></a>Ändra licensantal

Faktureringsdatumet är den 15:e i varje månad. Den 13 januari köper du en ny prenumeration med en licens för 4 USD/månad och väljer årlig fakturering. Den 15 januari licensbaserade avstämningsfilen innehåller följande faktureringsrad:

|Startdatum för avgift |Slutdatum för avgift |Avgiftstyp |Enhetspris |Kvantitet |Amount |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|Prorate fees when purchase (Prorate-avgifter vid köp)|48.00|1|48.00

Den 1 februari ökar du din licenskvantitet från en till två. Den 15 februari licensbaserade avstämningsfilen innehåller följande faktureringsrader:

|Startdatum för avgift |Slutdatum för avgift |Avgiftstyp |Enhetspris |Kvantitet |Amount |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|Cycle Instance Prorate|-48.00|1|-48.00
1/13/2018|1/31/2018|Cycle Instance Prorate|2.47|1|2.47
2/1/2018|1/12/2019|Cycle Instance Prorate|44.98|2|89.96

Årspriset är 48,00 vilket motsvarar det dagliga priset på 0,13 (48,00/365).

Enhetspris = dagar i tjänstperioden x dagligt pris x antal licenser.

Det finns 19 dagar i tjänstperioden 2018-01-13– 2018-01-31.

Därför är enhetspriset = 2,47 (19x0,13x1)

Det finns 346 dagar i tjänstperioden 2018-02-12 2019.

Enhetspris = 44,98 (346x0,13x2)

## <a name="suspend-before-30-days"></a>Pausa före 30 dagar

Faktureringsdatumet är den 15:e i varje månad. Den 13 januari köper du en ny prenumeration med en licens för 4 USD/månad och väljer årlig fakturering. Den 15 januari licensbaserade avstämningsfilen innehåller följande faktureringsrad:

|Startdatum för avgift |Slutdatum för avgift |Avgiftstyp |Enhetspris |Kvantitet |Amount |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|Prorate fees when purchase (Prorate-avgifter vid köp)|48.00|1|48.00

Den 1 februari pausar du prenumerationen. Den 15 februari licensbaserade avstämningsfilen innehåller följande faktureringsrad:

|Startdatum för avgift |Slutdatum för avgift |Avgiftstyp |Enhetspris |Kvantitet |Amount |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|Avbokningsavgift|-48.00|1|-48.00

## <a name="suspend-after-30-days"></a>Pausa efter 30 dagar

Faktureringsdatumet är den 15:e i varje månad. Den 13 januari köper du en ny prenumeration med en licens för 4 USD/månad och väljer årlig fakturering. Den 15 januari licensbaserade avstämningsfilen innehåller följande faktureringsrad:

|Startdatum för avgift |Slutdatum för avgift |Avgiftstyp |Enhetspris |Kvantitet |Amount |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|Prorate fees when purchase (Prorate-avgifter vid köp)|48.00|1|48.00

Den 15 februari licensbaserade avstämningsfilen innehåller inte några faktureringsrader för den här prenumerationen.
Den 1 mars pausar du prenumerationen. Licensbaserad avstämningsfil från den 15 mars innehåller följande faktureringsrad:

|Startdatum för avgift |Slutdatum för avgift |Avgiftstyp |Enhetspris |Kvantitet |Amount |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
3/1/2018|1/12/2019|Avbokningsavgift|-41.34|1|-41.34

Årspriset är 48,00 vilket motsvarar det dagliga priset på 0,13 (48,00/365).

Enhetspris = dagar i tjänstperioden x dagligt pris x antal licenser.

Det finns 318 dagar i tjänstperioden 3/1/2018 – 2019-1-12.

Enhetspris = 41,34 (318x0,13x1). Eftersom det här är en kredit är enhetspriset -41,34.

## <a name="suspend-and-reactivate"></a>Pausa och återaktivera

Faktureringsdatumet är den 15:e i varje månad. Den 13 januari köper du en ny prenumeration med en licens för 4 USD/månad och väljer årlig fakturering. Den 15 januari licensbaserade avstämningsfilen innehåller följande faktureringsrad:

|Startdatum för avgift |Slutdatum för avgift |Avgiftstyp |Enhetspris |Kvantitet |Amount |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|Prorate fees when purchase (Prorate-avgifter vid köp)|48.00|1|48.00

Den 1 februari pausar du prenumerationen. Den 15 februari licensbaserade avstämningsfilen innehåller följande faktureringsrad:

|Startdatum för avgift |Slutdatum för avgift |Avgiftstyp |Enhetspris |Kvantitet |Amount |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|Avbokningsavgift|-48.00|1|-48.00

Den 1 mars återaktiverar du din prenumeration. Licensbaserad avstämningsfil från den 15 mars innehåller följande faktureringsrad:

|Startdatum för avgift |Slutdatum för avgift |Avgiftstyp |Enhetspris |Kvantitet |Amount |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
3/1/2018|1/12/2019|Prorate fees when purchase (Prorate-avgifter vid köp)|41.34|1|41.34

Årspriset är 48,00 vilket motsvarar det dagliga priset på 0,13 (48,00/365).

Enhetspris = dagar i tjänstperioden x dagligt pris x antal licenser.

Det finns 318 dagar i tjänstperioden 3/1/2018 – 2019-1-12.

Enhetspris = 41,34 (318x0,13x1).
