---
title: Partner Center-insikter – Rapporter om molnocent- sida
description: Lär dig mer om cloudAscent Propensity-rapporter i Partnercenter. Innehåller information om en kunds ighet att köpa Microsoft-produkter.
ms.topic: conceptual
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 04/27/2021
ms.openlocfilehash: 430aea81964d1b75514b6e1377bd2ba1af41b538
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 05/19/2021
ms.locfileid: "110153046"
---
# <a name="cloudascent-propensity-reports-available-from-partner-center-dashboard"></a><span data-ttu-id="133c1-104">CloudAscent Propensity-rapporter som är tillgängliga från instrumentpanelen i Partnercenter</span><span class="sxs-lookup"><span data-stu-id="133c1-104">CloudAscent Propensity reports available from Partner Center dashboard</span></span>

<span data-ttu-id="133c1-105">**Lämpliga roller:** Användare av | Rapportvisningsprogram</span><span class="sxs-lookup"><span data-stu-id="133c1-105">**Appropriate roles**: Executive report viewer | Report viewer</span></span>

<span data-ttu-id="133c1-106">Instrumentpanelen i Partnercenter innehåller nedladdningsbara beständiga data från CloudAscent-programmet.</span><span class="sxs-lookup"><span data-stu-id="133c1-106">The Partner Center dashboard provides downloadable propensity data from the CloudAscent program.</span></span> <span data-ttu-id="133c1-107">Data visar kundernas sannolikhet att köpa Microsoft-produkter.</span><span class="sxs-lookup"><span data-stu-id="133c1-107">The data shows the customers' likelihood to purchase Microsoft products.</span></span>  <span data-ttu-id="133c1-108">I den här artikeln beskrivs analys av dessa data, hur bedömning används och vad det innebär.</span><span class="sxs-lookup"><span data-stu-id="133c1-108">This article describes the breakdown of this data, how to use the scoring, and what it means.</span></span>

## <a name="summary-definitions"></a><span data-ttu-id="133c1-109">Sammanfattningsdefinitioner</span><span class="sxs-lookup"><span data-stu-id="133c1-109">Summary definitions</span></span>

- <span data-ttu-id="133c1-110">**SMC-kunder**– Det här är det totala antalet kunder som har ighetsnedladdningar.</span><span class="sxs-lookup"><span data-stu-id="133c1-110">**SMC Customers**– This is the total number of customers in the propensity downloads.</span></span>  <span data-ttu-id="133c1-111">Kunder identifieras av en postpartner.</span><span class="sxs-lookup"><span data-stu-id="133c1-111">Customers are identified by partner of record.</span></span>
- <span data-ttu-id="133c1-112">**Upphör att** gälla – Under det aktuella räkenskapsåret tillhandahåller vi antalet utgångna avtal.</span><span class="sxs-lookup"><span data-stu-id="133c1-112">**Expire Agreements**– Within the current fiscal year, we're providing the number of expiring agreements.</span></span>
- <span data-ttu-id="133c1-113">**Öppna Förfallande intäkter**– De intäkter som är associerade med de öppna utgångna avtalen.</span><span class="sxs-lookup"><span data-stu-id="133c1-113">**Open Expiring Revenue**– The revenue associated to the open expiring agreements.</span></span>

:::image type="content" source="images/pci/cust-oppor-11.png" alt-text="Skärmbild av instrumentpanelen Sammanfattning av kundmöjligheter.":::

## <a name="cloudascent-smb-segmentation"></a><span data-ttu-id="133c1-115">CloudAscent SMB-segmentering</span><span class="sxs-lookup"><span data-stu-id="133c1-115">CloudAscent SMB segmentation</span></span>

<span data-ttu-id="133c1-116">SMB-segmentet (small to medium business) är indelat i tre distinkta delsegment.</span><span class="sxs-lookup"><span data-stu-id="133c1-116">The small to medium business (SMB) segment is divided into three distinct sub segments.</span></span>

