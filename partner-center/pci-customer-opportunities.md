---
title: Partner Center Insights – CloudAscent benägenhet-rapporter
description: Lär dig mer om CloudAscent benägenhet-rapporter i Partner Center. Innehåller information om en kunds benägenhet för att köpa Microsoft-produkter.
ms.topic: conceptual
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 09/18/2020
ms.openlocfilehash: fd017884c29df3874a06e8c4213c6fe5f05a8995
ms.sourcegitcommit: 3c45a181ef86b3a4866e97fb50efeae8714ab3f7
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 10/19/2020
ms.locfileid: "92532072"
---
# <a name="cloudascent-propensity-reports-available-from-partner-center-dashboard"></a><span data-ttu-id="e07a6-104">CloudAscent benägenhet-rapporter som är tillgängliga från instrument panelen för partner Center</span><span class="sxs-lookup"><span data-stu-id="e07a6-104">CloudAscent Propensity reports available from Partner Center dashboard</span></span>

<span data-ttu-id="e07a6-105">**Lämpliga roller**</span><span class="sxs-lookup"><span data-stu-id="e07a6-105">**Appropriate roles**</span></span>
- <span data-ttu-id="e07a6-106">Rapport visnings program för chefer</span><span class="sxs-lookup"><span data-stu-id="e07a6-106">Executive report viewer</span></span>
- <span data-ttu-id="e07a6-107">Rapport visnings program</span><span class="sxs-lookup"><span data-stu-id="e07a6-107">Report viewer</span></span>

<span data-ttu-id="e07a6-108">Instrument panelen för partner Center innehåller nedladdnings bara benägenhet-data från CloudAscent-programmet.</span><span class="sxs-lookup"><span data-stu-id="e07a6-108">The Partner Center Dashboard provides downloadable propensity data from the CloudAscent Program.</span></span> <span data-ttu-id="e07a6-109">Data visar kundernas benägenhet för att köpa Microsoft-produkter.</span><span class="sxs-lookup"><span data-stu-id="e07a6-109">The data shows the customers' propensity to purchase Microsoft products.</span></span>  <span data-ttu-id="e07a6-110">I den här artikeln beskrivs nedbrytningen av dessa data, hur du använder den och vad det innebär.</span><span class="sxs-lookup"><span data-stu-id="e07a6-110">This articles describes the breakdown of this data, how to utilize the scoring, and what it means.</span></span>

## <a name="summary-definitions"></a><span data-ttu-id="e07a6-111">Sammanfattnings definitioner</span><span class="sxs-lookup"><span data-stu-id="e07a6-111">Summary definitions</span></span>

- <span data-ttu-id="e07a6-112">**SMC-kunder** – detta är det totala antalet kunder i benägenhet nedladdning.</span><span class="sxs-lookup"><span data-stu-id="e07a6-112">**SMC Customers** – This is the total number of customers in the propensity downloads.</span></span>  <span data-ttu-id="e07a6-113">Kunderna identifieras av en partner av posten.</span><span class="sxs-lookup"><span data-stu-id="e07a6-113">Customers are identified by partner of record.</span></span>
- <span data-ttu-id="e07a6-114">**Avtalet upphör** att gälla – inom innevarande räkenskapsår tillhandahåller vi antalet avtals engångs avtal.</span><span class="sxs-lookup"><span data-stu-id="e07a6-114">**Expire Agreements** – within the current fiscal year, we're providing the number of expiring agreements.</span></span>
- <span data-ttu-id="e07a6-115">**Förfallo datum för intäkter** – den intäkt som är kopplad till avtalets upphör Ande.</span><span class="sxs-lookup"><span data-stu-id="e07a6-115">**Expiring Revenue** – the revenue associated to the expiring agreements.</span></span>
- <span data-ttu-id="e07a6-116">**Öppna förfallo** datum för intäkt – intäkten som är kopplad till Open agreementd-avtal.</span><span class="sxs-lookup"><span data-stu-id="e07a6-116">**Open Expiring Revenue** – The revenue associated to the open expiring agreements.</span></span>

