---
title: Fakturering av Azure-plan – & rekognoseringsfiler
ms.topic: article
ms.date: 01/20/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Lär dig hur du får åtkomst till och förstår strukturen för faktura- och avstämningsfiler relaterade till fakturering för Azure-planen.
author: khpavan
ms.author: sakhanda
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 757383ee264e58e7b4dc8ffefafe213cb49acb79
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 05/19/2021
ms.locfileid: "110149799"
---
# <a name="new-commerce-experience-in-csp---azure-billing"></a><span data-ttu-id="15369-103">Ny handelsupplevelse i CSP – Azure-fakturering</span><span class="sxs-lookup"><span data-stu-id="15369-103">New commerce experience in CSP - Azure billing</span></span> 

<span data-ttu-id="15369-104">**Lämpliga roller:** Administratörsagent | Faktureringsadministratörskonto | Global administratör</span><span class="sxs-lookup"><span data-stu-id="15369-104">**Appropriate roles**: Admin agent | Billing admin | Global admin</span></span>

<span data-ttu-id="15369-105">Den här artikeln förklarar hur du kommer åt och förstår strukturen för faktura- och avstämningsfiler relaterade till fakturering för Azure-planen.</span><span class="sxs-lookup"><span data-stu-id="15369-105">This article explains how to access and understand the invoice and reconciliation file structure related to billing for the Azure plan.</span></span> <span data-ttu-id="15369-106">Fakturering enligt Azure-planen är en förenklad faktureringsupplevelse med ett justerat enskilt faktureringsdatum och kalendermånadsbaserad faktureringsperiod.</span><span class="sxs-lookup"><span data-stu-id="15369-106">Billing under the Azure plan is a simplified billing experience using an aligned single billing date and calendar month-based billing period.</span></span>

## <a name="summary-of-billing-essentials"></a><span data-ttu-id="15369-107">Sammanfattning av faktureringsinformation</span><span class="sxs-lookup"><span data-stu-id="15369-107">Summary of billing essentials</span></span>

- <span data-ttu-id="15369-108">**Fakturadatum:** Faktura- och avstämningsfilen blir tillgänglig i Partnercenter-instrumentpanelen/API:et den 8:e (midnatt UTC).</span><span class="sxs-lookup"><span data-stu-id="15369-108">**Invoice date**: Invoice and reconciliation file will be available in the Partner Center dashboard/API by the 8th (midnight UTC).</span></span>

- <span data-ttu-id="15369-109">**Faktureringsperiod för** faktura: Faktureringsperioden justeras till kalendermånaden, till exempel 10/1-10/31, 11/1-11/30.</span><span class="sxs-lookup"><span data-stu-id="15369-109">**Invoice billing period**: The invoice billing period is aligned to the calendar month, for example,  10/1-10/31, 11/1-11/30.</span></span>

- <span data-ttu-id="15369-110">**Avgiftstjänstperioder:** Avgifterna justeras efter kalendermånaden.</span><span class="sxs-lookup"><span data-stu-id="15369-110">**Charge service periods**: Charges will align to the calendar month.</span></span> <span data-ttu-id="15369-111">Om den fakturerade partnern till exempel lägger till Azure-tjänster via en Azure-plan den 10/15 och kunden börjar använda Azure-tjänster den 10/15, får den fakturerade partnern faktura/rekognosering den 11/8 för kundförbrukning för tjänstperioden 10/15–10/31.</span><span class="sxs-lookup"><span data-stu-id="15369-111">For example, if billed partner adds Azure services through an Azure plan on 10/15 and the customer begins consumption of Azure services on 10/15, then billed partner will receive invoice/recon on 11/8 for customer consumption for the service period 10/15 - 10/31.</span></span> <span data-ttu-id="15369-112">Nästa månads faktura som genereras den 12/8 innehåller alla avgifter för tjänstperioden 11/1–11/31.</span><span class="sxs-lookup"><span data-stu-id="15369-112">The next month's invoice that is going to be generated on 12/8 contains all the charges for the service period 11/1- 11/31.</span></span>

- <span data-ttu-id="15369-113">**Fakturabetalning:** 60 dagar netto.</span><span class="sxs-lookup"><span data-stu-id="15369-113">**Invoice payment term**: Net 60 days.</span></span>

