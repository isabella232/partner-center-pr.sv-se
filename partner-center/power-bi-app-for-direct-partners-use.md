---
title: Använd partner Center Analytics för Power BI
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Lär dig hur du visar dina affärs data med hjälp av Partner Center Analytics-appen för Power BI (för direkta partner i CSP).
fwlink: https://go.microsoft.com/fwlink/?linkid=852581
author: v-sumukh
ms.author: v-sumukh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: f5bdb166562593b970f40c23921dc80b2a1cb8ad
ms.sourcegitcommit: a691d4cbe144a8fd71e344fd293cc658ac11d6f3
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/27/2021
ms.locfileid: "105633870"
---
# <a name="view-your-business-data-with-the-partner-center-analytics-app-for-microsoft-power-bi"></a><span data-ttu-id="f9279-103">Visa dina affärs data med partner Center Analytics-appen för Microsoft Power BI</span><span class="sxs-lookup"><span data-stu-id="f9279-103">View your business data with the Partner Center Analytics app for Microsoft Power BI</span></span>



<span data-ttu-id="f9279-104">**Lämpliga roller**</span><span class="sxs-lookup"><span data-stu-id="f9279-104">**Appropriate roles**</span></span>

- <span data-ttu-id="f9279-105">Global administratör</span><span class="sxs-lookup"><span data-stu-id="f9279-105">Global admin</span></span>
- <span data-ttu-id="f9279-106">Administratör för användar hantering</span><span class="sxs-lookup"><span data-stu-id="f9279-106">User management admin</span></span>
- <span data-ttu-id="f9279-107">Försäljnings agent</span><span class="sxs-lookup"><span data-stu-id="f9279-107">Sales agent</span></span>
- <span data-ttu-id="f9279-108">Administratörs agent</span><span class="sxs-lookup"><span data-stu-id="f9279-108">Admin agent</span></span>

## <a name="view-your-business-data"></a><span data-ttu-id="f9279-109">Visa dina affärs data</span><span class="sxs-lookup"><span data-stu-id="f9279-109">View your business data</span></span>

<span data-ttu-id="f9279-110">Få en visuell representation av dina affärs data med partner Center Analytics-appen för Power BI, inklusive:</span><span class="sxs-lookup"><span data-stu-id="f9279-110">Get a visual representation of your business data with the Partner Center Analytics app for Power BI, including:</span></span>

- <span data-ttu-id="f9279-111">Tillväxt av kund basen, prenumerationer och licenser</span><span class="sxs-lookup"><span data-stu-id="f9279-111">Growth of your customer base, subscriptions, and licenses</span></span>

- <span data-ttu-id="f9279-112">Användning av Office 365, Microsoft Dynamics och Microsoft Azure produkter</span><span class="sxs-lookup"><span data-stu-id="f9279-112">Usage of Office 365, Microsoft Dynamics, and Microsoft Azure products</span></span>

- <span data-ttu-id="f9279-113">Dagliga förbruknings enheter för varje avgiftsbelagd resurs i varje Azure-prenumeration under de senaste 60 dagarna</span><span class="sxs-lookup"><span data-stu-id="f9279-113">Daily consumption units for each metered resource in each Azure subscription for the last 60 days</span></span>

- <span data-ttu-id="f9279-114">Beräknad kostnad (baserat på senaste pris kortet)</span><span class="sxs-lookup"><span data-stu-id="f9279-114">Estimated cost (based on latest rate card)</span></span>

- <span data-ttu-id="f9279-115">Möjlighet att exportera data uppsättningar och skapa anpassade rapporter, inklusive per kund.</span><span class="sxs-lookup"><span data-stu-id="f9279-115">Ability to export datasets and create custom reports, including per customer.</span></span>

### <a name="about-the-partner-center-analytics-app-preview-release"></a><span data-ttu-id="f9279-116">Om för hands versionen av Partner Center Analytics-appen</span><span class="sxs-lookup"><span data-stu-id="f9279-116">About the Partner Center Analytics app preview release</span></span>

- <span data-ttu-id="f9279-117">Den här appen är endast för direkta partner i Cloud Solution Provider-programmet.</span><span class="sxs-lookup"><span data-stu-id="f9279-117">This app is for direct partners in the Cloud Solution Provider program only.</span></span> <span data-ttu-id="f9279-118">Andra partner i CSP (indirekt åter försäljare, till exempel) kan inte logga in.</span><span class="sxs-lookup"><span data-stu-id="f9279-118">Other partners in CSP (indirect resellers, for example) will not be able to sign in.</span></span>

