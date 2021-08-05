---
title: Rekognoseringsfilfält för CSP-köp vid ett tillfälle
ms.topic: conceptual
ms.date: 01/29/2021
description: Lär dig mer om alla objekt i CSP-filen för engångsköpavstämning i Partner center, inklusive exempelvärden.
ms.service: partner-dashboard
ms.subservice: partnercenter-billing
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.openlocfilehash: d5d404519c107a3e1f0e926451eef4935c993fbd
ms.sourcegitcommit: 90bf27df911b428b1222f483c32ba6367870e7c5
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/04/2021
ms.locfileid: "115100713"
---
# <a name="csp-one-time-purchase-reconciliation-file-fields"></a>Fält för CSP one-time purchase reconciliation file (CSP-fil för enköpsavstämning)

**Lämpliga roller:** Kontoadministratörsroller | Faktureringsagent

## <a name="using-the-recon-file"></a>Använda rekognoseringsfilen
Tabellen nedan innehåller beskrivningar och exempelvärden för fälten i avstämningsfilen för CSP-köp en gång.

Mer information om avstämningsfiler finns i [Använda avstämningsfilerna](use-the-reconciliation-files.md).

| Kolumn | Beskrivning | Exempelvärde |
| ------ | ----------- | ------------ |
| PartnerId | Unik identifierare i GUID-format för en specifik faktureringsenhet. Krävs inte för avstämning. Samma på alla rader. | *0e195b37-4574-4539-bc42-0e539b9684c0* |
| CustomerId | Unik Microsoft-identifierare för kunden i GUID-format. | *196e2273-9651-43a3-ba7e-7cbcd918fc40* |
| CustomerName | Kundens organisationsnamn enligt vad som rapporteras i Partnercenter. Den här kolumnen är viktig för att stämma av fakturan med systeminformationen. | *Johnny Modern Cust DE2* |
| CustomerDomainName | Kundens domännamn. | *testcustomerdomain.onmicrosoft.com* |
| CustomerCountry | Det land där kunden finns. Se den fullständiga [listan över länder](./regional-authorization-overview.md) för din region.  | *DE* |
| InvoiceNumber | Det fakturanummer som är associerat med avstämningsfilen.  | *G002297372* |
| MpnId | MPN-identifierare för CSP-partnern. Mer information finns i [hur du specificerar efter partner.](./use-the-reconciliation-files.md#itemize-reconciliation-files-by-partner) | *6034453* |
| ResellerMpnId | MPN-identifierare för återförsäljaren av posten för prenumerationen. | *6048879* |
| OrderId | Unik identifierare för en beställning på Microsofts faktureringsplattform. Kan vara användbart för att identifiera beställningen när du kontaktar supporten. Används inte för avstämning. | *0ET2qaZvJGfF9wgSKnWzR5JLmhp10lOc1* |
| OrderDate | Det datum i UTC som ordern gjordes. | *10/3/2020* |
| ProductId | Produktens unika identifierare. | *DZH318Z0BNZ5* |
| SkuId | Den unika SKU-identifieraren. | *006G* |
| AvailabilityId | Den unika identifieraren för tillgänglighet. | *DZH318Z08B80* |
| SkuName | SKU-namnet. | *Tabeller – LRS* |
| ProductName | Produktnamnet. | *Tabeller* |
| ChargeType | Typ [av avgift eller](./recon-file-charge-types.md) justering. | *Nytt* |
| UnitPrice | Pris per licens, enligt publicering i prislistan vid tidpunkten för köpet. Se till att detta matchar den information som lagras i ditt faktureringssystem under avstämningen. | *0.045* |
| Kvantitet | Antalet licenser. Se till att detta matchar den information som lagras i ditt faktureringssystem under avstämningen. | *1* |
| Delsumma | Totalsumma före skatt. Delsumman ska vara lika med den fakturerbara kvantiteten multiplicerat med det effektiva enhetspriset. | *0* |
| TaxTotal | Avgift skattebelopp. Baserat på din marknads skatteregler och specifika omständigheter. | *0* |
| Totalt | Det totala beloppet är lika med delsumman plus skattebeloppet. | *0* |
| Valuta | Fakturan genereras i kontexten för kundens valuta. Det innebär att om du är en partner som handlar med kunder från olika fakturerbara valutor får du en faktura för varje kundvalutatyp.  | *EUR* |
| PriceAdjustmentDescription | Orsakerna till justeringarna i enhetspriset. Det här är de huvudsakliga orsakerna, men inte begränsade till att fastställa det effektiva enhetspriset. | *["15,0 % partner intjänad kredit för hanterade tjänster"]* |
| PublisherName | Publisher av produkten.  | *Microsoft* |
| PublisherId | En unik identifierare som partnercentret använder för att identifiera utgivaren. | *NA* |
| SubscriptionDescription | Namnet på det tjänsterbjudande som köpts av kunden enligt definitionen i prislistan. Den här kolumnen är ett identiskt fält med OfferName. | *Azure-plan* |
| SubscriptionId | Unik identifierare för en prenumeration på Microsofts faktureringsplattform. Används inte för avstämning. Observera att den här identifieraren inte är samma som prenumerations-ID:t i partneradministratörskonsolen. | *307628f1-d9d2-f09c-ea1f-4183f0cae308* |
| ChargeStartDate | Det datum då faktureringsperioden för en prenumeration börjar. | *9/1/2020* |
| ChargeEndDate | Det datum då faktureringsperioden för en prenumeration upphör. | *2020-09-30* |
| TermAndBillingCycle | Varaktigheten för åtagandet att fortsätta prenumerationen vid tidpunkten för köpet. | *Lagrade data (GB/månad)* |
| EffectiveUnitPrice | Det prorrerade enhetspriset för att beräkna kostnaden för faktureringsperioden. Rabatter, justeringar i faktureringsdagar och andra faktorer avgör det effektiva enhetspriset. Mer information finns i [Effective Unit Price Calculation](./effective-unit-price-calculation.md).  | *0.03825* |
| UnitType | Typ av enhet där mätaren debiteras. | *1 GB/månad* |
| AlternateId | Alternativt ID för det refererade orderradsobjektet. | *6dc5c039750a* |
| BillableQuantity | Den totala kvantitet som faktureras.  | *0.005001* |
| BillingFrequency | Den faktureringsplan som valdes vid inköpet. | *NA*  |
| PricingCurrency | Valutan i prislistan. | *USD* |
| PCToBCExchangeRate | Den växelkurs som tillämpas för prissättningsvalutan för faktureringsvalutan. | *0.846202666* |
| PCToBCExchangeRateDate | Det datum då prissättningsvalutan för faktureringsvalutan bestäms. | *2020-09-30* |
| MeterDescription | Mätarbeskrivning.  | *Tabeller – LRS-lagrade data (GB/månad)* |
| ReservationOrderId | Reservationsbeställnings-ID:t. | *E21A6344E398FFC1C4D7...* |
| CreditReasonCode | Kreditbeskrivning. | *Azure-förbrukningskredit* |
| SubscriptionStartDate | Det datum då en prenumeration köps. | *5/1/2021* |
| SubscriptionEndDate | Det datum då en prenumeration upphör att gälla. | *4/30/2022* |
| ReferenceID | Länkningen till alla transaktioner som sker under uppgraderingar. | *025d68a6-1bd6-42ab-9636-15e8d776a30e* |
| ProductQualifiers | Identifierare för att känna till köp av tillägg eller utvärderingsversion. | *["Tillägg"]* |
| PromotionID | Identifieraren som ska användas för att hämta information om befordran. | *78bcf906-b945-4210-8818-cfb93caf12a1* |

>[!NOTE]
>Du kan stämma av din Azure-förbrukning i rekognoseringsfilen för ett köp en gång. Det gör du genom att gå till din dagliga avsökningsfil för användning och söka efter ditt SubscriptionID. Då visas alla kostnader som är kopplade till ditt Azure-plan-ID. Ditt Azure SubscriptionID visas som EntitlementID.
>

## <a name="how-to-connect-the-base-subscription-with-the-upgraded-subscription"></a>Hur ansluter jag basprenumerationen till den uppgraderade prenumerationen?

Du bör använda basproduktens prenumerations-ID för att hitta motsvarande referens-ID:n och använda dem för att hämta alla associerade transaktioner. I kombination med prenumerations-ID och referens-ID kan du ansluta alla uppgraderingar som inträffade i en enda händelse.

## <a name="next-steps"></a>Nästa steg

- [Fakturering och skatter](billing.md)
