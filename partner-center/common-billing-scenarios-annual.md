---
title: Årlig fakturering – vanliga scenarier
ms.topic: article
ms.date: 05/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-billing
description: Årlig fakturering för Partnercenter – när du lägger till nya prenumerationer, lägger till licenser före faktureringsdatum, ändrar licensantal eller inaktiverar/återaktiverar prenumerationer.
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 0f97c36c821955570965fcebb006610f4c5c0c79
ms.sourcegitcommit: e1da62b36420d78bf44e3962358d0af65ebc3402
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/27/2021
ms.locfileid: "129089495"
---
# <a name="common-annual-billing-scenarios-in-partner-center"></a>Vanliga årliga faktureringsscenarier i Partnercenter

**Lämpliga roller:** Administratörsagent | Faktureringsadministratörskonto | Supportagent för | Försäljningsagent

Dessa exempel [på vanliga faktureringsscenarier](common-billing-scenarios.md) gäller om du använder årlig fakturering i Partnercenter.

## <a name="new-annual-subscription"></a>Ny årsprenumeration

Faktureringsdatumet är den 15:e i varje månad. Den 13 januari köper du en ny prenumeration med en licens för 4 USD i månaden och väljer årlig fakturering. Licensbaserad avstämningsfil från den 15 januari innehåller följande faktureringsrad:

|Startdatum för avgift |Slutdatum för avgift |Avgiftstyp |Enhetspris |Kvantitet |Amount |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
Den 13 januari 2018|Den 12 januari 2019|Prorate fees when purchase (Prorate-avgifter vid köp)|48.00|1|48.00

## <a name="add-license-after-subscription-anniversary-date-but-before-billing-date"></a>Lägg till licens efter prenumerationens årsdag men före faktureringsdatum

Du köper en ny prenumeration den 11 februari 2017 med en licens för 211,20 USD per år. Årsdagen för prenumerationen anges till den 11:e i varje månad. Microsofts faktureringssystem skapar följande faktureringsrader:

- Avgift på 211,20 USD för perioden 11 februari 2017 – 10 februari 2018.

Den 12 februari 2017 köper du en andra licens. Faktureringsdatumet är 14 februari 2017. En faktura och avstämningsfil genereras. Avstämningsfilen innehåller följande faktureringsrader:

|Startdatum för avgift  |Slutdatum för avgift  |Avgiftstyp  |Enhetspris |Kvantitet | Amount |
|      :---:   |      :---:   |      :---:   |      :---:   |:---:   |:---:   |
|Den 11 februari 2017 |Den 10 februari 2018 |Prorate-avgifter vid köp |211.20 |1 | 211.20 |

På prenumerationens årsdag den 11 mars 2017 skapar Microsofts faktureringssystem följande faktureringsrader för licensökningen den 12 februari 2017:

- Kredit på 211,20 USD för perioden 11 februari 2017 till den 10 februari 2018.
- 0,58 USD i prorated charge per license (0,58 USD) per licens för perioden 11 februari 2017 till och med 11 februari 2017.
- 15,62 USD i prorated avgift per licens för två licenser för perioden 12 februari 2017 till 10 mars.
- 195,00 USD i prorated avgift per licens för två licenser för perioden 11 mars 2017 till 10 februari 2018.

Den 11 februari 2017 köper du en prenumeration. Den 12 februari 2017 lägger du till en licens. Faktureringsdatumet är 14 februari 2017. Den 11 februari 2018 förnyas din prenumeration.

Nästa faktureringsdatum är 14 mars 2017 och en faktura och avstämningsfil genereras. Avstämningsfilen innehåller följande faktureringsrader:

|Startdatum för avgift  |Slutdatum för avgift  |Avgiftstyp  |Enhetspris |Kvantitet | Amount |
|      :---:   |      :---:   |      :---:   |      :---:   |:---:   |:---:   |
|Den 11 februari 2017 |Den 10 februari 2018 |Cycle Instance Prorate |-211.20 |1 |-211.20 |
|Den 11 februari 2017 |Den 11 februari 2017 |Cycle Instance Prorate |0.58 |1 |0.58 |
|Den 12 februari 2017 |Den 10 mars 2017 |Cycle Instance Prorate |15.62 |2 |31.25 |
|Den 11 mars 2017 |Den 10 februari 2018 |Cycle Instance Prorate |195.00 |2 |390.00 |