- <span data-ttu-id="f9279-119">Eventuella beräknade kostnader är fakturerings-och faktura data för moms, och är inte juridiskt bindande.</span><span class="sxs-lookup"><span data-stu-id="f9279-119">Any estimated costs are pre-tax billing / invoice data, and are not legally binding.</span></span> <span data-ttu-id="f9279-120">Uppskattade kostnader är avsedda att användas enbart för data insikter.</span><span class="sxs-lookup"><span data-stu-id="f9279-120">Estimated costs are meant to be used for data insights only.</span></span>

- <span data-ttu-id="f9279-121">Kund information baseras på prenumerationer.</span><span class="sxs-lookup"><span data-stu-id="f9279-121">Customer information is based on subscriptions.</span></span> <span data-ttu-id="f9279-122">Alla kunder som du nyligen har skapat konton för, men som ännu inte har några prenumerationer, ingår inte i antal.</span><span class="sxs-lookup"><span data-stu-id="f9279-122">Any customers that you've recently created accounts for, but who don't yet have subscriptions, aren't included in counts.</span></span>

- <span data-ttu-id="f9279-123">Den uppskattade kostnaden baseras på det senaste avgifts kortet, som baseras på CSP-priset.</span><span class="sxs-lookup"><span data-stu-id="f9279-123">Estimated cost is based on latest rate card, which is based on CSP pricing.</span></span>

- <span data-ttu-id="f9279-124">Dagar är kalender dagar.</span><span class="sxs-lookup"><span data-stu-id="f9279-124">Days are calendar days.</span></span>

### <a name="business-insights-report"></a><span data-ttu-id="f9279-125">Rapporten affärs insikter</span><span class="sxs-lookup"><span data-stu-id="f9279-125">Business Insights report</span></span>

- <span data-ttu-id="f9279-126">**Kund klienter**: antal olika Azure AD-klienter med kunder som har köpt prenumerationer</span><span class="sxs-lookup"><span data-stu-id="f9279-126">**Customer tenants**: Number of distinct Azure AD tenants of customers that have purchased subscriptions</span></span>

- <span data-ttu-id="f9279-127">**Nytt (senaste 30 dagarna)**: nya kunder som köper minst en prenumeration under de senaste 30 dagarna</span><span class="sxs-lookup"><span data-stu-id="f9279-127">**New (last 30 days)**: New customers purchasing at least one subscription in last 30 days</span></span>

- <span data-ttu-id="f9279-128">**Omsättning (senaste 30 dagarna)**: kunder utan några "aktiva", "i respittiden" eller "inaktiverade" prenumerationer</span><span class="sxs-lookup"><span data-stu-id="f9279-128">**Churn (last 30 days)**: Customers without any “active", “in grace" or “disabled" subscriptions</span></span>

- <span data-ttu-id="f9279-129">**Nytt (senaste 24 timmarna)**: nya kunder som köper minst en prenumeration under de senaste 24 timmarna</span><span class="sxs-lookup"><span data-stu-id="f9279-129">**New (last 24 hours)**: New customers purchasing at least one subscription in last 24 hours</span></span>

- <span data-ttu-id="f9279-130">**Beräknad månads kostnad under de senaste 12 månaderna**: månads Visa månads trend för uppskattat belopp för förskotts betalning per månad under perioden de senaste 12 månaderna</span><span class="sxs-lookup"><span data-stu-id="f9279-130">**Estimated monthly cost over last 12 months**: Month over month trend of estimated pre-tax invoice dollar amount aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="f9279-131">**Uppskattad kostnad per produkt under de senaste 12 månaderna**: produkter som säljs sorterade efter uppskattat belopp för moms belopp som sammanställs under perioden de senaste 12 månaderna.</span><span class="sxs-lookup"><span data-stu-id="f9279-131">**Estimated cost by product over last 12 months**: Products sold sorted by estimated pre-tax invoice dollar amount aggregated over the period of last 12 months.</span></span> <span data-ttu-id="f9279-132">Den här statusen anger de främsta produkterna som visar de flesta intäkter.</span><span class="sxs-lookup"><span data-stu-id="f9279-132">This status indicates top products bringing most revenue.</span></span>

