---
title: Fakturering av Azure-plan – faktura & rekognoseringar-filer
ms.topic: article
ms.date: 07/02/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Lär dig hur du får åtkomst till och förstår den faktura och avstämnings fil struktur som är relaterad till faktureringen för Azure-prenumerationen.
author: khpavan
ms.author: sakhanda
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 5d8bb85357d796ae4917faf91c93db8fef4369c2
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/22/2020
ms.locfileid: "92531556"
---
# <a name="new-commerce-experience-in-csp---azure-billing"></a><span data-ttu-id="58215-103">Ny Commerce-upplevelse i CSP – Azure-fakturering</span><span class="sxs-lookup"><span data-stu-id="58215-103">New commerce experience in CSP - Azure billing</span></span> 

<span data-ttu-id="58215-104">**Lämpliga roller:**</span><span class="sxs-lookup"><span data-stu-id="58215-104">**Appropriate roles:**</span></span>

- <span data-ttu-id="58215-105">Administratörs agent</span><span class="sxs-lookup"><span data-stu-id="58215-105">Admin agent</span></span>
- <span data-ttu-id="58215-106">Faktureringsadministratör</span><span class="sxs-lookup"><span data-stu-id="58215-106">Billing admin</span></span>
- <span data-ttu-id="58215-107">Global administratör</span><span class="sxs-lookup"><span data-stu-id="58215-107">Global admin</span></span>

<span data-ttu-id="58215-108">Faktureringen enligt Azure-planen är en förenklad fakturerings upplevelse med ett justerat fakturerings datum och en månads-baserad fakturerings period.</span><span class="sxs-lookup"><span data-stu-id="58215-108">Billing under the Azure plan is a simplified billing experience using an aligned single billing date and calendar month-based billing period.</span></span>

## <a name="summary-of-billing-essentials"></a><span data-ttu-id="58215-109">Sammanfattning av fakturerings grunderna</span><span class="sxs-lookup"><span data-stu-id="58215-109">Summary of billing essentials</span></span>

- <span data-ttu-id="58215-110">**Faktura datum** : faktura-och avstämnings fil kommer att finnas i Partner Center Dashboard/API med 8 (midnatt UTC).</span><span class="sxs-lookup"><span data-stu-id="58215-110">**Invoice date** : Invoice and reconciliation file will be available in the Partner Center dashboard/API by the 8th (midnight UTC).</span></span>

- <span data-ttu-id="58215-111">**Fakturerings period för faktura** : faktura fakturerings perioden justeras till kalender månaden, till exempel 10/1-10/31, 11/1-11/30.</span><span class="sxs-lookup"><span data-stu-id="58215-111">**Invoice billing period** : The invoice billing period is aligned to the calendar month, for example,  10/1-10/31, 11/1-11/30.</span></span>

- <span data-ttu-id="58215-112">**Debitering av service perioder** : avgifterna justeras till kalender månaden.</span><span class="sxs-lookup"><span data-stu-id="58215-112">**Charge service periods** : Charges will align to the calendar month.</span></span> <span data-ttu-id="58215-113">Om den fakturerade partnern till exempel lägger till Azure-tjänster via en Azure-plan på 10/15 och kunden börjar förbrukningen av Azure-tjänster på 10/15, får fakturerad partner faktura-rekognoseringar på 11/8 för kund förbrukning för service perioden 10/15-10/31.</span><span class="sxs-lookup"><span data-stu-id="58215-113">For example, if billed partner adds Azure services through an Azure plan on 10/15 and the customer begins consumption of Azure services on 10/15, then billed partner will receive invoice/recon on 11/8 for customer consumption for the service period 10/15 - 10/31.</span></span> <span data-ttu-id="58215-114">Nästa månads faktura som ska genereras på 12/8 innehåller alla avgifter för service perioden 11/1-11/31.</span><span class="sxs-lookup"><span data-stu-id="58215-114">The next month's invoice that is going to be generated on 12/8 contains all the charges for the service period 11/1- 11/31.</span></span>