Den 11 februari 2018 förnyas prenumerationen med ytterligare 12 månader.

## <a name="change-license-quantity"></a>Ändra licensantal

Faktureringsdatumet är den 15:e i varje månad. Den 13 januari köper du en ny prenumeration med en licens för 4 USD i månaden och väljer årlig fakturering. Licensbaserad avstämningsfil från den 15 januari innehåller följande faktureringsrad:

|Startdatum för avgift |Slutdatum för avgift |Avgiftstyp |Enhetspris |Kvantitet |Amount |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
Den 13 januari 2018|Den 12 januari 2019|Prorate-avgifter vid köp|48.00|1|48.00

Den 1 februari ökar du din licenskvantitet från en till två. Licensbaserad avstämningsfil från 15 februari innehåller följande faktureringsrader:

|Startdatum för avgift |Slutdatum för avgift |Avgiftstyp |Enhetspris |Kvantitet |Amount |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
Den 13 januari 2018|Den 12 januari 2019|Cycle Instance Prorate|-48.00|1|-48.00
Den 13 januari 2018|31 januari 2018|Cycle Instance Prorate|2.47|1|2.47
Den 1 februari 2018|Den 12 januari 2019|Cycle Instance Prorate|44.98|2|89.96

Det årliga priset är 48,00 USD, vilket motsvarar det dagliga priset på 0,13 USD (48,00 USD/365).

Enhetspris = dagar i tjänstperioden x dagligt pris x antal licenser.

Det finns 19 dagar i tjänstperioden från 13 januari 2018 till och med 31 januari 2018.

Enhetspriset är alltså 2,47 USD (19 x 0,13 x 1)

Det finns 346 dagar i tjänstperioden 1 februari 2018 till 12 januari 2019.

Enhetspriset är alltså 44,98 USD (346 x 0,13 x 2)

## <a name="suspend-before-30-days"></a>Pausa före 30 dagar

Faktureringsdatumet är den 15:e i varje månad. Den 13 januari köper du en ny prenumeration med en licens för 4 USD i månaden och väljer årlig fakturering. Den 15 januari licensbaserade avstämningsfilen innehåller följande faktureringsrad:

|Startdatum för avgift |Slutdatum för avgift |Avgiftstyp |Enhetspris |Kvantitet |Amount |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
Den 13 januari 2018|Den 12 januari 2019|Betala avgifter vid köp|48.00|1|48.00

Den 1 februari pausar du prenumerationen. Licensbaserad avstämningsfil från 15 februari innehåller följande faktureringsrad:

|Startdatum för avgift |Slutdatum för avgift |Avgiftstyp |Enhetspris |Kvantitet |Amount |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
Den 13 januari 2018|Den 12 januari 2019|Avbryta avgift|-48.00|1|-48.00

## <a name="suspend-after-30-days"></a>Pausa efter 30 dagar

Faktureringsdatumet är den 15:e i varje månad. Den 13 januari köper du en ny prenumeration med en licens för 4 USD/månad och väljer årlig fakturering. Den 15 januari licensbaserade avstämningsfilen innehåller följande faktureringsrad:

|Startdatum för avgift |Slutdatum för avgift |Avgiftstyp |Enhetspris |Kvantitet |Amount |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
Den 13 januari 2018|Den 12 januari 2019|Betala avgifter när du köper|48.00|1|48.00

Licensbaserad avstämningsfil från den 15 februari innehåller inte några faktureringsrader för den här prenumerationen.
Den 1 mars inaktiverar du prenumerationen. Licensbaserad avstämningsfil från den 15 mars innehåller följande faktureringsrad:

|Startdatum för avgift |Slutdatum för avgift |Avgiftstyp |Enhetspris |Kvantitet |Amount |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1 mars 2018|Den 12 januari 2019|Avbryta avgift|-41.34|1|-41.34

Det årliga priset är 48,00 USD, vilket motsvarar det dagliga priset på 0,13 (48,00/365).

Enhetspris = dagar i tjänstperioden x dagligt pris x antal licenser.

Det finns 318 dagar i tjänstperioden 1 mars 2018 till 12 januari 2019.

Enhetspriset är alltså 41,34 USD (318 x 0,13 x 1). Eftersom det här är en kredit är enhetspriset -41,34 USD.