1. <span data-ttu-id="133c1-117">**De största ohanterade innehåller** de största SMB-kunderna med flest möjligheter för Microsoft.</span><span class="sxs-lookup"><span data-stu-id="133c1-117">**Top Unmanaged** includes the largest SMB customers with the most opportunity for Microsoft.</span></span> <span data-ttu-id="133c1-118">Vanliga kunder som inte är mest ohanterade har liknande egenskaper som hanterade konton, med ett stort antal anställda, stora IT-budgetar och -utgifter samt stora mängder potentiella intäkter för Microsoft.</span><span class="sxs-lookup"><span data-stu-id="133c1-118">Typical Top Unmanaged customers share similar characteristics to Managed accounts, with large number of employees, large IT budgets and spend, and large amounts of potential revenue for Microsoft.</span></span>

   <span data-ttu-id="133c1-119">Vi definierar Top Unmanaged på två sätt:</span><span class="sxs-lookup"><span data-stu-id="133c1-119">We define Top Unmanaged in two ways:</span></span>

   - <span data-ttu-id="133c1-120">**Top Unmanaged User Based**– innehåller konton med 300 eller fler anställda.</span><span class="sxs-lookup"><span data-stu-id="133c1-120">**Top Unmanaged User Based**– includes accounts with 300 or more employees.</span></span> <span data-ttu-id="133c1-121">User-Based-konton är bra mål för första gången köp eller expansion av användarbaserade prenumerationsprodukter som Microsoft 365, Dynamics 365 eller Surface.</span><span class="sxs-lookup"><span data-stu-id="133c1-121">User-Based accounts are great targets for first-time purchase, or expansion of user-based subscription products such as Microsoft 365, Dynamics 365, or Surface.</span></span>
   - <span data-ttu-id="133c1-122">**Top Unmanaged Compute Based –** innehåller konton med azure-potential som är större än 10 000 USD.</span><span class="sxs-lookup"><span data-stu-id="133c1-122">**Top Unmanaged Compute Based** – includes accounts with Azure potential greater than $10k.</span></span> <span data-ttu-id="133c1-123">Beräkningsbaserade konton omfattar befintliga Azure.</span><span class="sxs-lookup"><span data-stu-id="133c1-123">Compute based accounts include existing Azure.</span></span> <span data-ttu-id="133c1-124">konton med betydande framtida års potential och konton som ännu inte har köpt Azure men som har potential för Azure som är större än 10 000 USD.</span><span class="sxs-lookup"><span data-stu-id="133c1-124">accounts with significant future year potential and accounts who have yet to purchase Azure yet but have potential for Azure greater than $10k.</span></span>

2. <span data-ttu-id="133c1-125">**Medium Business** innehåller befintliga kunder och konton för potentiella kunder med 25 till 300 anställda.</span><span class="sxs-lookup"><span data-stu-id="133c1-125">**Medium Business** includes existing customers and prospect accounts with 25 to 300 employees.</span></span>

3. <span data-ttu-id="133c1-126">**Små företag** omfattar företag med 10–25 anställda.</span><span class="sxs-lookup"><span data-stu-id="133c1-126">**Small Business** includes businesses with 10-25 employees.</span></span>

4. <span data-ttu-id="133c1-127">**I Very Small Business** finns företag med 1–9 anställda.</span><span class="sxs-lookup"><span data-stu-id="133c1-127">**Very Small Business** includes businesses with 1-9 employees.</span></span>

:::image type="content" source="images/pci/cust-oppor-2.png" alt-text="Kund efter SMC-typ.":::

<span data-ttu-id="133c1-129">**De främsta delsegmenten för** ohanterade och medelstora företag representerar LTV-kunder (High Life-Time Value) för Microsoft och Microsoft-partner. </span><span class="sxs-lookup"><span data-stu-id="133c1-129">**Top Unmanaged** and **Medium Business** subsegments represent high life-time value (LTV) customers for Microsoft, and Microsoft Partners.</span></span> <span data-ttu-id="133c1-130">Därför är de de viktiga fokusområdena för att öka tillväxten i det här segmentet.</span><span class="sxs-lookup"><span data-stu-id="133c1-130">Because of this, they're the lead areas of focus for driving growth in this segment.</span></span> <span data-ttu-id="133c1-131">I dessa två undersegment är vi bättre positionerade för att skaffa socketen med Microsoft 365, tjäna pengar ytterligare med D365-/LOB-appar (LOB) för Azure och realisera en hög LTV för Microsoft.</span><span class="sxs-lookup"><span data-stu-id="133c1-131">In these two subsegments, we're better positioned to acquire the socket with Microsoft 365, monetize further with D365/Azure line of business (LOB) apps, and realize a high LTV for Microsoft.</span></span>