- <span data-ttu-id="15369-114">**Fakturavaluta:** Från och med 28 januari 2021 debiteras partner i regionen EU/EFTA och Storbritannien som har nya kunder och befintliga CSP-kunder som köper nya handelserbjudanden för första gången vars klienter skapades före den 11 maj 2020.</span><span class="sxs-lookup"><span data-stu-id="15369-114">**Invoice currency**: Starting January 28th 2021, partners in the EU/EFTA and UK region who have new customers and existing CSP customers purchasing new commerce offers for the first time whose tenants were created prior to 11 May 2020, will be billed for those purchases in partner location currency.</span></span> <span data-ttu-id="15369-115">Partner som är belägna utanför EU/EFTA- och Storbritannien-regionen fortsätter att debiteras i partnerns platsvaluta.</span><span class="sxs-lookup"><span data-stu-id="15369-115">Partners located outside of the EU/EFTA and UK region will continue to be billed in partner location currency.</span></span>

- <span data-ttu-id="15369-116">**Partnerincitament:** Betalas 45 dagar från slutet av fakturamånaden.</span><span class="sxs-lookup"><span data-stu-id="15369-116">**Partner incentives**: Paid 45 days from the end of the invoice month.</span></span>

## <a name="access-your-invoices-and-reconciliation-files"></a><span data-ttu-id="15369-117">Få åtkomst till dina fakturor och avstämningsfiler</span><span class="sxs-lookup"><span data-stu-id="15369-117">Access your invoices and reconciliation files</span></span>

<span data-ttu-id="15369-118">Den globala administratören eller faktureringsadministratören för ditt företag får ett e-postmeddelande när en faktura är redo att visas.</span><span class="sxs-lookup"><span data-stu-id="15369-118">The global admin or billing admin for your company will receive an email when an invoice is ready to view.</span></span>

<span data-ttu-id="15369-119">Så här kommer du åt fakturan och avstämningsfilen:</span><span class="sxs-lookup"><span data-stu-id="15369-119">To access the invoice and reconciliation file:</span></span>

