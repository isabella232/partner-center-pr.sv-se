---
title: Prislista för Azure-plan för CSP-partner
ms.topic: how-to
ms.date: 05/04/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Lär dig hur CSP-programpartner kan använda Partnercenter för att se prislistan för prenumerationer under Azure-planen.
author: brentserbus
ms.author: brserbus
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 6d8e73e664d400e8e6d80e529326e566c5fd88a8
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 05/19/2021
ms.locfileid: "110149578"
---
# <a name="price-list-for-the-new-commerce-experience-in-csp-for-azure"></a>Prislista för den nya handelsupplevelsen i CSP för Azure

**Lämpliga roller:** Administratörsagent | Faktureringsadministratörskonto | Global | Supportagent | Försäljningsagentens | Administratör för användarhantering

Prislistan för den nya Azure-handelsupplevelsen i CSP publiceras i Partnercenter. Prislistan levereras dynamiskt i en korrekt realtidsfil och priserna visas endast i USD. Från och med 28 januari 2021 debiteras partner i regionen EU/EFTA och Storbritannien som har nya kunder och befintliga CSP-kunder som köper nya handelserbjudanden för första gången vars klienter skapades före den 11 maj 2020.  Partner utanför regionen EU/EFTA och Storbritannien fortsätter att debiteras i partnerns platsvaluta. Läs [Azure-plan – fakturering.](azure-plan-billing.md)

## <a name="see-pricing-for-subscriptions-under-the-azure-plan-pricing"></a>Se priser för prenumerationer under prissättningen för Azure-planen

1. I menyn i Partnercenter till vänster väljer **du Sälj** och sedan **Marketplace.**

2. Under Prissättning för Azure-plan väljer du det land som du vill ha prissättning för.

3. Bredvid Exportera **typ väljer du** priser för förbrukning för **Azure-plan,** **priser för Azure-planreservationer** eller **FX-priser.** 

>[!NOTE] 
>**FX-priser** är inte landsspecifika.

4. Bredvid **Priser för datum väljer** du det datum du vill ha, till exempel **Aktuell**.

   :::image type="content" source="images/azure/pricingnew.png" alt-text="landspecifik":::

>[!NOTE] 
>Du kan exportera två olika prislistor – priser för Azure-planer och priser från tredje part på Marketplace.

## <a name="azure-price-list-specifics"></a>Information om Azure-prislistan

- Priser för Azure-planer kommer att vara tillgängliga på Marketplace-sidan i Partnercenter, under **Sälj**.

- Exporter kommer att vara tillgängliga för förbrukningstjänster i Azure-plan, Azure-reservationer och FX-priser.

- Exportalternativen är:

  - **Dagens priser:** Detta inkluderar alla mätare och priser från den 1:a i månaden till aktuellt datum för den aktuella månaden. Detta inkluderar nya priser, ändrade priser eller borttagna priser. Alla priser har effektiva start- och slutdatum för att förklara om de är nya eller borttagna.

  - **Föregående månads priser:** Hämtningar av varje typ av resurs kommer att ske per månad. För prisfiler inkluderar detta alla mätare som var tillgängliga under den månaden. Om en ny mätare visas i mitten av månaden visas jag som en mätare med ett effektivt datum som återspeglar dess tillgänglighet. Liknande för priser som har upphört att gälla och visas med ett effektivt slutdatum som beskriver när de inte längre är tillgängliga.

  - **FX-priser:** FX-priser är tillgängliga för nedladdning dagen före den 1:a i månaden, pst kl. 18:00. Om du till exempel vill ha priserna för november laddar du ned priserna den 31 oktober. Tidigare månads FX-priser kommer också att vara tillgängliga.

- Priserna i prislistorna är direkta priser. Vissa partner kan vara berättigade till partner-intjänade krediter. Information om hur partnerns intjänade kredit beräknas finns i [Så här beräknas och betalas partnerns intjänade kredit.](partner-earned-credit-explanation.md)