<span data-ttu-id="133c1-132">Idag har vi två viktiga affärsmöjlighetsområden – 1.</span><span class="sxs-lookup"><span data-stu-id="133c1-132">Today we have two key areas of opportunity – 1.</span></span> <span data-ttu-id="133c1-133">vår kund ökar tillväxten; 2.</span><span class="sxs-lookup"><span data-stu-id="133c1-133">our customer adds growth; 2.</span></span> <span data-ttu-id="133c1-134">Även om det går bra att skaffa molnsocketar som leder Microsoft 365, har vi stora möjligheter i Dynamics 365 och Azure.</span><span class="sxs-lookup"><span data-stu-id="133c1-134">while we do well acquiring cloud sockets leading with Microsoft 365, we have a large opportunity in Dynamics 365 and Azure.</span></span>

<span data-ttu-id="133c1-135">Följande skärmbild representerar de fyra SMB-undersegmenten.</span><span class="sxs-lookup"><span data-stu-id="133c1-135">The following screenshot represents the four SMB Subsegments.</span></span> <span data-ttu-id="133c1-136">CloudAscent prioriterar profilering, bedömning och modellering av alla konton i de främsta ohanterade och medelstora företagarna.</span><span class="sxs-lookup"><span data-stu-id="133c1-136">CloudAscent prioritize the profiling, scoring, and modeling of all Top Unmanaged and Medium Business accounts.</span></span>

:::image type="content" source="images/pci/cust-oppor-32.png" alt-text="Skärmbild av SMB-undersegment.":::

## <a name="cloudascent-machine-learning"></a><span data-ttu-id="133c1-138">CloudAscent Machine Learning</span><span class="sxs-lookup"><span data-stu-id="133c1-138">CloudAscent Machine Learning</span></span>

<span data-ttu-id="133c1-139">SMB använder maskininlärningsteknik för att driva kundförutsägelser för försäljning och marknadsföring inom de viktigaste segmenten ohanterade och medelstora företag.</span><span class="sxs-lookup"><span data-stu-id="133c1-139">SMB uses machine learning technology to drive sales and marketing customer predictions within the Top Unmanaged and Medium Business segments.</span></span> <span data-ttu-id="133c1-140">Hur samlas signaler in och omvandlas till rekommendationer om benägenhet?</span><span class="sxs-lookup"><span data-stu-id="133c1-140">How are signals collected and turned into propensity recommendations?</span></span>

- <span data-ttu-id="133c1-141">**Datainsamling:** Webbrobotar söker igenom och samlar in miljarder kundsignaler genom att pinga företagsdomänerna och övervaka blogginlägg, pressutgåor, sociala strömmar och tekniska forum.</span><span class="sxs-lookup"><span data-stu-id="133c1-141">**Data Collection**: Web crawlers scan and collect billions of customer signals by pinging the company domains, and monitoring blog posts, press releases, social streams, and technical forums.</span></span>  <span data-ttu-id="133c1-142">Förutom insamlade signaler samlas företagsinformation in från både interna och externa källor som D&B, Microsoft Internal-prenumeration och transaktionsdata.</span><span class="sxs-lookup"><span data-stu-id="133c1-142">In addition to the collected signals, firmographics information is collected from both internal and external sources such as D&B, Microsoft Internal subscription and transactional data.</span></span>

- <span data-ttu-id="133c1-143">**Machine Learning:** Signalerna matas in i maskininlärningsmodellen som matar ut en strukturerad datauppsättning med försäljnings- och marknadsföringsförutsägelser för varje kund efter molnprodukt och kluster.</span><span class="sxs-lookup"><span data-stu-id="133c1-143">**Machine Learning**: The signals are fed into the machine learning model that outputs a structured data set of Sales and Marketing predictions for each customer by cloud product and cluster.</span></span>  <span data-ttu-id="133c1-144">Varje kund poängeras med en modell av samma utseende som Microsofts främsta SMB som avgör kundens Anpassa, och maskininlärningsalgoritmer som integrerar kundens onlinebeteende definieras som Avsikt.</span><span class="sxs-lookup"><span data-stu-id="133c1-144">Each customer is scored using a look alike model to Microsoft's top SMB that determines the customer's Fit, and machine learning algorithms that integrate the customer's online behavior define as Intent.</span></span> <span data-ttu-id="133c1-145">Poängen sammanfogas i kluster som visar en kunds önskemål om att köpa Microsoft Cloud Products.</span><span class="sxs-lookup"><span data-stu-id="133c1-145">The scoring is merged into clusters that show a customer's propensity to purchase Microsoft Cloud Products.</span></span>