- <span data-ttu-id="f9279-133">**Kunder under de senaste 12 månaderna**: månads Visa månads trend för nya kunder och omsättnings kunder sammanlagt månads vis under perioden de senaste 12 månaderna</span><span class="sxs-lookup"><span data-stu-id="f9279-133">**Customers over last 12 months**: Month over month trend of new customers and churn customers aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="f9279-134">**Uppskattad kostnad per kund under de senaste 12 månaderna**: kunder sorteras efter uppskattat belopp för moms belopp som sammanställs under perioden de senaste 12 månaderna.</span><span class="sxs-lookup"><span data-stu-id="f9279-134">**Estimated cost by customer over last 12 months**: Customers sorted by estimated pre-tax invoice dollar amount aggregated over the period of last 12 months.</span></span> <span data-ttu-id="f9279-135">Den här statusen anger de främsta kunderna som har störst intäkt.</span><span class="sxs-lookup"><span data-stu-id="f9279-135">This status indicates top customers bringing most revenue.</span></span>

- <span data-ttu-id="f9279-136">**Kund antal per produkt**: produkter som säljs sorterade efter associerade kunder.</span><span class="sxs-lookup"><span data-stu-id="f9279-136">**Customer count by product**: Products sold sorted by associated customers.</span></span> <span data-ttu-id="f9279-137">Denna status anger de produkter som säljs till de flesta kunder.</span><span class="sxs-lookup"><span data-stu-id="f9279-137">This status indicates top products sold to most customers.</span></span>

### <a name="subscription-insights-report"></a><span data-ttu-id="f9279-138">Rapport om prenumerations Insights</span><span class="sxs-lookup"><span data-stu-id="f9279-138">Subscription Insights report</span></span>

- <span data-ttu-id="f9279-139">**Prenumerations status**:</span><span class="sxs-lookup"><span data-stu-id="f9279-139">**Subscription status**:</span></span>

- <span data-ttu-id="f9279-140">Aktiv: prenumerationer som tillhör status "aktiv" eller "i respittid"</span><span class="sxs-lookup"><span data-stu-id="f9279-140">Active: Subscriptions belonging to either “active" or “in grace" state</span></span>

  - <span data-ttu-id="f9279-141">Pausad: prenumerationer som tillhör tillståndet "inaktiverat"</span><span class="sxs-lookup"><span data-stu-id="f9279-141">Suspended: Subscriptions belonging to “disabled" state</span></span>

  - <span data-ttu-id="f9279-142">Insamlad: prenumerationer som hör till statusen företablerad eller upphört att gälla</span><span class="sxs-lookup"><span data-stu-id="f9279-142">De-provisioned: Subscriptions belonging to “de-provisioned" or “expired" status</span></span>

- <span data-ttu-id="f9279-143">**Förfallo status**:</span><span class="sxs-lookup"><span data-stu-id="f9279-143">**Expiry status**:</span></span>

  - <span data-ttu-id="f9279-144">Utgånget: prenumerationer som redan har upphört att gälla (där prenumerationens slutdatum har passerat)</span><span class="sxs-lookup"><span data-stu-id="f9279-144">Expired: Subscriptions that have already expired (where subscription end date is in past)</span></span>

  - <span data-ttu-id="f9279-145">Upphör att gälla efter 30 dagar: prenumerationer som upphör att gälla efter 30 dagar (där prenumerationens slutdatum är efter nästa 30 dagar)</span><span class="sxs-lookup"><span data-stu-id="f9279-145">Expiring after 30 days: Subscriptions that will expire after 30 days (where subscription end date is after next 30 days)</span></span>

  - <span data-ttu-id="f9279-146">Går ut om 30 dagar: prenumerationer som upphör att gälla inom de närmaste 30 dagarna (där prenumerationens slutdatum infaller mellan idag och de närmaste 30 dagarna)</span><span class="sxs-lookup"><span data-stu-id="f9279-146">Expiring in 30 days: Subscriptions that will expire within next 30 days (where subscription end date is between today and next 30 days)</span></span>

- <span data-ttu-id="f9279-147">**Totalt antal prenumerationer**: prenumerationer i "aktiv", "i respittiden" eller "inaktive rad" status</span><span class="sxs-lookup"><span data-stu-id="f9279-147">**Total subscriptions**: Subscriptions in “active," “in grace" or “disabled" status</span></span>