- **Berättigade tjänster:** Partnerintjänad kredit gäller för tjänster som anges i prissättningspartners för **Azure-planpriser** kan exportera från [sidan med priser för Azure-plan.](https://partner.microsoft.com/commerce/sales) Observera att det finns undantag som inkluderar, men inte begränsat till, produkter från tredje part som identifieras som "tredje part" i kolumnen Taggar i prislistan för Förbrukningspris för Azure-plan och Azure-prenumerationsreservationer.

## <a name="price-list-data"></a>Prislistedata

|**Fält**   |**Beskrivning**   |
|--------------------------|:---------------------------|
|ProductTitle  |Produktens titel eller namn|
|ProductID   |ID för produkten|
|SKuId|ID för SKU|
|SkuTitle|Rubrik eller namn på SKU|
|Publisher|Första part kommer alltid att vara Microsoft|
|SkuDescription|Beskrivning av SKU:n|
|UnitOfMeasure|De enheter som debiteras eller faktureras|
|TermDuration|För termbaserade produkter, längden på termen, som gäller för reservationer|
|Marknaden|Prissättningens marknad|
|Valuta|Prissättningens valuta|
|UnitPrice|Pris per enhet|
|PricingTierRangeMin|För nivåindelade priser gäller minimipriset|
|PricingTierRangeMax|För nivåindelade priser gäller det högsta priset|
|EffectiveStartDate|Startdatum för prissättning|
|EffectiveEndDate|Slutdatum för prissättningen|
|MeterIds|Mätar-ID för produkt-SKU:n|
|MeterType|Typ av mätare|
|Taggar|Egenskaper för objektet, för priser för Azure-plan är detta Azure eller Azure och reservationer (specifikt för reservationer)|

Prislistor för Azure-plan kan exporteras från [sidan Priser och erbjudanden](https://partner.microsoft.com/dashboard/sell/pricingandoffers) i Partnercenter.

## <a name="tiered-pricing"></a>Nivåindelad prissättning

Vissa förbrukningstjänster för Azure-plan stöder nivåindelade priser. Partner hittar dessa produkter och SKU:er i prislistan för Azure-planen. Objekt som har värden i kolumnerna för prisnivåintervall gör det möjligt för partner att förstå priset baserat på användning. I exemplet nedan med exempeldata har vi en produkt-SKU med tre prisnivåer.

|**Produktionen**   |**SkuId**   |**UnitPrice**   |**PricingTierRangeMin**   |**PricingTierRangeMax**   |
|:---------------|:-----------|:---------------|:-------------------------|:-------------------------|
|DDD123456ABC|01AB|.50|100001|9223372036854780000|
|DDD123456ABC|01AB|.80|101|100000|
|DDD123456ABC|01AB|1|1|100|

I det här exemplet skulle avgiften vara 100,80 om 101 enheter används. De första 100 enheterna är en i varje och nästa enhet debiteras till 0,80.

## <a name="pricing-api-for-azure-plan"></a>Prissättnings-API för Azure-plan

Du kan använda [prissättnings-API:et](/partner/develop/pricing) för att hämta priser för Azure-planer för förbrukning och reservationer programmatiskt. Du kan också hämta växelkurser.

Prissättnings-API:et finns på en annan slutpunkt än de andra Partner Center-API:erna. Prisinformationen innehåller mätarpriser i USD för Azure-planresurser och reservationer som tillämpas på Prenumerationer på Azure-plan.

Det här API:et gör det också möjligt för partner att hämta månatliga växelkurser eftersom prissättningen för Azure-planen endast är i USD. Du kan använda API:erna för att hämta både priser och växelkurser för den aktuella månaden eller föregående månader.

>[!NOTE]
> Prissättnings-API:et är specifikt för priser för Azure-planer. Du bör fortfarande använda det befintliga RateCard-API:et och prislistorna som publiceras på partnercentrets sida "Priser och erbjudanden" för Azure-resurser eller reservationer som distribuerats till prenumerationer som inte är Azure-planer. Pris-API:et för Azure-plan stöder inte programvara, Marketplace eller licensbaserad prissättning, till exempel Microsoft 365 eller Dynamics 365.

Mer information om priser för Azure-planer och API:er för växelkurser finns i den fullständiga [api-dokumentationen för priser.](/partner/develop/pricing)

## <a name="next-steps"></a>Nästa steg

- [Hantera prenumerationer och resurser under Azure-planen](azure-plan-manage.md)