- <span data-ttu-id="133c1-146">**Optimering:** Machine Learning optimerar modellerna genom att använda transaktionsdata varje månad och prenumerationsdata kvartalsvis.</span><span class="sxs-lookup"><span data-stu-id="133c1-146">**Optimization**: The Machine Learning system optimizes the models by consuming the transaction data monthly and the subscription data quarterly.</span></span>  <span data-ttu-id="133c1-147">Med hjälp av win/loss-data justerar Machine Learning algoritmerna och verifierar att modellerna fungerar som förväntat genom att jämföra klusterrekommendationerna med affärsmöjligheter som åtgärdas i MSX.</span><span class="sxs-lookup"><span data-stu-id="133c1-147">Using the win/loss data, the Machine Learning adjusts the algorithms and validates that the models are working as expected by comparing cluster recommendations to opportunities acted upon in MSX.</span></span>

:::image type="content" source="images/pci/cust-oppor-4.png" alt-text="Skärmbild av SMB-maskininlärning.":::

## <a name="cloudascent-propensity"></a><span data-ttu-id="133c1-149">CloudAscent-ständiga</span><span class="sxs-lookup"><span data-stu-id="133c1-149">CloudAscent Propensity</span></span>

<span data-ttu-id="133c1-150">Hur skapas rekommendationer för rekommendationer om rekommendationer för rekommendationer?</span><span class="sxs-lookup"><span data-stu-id="133c1-150">How are propensity recommendations created?</span></span>

<span data-ttu-id="133c1-151">Med hjälp av signaler som samlas in via webb crawlers och data från olika källor konsoliderar vi företagets data och kundens signaler på sociala medier.</span><span class="sxs-lookup"><span data-stu-id="133c1-151">Using signals collected via web crawlers and data provided from various sources, we consolidate the firmographics data and customer's social media signals.</span></span>  <span data-ttu-id="133c1-152">Poängen använder dessa signaler och data i jämförelsemodeller för anpassa och bedömningsmodeller för avsikt.</span><span class="sxs-lookup"><span data-stu-id="133c1-152">The scoring uses these signals and data in comparison models for fit and scoring models for Intent.</span></span>

1. <span data-ttu-id="133c1-153">Anpassa kundkonto</span><span class="sxs-lookup"><span data-stu-id="133c1-153">Customer Account Fit</span></span>

   - <span data-ttu-id="133c1-154">Interna och externa datapunkter som definierar företagsgrafiska data.</span><span class="sxs-lookup"><span data-stu-id="133c1-154">Internal and External data points that define firmographics.</span></span>

   - <span data-ttu-id="133c1-155">Fit scoring använder en modell av samma utseende som vår bästa SMB för att jämföra kunder och se om de är lämpliga för Microsoft Cloud Products.</span><span class="sxs-lookup"><span data-stu-id="133c1-155">Fit scoring uses a look alike model to our best SMB to compare customers and see if they're a potential  fit for Microsoft Cloud Products.</span></span>

   - <span data-ttu-id="133c1-156">Bedömning av passning uppdateras kvartalsvis</span><span class="sxs-lookup"><span data-stu-id="133c1-156">Fit scoring is updated quarterly</span></span>

2. <span data-ttu-id="133c1-157">Avsikt för kundkonto</span><span class="sxs-lookup"><span data-stu-id="133c1-157">Customer Account Intent</span></span>

   - <span data-ttu-id="133c1-158">Signaler relaterade till sociala medier och en kunds onlinebeteende definierar Intent.</span><span class="sxs-lookup"><span data-stu-id="133c1-158">Signals related to Social media and a customer's online behavior define Intent.</span></span>

   - <span data-ttu-id="133c1-159">Avsiktsbedömningen överlagras ovanpå passning för att definiera klustren.</span><span class="sxs-lookup"><span data-stu-id="133c1-159">Intent scoring is overlaid on top of fit to define the clusters.</span></span>

   - <span data-ttu-id="133c1-160">Avsiktsbedömningen uppdateras varje månad.</span><span class="sxs-lookup"><span data-stu-id="133c1-160">Intent scoring is updated monthly.</span></span>

   :::image type="content" source="images/pci/cust-oppor-5.png" alt-text="CloudAscent SMB-förutsägelsemodeller.":::

