---
title: Fakturering av Azure-plan – faktura & rekognoseringar-filer
ms.topic: article
ms.date: 01/20/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Lär dig hur du får åtkomst till och förstår den faktura och avstämnings fil struktur som är relaterad till faktureringen för Azure-prenumerationen.
author: khpavan
ms.author: sakhanda
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 819f90ca9a8467de4a8001a1b10f8409d3fb1b81
ms.sourcegitcommit: fc1f9cb5a542bdc92d62d2a7e1ab2f4e69903e49
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 01/28/2021
ms.locfileid: "98925006"
---
# <a name="new-commerce-experience-in-csp---azure-billing"></a><span data-ttu-id="ecf4d-103">Ny handelsupplevelse i CSP – Azure-fakturering</span><span class="sxs-lookup"><span data-stu-id="ecf4d-103">New commerce experience in CSP - Azure billing</span></span> 

<span data-ttu-id="ecf4d-104">**Lämpliga roller**</span><span class="sxs-lookup"><span data-stu-id="ecf4d-104">**Appropriate roles**</span></span>

- <span data-ttu-id="ecf4d-105">Administratörs agent</span><span class="sxs-lookup"><span data-stu-id="ecf4d-105">Admin agent</span></span>
- <span data-ttu-id="ecf4d-106">Faktureringsadministratör</span><span class="sxs-lookup"><span data-stu-id="ecf4d-106">Billing admin</span></span>
- <span data-ttu-id="ecf4d-107">Global administratör</span><span class="sxs-lookup"><span data-stu-id="ecf4d-107">Global admin</span></span>

<span data-ttu-id="ecf4d-108">Den här artikeln förklarar hur du får åtkomst till och förstår strukturen på fakturan och avstämnings filen som är relaterad till faktureringen för Azure-prenumerationen.</span><span class="sxs-lookup"><span data-stu-id="ecf4d-108">This article explains how to access and understand the invoice and reconciliation file structure related to billing for the Azure plan.</span></span> <span data-ttu-id="ecf4d-109">Faktureringen enligt Azure-planen är en förenklad fakturerings upplevelse med ett justerat fakturerings datum och en månads-baserad fakturerings period.</span><span class="sxs-lookup"><span data-stu-id="ecf4d-109">Billing under the Azure plan is a simplified billing experience using an aligned single billing date and calendar month-based billing period.</span></span>

## <a name="summary-of-billing-essentials"></a><span data-ttu-id="ecf4d-110">Sammanfattning av fakturerings grunderna</span><span class="sxs-lookup"><span data-stu-id="ecf4d-110">Summary of billing essentials</span></span>

- <span data-ttu-id="ecf4d-111">**Faktura datum**: faktura-och avstämnings fil kommer att finnas i Partner Center Dashboard/API med 8 (midnatt UTC).</span><span class="sxs-lookup"><span data-stu-id="ecf4d-111">**Invoice date**: Invoice and reconciliation file will be available in the Partner Center dashboard/API by the 8th (midnight UTC).</span></span>

- <span data-ttu-id="ecf4d-112">**Fakturerings period för faktura**: faktura fakturerings perioden justeras till kalender månaden, till exempel 10/1-10/31, 11/1-11/30.</span><span class="sxs-lookup"><span data-stu-id="ecf4d-112">**Invoice billing period**: The invoice billing period is aligned to the calendar month, for example,  10/1-10/31, 11/1-11/30.</span></span>

- <span data-ttu-id="ecf4d-113">**Debitering av service perioder**: avgifterna justeras till kalender månaden.</span><span class="sxs-lookup"><span data-stu-id="ecf4d-113">**Charge service periods**: Charges will align to the calendar month.</span></span> <span data-ttu-id="ecf4d-114">Om den fakturerade partnern till exempel lägger till Azure-tjänster via en Azure-plan på 10/15 och kunden börjar förbrukningen av Azure-tjänster på 10/15, får fakturerad partner faktura-rekognoseringar på 11/8 för kund förbrukning för service perioden 10/15-10/31.</span><span class="sxs-lookup"><span data-stu-id="ecf4d-114">For example, if billed partner adds Azure services through an Azure plan on 10/15 and the customer begins consumption of Azure services on 10/15, then billed partner will receive invoice/recon on 11/8 for customer consumption for the service period 10/15 - 10/31.</span></span> <span data-ttu-id="ecf4d-115">Nästa månads faktura som ska genereras på 12/8 innehåller alla avgifter för service perioden 11/1-11/31.</span><span class="sxs-lookup"><span data-stu-id="ecf4d-115">The next month's invoice that is going to be generated on 12/8 contains all the charges for the service period 11/1- 11/31.</span></span>