## <a name="suspend-and-reactivate"></a>Pausa och återaktivera

Faktureringsdatumet är den 15:e i varje månad. Den 13 januari köper du en ny prenumeration med en licens för 4 USD i månaden och väljer årlig fakturering. Licensbaserad avstämningsfil från den 15 januari innehåller följande faktureringsrad:

|Startdatum för avgift |Slutdatum för avgift |Avgiftstyp |Enhetspris |Kvantitet |Amount |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
Den 13 januari 2018|Den 12 januari 2019|Prorate fees when purchase (Prorate-avgifter vid köp)|48.00|1|48.00

Den 1 februari pausar du prenumerationen. Den 15 februari licensbaserade avstämningsfilen innehåller följande faktureringsrad:

|Startdatum för avgift |Slutdatum för avgift |Avgiftstyp |Enhetspris |Kvantitet |Amount |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
Den 13 januari 2018|Den 12 januari 2019|Avbokningsavgift|-48.00|1|-48.00

Den 1 mars återaktiverar du din prenumeration. Licensbaserad avstämningsfil från den 15 mars innehåller följande faktureringsrad:

|Startdatum för avgift |Slutdatum för avgift |Avgiftstyp |Enhetspris |Kvantitet |Amount |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1 mars 2018|Den 12 januari 2019|Prorate fees when purchase (Prorate-avgifter vid köp)|41.34|1|41.34

Årspriset är 48,00, vilket motsvarar det dagliga priset på 0,13 (48,00/365).

Enhetspris = dagar i tjänstperioden x dagligt pris x antal licenser.

Det finns 318 dagar i tjänstperioden 1 mars 2018 – 12 januari 2019.

Enhetspriset är alltså 41,34 USD (318 x 0,13 x 1).

## <a name="multiyear-offers-with-annual-billing"></a>Erbjudanden för flera år med årlig fakturering

För erbjudanden för flera år med årlig fakturering börjar avgifterna på inköpsdatum och fortsätter i ett år.

(I [](#example-of-multiyear-billing) exemplet med flerårsfakturering börjar avgifterna för det första året den 20 mars 2020 och avslutas ett år senare den 19 mars 2021.)

Avgifter för det andra årets start en månad före debiterings slutdatumet för det första året.

(I det här exemplet börjar avgifter för det andra året den 20 februari 2021, en månad före det första årets slutdatum för debitering den 19 mars 2021.)

Den här årliga faktureringsprocessen har en månadsskillnad mellan slutdatumet för prenumerationen och slutdatumet för debiteringen för det tredje året. Prenumerationen förblir dock aktiv fram till prenumerationens slutdatum.

(I det här exemplet är slutdatumet för prenumerationen den 19 mars 2023 det tredje året en månad efter slutdatumet för avgiften den 19 februari 2023.)

### <a name="example-of-multiyear-billing"></a>Exempel på fakturering för flera år

För ett 36 månaders erbjudande som köpts den 20 mars 2020 som visas i tabellerna som följer skulle avstämningsfilen vara:

#### <a name="first-year"></a>Första året

|Startdatum för prenumeration  |Slutdatum för prenumeration  |Startdatum för avgift  |Slutdatum för avgift  |Kostnadstyp  |
|:-:|:-:|:-:|:-:|:-:|
|Den 20 mars 2020|Den 19 mars 2023|Den 20 mars 2020|Den 19 mars 2021|Prorate-avgifter vid köp|

#### <a name="second-year"></a>Andra året

|Startdatum för prenumeration  |Slutdatum för prenumeration  |Startdatum för avgift  |Slutdatum för avgift  |Kostnadstyp  |
|:-:|:-:|:-:|:-:|:-:|
|Den 20 mars 2020|Den 19 mars 2023|Den 20 februari 2021|Den 19 februari 2022|Cykelavgift|

#### <a name="third-year"></a>Tredje året

|Startdatum för prenumeration  |Slutdatum för prenumeration  |Startdatum för avgift  |Slutdatum för avgift  |Kostnadstyp  |
|:-:|:-:|:-:|:-:|:-:|
|Den 20 mars 2020|Den 19 mars 2023|Den 20 februari 2022|Den 19 februari 2023|Cykelavgift|