- <span data-ttu-id="f9279-148">**Nytt (senaste 30 dagarna)**: nya prenumerationer som har köpts av kunder under de senaste 30 dagarna</span><span class="sxs-lookup"><span data-stu-id="f9279-148">**New (last 30 days)**: New subscriptions purchased by customers within last 30 days</span></span>

- <span data-ttu-id="f9279-149">**Nytt (senaste 24 timmarna)**: nya prenumerationer som har köpts av kunder inom de senaste 24 timmarna</span><span class="sxs-lookup"><span data-stu-id="f9279-149">**New (last 24 hours)**: New subscriptions purchased by customers within last 24 hours</span></span>

- <span data-ttu-id="f9279-150">**Upphör att gälla om 30 dagar**: prenumerationer som upphör att gälla inom de närmaste 30 dagarna</span><span class="sxs-lookup"><span data-stu-id="f9279-150">**Expiring in 30 days**: Subscriptions that will expire within next 30 days</span></span>

- <span data-ttu-id="f9279-151">**Omsättning (senaste 30 dagarna)**: prenumerationer som har avbrutits eller skjutits upp (inaktiverade) inom de senaste 30 dagarna</span><span class="sxs-lookup"><span data-stu-id="f9279-151">**Churn (last 30 days)**: Subscriptions that have been de-provisioned or Suspended (disabled) within last 30 days</span></span>

- <span data-ttu-id="f9279-152">**Distribution efter prenumerations typer**:% distribution av totala prenumerationer efter licens typ och användnings beroende prenumerations typ</span><span class="sxs-lookup"><span data-stu-id="f9279-152">**Distribution by subscription types**: % distribution of total subscriptions by License based and usage-based subscription type</span></span>

- <span data-ttu-id="f9279-153">**Antal aktiva prenumerationer per produkt**: produkter som säljs sorterade efter antal aktiva prenumerationer</span><span class="sxs-lookup"><span data-stu-id="f9279-153">**Active subscription count by product**: Products sold sorted by active subscriptions count</span></span>

- <span data-ttu-id="f9279-154">**Prenumerationer under de senaste 12 månaderna**: månads Visa månads trend för nya prenumerationer och omsättnings prenumerationer sammanlagt månads vis under perioden de senaste 12 månaderna</span><span class="sxs-lookup"><span data-stu-id="f9279-154">**Subscriptions over last 12 months**: Month over month trend of new subscriptions and churn subscriptions aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="f9279-155">**Kund prenumerations information**: detaljerad vy över kunder, prenumerationer och erbjudanden</span><span class="sxs-lookup"><span data-stu-id="f9279-155">**Customer subscription details**: Detailed view of the customers, subscriptions, and offers</span></span>

### <a name="license-insights-report"></a><span data-ttu-id="f9279-156">Licens insikts rapport:</span><span class="sxs-lookup"><span data-stu-id="f9279-156">License Insights report:</span></span>

- <span data-ttu-id="f9279-157">**Totalt antal licenser**: totalt antal licenser som sammanställts i alla licensbaserade prenumerationer</span><span class="sxs-lookup"><span data-stu-id="f9279-157">**Total licenses**: Total number of licenses aggregated across all license-based subscriptions</span></span>

- <span data-ttu-id="f9279-158">**Ny (senaste 30 dagarna)**: licens tillägget inom de senaste 30 dagarna</span><span class="sxs-lookup"><span data-stu-id="f9279-158">**New (last 30 days)**: License addition within last 30 days</span></span>

- <span data-ttu-id="f9279-159">**Omsättning (senaste 30 dagarna)**: licens minskning inom de senaste 30 dagarna</span><span class="sxs-lookup"><span data-stu-id="f9279-159">**Churn (last 30 days)**: License reduction within last 30 days</span></span>

- <span data-ttu-id="f9279-160">**Nytt (senaste 24 timmarna)**: licens tillägget inom de senaste 24 timmarna</span><span class="sxs-lookup"><span data-stu-id="f9279-160">**New (last 24 hours)**: License addition within last 24 hours</span></span>

