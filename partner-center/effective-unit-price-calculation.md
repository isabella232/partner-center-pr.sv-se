---
title: Effektiv enhetsprisberäkning
ms.topic: how-to
ms.date: 11/10/2020
description: Läs om det effektiva enhets priset och hur det beräknas. Den här artikeln innehåller även en exempel beräkning.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 6ca6e9bf6a49e695314a3e33e36d2d1d5d4d2a25
ms.sourcegitcommit: 147813ba322653c989df5afe0b3bf0c252523a92
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 12/03/2020
ms.locfileid: "96556335"
---
# <a name="effective-unit-price-calculation-for-azure-plan-consumption"></a>Effektiv enhets pris beräkning för Azure plan-förbrukning

## <a name="the-effective-unit-price"></a>Det effektiva enhets priset

Det effektiva enhets priset beräknas på mätar nivån (till skillnad från resurs nivån) och justeras dagligen enligt mätnings användningen.

Vi beräknar det effektiva enhets priset med följande tre faktorer:

- Förbrukning, som övervakas dagligen under fakturerings perioden
- Fakturerbar kostnad för mätaren
- Skiktning (om tillämpligt)

Eftersom vi övervakar förbrukning dagligen under hela fakturerings perioden kommer det effektiva enhets priset att variera. Det slutgiltiga priset för en viss fakturerings cykel blir tillgängligt efter att du har stoppat förbruknings beräkningen och stängt fakturerings perioden. Du ser de flesta förändringar i förbrukningen efter den fjärde eller femte decimalen.

## <a name="find-out-whether-your-meter-uses-tiered-pricing"></a>Ta reda på om din mätning använder nivå priser

Om du inte vet om mätaren använder nivå priser använder du proceduren nedan för att ta reda på det. 

1. Logga in på [instrumentpanelen i Partnercenter](https://partner.microsoft.com/dashboard/).
2. Välj **sälja**, Välj **priser och erbjudanden** och välj sedan **pris för Azure-prenumeration**.
3. Leta upp din mätning efter ID och ladda ned dina pris data. 

## <a name="sample-calculation"></a>Exempel beräkning

Tabellen nedan visar ett exempel på hur vi beräknar det effektiva enhets priset under den öppna perioden.

I tabellen gäller följande värden: 

- **Upp** = enhets priset för resursen/timmen = 0,868

- **BCU** = fakturerbar förbruknings enhet för mätaren

- **BC** = fakturerbar kostnad för mätaren = BCU * upp * 0,85. Detta motsvarar en justering för 15% PEC-rabatten. Vi använder sedan den nedre gränsen för funktionen för att begränsa värdet till två siffror efter decimal tecknet, för att debitera minimi beloppet. 

- **Effektivt enhets pris** = BCU/BC

>[!NOTE]
>Obs! mätaren i det här exemplet har inga nivåer i prissättningen.

| Datum | BCU (fakturerbar förbruknings enhet) | BC (fakturerbar kostnad) | Effektivt enhets pris |
| ------ | ----------- | ----------- | ----------- |  
| 3 – aug | 29 | 21,39 | 0.737586206896552 |
| 10 – aug | 210,950039 | 155,63 | 0.737757626107858 |
| 25 – aug | 555,950039 | 410,17 | 0.737782122900436 |

## <a name="next-steps"></a>Nästa steg

- [Fakturering och skatter](billing.md)