1. <span data-ttu-id="15369-120">Logga in i Partnercenter och gå till [instrumentpanelen](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="15369-120">Sign in to the Partner Center [dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="15369-121">I menyn i Partnercenter väljer du **Fakturering.**</span><span class="sxs-lookup"><span data-stu-id="15369-121">From the Partner Center menu, select **Billing**.</span></span>

3. <span data-ttu-id="15369-122">Välj fliken för **Återkommande och** **Engångs och den** valuta som du är intresserad av.</span><span class="sxs-lookup"><span data-stu-id="15369-122">Select the tab for the **Recurring** and **One-time** and the currency you are interested in.</span></span>

   :::image type="content" source="images/azure/billing3.png" alt-text="Fakturering":::

4. <span data-ttu-id="15369-124">Välj **Faktura eller** **Avstämningsfil**.</span><span class="sxs-lookup"><span data-stu-id="15369-124">Select **Invoice** or **Reconciliation file**.</span></span>  

   <span data-ttu-id="15369-125">Om du vill visa historiska fakturor och rekognoseringsfiler expanderar du raden Faktureringshistorik nedan.</span><span class="sxs-lookup"><span data-stu-id="15369-125">To view historical invoices and recon files expand the Billing history row below.</span></span>

## <a name="understanding-usage-data"></a><span data-ttu-id="15369-126">Förstå användningsdata</span><span class="sxs-lookup"><span data-stu-id="15369-126">Understanding usage data</span></span> 

1. <span data-ttu-id="15369-127">Azure-planen är rot- eller toppnivåcontainern för användning.</span><span class="sxs-lookup"><span data-stu-id="15369-127">Azure plan is the root or top-level container for usage.</span></span> <span data-ttu-id="15369-128">All användning är kopplad till en enda Azure-plan.</span><span class="sxs-lookup"><span data-stu-id="15369-128">All usage is tied back to a single Azure plan.</span></span>

2. <span data-ttu-id="15369-129">Inom en plan finns det en eller flera Azure-prenumerationer.</span><span class="sxs-lookup"><span data-stu-id="15369-129">Within a plan, there will be one or more Azure subscriptions.</span></span> <span data-ttu-id="15369-130">Det här är containrar som används för resurshantering och distribution.</span><span class="sxs-lookup"><span data-stu-id="15369-130">These are containers used for resource management and deployment.</span></span> 

3. <span data-ttu-id="15369-131">I en prenumeration lägger resursgrupper till i gruppresurser.</span><span class="sxs-lookup"><span data-stu-id="15369-131">Within a subscription, resource groups add to group resources.</span></span> <span data-ttu-id="15369-132">Varje resurs distribueras till en resursgrupp.</span><span class="sxs-lookup"><span data-stu-id="15369-132">Every resource is deployed to one resource group.</span></span> 

4. <span data-ttu-id="15369-133">Exempel på resurser är virtuella datorer och lagringskonton.</span><span class="sxs-lookup"><span data-stu-id="15369-133">Examples of resources include virtual machines and storage accounts.</span></span> 

5. <span data-ttu-id="15369-134">Resursavsändarmätare: Mätare är mätningar av förbrukningen för en resurs och en resurs kan generera användning för flera mätare.</span><span class="sxs-lookup"><span data-stu-id="15369-134">Resource emit meters: Meters are measurements of consumption of a resource, and one resource may emit usage for multiple meters.</span></span> <span data-ttu-id="15369-135">Mätare identifieras av ett ProductId, SKUId och AvailabilityId.</span><span class="sxs-lookup"><span data-stu-id="15369-135">Meters are identified by a ProductId, SKUId, and AvailabilityId.</span></span> 

### <a name="hierarchy-of-subscription-resource-groups-and-metering"></a><span data-ttu-id="15369-136">Hierarki för prenumerationsresursgrupper och mätning</span><span class="sxs-lookup"><span data-stu-id="15369-136">Hierarchy of subscription resource groups and metering</span></span>

<span data-ttu-id="15369-137">**Azure-konto (klient)**</span><span class="sxs-lookup"><span data-stu-id="15369-137">**Azure account (tenant)**</span></span>

- <span data-ttu-id="15369-138">Prenumeration A</span><span class="sxs-lookup"><span data-stu-id="15369-138">Subscription A</span></span>
    - <span data-ttu-id="15369-139">ResourceGroup 1</span><span class="sxs-lookup"><span data-stu-id="15369-139">ResourceGroup 1</span></span>
        - <span data-ttu-id="15369-140">Virtuell dator (resurs)</span><span class="sxs-lookup"><span data-stu-id="15369-140">Virtual machine (resource)</span></span>
            - <span data-ttu-id="15369-141">Beräkningsmätare</span><span class="sxs-lookup"><span data-stu-id="15369-141">Compute meter</span></span>
        - <span data-ttu-id="15369-142">Virtuellt nätverk (resurs)</span><span class="sxs-lookup"><span data-stu-id="15369-142">Virtual network (resource)</span></span>
            - <span data-ttu-id="15369-143">Ingen faktureringsmätare</span><span class="sxs-lookup"><span data-stu-id="15369-143">No billing meter</span></span>

    - <span data-ttu-id="15369-144">ResourceGroup 2</span><span class="sxs-lookup"><span data-stu-id="15369-144">ResourceGroup 2</span></span>
        - <span data-ttu-id="15369-145">Virtuell dator (resurs)</span><span class="sxs-lookup"><span data-stu-id="15369-145">Virtual machine (resource)</span></span>
            - <span data-ttu-id="15369-146">Datormätare</span><span class="sxs-lookup"><span data-stu-id="15369-146">Computer meter</span></span>
        - <span data-ttu-id="15369-147">Premium SSD hanterad disk (resurs)</span><span class="sxs-lookup"><span data-stu-id="15369-147">Premium SSD-managed disk (resource)</span></span>
            - <span data-ttu-id="15369-148">Lagringskapacitetsmätare</span><span class="sxs-lookup"><span data-stu-id="15369-148">Storage capacity meter</span></span>
            - <span data-ttu-id="15369-149">Mätare för lagringsåtgärder</span><span class="sxs-lookup"><span data-stu-id="15369-149">Storage operations meter</span></span>

- <span data-ttu-id="15369-150">Prenumeration B – ResourceGroup 1 – Azure SQL (resurs) – DTU-mätare – VPN Gateway (resurs) – VPN-gatewaymätare</span><span class="sxs-lookup"><span data-stu-id="15369-150">Subscription B   -ResourceGroup 1       - Azure SQL (resource)           - DTU meter       - VPN Gateway (resource)           - VPN gateway meter</span></span>

    - <span data-ttu-id="15369-151">ResourceGroup 2</span><span class="sxs-lookup"><span data-stu-id="15369-151">ResourceGroup 2</span></span>
        - <span data-ttu-id="15369-152">Virtual Network (resurs)</span><span class="sxs-lookup"><span data-stu-id="15369-152">Virtual Network Interface (resource)</span></span>
            - <span data-ttu-id="15369-153">Ingen faktureringsmätare</span><span class="sxs-lookup"><span data-stu-id="15369-153">No billing meter</span></span>

## <a name="read-the-invoice"></a><span data-ttu-id="15369-154">Läsa fakturan</span><span class="sxs-lookup"><span data-stu-id="15369-154">Read the invoice</span></span>

1. <span data-ttu-id="15369-155">Fakturan blir tillgänglig senast den åttonde i varje månad.</span><span class="sxs-lookup"><span data-stu-id="15369-155">Invoice will be available no later than the eighth of each month.</span></span>

2. <span data-ttu-id="15369-156">Partner har 60 dagar på sig att betala.</span><span class="sxs-lookup"><span data-stu-id="15369-156">Partners have 60 days to remit payment.</span></span>

3. <span data-ttu-id="15369-157">Faktureringsperioden omfattar en viss kalendermånad, till exempel 10/1-10/31.</span><span class="sxs-lookup"><span data-stu-id="15369-157">The billing period will cover a given calendar month, for example, 10/1-10/31.</span></span>

4. <span data-ttu-id="15369-158">Avgifterna är nettojusteringar (beloppet är netto efter "Partner-intjänad kredit för hanterade tjänster").</span><span class="sxs-lookup"><span data-stu-id="15369-158">Charges are net of adjustments (amount is net of “Partner earned credit for services managed").</span></span>

5. <span data-ttu-id="15369-159">Granska fakturans rekognoseringsfil och den dagliga klassificerade användningsfilen för ytterligare faktureringsinformation.</span><span class="sxs-lookup"><span data-stu-id="15369-159">Review the invoice recon file and daily rated usage file for additional billing details.</span></span>

   :::image type="content" source="images/azure/invoice1.png" alt-text="Faktura":::

## <a name="read-the-invoice-reconciliation-file"></a><span data-ttu-id="15369-161">Läsa fakturaavstämningsfilen</span><span class="sxs-lookup"><span data-stu-id="15369-161">Read the invoice reconciliation file</span></span>

1. <span data-ttu-id="15369-162">Varje kombination av Azure-plan och mätare kan ha upp till två faktureringsrader i rekognoseringsfilen.</span><span class="sxs-lookup"><span data-stu-id="15369-162">Each Azure plan and meter combination may have up to two billing lines on the recon file.</span></span>

2. <span data-ttu-id="15369-163">Om mätaren är kvalificerad för någon typ av rabatt eller kredit (till exempel nivåindelade rabatter eller partnerintjänad kredit för tjänster som hanteras) under hela kalendermånaden innehåller rekognoseringsfilen endast en faktureringsrad.</span><span class="sxs-lookup"><span data-stu-id="15369-163">If the meter qualified for any type of discount or credit (such as tiered discounts or the Partner earned credit for services managed) throughout the entire calendar month, then the recon file will only contain one billing line.</span></span> <span data-ttu-id="15369-164">Kolumnen **PriceAdjusmentDescription refererar till** rabatten eller den intjänade krediten.</span><span class="sxs-lookup"><span data-stu-id="15369-164">The column **PriceAdjusmentDescription** will reference the discount or earned credit.</span></span>

3. <span data-ttu-id="15369-165">Om det inte finns några resurser för en viss mätare som är kvalificerade för rabatt eller partner-intjänad kredit innehåller rekognoseringsfilen bara en faktureringsrad och det effektiva enhetspriset är detaljhandelspriset (vilket är enhetspriset).</span><span class="sxs-lookup"><span data-stu-id="15369-165">If there are no resources for a particular meter that qualified for discount or partner earned credit, then the recon file will only contain one billing line and the effective unit price will be the retail price (which is the unit price).</span></span>

4. <span data-ttu-id="15369-166">Om mätaren, eller några resurser som  sänder mätaren, är kvalificerad för partner-intjänad kredit för tjänster som hanteras under en del av månaden, innehåller rekognoseringsfilen två faktureringsrader.</span><span class="sxs-lookup"><span data-stu-id="15369-166">If the meter, or any resources emitting that meter, qualified for **Partner earned credit for services managed** for a part of the month, the recon file will contain two billing lines.</span></span> <span data-ttu-id="15369-167">En rad representerar de dagar då mätaren kvalificerades och den andra raden representerar de dagar då mätaren inte var kvalificerad.</span><span class="sxs-lookup"><span data-stu-id="15369-167">One line will represent the days the meter qualified and the second line will represent the days the meter did not qualify.</span></span>

## <a name="read-the-daily-usage-file"></a><span data-ttu-id="15369-168">Läsa filen för daglig användning</span><span class="sxs-lookup"><span data-stu-id="15369-168">Read the daily usage file</span></span>

- <span data-ttu-id="15369-169">Prenumerationsmätare under en Azure-plan klassificeras och ackumuleras dagligen.</span><span class="sxs-lookup"><span data-stu-id="15369-169">Subscription meters under an Azure plan are rated, and are cumulated, on a daily basis.</span></span>

- <span data-ttu-id="15369-170">**Partnerns intjänade kredit för** tjänster som hanteras fastställs och tillämpas dagligen.</span><span class="sxs-lookup"><span data-stu-id="15369-170">**Partner earned credit for services managed** is determined and applied on a daily basis.</span></span>

- <span data-ttu-id="15369-171">Varje prenumerationsmätare har en rad för varje dag i månaden där det fanns förbrukning.</span><span class="sxs-lookup"><span data-stu-id="15369-171">Every subscription meter will have a row for every day of the month where there was consumption.</span></span>

- <span data-ttu-id="15369-172">I exemplet nedan:</span><span class="sxs-lookup"><span data-stu-id="15369-172">In the example below:</span></span>

  - <span data-ttu-id="15369-173">Mätare som är kvalificerade för partner-intjänad kredit för tjänster som hanteras från 7/1 till 7/3 (observera att det effektiva enhetspriset är återförsäljarpris minus partner-intjänad kredit. </span><span class="sxs-lookup"><span data-stu-id="15369-173">Meter qualified for **Partner earned credit for services managed** from 7/1 - 7/3 (note the effective unit price is retail price less partner earned credit.</span></span>

  - <span data-ttu-id="15369-174">Meter var inte  kvalificerat för partner-intjänad kredit för tjänster som hanteras 7/4–7/7 (observera att det effektiva enhetspriset är återförsäljarpris).</span><span class="sxs-lookup"><span data-stu-id="15369-174">Meter didn't qualify for **Partner earned credit for services managed** from 7/4 - 7/7 (note the effective unit price is retail price).</span></span>

  - <span data-ttu-id="15369-175">Mätare som är kvalificerad för partner-intjänad kredit för tjänster som hanteras från 7/8 till 7/31 (observera att det effektiva enhetspriset är återförsäljarpris minus partners intjänade kredit). </span><span class="sxs-lookup"><span data-stu-id="15369-175">Meter qualified for **Partner earned credit for services managed** from 7/8 - 7/31 (note the effective unit price is retail price less partner earned credit).</span></span>

   :::image type="content" source="images/azure/pecfinal.png" alt-text="recon2":::

## <a name="invoice-in-customer-currency"></a><span data-ttu-id="15369-177">Faktura i kundvaluta</span><span class="sxs-lookup"><span data-stu-id="15369-177">Invoice in customer currency</span></span>

<span data-ttu-id="15369-178">Azure-tjänster via en Azure-plan prissätts i USD och faktureras i kundens landstilldelade valuta.</span><span class="sxs-lookup"><span data-stu-id="15369-178">Azure services through an Azure plan will be priced in USD and billed in the customer country assigned currency.</span></span> <span data-ttu-id="15369-179">Om faktureringsvalutan inte är USD visas det valutautbytespris (FX) som används på den sista sidan på fakturan.</span><span class="sxs-lookup"><span data-stu-id="15369-179">If the billing currency is non-USD, then the Foreign exchange (FX) rate used will be shown on the last page of the invoice.</span></span> <span data-ttu-id="15369-180">FX-priser bestäms varje månad och tillämpas på följande faktura.</span><span class="sxs-lookup"><span data-stu-id="15369-180">FX rates are determined monthly and applied to the following invoice.</span></span> <span data-ttu-id="15369-181">En fullständig lista över valutor för länder finns i den nya handelslösningen med [landstillgänglighet och kundvalutamatrisen](https://go.microsoft.com/fwlink/?linkid=2112354).</span><span class="sxs-lookup"><span data-stu-id="15369-181">For a full list of country currencies, please view the [new commerce offers country availability and customer currency matrix](https://go.microsoft.com/fwlink/?linkid=2112354).</span></span>

<span data-ttu-id="15369-182">Microsoft följer London-börsen för konvertering.</span><span class="sxs-lookup"><span data-stu-id="15369-182">Microsoft follows the London Stock Exchange for conversion.</span></span> <span data-ttu-id="15369-183">Vi använder växelkursen, som är lika med växelkursen som avbildades den sista sekunden av den sista arbetsdagen i månaden på London-börsen.</span><span class="sxs-lookup"><span data-stu-id="15369-183">We use the exchange rate, which is equal to the exchange rate captured on the last second of the last business day of the month on the London Stock Exchange.</span></span> <span data-ttu-id="15369-184">FX-priserna uppdateras och är tillgängliga dagen före den första i månaden som de gäller för.</span><span class="sxs-lookup"><span data-stu-id="15369-184">The FX rates will be refreshed and available on the day before the first of the month for which they apply.</span></span>

## <a name="azure-reservations"></a><span data-ttu-id="15369-185">Azure-reservationer</span><span class="sxs-lookup"><span data-stu-id="15369-185">Azure reservations</span></span>


<span data-ttu-id="15369-186">Om du [köper Azure-reservationer](azure-reservations.md) via en Azure-plan kan du välja antingen en gång eller månatlig fakturering.</span><span class="sxs-lookup"><span data-stu-id="15369-186">If purchasing [Azure reservations](azure-reservations.md) through an Azure plan, you can choose either one-time or monthly billing.</span></span>


## <a name="azure-spending"></a><span data-ttu-id="15369-187">Utgift i Azure</span><span class="sxs-lookup"><span data-stu-id="15369-187">Azure spending</span></span>

<span data-ttu-id="15369-188">Den befintliga Azure-utgiftsupplevelsen har uppdaterats för att stödja den nya Azure-planfakturering i Partnercenter.</span><span class="sxs-lookup"><span data-stu-id="15369-188">The existing Azure spending experience is updated to support the new Azure plan billing in Partner Center.</span></span> <span data-ttu-id="15369-189">Detta gör att partner kan:</span><span class="sxs-lookup"><span data-stu-id="15369-189">This enables partners to:</span></span>

- <span data-ttu-id="15369-190">Visa, hantera och ta emot aviseringar för budget som angetts på kundnivå</span><span class="sxs-lookup"><span data-stu-id="15369-190">View, manage, and receive alerts for budget set at a customer level</span></span> 

- <span data-ttu-id="15369-191">Visa totala beräknade utgifter för en Azure-plan (uppdelade efter resurs- och mätarnivå)</span><span class="sxs-lookup"><span data-stu-id="15369-191">View total estimated spending on an Azure plan (broken down by resource and meter level)</span></span>

<span data-ttu-id="15369-192">Eftersom faktureringsmodellen för Azure-tjänster via en Azure-plan är förbrukning efter betalning kan partner använda en månatlig budget och spåra procentandelen av användningen för att undvika en större faktura än förväntat.</span><span class="sxs-lookup"><span data-stu-id="15369-192">Because the billing model for Azure services through an Azure plan is post-pay consumption, to avoid a bigger bill than anticipated, partners can apply a monthly budget and track the percentage of usage.</span></span> <span data-ttu-id="15369-193">En budget kan tillämpas på en kund eller flera kunder i taget.</span><span class="sxs-lookup"><span data-stu-id="15369-193">A budget can be applied to one customer or multiple customers at one time.</span></span> 

:::image type="content" source="images/azure/azurespend.png" alt-text="Utgift i Azure":::

## <a name="next-steps"></a><span data-ttu-id="15369-195">Nästa steg</span><span class="sxs-lookup"><span data-stu-id="15369-195">Next steps</span></span>

- <span data-ttu-id="15369-196">Se hur partnerns intjänade kredit (PEC) beräknas.</span><span class="sxs-lookup"><span data-stu-id="15369-196">See how the partner earned credit (PEC) is calculated.</span></span> <span data-ttu-id="15369-197">Logga in på instrumentpanelen [i Partnercenter](https://partner.microsoft.com/dashboard/) och leta upp den tillgängliga prislistan.</span><span class="sxs-lookup"><span data-stu-id="15369-197">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard/) and locate the price list available.</span></span>

- <span data-ttu-id="15369-198">Lär dig mer [om att köpa Azure-planen](purchase-azure-plan.md)</span><span class="sxs-lookup"><span data-stu-id="15369-198">Learn about [purchasing the Azure plan](purchase-azure-plan.md)</span></span>

- <span data-ttu-id="15369-199">Se [prislistan för den nya handelsupplevelsen i CSP](azure-plan-price-list.md)</span><span class="sxs-lookup"><span data-stu-id="15369-199">See the [price list for the new commerce experience in CSP](azure-plan-price-list.md)</span></span>
