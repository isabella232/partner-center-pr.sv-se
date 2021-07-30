---
title: Effektiv enhetsprisberäkning
ms.topic: how-to
ms.date: 04/02/2021
description: Lär dig mer om det effektiva enhetspriset och hur det beräknas. Den här artikeln innehåller även en exempelberäkning.
ms.service: partner-dashboard
ms.subservice: partnercenter-billing
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 4148e9be6ab5bd3e5a146c0ed5479d8ad9723204
ms.sourcegitcommit: ad1af627f5ee6b6e3a70655f90927e932cf4c985
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 07/29/2021
ms.locfileid: "114837330"
---
# <a name="effective-unit-price-calculation-for-azure-plan-consumption"></a>Effektiv beräkning av enhetspris för Förbrukning av Azure-plan

**Lämpliga roller:** Faktureringsadministratör

## <a name="the-effective-unit-price"></a>Det effektiva enhetspriset

Det effektiva enhetspriset beräknas på mätarnivå (till skillnad från resursnivån) och justeras dagligen enligt mätaranvändningen.

Vi beräknar det effektiva enhetspriset med hjälp av följande tre faktorer:

- Förbrukning, som övervakas dagligen under faktureringsperioden
- Fakturerbar kostnad för mätaren
- Nivåindelad (om tillämpligt)

Eftersom vi övervakar förbrukning dagligen under faktureringsperioden varierar det effektiva enhetspriset. Det slutliga priset för en viss faktureringsperiod blir tillgängligt när vi stoppar förbrukningsberäkningen och stänger faktureringsperioden. Du ser de flesta förbrukningsändringarna efter den fjärde eller femte decimalen.

## <a name="find-out-whether-your-meter-uses-tiered-pricing"></a>Ta reda på om mätaren använder nivåindelade priser

Om du inte vet om mätaren använder nivåindelad prissättning kan du använda proceduren nedan för att ta reda på det. 

1. Logga in på [instrumentpanelen i Partnercenter](https://partner.microsoft.com/dashboard/).
2. Välj **Sälj,** välj **Priser och erbjudanden och** välj sedan Priser för **Azure-plan.**
3. Leta upp din mätare efter ID och ladda sedan ned dina prisdata. 

## <a name="sample-calculation"></a>Exempelberäkning

Tabellen nedan ger ett exempel på hur vi beräknar det effektiva enhetspriset under den öppna perioden.

I tabellen gäller följande värden: 

- **UP** = Enhetspris för resursen/timmen = 0,868

- **BCU** = Fakturerbar förbrukningsenhet för mätaren

- **BC** = Fakturerbar kostnad för mätaren = BCU * UP * 0,85. Detta återspeglar en justering för 15 % PEC-rabatten. Sedan använder vi den nedre gränsen för funktionen för att begränsa värdet till två siffror efter decimaltecknet för att debitera det minsta beloppet. 

- **Gällande enhetspris** = BCU/BC

>[!NOTE]

>Obs! Mätaren i det här exemplet har inga prisnivåer eller andra rabatter – de effektiva enhetsprisfaktorerna i rabattprocent och andra justeringar.


| Datum | BCU (fakturerbar förbrukningsenhet) | BC (fakturerbar kostnad) | Effektivt enhetspris |
| ------ | ----------- | ----------- | ----------- |  
| 3 augusti | 29 | 21.39 | 0.737586206896552 |
| 10 augusti | 210.950039 | 155.63 | 0.737757626107858 |
| 25 augusti | 555.950039 | 410.17 | 0.737782122900436 |

## <a name="next-steps"></a>Nästa steg

- [Fakturering och skatter](billing.md)