:::image type="content" source="images/pci/cust-oppor-1.png" alt-text="Skärm bild av instrument panelen Sammanfattning av kund möjligheter.":::

## <a name="cloudascent-smb-segmentation"></a><span data-ttu-id="e07a6-118">CloudAscent SMB-segmentering</span><span class="sxs-lookup"><span data-stu-id="e07a6-118">CloudAscent SMB segmentation</span></span>

<span data-ttu-id="e07a6-119">Det lilla till mellanliggande segmentet (SMB) är indelat i tre distinkta del segment.</span><span class="sxs-lookup"><span data-stu-id="e07a6-119">The small to medium business (SMB) segment is further divided into three distinct sub segments.</span></span>

1. <span data-ttu-id="e07a6-120">De mest **ohanterade** innehåller de största SMB-kunderna med flest möjligheter för Microsoft.</span><span class="sxs-lookup"><span data-stu-id="e07a6-120">**Top Unmanaged** includes the largest SMB customers with the most opportunity for Microsoft.</span></span> <span data-ttu-id="e07a6-121">Vanliga ohanterade kunder delar liknande egenskaper som hanterade konton, med ett stort antal anställda, stora IT-budgetar och utgifter och stora mängder potentiella intäkter för Microsoft.</span><span class="sxs-lookup"><span data-stu-id="e07a6-121">Typical Top Unmanaged customers share similar characteristics as Managed accounts, with large number of employees, large IT budgets and spend, and large amounts of potential revenue for Microsoft.</span></span>

   <span data-ttu-id="e07a6-122">Vi definierar de vanligaste ohanterade två sätten:</span><span class="sxs-lookup"><span data-stu-id="e07a6-122">We define Top Unmanaged two ways:</span></span>

   - <span data-ttu-id="e07a6-123">**Topp ohanterad användare baserad** – inkluderar konton med 300 eller fler anställda.</span><span class="sxs-lookup"><span data-stu-id="e07a6-123">**Top Unmanaged User Based** – includes accounts with 300 or more employees.</span></span> <span data-ttu-id="e07a6-124">User-Based konton är bra mål för första inköpet, eller en utbyggnad av användarbaserade prenumerations produkter som M365, D365 eller Surface.</span><span class="sxs-lookup"><span data-stu-id="e07a6-124">User-Based accounts are great targets for first-time purchase, or expansion of user-based subscription products such as M365, D365, or Surface.</span></span>
   - <span data-ttu-id="e07a6-125">**Topp ohanterad beräkning baserad** – innehåller konton med Azure-potential som är större än $10 000.</span><span class="sxs-lookup"><span data-stu-id="e07a6-125">**Top Unmanaged Compute Based** – includes accounts with Azure potential greater than $10k.</span></span> <span data-ttu-id="e07a6-126">Compute-baserade konton inkluderar befintliga Azure.</span><span class="sxs-lookup"><span data-stu-id="e07a6-126">Compute based accounts include existing Azure.</span></span> <span data-ttu-id="e07a6-127">konton med betydande framtida års potential och konton som ännu inte har köpt Azure men som har potential för Azure större än $10 000.</span><span class="sxs-lookup"><span data-stu-id="e07a6-127">accounts with significant future year potential and accounts who have yet to purchase Azure yet but have potential for Azure greater than $10k.</span></span>

2. <span data-ttu-id="e07a6-128">**Medel stora företag** inkluderar befintliga kunder och kund konton med 25 till 300 anställda.</span><span class="sxs-lookup"><span data-stu-id="e07a6-128">**Medium Business** includes existing customers and prospect accounts with 25 to 300 employees.</span></span>

