---
title: Använda Partner Center Analytics för Power BI
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Lär dig hur du visar dina affärsdata med hjälp av appen Partnercenteranalys för Power BI (för direkta partner i programmet Molnlösningsleverantör (CSP).
fwlink: https://go.microsoft.com/fwlink/?linkid=852581
author: v-sumukh
ms.author: v-sumukh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 95eb018a3284d2de98c0ce6a9cd0ce6299d5571a
ms.sourcegitcommit: 4118de5cf55d1bd618ecca13c1b2ec59d80f43db
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/24/2021
ms.locfileid: "112564989"
---
# <a name="view-your-business-data-with-the-partner-center-analytics-app-for-microsoft-power-bi"></a><span data-ttu-id="d489f-103">Visa dina affärsdata med PartnerCenter Analytics-appen för Microsoft Power BI</span><span class="sxs-lookup"><span data-stu-id="d489f-103">View your business data with the Partner Center Analytics app for Microsoft Power BI</span></span>



<span data-ttu-id="d489f-104">**Lämpliga roller:** Global | Administratörsbehörighet för användarhantering | Försäljningsagentens | Administratörsagent</span><span class="sxs-lookup"><span data-stu-id="d489f-104">**Appropriate roles**: Global admin | User management admin | Sales agent | Admin agent</span></span>

## <a name="view-your-business-data"></a><span data-ttu-id="d489f-105">Visa dina affärsdata</span><span class="sxs-lookup"><span data-stu-id="d489f-105">View your business data</span></span>

<span data-ttu-id="d489f-106">Hämta en visuell representation av dina affärsdata med Partner Center Analytics-appen för Microsoft Power BI, inklusive:</span><span class="sxs-lookup"><span data-stu-id="d489f-106">Get a visual representation of your business data with the Partner Center Analytics app for Microsoft Power BI, including:</span></span>

- <span data-ttu-id="d489f-107">Tillväxt av kundbasen, prenumerationer och licenser</span><span class="sxs-lookup"><span data-stu-id="d489f-107">Growth of your customer base, subscriptions, and licenses</span></span>

- <span data-ttu-id="d489f-108">Användning av Office 365, Microsoft Dynamics och Microsoft Azure produkter</span><span class="sxs-lookup"><span data-stu-id="d489f-108">Usage of Office 365, Microsoft Dynamics, and Microsoft Azure products</span></span>

- <span data-ttu-id="d489f-109">Dagliga förbrukningsenheter för varje förbrukningsresurs i varje Azure-prenumeration under de senaste 60 dagarna</span><span class="sxs-lookup"><span data-stu-id="d489f-109">Daily consumption units for each metered resource in each Azure subscription for the last 60 days</span></span>

- <span data-ttu-id="d489f-110">Uppskattad kostnad (baserat på det senaste priskortet)</span><span class="sxs-lookup"><span data-stu-id="d489f-110">Estimated cost (based on latest rate card)</span></span>

- <span data-ttu-id="d489f-111">Möjlighet att exportera datauppsättningar och skapa anpassade rapporter, inklusive per kund.</span><span class="sxs-lookup"><span data-stu-id="d489f-111">Ability to export datasets and create custom reports, including per customer.</span></span>

### <a name="about-the-partner-center-analytics-app-preview-release"></a><span data-ttu-id="d489f-112">Om förhandsversionen av Partner Center Analytics-appen</span><span class="sxs-lookup"><span data-stu-id="d489f-112">About the Partner Center Analytics app preview release</span></span>

- <span data-ttu-id="d489f-113">Den här appen är endast för direkta partner i Molnlösningsleverantör-programmet (CSP).</span><span class="sxs-lookup"><span data-stu-id="d489f-113">This app is for direct partners in the Cloud Solution Provider (CSP) program only.</span></span> <span data-ttu-id="d489f-114">Andra partner i CSP (indirekta återförsäljare till exempel) kommer inte att kunna logga in.</span><span class="sxs-lookup"><span data-stu-id="d489f-114">Other partners in CSP (indirect resellers, for example) will not be able to sign in.</span></span>

- <span data-ttu-id="d489f-115">Uppskattade kostnader är fakturerings-/fakturadata före skatt och är inte juridiskt bindningsbaserade.</span><span class="sxs-lookup"><span data-stu-id="d489f-115">Any estimated costs are pre-tax billing / invoice data, and are not legally binding.</span></span> <span data-ttu-id="d489f-116">Uppskattade kostnader är endast avsedda att användas för datainsikter.</span><span class="sxs-lookup"><span data-stu-id="d489f-116">Estimated costs are meant to be used for data insights only.</span></span>

- <span data-ttu-id="d489f-117">Kundinformation baseras på prenumerationer.</span><span class="sxs-lookup"><span data-stu-id="d489f-117">Customer information is based on subscriptions.</span></span> <span data-ttu-id="d489f-118">Alla kunder som du nyligen har skapat konton för, men som ännu inte har prenumerationer, ingår inte i antalet.</span><span class="sxs-lookup"><span data-stu-id="d489f-118">Any customers that you've recently created accounts for, but who don't yet have subscriptions, aren't included in counts.</span></span>

- <span data-ttu-id="d489f-119">Den uppskattade kostnaden baseras på det senaste priskortet, som baseras på CSP-priser.</span><span class="sxs-lookup"><span data-stu-id="d489f-119">Estimated cost is based on latest rate card, which is based on CSP pricing.</span></span>

- <span data-ttu-id="d489f-120">Dagar är kalenderdagar.</span><span class="sxs-lookup"><span data-stu-id="d489f-120">Days are calendar days.</span></span>

### <a name="business-insights-report"></a><span data-ttu-id="d489f-121">Business Insights-rapport</span><span class="sxs-lookup"><span data-stu-id="d489f-121">Business Insights report</span></span>

- <span data-ttu-id="d489f-122">**Kundklienter:** Antal distinkta Azure Active Directory (Azure AD) för kunder som har köpt prenumerationer</span><span class="sxs-lookup"><span data-stu-id="d489f-122">**Customer tenants**: Number of distinct Azure Active Directory (Azure AD) tenants of customers that have purchased subscriptions</span></span>

- <span data-ttu-id="d489f-123">**Ny (senaste 30 dagarna):** Nya kunder har köpt minst en prenumeration under de senaste 30 dagarna</span><span class="sxs-lookup"><span data-stu-id="d489f-123">**New (last 30 days)**: New customers purchasing at least one subscription in last 30 days</span></span>

- <span data-ttu-id="d489f-124">**Omsättning (senaste 30 dagarna):** Kunder utan prenumerationer som är "aktiva", "i respit" eller "inaktiverade"</span><span class="sxs-lookup"><span data-stu-id="d489f-124">**Churn (last 30 days)**: Customers without any “active", “in grace" or “disabled" subscriptions</span></span>

- <span data-ttu-id="d489f-125">**Ny (senaste 24 timmarna)**: Nya kunder har köpt minst en prenumeration under de senaste 24 timmarna</span><span class="sxs-lookup"><span data-stu-id="d489f-125">**New (last 24 hours)**: New customers purchasing at least one subscription in last 24 hours</span></span>

- <span data-ttu-id="d489f-126">**Uppskattad månadskostnad under de senaste 12** månaderna: Månad över månad-trend för beräknat belopp före skatt i dollar aggregerat månadsvis under de senaste 12 månaderna</span><span class="sxs-lookup"><span data-stu-id="d489f-126">**Estimated monthly cost over last 12 months**: Month over month trend of estimated pre-tax invoice dollar amount aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="d489f-127">**Uppskattad kostnad per produkt under de senaste 12** månaderna: Produkter som sålts sorterade efter beräknat belopp före skatt som aggregerats under de senaste 12 månaderna.</span><span class="sxs-lookup"><span data-stu-id="d489f-127">**Estimated cost by product over last 12 months**: Products sold sorted by estimated pre-tax invoice dollar amount aggregated over the period of last 12 months.</span></span> <span data-ttu-id="d489f-128">Den här statusen anger de främsta produkterna som ger mest intäkter.</span><span class="sxs-lookup"><span data-stu-id="d489f-128">This status indicates top products bringing most revenue.</span></span>

- <span data-ttu-id="d489f-129">**Kunder under de senaste 12** månaderna: Trenden månad för månad för nya kunder och omsättningskunder aggregerats månadsvis under de senaste 12 månaderna</span><span class="sxs-lookup"><span data-stu-id="d489f-129">**Customers over last 12 months**: Month over month trend of new customers and churn customers aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="d489f-130">**Uppskattad kostnad per kund under de senaste 12** månaderna: Kunder sorterade efter beräknat belopp före skatt som aggregerats under de senaste 12 månaderna.</span><span class="sxs-lookup"><span data-stu-id="d489f-130">**Estimated cost by customer over last 12 months**: Customers sorted by estimated pre-tax invoice dollar amount aggregated over the period of last 12 months.</span></span> <span data-ttu-id="d489f-131">Den här statusen anger att de främsta kunderna har störst intäkter.</span><span class="sxs-lookup"><span data-stu-id="d489f-131">This status indicates top customers bringing most revenue.</span></span>

- <span data-ttu-id="d489f-132">**Antal kunder efter produkt:** Sålda produkter sorterade efter associerade kunder.</span><span class="sxs-lookup"><span data-stu-id="d489f-132">**Customer count by product**: Products sold sorted by associated customers.</span></span> <span data-ttu-id="d489f-133">Den här statusen anger de främsta produkter som sålts till de flesta kunder.</span><span class="sxs-lookup"><span data-stu-id="d489f-133">This status indicates top products sold to most customers.</span></span>

### <a name="subscription-insights-report"></a><span data-ttu-id="d489f-134">Prenumerationsinformationsrapport</span><span class="sxs-lookup"><span data-stu-id="d489f-134">Subscription Insights report</span></span>

- <span data-ttu-id="d489f-135">**Prenumerationsstatus:**</span><span class="sxs-lookup"><span data-stu-id="d489f-135">**Subscription status**:</span></span>

- <span data-ttu-id="d489f-136">Aktiv: Prenumerationer som hör till antingen "aktiv" eller "i respittillstånd"</span><span class="sxs-lookup"><span data-stu-id="d489f-136">Active: Subscriptions belonging to either “active" or “in grace" state</span></span>

  - <span data-ttu-id="d489f-137">Inaktiverad: Prenumerationer som hör till tillståndet "inaktiverad"</span><span class="sxs-lookup"><span data-stu-id="d489f-137">Suspended: Subscriptions belonging to “disabled" state</span></span>

  - <span data-ttu-id="d489f-138">Avetablerat: Prenumerationer som tillhör statusen "avetablerat" eller "upphört att gälla"</span><span class="sxs-lookup"><span data-stu-id="d489f-138">De-provisioned: Subscriptions belonging to “de-provisioned" or “expired" status</span></span>

- <span data-ttu-id="d489f-139">**Förfallostatus:**</span><span class="sxs-lookup"><span data-stu-id="d489f-139">**Expiry status**:</span></span>

  - <span data-ttu-id="d489f-140">Har upphört att gälla: Prenumerationer som redan har upphört att gälla (där prenumerationens slutdatum har passerat)</span><span class="sxs-lookup"><span data-stu-id="d489f-140">Expired: Subscriptions that have already expired (where subscription end date is in past)</span></span>

  - <span data-ttu-id="d489f-141">Upphör att gälla efter 30 dagar: Prenumerationer som upphör att gälla efter 30 dagar (där prenumerationens slutdatum infaller efter de kommande 30 dagarna)</span><span class="sxs-lookup"><span data-stu-id="d489f-141">Expiring after 30 days: Subscriptions that will expire after 30 days (where subscription end date is after next 30 days)</span></span>

  - <span data-ttu-id="d489f-142">Upphör att gälla om 30 dagar: Prenumerationer som upphör att gälla inom de närmaste 30 dagarna (där slutdatumet för prenumerationen är mellan i dag och nästa 30 dagar)</span><span class="sxs-lookup"><span data-stu-id="d489f-142">Expiring in 30 days: Subscriptions that will expire within next 30 days (where subscription end date is between today and next 30 days)</span></span>

- <span data-ttu-id="d489f-143">**Totalt antal** prenumerationer: Prenumerationer i statusen "aktiv", "i respit" eller "inaktiverad"</span><span class="sxs-lookup"><span data-stu-id="d489f-143">**Total subscriptions**: Subscriptions in “active," “in grace" or “disabled" status</span></span>

- <span data-ttu-id="d489f-144">**Nytt (senaste 30 dagarna): Nya** prenumerationer som köpts av kunder under de senaste 30 dagarna</span><span class="sxs-lookup"><span data-stu-id="d489f-144">**New (last 30 days)**: New subscriptions purchased by customers within last 30 days</span></span>

- <span data-ttu-id="d489f-145">**Nytt (senaste 24 timmarna)**: Nya prenumerationer som köpts av kunder under de senaste 24 timmarna</span><span class="sxs-lookup"><span data-stu-id="d489f-145">**New (last 24 hours)**: New subscriptions purchased by customers within last 24 hours</span></span>

- <span data-ttu-id="d489f-146">**Går ut om 30 dagar:** Prenumerationer som upphör att gälla inom 30 dagar</span><span class="sxs-lookup"><span data-stu-id="d489f-146">**Expiring in 30 days**: Subscriptions that will expire within next 30 days</span></span>

- <span data-ttu-id="d489f-147">**Omsättning (senaste 30 dagarna):** Prenumerationer som har avetablerades eller inaktiverats (inaktiverats) under de senaste 30 dagarna</span><span class="sxs-lookup"><span data-stu-id="d489f-147">**Churn (last 30 days)**: Subscriptions that have been de-provisioned or suspended (disabled) within last 30 days</span></span>

- <span data-ttu-id="d489f-148">**Fördelning efter prenumerationstyper:**% fördelning av totalt antal prenumerationer efter licensbaserad och användningsbaserad prenumerationstyp</span><span class="sxs-lookup"><span data-stu-id="d489f-148">**Distribution by subscription types**: % distribution of total subscriptions by License based and usage-based subscription type</span></span>

- <span data-ttu-id="d489f-149">**Antal aktiva prenumerationer efter produkt:** Sålda produkter sorterade efter antal aktiva prenumerationer</span><span class="sxs-lookup"><span data-stu-id="d489f-149">**Active subscription count by product**: Products sold sorted by active subscriptions count</span></span>

- <span data-ttu-id="d489f-150">**Prenumerationer under de senaste 12 månaderna:** Månad över månad-trenden för nya prenumerationer och omsättningsprenumerationer aggregerade månadsvis under de senaste 12 månaderna</span><span class="sxs-lookup"><span data-stu-id="d489f-150">**Subscriptions over last 12 months**: Month over month trend of new subscriptions and churn subscriptions aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="d489f-151">**Information om** kundprenumeration: Detaljerad vy över kunder, prenumerationer och erbjudanden</span><span class="sxs-lookup"><span data-stu-id="d489f-151">**Customer subscription details**: Detailed view of the customers, subscriptions, and offers</span></span>

### <a name="license-insights-report"></a><span data-ttu-id="d489f-152">License Insights-rapport:</span><span class="sxs-lookup"><span data-stu-id="d489f-152">License Insights report:</span></span>

- <span data-ttu-id="d489f-153">**Totalt antal** licenser: Totalt antal licenser aggregerade för alla licensbaserade prenumerationer</span><span class="sxs-lookup"><span data-stu-id="d489f-153">**Total licenses**: Total number of licenses aggregated across all license-based subscriptions</span></span>

- <span data-ttu-id="d489f-154">**Nytt (senaste 30 dagarna):** Licens utöver de senaste 30 dagarna</span><span class="sxs-lookup"><span data-stu-id="d489f-154">**New (last 30 days)**: License addition within last 30 days</span></span>

- <span data-ttu-id="d489f-155">**Omsättning (senaste 30 dagarna): Licensminskning** under de senaste 30 dagarna</span><span class="sxs-lookup"><span data-stu-id="d489f-155">**Churn (last 30 days)**: License reduction within last 30 days</span></span>

- <span data-ttu-id="d489f-156">**Nytt (senaste 24 timmarna)**: Licens utöver de senaste 24 timmarna</span><span class="sxs-lookup"><span data-stu-id="d489f-156">**New (last 24 hours)**: License addition within last 24 hours</span></span>

- <span data-ttu-id="d489f-157">**Licenser under de senaste 90 dagarna:** Trenden månad för månad för licens tillägg och minskningar aggregeras månadsvis under de senaste 90 dagarna</span><span class="sxs-lookup"><span data-stu-id="d489f-157">**Licenses over last 90 days**: Month over month trend of license additions and reductions aggregated monthly over the period of last 90 days</span></span>

- <span data-ttu-id="d489f-158">**Antal aktiva licenser efter produkt:** Sålda produkter sorterade efter antal aktiva licenser</span><span class="sxs-lookup"><span data-stu-id="d489f-158">**Active license count by product**: Products sold sorted by active license count</span></span>

- <span data-ttu-id="d489f-159">**Antal aktiva licenser per kund:** Kunder sorterade efter antal aktiva licenser</span><span class="sxs-lookup"><span data-stu-id="d489f-159">**Active license count by customer**: Customers sorted by active license count</span></span>

- <span data-ttu-id="d489f-160">**Information om kundlicenshändelser under de senaste 90** dagarna: Detaljerad vy över kunder, prenumerationer och prenumerationshändelser, inklusive händelsedatum, händelsenamn, kvantitet och ändring i kvantitet.</span><span class="sxs-lookup"><span data-stu-id="d489f-160">**Customer license event details over last 90 days**: Detailed view of the customers, subscriptions, and subscription events including event date, event name, quantity, and change in quantity.</span></span>

### <a name="licenses-usage-report"></a><span data-ttu-id="d489f-161">Användningsrapport för licenser:</span><span class="sxs-lookup"><span data-stu-id="d489f-161">Licenses Usage report:</span></span>

- <span data-ttu-id="d489f-162">**Licenser tilldelade efter produkt:** Sålda produkter sorterade efter antal licenstilldelningar</span><span class="sxs-lookup"><span data-stu-id="d489f-162">**Licenses assigned by product**: Products sold sorted by license assignment count</span></span>

- <span data-ttu-id="d489f-163">**Licenser som används efter produkt:** Sålda produkter sorterade efter licensanvändningsantal</span><span class="sxs-lookup"><span data-stu-id="d489f-163">**Licenses in use by product**: Products sold sorted by license usage count</span></span>

- <span data-ttu-id="d489f-164">**Kunddistribution av tilldelade licenser:**% fördelning av totalt antal kunder uppdelade i bucketar med 20 % intervall efter licenstilldelning %</span><span class="sxs-lookup"><span data-stu-id="d489f-164">**Customer distribution of licenses assigned**: % distribution of total customers broken in buckets of 20% range by license assignment %</span></span>

- <span data-ttu-id="d489f-165">**Kunddistribution av licenser som används:**% fördelning av totalt antal kunder uppdelade i bucketar på 20 % intervall efter licensanvändning %</span><span class="sxs-lookup"><span data-stu-id="d489f-165">**Customer distribution of licenses in use**: % distribution of total customers broken in buckets of 20% range by license usage %</span></span>

- <span data-ttu-id="d489f-166">**Licenser som tilldelats av kunden:** Detaljerad vy över sålda licenser och licenser som tilldelats av kunder och produkter</span><span class="sxs-lookup"><span data-stu-id="d489f-166">**Licenses assigned by customer**: Detailed view of licenses sold and licenses assigned by customers and products</span></span>

- <span data-ttu-id="d489f-167">**Licenser som används av kunden:** Detaljerad vy över sålda licenser och licenser som används av kunder och produkter</span><span class="sxs-lookup"><span data-stu-id="d489f-167">**Licenses in use by customer**: Detailed view of licenses sold and licenses in use by customers and products</span></span>

### <a name="azure-insights-report"></a><span data-ttu-id="d489f-168">Azure Insights-rapport:</span><span class="sxs-lookup"><span data-stu-id="d489f-168">Azure Insights report:</span></span>

- <span data-ttu-id="d489f-169">**Användningsbaserade kunder under** de senaste 12 månaderna: Trenden månad för månad för nya användningsbaserade kunder och omsättningsbaserade kunder aggregerade månadsvis under de senaste 12 månaderna</span><span class="sxs-lookup"><span data-stu-id="d489f-169">**Usage-based customers over last 12 months**: Month over month trend of new usage-based customers and churned usage-based customers aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="d489f-170">**Användningsbaserade prenumerationer under de senaste 12** månaderna: Trenden månad för månad för nya användningsbaserade prenumerationer och omsade användningsbaserade prenumerationer aggregerade månadsvis under de senaste 12 månaderna</span><span class="sxs-lookup"><span data-stu-id="d489f-170">**Usage-based subscriptions over last 12 months**: Month over month trend of new usage-based subscriptions and churned usage-based subscriptions aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="d489f-171">Uppskattad kostnad för användning per kund under de **senaste 60** dagarna: Användningsbaserade kunder sorterade efter beräknat belopp före skatt i dollar aggregerat under de senaste 60 dagarna.</span><span class="sxs-lookup"><span data-stu-id="d489f-171">**Estimated cost of usage by customer over last 60 days**: Usage-based customers sorted by estimated pre-tax invoice dollar amount aggregated over the period of last 60 days.</span></span> <span data-ttu-id="d489f-172">Den här statusen anger de främsta användningsbaserade kunderna som har störst intäkter</span><span class="sxs-lookup"><span data-stu-id="d489f-172">This status indicates top usage-based customers bringing most revenue</span></span>

- <span data-ttu-id="d489f-173">Uppskattad kostnad för användning efter kategori under de **senaste 60** dagarna: Mätarkategorier för användningsbaserade prenumerationer sorterade efter beräknat belopp före skatt som aggregerats under de senaste 60 dagarna.</span><span class="sxs-lookup"><span data-stu-id="d489f-173">**Estimated cost of usage by category over last 60 days**: Meter categories of usage-based subscriptions sorted by estimated pre-tax invoice dollar amount aggregated over the period of last 60 days.</span></span>

- <span data-ttu-id="d489f-174">Uppskattad kostnad för användning per prenumeration under de **senaste 60** dagarna: Användningsbaserade prenumerationer efter beräknat belopp före skatt som aggregerats under de senaste 60 dagarna.</span><span class="sxs-lookup"><span data-stu-id="d489f-174">**Estimated cost of usage by subscription over last 60 days**: Usage-based subscriptions by estimated pre-tax invoice dollar amount aggregated over the period of last 60 days.</span></span>

- <span data-ttu-id="d489f-175">**Kundens uppskattade användningskostnad efter utgiftsbudget:** Kunder sorterade efter procentandel av den aktuella användningsbudgeten överskrider tröskelvärdet (100 %).</span><span class="sxs-lookup"><span data-stu-id="d489f-175">**Customer estimated usage cost by spending budget**: Customers sorted by percentage of their current usage spending budget exceeding threshold (100%).</span></span>

### <a name="azure-resource-usage-report"></a><span data-ttu-id="d489f-176">Rapport om Azure-resursanvändning:</span><span class="sxs-lookup"><span data-stu-id="d489f-176">Azure Resource Usage report:</span></span>

- <span data-ttu-id="d489f-177">**Användning av Azure-resurser per dag** för den valda perioden: Dagliga förbrukningsenheter för varje förbrukningsresurs i varje användningsbaserad prenumeration under den valda perioden under de senaste 60 dagarna.</span><span class="sxs-lookup"><span data-stu-id="d489f-177">**Usage of Azure resources by day for selected period**: Daily consumption units for each metered resource in each usage-based subscription for selected period within the last 60 days.</span></span>

- <span data-ttu-id="d489f-178">**Uppskattad användningskostnad för Azure-resurser** för den valda perioden: Uppskattad kostnad baserat på det senaste priskortet för varje avgiftsbaserad resurs i varje användningsbaserad prenumeration för den valda perioden under de senaste 60 dagarna.</span><span class="sxs-lookup"><span data-stu-id="d489f-178">**Estimated usage cost of Azure resources for selected period**: Estimated cost based on latest rate card for each metered resource in each usage-based subscription for selected period within the last 60 days.</span></span> 

## <a name="next-steps"></a><span data-ttu-id="d489f-179">Nästa steg</span><span class="sxs-lookup"><span data-stu-id="d489f-179">Next steps</span></span>

- [<span data-ttu-id="d489f-180">Översikt över partnercenteranalys Power BI app</span><span class="sxs-lookup"><span data-stu-id="d489f-180">Partner Center Analytics for Power BI app overview</span></span>](power-bi-app-for-direct-partners.md)

- [<span data-ttu-id="d489f-181">Installera och förhandsgranska partnercenteranalysappen för Microsoft Power BI</span><span class="sxs-lookup"><span data-stu-id="d489f-181">Install and preview the Partner Center Analytics app for Microsoft Power BI</span></span>](power-bi-app-for-direct-partners-install.md)