- <span data-ttu-id="58215-115">**Faktura betalnings villkor** : net 60 dagar.</span><span class="sxs-lookup"><span data-stu-id="58215-115">**Invoice payment term** : Net 60 days.</span></span>

- <span data-ttu-id="58215-116">**Faktura valuta** : partner kommer fortsätta att faktureras i kundens country's-tilldelade valuta.</span><span class="sxs-lookup"><span data-stu-id="58215-116">**Invoice currency** : Partners will continue to be billed in the customer's country's assigned currency.</span></span> <span data-ttu-id="58215-117">Om den fakturerade partnern till exempel är i Irland med kunder i Storbritannien, Norge och Tyskland får den fakturerade partnern ett GBP, NOK och faktura/rekognoseringar EUR.</span><span class="sxs-lookup"><span data-stu-id="58215-117">For example, if the billed partner is in Ireland with customers in the UK, Norway, and Germany, then the billed partner will receive a GBP, NOK, and EUR invoice/recon.</span></span>

- <span data-ttu-id="58215-118">**Partner incitament** : betalda 45 dagar från slutet av faktura månaden.</span><span class="sxs-lookup"><span data-stu-id="58215-118">**Partner incentives** : Paid 45 days from the end of the invoice month.</span></span>

## <a name="access-your-invoices-and-reconciliation-files"></a><span data-ttu-id="58215-119">Få åtkomst till dina fakturor och avstämnings filer</span><span class="sxs-lookup"><span data-stu-id="58215-119">Access your invoices and reconciliation files</span></span>

<span data-ttu-id="58215-120">Den globala administratörs-eller fakturerings administratören för ditt företag får ett e-postmeddelande när en faktura är klar att visa.</span><span class="sxs-lookup"><span data-stu-id="58215-120">The global admin or billing admin for your company will receive an email when an invoice is ready to view.</span></span>

<span data-ttu-id="58215-121">För att få åtkomst till fakturan och avstämnings filen:</span><span class="sxs-lookup"><span data-stu-id="58215-121">To access the invoice and reconciliation file:</span></span>

