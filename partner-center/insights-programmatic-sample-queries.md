---
title: Lista över exempelfrågor
description: Använd exempelfrågorna för att programmatiskt komma åt analysdata från partnerinsikter.
ms.topic: reference
ms.service: partner-dashboard
ms.subservice: partnercenter-insights
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.date: 07/14/2021
ms.openlocfilehash: 18e50ec8108f5998b57630960026d039ab68803a
ms.sourcegitcommit: d731813da1d31519dc2dc583d17899e5cf4ec1b2
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/27/2021
ms.locfileid: "129075337"
---
# <a name="sample-queries-for-partner-center-insights-report"></a>Exempelfrågor för partnercenterinsiktsrapport

Den här artikeln innehåller exempelfrågor för Partner Insights rapporter. Du kan använda de här frågorna genom att anropa slutpunkten för API:et Skapa rapportfråga. Om det behövs kan [anropet Skapa rapportfråge-API](insights-programmatic-access-paradigm.md#create-report-query-api) ändras för att lägga till fler kolumner, justera beräkningsperioden och lägga till filtervillkor.

Mer information om kolumnnamn, attribut och beskrivningar finns i [Datadefinitioner.](insights-data-definitions.md)

## <a name="customer-details"></a>Kundinformation

Dessa exempelfrågor gäller för kundinformationsrapporten:

### <a name="by-geography"></a>Efter geografiskt område

Lista över kunder från ett visst geografiskt område under den senaste månaden.

```sql
SELECT CustomerName, CustomerTpid, Product 
FROM CustomersAndTenants 
WHERE CustomerMarket='United States' TIMESPAN LAST_MONTH
```

### <a name="by-sku-and-billed-revenue"></a>Efter SKU och fakturerade intäkter

Lista över kunder som använder specifik SKU och fakturerade intäkter är mer än 20 000 under de senaste 6 månaderna

```sql
SELECT CustomerName, CustomerTpid, SKU, Month, BilledRevenueUSD 
FROM CustomersAndTenants 
WHERE SKU='MICROSOFT 365 BUSINESS STANDARD' AND BilledRevenueUSD>20000 TIMESPAN LAST_6_MONTHS
```

### <a name="by-available-seats"></a>Efter tillgängliga platser

De 10 främsta kunderna baserat på tillgängliga platser under den senaste månaden

```sql
SELECT CustomerName, CustomerTpid, Product, AvailableSeats 
FROM CustomersAndTenants ORDER BY AvailableSeats DESC LIMIT 10 TIMESPAN LAST_MONTH
```

## <a name="partner-profile"></a>Partnerprofil

Dessa exempelfrågor gäller för partnerprofilrapporten:

### <a name="by-geography"></a>Efter geografiskt område

Lista över partner från ett visst geografiskt område.

```sql
SELECT MPNId, PartnerName 
FROM Profile 
WHERE Country='United States'
```

### <a name="by-mpn-partner"></a>Av MPN-partner

Lista över partner under samma PGA MPN-partner

```sql
SELECT MPNId, PartnerName, PGAMpnId 
FROM Profile 
WHERE PGAMpnId='1001xx'
```

## <a name="reseller-performance"></a>Återförsäljares prestanda

De här exempelfrågorna gäller för återförsäljares prestandarapport:

### <a name="by-geography"></a>Efter geografiskt område

Lista över återförsäljare från ett visst geografiskt område under den senaste månaden.

```sql
SELECT ResellerMpnId, ResellerName 
FROM ResellerPerformance 
WHERE ResellerMarket='US' TIMESPAN LAST_MONTH
```

### <a name="by-reseller"></a>Efter återförsäljare

Antal kunder, prenumerationsantal, totalt antal tillgängliga platser, totalt antal tilldelade platser, totala intäkter för en specifik återförsäljare.

```sql
SELECT ResellerMpnId, ResellerName, CustomerCount, SubscriptionCount, TotalAvailableSeats, TotalAssignedSeats, TotalRevenue 
FROM ResellerPerformance 
WHERE ResellerMpnId='1051xxx'
```

### <a name="top-10-by-revenue"></a>De 10 främsta efter intäkter

De 10 främsta återförsäljarna baserat på de totala intäkterna under den senaste månaden.

```sql
SELECT ResellerMpnId, ResellerName, TotalRevenue 
FROM ResellerPerformance 
ORDER BY TotalRevenue 
LIMIT 10 
TIMESPAN LAST_MONTH
```

## <a name="subscription-details"></a>Prenumerationsinformation

Dessa exempelfrågor gäller för rapporten med prenumerationsinformation:

### <a name="by-renewal-eligibility"></a>Efter berättigande till förnyelse

Lista över prenumerationer som inte är berättigade till automatisk förnyelse under den senaste månaden.

```sql
SELECT SubscriptionId, SubscriptionEndDate, CustomerName, CustomerTpid, Product 
FROM SeatsSubscriptionsAndRevenue 
WHERE IsAutoRenew='N' TIMESPAN LAST_MONTH
```

### <a name="by-subscription-state"></a>Efter prenumerationstillstånd

Lista över prenumerationer som har statusen Inaktivera under den senaste månaden.

```sql
SELECT SubscriptionId, SubscriptionEndDate, CustomerName, CustomerTpid, Product 
FROM SeatsSubscriptionsAndRevenue 
WHERE SubscriptionState='Disabled' TIMESPAN LAST_MONTH
```

### <a name="counts-for-six-months"></a>Antal i sex månader

Antal prenumerationer, totalt antal sålda platser, kundantal för en specifik partner under de senaste sex månaderna.

```sql
SELECT MPNId, SubscriptionCount, TotalSoldSeats, BilledRevenueUSD, CustomerCount 
FROM SeatsSubscriptionsAndRevenue 
WHERE MPNId=6096xxx TIMESPAN LAST_6_MONTHS
```

## <a name="azure-usage"></a>Azure-användning

De här exempelfrågorna gäller för Azure-användningsrapporten:

### <a name="by-meter-category"></a>Efter mätarkategori

Lista över Azure-användningsprenumerationer med användningsenheter och ACR för specifik mätarkategori under de senaste sex månaderna.

```sql
SELECT SubscriptionId, CustomerName, Month, UsageUnits, UsageQuantity, TotalACR 
FROM AzureUsage 
WHERE MeterCategory='Azure DNS' 
TIMESPAN LAST_6_MONTHS
```

### <a name="by-total-acr"></a>Efter totalt ACR

Lista över Azure-användningsprenumerationer där det totala antalet ACR är större än 20 000 under de senaste sex månaderna

```sql
SELECT SubscriptionId, ServiceName, CustomerName, Month, UsageUnits, UsageQuantity, TotalACR 
FROM AzureUsage 
WHERE TotalACR>20000 TIMESPAN LAST_6_MONTHS
```

## <a name="next-steps"></a>Nästa steg

- [API:er för åtkomst till analysdata från partnerinsikter](insights-programmatic-analytics-available-api.md)