3. <span data-ttu-id="133c1-162">Klustring</span><span class="sxs-lookup"><span data-stu-id="133c1-162">Clustering</span></span>

   <span data-ttu-id="133c1-163">Signalerna för passning och avsikt konsolideras till en klustringspoäng.</span><span class="sxs-lookup"><span data-stu-id="133c1-163">The Signals for fit and intent are consolidated into a clustering score.</span></span> <span data-ttu-id="133c1-164">CloudAscent har fyra kluster:</span><span class="sxs-lookup"><span data-stu-id="133c1-164">CloudAscent has four clusters:</span></span>

      - <span data-ttu-id="133c1-165">Agera nu – kunder som är redo för försäljning</span><span class="sxs-lookup"><span data-stu-id="133c1-165">Act Now - sales ready customers</span></span>
      - <span data-ttu-id="133c1-166">Utvärdera – marknadsföringsklara kunder</span><span class="sxs-lookup"><span data-stu-id="133c1-166">Evaluate - marketing ready customers</span></span>
      - <span data-ttu-id="133c1-167">Vård – främja medvetenhetskampanjer</span><span class="sxs-lookup"><span data-stu-id="133c1-167">Nurture - drive awareness campaigns</span></span>
      - <span data-ttu-id="133c1-168">Utbilda – utbilda och övervaka avsikter</span><span class="sxs-lookup"><span data-stu-id="133c1-168">Educate - educate and monitor for intent</span></span>

   <span data-ttu-id="133c1-169">Klustringen gör att användare kan rikta in sig på specifika kunder för sälj- och marknadsföringsinitiativ baserat på segmentfaktorer, till exempel produkt, geo, bransch och vertikal.</span><span class="sxs-lookup"><span data-stu-id="133c1-169">The clustering allows users to target specific customers for sales and marketing initiatives based on segment factors, for example: product, geo, industry and vertical.</span></span>

   <span data-ttu-id="133c1-170">Fliken **Propensity model (Propensity Model)** i CloudAscent-arbetsböcker delar heten och de beräknade utrymmesintäkterna.</span><span class="sxs-lookup"><span data-stu-id="133c1-170">The **Propensity model** tab in the CloudAscent Workbooks shares the propensity and the estimated whitespace revenue.</span></span> <span data-ttu-id="133c1-171">För att definiera klustringen av Anpassa och Avsikt går vi igenom följande steg:</span><span class="sxs-lookup"><span data-stu-id="133c1-171">To define the clustering of Fit and Intent, we go through the following steps:</span></span>

      1. <span data-ttu-id="133c1-172">Med hjälp av ML-modeller beräknar vi först kundpoäng och avsiktspoäng på en skala på 100.</span><span class="sxs-lookup"><span data-stu-id="133c1-172">Using ML Models, we first calculate Customer Fit Score and intent Score on a scale of 100.</span></span>  <span data-ttu-id="133c1-173">Exakta poäng varierar beroende på ML-modeller.</span><span class="sxs-lookup"><span data-stu-id="133c1-173">Exact Scores will vary based on ML Models.</span></span>  <span data-ttu-id="133c1-174">Exempelresultat nedan:</span><span class="sxs-lookup"><span data-stu-id="133c1-174">Example Scores Below:</span></span>

         |<span data-ttu-id="133c1-175">**Klassificering**</span><span class="sxs-lookup"><span data-stu-id="133c1-175">**Classification**</span></span>|<span data-ttu-id="133c1-176">**Poäng**</span><span class="sxs-lookup"><span data-stu-id="133c1-176">**Score**</span></span>|
         |---------|:---------|
         |<span data-ttu-id="133c1-177">Högt</span><span class="sxs-lookup"><span data-stu-id="133c1-177">High</span></span>|<span data-ttu-id="133c1-178">75 - 100</span><span class="sxs-lookup"><span data-stu-id="133c1-178">75 - 100</span></span>|
         |<span data-ttu-id="133c1-179">Medel</span><span class="sxs-lookup"><span data-stu-id="133c1-179">Medium</span></span>|<span data-ttu-id="133c1-180">55 - 74</span><span class="sxs-lookup"><span data-stu-id="133c1-180">55 - 74</span></span>|
         |<span data-ttu-id="133c1-181">Låg</span><span class="sxs-lookup"><span data-stu-id="133c1-181">Low</span></span>|<span data-ttu-id="133c1-182">30 - 54</span><span class="sxs-lookup"><span data-stu-id="133c1-182">30 - 54</span></span>|
         |<span data-ttu-id="133c1-183">Mycket låg</span><span class="sxs-lookup"><span data-stu-id="133c1-183">Very Low</span></span>|<span data-ttu-id="133c1-184">0 - 29</span><span class="sxs-lookup"><span data-stu-id="133c1-184">0 - 29</span></span>|

      2. <span data-ttu-id="133c1-185">Med hjälp av regeln ovan klassificerar vi företag som Hög, Medel, Låg och Mycket låg för både Customer Fit och Intent Signals.</span><span class="sxs-lookup"><span data-stu-id="133c1-185">Using the rule above, we classify companies to be High, Medium, Low, and Very Low across both Customer Fit and Intent Signals.</span></span>

      3. <span data-ttu-id="133c1-186">Vi ritar kundens passnings- och avsiktssignaler på en 2D-matris där varje skärningspunkt representerar återgivningen.</span><span class="sxs-lookup"><span data-stu-id="133c1-186">We plot customer fit and intent signals on a 2D matrix with each intersection representing the propensity.</span></span> <span data-ttu-id="133c1-187">Till exempel hög passning + hög avsikt = A1, som representerar den högsta återgivningen.</span><span class="sxs-lookup"><span data-stu-id="133c1-187">For Example, High Fit + High Intent = A1, representing the highest propensity.</span></span>

      4. <span data-ttu-id="133c1-188">Slutligen grupperar dessa segment för att bilda kluster.</span><span class="sxs-lookup"><span data-stu-id="133c1-188">Finally, these segments group to form clusters.</span></span>  <span data-ttu-id="133c1-189">A1, A2, A3 och A4 utgör till exempel Act Now-klustret.</span><span class="sxs-lookup"><span data-stu-id="133c1-189">For Example, A1, A2, A3, A4 form the Act Now cluster.</span></span>

         :::image type="content" source="images/pci/cust-oppor-6.png" alt-text="CloudAscent-modeller.":::

   <span data-ttu-id="133c1-191">För dessa kunder rekommenderar vi att du riktar in dig på Agera nu och Utvärdera kunder.</span><span class="sxs-lookup"><span data-stu-id="133c1-191">For these customers, we recommend targeting Act Now and Evaluate customers.</span></span>

