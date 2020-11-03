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
ms.openlocfilehash: 248527fdbc536c552f7b2d00f208838b4ef19085
ms.sourcegitcommit: 0a6b1e6d845391539f54213efff00af4d23f028c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 07/14/2020
ms.locfileid: "92529209"
---
# <a name="view-your-business-data-with-the-partner-center-analytics-app-for-microsoft-power-bi"></a><span data-ttu-id="2f5f4-103">Visa dina affärs data med partner Center Analytics-appen för Microsoft Power BI</span><span class="sxs-lookup"><span data-stu-id="2f5f4-103">View your business data with the Partner Center Analytics app for Microsoft Power BI</span></span>

<span data-ttu-id="2f5f4-104">**Gäller för**</span><span class="sxs-lookup"><span data-stu-id="2f5f4-104">**Applies to**</span></span>

- <span data-ttu-id="2f5f4-105">Partnercenter</span><span class="sxs-lookup"><span data-stu-id="2f5f4-105">Partner Center</span></span>

<span data-ttu-id="2f5f4-106">**Lämpliga roller**</span><span class="sxs-lookup"><span data-stu-id="2f5f4-106">**Appropriate roles**</span></span>

- <span data-ttu-id="2f5f4-107">Global administratör</span><span class="sxs-lookup"><span data-stu-id="2f5f4-107">Global admin</span></span>
- <span data-ttu-id="2f5f4-108">Användaradministratör</span><span class="sxs-lookup"><span data-stu-id="2f5f4-108">User admin</span></span>
- <span data-ttu-id="2f5f4-109">Försäljnings agent</span><span class="sxs-lookup"><span data-stu-id="2f5f4-109">Sales agent</span></span>
- <span data-ttu-id="2f5f4-110">Administratörs agent</span><span class="sxs-lookup"><span data-stu-id="2f5f4-110">Admin agent</span></span>

## <a name="view-your-business-data"></a><span data-ttu-id="2f5f4-111">Visa dina affärs data</span><span class="sxs-lookup"><span data-stu-id="2f5f4-111">View your business data</span></span>

<span data-ttu-id="2f5f4-112">Få en visuell representation av dina affärs data med partner Center Analytics-appen för Power BI, inklusive:</span><span class="sxs-lookup"><span data-stu-id="2f5f4-112">Get a visual representation of your business data with the Partner Center Analytics app for Power BI, including:</span></span>

- <span data-ttu-id="2f5f4-113">Tillväxt av kund basen, prenumerationer och licenser</span><span class="sxs-lookup"><span data-stu-id="2f5f4-113">Growth of your customer base, subscriptions, and licenses</span></span>

- <span data-ttu-id="2f5f4-114">Användning av Office 365, Microsoft Dynamics och Microsoft Azure produkter</span><span class="sxs-lookup"><span data-stu-id="2f5f4-114">Usage of Office 365, Microsoft Dynamics, and Microsoft Azure products</span></span>

- <span data-ttu-id="2f5f4-115">Dagliga förbruknings enheter för varje avgiftsbelagd resurs i varje Azure-prenumeration under de senaste 60 dagarna</span><span class="sxs-lookup"><span data-stu-id="2f5f4-115">Daily consumption units for each metered resource in each Azure subscription for the last 60 days</span></span>

- <span data-ttu-id="2f5f4-116">Beräknad kostnad (baserat på senaste pris kortet)</span><span class="sxs-lookup"><span data-stu-id="2f5f4-116">Estimated cost (based on latest rate card)</span></span>

- <span data-ttu-id="2f5f4-117">Möjlighet att exportera data uppsättningar och skapa anpassade rapporter, inklusive per kund.</span><span class="sxs-lookup"><span data-stu-id="2f5f4-117">Ability to export datasets and create custom reports, including per customer.</span></span>

### <a name="about-the-partner-center-analytics-app-preview-release"></a><span data-ttu-id="2f5f4-118">Om för hands versionen av Partner Center Analytics-appen</span><span class="sxs-lookup"><span data-stu-id="2f5f4-118">About the Partner Center Analytics app preview release</span></span>

- <span data-ttu-id="2f5f4-119">Den här appen är endast för direkta partner i Cloud Solution Provider-programmet.</span><span class="sxs-lookup"><span data-stu-id="2f5f4-119">This app is for direct partners in the Cloud Solution Provider program only.</span></span> <span data-ttu-id="2f5f4-120">Andra partner i CSP (indirekt åter försäljare, till exempel) kan inte logga in.</span><span class="sxs-lookup"><span data-stu-id="2f5f4-120">Other partners in CSP (indirect resellers, for example) will not be able to sign in.</span></span>