3. <span data-ttu-id="e07a6-129">**Små företag** omfattar alla återstående företag med färre än 25 anställda.</span><span class="sxs-lookup"><span data-stu-id="e07a6-129">**Small Business** includes all remaining businesses with fewer than 25 employees.</span></span>

:::image type="content" source="images/pci/cust-oppor-2.png" alt-text="Kund av SMC-typ.":::

<span data-ttu-id="e07a6-131">**De främsta** del segmenten med ohanterade och **medel stora företag** representerar höga LTV-kunder (Life-Time-Time) för Microsoft och Microsoft-partner.</span><span class="sxs-lookup"><span data-stu-id="e07a6-131">**Top Unmanaged** and **Medium Business** subsegments represent high life-time value (LTV) customers for Microsoft, and Microsoft Partners.</span></span> <span data-ttu-id="e07a6-132">Därför är de de ledande områdena i fokus för att öka tillväxten i det här segmentet.</span><span class="sxs-lookup"><span data-stu-id="e07a6-132">Hence they are the lead areas of focus for driving growth in this segment.</span></span> <span data-ttu-id="e07a6-133">I de här två del segmenten är vi bättre placerade för att hämta socketen med M365, köpa ytterligare med D365/Azures branschspecifika appar och inse en hög LTV för Microsoft.</span><span class="sxs-lookup"><span data-stu-id="e07a6-133">In these two subsegments, we are better positioned to acquire the socket with M365, monetize further with D365/Azure line of business (LOB) apps, and realize a high LTV for Microsoft.</span></span>

<span data-ttu-id="e07a6-134">Idag har vi två viktiga områden i affärs möjligheten – 1.</span><span class="sxs-lookup"><span data-stu-id="e07a6-134">Today we have two key areas of opportunity – 1.</span></span> <span data-ttu-id="e07a6-135">vår kund ökar tillväxten; 11.2.</span><span class="sxs-lookup"><span data-stu-id="e07a6-135">our customer adds growth; 2.</span></span> <span data-ttu-id="e07a6-136">Vi har också bra att köpa moln platser som är ledande med M365, men vi har en stor möjlighet i D365 och Azure.</span><span class="sxs-lookup"><span data-stu-id="e07a6-136">while we do well acquiring cloud sockets leading with M365, we have a large opportunity in D365 and Azure.</span></span>

<span data-ttu-id="e07a6-137">Följande skärm bild visar de tre SMB-undersegmenten och optimerade vägar till marknaden.</span><span class="sxs-lookup"><span data-stu-id="e07a6-137">The following screenshot represents the three SMB Subsegments and optimized routes to market.</span></span> <span data-ttu-id="e07a6-138">CloudAscent prioriterar profileringen, poängsättningen och modelleringen av alla topp ohanterade och medel stora företags konton.</span><span class="sxs-lookup"><span data-stu-id="e07a6-138">CloudAscent prioritize the profiling, scoring, and modeling of all Top Unmanaged and Medium Business accounts.</span></span>

:::image type="content" source="images/pci/cust-oppor-3.png" alt-text="Skärm bild av SMB-undersegment.":::

## <a name="cloudascent-machine-learning"></a><span data-ttu-id="e07a6-140">CloudAscent Machine Learning</span><span class="sxs-lookup"><span data-stu-id="e07a6-140">CloudAscent Machine Learning</span></span>

<span data-ttu-id="e07a6-141">SMB använder maskin inlärnings teknik för att driva försäljnings-och marknadsförings kund förutsägelser inom de högsta ohanterade och medel stora affärs segmenten.</span><span class="sxs-lookup"><span data-stu-id="e07a6-141">SMB uses machine learning technology to drive sales and marketing customer predictions within the Top Unmanaged and Medium Business segments.</span></span> <span data-ttu-id="e07a6-142">Hur samlas signaler in och omvandlas till benägenhet-rekommendationer?</span><span class="sxs-lookup"><span data-stu-id="e07a6-142">How are signals collected and turned into propensity recommendations?</span></span>