- <span data-ttu-id="f9279-161">**Licenser under de senaste 90 dagarna**: månads Visa månads trend för licens tillägg och minskning sammanlagt månads vis under perioden de senaste 90 dagarna</span><span class="sxs-lookup"><span data-stu-id="f9279-161">**Licenses over last 90 days**: Month over month trend of license additions and reductions aggregated monthly over the period of last 90 days</span></span>

- <span data-ttu-id="f9279-162">**Antal aktiva licenser per produkt**: produkter som säljs sorterade efter aktiva licens antal</span><span class="sxs-lookup"><span data-stu-id="f9279-162">**Active license count by product**: Products sold sorted by active license count</span></span>

- <span data-ttu-id="f9279-163">**Antal aktiva licenser per kund**: kunder sorterade efter aktiva licens antal</span><span class="sxs-lookup"><span data-stu-id="f9279-163">**Active license count by customer**: Customers sorted by active license count</span></span>

- <span data-ttu-id="f9279-164">**Information om kund licens händelser under de senaste 90 dagarna**: detaljerad vy över kunder, prenumerationer och prenumerations händelser, inklusive händelse datum, händelse namn, kvantitet och ändring av kvantitet.</span><span class="sxs-lookup"><span data-stu-id="f9279-164">**Customer license event details over last 90 days**: Detailed view of the customers, subscriptions, and subscription events including event date, event name, quantity, and change in quantity.</span></span>

### <a name="licenses-usage-report"></a><span data-ttu-id="f9279-165">Licens användnings rapport:</span><span class="sxs-lookup"><span data-stu-id="f9279-165">Licenses Usage report:</span></span>

- <span data-ttu-id="f9279-166">**Licenser som tilldelas av produkten**: produkter som säljs sorterade efter licens tilldelnings antal</span><span class="sxs-lookup"><span data-stu-id="f9279-166">**Licenses assigned by product**: Products sold sorted by license assignment count</span></span>

- <span data-ttu-id="f9279-167">**Licenser som används av produkten**: produkter som säljs sorterade efter licens användning</span><span class="sxs-lookup"><span data-stu-id="f9279-167">**Licenses in use by product**: Products sold sorted by license usage count</span></span>

- <span data-ttu-id="f9279-168">**Kund distribution av tilldelade licenser**:% distribution av totalt antal kunder som brutits i Bucket med 20% intervall av licens tilldelningen%</span><span class="sxs-lookup"><span data-stu-id="f9279-168">**Customer distribution of licenses assigned**: % distribution of total customers broken in buckets of 20% range by license assignment %</span></span>

- <span data-ttu-id="f9279-169">**Kund distribution av licenser som används**:% distribution av totalt antal kunder som är brutna i Bucket med 20% intervall med licens användning%</span><span class="sxs-lookup"><span data-stu-id="f9279-169">**Customer distribution of licenses in use**: % distribution of total customers broken in buckets of 20% range by license usage %</span></span>

- <span data-ttu-id="f9279-170">**Licenser tilldelade av kunden**: detaljerad vy över licenser som har sålts och licenser tilldelade av kunder och produkter</span><span class="sxs-lookup"><span data-stu-id="f9279-170">**Licenses assigned by customer**: Detailed view of licenses sold and licenses assigned by customers and products</span></span>

- <span data-ttu-id="f9279-171">**Licenser som används av kunden**: detaljerad vy över licenser som har sålts och licenser som används av kunder och produkter</span><span class="sxs-lookup"><span data-stu-id="f9279-171">**Licenses in use by customer**: Detailed view of licenses sold and licenses in use by customers and products</span></span>

### <a name="azure-insights-report"></a><span data-ttu-id="f9279-172">Azure Insights-rapport:</span><span class="sxs-lookup"><span data-stu-id="f9279-172">Azure Insights report:</span></span>