- <span data-ttu-id="2f5f4-121">Eventuella beräknade kostnader är fakturerings-och faktura data för moms, och är inte juridiskt bindande.</span><span class="sxs-lookup"><span data-stu-id="2f5f4-121">Any estimated costs are pre-tax billing / invoice data, and are not legally binding.</span></span> <span data-ttu-id="2f5f4-122">Uppskattade kostnader är avsedda att användas enbart för data insikter.</span><span class="sxs-lookup"><span data-stu-id="2f5f4-122">Estimated costs are meant to be used for data insights only.</span></span>

- <span data-ttu-id="2f5f4-123">Kund information baseras på prenumerationer.</span><span class="sxs-lookup"><span data-stu-id="2f5f4-123">Customer information is based on subscriptions.</span></span> <span data-ttu-id="2f5f4-124">Alla kunder som du nyligen har skapat konton för, men som ännu inte har några prenumerationer, ingår inte i antal.</span><span class="sxs-lookup"><span data-stu-id="2f5f4-124">Any customers that you've recently created accounts for, but who do not yet have subscriptions, are not included in counts.</span></span>

- <span data-ttu-id="2f5f4-125">Den uppskattade kostnaden baseras på det senaste avgifts kortet, som baseras på CSP-priset.</span><span class="sxs-lookup"><span data-stu-id="2f5f4-125">Estimated cost is based on latest rate card, which is based on CSP pricing.</span></span>

- <span data-ttu-id="2f5f4-126">Dagar är kalender dagar.</span><span class="sxs-lookup"><span data-stu-id="2f5f4-126">Days are calendar days.</span></span>

### <a name="business-insights-report"></a><span data-ttu-id="2f5f4-127">Rapporten affärs insikter</span><span class="sxs-lookup"><span data-stu-id="2f5f4-127">Business Insights report</span></span>

- <span data-ttu-id="2f5f4-128">**Kund klienter** : antal olika Azure AD-klienter med kunder som har köpt prenumerationer</span><span class="sxs-lookup"><span data-stu-id="2f5f4-128">**Customer tenants** : Number of distinct Azure AD tenants of customers that have purchased subscriptions</span></span>

- <span data-ttu-id="2f5f4-129">**Nytt (senaste 30 dagarna)** : nya kunder som köper minst en prenumeration under de senaste 30 dagarna</span><span class="sxs-lookup"><span data-stu-id="2f5f4-129">**New (last 30 days)** : New customers purchasing at least one subscription in last 30 days</span></span>

- <span data-ttu-id="2f5f4-130">**Omsättning (senaste 30 dagarna)** : kunder utan några "aktiva", "i respittiden" eller "inaktiverade" prenumerationer</span><span class="sxs-lookup"><span data-stu-id="2f5f4-130">**Churn (last 30 days)** : Customers without any “active", “in grace" or “disabled" subscriptions</span></span>

- <span data-ttu-id="2f5f4-131">**Nytt (senaste 24 timmarna)** : nya kunder som köper minst en prenumeration under de senaste 24 timmarna</span><span class="sxs-lookup"><span data-stu-id="2f5f4-131">**New (last 24 hours)** : New customers purchasing at least one subscription in last 24 hours</span></span>

- <span data-ttu-id="2f5f4-132">**Beräknad månads kostnad under de senaste 12 månaderna** : månads Visa månads trend för uppskattat belopp för förskotts betalning per månad under perioden de senaste 12 månaderna</span><span class="sxs-lookup"><span data-stu-id="2f5f4-132">**Estimated monthly cost over last 12 months** : Month over month trend of estimated pre-tax invoice dollar amount aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="2f5f4-133">**Uppskattad kostnad per produkt under de senaste 12 månaderna** : produkter som säljs sorterade efter uppskattat belopp för moms belopp som sammanställs under perioden de senaste 12 månaderna.</span><span class="sxs-lookup"><span data-stu-id="2f5f4-133">**Estimated cost by product over last 12 months** : Products sold sorted by estimated pre-tax invoice dollar amount aggregated over the period of last 12 months.</span></span> <span data-ttu-id="2f5f4-134">Den här statusen anger de främsta produkterna som visar de flesta intäkter.</span><span class="sxs-lookup"><span data-stu-id="2f5f4-134">This status indicates top products bringing most revenue.</span></span>