- <span data-ttu-id="e07a6-143">**Data insamling** : webbcrawler genomsöker och samlar in miljarder kund signaler genom att skicka ping till företagets domäner och övervakning: blogg inlägg, pressmeddelanden, sociala data strömmar och tekniska forum.</span><span class="sxs-lookup"><span data-stu-id="e07a6-143">**Data Collection** : Web crawlers scan and collect billions of customer signals by pinging the company domains, and monitoring: blog posts, press releases, social streams, and technical forums.</span></span>  <span data-ttu-id="e07a6-144">Utöver de insamlade signalerna samlas firmographics information in från både interna och externa källor som D&B, Microsoft intern prenumeration och transaktions data.</span><span class="sxs-lookup"><span data-stu-id="e07a6-144">In addition to the collected signals, firmographics information is collected from both internal and external sources such as D&B, Microsoft Internal subscription and transactional data.</span></span>

- <span data-ttu-id="e07a6-145">**Machine Learning** : signalerna matas in i Machine Learning-modellen som ger en strukturerad data uppsättning av försäljnings-och marknadsförings förutsägelser för varje kund enligt moln produkt och-kluster.</span><span class="sxs-lookup"><span data-stu-id="e07a6-145">**Machine Learning** : The signals are fed into the machine learning model that outputs a structured data set of Sales and Marketing predictions for each customer by cloud product and cluster.</span></span>  <span data-ttu-id="e07a6-146">Varje kund betygs ätter en valfri modell till Microsofts främsta SMB som fastställer kundens anpassnings-och Machine Learning-algoritmer som integrerar kundens beteende för online-beteendet.</span><span class="sxs-lookup"><span data-stu-id="e07a6-146">Each customer is scored using a look alike model to Microsoft's top SMB that determines the customer's Fit, and machine learning algorithms that integrate the customer's online behavior define as Intent.</span></span> <span data-ttu-id="e07a6-147">Poängen slås samman i kluster som visar en kunds benägenhet att köpa Microsoft Cloud produkter.</span><span class="sxs-lookup"><span data-stu-id="e07a6-147">The scoring is merged into clusters that show a customer's propensity to purchase Microsoft Cloud Products.</span></span>

- <span data-ttu-id="e07a6-148">**Optimering** : Machine Learning systemet optimerar modellerna genom att förbruka transaktions data varje månad och prenumerations data kvartals vis.</span><span class="sxs-lookup"><span data-stu-id="e07a6-148">**Optimization** : The Machine Learning system optimizes the models by consuming the transaction data monthly and the subscription data quarterly.</span></span>  <span data-ttu-id="e07a6-149">Med hjälp av vinst-/förlust data justerar Machine Learning algoritmerna och validerar att modellerna fungerar som förväntat genom att jämföra kluster rekommendationer med affärs möjligheter som har bearbetats i MSX.</span><span class="sxs-lookup"><span data-stu-id="e07a6-149">Using the win/loss data, the Machine Learning adjusts the algorithms and validates that the models are working as expected by comparing cluster recommendations to opportunities acted upon in MSX.</span></span>

:::image type="content" source="images/pci/cust-oppor-4.png" alt-text="Skärm bild av SMB Machine Learning.":::

## <a name="cloudascent-propensity"></a><span data-ttu-id="e07a6-151">CloudAscent benägenhet</span><span class="sxs-lookup"><span data-stu-id="e07a6-151">CloudAscent Propensity</span></span>

<span data-ttu-id="e07a6-152">Hur skapas benägenhet-rekommendationer?</span><span class="sxs-lookup"><span data-stu-id="e07a6-152">How are propensity recommendations created?</span></span>