## <a name="cloudascent-products--models"></a><span data-ttu-id="133c1-192">CloudAscent Products & Models</span><span class="sxs-lookup"><span data-stu-id="133c1-192">CloudAscent Products & Models</span></span>

<span data-ttu-id="133c1-193">Följande bild visar en vy över varje benägenhetsmodell i CloudAscent:</span><span class="sxs-lookup"><span data-stu-id="133c1-193">The following graphic provides a view of each propensity model within CloudAscent:</span></span>

:::image type="content" source="images/pci/cust-oppor-7.png" alt-text="CloudAscent-benägenhetsmodell.":::

<span data-ttu-id="133c1-195">Blankstegsmodeller består av förutsägelser för befintliga Microsoft-kunder där de inte har någon produkt och/eller är netto nya kunder.</span><span class="sxs-lookup"><span data-stu-id="133c1-195">Whitespace models are composed of predictions for existing Microsoft customers where they don't have a product and/or are net new prospect customers.</span></span>

<span data-ttu-id="133c1-196">Modeller för merförsäljning använder transaktionsdata för att förutsäga potentialen för merförsäljning i Azure och Microsoft 365 SKU:er.</span><span class="sxs-lookup"><span data-stu-id="133c1-196">Upsell models use transaction data to predict the potential for upsell in Azure and Microsoft 365 SKUs.</span></span>

<span data-ttu-id="133c1-197">Dessa kunder kommer redan att ha både Azure Microsoft 365 och uppförsäljningsmodellen visar att de sannolikt kommer att köpa mer av sin befintliga SKU.</span><span class="sxs-lookup"><span data-stu-id="133c1-197">These customers will already have both Azure or Microsoft 365 and the upsell model shows that they’re likely to purchase more of their existing SKU.</span></span>

<span data-ttu-id="133c1-198">EOS delar EOS-kunder (End of Service) för Win 7, Office 2010, SQL Server och Windows Server.</span><span class="sxs-lookup"><span data-stu-id="133c1-198">EOS shares the end of service (EOS) customers for Win 7, Office 2010, SQL Server, and Windows Server.</span></span> <span data-ttu-id="133c1-199">EOS-data hämtas från MS Sales och överlagras med CloudAscent-modellering där det är tillgängligt.</span><span class="sxs-lookup"><span data-stu-id="133c1-199">The EOS data is pulled from MS Sales and overlaid with the CloudAscent propensity modeling where available.</span></span> <span data-ttu-id="133c1-200">EOS-data finns i Modern Work och Azure Sales spelar.</span><span class="sxs-lookup"><span data-stu-id="133c1-200">EOS data lives in the Modern Work and Azure Sales plays.</span></span>
