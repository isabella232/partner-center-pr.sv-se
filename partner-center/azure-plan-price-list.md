---
title: Prislista för Azure-plan för CSP-partner
ms.topic: how-to
ms.date: 07/21/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
description: Lär dig hur CSP-programpartner kan använda Partnercenter för att se prislistan för prenumerationer under Azure-planen.
author: brentserbus
ms.author: brserbus
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 750dd081ea9486173b933e290c7c186f8e0844016c92100d828f1fdc0fa765b5
ms.sourcegitcommit: 121f1b9cbd88faeba60dc9b475f9c0647cdc933c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/06/2021
ms.locfileid: "115680845"
---
# <a name="price-list-for-the-new-commerce-experience-in-csp-for-azure"></a>Prislista för den nya handelsupplevelsen i CSP för Azure

**Lämpliga roller:** Administratörsagent | Faktureringsadministratörskonto | Global | Supportagent | Försäljningsagentens | Administratör för användarhantering

Realtidspriserna för den nya Azure-handelsupplevelsen i CSP levereras dynamiskt i realtid på Partnercenter. Priserna visas endast i USD. Från och med den 28 januari 2021 debiteras alla partner i regionen EU/EFTA och Storbritannien som har nya eller befintliga CSP-kunder för första gången och dessa klienter skapades före den 11 maj 2020 för dessa köp i partnerns platsvaluta. Partner utanför regionen EU/EFTA och Storbritannien fortsätter att debiteras i valuta för partnerplats. Mer information finns i [Azure-plan – fakturering.](azure-plan-billing.md)

Som en del av den nya handelsupplevelsen för Azure i CSP har vi introducerat ett [nytt Azure-erbjudande.](./azure-plan-lp.md) Viktiga datum som rör det tidigare Azure-erbjudandet (MS-AZR-0145p) finns i [erbjudandedokumentet](https://go.microsoft.com/fwlink/p/?linkid=2164140).

Om du har registrerat dig *före* 21 juli 2021
- Du kommer att fortsätta att se det tidigare Azure-erbjudandet i prislistan.

Om du har registrerat *dig den 21* juli 2021 eller senare
- Du ser *inte* det tidigare Azure-erbjudandet i prislistan.

## <a name="see-pricing-for-subscriptions-under-the-azure-plan-pricing"></a>Se priser för prenumerationer under prissättningen för Azure-planen

1.  I menyn i Partnercenter väljer du **Sälj** och sedan **Priser och erbjudanden.**
2.  Under **Prissättning för Azure-planförbrukning** **och prissättning för Azure-planreservationer** väljer du land och sedan nedladdningslänken.
   - För **Växelkurser** väljer du nedladdningslänken under avsnittet .

   > [!NOTE] 
   > **FX-priser** är inte landsspecifika.

   :::image type="content" source="images/azure/pricing-new.png" alt-text="Skärmbild av priser och erbjudanden som visar den nya handelsupplevelsen.":::

   > [!NOTE] 
   > Du kan exportera två olika prislistor: priser för Azure-planer och priser från tredje part på Marketplace.

## <a name="azure-price-list-specifics"></a>Information om Azure-prislistan

- Priser för Azure-planer kommer att vara tillgängliga **på sidan Priser** och erbjudanden i Partnercenter, under **Sälj**.

- Exporter kommer att vara tillgängliga för förbrukningstjänster i Azure-planer, Azure-reservationer och FX-priser.

- Exportalternativen är:

  - **Aktuell prissättning:** Det här alternativet innehåller alla mätare och priser från den första i månaden till det aktuella datumet i månaden, till exempel nya priser, ändrade priser eller borttagna priser. Alla priser har effektiva start- och slutdatum för att förklara om de är nya eller borttagna.

  - **Priser för föregående månad:** Hämtningar av varje typ av resurs kommer att ske per månad. För prisfiler inkluderar detta alla mätare som var tillgängliga under den månaden. Om en ny mätare visas i mitten av månaden visas jag som en mätare med ett effektivt datum som återspeglar dess tillgänglighet. Liknande för priser som upphör att gälla och visas med ett effektivt slutdatum som beskriver när de inte längre är tillgängliga.

  - **FX-priser:** FX-priser är tillgängliga för nedladdning dagen före den 1:a i månaden, 18:00 PST. Om du till exempel vill ha priserna för november laddar du ned priserna den 31 oktober. Tidigare månads FX-priser kommer också att vara tillgängliga.

- Priserna i prislistorna är direkta priser. Vissa partner kan vara berättigade till partner-intjänade krediter. Information om hur partnerns intjänade kredit beräknas finns i [Så här beräknas och betalas partnerns intjänade kredit.](partner-earned-credit-explanation.md)

- **Berättigade tjänster:** Partnerintjänad kredit gäller för tjänster som anges i prissättningspartnerna för **Azure-planförbrukning** kan exportera från [sidan med priser för Azure-plan.](https://partner.microsoft.com/commerce/sales)
   > [!NOTE]
   > Det finns undantag, inklusive, men inte begränsat till, produkter från  tredje part som identifierats som "Tredje part" i kolumnen Taggar i azure-planens förbrukningsprislista och Azure-planreservationer.

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

Vissa förbrukningstjänster i Azure-plan har stöd för nivåindelade priser. Partner hittar dessa produkter och SKU:er i prislistan för Azure-planen. Objekt som har värden i kolumnerna för prisnivåintervall gör det möjligt för partner att förstå priset baserat på användning. I exemplet nedan med exempeldata har vi en produkt-SKU med tre prisnivåer.

|**Produktionen**   |**SkuId**   |**UnitPrice**   |**PricingTierRangeMin**   |**PricingTierRangeMax**   |
|:---------------|:-----------|:---------------|:-------------------------|:-------------------------|
|DDD123456ABC|01AB|0,50|100001|9223372036854780000|
|DDD123456ABC|01AB|0,80|101|100000|
|DDD123456ABC|01AB|1|1|100|

Om 101 enheter används i det här exemplet skulle avgiften vara 100,80. De första 100 enheterna är en i varje och nästa enhet debiteras vid 0,80.

## <a name="pricing-api-for-azure-plan"></a>Prissättnings-API för Azure-plan

Du kan använda [prissättnings-API:et](/partner/develop/pricing) för att hämta priser för Azure-planer för förbrukning och reservationer programmatiskt. Du kan också hämta växelkurser.

Prissättnings-API:et finns på en annan slutpunkt än de andra Partner Center-API:erna. Prisinformationen innehåller mätarpriser i USD för Azure-planresurser och priser för reservationer som tillämpas på Prenumerationer på Azure-plan.

Det här API:et gör det också möjligt för partner att hämta månatliga växelkurser eftersom priserna för Azure-planen endast är i USD. Du kan använda API:erna för att hämta både priser och växelkurser för den aktuella månaden eller föregående månader.

> [!NOTE]
> Prissättnings-API:et är specifikt för priser för Azure-planer. Du bör fortfarande använda det befintliga RateCard-API:et och prislistorna som publicerats på partnercentrets sida "Priser och erbjudanden" för Azure-resurser eller reservationer som distribuerats till prenumerationer som inte är Azure-planer. Pris-API:et för Azure-planer stöder inte programvara, Marketplace- eller licensbaserad prissättning, till exempel Microsoft 365 eller Dynamics 365.

Mer information om priser för Azure-planer och API:er för växelkurser finns i den fullständiga [api-dokumentationen för priser.](/partner/develop/pricing)

## <a name="next-steps"></a>Nästa steg

- [Hantera prenumerationer och resurser under Azure-planen](azure-plan-manage.md)