<span data-ttu-id="e07a6-153">Genom att använda signaler som samlats in via webbcrawler och data från olika källor konsoliderar vi firmographics-data och kundens sociala medie signaler.</span><span class="sxs-lookup"><span data-stu-id="e07a6-153">Using signals collected via web crawlers and data provided from various sources, we consolidate the firmographics data and customer's social media signals.</span></span>  <span data-ttu-id="e07a6-154">Poängen använder dessa signaler och data i jämförelse modeller för anpassningar och bedömnings modeller för avsikten.</span><span class="sxs-lookup"><span data-stu-id="e07a6-154">The scoring uses these signals and data in comparison models for fit and scoring models for Intent.</span></span>

1. <span data-ttu-id="e07a6-155">Kund konto passning</span><span class="sxs-lookup"><span data-stu-id="e07a6-155">Customer Account Fit</span></span>

   - <span data-ttu-id="e07a6-156">Interna och externa data punkter som definierar firmographics.</span><span class="sxs-lookup"><span data-stu-id="e07a6-156">Internal and External data points that define firmographics.</span></span>

   - <span data-ttu-id="e07a6-157">Anpassnings bedömnings använder en modell som liknar vår bästa SMB för att jämföra kunder och se om de är en potentiell anpassning för Microsoft Cloud produkter.</span><span class="sxs-lookup"><span data-stu-id="e07a6-157">Fit scoring uses a look alike model to our best SMB to compare customers and see if they're a potential  fit for Microsoft Cloud Products.</span></span>

   - <span data-ttu-id="e07a6-158">Anpassnings resultat uppdateras varje kvartal</span><span class="sxs-lookup"><span data-stu-id="e07a6-158">Fit scoring is updated quarterly</span></span>

2. <span data-ttu-id="e07a6-159">Avsikt för kund konto</span><span class="sxs-lookup"><span data-stu-id="e07a6-159">Customer Account Intent</span></span>

   - <span data-ttu-id="e07a6-160">Signaler som rör sociala medier och en kunds beteende för online-beteende definierar avsikt.</span><span class="sxs-lookup"><span data-stu-id="e07a6-160">Signals related to Social media and a customer's online behavior define Intent.</span></span>

   - <span data-ttu-id="e07a6-161">Poängen för avsikten är överordnad för att definiera klustren.</span><span class="sxs-lookup"><span data-stu-id="e07a6-161">Intent scoring is overlaid on top of fit to define the clusters.</span></span>

   - <span data-ttu-id="e07a6-162">Avsikts poängen uppdateras varje månad.</span><span class="sxs-lookup"><span data-stu-id="e07a6-162">Intent scoring is updated monthly.</span></span>

   :::image type="content" source="images/pci/cust-oppor-5.png" alt-text="CloudAscent SMB förutsägande modeller.":::

