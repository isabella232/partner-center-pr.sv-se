---
title: Azure plan pris lista för CSP-partner
ms.topic: how-to
ms.date: 05/04/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Lär dig hur CSP-programpartner kan använda Partner Center för att visa pris listan för prenumerationer i Azure-planen.
author: brentserbus
ms.author: brserbus
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: f11031c6071dadb427d2d5b93edd90af1a844131
ms.sourcegitcommit: fc1f9cb5a542bdc92d62d2a7e1ab2f4e69903e49
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 01/28/2021
ms.locfileid: "98924976"
---
# <a name="price-list-for-the-new-commerce-experience-in-csp-for-azure"></a>Prislista för den nya handelsupplevelsen i CSP för Azure

**Lämpliga roller**

- Administratörs agent
- Faktureringsadministratör
- Global administratör
- Support agent
- Försäljnings agent
- Administratör för användar hantering

Pris listan för den nya Azure Commerce-upplevelsen i CSP publiceras i Partner Center. Pris listan levereras dynamiskt i real tid och priserna visas endast i USD. Från januari 28 2021 debiteras partners i EU/EFTA-och Storbritannien-regionen som har nya kunder och befintliga CSP-kunder som köper nya Commerce-erbjudanden för första gången vars innehavare skapades före 11 maj 2020, faktureras för dessa inköp i partner platsens valuta.  Partner som finns utanför EU/EFTA-och Storbritannien-regionen fortsätter att faktureras i partner platsens valuta. Läs [Azure plan-fakturering](azure-plan-billing.md).

## <a name="see-pricing-for-subscriptions-under-the-azure-plan-pricing"></a>Se prissättning för prenumerationer under priser för Azure-prenumeration

1. Från menyn Partner Center till vänster väljer du **försäljning** och sedan **Marketplace**.

2. Under priser för Azure-prenumeration väljer du det land som du vill ha prissättning för.

3. Bredvid **export typ** väljer du **priser för Azure plan förbrukning**, **priser för Azure-prenumerations reservationer** eller **FX-priser**. 

>[!NOTE] 
>**FX-priser** är inte land-/regionsspecifika.

4. Välj det datum som du vill ha, till exempel **aktuell**, bredvid **prissättning för datum**.

   :::image type="content" source="images/azure/pricingnew.png" alt-text="lands information":::

>[!NOTE] 
>Du kan exportera två olika pris listor – priser för Azure-prenumeration och marknads plats från tredje part.

## <a name="azure-price-list-specifics"></a>Information om Azure pris lista

- Priser för Azure-abonnemang kommer att vara tillgängliga från Marketplace-sidan i Partner Center under **Sälj**.

- Exporter kommer att vara tillgängliga för Azure plan förbruknings tjänster, Azure Reservations och FX-priser.

- Alternativen för export är:

  - **Dagens pris**: Detta omfattar alla mätare och priser från den 1: e i månaden till det aktuella datumet för den aktuella månaden. Detta omfattar nya priser, ändrade priser eller borttagna priser. Alla priser kommer att ha effektiva start-och slutdatum för att förklara om de är nya eller borttagna.

  - **Föregående månads priser**: hämtningar av varje typ av resurs kommer att vara per månad. För filer med priser ingår alla mätare som var tillgängliga under den månaden. Om en ny mätare visas i mitten av månaden visas en mätare med ett effektivt datum som visar dess tillgänglighet. Liknande för priser som är avvecklade, och som visar ett effektivt slutdatum som beskriver när de inte längre är tillgängliga.

  - **FX-priser**: FX-priser kommer att vara tillgängliga för hämtning av dagen före den 1: e i månaden,. 18:00 PST. Om du till exempel vill ha priserna för november laddar du ned priserna den 31 oktober. Tidigare månads FX-priser kommer också att vara tillgängliga.

- Priserna i pris listorna är direkt priser. Vissa partner kan vara berättigade till partner intjänade krediter. Mer information om hur den intjänade partner krediten beräknas finns [i så här beräknas och betalas den intjänade krediten](partner-earned-credit-explanation.md).