- <span data-ttu-id="f9279-173">**Användnings kunder under de senaste 12 månaderna**: månads Visa månads trend för nya användnings kunder och omsättnings bara användnings kunder sammanställda månads vis under perioden de senaste 12 månaderna</span><span class="sxs-lookup"><span data-stu-id="f9279-173">**Usage-based customers over last 12 months**: Month over month trend of new usage-based customers and churned usage-based customers aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="f9279-174">**Användnings prenumerationer under de senaste 12 månaderna**: månads Visa månads trend för nya användnings prenumerationer och indelade användnings prenumerationer sammanställda månads vis under perioden de senaste 12 månaderna</span><span class="sxs-lookup"><span data-stu-id="f9279-174">**Usage-based subscriptions over last 12 months**: Month over month trend of new usage-based subscriptions and churned usage-based subscriptions aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="f9279-175">**Uppskattad kostnad för användning av kunden under de senaste 60 dagarna**: användnings kunder sorteras efter uppskattat belopp belopp för förskotts betalning som sammanställs under perioden senaste 60 dagar.</span><span class="sxs-lookup"><span data-stu-id="f9279-175">**Estimated cost of usage by customer over last 60 days**: Usage-based customers sorted by estimated pre-tax invoice dollar amount aggregated over the period of last 60 days.</span></span> <span data-ttu-id="f9279-176">Denna status anger de mest använda användnings kunderna som tar de flesta intäkter</span><span class="sxs-lookup"><span data-stu-id="f9279-176">This status indicates top usage-based customers bringing most revenue</span></span>

- <span data-ttu-id="f9279-177">**Uppskattad kostnad för användning per kategori över de senaste 60 dagarna**: mätar kategorier med användnings prenumerationer sorterade efter uppskattat belopp för förskotts betalning som sammanställs under perioden senaste 60 dagar.</span><span class="sxs-lookup"><span data-stu-id="f9279-177">**Estimated cost of usage by category over last 60 days**: Meter categories of usage-based subscriptions sorted by estimated pre-tax invoice dollar amount aggregated over the period of last 60 days.</span></span>

- <span data-ttu-id="f9279-178">**Uppskattad kostnad för användning av prenumeration under de senaste 60 dagarna**: användnings prenumerationer efter uppskattat belopp belopp för förskotts betalning som sammanställts under perioden senaste 60 dagar.</span><span class="sxs-lookup"><span data-stu-id="f9279-178">**Estimated cost of usage by subscription over last 60 days**: Usage-based subscriptions by estimated pre-tax invoice dollar amount aggregated over the period of last 60 days.</span></span>

- <span data-ttu-id="f9279-179">**Kund Beräknad användnings kostnad per utgifts budget**: kunderna sorteras efter procent andel av den aktuella förbruknings utgifts budgeten som överskrider tröskelvärdet (100%).</span><span class="sxs-lookup"><span data-stu-id="f9279-179">**Customer estimated usage cost by spending budget**: Customers sorted by percentage of their current usage spending budget exceeding threshold (100%).</span></span>

### <a name="azure-resource-usage-report"></a><span data-ttu-id="f9279-180">Azure-resurs användnings rapport:</span><span class="sxs-lookup"><span data-stu-id="f9279-180">Azure Resource Usage report:</span></span>

- <span data-ttu-id="f9279-181">**Användning av Azure-resurser per dag för vald period**: dagliga förbruknings enheter för varje mätnings resurs i varje Använd prenumeration för vald period under de senaste 60 dagarna.</span><span class="sxs-lookup"><span data-stu-id="f9279-181">**Usage of Azure resources by day for selected period**: Daily consumption units for each metered resource in each usage-based subscription for selected period within the last 60 days.</span></span>

- <span data-ttu-id="f9279-182">**Uppskattad användnings kostnad för Azure-resurser för vald period**: uppskattad kostnad baserat på det senaste kortet för varje mätnings resurs i varje Använd prenumeration för den valda perioden under de senaste 60 dagarna.</span><span class="sxs-lookup"><span data-stu-id="f9279-182">**Estimated usage cost of Azure resources for selected period**: Estimated cost based on latest rate card for each metered resource in each usage-based subscription for selected period within the last 60 days.</span></span> 

## <a name="next-steps"></a><span data-ttu-id="f9279-183">Nästa steg</span><span class="sxs-lookup"><span data-stu-id="f9279-183">Next steps</span></span>

- [<span data-ttu-id="f9279-184">Översikt över partner Center-analys för Power BI app</span><span class="sxs-lookup"><span data-stu-id="f9279-184">Partner Center Analytics for Power BI app overview</span></span>](power-bi-app-for-direct-partners.md)

- [<span data-ttu-id="f9279-185">Installera och förhandsgranska partnercenteranalysappen för Microsoft Power BI</span><span class="sxs-lookup"><span data-stu-id="f9279-185">Install and preview the Partner Center Analytics app for Microsoft Power BI</span></span>](power-bi-app-for-direct-partners-install.md)
