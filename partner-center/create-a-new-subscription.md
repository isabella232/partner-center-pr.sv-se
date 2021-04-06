---
title: Skapa kund prenumerationer i Partner Center
ms.topic: how-to
ms.date: 07/22/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 'Lär dig hur du säljer prenumerationer till dina kunder för produkter som publicerats av Microsoft samt SaaS-produkter som publicerats av tredjeparts-ISV: er.'
author: BillLinzbach
ms.author: BillLi
ms.custom: SEOAPR.20
ms.localizationpriority: medium
ms.openlocfilehash: 559d1fbd2efc1417ae89931279b9d3c9a1d67f7c
ms.sourcegitcommit: 3d7d5064c5e021079ed7e6f93f03869cbf425a32
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/06/2021
ms.locfileid: "106502943"
---
# <a name="create-suspend-or-cancel-customer-subscriptions"></a><span data-ttu-id="b9e64-103">Skapa, pausa eller avbryta kundprenumerationer</span><span class="sxs-lookup"><span data-stu-id="b9e64-103">Create, suspend, or cancel customer subscriptions</span></span>

<span data-ttu-id="b9e64-104">**Gäller för**</span><span class="sxs-lookup"><span data-stu-id="b9e64-104">**Applies to**</span></span>

- <span data-ttu-id="b9e64-105">Välkommen till Partnercenter för Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="b9e64-105">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="b9e64-106">**Lämpliga roller**</span><span class="sxs-lookup"><span data-stu-id="b9e64-106">**Appropriate roles**</span></span>

- <span data-ttu-id="b9e64-107">Administratörs agent</span><span class="sxs-lookup"><span data-stu-id="b9e64-107">Admin agent</span></span>
- <span data-ttu-id="b9e64-108">Faktureringsadministratör</span><span class="sxs-lookup"><span data-stu-id="b9e64-108">Billing admin</span></span>
- <span data-ttu-id="b9e64-109">Global administratör</span><span class="sxs-lookup"><span data-stu-id="b9e64-109">Global admin</span></span>
- <span data-ttu-id="b9e64-110">Support agent</span><span class="sxs-lookup"><span data-stu-id="b9e64-110">Helpdesk agent</span></span>
- <span data-ttu-id="b9e64-111">Försäljnings agent</span><span class="sxs-lookup"><span data-stu-id="b9e64-111">Sales agent</span></span>

<span data-ttu-id="b9e64-112">När du har skapat en post för din kund i Partner Center kan du sälja prenumerationer till produkter i katalogen.</span><span class="sxs-lookup"><span data-stu-id="b9e64-112">After you've created a record of your customer in the Partner Center, you can sell them subscriptions to products in the catalog.</span></span> <span data-ttu-id="b9e64-113">Detta inkluderar produkter som publicerats av Microsoft och SaaS-produkter (program vara som en tjänst) som publicerats av tredjeparts oberoende program varu leverantörer (ISV) till den [kommersiella marknads platsen](https://azuremarketplace.microsoft.com/marketplace).</span><span class="sxs-lookup"><span data-stu-id="b9e64-113">This includes products published by Microsoft and Software as a Service (SaaS) products published by third-party Independent Software Vendors (ISVs) to the [commercial marketplace](https://azuremarketplace.microsoft.com/marketplace).</span></span>

<span data-ttu-id="b9e64-114">Vissa erbjudanden är begränsade till en prenumeration per kund.</span><span class="sxs-lookup"><span data-stu-id="b9e64-114">Some offers are limited to one subscription per customer.</span></span> <span data-ttu-id="b9e64-115">Om du vill se en lista över vilka erbjudanden som är begränsade besöker du sidan priser och erbjudanden för partner Center.</span><span class="sxs-lookup"><span data-stu-id="b9e64-115">To see a list of which offers are restricted, visit the Partner Center Pricing and Offers page.</span></span>