- <span data-ttu-id="ecf4d-116">**Faktura betalnings villkor**: net 60 dagar.</span><span class="sxs-lookup"><span data-stu-id="ecf4d-116">**Invoice payment term**: Net 60 days.</span></span>

- <span data-ttu-id="ecf4d-117">**Faktura valuta**: från januari 28 2021, partners i EU/Efta-och Storbritannien-regionen som har nya kunder och befintliga CSP-kunder som köper nya Commerce-erbjudanden för första gången vars innehavare skapades före 11 maj 2020, debiteras för dessa inköp i partner platsens valuta.</span><span class="sxs-lookup"><span data-stu-id="ecf4d-117">**Invoice currency**: Starting January 28th 2021, partners in the EU/EFTA and UK region who have new customers and existing CSP customers purchasing new commerce offers for the first time whose tenants were created prior to 11 May 2020, will be billed for those purchases in partner location currency.</span></span> <span data-ttu-id="ecf4d-118">Partner som finns utanför EU/EFTA-och Storbritannien-regionen fortsätter att faktureras i partner platsens valuta.</span><span class="sxs-lookup"><span data-stu-id="ecf4d-118">Partners located outside of the EU/EFTA and UK region will continue to be billed in partner location currency.</span></span>

- <span data-ttu-id="ecf4d-119">**Partner incitament**: betalda 45 dagar från slutet av faktura månaden.</span><span class="sxs-lookup"><span data-stu-id="ecf4d-119">**Partner incentives**: Paid 45 days from the end of the invoice month.</span></span>

## <a name="access-your-invoices-and-reconciliation-files"></a><span data-ttu-id="ecf4d-120">Få åtkomst till dina fakturor och avstämnings filer</span><span class="sxs-lookup"><span data-stu-id="ecf4d-120">Access your invoices and reconciliation files</span></span>

<span data-ttu-id="ecf4d-121">Den globala administratörs-eller fakturerings administratören för ditt företag får ett e-postmeddelande när en faktura är klar att visa.</span><span class="sxs-lookup"><span data-stu-id="ecf4d-121">The global admin or billing admin for your company will receive an email when an invoice is ready to view.</span></span>

<span data-ttu-id="ecf4d-122">För att få åtkomst till fakturan och avstämnings filen:</span><span class="sxs-lookup"><span data-stu-id="ecf4d-122">To access the invoice and reconciliation file:</span></span>