3. <span data-ttu-id="e07a6-164">Klustring</span><span class="sxs-lookup"><span data-stu-id="e07a6-164">Clustering</span></span>

   <span data-ttu-id="e07a6-165">Signalerna för passa och avsikten samlas in i ett kluster poäng.</span><span class="sxs-lookup"><span data-stu-id="e07a6-165">The Signals for fit and intent are consolidated into a clustering score.</span></span> <span data-ttu-id="e07a6-166">CloudAscent har fyra kluster:</span><span class="sxs-lookup"><span data-stu-id="e07a6-166">CloudAscent has four clusters:</span></span>

      - <span data-ttu-id="e07a6-167">Handla nu – försäljnings klara kunder</span><span class="sxs-lookup"><span data-stu-id="e07a6-167">Act Now - sales ready customers</span></span>
      - <span data-ttu-id="e07a6-168">Utvärdera – marknadsförings klara kunder</span><span class="sxs-lookup"><span data-stu-id="e07a6-168">Evaluate - marketing ready customers</span></span>
      - <span data-ttu-id="e07a6-169">Nurture – disk medvetenhets kampanjer</span><span class="sxs-lookup"><span data-stu-id="e07a6-169">Nurture - drive awareness campaigns</span></span>
      - <span data-ttu-id="e07a6-170">Utbilda – utbilda och övervaka för avsikt</span><span class="sxs-lookup"><span data-stu-id="e07a6-170">Educate - educate and monitor for intent</span></span>

   <span data-ttu-id="e07a6-171">Med klustringen kan användarna rikta in sig på specifika kunder för försäljnings-och marknadsförings initiativ baserat på segment faktorer, till exempel: produkt, geo, bransch och vertikal.</span><span class="sxs-lookup"><span data-stu-id="e07a6-171">The clustering allows users to target specific customers for sales and marketing initiatives based on segment factors, for example: product, geo, industry and vertical.</span></span>

   <span data-ttu-id="e07a6-172">Fliken **benägenhet modell** i arbets böckerna CloudAscent delar benägenhet och den beräknade intäkten på tomt utrymme.</span><span class="sxs-lookup"><span data-stu-id="e07a6-172">The **Propensity model** tab in the CloudAscent Workbooks shares the propensity and the estimated whitespace revenue.</span></span> <span data-ttu-id="e07a6-173">Vi går igenom följande steg för att definiera klustring av anpassning och avsikt:</span><span class="sxs-lookup"><span data-stu-id="e07a6-173">To define the clustering of Fit and Intent, we go through the following steps:</span></span>

      1. <span data-ttu-id="e07a6-174">Med hjälp av ML-modeller beräknar vi först kund anpassnings poängen och avsikts poängen på en skala på 100.</span><span class="sxs-lookup"><span data-stu-id="e07a6-174">Using ML Models, we first calculate Customer Fit Score and intent Score on a scale of 100.</span></span>  <span data-ttu-id="e07a6-175">Exakta resultat varierar beroende på ML-modeller.</span><span class="sxs-lookup"><span data-stu-id="e07a6-175">Exact Scores will vary based on ML Models.</span></span>  <span data-ttu-id="e07a6-176">Exempel resultat nedan:</span><span class="sxs-lookup"><span data-stu-id="e07a6-176">Example Scores Below:</span></span>

         |<span data-ttu-id="e07a6-177">**Klassificering**</span><span class="sxs-lookup"><span data-stu-id="e07a6-177">**Classification**</span></span>|<span data-ttu-id="e07a6-178">**Resultat**</span><span class="sxs-lookup"><span data-stu-id="e07a6-178">**Score**</span></span>|
         |---------|:---------|
         |<span data-ttu-id="e07a6-179">Hög</span><span class="sxs-lookup"><span data-stu-id="e07a6-179">High</span></span>|<span data-ttu-id="e07a6-180">75 – 100</span><span class="sxs-lookup"><span data-stu-id="e07a6-180">75 - 100</span></span>|
         |<span data-ttu-id="e07a6-181">Medium</span><span class="sxs-lookup"><span data-stu-id="e07a6-181">Medium</span></span>|<span data-ttu-id="e07a6-182">55 – 74</span><span class="sxs-lookup"><span data-stu-id="e07a6-182">55 - 74</span></span>|
         |<span data-ttu-id="e07a6-183">Låg</span><span class="sxs-lookup"><span data-stu-id="e07a6-183">Low</span></span>|<span data-ttu-id="e07a6-184">30 - 54</span><span class="sxs-lookup"><span data-stu-id="e07a6-184">30 - 54</span></span>|
         |<span data-ttu-id="e07a6-185">Mycket låg</span><span class="sxs-lookup"><span data-stu-id="e07a6-185">Very Low</span></span>|<span data-ttu-id="e07a6-186">0 - 29</span><span class="sxs-lookup"><span data-stu-id="e07a6-186">0 - 29</span></span>|

      2. <span data-ttu-id="e07a6-187">Med regeln ovan klassificerar vi företag som hög, medel, låg och mycket låg i både kund anpassningar och avsikts signaler.</span><span class="sxs-lookup"><span data-stu-id="e07a6-187">Using the rule above, we classify companies to be High, Medium, Low, and Very Low across both Customer Fit    and Intent Signals.</span></span>

      3. <span data-ttu-id="e07a6-188">Vi åker kundernas passnings-och avsikts signaler på en 2D-matris med varje skärnings punkt som representerar benägenhet.</span><span class="sxs-lookup"><span data-stu-id="e07a6-188">We plot customer fit and intent signals on a 2D matrix with each intersection representing the propensity.</span></span>     <span data-ttu-id="e07a6-189">Till exempel hög passning + hög avsikt = a1 som representerar den högsta benägenhet.</span><span class="sxs-lookup"><span data-stu-id="e07a6-189">For Example, High Fit + High Intent = A1, representing the highest propensity.</span></span>

      4. <span data-ttu-id="e07a6-190">Slutligen är segment gruppen till att bilda kluster.</span><span class="sxs-lookup"><span data-stu-id="e07a6-190">Finally, these segments group to form clusters.</span></span>  <span data-ttu-id="e07a6-191">Till exempel a1, a2, A3, A4 form fungerar nu-klustret.</span><span class="sxs-lookup"><span data-stu-id="e07a6-191">For Example, A1, A2, A3, A4 form the Act Now cluster.</span></span>

         :::image type="content" source="images/pci/cust-oppor-6.png" alt-text="CloudAscent-modeller.":::

   <span data-ttu-id="e07a6-193">För dessa kunder rekommenderar vi att du riktar in dig på målet och utvärderar kunderna.</span><span class="sxs-lookup"><span data-stu-id="e07a6-193">For these customers, we recommend targeting Act Now and Evaluate customers.</span></span>

