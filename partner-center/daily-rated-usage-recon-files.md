---
title: Filer för dagligt klassificerad användningsavstämning
ms.topic: article
ms.date: 06/12/2020
description: Lär dig hur du läser filer för daglig användningsavstämning i Partnercenter. Innehåller beskrivningar för specifika fält i rekognoseringsfilen.
ms.service: partner-dashboard
ms.subservice: partnercenter-billing
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 28b61ba66fa887db5b27667318ac8f3dcfbff0a14b73925db5a7be1b77dca266
ms.sourcegitcommit: 121f1b9cbd88faeba60dc9b475f9c0647cdc933c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/06/2021
ms.locfileid: "115689312"
---
# <a name="learn-how-to-read-daily-rated-usage-reconciliation-files-in-partner-center"></a>Lär dig hur du läser filer för daglig användningsavstämning i Partnercenter

**Gäller för**: Partner Center-| Partnercenter för Microsoft Cloud for US Government

**Lämpliga roller:** Administratörsagent | Faktureringsadministratörskonto | Försäljningsagentens | Supportagent

Den här artikeln förklarar hur du läser filer för daglig användningsavstämning.

>[!NOTE]
>Daglig beräknad användning tar normalt 24 timmar att visas i Partnercenter eller nås via API:et.

## <a name="fields-in-daily-rated-usage-reconciliation-files"></a>Fält i filer för dagligt klassificerad användningsavstämning

| Kolumn | Beskrivning |
| ------ | ----------- |
| PartnerId | Partneridentifierare i GUID-format. |
| PartnerName | Partnerns namn. |
| CustomerId | Unik Microsoft-identifierare för kunden i GUID-format. |
| CustomerName | Kundens organisationsnamn enligt vad som rapporteras i Partnercenter. *Den här kolumnen är viktig för att stämma av fakturan med systeminformationen.* |
| CustomerDomainName | Kundens domännamn. |
| CustomerCountry | Det land där kunden finns. |
| MpnId | MPN-identifierare för CSP-partnern. |
| Tier2MpnId | MPN-identifierare för återförsäljaren av posten för prenumerationen. |
| InvoiceNumber | Fakturanummer där den angivna transaktionen visas. |
| ProductId | Identifieraren för produkten. |
| SkuId | Identifieraren för en viss SKU. |
| AvailabilityId | Identifieraren för en viss SKU:s tillgänglighet. Den här kolumnen visar om SKU:n är tillgänglig för inköp i det angivna landet, valutan, branschsegmentet osv. |
| SkuName | Rubriken för en viss SKU. |
| ProductName | Namnet på produkten. |
| PublisherName | Namnet på utgivaren. |
| PublisherId | Identifieraren för utgivaren i GUID-format. |
| SubscriptionDescription | Namnet på det tjänsterbjudande som köpts av kunden enligt definitionen i prislistan. (Den här kolumnen är ett identiskt fält **med OfferName**). |
| SubscriptionId | Unik identifierare för en prenumeration på Microsofts faktureringsplattform. Används inte för avstämning. *Den här identifieraren är inte samma som **prenumerations-ID:t** i partneradministratörskonsolen.* |
| ChargeStartDate | Startdatum för faktureringsperioden (förutom när du presenterar datum för tidigare ej debiterade latent användningsdata från föregående faktureringsperiod). Tiden är alltid början på dagen, 0:00. |
| ChargeEndDate | Slutdatum för faktureringsperioden (förutom när datum för tidigare ej debiterade latent användningsdata från föregående faktureringsperiod presenterats). Tiden är alltid dagens slut, 23:59. |
| UsageDate | Datum för tjänstanvändning. |
| MeterType | Typ av mätare. |
| MeterCategory | Huvudtjänst som användningen gäller. |
| MeterId | Identifieraren för den mätare som används. |
| MeterSubCategory | Typen av Azure-tjänst, vilket kan påverka priset. |
| MeterName | Måttenheten för den mätare som förbrukas. |
| MeterRegion | Den här kolumnen identifierar platsen för ett datacenter i regionen för tjänster där MeterRegion är tillämpligt och ifylld. |
| Enhet | Enheten för **resursnamnet**. |
| ResourceLocation | Datacentret där mätaren körs. |
| ConsumedService | Den Azure-plattformstjänst som du använde. |
| ResourceGroup | Representerar en container som innehåller relaterade resurser för en Azure-lösning. |
| ResourceURI | URI för resursen som används. |
| ChargeType | Typ av avgift eller justering.  |
| UnitPrice | Pris per licens, enligt vad som publicerades i prislistan vid tidpunkten för köpet. Kontrollera att det här priset matchar den information som lagras i faktureringssystemet under avstämningen. |
| Kvantitet | Antal licenser. Kontrollera att det här priset matchar den information som lagras i faktureringssystemet under avstämningen. |
| UnitType | Den typ av enhet som mätaren debiteras i.  |
| BillingPreTaxTotal | Totalt faktureringsbelopp före skatter.<br/> _**BillingPreTaxTotal** = FLOOR(([ @EffectiveUnitPrice ]*[ @Quantity ]*[ @PCToBCExchangeRate ]), 2)_ |
| BillingCurrency | Valutan i kundens geografiska region. |
| PricingPreTaxTotal | Prissättningen, innan skatter läggs till. |
| PricingCurrency | Valutan i prislistan. |
| ServiceInfo1 | Antalet anslutningar Service Bus har etablerats och använts en viss dag. |
| ServiceInfo2 | Ett äldre fält som samlar in valfria tjänstspecifika metadata. |
| Taggar | Representerar en logisk organisation av Azure-resurser som angetts av användaren. |
| AdditionalInfo | Eventuell ytterligare information som inte omfattas i andra kolumner. |
| EffectiveUnitPrice | Det faktiska värdet som debiteras per enhet, inklusive eventuella rabatter, intjänad kredit och så vidare. |
| PCToBCExchangeRate | Exchange som tillämpas för prissättningsvalutan för faktureringsvalutan. |
| PCToBCExchangeRateDate | Det datum då prissättningsvalutan för faktureringsvalutan bestäms. |
| EntitlementId | Representerar Azure-prenumerations-ID:t. |
| EntitlementDescription | Representerar namnet på Azure-prenumerations-ID:t. |
| PartnerEarnedCreditPercentage | Visar PartnerEarnedCredit för radobjektet. Intjänad kredit är antingen 0 eller 15 procent |
| CreditPercentage | Visar Azure-förbrukningskrediten. Den intjänade krediten är antingen 0 eller 100 procent. |
| CreditType | Typ av kredit. Till exempel **Tillämpad Azure-kredit.** |
>[!NOTE]
>Daglig beräknad användning tar normalt 24 timmar att visas i Partnercenter eller nås via API.