- <span data-ttu-id="2f5f4-135">**Kunder under de senaste 12 månaderna** : månads Visa månads trend för nya kunder och omsättnings kunder sammanlagt månads vis under perioden de senaste 12 månaderna</span><span class="sxs-lookup"><span data-stu-id="2f5f4-135">**Customers over last 12 months** : Month over month trend of new customers and churn customers aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="2f5f4-136">**Uppskattad kostnad per kund under de senaste 12 månaderna** : kunder sorteras efter uppskattat belopp för moms belopp som sammanställs under perioden de senaste 12 månaderna.</span><span class="sxs-lookup"><span data-stu-id="2f5f4-136">**Estimated cost by customer over last 12 months** : Customers sorted by estimated pre-tax invoice dollar amount aggregated over the period of last 12 months.</span></span> <span data-ttu-id="2f5f4-137">Den här statusen anger de främsta kunderna som har störst intäkt.</span><span class="sxs-lookup"><span data-stu-id="2f5f4-137">This status indicates top customers bringing most revenue.</span></span>

- <span data-ttu-id="2f5f4-138">**Kund antal per produkt** : produkter som säljs sorterade efter associerade kunder.</span><span class="sxs-lookup"><span data-stu-id="2f5f4-138">**Customer count by product** : Products sold sorted by associated customers.</span></span> <span data-ttu-id="2f5f4-139">Denna status anger de produkter som säljs till de flesta kunder.</span><span class="sxs-lookup"><span data-stu-id="2f5f4-139">This status indicates top products sold to most customers.</span></span>

### <a name="subscription-insights-report"></a><span data-ttu-id="2f5f4-140">Rapport om prenumerations Insights</span><span class="sxs-lookup"><span data-stu-id="2f5f4-140">Subscription Insights report</span></span>

- <span data-ttu-id="2f5f4-141">**Prenumerations status** :</span><span class="sxs-lookup"><span data-stu-id="2f5f4-141">**Subscription status** :</span></span>

- <span data-ttu-id="2f5f4-142">Aktiv: prenumerationer som tillhör status "aktiv" eller "i respittid"</span><span class="sxs-lookup"><span data-stu-id="2f5f4-142">Active: Subscriptions belonging to either “active" or “in grace" state</span></span>

  - <span data-ttu-id="2f5f4-143">Pausad: prenumerationer som tillhör tillståndet "inaktiverat"</span><span class="sxs-lookup"><span data-stu-id="2f5f4-143">Suspended: Subscriptions belonging to “disabled" state</span></span>

  - <span data-ttu-id="2f5f4-144">Insamlad: prenumerationer som hör till statusen företablerad eller upphört att gälla</span><span class="sxs-lookup"><span data-stu-id="2f5f4-144">De-provisioned: Subscriptions belonging to “de-provisioned" or “expired" status</span></span>

- <span data-ttu-id="2f5f4-145">**Förfallo status** :</span><span class="sxs-lookup"><span data-stu-id="2f5f4-145">**Expiry status** :</span></span>

  - <span data-ttu-id="2f5f4-146">Utgånget: prenumerationer som redan har upphört att gälla (där prenumerationens slutdatum har passerat)</span><span class="sxs-lookup"><span data-stu-id="2f5f4-146">Expired: Subscriptions that have already expired (where subscription end date is in past)</span></span>

  - <span data-ttu-id="2f5f4-147">Upphör att gälla efter 30 dagar: prenumerationer som upphör att gälla efter 30 dagar (där prenumerationens slutdatum är efter nästa 30 dagar)</span><span class="sxs-lookup"><span data-stu-id="2f5f4-147">Expiring after 30 days: Subscriptions that will expire after 30 days (where subscription end date is after next 30 days)</span></span>

  - <span data-ttu-id="2f5f4-148">Går ut om 30 dagar: prenumerationer som upphör att gälla inom de närmaste 30 dagarna (där prenumerationens slutdatum infaller mellan idag och de närmaste 30 dagarna)</span><span class="sxs-lookup"><span data-stu-id="2f5f4-148">Expiring in 30 days: Subscriptions that will expire within next 30 days (where subscription end date is between today and next 30 days)</span></span>

- <span data-ttu-id="2f5f4-149">**Totalt antal prenumerationer** : prenumerationer i "aktiv", "i respittiden" eller "inaktive rad" status</span><span class="sxs-lookup"><span data-stu-id="2f5f4-149">**Total subscriptions** : Subscriptions in “active," “in grace" or “disabled" status</span></span>