## <a name="cloudascent-products--models"></a><span data-ttu-id="e07a6-194">CloudAscent-produkter & modeller</span><span class="sxs-lookup"><span data-stu-id="e07a6-194">CloudAscent Products & Models</span></span>

<span data-ttu-id="e07a6-195">Följande bild visar en vy över varje benägenhet-modell i CloudAscent:</span><span class="sxs-lookup"><span data-stu-id="e07a6-195">The following graphic provides a view of each propensity model within CloudAscent:</span></span>

:::image type="content" source="images/pci/cust-oppor-7.png" alt-text="CloudAscent benägenhet-modell.":::

<span data-ttu-id="e07a6-197">Blank stegs modeller består av förutsägelser för befintliga Microsoft-kunder där de inte har en produkt och/eller är kunder med nya kunder.</span><span class="sxs-lookup"><span data-stu-id="e07a6-197">Whitespace models are composed of predictions for existing Microsoft customers where they don't have a product and/or are net new prospect customers.</span></span>

<span data-ttu-id="e07a6-198">Merförsäljning-modeller använder transaktions data för att förutsäga potentialen för merförsäljning i Azure-och M365-SKU: er.</span><span class="sxs-lookup"><span data-stu-id="e07a6-198">Upsell models use transaction data to predict the potential for upsell in Azure and M365 SKUs.</span></span>

<span data-ttu-id="e07a6-199">EOS delar service kundernas slut för Win 7, Office 2010, SQL Server och Windows Server.</span><span class="sxs-lookup"><span data-stu-id="e07a6-199">EOS shares the end of service customers for Win 7, Office 2010, SQL Server, and Windows Server.</span></span> <span data-ttu-id="e07a6-200">EOS-data hämtas från MS Sales och överlappar med CloudAscent benägenhet-modellen där det är möjligt.</span><span class="sxs-lookup"><span data-stu-id="e07a6-200">The EOS data is pulled from MS Sales and overlaid with the CloudAscent propensity modeling where available.</span></span> <span data-ttu-id="e07a6-201">EOS data liv i det moderna arbetet och Azure Sales spelar.</span><span class="sxs-lookup"><span data-stu-id="e07a6-201">EOS data lives in the Modern Work and Azure Sales plays.</span></span>