>[!IMPORTANT]
> <span data-ttu-id="b9e64-116">Som partner i CSP-programmet kan du köpa **licensbaserade** eller **avgiftsbelagda** SaaS-prenumerationer från ISV-utgivare i Partner Center.</span><span class="sxs-lookup"><span data-stu-id="b9e64-116">As a partner in the CSP program, you can purchase **license-based** or **metered** SaaS subscriptions from ISV publishers within Partner Center.</span></span> <span data-ttu-id="b9e64-117">Det innebär att du kan köpa alla **licensbaserade** eller **avgiftsbelagda** SaaS-erbjudanden som ISV-utgivaren har gjort tillgängligt för dig, inklusive [exklusiva erbjudanden](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) som du har åtkomst till.</span><span class="sxs-lookup"><span data-stu-id="b9e64-117">This means you can purchase any **license-based** or **metered** SaaS offer the ISV publisher has made available to you, including [exclusive offers](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) to which you have access.</span></span> <span data-ttu-id="b9e64-118">För att köpa eller hantera andra erbjudanden från kommersiella Marketplace från ISV: er (till exempel användnings erbjudanden som rör Azure-program, behållare eller virtuella datorer) måste du gå till [Azure Portal](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="b9e64-118">To purchase or manage other, commercial marketplace offers from ISVs (such as usage-based offers involving Azure applications, Containers or VMs), you must go to the [Azure portal](https://portal.azure.com/).</span></span>

## <a name="create-a-new-subscription"></a><span data-ttu-id="b9e64-119">Skapa en ny prenumeration</span><span class="sxs-lookup"><span data-stu-id="b9e64-119">Create a new subscription</span></span>

1. <span data-ttu-id="b9e64-120">Logga in på [instrumentpanelen i Partnercenter](https://partner.microsoft.com/dashboard).</span><span class="sxs-lookup"><span data-stu-id="b9e64-120">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="b9e64-121">Från menyn Partner Center väljer du **kunder** och väljer sedan en kund i listan.</span><span class="sxs-lookup"><span data-stu-id="b9e64-121">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="b9e64-122">Välj **Lägg till prenumeration**.</span><span class="sxs-lookup"><span data-stu-id="b9e64-122">Select **Add subscription**.</span></span> <span data-ttu-id="b9e64-123">På fliken **online tjänster** visas alla tillgängliga Marketplace SaaS-erbjudanden.</span><span class="sxs-lookup"><span data-stu-id="b9e64-123">The **Online Services** tab will show all available Marketplace SaaS offers.</span></span>

4. <span data-ttu-id="b9e64-124">Om du bara vill se vissa typer av prenumerationer gör du inställningarna i de tillgängliga filtren:</span><span class="sxs-lookup"><span data-stu-id="b9e64-124">To see only certain types of subscriptions, make selections in the available filters:</span></span>
   - <span data-ttu-id="b9e64-125">**Utgivare**: Välj **Microsoft** om du bara vill se erbjudanden från Microsoft eller **partner** för att se produkter för kommersiella Marketplace som publicerats av ISV: er.</span><span class="sxs-lookup"><span data-stu-id="b9e64-125">**Publisher**: Choose **Microsoft** to see only offers from Microsoft, or **Partner** to see commercial marketplace products published by ISVs.</span></span>
   - <span data-ttu-id="b9e64-126">**Fakturerings typ**: Välj den typ av prenumerations fakturering som du vill använda: **licens** eller **användning**.</span><span class="sxs-lookup"><span data-stu-id="b9e64-126">**Billing type**: Select the type of subscription billing you want to use: **License** or **Usage**.</span></span> <span data-ttu-id="b9e64-127">Se [licensbaserade fakturerings](license-based-billing.md) information som hjälper dig att välja mellan månads-och års fakturerings frekvens.</span><span class="sxs-lookup"><span data-stu-id="b9e64-127">See [License-based billing](license-based-billing.md) for information that will help you decide between the monthly and annual billing frequency.</span></span>
   - <span data-ttu-id="b9e64-128">**Kategori**: Välj **företag**, **små företag** eller **utvärderings version**.</span><span class="sxs-lookup"><span data-stu-id="b9e64-128">**Category**: Choose **Enterprise**, **Small business**, or **Trial**.</span></span> <span data-ttu-id="b9e64-129">Information om utvärderings prenumerationer finns i [erbjuda dina kunders utvärdering av Microsoft-produkter](offer-your-customers-trials-of-microsoft-products.md).</span><span class="sxs-lookup"><span data-stu-id="b9e64-129">For info about trial subscriptions, see [Offer your customers trials of Microsoft products](offer-your-customers-trials-of-microsoft-products.md).</span></span>

5. <span data-ttu-id="b9e64-130">Välj de produkt prenumerationer som du vill köpa för kunden.</span><span class="sxs-lookup"><span data-stu-id="b9e64-130">Select the product subscriptions you want to purchase for your customer.</span></span> <span data-ttu-id="b9e64-131">Vilka produkter som visas beror på typen av kund segment (utbildning, myndigheter osv.) och de filter som du har tillämpat.</span><span class="sxs-lookup"><span data-stu-id="b9e64-131">The products you see depend on the type of customer segment (education, government, etc.) and the filters you have applied.</span></span> <span data-ttu-id="b9e64-132">Vissa erbjudanden som visas på Marketplace kanske inte alltid är tillgängliga för en viss kund eller en specifik CSP-partner.</span><span class="sxs-lookup"><span data-stu-id="b9e64-132">Some offers shown on the Marketplace may not always be available to a specific customer or a specific CSP partner.</span></span> <span data-ttu-id="b9e64-133">Detta kan bero på att:</span><span class="sxs-lookup"><span data-stu-id="b9e64-133">This can be because:</span></span>

   - <span data-ttu-id="b9e64-134">Kunden har redan en prenumeration på produkten och är bara tillåten en</span><span class="sxs-lookup"><span data-stu-id="b9e64-134">The customer already has a subscription to that product and is only allowed one</span></span>

   - <span data-ttu-id="b9e64-135">Kundens prenumeration kan ha inaktiverats (i det här fallet kan du återaktivera prenumerationen i stället för att köpa en ny.)</span><span class="sxs-lookup"><span data-stu-id="b9e64-135">The customer's subscription may have been suspended (In this case, you can reactivate the subscription rather than purchase a new one.)</span></span>

   - <span data-ttu-id="b9e64-136">För ISV SaaS-erbjudanden kan det finnas några skäl till varför erbjudandet inte kan köpas: ISV kanske inte har stöd för kundens fakturerings land eller region. ISV: n kanske har valt att inte göra erbjudandet tillgängligt via CSP-programmet. eller så kan ISV: n ha gjort erbjudandet [exklusivt](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) för vissa CSP-partner.</span><span class="sxs-lookup"><span data-stu-id="b9e64-136">For ISV SaaS offers, there may be a few reasons why the offer is not available to purchase: The ISV may not support the customer's billing country or region; the ISV may have chosen not to make the offer available through the CSP program; or, the ISV may have made the offer [exclusive](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) to only certain CSP partners.</span></span> <span data-ttu-id="b9e64-137">Det går inte heller att använda ISV-erbjudandet via partner Center (till exempel behållare eller vissa användnings erbjudanden).</span><span class="sxs-lookup"><span data-stu-id="b9e64-137">The ISV offer may also not be transactable through the Partner Center (for example, containers or some usage-based offers).</span></span>  

6. <span data-ttu-id="b9e64-138">Ange antalet licenser (om det behövs) för varje prenumeration som du vill lägga till och välj **Lägg till i kundvagn**.</span><span class="sxs-lookup"><span data-stu-id="b9e64-138">For each subscription you want to add, enter the number of licenses (if needed) and select **Add to cart**.</span></span>

7. <span data-ttu-id="b9e64-139">När du har lagt till prenumerationerna väljer du **Granska** och granska din beställning.</span><span class="sxs-lookup"><span data-stu-id="b9e64-139">When you are finished adding subscriptions, select **Review** and review your order.</span></span>

8. <span data-ttu-id="b9e64-140">När du har granskat dina beställningar och är redo att köpa dessa prenumerationer väljer du **köp**.</span><span class="sxs-lookup"><span data-stu-id="b9e64-140">Once you've reviewed your orders and are ready to purchase these subscriptions, select **Buy**.</span></span>

9. <span data-ttu-id="b9e64-141">När du har köpt en prenumeration för en kund görs följande:</span><span class="sxs-lookup"><span data-stu-id="b9e64-141">After you buy a subscription for a customer, the following will occur:</span></span>

    - <span data-ttu-id="b9e64-142">Du kan granska eller redigera prenumerationen genom att välja prenumerations namnet från kund **prenumerations** sidan.</span><span class="sxs-lookup"><span data-stu-id="b9e64-142">You can review or edit the subscription by selecting the subscription name from that customer's **Subscriptions** page.</span></span> <span data-ttu-id="b9e64-143">Härifrån kan du välja tilläggs licenser om de är tillgängliga, ändra antalet licenser eller pausa prenumerationen.</span><span class="sxs-lookup"><span data-stu-id="b9e64-143">From here, you can select add-on licenses if any are available, change the quantity of licenses, or suspend the subscription.</span></span>

    <span data-ttu-id="b9e64-144">**För ISV SaaS (licensbaserade och avgiftsbelagda) prenumerationer:**</span><span class="sxs-lookup"><span data-stu-id="b9e64-144">**For ISV SaaS (license-based and metered) subscriptions:**</span></span>
    - <span data-ttu-id="b9e64-145">Du får en länk till ISV-utgivarens webbplats.</span><span class="sxs-lookup"><span data-stu-id="b9e64-145">You will receive a link to the ISV publisher's site.</span></span> <span data-ttu-id="b9e64-146">Den här länken bör hjälpa dig att slutföra distributions-eller konto konfigurationen för kundens prenumeration.</span><span class="sxs-lookup"><span data-stu-id="b9e64-146">This link should help you complete the deployment or account setup of the customer's subscription.</span></span>
      
    >[!NOTE]
    > <span data-ttu-id="b9e64-147">Varken du eller din kund får ett e-postmeddelande med instruktioner för att slutföra konto konfigurationen/etableringen för den här typen av ISV-prenumeration.)</span><span class="sxs-lookup"><span data-stu-id="b9e64-147">Neither you nor your customer will receive an email with instructions to complete account set up/provisioning for this type of ISV subscription.)</span></span>

    - <span data-ttu-id="b9e64-148">Om din prenumeration kommer med en 30-dagars kostnads fri utvärderings period, kommer den kostnads fria utvärderings perioden att tillämpas automatiskt.</span><span class="sxs-lookup"><span data-stu-id="b9e64-148">If your subscription comes with a 30-day free trial, the free trial period will be applied automatically.</span></span> <span data-ttu-id="b9e64-149">Som partner i CSP-programmet kan du inte avstå från den kostnads fria utvärderings perioden på erbjudanden som du köper för kunder.</span><span class="sxs-lookup"><span data-stu-id="b9e64-149">As a partner in the CSP program, you cannot waive the free trial period on offers you purchase for customers.</span></span> <span data-ttu-id="b9e64-150">När den kostnads fria utvärderings perioden är slut börjar prenumerations perioden och prenumerationen kommer att konverteras till betald status.</span><span class="sxs-lookup"><span data-stu-id="b9e64-150">Once the free trial period ends, the subscription term will begin and the subscription will convert to paid status.</span></span> <span data-ttu-id="b9e64-151">Prenumerationen förnyas då automatiskt enligt samma schema.</span><span class="sxs-lookup"><span data-stu-id="b9e64-151">The subscription will then auto-renew according to the same schedule.</span></span>
   
## <a name="update-subscriptions-with-add-ons"></a><span data-ttu-id="b9e64-152">Uppdatera prenumerationer med tillägg</span><span class="sxs-lookup"><span data-stu-id="b9e64-152">Update subscriptions with add-ons</span></span> 

<span data-ttu-id="b9e64-153">För att köpa ett tillägg måste kunden först ha en aktiv bas prenumeration.</span><span class="sxs-lookup"><span data-stu-id="b9e64-153">To purchase an add-on, the customer must first have an active base subscription.</span></span>  <span data-ttu-id="b9e64-154">Det går inte att köpa tillägg via katalogen.</span><span class="sxs-lookup"><span data-stu-id="b9e64-154">You can't purchase add-ons through the catalog.</span></span>

1. <span data-ttu-id="b9e64-155">Logga in på [instrument panelen](https://partner.microsoft.com/dashboard)för partner Center.</span><span class="sxs-lookup"><span data-stu-id="b9e64-155">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="b9e64-156">Från menyn Partner Center väljer du **kunder** och väljer sedan en kund i listan.</span><span class="sxs-lookup"><span data-stu-id="b9e64-156">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="b9e64-157">Välj den prenumeration som du vill hantera.</span><span class="sxs-lookup"><span data-stu-id="b9e64-157">Choose the subscription you want to manage.</span></span>

4. <span data-ttu-id="b9e64-158">Under avsnittet **status** finns en lista över tillgängliga tilläggs komponenter för prenumerationen.</span><span class="sxs-lookup"><span data-stu-id="b9e64-158">Below the **Status** section, are a list of available Add-ons for the subscription.</span></span>  

5. <span data-ttu-id="b9e64-159">Uppdatera antalet licenser för varje nödvändigt tillägg.</span><span class="sxs-lookup"><span data-stu-id="b9e64-159">Update the quantity of licenses for each required Add-on.</span></span> <span data-ttu-id="b9e64-160">**Skicka** sedan dina ändringar.</span><span class="sxs-lookup"><span data-stu-id="b9e64-160">Then **Submit** your changes.</span></span>

<span data-ttu-id="b9e64-161">Möjligheten att köpa tillägg via partner Center är bara tillgänglig för direkta fakturerings-och indirekta leverantörer.</span><span class="sxs-lookup"><span data-stu-id="b9e64-161">The ability to purchase add-ons through Partner Center is only available to direct bill and indirect providers.</span></span>
<span data-ttu-id="b9e64-162">Endast kvalificerade tillägg visas baserat på grundläggande krav och regional tillgänglighet.</span><span class="sxs-lookup"><span data-stu-id="b9e64-162">Only eligible add-ons are displayed based on the base requirements and regional availability.</span></span> <span data-ttu-id="b9e64-163">Mer information om priser och erbjudanden finns i matrisen för moln åter försäljare.</span><span class="sxs-lookup"><span data-stu-id="b9e64-163">For more information about pricing and offers, refer to the Cloud Reseller offer matrix.</span></span> <span data-ttu-id="b9e64-164">Om du avbryter basprenumerationen inaktiveras även eventuella associerade tillägg.</span><span class="sxs-lookup"><span data-stu-id="b9e64-164">Suspending the base subscription will also suspend any associated add-ons.</span></span>

<span data-ttu-id="b9e64-165">Startdatumen för tillägg följer basprenumerationen och avgifterna beräknas utifrån startdatumet för debitering och slutdatumet för debitering med proportionella avgifter på den första fakturan.</span><span class="sxs-lookup"><span data-stu-id="b9e64-165">Start dates for add-ons align to the base subscription and charges are calculated from the Charge start date and Charge end date with pro-rata charges in the first invoice.</span></span> <span data-ttu-id="b9e64-166">Mer information finns i [licensbaserade fakturering](license-based-billing.md).</span><span class="sxs-lookup"><span data-stu-id="b9e64-166">For additional information see, [License-based billing](license-based-billing.md).</span></span>


## <a name="suspend-or-cancel-a-subscription"></a><span data-ttu-id="b9e64-167">Pausa eller avbryta en prenumeration</span><span class="sxs-lookup"><span data-stu-id="b9e64-167">Suspend or cancel a subscription</span></span>

<span data-ttu-id="b9e64-168">Partner kan pausa eller avbryta en prenumeration om det begärs av kunden, eller i fall av inbetalning eller bedrägerier.</span><span class="sxs-lookup"><span data-stu-id="b9e64-168">Partners can suspend or cancel a subscription if requested by the customer, or in cases of nonpayment or fraud.</span></span>

### <a name="suspend-a-subscription"></a><span data-ttu-id="b9e64-169">Inaktivera en prenumeration</span><span class="sxs-lookup"><span data-stu-id="b9e64-169">Suspend a subscription</span></span>

<span data-ttu-id="b9e64-170">När du ändrar status för en prenumeration till **inaktive** rad kan användarna inte logga in eller komma åt tjänster.</span><span class="sxs-lookup"><span data-stu-id="b9e64-170">When you change the status of a subscription to **Suspended**, users are not able to sign in or access services.</span></span>

1. <span data-ttu-id="b9e64-171">Logga in på [instrument panelen](https://partner.microsoft.com/dashboard)för partner Center.</span><span class="sxs-lookup"><span data-stu-id="b9e64-171">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="b9e64-172">Från menyn Partner Center väljer du **kunder** och väljer sedan en kund i listan.</span><span class="sxs-lookup"><span data-stu-id="b9e64-172">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="b9e64-173">Välj den prenumeration som du vill hantera.</span><span class="sxs-lookup"><span data-stu-id="b9e64-173">Choose the subscription you want to manage.</span></span>

4. <span data-ttu-id="b9e64-174">I avsnittet **Status** väljer du **Tillfälligt avbruten**.</span><span class="sxs-lookup"><span data-stu-id="b9e64-174">In the **Status** section, choose **Suspended**.</span></span> <span data-ttu-id="b9e64-175">**Skicka** sedan dina ändringar.</span><span class="sxs-lookup"><span data-stu-id="b9e64-175">Then **Submit** your changes.</span></span>

5. <span data-ttu-id="b9e64-176">Alla data tas bort om inte prenumerationen återaktiveras inom 90 dagar, eller 90 dagar plus antalet dagar mellan den tidpunkt då kontot öppnades och den första fakturerings perioden (maximalt 120 dagar).</span><span class="sxs-lookup"><span data-stu-id="b9e64-176">All data will be deleted unless the subscription is reactivated within 90 days, or 90 days plus the number of days between the time the account was opened and the first billing period (maximum 120 days).</span></span>

<span data-ttu-id="b9e64-177">När du pausar en prenumeration visar datumet som visas under den **nedbrutna** knappen när prenumerationen upphör att gälla automatiskt om du inte återaktiverar den.</span><span class="sxs-lookup"><span data-stu-id="b9e64-177">When you suspend a subscription, the date you see below the **Suspended** button indicates when the subscription would automatically expire if you don't reactivate it.</span></span> 

### <a name="cancel-a-subscription"></a><span data-ttu-id="b9e64-178">Avbryta en prenumeration</span><span class="sxs-lookup"><span data-stu-id="b9e64-178">Cancel a subscription</span></span>

<span data-ttu-id="b9e64-179">Du kan avbryta licensbaserade SaaS-prenumerationer från tredjeparts ISV-utgivare i Partner Center- [kommersiella marknads platser](csp-commercial-marketplace-overview.md).</span><span class="sxs-lookup"><span data-stu-id="b9e64-179">You can cancel license-based SaaS subscriptions from third-party ISV publishers within the Partner Center [commercial marketplace](csp-commercial-marketplace-overview.md).</span></span> <span data-ttu-id="b9e64-180">Så länge som du avbryter inom uppsägnings perioden får du en fullständig åter betalning.</span><span class="sxs-lookup"><span data-stu-id="b9e64-180">As long as you cancel within the cancellation period, you will receive a full refund.</span></span>

<span data-ttu-id="b9e64-181">För ISV-erbjudanden faktureras månads vis:</span><span class="sxs-lookup"><span data-stu-id="b9e64-181">For ISV offers billed monthly:</span></span>

- <span data-ttu-id="b9e64-182">Om du avbryter mindre än 24 timmar efter att du har placerat beställningen får du en fullständig kredit på nästa faktura.</span><span class="sxs-lookup"><span data-stu-id="b9e64-182">If you cancel less than 24 hours after you placed the order, you will receive a full credit on the next invoice.</span></span>

- <span data-ttu-id="b9e64-183">Om du avbryter senare än 24 timmar efter att du har placerat ordern schemaläggs annulleringen till att ske vid förnyelse.</span><span class="sxs-lookup"><span data-stu-id="b9e64-183">If you cancel later than 24 hours after you placed the order, the cancellation will be scheduled to occur at renewal.</span></span>

<span data-ttu-id="b9e64-184">För fakturerade per år:</span><span class="sxs-lookup"><span data-stu-id="b9e64-184">For offers billed annually:</span></span>

- <span data-ttu-id="b9e64-185">Om du avbryter mindre än 14 dagar efter att du har placerat beställningen får du en fullständig kredit på nästa faktura.</span><span class="sxs-lookup"><span data-stu-id="b9e64-185">If you cancel less than 14 days after you place the order, you will receive a full credit on the next invoice.</span></span>

- <span data-ttu-id="b9e64-186">Om du avbryter senare än 14 dagar efter att du har placerat ordern schemaläggs annulleringen till att ske vid förnyelse.</span><span class="sxs-lookup"><span data-stu-id="b9e64-186">If you cancel later than 14 days after you place the order, the cancellation will be scheduled to occur at renewal.</span></span>

<span data-ttu-id="b9e64-187">När dessa perioder är över visas inte längre alternativet för att avbryta prenumerationen.</span><span class="sxs-lookup"><span data-stu-id="b9e64-187">After these periods are over, you will no longer see the option to cancel the subscription.</span></span>

> [!NOTE]
> <span data-ttu-id="b9e64-188">Användnings och avgiftsbelagda ISV-tjänster (som använder virtuella datorer eller behållare, till exempel) är inte tillgängliga för retur.</span><span class="sxs-lookup"><span data-stu-id="b9e64-188">Usage-based and metered, third-party ISV services (that use virtual machines or containers, for example) are not eligible for return.</span></span> <span data-ttu-id="b9e64-189">Användnings tjänster kan avetableras som en avbrotts metod.</span><span class="sxs-lookup"><span data-stu-id="b9e64-189">Usage-based services can be de-provisioned as a cancellation method.</span></span> <span data-ttu-id="b9e64-190">Eftersom avgifter faktureras efter användningen är dessa tjänster inte berättigade till åter betalning.</span><span class="sxs-lookup"><span data-stu-id="b9e64-190">Since charges are billed after use, these services are not eligible for a refund.</span></span>

<span data-ttu-id="b9e64-191">Så här avbryter du en licensbaserad SaaS-prenumeration från en ISV-utgivare:</span><span class="sxs-lookup"><span data-stu-id="b9e64-191">To cancel a license-based SaaS subscription from an ISV publisher, do the following:</span></span>

1. <span data-ttu-id="b9e64-192">Logga in på [instrument panelen](https://partner.microsoft.com/dashboard)för partner Center.</span><span class="sxs-lookup"><span data-stu-id="b9e64-192">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="b9e64-193">Från menyn Partner Center väljer du **kunder** och väljer sedan en kund i listan.</span><span class="sxs-lookup"><span data-stu-id="b9e64-193">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="b9e64-194">Leta upp den prenumeration som du vill avbryta.</span><span class="sxs-lookup"><span data-stu-id="b9e64-194">Locate the subscription you want to cancel.</span></span>

4. <span data-ttu-id="b9e64-195">I kolumnen **status** väljer du **Avbryt**.</span><span class="sxs-lookup"><span data-stu-id="b9e64-195">In the **Status** column, select **Cancel**.</span></span> <span data-ttu-id="b9e64-196">**Skicka** sedan dina ändringar.</span><span class="sxs-lookup"><span data-stu-id="b9e64-196">Then **Submit** your changes.</span></span>

5. <span data-ttu-id="b9e64-197">Om en dialog ruta visas, Fyll i all relevant information och välj sedan **Skicka**.</span><span class="sxs-lookup"><span data-stu-id="b9e64-197">If a dialog box appears, fill out any relevant details then select **Submit**.</span></span>

6. <span data-ttu-id="b9e64-198">Bekräfta annulleringen genom att välja **Ja, Avbryt**.</span><span class="sxs-lookup"><span data-stu-id="b9e64-198">To confirm the cancellation, select **Yes, cancel**.</span></span>

> [!NOTE]
> <span data-ttu-id="b9e64-199">Du kan också välja att avbryta en Azure Marketplace-prenumeration med hjälp av API: er.</span><span class="sxs-lookup"><span data-stu-id="b9e64-199">You can also choose to cancel an Azure Marketplace subscription using APIs.</span></span> <span data-ttu-id="b9e64-200">För att göra det, se [avbryta en prenumeration på Azure Marketplace](/partner-center/develop/cancel-an-azure-marketplace-subscription).</span><span class="sxs-lookup"><span data-stu-id="b9e64-200">To do so, see [Cancel an Azure Marketplace subscription](/partner-center/develop/cancel-an-azure-marketplace-subscription).</span></span>

### <a name="choose-whether-to-automatically-renew-a-commercial-marketplace-subscription"></a><span data-ttu-id="b9e64-201">Välj om du vill förnya en prenumeration på en extern Marketplace automatiskt</span><span class="sxs-lookup"><span data-stu-id="b9e64-201">Choose whether to automatically renew a commercial marketplace subscription</span></span>

<span data-ttu-id="b9e64-202">Som standard förnyas prenumerationer automatiskt när prenumerationstiden går ut.</span><span class="sxs-lookup"><span data-stu-id="b9e64-202">By default, active subscriptions are set to automatically renew when the subscription period expires.</span></span> <span data-ttu-id="b9e64-203">För [prenumerationer på kommersiella Marketplace-produkter](csp-commercial-marketplace-overview.md)kan du välja att inte förnya prenumerationen automatiskt.</span><span class="sxs-lookup"><span data-stu-id="b9e64-203">For [subscriptions to commercial marketplace products](csp-commercial-marketplace-overview.md), you can optionally choose not to automatically renew the subscription.</span></span>

<span data-ttu-id="b9e64-204">Så här stoppar du en aktiv prenumeration på kommersiell marknads plats från automatisk förnyelse:</span><span class="sxs-lookup"><span data-stu-id="b9e64-204">To stop an active commercial marketplace subscription from automatically renewing:</span></span>

1. <span data-ttu-id="b9e64-205">Logga in på [instrument panelen](https://partner.microsoft.com/dashboard)för partner Center.</span><span class="sxs-lookup"><span data-stu-id="b9e64-205">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="b9e64-206">Från menyn Partner Center väljer du **kunder** och väljer sedan en kund i listan.</span><span class="sxs-lookup"><span data-stu-id="b9e64-206">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="b9e64-207">Välj **Prenumerationer**.</span><span class="sxs-lookup"><span data-stu-id="b9e64-207">Select **Subscriptions**.</span></span> <span data-ttu-id="b9e64-208">Här listas alla licensbaserade prenumerationer som du har köpt för kunden.</span><span class="sxs-lookup"><span data-stu-id="b9e64-208">This lists any license-based subscriptions you have purchased for the customer.</span></span>

4. <span data-ttu-id="b9e64-209">I kolumnen **prenumeration** väljer du den prenumeration som du vill ändra.</span><span class="sxs-lookup"><span data-stu-id="b9e64-209">In the **Subscription** column, select the subscription you want to modify.</span></span>

5. <span data-ttu-id="b9e64-210">På sidan prenumerations information letar du reda på avsnittet **status** och avmarkerar rutan **förnya automatiskt** .</span><span class="sxs-lookup"><span data-stu-id="b9e64-210">In the subscription details page, locate the **Status** section and uncheck the **Auto-renew** box.</span></span>

6. <span data-ttu-id="b9e64-211">Välj **Skicka**.</span><span class="sxs-lookup"><span data-stu-id="b9e64-211">Select **Submit**.</span></span>

## <a name="next-steps"></a><span data-ttu-id="b9e64-212">Nästa steg</span><span class="sxs-lookup"><span data-stu-id="b9e64-212">Next steps</span></span>

- [<span data-ttu-id="b9e64-213">Köp kommersiella Marketplace-produkter för dina kunder</span><span class="sxs-lookup"><span data-stu-id="b9e64-213">Purchase commercial marketplace products for your customers</span></span>](csp-commercial-marketplace-purchase.md)

- [<span data-ttu-id="b9e64-214">Hantera kommersiella Marketplace-produkter för dina kunder</span><span class="sxs-lookup"><span data-stu-id="b9e64-214">Manage commercial marketplace products for your customers</span></span>](csp-commercial-marketplace-manage.md)

- [<span data-ttu-id="b9e64-215">Översikt över kommersiell marknadsplats</span><span class="sxs-lookup"><span data-stu-id="b9e64-215">Commercial marketplace overview</span></span>](csp-commercial-marketplace-overview.md)