- <span data-ttu-id="2f5f4-150">**Nytt (senaste 30 dagarna)** : nya prenumerationer som har köpts av kunder under de senaste 30 dagarna</span><span class="sxs-lookup"><span data-stu-id="2f5f4-150">**New (last 30 days)** : New subscriptions purchased by customers within last 30 days</span></span>

- <span data-ttu-id="2f5f4-151">**Nytt (senaste 24 timmarna)** : nya prenumerationer som har köpts av kunder inom de senaste 24 timmarna</span><span class="sxs-lookup"><span data-stu-id="2f5f4-151">**New (last 24 hours)** : New subscriptions purchased by customers within last 24 hours</span></span>

- <span data-ttu-id="2f5f4-152">**Upphör att gälla om 30 dagar** : prenumerationer som upphör att gälla inom de närmaste 30 dagarna</span><span class="sxs-lookup"><span data-stu-id="2f5f4-152">**Expiring in 30 days** : Subscriptions that will expire within next 30 days</span></span>

- <span data-ttu-id="2f5f4-153">**Omsättning (senaste 30 dagarna)** : prenumerationer som har avbrutits eller skjutits upp (inaktiverade) inom de senaste 30 dagarna</span><span class="sxs-lookup"><span data-stu-id="2f5f4-153">**Churn (last 30 days)** : Subscriptions that have been de-provisioned or Suspended (disabled) within last 30 days</span></span>

- <span data-ttu-id="2f5f4-154">**Distribution efter prenumerations typer** :% distribution av totala prenumerationer efter licens typ och användnings beroende prenumerations typ</span><span class="sxs-lookup"><span data-stu-id="2f5f4-154">**Distribution by subscription types** : % distribution of total subscriptions by License based and usage-based subscription type</span></span>

- <span data-ttu-id="2f5f4-155">**Antal aktiva prenumerationer per produkt** : produkter som säljs sorterade efter antal aktiva prenumerationer</span><span class="sxs-lookup"><span data-stu-id="2f5f4-155">**Active subscription count by product** : Products sold sorted by active subscriptions count</span></span>

- <span data-ttu-id="2f5f4-156">**Prenumerationer under de senaste 12 månaderna** : månads Visa månads trend för nya prenumerationer och omsättnings prenumerationer sammanlagt månads vis under perioden de senaste 12 månaderna</span><span class="sxs-lookup"><span data-stu-id="2f5f4-156">**Subscriptions over last 12 months** : Month over month trend of new subscriptions and churn subscriptions aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="2f5f4-157">**Kund prenumerations information** : detaljerad vy över kunder, prenumerationer och erbjudanden</span><span class="sxs-lookup"><span data-stu-id="2f5f4-157">**Customer subscription details** : Detailed view of the customers, subscriptions, and offers</span></span>

### <a name="license-insights-report"></a><span data-ttu-id="2f5f4-158">Licens insikts rapport:</span><span class="sxs-lookup"><span data-stu-id="2f5f4-158">License Insights report:</span></span>

- <span data-ttu-id="2f5f4-159">**Totalt antal licenser** : totalt antal licenser som sammanställts i alla licensbaserade prenumerationer</span><span class="sxs-lookup"><span data-stu-id="2f5f4-159">**Total licenses** : Total number of licenses aggregated across all license-based subscriptions</span></span>

- <span data-ttu-id="2f5f4-160">**Ny (senaste 30 dagarna)** : licens tillägget inom de senaste 30 dagarna</span><span class="sxs-lookup"><span data-stu-id="2f5f4-160">**New (last 30 days)** : License addition within last 30 days</span></span>

- <span data-ttu-id="2f5f4-161">**Omsättning (senaste 30 dagarna)** : licens minskning inom de senaste 30 dagarna</span><span class="sxs-lookup"><span data-stu-id="2f5f4-161">**Churn (last 30 days)** : License reduction within last 30 days</span></span>

- <span data-ttu-id="2f5f4-162">**Nytt (senaste 24 timmarna)** : licens tillägget inom de senaste 24 timmarna</span><span class="sxs-lookup"><span data-stu-id="2f5f4-162">**New (last 24 hours)** : License addition within last 24 hours</span></span>

