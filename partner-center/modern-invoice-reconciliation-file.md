---
title: Rekognoseringar-filfält för CSP-inköp med ett tillfälle
ms.topic: conceptual
ms.date: 01/29/2021
description: Lär dig mer om alla objekt i din CSP-fil för inköps avstämning vid en tidpunkt i Partner Center, inklusive exempel värden.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.openlocfilehash: 66159d886914336180e8531ec07db3a9d8880a88
ms.sourcegitcommit: 766b2bb46dffd29e532b42106359f83e51b96700
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/31/2021
ms.locfileid: "106103782"
---
# <a name="csp-one-time-purchase-reconciliation-file-fields"></a>Fält för att avstämnings fil för CSP vid en tidpunkt

## <a name="using-the-recon-file"></a>Använda rekognoseringar-filen
Tabellen nedan innehåller beskrivningar och exempel värden för fälten i avstämnings filen för ett köp av CSP-tid.

Mer information om avstämnings filer finns i [använda avstämnings filer](use-the-reconciliation-files.md).

| Kolumn | Beskrivning | Exempelvärde |
| ------ | ----------- | ------------ |
| Partner | Unikt ID i GUID-format för en angiven fakturerings enhet. Krävs inte för avstämning. Samma i alla rader. | *0e195b37-4574-4539-bc42-0e539b9684c0* |
| CustomerId | Unikt Microsoft-ID för kunden i GUID-format. | *196e2273-9651-43a3-ba7e-7cbcd918fc40* |
| CustomerName | Kundens organisations namn som rapporteras i Partner Center. Den här kolumnen är viktig för att stämma av fakturan med din system information. | *Johnny modern kund-DE2* |
| CustomerDomainName | Kundens domän namn. | *testcustomerdomain.onmicrosoft.com* |
| CustomerCountry | Det land där kunden befinner sig. Se den fullständiga [listan över länder](./regional-authorization-overview.md) för din region.  | *DE* |
| InvoiceNumber | Faktura numret som är kopplat till avstämnings filen.  | *G002297372* |
| MpnId | MPN identifierare för CSP-partnern. Mer information finns i [så här specificerar du en partner](./use-the-reconciliation-files.md#itemize-reconciliation-files-by-partner). | *6034453* |
| ResellerMpnId | MPN identifierare för åter försäljaren av posten för prenumerationen. | *6048879* |
| OrderId | Unik identifierare för en beställning i Microsofts fakturerings plattform. Kan vara användbart för att identifiera ordningen när du kontaktar supporten. Används inte för avstämning. | *0ET2qaZvJGfF9wgSKnWzR5JLmhp10lOc1* |
| OrderDate | Datum då ordern placerades. | *10/3/2020* |
| ProductId | Produktens unika identifierare. | *DZH318Z0BNZ5* |
| SkuId | SKU: n unika identifierare. | *006G* |
| AvailabilityId | Unikt ID för tillgänglighet. | *DZH318Z08B80* |
| SkuName | SKU-namn. | *Tabeller – LRS* |
| ProductName | Produkt namnet. | *Tabeller* |
| ChargeType | [Typ av kostnad](./recon-file-charge-types.md) eller justering. | *Nytt* |
| UnitPrice | Pris per licens, som publicerat i pris listan vid inköps tillfället. Se till att detta matchar informationen som lagras i fakturerings systemet under avstämning. | *0,045* |
| Kvantitet | Antalet licenser. Se till att detta matchar informationen som lagras i fakturerings systemet under avstämning. | *1* |
| Delsumma | Totalt före skatt. Del summan ska vara lika med det fakturerbara antalet multiplicerat med det effektiva enhets priset. | *0* |
| TaxTotal | Avgift för moms belopp. Baserat på marknadens skatte regler och särskilda omständigheter. | *0* |
| Totalt | Den totala mängden är lika med del summan plus moms beloppet. | *0* |
| Valuta | Din faktura skapas i samband med kundens valuta. Det innebär att om du är en partner som kommunicerar med kunder från olika fakturerbara valutor får du en faktura för varje kund valuta typ.  | *EUR* |
| PriceAdjustmentDescription | Orsakerna till justeringarna i enhets priset. Detta är de viktigaste orsakerna, men inte begränsat till att fastställa det effektiva enhets priset. | *["15,0% partner intjänad kredit för tjänster som hanteras"]* |
| PublisherName | Produkt utgivare.  | *Microsoft* |
| PublisherId | En unik identifierare som partner Center använder för att identifiera utgivaren. | *NA* |
| SubscriptionDescription | Namnet på det tjänst erbjudande som kunden har köpt, enligt definitionen i pris listan. Den här kolumnen är ett identiskt fält för OfferName. | *Azure-plan* |
| SubscriptionId | Unikt ID för en prenumeration i Microsofts fakturerings plattform. Används inte för avstämning. Observera att den här identifieraren inte är samma som prenumerations-ID: t i partner administratörs konsolen. | *307628f1-d9d2-f09c-ea1f-4183f0cae308* |
| ChargeStartDate | Datumet då en prenumerations fakturerings period börjar. | *9/1/2020* |
| ChargeEndDate | Datumet då en prenumerations fakturerings period upphör. | *2020-09-30* |
| TermAndBillingCycle | Varaktighets åtagandet för att fortsätta prenumerationen vid tidpunkten för köpet. | *Lagrade data (GB/månad)* |
| EffectiveUnitPrice | Det beräknade enhets priset för att beräkna kostnaden för fakturerings perioden. Rabatter, justeringar av fakturerings dagar och andra faktorer fastställer det effektiva enhets priset. Mer information finns i [pris beräkning för effektiv enhet](./effective-unit-price-calculation.md).  | *0,03825* |
| UnitType | Den typ av enhet som mätaren debiteras i. | *1 GB/månad* |
| AlternateId | Alternativt-ID för det refererade order rads objektet. | *6dc5c039750a* |
| BillableQuantity | Det totala antalet som faktureras.  | *0,005001* |
| BillingFrequency | Den fakturerings plan som valts vid inköps tillfället. | *NA*  |
| PricingCurrency | Valutan i prislistan. | *USD* |
| PCToBCExchangeRate | Växelkursen som används för pris valutan till fakturerings valutan. | *0,846202666* |
| PCToBCExchangeRateDate | Det datum då pris nivån för fakturerings valutan fastställs. | *2020-09-30* |
| MeterDescription | Beskrivning av mätare.  | *Tabeller – LRS data lagring (GB/månad)* |
| ReservationOrderId | ID för reservations order. | *E21A6344E398FFC1C4D7...* |
| CreditReasonCode | Kredit beskrivningen. | *Azures förbruknings kredit* |

>[!NOTE]
>Du kan stämma av din Azure-förbrukning i din rekognoseringar-fil för inköp i taget. Det gör du genom att gå till din dagliga rekognoseringar-fil för användning och söka efter ditt SubscriptionID. Detta visar alla kostnader som är kopplade till ditt Azure-Plans-ID. Ditt Azure-SubscriptionID visas som EntitlementID.

## <a name="next-steps"></a>Nästa steg

- [Fakturering och skatter](billing.md)