1. <span data-ttu-id="58215-122">Logga in på Partner Center- [instrumentpanelen](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="58215-122">Sign in to the Partner Center [dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="58215-123">Från menyn Partner Center väljer du **fakturering** .</span><span class="sxs-lookup"><span data-stu-id="58215-123">From the Partner Center menu, select **Billing** .</span></span>

3. <span data-ttu-id="58215-124">Välj fliken för den **återkommande** **tiden** och den valuta som du är intresse rad av.</span><span class="sxs-lookup"><span data-stu-id="58215-124">Select the tab for the **Recurring** and **One-time** and the currency you are interested in.</span></span>

   :::image type="content" source="images/azure/billing3.png" alt-text="fakturerings":::

4. <span data-ttu-id="58215-126">Välj **faktura** eller **avstämnings fil** .</span><span class="sxs-lookup"><span data-stu-id="58215-126">Select **Invoice** or **Reconciliation file** .</span></span>  

   <span data-ttu-id="58215-127">Om du vill visa historiska fakturor och rekognoseringar-filer expanderar du raden för fakturerings historiken nedan.</span><span class="sxs-lookup"><span data-stu-id="58215-127">To view historical invoices and recon files expand the Billing history row below.</span></span>

## <a name="understanding-usage-data"></a><span data-ttu-id="58215-128">Förstå användnings data</span><span class="sxs-lookup"><span data-stu-id="58215-128">Understanding usage data</span></span> 

1. <span data-ttu-id="58215-129">Azure-prenumeration är rot-eller toppnivå behållaren för användning.</span><span class="sxs-lookup"><span data-stu-id="58215-129">Azure plan is the root or top-level container for usage.</span></span> <span data-ttu-id="58215-130">All användning är bunden tillbaka till en enda Azure-plan.</span><span class="sxs-lookup"><span data-stu-id="58215-130">All usage is tied back to a single Azure plan.</span></span>

2. <span data-ttu-id="58215-131">Inom en plan kommer det att finnas en eller flera Azure-prenumerationer.</span><span class="sxs-lookup"><span data-stu-id="58215-131">Within a plan, there will be one or more Azure subscriptions.</span></span> <span data-ttu-id="58215-132">Dessa är behållare som används för resurs hantering och distribution.</span><span class="sxs-lookup"><span data-stu-id="58215-132">These are containers used for resource management and deployment.</span></span> 

3. <span data-ttu-id="58215-133">I en prenumeration lägger resurs grupper till i grupp resurser.</span><span class="sxs-lookup"><span data-stu-id="58215-133">Within a subscription, resource groups add to group resources.</span></span> <span data-ttu-id="58215-134">Varje resurs distribueras till en resurs grupp.</span><span class="sxs-lookup"><span data-stu-id="58215-134">Every resource is deployed to one resource group.</span></span> 

4. <span data-ttu-id="58215-135">Exempel på resurser är virtuella datorer och lagrings konton.</span><span class="sxs-lookup"><span data-stu-id="58215-135">Examples of resources include virtual machines and storage accounts.</span></span> 

5. <span data-ttu-id="58215-136">Antal resurs utsändare: mätare är mätningar av förbrukningen av en resurs och en resurs kan generera användning för flera mätare.</span><span class="sxs-lookup"><span data-stu-id="58215-136">Resource emit meters: Meters are measurements of consumption of a resource, and one resource may emit usage for multiple meters.</span></span> <span data-ttu-id="58215-137">Mätare identifieras av ett ProductId-, SKUId-och AvailabilityId.</span><span class="sxs-lookup"><span data-stu-id="58215-137">Meters are identified by a ProductId, SKUId, and AvailabilityId.</span></span> 

### <a name="hierarchy-of-subscription-resource-groups-and-metering"></a><span data-ttu-id="58215-138">Hierarki för resurs grupper för prenumerationer och mätning</span><span class="sxs-lookup"><span data-stu-id="58215-138">Hierarchy of subscription resource groups and metering</span></span>

<span data-ttu-id="58215-139">**Azure-konto (klient organisation)**</span><span class="sxs-lookup"><span data-stu-id="58215-139">**Azure account (tenant)**</span></span>

- <span data-ttu-id="58215-140">Prenumeration A</span><span class="sxs-lookup"><span data-stu-id="58215-140">Subscription A</span></span>
    - <span data-ttu-id="58215-141">ResourceGroup 1</span><span class="sxs-lookup"><span data-stu-id="58215-141">ResourceGroup 1</span></span>
        - <span data-ttu-id="58215-142">Virtuell dator (resurs)</span><span class="sxs-lookup"><span data-stu-id="58215-142">Virtual machine (resource)</span></span>
            - <span data-ttu-id="58215-143">Beräknings mätare</span><span class="sxs-lookup"><span data-stu-id="58215-143">Compute meter</span></span>
        - <span data-ttu-id="58215-144">Virtuellt nätverk (resurs)</span><span class="sxs-lookup"><span data-stu-id="58215-144">Virtual network (resource)</span></span>
            - <span data-ttu-id="58215-145">Ingen fakturerings mätare</span><span class="sxs-lookup"><span data-stu-id="58215-145">No billing meter</span></span>

    - <span data-ttu-id="58215-146">ResourceGroup 2</span><span class="sxs-lookup"><span data-stu-id="58215-146">ResourceGroup 2</span></span>
        - <span data-ttu-id="58215-147">Virtuell dator (resurs)</span><span class="sxs-lookup"><span data-stu-id="58215-147">Virtual machine (resource)</span></span>
            - <span data-ttu-id="58215-148">Dator mätare</span><span class="sxs-lookup"><span data-stu-id="58215-148">Computer meter</span></span>
        - <span data-ttu-id="58215-149">Premium SSD-hanterad disk (resurs)</span><span class="sxs-lookup"><span data-stu-id="58215-149">Premium SSD-managed disk (resource)</span></span>
            - <span data-ttu-id="58215-150">Lagrings kapacitets mätare</span><span class="sxs-lookup"><span data-stu-id="58215-150">Storage capacity meter</span></span>
            - <span data-ttu-id="58215-151">Lagrings åtgärds mätare</span><span class="sxs-lookup"><span data-stu-id="58215-151">Storage operations meter</span></span>

- <span data-ttu-id="58215-152">Prenumeration B-ResourceGroup 1 – Azure SQL (resurs)-DTU-mätare-VPN Gateway (resurs) – VPN gateway-mätare</span><span class="sxs-lookup"><span data-stu-id="58215-152">Subscription B   -ResourceGroup 1       - Azure SQL (resource)           - DTU meter       - VPN Gateway (resource)           - VPN gateway meter</span></span>

    - <span data-ttu-id="58215-153">ResourceGroup 2</span><span class="sxs-lookup"><span data-stu-id="58215-153">ResourceGroup 2</span></span>
        - <span data-ttu-id="58215-154">Virtual Network gränssnitt (resurs)</span><span class="sxs-lookup"><span data-stu-id="58215-154">Virtual Network Interface (resource)</span></span>
            - <span data-ttu-id="58215-155">Ingen fakturerings mätare</span><span class="sxs-lookup"><span data-stu-id="58215-155">No billing meter</span></span>

## <a name="read-the-invoice"></a><span data-ttu-id="58215-156">Läs fakturan</span><span class="sxs-lookup"><span data-stu-id="58215-156">Read the invoice</span></span>

1. <span data-ttu-id="58215-157">Fakturan kommer att vara tillgänglig senast den åttonde dagen i varje månad.</span><span class="sxs-lookup"><span data-stu-id="58215-157">Invoice will be available no later than the eighth of each month.</span></span>

2. <span data-ttu-id="58215-158">Partner har 60 dagar på sig att betala.</span><span class="sxs-lookup"><span data-stu-id="58215-158">Partners have 60 days to remit payment.</span></span>

3. <span data-ttu-id="58215-159">Fakturerings perioden kommer att avse en viss kalender månad, till exempel 10/1-10/31.</span><span class="sxs-lookup"><span data-stu-id="58215-159">The billing period will cover a given calendar month, for example, 10/1-10/31.</span></span>

4. <span data-ttu-id="58215-160">Avgifterna är netto av justeringar (beloppet är netto av "partner intjänad kredit för tjänster som hanteras").</span><span class="sxs-lookup"><span data-stu-id="58215-160">Charges are net of adjustments (amount is net of “Partner earned credit for services managed").</span></span>

5. <span data-ttu-id="58215-161">Granska fakturan rekognoseringar-filen och den dagliga, beräknade användnings filen för ytterligare fakturerings information.</span><span class="sxs-lookup"><span data-stu-id="58215-161">Review the invoice recon file and daily rated usage file for additional billing details.</span></span>

   :::image type="content" source="images/azure/invoice1.png" alt-text="Voice":::

## <a name="read-the-invoice-reconciliation-file"></a><span data-ttu-id="58215-163">Läs faktura avstämnings filen</span><span class="sxs-lookup"><span data-stu-id="58215-163">Read the invoice reconciliation file</span></span>

1. <span data-ttu-id="58215-164">Varje kombination av Azure-plan och-mätare kan ha upp till två fakturerings rader i rekognoseringar-filen.</span><span class="sxs-lookup"><span data-stu-id="58215-164">Each Azure plan and meter combination may have up to two billing lines on the recon file.</span></span>

2. <span data-ttu-id="58215-165">Om mätaren är kvalificerad för någon typ av rabatt eller kredit (till exempel rabatterade rabatter eller partner intjänade kredit för tjänster som hanteras) under hela kalender månaden, kommer rekognoseringar-filen bara att innehålla en fakturerings rad.</span><span class="sxs-lookup"><span data-stu-id="58215-165">If the meter qualified for any type of discount or credit (such as tiered discounts or the Partner earned credit for services managed) throughout the entire calendar month, then the recon file will only contain one billing line.</span></span> <span data-ttu-id="58215-166">Kolumnen **PriceAdjusmentDescription** kommer att referera till rabatten eller den intjänade krediten.</span><span class="sxs-lookup"><span data-stu-id="58215-166">The column **PriceAdjusmentDescription** will reference the discount or earned credit.</span></span>

3. <span data-ttu-id="58215-167">Om det inte finns några resurser för en viss mätare som är kvalificerad för rabatt eller partner intjänad kredit, kommer rekognoseringar-filen bara innehålla en fakturerings rad och det effektiva enhets priset blir åter försäljnings priset (vilket är enhets priset).</span><span class="sxs-lookup"><span data-stu-id="58215-167">If there are no resources for a particular meter that qualified for discount or partner earned credit, then the recon file will only contain one billing line and the effective unit price will be the retail price (which is the unit price).</span></span>

4. <span data-ttu-id="58215-168">Om mätaren eller eventuella resurser som avger denna mätare, kvalificerat för **partner intjänad kredit för tjänster som hanteras** i en del av månaden, innehåller rekognoseringar-filen två fakturerings rader.</span><span class="sxs-lookup"><span data-stu-id="58215-168">If the meter, or any resources emitting that meter, qualified for **Partner earned credit for services managed** for a part of the month, the recon file will contain two billing lines.</span></span> <span data-ttu-id="58215-169">En rad representerar de dagar som mätaren kvalificeras och den andra raden visar de dagar som mätaren inte kvalificerade sig.</span><span class="sxs-lookup"><span data-stu-id="58215-169">One line will represent the days the meter qualified and the second line will represent the days the meter did not qualify.</span></span>

## <a name="read-the-daily-usage-file"></a><span data-ttu-id="58215-170">Läs den dagliga användnings filen</span><span class="sxs-lookup"><span data-stu-id="58215-170">Read the daily usage file</span></span>

- <span data-ttu-id="58215-171">Prenumerations mätare enligt en Azure-plan klassificeras och ackumuleras per dag.</span><span class="sxs-lookup"><span data-stu-id="58215-171">Subscription meters under an Azure plan are rated, and are cumulated, on a daily basis.</span></span>

- <span data-ttu-id="58215-172">**Partner intjänad kredit för tjänster som hanteras** bestäms och tillämpas dagligen.</span><span class="sxs-lookup"><span data-stu-id="58215-172">**Partner earned credit for services managed** is determined and applied on a daily basis.</span></span>

- <span data-ttu-id="58215-173">Varje prenumerations mätare har en rad för varje dag i månaden där förbrukningen pågick.</span><span class="sxs-lookup"><span data-stu-id="58215-173">Every subscription meter will have a row for every day of the month where there was consumption.</span></span>

- <span data-ttu-id="58215-174">I exemplet nedan:</span><span class="sxs-lookup"><span data-stu-id="58215-174">In the example below:</span></span>

  - <span data-ttu-id="58215-175">Mätar kvalificerare för **partner intjänade krediter för tjänster som hanteras** från 7/1-7/3 (Observera att det effektiva enhets priset är i detalj handels pris minus partner intjänande</span><span class="sxs-lookup"><span data-stu-id="58215-175">Meter qualified for **Partner earned credit for services managed** from 7/1 - 7/3 (note the effective unit price is retail price less partner earned credit.</span></span>

  - <span data-ttu-id="58215-176">Mätaren var inte berättigad till **partner intjänad kredit för tjänster som hanteras** från 7/4-7/7 (Observera att det effektiva enhets priset är försäljnings pris).</span><span class="sxs-lookup"><span data-stu-id="58215-176">Meter didn't qualify for **Partner earned credit for services managed** from 7/4 - 7/7 (note the effective unit price is retail price).</span></span>

  - <span data-ttu-id="58215-177">Mätning som är kvalificerad för **partner intjänad kredit för tjänster som hanteras** från 7/8-7/31 (Observera att det effektiva enhets priset är åter försäljnings pris minus partner intjänad kredit)</span><span class="sxs-lookup"><span data-stu-id="58215-177">Meter qualified for **Partner earned credit for services managed** from 7/8 - 7/31 (note the effective unit price is retail price less partner earned credit).</span></span>

   :::image type="content" source="images/azure/pecfinal.png" alt-text="recon2":::

## <a name="invoice-in-customer-currency"></a><span data-ttu-id="58215-179">Faktura i kund valuta</span><span class="sxs-lookup"><span data-stu-id="58215-179">Invoice in customer currency</span></span>

<span data-ttu-id="58215-180">Azure-tjänster via en Azure-prenumeration priss ätts i USD och faktureras i kund landets tilldelade valuta.</span><span class="sxs-lookup"><span data-stu-id="58215-180">Azure services through an Azure plan will be priced in USD and billed in the customer country assigned currency.</span></span> <span data-ttu-id="58215-181">Om fakturerings valutan är icke-USD visas den utländska växelkursen (FX) som används på den sista sidan i fakturan.</span><span class="sxs-lookup"><span data-stu-id="58215-181">If the billing currency is non-USD, then the Foreign exchange (FX) rate used will be shown on the last page of the invoice.</span></span> <span data-ttu-id="58215-182">FX-priser fastställs varje månad och tillämpas på följande faktura.</span><span class="sxs-lookup"><span data-stu-id="58215-182">FX rates are determined monthly and applied to the following invoice.</span></span> <span data-ttu-id="58215-183">En fullständig lista över lands valutor finns i den [nya Commerces tillgänglighet för land och kund valuta mat ris](https://go.microsoft.com/fwlink/?linkid=2112354).</span><span class="sxs-lookup"><span data-stu-id="58215-183">For a full list of country currencies, please view the [new commerce offers country availability and customer currency matrix](https://go.microsoft.com/fwlink/?linkid=2112354).</span></span>

<span data-ttu-id="58215-184">Microsoft använder Thomson-Reuters för att fastställa de FX-priser som används för att fastställa pris valuta för konvertering av fakturerings valuta.</span><span class="sxs-lookup"><span data-stu-id="58215-184">Microsoft will use Thomson Reuters to determine the FX rates used to determine pricing currency to billing currency conversion.</span></span> <span data-ttu-id="58215-185">FX-priserna kommer att uppdateras och vara tillgängliga på dagen före den första av den månad som de gäller.</span><span class="sxs-lookup"><span data-stu-id="58215-185">The FX rates will be refreshed and available on the day before the first of the month for which they apply.</span></span>

<span data-ttu-id="58215-186">**Exempel** : användnings debitering för service perioden 1 augusti 31 debiteras med den FX-taxa som publicerades den 31 juli.</span><span class="sxs-lookup"><span data-stu-id="58215-186">**Example** :  Usage charges for the service period August 1 - August 31 will be billed using the FX rate published on July 31.</span></span> <span data-ttu-id="58215-187">De här avgifterna visas på fakturan i september och FX-priset anges på den sista sidan i fakturan.</span><span class="sxs-lookup"><span data-stu-id="58215-187">These charges will appear on the September invoice and the FX rate will be noted on the last page of the invoice.</span></span>

## <a name="azure-reservations"></a><span data-ttu-id="58215-188">Azure-reservationer</span><span class="sxs-lookup"><span data-stu-id="58215-188">Azure reservations</span></span>


<span data-ttu-id="58215-189">Om du köper [Azure-reservationer](azure-reservations.md) via en Azure-prenumeration kan du välja antingen en gång eller månatlig fakturering.</span><span class="sxs-lookup"><span data-stu-id="58215-189">If purchasing [Azure reservations](azure-reservations.md) through an Azure plan, you can choose either one-time or monthly billing.</span></span>


## <a name="azure-spending"></a><span data-ttu-id="58215-190">Utgift i Azure</span><span class="sxs-lookup"><span data-stu-id="58215-190">Azure spending</span></span>

<span data-ttu-id="58215-191">Den befintliga Azure-utgifts upplevelsen uppdateras för att stödja den nya faktureringen av Azure-plan i Partner Center.</span><span class="sxs-lookup"><span data-stu-id="58215-191">The existing Azure spending experience is updated to support the new Azure plan billing in Partner Center.</span></span> <span data-ttu-id="58215-192">Detta gör att partner kan:</span><span class="sxs-lookup"><span data-stu-id="58215-192">This enables partners to:</span></span>

- <span data-ttu-id="58215-193">Visa, hantera och ta emot aviseringar för budget uppsättning på en kund nivå</span><span class="sxs-lookup"><span data-stu-id="58215-193">View, manage, and receive alerts for budget set at a customer level</span></span> 

- <span data-ttu-id="58215-194">Visa totala uppskattade utgifter i en Azure-plan (uppdelad efter resurs och mätar nivå)</span><span class="sxs-lookup"><span data-stu-id="58215-194">View total estimated spending on an Azure plan (broken down by resource and meter level)</span></span>

<span data-ttu-id="58215-195">Eftersom fakturerings modellen för Azure-tjänster via en Azure-plan är efter löne förbrukning, för att undvika en större faktura än förväntat, kan partner tillämpa en månads budget och spåra procent andelen av användningen.</span><span class="sxs-lookup"><span data-stu-id="58215-195">Because the billing model for Azure services through an Azure plan is post-pay consumption, to avoid a bigger bill than anticipated, partners can apply a monthly budget and track the percentage of usage.</span></span> <span data-ttu-id="58215-196">En budget kan tillämpas på en kund eller flera kunder på en och samma tidpunkt.</span><span class="sxs-lookup"><span data-stu-id="58215-196">A budget can be applied to one customer or multiple customers at one time.</span></span> 

:::image type="content" source="images/azure/azurespend.png" alt-text="Utgift i Azure":::

## <a name="next-steps"></a><span data-ttu-id="58215-198">Nästa steg</span><span class="sxs-lookup"><span data-stu-id="58215-198">Next steps</span></span>

- <span data-ttu-id="58215-199">Se hur partnern för intjänad kredit (PEC) beräknas.</span><span class="sxs-lookup"><span data-stu-id="58215-199">See how the partner earned credit (PEC) is calculated.</span></span> <span data-ttu-id="58215-200">Logga in på Partner Center- [instrumentpanelen](https://partner.microsoft.com/dashboard/) och leta upp pris listan som är tillgänglig.</span><span class="sxs-lookup"><span data-stu-id="58215-200">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard/) and locate the price list available.</span></span>

- <span data-ttu-id="58215-201">Lär dig mer om [att köpa Azure-prenumerationen](purchase-azure-plan.md)</span><span class="sxs-lookup"><span data-stu-id="58215-201">Learn about [purchasing the Azure plan](purchase-azure-plan.md)</span></span>

- <span data-ttu-id="58215-202">Se [pris listan för den nya Commerce-upplevelsen i CSP](azure-plan-price-list.md)</span><span class="sxs-lookup"><span data-stu-id="58215-202">See the [price list for the new commerce experience in CSP](azure-plan-price-list.md)</span></span>