- <span data-ttu-id="2f5f4-163">**Licenser under de senaste 90 dagarna** : månads Visa månads trend för licens tillägg och minskning sammanlagt månads vis under perioden de senaste 90 dagarna</span><span class="sxs-lookup"><span data-stu-id="2f5f4-163">**Licenses over last 90 days** : Month over month trend of license additions and reductions aggregated monthly over the period of last 90 days</span></span>

- <span data-ttu-id="2f5f4-164">**Antal aktiva licenser per produkt** : produkter som säljs sorterade efter aktiva licens antal</span><span class="sxs-lookup"><span data-stu-id="2f5f4-164">**Active license count by product** : Products sold sorted by active license count</span></span>

- <span data-ttu-id="2f5f4-165">**Antal aktiva licenser per kund** : kunder sorterade efter aktiva licens antal</span><span class="sxs-lookup"><span data-stu-id="2f5f4-165">**Active license count by customer** : Customers sorted by active license count</span></span>

- <span data-ttu-id="2f5f4-166">**Information om kund licens händelser under de senaste 90 dagarna** : detaljerad vy över kunder, prenumerationer och prenumerations händelser, inklusive händelse datum, händelse namn, kvantitet och ändring av kvantitet.</span><span class="sxs-lookup"><span data-stu-id="2f5f4-166">**Customer license event details over last 90 days** : Detailed view of the customers, subscriptions, and subscription events including event date, event name, quantity, and change in quantity.</span></span>

### <a name="licenses-usage-report"></a><span data-ttu-id="2f5f4-167">Licens användnings rapport:</span><span class="sxs-lookup"><span data-stu-id="2f5f4-167">Licenses Usage report:</span></span>

- <span data-ttu-id="2f5f4-168">**Licenser som tilldelas av produkten** : produkter som säljs sorterade efter licens tilldelnings antal</span><span class="sxs-lookup"><span data-stu-id="2f5f4-168">**Licenses assigned by product** : Products sold sorted by license assignment count</span></span>

- <span data-ttu-id="2f5f4-169">**Licenser som används av produkten** : produkter som säljs sorterade efter licens användning</span><span class="sxs-lookup"><span data-stu-id="2f5f4-169">**Licenses in use by product** : Products sold sorted by license usage count</span></span>

- <span data-ttu-id="2f5f4-170">**Kund distribution av tilldelade licenser** :% distribution av totalt antal kunder som brutits i Bucket med 20% intervall av licens tilldelningen%</span><span class="sxs-lookup"><span data-stu-id="2f5f4-170">**Customer distribution of licenses assigned** : % distribution of total customers broken in buckets of 20% range by license assignment %</span></span>

- <span data-ttu-id="2f5f4-171">**Kund distribution av licenser som används** :% distribution av totalt antal kunder som är brutna i Bucket med 20% intervall med licens användning%</span><span class="sxs-lookup"><span data-stu-id="2f5f4-171">**Customer distribution of licenses in use** : % distribution of total customers broken in buckets of 20% range by license usage %</span></span>

- <span data-ttu-id="2f5f4-172">**Licenser tilldelade av kunden** : detaljerad vy över licenser som har sålts och licenser tilldelade av kunder och produkter</span><span class="sxs-lookup"><span data-stu-id="2f5f4-172">**Licenses assigned by customer** : Detailed view of licenses sold and licenses assigned by customers and products</span></span>

- <span data-ttu-id="2f5f4-173">**Licenser som används av kunden** : detaljerad vy över licenser som har sålts och licenser som används av kunder och produkter</span><span class="sxs-lookup"><span data-stu-id="2f5f4-173">**Licenses in use by customer** : Detailed view of licenses sold and licenses in use by customers and products</span></span>

### <a name="azure-insights-report"></a><span data-ttu-id="2f5f4-174">Azure Insights-rapport:</span><span class="sxs-lookup"><span data-stu-id="2f5f4-174">Azure Insights report:</span></span>