1. <span data-ttu-id="ecf4d-123">Logga in i Partnercenter och gå till [instrumentpanelen](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="ecf4d-123">Sign in to the Partner Center [dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="ecf4d-124">Från menyn Partner Center väljer du **fakturering**.</span><span class="sxs-lookup"><span data-stu-id="ecf4d-124">From the Partner Center menu, select **Billing**.</span></span>

3. <span data-ttu-id="ecf4d-125">Välj fliken för den **återkommande** **tiden** och den valuta som du är intresse rad av.</span><span class="sxs-lookup"><span data-stu-id="ecf4d-125">Select the tab for the **Recurring** and **One-time** and the currency you are interested in.</span></span>

   :::image type="content" source="images/azure/billing3.png" alt-text="fakturerings":::

4. <span data-ttu-id="ecf4d-127">Välj **faktura** eller **avstämnings fil**.</span><span class="sxs-lookup"><span data-stu-id="ecf4d-127">Select **Invoice** or **Reconciliation file**.</span></span>  

   <span data-ttu-id="ecf4d-128">Om du vill visa historiska fakturor och rekognoseringar-filer expanderar du raden för fakturerings historiken nedan.</span><span class="sxs-lookup"><span data-stu-id="ecf4d-128">To view historical invoices and recon files expand the Billing history row below.</span></span>

## <a name="understanding-usage-data"></a><span data-ttu-id="ecf4d-129">Förstå användnings data</span><span class="sxs-lookup"><span data-stu-id="ecf4d-129">Understanding usage data</span></span> 

1. <span data-ttu-id="ecf4d-130">Azure-prenumeration är rot-eller toppnivå behållaren för användning.</span><span class="sxs-lookup"><span data-stu-id="ecf4d-130">Azure plan is the root or top-level container for usage.</span></span> <span data-ttu-id="ecf4d-131">All användning är bunden tillbaka till en enda Azure-plan.</span><span class="sxs-lookup"><span data-stu-id="ecf4d-131">All usage is tied back to a single Azure plan.</span></span>

2. <span data-ttu-id="ecf4d-132">Inom en plan kommer det att finnas en eller flera Azure-prenumerationer.</span><span class="sxs-lookup"><span data-stu-id="ecf4d-132">Within a plan, there will be one or more Azure subscriptions.</span></span> <span data-ttu-id="ecf4d-133">Dessa är behållare som används för resurs hantering och distribution.</span><span class="sxs-lookup"><span data-stu-id="ecf4d-133">These are containers used for resource management and deployment.</span></span> 

3. <span data-ttu-id="ecf4d-134">I en prenumeration lägger resurs grupper till i grupp resurser.</span><span class="sxs-lookup"><span data-stu-id="ecf4d-134">Within a subscription, resource groups add to group resources.</span></span> <span data-ttu-id="ecf4d-135">Varje resurs distribueras till en resurs grupp.</span><span class="sxs-lookup"><span data-stu-id="ecf4d-135">Every resource is deployed to one resource group.</span></span> 

4. <span data-ttu-id="ecf4d-136">Exempel på resurser är virtuella datorer och lagrings konton.</span><span class="sxs-lookup"><span data-stu-id="ecf4d-136">Examples of resources include virtual machines and storage accounts.</span></span> 

5. <span data-ttu-id="ecf4d-137">Antal resurs utsändare: mätare är mätningar av förbrukningen av en resurs och en resurs kan generera användning för flera mätare.</span><span class="sxs-lookup"><span data-stu-id="ecf4d-137">Resource emit meters: Meters are measurements of consumption of a resource, and one resource may emit usage for multiple meters.</span></span> <span data-ttu-id="ecf4d-138">Mätare identifieras av ett ProductId-, SKUId-och AvailabilityId.</span><span class="sxs-lookup"><span data-stu-id="ecf4d-138">Meters are identified by a ProductId, SKUId, and AvailabilityId.</span></span> 

### <a name="hierarchy-of-subscription-resource-groups-and-metering"></a><span data-ttu-id="ecf4d-139">Hierarki för resurs grupper för prenumerationer och mätning</span><span class="sxs-lookup"><span data-stu-id="ecf4d-139">Hierarchy of subscription resource groups and metering</span></span>

<span data-ttu-id="ecf4d-140">**Azure-konto (klient organisation)**</span><span class="sxs-lookup"><span data-stu-id="ecf4d-140">**Azure account (tenant)**</span></span>

- <span data-ttu-id="ecf4d-141">Prenumeration A</span><span class="sxs-lookup"><span data-stu-id="ecf4d-141">Subscription A</span></span>
    - <span data-ttu-id="ecf4d-142">ResourceGroup 1</span><span class="sxs-lookup"><span data-stu-id="ecf4d-142">ResourceGroup 1</span></span>
        - <span data-ttu-id="ecf4d-143">Virtuell dator (resurs)</span><span class="sxs-lookup"><span data-stu-id="ecf4d-143">Virtual machine (resource)</span></span>
            - <span data-ttu-id="ecf4d-144">Beräknings mätare</span><span class="sxs-lookup"><span data-stu-id="ecf4d-144">Compute meter</span></span>
        - <span data-ttu-id="ecf4d-145">Virtuellt nätverk (resurs)</span><span class="sxs-lookup"><span data-stu-id="ecf4d-145">Virtual network (resource)</span></span>
            - <span data-ttu-id="ecf4d-146">Ingen fakturerings mätare</span><span class="sxs-lookup"><span data-stu-id="ecf4d-146">No billing meter</span></span>

    - <span data-ttu-id="ecf4d-147">ResourceGroup 2</span><span class="sxs-lookup"><span data-stu-id="ecf4d-147">ResourceGroup 2</span></span>
        - <span data-ttu-id="ecf4d-148">Virtuell dator (resurs)</span><span class="sxs-lookup"><span data-stu-id="ecf4d-148">Virtual machine (resource)</span></span>
            - <span data-ttu-id="ecf4d-149">Dator mätare</span><span class="sxs-lookup"><span data-stu-id="ecf4d-149">Computer meter</span></span>
        - <span data-ttu-id="ecf4d-150">Premium SSD-hanterad disk (resurs)</span><span class="sxs-lookup"><span data-stu-id="ecf4d-150">Premium SSD-managed disk (resource)</span></span>
            - <span data-ttu-id="ecf4d-151">Lagrings kapacitets mätare</span><span class="sxs-lookup"><span data-stu-id="ecf4d-151">Storage capacity meter</span></span>
            - <span data-ttu-id="ecf4d-152">Lagrings åtgärds mätare</span><span class="sxs-lookup"><span data-stu-id="ecf4d-152">Storage operations meter</span></span>

- <span data-ttu-id="ecf4d-153">Prenumeration B-ResourceGroup 1 – Azure SQL (resurs)-DTU-mätare-VPN Gateway (resurs) – VPN gateway-mätare</span><span class="sxs-lookup"><span data-stu-id="ecf4d-153">Subscription B   -ResourceGroup 1       - Azure SQL (resource)           - DTU meter       - VPN Gateway (resource)           - VPN gateway meter</span></span>

    - <span data-ttu-id="ecf4d-154">ResourceGroup 2</span><span class="sxs-lookup"><span data-stu-id="ecf4d-154">ResourceGroup 2</span></span>
        - <span data-ttu-id="ecf4d-155">Virtual Network gränssnitt (resurs)</span><span class="sxs-lookup"><span data-stu-id="ecf4d-155">Virtual Network Interface (resource)</span></span>
            - <span data-ttu-id="ecf4d-156">Ingen fakturerings mätare</span><span class="sxs-lookup"><span data-stu-id="ecf4d-156">No billing meter</span></span>

## <a name="read-the-invoice"></a><span data-ttu-id="ecf4d-157">Läs fakturan</span><span class="sxs-lookup"><span data-stu-id="ecf4d-157">Read the invoice</span></span>

1. <span data-ttu-id="ecf4d-158">Fakturan kommer att vara tillgänglig senast den åttonde dagen i varje månad.</span><span class="sxs-lookup"><span data-stu-id="ecf4d-158">Invoice will be available no later than the eighth of each month.</span></span>

2. <span data-ttu-id="ecf4d-159">Partner har 60 dagar på sig att betala.</span><span class="sxs-lookup"><span data-stu-id="ecf4d-159">Partners have 60 days to remit payment.</span></span>

3. <span data-ttu-id="ecf4d-160">Fakturerings perioden kommer att avse en viss kalender månad, till exempel 10/1-10/31.</span><span class="sxs-lookup"><span data-stu-id="ecf4d-160">The billing period will cover a given calendar month, for example, 10/1-10/31.</span></span>

4. <span data-ttu-id="ecf4d-161">Avgifterna är netto av justeringar (beloppet är netto av "partner intjänad kredit för tjänster som hanteras").</span><span class="sxs-lookup"><span data-stu-id="ecf4d-161">Charges are net of adjustments (amount is net of “Partner earned credit for services managed").</span></span>

5. <span data-ttu-id="ecf4d-162">Granska fakturan rekognoseringar-filen och den dagliga, beräknade användnings filen för ytterligare fakturerings information.</span><span class="sxs-lookup"><span data-stu-id="ecf4d-162">Review the invoice recon file and daily rated usage file for additional billing details.</span></span>

   :::image type="content" source="images/azure/invoice1.png" alt-text="Voice":::

## <a name="read-the-invoice-reconciliation-file"></a><span data-ttu-id="ecf4d-164">Läs faktura avstämnings filen</span><span class="sxs-lookup"><span data-stu-id="ecf4d-164">Read the invoice reconciliation file</span></span>

1. <span data-ttu-id="ecf4d-165">Varje kombination av Azure-plan och-mätare kan ha upp till två fakturerings rader i rekognoseringar-filen.</span><span class="sxs-lookup"><span data-stu-id="ecf4d-165">Each Azure plan and meter combination may have up to two billing lines on the recon file.</span></span>

2. <span data-ttu-id="ecf4d-166">Om mätaren är kvalificerad för någon typ av rabatt eller kredit (till exempel rabatterade rabatter eller partner intjänade kredit för tjänster som hanteras) under hela kalender månaden, kommer rekognoseringar-filen bara att innehålla en fakturerings rad.</span><span class="sxs-lookup"><span data-stu-id="ecf4d-166">If the meter qualified for any type of discount or credit (such as tiered discounts or the Partner earned credit for services managed) throughout the entire calendar month, then the recon file will only contain one billing line.</span></span> <span data-ttu-id="ecf4d-167">Kolumnen **PriceAdjusmentDescription** kommer att referera till rabatten eller den intjänade krediten.</span><span class="sxs-lookup"><span data-stu-id="ecf4d-167">The column **PriceAdjusmentDescription** will reference the discount or earned credit.</span></span>

3. <span data-ttu-id="ecf4d-168">Om det inte finns några resurser för en viss mätare som är kvalificerad för rabatt eller partner intjänad kredit, kommer rekognoseringar-filen bara innehålla en fakturerings rad och det effektiva enhets priset blir åter försäljnings priset (vilket är enhets priset).</span><span class="sxs-lookup"><span data-stu-id="ecf4d-168">If there are no resources for a particular meter that qualified for discount or partner earned credit, then the recon file will only contain one billing line and the effective unit price will be the retail price (which is the unit price).</span></span>

4. <span data-ttu-id="ecf4d-169">Om mätaren eller eventuella resurser som avger denna mätare, kvalificerat för **partner intjänad kredit för tjänster som hanteras** i en del av månaden, innehåller rekognoseringar-filen två fakturerings rader.</span><span class="sxs-lookup"><span data-stu-id="ecf4d-169">If the meter, or any resources emitting that meter, qualified for **Partner earned credit for services managed** for a part of the month, the recon file will contain two billing lines.</span></span> <span data-ttu-id="ecf4d-170">En rad representerar de dagar som mätaren kvalificeras och den andra raden visar de dagar som mätaren inte kvalificerade sig.</span><span class="sxs-lookup"><span data-stu-id="ecf4d-170">One line will represent the days the meter qualified and the second line will represent the days the meter did not qualify.</span></span>

## <a name="read-the-daily-usage-file"></a><span data-ttu-id="ecf4d-171">Läs den dagliga användnings filen</span><span class="sxs-lookup"><span data-stu-id="ecf4d-171">Read the daily usage file</span></span>

- <span data-ttu-id="ecf4d-172">Prenumerations mätare enligt en Azure-plan klassificeras och ackumuleras per dag.</span><span class="sxs-lookup"><span data-stu-id="ecf4d-172">Subscription meters under an Azure plan are rated, and are cumulated, on a daily basis.</span></span>

- <span data-ttu-id="ecf4d-173">**Partner intjänad kredit för tjänster som hanteras** bestäms och tillämpas dagligen.</span><span class="sxs-lookup"><span data-stu-id="ecf4d-173">**Partner earned credit for services managed** is determined and applied on a daily basis.</span></span>

- <span data-ttu-id="ecf4d-174">Varje prenumerations mätare har en rad för varje dag i månaden där förbrukningen pågick.</span><span class="sxs-lookup"><span data-stu-id="ecf4d-174">Every subscription meter will have a row for every day of the month where there was consumption.</span></span>

- <span data-ttu-id="ecf4d-175">I exemplet nedan:</span><span class="sxs-lookup"><span data-stu-id="ecf4d-175">In the example below:</span></span>

  - <span data-ttu-id="ecf4d-176">Mätar kvalificerare för **partner intjänade krediter för tjänster som hanteras** från 7/1-7/3 (Observera att det effektiva enhets priset är i detalj handels pris minus partner intjänande</span><span class="sxs-lookup"><span data-stu-id="ecf4d-176">Meter qualified for **Partner earned credit for services managed** from 7/1 - 7/3 (note the effective unit price is retail price less partner earned credit.</span></span>

  - <span data-ttu-id="ecf4d-177">Mätaren var inte berättigad till **partner intjänad kredit för tjänster som hanteras** från 7/4-7/7 (Observera att det effektiva enhets priset är försäljnings pris).</span><span class="sxs-lookup"><span data-stu-id="ecf4d-177">Meter didn't qualify for **Partner earned credit for services managed** from 7/4 - 7/7 (note the effective unit price is retail price).</span></span>

  - <span data-ttu-id="ecf4d-178">Mätning som är kvalificerad för **partner intjänad kredit för tjänster som hanteras** från 7/8-7/31 (Observera att det effektiva enhets priset är åter försäljnings pris minus partner intjänad kredit)</span><span class="sxs-lookup"><span data-stu-id="ecf4d-178">Meter qualified for **Partner earned credit for services managed** from 7/8 - 7/31 (note the effective unit price is retail price less partner earned credit).</span></span>

   :::image type="content" source="images/azure/pecfinal.png" alt-text="recon2":::

## <a name="invoice-in-customer-currency"></a><span data-ttu-id="ecf4d-180">Faktura i kund valuta</span><span class="sxs-lookup"><span data-stu-id="ecf4d-180">Invoice in customer currency</span></span>

<span data-ttu-id="ecf4d-181">Azure-tjänster via en Azure-prenumeration priss ätts i USD och faktureras i kund landets tilldelade valuta.</span><span class="sxs-lookup"><span data-stu-id="ecf4d-181">Azure services through an Azure plan will be priced in USD and billed in the customer country assigned currency.</span></span> <span data-ttu-id="ecf4d-182">Om fakturerings valutan är icke-USD visas den utländska växelkursen (FX) som används på den sista sidan i fakturan.</span><span class="sxs-lookup"><span data-stu-id="ecf4d-182">If the billing currency is non-USD, then the Foreign exchange (FX) rate used will be shown on the last page of the invoice.</span></span> <span data-ttu-id="ecf4d-183">FX-priser fastställs varje månad och tillämpas på följande faktura.</span><span class="sxs-lookup"><span data-stu-id="ecf4d-183">FX rates are determined monthly and applied to the following invoice.</span></span> <span data-ttu-id="ecf4d-184">En fullständig lista över lands valutor finns i den [nya Commerces tillgänglighet för land och kund valuta mat ris](https://go.microsoft.com/fwlink/?linkid=2112354).</span><span class="sxs-lookup"><span data-stu-id="ecf4d-184">For a full list of country currencies, please view the [new commerce offers country availability and customer currency matrix](https://go.microsoft.com/fwlink/?linkid=2112354).</span></span>

<span data-ttu-id="ecf4d-185">Microsoft följer Londons aktie kurs för konvertering.</span><span class="sxs-lookup"><span data-stu-id="ecf4d-185">Microsoft follows the London Stock Exchange for conversion.</span></span> <span data-ttu-id="ecf4d-186">Vi använder växelkursen, som är lika med den växelkurs som inhämtats den senaste sekunden i månaden för den senaste arbets dagen i månaden för Londons fondbörs.</span><span class="sxs-lookup"><span data-stu-id="ecf4d-186">We use the exchange rate, which is equal to the exchange rate captured on the last second of the last business day of the month on the London Stock Exchange.</span></span> <span data-ttu-id="ecf4d-187">FX-priserna kommer att uppdateras och vara tillgängliga på dagen före den första av den månad som de gäller.</span><span class="sxs-lookup"><span data-stu-id="ecf4d-187">The FX rates will be refreshed and available on the day before the first of the month for which they apply.</span></span>

## <a name="azure-reservations"></a><span data-ttu-id="ecf4d-188">Azure-reservationer</span><span class="sxs-lookup"><span data-stu-id="ecf4d-188">Azure reservations</span></span>


<span data-ttu-id="ecf4d-189">Om du köper [Azure-reservationer](azure-reservations.md) via en Azure-prenumeration kan du välja antingen en gång eller månatlig fakturering.</span><span class="sxs-lookup"><span data-stu-id="ecf4d-189">If purchasing [Azure reservations](azure-reservations.md) through an Azure plan, you can choose either one-time or monthly billing.</span></span>


## <a name="azure-spending"></a><span data-ttu-id="ecf4d-190">Utgift i Azure</span><span class="sxs-lookup"><span data-stu-id="ecf4d-190">Azure spending</span></span>

<span data-ttu-id="ecf4d-191">Den befintliga Azure-utgifts upplevelsen uppdateras för att stödja den nya faktureringen av Azure-plan i Partner Center.</span><span class="sxs-lookup"><span data-stu-id="ecf4d-191">The existing Azure spending experience is updated to support the new Azure plan billing in Partner Center.</span></span> <span data-ttu-id="ecf4d-192">Detta gör att partner kan:</span><span class="sxs-lookup"><span data-stu-id="ecf4d-192">This enables partners to:</span></span>

- <span data-ttu-id="ecf4d-193">Visa, hantera och ta emot aviseringar för budget uppsättning på en kund nivå</span><span class="sxs-lookup"><span data-stu-id="ecf4d-193">View, manage, and receive alerts for budget set at a customer level</span></span> 

- <span data-ttu-id="ecf4d-194">Visa totala uppskattade utgifter i en Azure-plan (uppdelad efter resurs och mätar nivå)</span><span class="sxs-lookup"><span data-stu-id="ecf4d-194">View total estimated spending on an Azure plan (broken down by resource and meter level)</span></span>

<span data-ttu-id="ecf4d-195">Eftersom fakturerings modellen för Azure-tjänster via en Azure-plan är efter löne förbrukning, för att undvika en större faktura än förväntat, kan partner tillämpa en månads budget och spåra procent andelen av användningen.</span><span class="sxs-lookup"><span data-stu-id="ecf4d-195">Because the billing model for Azure services through an Azure plan is post-pay consumption, to avoid a bigger bill than anticipated, partners can apply a monthly budget and track the percentage of usage.</span></span> <span data-ttu-id="ecf4d-196">En budget kan tillämpas på en kund eller flera kunder på en och samma tidpunkt.</span><span class="sxs-lookup"><span data-stu-id="ecf4d-196">A budget can be applied to one customer or multiple customers at one time.</span></span> 

:::image type="content" source="images/azure/azurespend.png" alt-text="Utgift i Azure":::

## <a name="next-steps"></a><span data-ttu-id="ecf4d-198">Nästa steg</span><span class="sxs-lookup"><span data-stu-id="ecf4d-198">Next steps</span></span>

- <span data-ttu-id="ecf4d-199">Se hur partnern för intjänad kredit (PEC) beräknas.</span><span class="sxs-lookup"><span data-stu-id="ecf4d-199">See how the partner earned credit (PEC) is calculated.</span></span> <span data-ttu-id="ecf4d-200">Logga in på Partner Center- [instrumentpanelen](https://partner.microsoft.com/dashboard/) och leta upp pris listan som är tillgänglig.</span><span class="sxs-lookup"><span data-stu-id="ecf4d-200">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard/) and locate the price list available.</span></span>

- <span data-ttu-id="ecf4d-201">Lär dig mer om [att köpa Azure-prenumerationen](purchase-azure-plan.md)</span><span class="sxs-lookup"><span data-stu-id="ecf4d-201">Learn about [purchasing the Azure plan](purchase-azure-plan.md)</span></span>

- <span data-ttu-id="ecf4d-202">Se [pris listan för den nya Commerce-upplevelsen i CSP](azure-plan-price-list.md)</span><span class="sxs-lookup"><span data-stu-id="ecf4d-202">See the [price list for the new commerce experience in CSP](azure-plan-price-list.md)</span></span>
