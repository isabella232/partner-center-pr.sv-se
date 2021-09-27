---
title: Effektiv enhetsprisberäkning
ms.topic: how-to
ms.date: 09/27/2021
description: Lär dig mer om det effektiva enhetspriset och hur det beräknas. Den här artikeln innehåller även en exempelberäkning.
ms.service: partner-dashboard
ms.subservice: partnercenter-billing
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 252ec080dcc7e521e1db74eb5bdd668d8cd081e7
ms.sourcegitcommit: d731813da1d31519dc2dc583d17899e5cf4ec1b2
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/27/2021
ms.locfileid: "129071507"
---
# <a name="effective-unit-price-calculation-for-azure-plan-consumption"></a>Effektiv enhetsprisberäkning för Förbrukning i Azure-plan

**Lämpliga roller:** Faktureringsadministratör

## <a name="the-effective-unit-price"></a>Det effektiva enhetspriset

Det effektiva enhetspriset beräknas på mätarnivå (till skillnad från resursnivån) och justeras dagligen enligt mätaranvändningen.

Vi beräknar det effektiva enhetspriset med hjälp av följande tre faktorer:

- Förbrukning, som övervakas dagligen under faktureringsperioden
- Fakturerbar kostnad för mätaren
- Nivåindelad (om tillämpligt)

Eftersom vi övervakar förbrukningen varje dag under faktureringsperioden varierar det effektiva enhetspriset. Det slutliga priset för en viss faktureringsperiod blir tillgängligt när vi stoppar förbrukningsberäkningen och stänger faktureringsperioden. Du ser de flesta förbrukningsändringarna efter den fjärde eller femte decimalen.

## <a name="find-out-whether-your-meter-uses-tiered-pricing"></a>Ta reda på om din mätare använder nivåindelade priser

Om du inte vet om mätaren använder nivåindelad prissättning kan du använda proceduren nedan för att ta reda på det.

> [!NOTE]
> Förhandsversionsgränssnittet i Partnercenter ger en mer effektiv och produktiv användarupplevelse via logiskt grupperade arbetsytor. Mer information om arbetsytegränssnittet och hur du aktiverar det finns i [Getting around Partner Center (Ta sig runt i Partnercenter).](get-around-partner-center.md#turn-workspaces-on-and-off)

#### <a name="workspaces-view"></a>[Vy över arbetsytor](#tab/workspaces-view)

1. Logga in på [instrumentpanelen i Partnercenter](https://partner.microsoft.com/dashboard/).

2. Välj panelen **Prissättning** och välj sedan **Priser för Azure-plan.**

3. Leta upp din mätare efter ID och ladda sedan ned dina prisdata.

#### <a name="current-view"></a>[Aktuell vy](#tab/current-view)

1. Logga in på [instrumentpanelen i Partnercenter](https://partner.microsoft.com/dashboard/).

2. Välj **Sälj,** välj **Priser och erbjudanden** och välj sedan Priser för **Azure-plan.**

3. Leta upp din mätare efter ID och ladda sedan ned dina prisdata.

* * *

## <a name="sample-calculation"></a>Exempelberäkning

Tabellen nedan ger ett exempel på hur vi beräknar det effektiva enhetspriset under den öppna perioden.

I tabellen gäller följande värden: 

- **UP** = Enhetspris för resursen/timmen = 0,868

- **BCU** = Fakturerbar förbrukningsenhet för mätaren

- **BC** = fakturerbar kostnad för mätaren = BCU * UP * 0,85. Detta återspeglar en justering för 15 % PEC-rabatten. Vi använder sedan den nedre gränsen för funktionen för att begränsa värdet till två siffror efter decimaltecknet för att debitera minimibeloppet. 

- **Effektivt enhetspris** = BCU/BC

> [!NOTE]
> Mätaren i det här exemplet har inga prisnivåer eller andra rabatter – de effektiva enhetsprisfaktorerna i rabattprocent och andra justeringar.

| Datum | BCU (fakturerbar förbrukningsenhet) | BC (fakturerbar kostnad) | Effektivt enhetspris |
| ------ | ----------- | ----------- | ----------- |  
| 3 augusti | 29 | 21.39 | 0.737586206896552 |
| 10 augusti | 210.950039 | 155.63 | 0.737757626107858 |
| 25 augusti | 555.950039 | 410.17 | 0.737782122900436 |

## <a name="next-steps"></a>Nästa steg

- [Fakturering och skatter](billing.md)