- <span data-ttu-id="2f5f4-175">**Användnings kunder under de senaste 12 månaderna** : månads Visa månads trend för nya användnings kunder och omsättnings bara användnings kunder sammanställda månads vis under perioden de senaste 12 månaderna</span><span class="sxs-lookup"><span data-stu-id="2f5f4-175">**Usage-based customers over last 12 months** : Month over month trend of new usage-based customers and churned usage-based customers aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="2f5f4-176">**Användnings prenumerationer under de senaste 12 månaderna** : månads Visa månads trend för nya användnings prenumerationer och indelade användnings prenumerationer sammanställda månads vis under perioden de senaste 12 månaderna</span><span class="sxs-lookup"><span data-stu-id="2f5f4-176">**Usage-based subscriptions over last 12 months** : Month over month trend of new usage-based subscriptions and churned usage-based subscriptions aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="2f5f4-177">**Uppskattad kostnad för användning av kunden under de senaste 60 dagarna** : användnings kunder sorteras efter uppskattat belopp belopp för förskotts betalning som sammanställs under perioden senaste 60 dagar.</span><span class="sxs-lookup"><span data-stu-id="2f5f4-177">**Estimated cost of usage by customer over last 60 days** : Usage-based customers sorted by estimated pre-tax invoice dollar amount aggregated over the period of last 60 days.</span></span> <span data-ttu-id="2f5f4-178">Denna status anger de mest använda användnings kunderna som tar de flesta intäkter</span><span class="sxs-lookup"><span data-stu-id="2f5f4-178">This status indicates top usage-based customers bringing most revenue</span></span>

- <span data-ttu-id="2f5f4-179">**Uppskattad kostnad för användning per kategori över de senaste 60 dagarna** : mätar kategorier med användnings prenumerationer sorterade efter uppskattat belopp för förskotts betalning som sammanställs under perioden senaste 60 dagar.</span><span class="sxs-lookup"><span data-stu-id="2f5f4-179">**Estimated cost of usage by category over last 60 days** : Meter categories of usage-based subscriptions sorted by estimated pre-tax invoice dollar amount aggregated over the period of last 60 days.</span></span>

- <span data-ttu-id="2f5f4-180">**Uppskattad kostnad för användning av prenumeration under de senaste 60 dagarna** : användnings prenumerationer efter uppskattat belopp belopp för förskotts betalning som sammanställts under perioden senaste 60 dagar.</span><span class="sxs-lookup"><span data-stu-id="2f5f4-180">**Estimated cost of usage by subscription over last 60 days** : Usage-based subscriptions by estimated pre-tax invoice dollar amount aggregated over the period of last 60 days.</span></span>

- <span data-ttu-id="2f5f4-181">**Kund Beräknad användnings kostnad per utgifts budget** : kunderna sorteras efter procent andel av den aktuella förbruknings utgifts budgeten som överskrider tröskelvärdet (100%).</span><span class="sxs-lookup"><span data-stu-id="2f5f4-181">**Customer estimated usage cost by spending budget** : Customers sorted by percentage of their current usage spending budget exceeding threshold (100%).</span></span>

### <a name="azure-resource-usage-report"></a><span data-ttu-id="2f5f4-182">Azure-resurs användnings rapport:</span><span class="sxs-lookup"><span data-stu-id="2f5f4-182">Azure Resource Usage report:</span></span>

- <span data-ttu-id="2f5f4-183">**Användning av Azure-resurser per dag för vald period** : dagliga förbruknings enheter för varje mätnings resurs i varje Använd prenumeration för vald period under de senaste 60 dagarna.</span><span class="sxs-lookup"><span data-stu-id="2f5f4-183">**Usage of Azure resources by day for selected period** : Daily consumption units for each metered resource in each usage-based subscription for selected period within the last 60 days.</span></span>

- <span data-ttu-id="2f5f4-184">**Uppskattad användnings kostnad för Azure-resurser för vald period** : uppskattad kostnad baserat på det senaste kortet för varje mätnings resurs i varje Använd prenumeration för den valda perioden under de senaste 60 dagarna.</span><span class="sxs-lookup"><span data-stu-id="2f5f4-184">**Estimated usage cost of Azure resources for selected period** : Estimated cost based on latest rate card for each metered resource in each usage-based subscription for selected period within the last 60 days.</span></span> 

## <a name="next-steps"></a><span data-ttu-id="2f5f4-185">Nästa steg</span><span class="sxs-lookup"><span data-stu-id="2f5f4-185">Next steps</span></span>

- [<span data-ttu-id="2f5f4-186">Översikt över partner Center-analys för Power BI app</span><span class="sxs-lookup"><span data-stu-id="2f5f4-186">Partner Center Analytics for Power BI app overview</span></span>](power-bi-app-for-direct-partners.md)

- [<span data-ttu-id="2f5f4-187">Installera och förhandsgranska partnercenteranalysappen för Microsoft Power BI</span><span class="sxs-lookup"><span data-stu-id="2f5f4-187">Install and preview the Partner Center Analytics app for Microsoft Power BI</span></span>](power-bi-app-for-direct-partners-install.md)