- **Berättigade tjänster**: partner intjänad kredit gäller för tjänster som anges i **pris sättnings** samarbets [partners för](https://partner.microsoft.com/commerce/sales) Azure-prenumerationen. Obs! det finns undantag inklusive, men inte begränsat till, produkter från tredje part som identifieras som "tredje part" i kolumnen Taggar i pris listan för Azure plan-förbrukning och Azure plan-reservationer.

## <a name="price-list-data"></a>Pris List data

|**Fält**   |**Beskrivning**   |
|--------------------------|:---------------------------|
|ProductTitle  |Produktens titel eller namn|
|ProductID   |ID för produkten|
|SKuId|ID för SKU|
|SkuTitle|Rubrik eller namn på SKU|
|Publisher|den första parten är alltid Microsoft|
|SkuDescription|Beskrivning av SKU: n|
|UnitOfMeasure|Enheter som ska debiteras eller faktureras|
|TermDuration|För termbaserade produkter, längden på termen, som är tillämplig på reservationer|
|Telefonförsäljning|Marknads priser|
|Valuta|Prissättningens valuta|
|UnitPrice|Pris per enhet|
|PricingTierRangeMin|För pris nivå priser gäller minimi priset|
|PricingTierRangeMax|För pris nivå priser gäller det högsta priset|
|EffectiveStartDate|Start datum för prissättning|
|EffectiveEndDate|Slutdatum för prissättningen|
|MeterIds|Mätar-ID för produkt-SKU: n|
|MeterType|Typ av mätare|
|Taggar|Egenskaper för objektet, för priser för Azure-prenumerationen är detta Azure eller Azure och reservationer (för reservationer specifikt)|

Pris listor för Azure-plan kan exporteras från [sidan priser och erbjudanden](https://partner.microsoft.com/dashboard/sell/pricingandoffers) i Partner Center.

## <a name="tiered-pricing"></a>Pris nivå prissättning

Vissa Azure plan förbruknings tjänster stöder pris nivåer. Partner kan hitta dessa produkter och SKU: er i pris listan för Azure-abonnemang. Objekt som har värden i kolumnerna pris nivå intervall gör det möjligt för partner att förstå priset baserat på användning. I exemplet nedan med exempel data har vi en produkt-SKU med tre pris nivåer.

|**ProductId**   |**SkuId**   |**UnitPrice**   |**PricingTierRangeMin**   |**PricingTierRangeMax**   |
|:---------------|:-----------|:---------------|:-------------------------|:-------------------------|
|DDD123456ABC|01AB|.50|100001|9223372036854780000|
|DDD123456ABC|01AB|.80|101|100000|
|DDD123456ABC|01AB|1|1|100|

Om 101 enheter används i det här exemplet blir avgiften 100,80. De första 100 enheterna är var och en och nästa enhet debiteras med. 80.

## <a name="pricing-api-for-azure-plan"></a>Prissättnings-API för Azure-plan

Du kan använda [prissättnings-API: n](/partner/develop/pricing) för att hämta pris information om Azure-plan för användning och reservationer program mässigt. Du kan också hämta utländska växelkurser.

Prissättnings-API: et finns på en annan slut punkt än de andra API: erna för partner Center. Pris informationen omfattar mätar priser i USD för Azure plan-resurser och reservationer som tillämpas på Azure plan-prenumerationer.

Det här API: et gör det också möjligt för partner att hämta månatliga växelkurser eftersom priset för Azure-prenumerationen bara är USD. Du kan använda API: erna för att hämta både priser och utländska växelkurser för den aktuella månaden eller föregående månad.

>[!NOTE]
> Prissättnings-API: et är bara för pris information för Azure-prenumeration. Du bör fortfarande använda de befintliga RateCard-API: erna och pris listorna som publicerats på sidan "priser och erbjudanden" i partner centret för Azure-resurser eller-reservationer som distribueras till prenumerationer som inte tillhör Azure. Prissättnings-API: et för Azure-prenumerationen stöder inte program vara, marknads plats eller licensbaserade priser, till exempel Microsoft 365 eller Dynamics 365.

Mer information om priser för Azure-prenumeration och API: er för externa växelkurser finns i fullständig [prissättnings-API-dokumentation](/partner/develop/pricing).

## <a name="next-steps"></a>Nästa steg

- [Hantera prenumerationer och resurser under Azure-planen](azure-plan-manage.md)
