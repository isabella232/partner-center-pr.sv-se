---
title: Filer för dagligt Beräknad användnings avstämning
ms.topic: article
ms.date: 06/12/2020
description: Lär dig mer om att läsa dagliga, klassificerade användnings avstämnings filer i Partner Center. Innehåller beskrivningar av vissa fält i rekognoseringar-filen.
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 531f28ae2bceed2d854c6fb139d0abb837a047b5
ms.sourcegitcommit: e8e8362d2777d25efac3e1076af5939765ed13d0
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/20/2021
ms.locfileid: "104712247"
---
# <a name="learn-how-to-read-daily-rated-usage-reconciliation-files-in-partner-center"></a>Lär dig mer om att läsa dagliga, klassificerade användnings avstämnings filer i Partner Center

**Gäller för**

- Partnercenter
- Välkommen till Partnercenter för Microsoft Cloud for US Government

**Lämpliga roller**

- Administratörs agent
- Faktureringsadministratör
- Försäljnings agent
- Support agent

I den här artikeln förklaras hur du läser filer med dagligt Beräknad användning av filer.

>[!NOTE]
>Dagligt Beräknad användning tar normalt 24 timmar att visas i Partner Center eller nås via API: et.

## <a name="fields-in-daily-rated-usage-reconciliation-files"></a>Fält i dagligt klassificerade användnings avstämnings filer

| Kolumn | Beskrivning |
| ------ | ----------- |
| Partner | Partner-ID i GUID-format. |
| PartnerName | Partnerns namn. |
| CustomerId | Unikt Microsoft-ID för kunden i GUID-format. |
| CustomerName | Kundens organisations namn som rapporteras i Partner Center. *Den här kolumnen är viktig för att stämma av fakturan med din system information.* |
| CustomerDomainName | Kundens domän namn. |
| CustomerCountry | Det land där kunden befinner sig. |
| MpnId | MPN identifierare för CSP-partnern. |
| Tier2MpnId | MPN identifierare för åter försäljaren av posten för prenumerationen. |
| InvoiceNumber | Faktura nummer där den angivna transaktionen visas. |
| ProductId | Identifieraren för produkten. |
| SkuId | Identifieraren för en viss SKU. |
| AvailabilityId | Identifieraren för en viss SKU: s tillgänglighet. Den här kolumnen visar om SKU: n är tillgänglig för köp i angivet land, valuta, bransch segment osv. |
| SkuName | Rubriken för en viss SKU. |
| ProductName | Produktens namn. |
| PublisherName | Utgivarens namn. |
| PublisherId | Identifieraren för utgivaren i GUID-format. |
| SubscriptionDescription | Namnet på det tjänst erbjudande som kunden har köpt, enligt definitionen i pris listan. (Den här kolumnen är ett identiskt fält för **OfferName**). |
| SubscriptionId | Unikt ID för en prenumeration i Microsofts fakturerings plattform. Används inte för avstämning. *Den här identifieraren är inte samma som **prenumerations-ID: t** i partner administratörs konsolen.* |
| ChargeStartDate | Start datum för fakturerings perioden (utom när du presenterar datum för tidigare avlastade latens användnings data från föregående fakturerings period). Tiden är alltid början på dagen, 0:00. |
| ChargeEndDate | Slutdatum för fakturerings perioden (utom när du presenterar datum för tidigare avlastade latens användnings data från föregående fakturerings period). Tiden är alltid slutet på dagen, 23:59. |
| UsageDate | Datum för användning av tjänsten. |
| MeterType | Typ av mätare. |
| MeterCategory | Huvudtjänst som användningen gäller. |
| MeterId | Identifieraren för mätaren som används. |
| MeterSubCategory | Typen av Azure-tjänst, vilket kan påverka priset. |
| MeterName | Mått enheten för mätaren som används. |
| MeterRegion | Den här kolumnen identifierar platsen för ett Data Center i regionen för tjänster där MeterRegion är tillämpligt och ifyllt. |
| Enhet | Enhet för resurs **namnet**. |
| ResourceLocation | Data centret där mätaren körs. |
| ConsumedService | Den Azure-plattform som du använde. |
| ResourceGroup | Representerar en behållare som innehåller relaterade resurser för en Azure-lösning. |
| ResourceURI | URI för den resurs som används. |
| ChargeType | Typ av avgift eller justering.  |
| UnitPrice | Pris per licens, som publicerat i pris listan vid inköps tillfället. Se till att det här priset överensstämmer med informationen som lagras i fakturerings systemet under avstämningen. |
| Kvantitet | Antal licenser. Se till att det här priset överensstämmer med informationen som lagras i fakturerings systemet under avstämningen. |
| UnitType | Den typ av enhet som mätaren debiteras i.  |
| BillingPreTaxTotal | Totalt fakturerings belopp före skatt.<br/> _**BillingPreTaxTotal** = golv (([ @EffectiveUnitPrice ]*[ @Quantity ]*[ @PCToBCExchangeRate ]), 2)_ |
| BillingCurrency | Valutan i kundens geografiska region. |
| PricingPreTaxTotal | Priserna, innan skatter läggs till. |
| PricingCurrency | Valutan i prislistan. |
| ServiceInfo1 | Antalet Service Bus anslutningar som etablerades och använts på en bestämd dag. |
| ServiceInfo2 | Ett äldre fält som fångar valfria tjänstspecifika metadata. |
| Taggar | Representerar en logisk organisation av Azure-resurser som anges av användaren. |
| AdditionalInfo | Eventuell ytterligare information som inte omfattas i andra kolumner. |
| EffectiveUnitPrice | Det faktiska värdet som debiteras per enhet, inklusive eventuella rabatter, intjänad kredit och så vidare. |
| PCToBCExchangeRate | Växelkurs som tillämpas för pris valuta till fakturerings valuta. |
| PCToBCExchangeRateDate | Det datum då pris nivån för fakturerings valutan fastställs. |
| EntitlementId | Representerar ID för Azure-prenumerationen. |
| EntitlementDescription | Representerar namnet på ID för Azure-prenumerationen. |
| PartnerEarnedCreditPercentage | Visar PartnerEarnedCredit för rad objektet. Den intjänade krediten är antingen 0 eller 15 procent |
| CreditPercentage | Visar Azures förbruknings kredit. Den intjänade krediten är antingen 0 eller 100 procent. |
| CreditType | Typ av kredit. Till exempel använder **Azure-krediten.** |
>[!NOTE]
>Dagligt Beräknad användning tar normalt 24 timmar att visas i Partner Center eller nås via API.


