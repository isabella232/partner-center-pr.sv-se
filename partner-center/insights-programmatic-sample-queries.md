---
title: Lista över exempelfrågor
description: Använd exempelfrågorna för att programmatiskt komma åt analysdata för partnerinsikter.
ms.topic: reference
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 07/14/2021
ms.openlocfilehash: e25784585a1ac505db99e58265939a8851edcbad
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 07/16/2021
ms.locfileid: "114376940"
---
# <a name="sample-queries-for-partner-center-insights-report"></a><span data-ttu-id="1285f-103">Exempelfrågor för partnercenterinsiktsrapport</span><span class="sxs-lookup"><span data-stu-id="1285f-103">Sample queries for Partner Center insights report</span></span>

<span data-ttu-id="1285f-104">Den här artikeln innehåller exempelfrågor för partnerrapporterna Insights rapporter.</span><span class="sxs-lookup"><span data-stu-id="1285f-104">This article provides sample queries for the Partner Insights reports.</span></span> <span data-ttu-id="1285f-105">Du kan använda dessa frågor genom att anropa slutpunkten för API:et Skapa rapportfråga.</span><span class="sxs-lookup"><span data-stu-id="1285f-105">You can use these queries by calling the Create Report Query API endpoint.</span></span> <span data-ttu-id="1285f-106">Om det behövs kan [api-anropet Skapa](insights-programmatic-access-paradigm.md#create-report-query-api) rapportfråga ändras för att lägga till fler kolumner, justera beräkningsperioden och lägga till filtervillkor.</span><span class="sxs-lookup"><span data-stu-id="1285f-106">If necessary, the [Create Report Query API](insights-programmatic-access-paradigm.md#create-report-query-api) call can be modified to add more columns, adjust the computation period, and add filter conditions.</span></span>

<span data-ttu-id="1285f-107">Mer information om kolumnnamn, attribut och beskrivningar finns i [Datadefinitioner.](insights-data-definitions.md)</span><span class="sxs-lookup"><span data-stu-id="1285f-107">For details about the column names, attributes, and descriptions, refer to the [Data Definitions](insights-data-definitions.md).</span></span>

## <a name="customer-details"></a><span data-ttu-id="1285f-108">Kundinformation</span><span class="sxs-lookup"><span data-stu-id="1285f-108">Customer details</span></span>

<span data-ttu-id="1285f-109">Dessa exempelfrågor gäller för kundinformationsrapporten:</span><span class="sxs-lookup"><span data-stu-id="1285f-109">These sample queries apply to the customers details report:</span></span>

### <a name="by-geography"></a><span data-ttu-id="1285f-110">Efter geografiskt område</span><span class="sxs-lookup"><span data-stu-id="1285f-110">By geography</span></span>

<span data-ttu-id="1285f-111">Lista över kunder från ett visst geografiskt område under den senaste månaden.</span><span class="sxs-lookup"><span data-stu-id="1285f-111">List of customers from a specific geography in last month.</span></span>

```sql
SELECT CustomerName, CustomerTpid, Product 
FROM CustomersAndTenants 
WHERE CustomerMarket='United States' TIMESPAN LAST_MONTH
```

### <a name="by-sku-and-billed-revenue"></a><span data-ttu-id="1285f-112">Efter SKU och fakturerade intäkter</span><span class="sxs-lookup"><span data-stu-id="1285f-112">By SKU and billed revenue</span></span>

<span data-ttu-id="1285f-113">En lista över kunder som använder en specifik SKU och fakturerade intäkter är fler än 20 000 under de senaste 6 månaderna</span><span class="sxs-lookup"><span data-stu-id="1285f-113">List of customers using specific SKU and Billed Revenue is more than 20,000 in the last 6 months</span></span>

```sql
SELECT CustomerName, CustomerTpid, SKU, Month, BilledRevenueUSD 
FROM CustomersAndTenants 
WHERE SKU='MICROSOFT 365 BUSINESS STANDARD' AND BilledRevenueUSD>20000 TIMESPAN LAST_6_MONTHS
```

### <a name="by-available-seats"></a><span data-ttu-id="1285f-114">Efter tillgängliga platser</span><span class="sxs-lookup"><span data-stu-id="1285f-114">By available seats</span></span>

<span data-ttu-id="1285f-115">De 10 främsta kunderna baserat på tillgängliga platser under den senaste månaden</span><span class="sxs-lookup"><span data-stu-id="1285f-115">Top 10 customers based on Available seats in last month</span></span>

```sql
SELECT CustomerName, CustomerTpid, Product, AvailableSeats 
FROM CustomersAndTenants ORDER BY AvailableSeats DESC LIMIT 10 TIMESPAN LAST_MONTH
```

## <a name="partner-profile"></a><span data-ttu-id="1285f-116">Partnerprofil</span><span class="sxs-lookup"><span data-stu-id="1285f-116">Partner Profile</span></span>

<span data-ttu-id="1285f-117">Dessa exempelfrågor gäller för partnerprofilrapporten:</span><span class="sxs-lookup"><span data-stu-id="1285f-117">These sample queries apply to the partner profile report:</span></span>

### <a name="by-geography"></a><span data-ttu-id="1285f-118">Efter geografiskt område</span><span class="sxs-lookup"><span data-stu-id="1285f-118">By geography</span></span>

<span data-ttu-id="1285f-119">Lista över partner från ett visst geografiskt område.</span><span class="sxs-lookup"><span data-stu-id="1285f-119">List of partners from a specific geography.</span></span>

```sql
SELECT MPNId, PartnerName 
FROM Profile 
WHERE Country='United States'
```

### <a name="by-mpn-partner"></a><span data-ttu-id="1285f-120">Av MPN-partner</span><span class="sxs-lookup"><span data-stu-id="1285f-120">By MPN partner</span></span>

<span data-ttu-id="1285f-121">Lista över partner under samma PGA MPN-partner</span><span class="sxs-lookup"><span data-stu-id="1285f-121">List of partners under same PGA MPN Partner</span></span>

```sql
SELECT MPNId, PartnerName, PGAMpnId 
FROM Profile 
WHERE PGAMpnId='1001xx'
```

## <a name="reseller-performance"></a><span data-ttu-id="1285f-122">Återförsäljares prestanda</span><span class="sxs-lookup"><span data-stu-id="1285f-122">Reseller Performance</span></span>

<span data-ttu-id="1285f-123">Dessa exempelfrågor gäller för återförsäljares prestandarapport:</span><span class="sxs-lookup"><span data-stu-id="1285f-123">These sample queries apply to the reseller performance report:</span></span>

### <a name="by-geography"></a><span data-ttu-id="1285f-124">Efter geografiskt område</span><span class="sxs-lookup"><span data-stu-id="1285f-124">By geography</span></span>

<span data-ttu-id="1285f-125">Lista över återförsäljare från ett visst geografiskt område under den senaste månaden.</span><span class="sxs-lookup"><span data-stu-id="1285f-125">List of resellers from a specific geography in last month.</span></span>

```sql
SELECT ResellerMpnId, ResellerName 
FROM ResellerPerformance 
WHERE ResellerMarket='US' TIMESPAN LAST_MONTH
```

### <a name="by-reseller"></a><span data-ttu-id="1285f-126">Efter återförsäljare</span><span class="sxs-lookup"><span data-stu-id="1285f-126">By reseller</span></span>

<span data-ttu-id="1285f-127">Kundantal, prenumerationsantal, totalt antal tillgängliga platser, totalt antal tilldelade platser, totala intäkter för en specifik återförsäljare.</span><span class="sxs-lookup"><span data-stu-id="1285f-127">Customer count, subscription count, total available seats, total assigned seats, total revenue for a specific reseller.</span></span>

```sql
SELECT ResellerMpnId, ResellerName, CustomerCount, SubscriptionCount, TotalAvailableSeats, TotalAssignedSeats, TotalRevenue 
FROM ResellerPerformance 
WHERE ResellerMpnId='1051xxx'
```

### <a name="top-10-by-revenue"></a><span data-ttu-id="1285f-128">De 10 främsta efter intäkter</span><span class="sxs-lookup"><span data-stu-id="1285f-128">Top 10 by revenue</span></span>

<span data-ttu-id="1285f-129">De 10 främsta återförsäljarna baserat på de totala intäkterna under den senaste månaden.</span><span class="sxs-lookup"><span data-stu-id="1285f-129">Top 10 resellers based on total revenue in last month.</span></span>

```sql
SELECT ResellerMpnId, ResellerName, TotalRevenue 
FROM ResellerPerformance 
ORDER BY TotalRevenue 
LIMIT 10 
TIMESPAN LAST_MONTH
```

## <a name="subscription-details"></a><span data-ttu-id="1285f-130">Prenumerationsinformation</span><span class="sxs-lookup"><span data-stu-id="1285f-130">Subscription Details</span></span>

<span data-ttu-id="1285f-131">De här exempelfrågorna gäller för prenumerationsinformationsrapporten:</span><span class="sxs-lookup"><span data-stu-id="1285f-131">These sample queries apply to the subscription details report:</span></span>

### <a name="by-renewal-eligibility"></a><span data-ttu-id="1285f-132">Efter berättigande till förnyelse</span><span class="sxs-lookup"><span data-stu-id="1285f-132">By renewal eligibility</span></span>

<span data-ttu-id="1285f-133">Lista över prenumerationer som inte är berättigade till automatisk förnyelse under den senaste månaden.</span><span class="sxs-lookup"><span data-stu-id="1285f-133">List of subscriptions who are not eligible for auto renewal in last month.</span></span>

```sql
SELECT SubscriptionId, SubscriptionEndDate, CustomerName, CustomerTpid, Product 
FROM SeatsSubscriptionsAndRevenue 
WHERE IsAutoRenew='N' TIMESPAN LAST_MONTH
```

### <a name="by-subscription-state"></a><span data-ttu-id="1285f-134">Efter prenumerationstillstånd</span><span class="sxs-lookup"><span data-stu-id="1285f-134">By subscription state</span></span>

<span data-ttu-id="1285f-135">Lista över prenumerationer som har statusen Inaktivera under den senaste månaden.</span><span class="sxs-lookup"><span data-stu-id="1285f-135">List of subscriptions who are in Disable state in last month.</span></span>

```sql
SELECT SubscriptionId, SubscriptionEndDate, CustomerName, CustomerTpid, Product 
FROM SeatsSubscriptionsAndRevenue 
WHERE SubscriptionState='Disabled' TIMESPAN LAST_MONTH
```

### <a name="counts-for-six-months"></a><span data-ttu-id="1285f-136">Antal i sex månader</span><span class="sxs-lookup"><span data-stu-id="1285f-136">Counts for six months</span></span>

<span data-ttu-id="1285f-137">Antal prenumerationer, totalt antal sålda platser, kundantal för en specifik partner under de senaste sex månaderna.</span><span class="sxs-lookup"><span data-stu-id="1285f-137">Subscription count, total sold seats, customer count for a specific partner in last six months.</span></span>

```sql
SELECT MPNId, SubscriptionCount, TotalSoldSeats, BilledRevenueUSD, CustomerCount 
FROM SeatsSubscriptionsAndRevenue 
WHERE MPNId=6096xxx TIMESPAN LAST_6_MONTHS
```

## <a name="azure-usage"></a><span data-ttu-id="1285f-138">Azure-användning</span><span class="sxs-lookup"><span data-stu-id="1285f-138">Azure Usage</span></span>

<span data-ttu-id="1285f-139">De här exempelfrågorna gäller för Azure-användningsrapporten:</span><span class="sxs-lookup"><span data-stu-id="1285f-139">These sample queries apply to the Azure usage report:</span></span>

### <a name="by-meter-category"></a><span data-ttu-id="1285f-140">Efter mätarkategori</span><span class="sxs-lookup"><span data-stu-id="1285f-140">By meter category</span></span>

<span data-ttu-id="1285f-141">Lista över Azure-användningsprenumerationer med användningsenheter och ACR för specifik mätarkategori under de senaste sex månaderna.</span><span class="sxs-lookup"><span data-stu-id="1285f-141">List of Azure usage subscriptions with usage units and ACR for specific meter category in last six months.</span></span>

```sql
SELECT SubscriptionId, CustomerName, Month, UsageUnits, UsageQuantity, TotalACR 
FROM AzureUsage 
WHERE MeterCategory='Azure DNS' 
TIMESPAN LAST_6_MONTHS
```

### <a name="by-total-acr"></a><span data-ttu-id="1285f-142">Efter totalt ACR</span><span class="sxs-lookup"><span data-stu-id="1285f-142">By total ACR</span></span>

<span data-ttu-id="1285f-143">Lista över Azure-användningsprenumerationer där det totala antalet ACR är större än 20 000 under de senaste sex månaderna</span><span class="sxs-lookup"><span data-stu-id="1285f-143">List of Azure usage subscriptions where total ACR is greater than 20,000 in last six months</span></span>

```sql
SELECT SubscriptionId, ServiceName, CustomerName, Month, UsageUnits, UsageQuantity, TotalACR 
FROM AzureUsage 
WHERE TotalACR>20000 TIMESPAN LAST_6_MONTHS
```

## <a name="next-steps"></a><span data-ttu-id="1285f-144">Nästa steg</span><span class="sxs-lookup"><span data-stu-id="1285f-144">Next steps</span></span>

- [<span data-ttu-id="1285f-145">API:er för åtkomst till analysdata för partnerinsikter</span><span class="sxs-lookup"><span data-stu-id="1285f-145">APIs for accessing partner insights analytics data</span></span>](insights-programmatic-analytics-available-api.md)