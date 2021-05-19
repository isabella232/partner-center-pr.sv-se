---
title: Skapa kundprenumerationer i Partnercenter
ms.topic: how-to
ms.date: 05/17/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Lär dig hur du säljer prenumerationer till dina kunder för produkter som publicerats av Microsoft samt SaaS-produkter som publicerats av tredjeparts-ISV:er.
author: BillLinzbach
ms.author: BillLi
ms.custom: SEOAPR.20
ms.localizationpriority: medium
ms.openlocfilehash: 3269fa994d704c0a0dae067087bad8589a7ce031
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 05/19/2021
ms.locfileid: "110148213"
---
# <a name="create-suspend-or-cancel-customer-subscriptions"></a><span data-ttu-id="b009a-103">Skapa, pausa eller avbryta kundprenumerationer</span><span class="sxs-lookup"><span data-stu-id="b009a-103">Create, suspend, or cancel customer subscriptions</span></span>

<span data-ttu-id="b009a-104">**Gäller för:** Partner Center-| Partnercenter för Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="b009a-104">**Applies to**: Partner Center | Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="b009a-105">**Lämpliga roller:** Administratörsagent | Faktureringsadministratörskonto | Globala | Supportagent för | Försäljningsagent</span><span class="sxs-lookup"><span data-stu-id="b009a-105">**Appropriate roles**: Admin agent | Billing admin | Global admin | Helpdesk agent | Sales agent</span></span>

<span data-ttu-id="b009a-106">När du har skapat en post för kunden i Partnercenter kan du sälja dem prenumerationer till produkter i katalogen.</span><span class="sxs-lookup"><span data-stu-id="b009a-106">After you've created a record of your customer in the Partner Center, you can sell them subscriptions to products in the catalog.</span></span> <span data-ttu-id="b009a-107">Detta omfattar produkter som publicerats av Microsoft och SaaS-produkter (Software as a Service) som publicerats av oberoende programvaruleverantörer (ISV: er) från tredje part på den [kommersiella marknadsplatsen.](https://azuremarketplace.microsoft.com/marketplace)</span><span class="sxs-lookup"><span data-stu-id="b009a-107">This includes products published by Microsoft and Software as a Service (SaaS) products published by third-party Independent Software Vendors (ISVs) to the [commercial marketplace](https://azuremarketplace.microsoft.com/marketplace).</span></span>

<span data-ttu-id="b009a-108">Vissa erbjudanden är begränsade till en prenumeration per kund.</span><span class="sxs-lookup"><span data-stu-id="b009a-108">Some offers are limited to one subscription per customer.</span></span> <span data-ttu-id="b009a-109">Om du vill se en lista över vilka erbjudanden som är begränsade går du till sidan Priser och erbjudanden för Partnercenter.</span><span class="sxs-lookup"><span data-stu-id="b009a-109">To see a list of which offers are restricted, visit the Partner Center Pricing and Offers page.</span></span>

>[!IMPORTANT]
> <span data-ttu-id="b009a-110">Som partner i CSP-programmet kan du köpa  licensbaserade eller uppmätta SaaS-prenumerationer från **ISV-utgivare** i Partnercenter.</span><span class="sxs-lookup"><span data-stu-id="b009a-110">As a partner in the CSP program, you can purchase **license-based** or **metered** SaaS subscriptions from ISV publishers within Partner Center.</span></span> <span data-ttu-id="b009a-111">Det innebär att du kan köpa alla licensbaserade eller uppmätta SaaS-erbjudanden [](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) som  **ISV-utgivaren** har gjort tillgängliga för dig, inklusive exklusiva erbjudanden som du har åtkomst till.</span><span class="sxs-lookup"><span data-stu-id="b009a-111">This means you can purchase any **license-based** or **metered** SaaS offer the ISV publisher has made available to you, including [exclusive offers](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) to which you have access.</span></span> <span data-ttu-id="b009a-112">Om du vill köpa eller hantera andra erbjudanden på den kommersiella marknadsplatsen från ISV:er (till exempel användningsbaserade erbjudanden som rör Azure-program, containrar eller virtuella datorer) [måste du gå till Azure Portal](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="b009a-112">To purchase or manage other, commercial marketplace offers from ISVs (such as usage-based offers involving Azure applications, Containers or VMs), you must go to the [Azure portal](https://portal.azure.com/).</span></span>

## <a name="create-a-new-subscription"></a><span data-ttu-id="b009a-113">Skapa en ny prenumeration</span><span class="sxs-lookup"><span data-stu-id="b009a-113">Create a new subscription</span></span>

1. <span data-ttu-id="b009a-114">Logga in på [instrumentpanelen i Partnercenter](https://partner.microsoft.com/dashboard).</span><span class="sxs-lookup"><span data-stu-id="b009a-114">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="b009a-115">I menyn i Partnercenter väljer **du Kunder** och sedan en kund i listan.</span><span class="sxs-lookup"><span data-stu-id="b009a-115">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="b009a-116">Välj **Lägg till prenumeration.**</span><span class="sxs-lookup"><span data-stu-id="b009a-116">Select **Add subscription**.</span></span> <span data-ttu-id="b009a-117">På **fliken Onlinetjänster** visas alla tillgängliga SaaS-erbjudanden på Marketplace.</span><span class="sxs-lookup"><span data-stu-id="b009a-117">The **Online Services** tab will show all available Marketplace SaaS offers.</span></span>

4. <span data-ttu-id="b009a-118">Om du bara vill se vissa typer av prenumerationer gör du val i de tillgängliga filtren:</span><span class="sxs-lookup"><span data-stu-id="b009a-118">To see only certain types of subscriptions, make selections in the available filters:</span></span>
   - <span data-ttu-id="b009a-119">**Utgivare:** Välj **Microsoft om** du bara vill se erbjudanden från Microsoft eller Partner om **du vill** se produkter från den kommersiella marknadsplatsen som publicerats av ISV:er.</span><span class="sxs-lookup"><span data-stu-id="b009a-119">**Publisher**: Choose **Microsoft** to see only offers from Microsoft, or **Partner** to see commercial marketplace products published by ISVs.</span></span>
   - <span data-ttu-id="b009a-120">**Faktureringstyp:** Välj vilken typ av prenumerationsfakturering du vill använda: **Licens** eller **Användning.**</span><span class="sxs-lookup"><span data-stu-id="b009a-120">**Billing type**: Select the type of subscription billing you want to use: **License** or **Usage**.</span></span> <span data-ttu-id="b009a-121">Se [Licensbaserad fakturering för](license-based-billing.md) information som hjälper dig att välja mellan månatlig och årlig faktureringsfrekvens.</span><span class="sxs-lookup"><span data-stu-id="b009a-121">See [License-based billing](license-based-billing.md) for information that will help you decide between the monthly and annual billing frequency.</span></span>
   - <span data-ttu-id="b009a-122">**Kategori:** Välj **Företag,** **Litet företag** eller **Utvärderingsversion.**</span><span class="sxs-lookup"><span data-stu-id="b009a-122">**Category**: Choose **Enterprise**, **Small business**, or **Trial**.</span></span> <span data-ttu-id="b009a-123">Information om utvärderingsprenumerationer finns [i Offer your customers trials of Microsoft products (Erbjuda dina kunder utvärderingsversioner av Microsoft-produkter).](offer-your-customers-trials-of-microsoft-products.md)</span><span class="sxs-lookup"><span data-stu-id="b009a-123">For info about trial subscriptions, see [Offer your customers trials of Microsoft products](offer-your-customers-trials-of-microsoft-products.md).</span></span>

5. <span data-ttu-id="b009a-124">Välj de produktprenumerationer som du vill köpa för kunden.</span><span class="sxs-lookup"><span data-stu-id="b009a-124">Select the product subscriptions you want to purchase for your customer.</span></span> <span data-ttu-id="b009a-125">Vilka produkter du ser beror på typen av kundsegment (utbildning, myndigheter osv.) och de filter som du har tillämpat.</span><span class="sxs-lookup"><span data-stu-id="b009a-125">The products you see depend on the type of customer segment (education, government, etc.) and the filters you have applied.</span></span> <span data-ttu-id="b009a-126">Vissa erbjudanden som visas på Marketplace kanske inte alltid är tillgängliga för en specifik kund eller en specifik CSP-partner.</span><span class="sxs-lookup"><span data-stu-id="b009a-126">Some offers shown on the Marketplace may not always be available to a specific customer or a specific CSP partner.</span></span> <span data-ttu-id="b009a-127">Det kan vara så här:</span><span class="sxs-lookup"><span data-stu-id="b009a-127">This can be because:</span></span>

   - <span data-ttu-id="b009a-128">Kunden har redan en prenumeration på produkten och tillåts bara en</span><span class="sxs-lookup"><span data-stu-id="b009a-128">The customer already has a subscription to that product and is only allowed one</span></span>

   - <span data-ttu-id="b009a-129">Kundens prenumeration kan ha inaktiverats (i det här fallet kan du återaktivera prenumerationen i stället för att köpa en ny.)</span><span class="sxs-lookup"><span data-stu-id="b009a-129">The customer's subscription may have been suspended (In this case, you can reactivate the subscription rather than purchase a new one.)</span></span>

   - <span data-ttu-id="b009a-130">För ISV SaaS-erbjudanden kan det finnas några orsaker till varför erbjudandet inte är tillgängligt att köpa: ISV:en kanske inte stöder kundens faktureringsland eller region; ISV:en kan ha valt att inte göra erbjudandet tillgängligt via CSP-programmet, eller så kan ISV:en ha gjort erbjudandet [exklusivt för](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) vissa CSP-partner.</span><span class="sxs-lookup"><span data-stu-id="b009a-130">For ISV SaaS offers, there may be a few reasons why the offer is not available to purchase: The ISV may not support the customer's billing country or region; the ISV may have chosen not to make the offer available through the CSP program; or, the ISV may have made the offer [exclusive](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) to only certain CSP partners.</span></span> <span data-ttu-id="b009a-131">ISV-erbjudandet kanske inte heller kan göras via Partnercenter (till exempel containrar eller vissa användningsbaserade erbjudanden).</span><span class="sxs-lookup"><span data-stu-id="b009a-131">The ISV offer may also not be transactable through the Partner Center (for example, containers or some usage-based offers).</span></span>  

6. <span data-ttu-id="b009a-132">För varje prenumeration som du vill lägga till anger du antalet licenser (om det behövs) och väljer Lägg **till i kundvagn.**</span><span class="sxs-lookup"><span data-stu-id="b009a-132">For each subscription you want to add, enter the number of licenses (if needed) and select **Add to cart**.</span></span>

7. <span data-ttu-id="b009a-133">När du är klar med att lägga till prenumerationer väljer **du Granska** och granskar din beställning.</span><span class="sxs-lookup"><span data-stu-id="b009a-133">When you are finished adding subscriptions, select **Review** and review your order.</span></span>

8. <span data-ttu-id="b009a-134">När du har granskat dina beställningar och är redo att köpa dessa prenumerationer väljer du **Köp.**</span><span class="sxs-lookup"><span data-stu-id="b009a-134">Once you've reviewed your orders and are ready to purchase these subscriptions, select **Buy**.</span></span>

9. <span data-ttu-id="b009a-135">När du har köpt en prenumeration för en kund sker följande:</span><span class="sxs-lookup"><span data-stu-id="b009a-135">After you buy a subscription for a customer, the following will occur:</span></span>

    - <span data-ttu-id="b009a-136">Du kan granska eller redigera prenumerationen genom att välja prenumerationsnamnet på kundens **prenumerationssida.**</span><span class="sxs-lookup"><span data-stu-id="b009a-136">You can review or edit the subscription by selecting the subscription name from that customer's **Subscriptions** page.</span></span> <span data-ttu-id="b009a-137">Härifrån kan du välja tilläggslicenser om det finns några, ändra antalet licenser eller pausa prenumerationen.</span><span class="sxs-lookup"><span data-stu-id="b009a-137">From here, you can select add-on licenses if any are available, change the quantity of licenses, or suspend the subscription.</span></span>

    <span data-ttu-id="b009a-138">**För ISV SaaS-prenumerationer (licensbaserade och uppmätta):**</span><span class="sxs-lookup"><span data-stu-id="b009a-138">**For ISV SaaS (license-based and metered) subscriptions:**</span></span>
    - <span data-ttu-id="b009a-139">Du får en länk till ISV-utgivarens webbplats.</span><span class="sxs-lookup"><span data-stu-id="b009a-139">You will receive a link to the ISV publisher's site.</span></span> <span data-ttu-id="b009a-140">Den här länken hjälper dig att slutföra distributionen eller kontokonfigurationen av kundens prenumeration.</span><span class="sxs-lookup"><span data-stu-id="b009a-140">This link should help you complete the deployment or account setup of the customer's subscription.</span></span>
      
    >[!NOTE]
    > <span data-ttu-id="b009a-141">Varken du eller kunden får ett e-postmeddelande med instruktioner för att slutföra konto set up/provisioning för den här typen av ISV-prenumeration.)</span><span class="sxs-lookup"><span data-stu-id="b009a-141">Neither you nor your customer will receive an email with instructions to complete account set up/provisioning for this type of ISV subscription.)</span></span>

    - <span data-ttu-id="b009a-142">Om din prenumeration har en 30-dagars kostnadsfri utvärderingsversion tillämpas den kostnadsfria utvärderingsperioden automatiskt.</span><span class="sxs-lookup"><span data-stu-id="b009a-142">If your subscription comes with a 30-day free trial, the free trial period will be applied automatically.</span></span> <span data-ttu-id="b009a-143">Som partner i CSP-programmet kan du inte undanta den kostnadsfria utvärderingsperioden för erbjudanden som du köper till kunder.</span><span class="sxs-lookup"><span data-stu-id="b009a-143">As a partner in the CSP program, you cannot waive the free trial period on offers you purchase for customers.</span></span> <span data-ttu-id="b009a-144">När den kostnadsfria utvärderingsperioden har avslutats börjar prenumerationsperioden och prenumerationen konverteras till betald status.</span><span class="sxs-lookup"><span data-stu-id="b009a-144">Once the free trial period ends, the subscription term will begin and the subscription will convert to paid status.</span></span> <span data-ttu-id="b009a-145">Prenumerationen förnyas sedan automatiskt enligt samma schema.</span><span class="sxs-lookup"><span data-stu-id="b009a-145">The subscription will then auto-renew according to the same schedule.</span></span>
   
## <a name="update-subscriptions-with-add-ons"></a><span data-ttu-id="b009a-146">Uppdatera prenumerationer med tillägg</span><span class="sxs-lookup"><span data-stu-id="b009a-146">Update subscriptions with add-ons</span></span> 

<span data-ttu-id="b009a-147">För att kunna köpa ett tillägg måste kunden först ha en aktiv basprenumeration.</span><span class="sxs-lookup"><span data-stu-id="b009a-147">To purchase an add-on, the customer must first have an active base subscription.</span></span>  <span data-ttu-id="b009a-148">Det går inte att köpa tillägg via katalogen.</span><span class="sxs-lookup"><span data-stu-id="b009a-148">You can't purchase add-ons through the catalog.</span></span>

1. <span data-ttu-id="b009a-149">Logga in på instrumentpanelen i [Partnercenter.](https://partner.microsoft.com/dashboard)</span><span class="sxs-lookup"><span data-stu-id="b009a-149">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="b009a-150">I menyn i Partnercenter väljer **du Kunder** och sedan en kund i listan.</span><span class="sxs-lookup"><span data-stu-id="b009a-150">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="b009a-151">Välj den prenumeration som du vill hantera.</span><span class="sxs-lookup"><span data-stu-id="b009a-151">Choose the subscription you want to manage.</span></span>

4. <span data-ttu-id="b009a-152">Under **avsnittet Status** finns en lista över tillgängliga tillägg för prenumerationen.</span><span class="sxs-lookup"><span data-stu-id="b009a-152">Below the **Status** section, are a list of available Add-ons for the subscription.</span></span>  

5. <span data-ttu-id="b009a-153">Uppdatera antalet licenser för varje obligatoriskt tillägg.</span><span class="sxs-lookup"><span data-stu-id="b009a-153">Update the quantity of licenses for each required Add-on.</span></span> <span data-ttu-id="b009a-154">**Skicka** sedan dina ändringar.</span><span class="sxs-lookup"><span data-stu-id="b009a-154">Then **Submit** your changes.</span></span>

<span data-ttu-id="b009a-155">Möjligheten att köpa tillägg via Partnercenter är endast tillgänglig för direkta fakturerade och indirekta leverantörer.</span><span class="sxs-lookup"><span data-stu-id="b009a-155">The ability to purchase add-ons through Partner Center is only available to direct bill and indirect providers.</span></span>
<span data-ttu-id="b009a-156">Endast berättigade tillägg visas baserat på grundkraven och regional tillgänglighet.</span><span class="sxs-lookup"><span data-stu-id="b009a-156">Only eligible add-ons are displayed based on the base requirements and regional availability.</span></span> <span data-ttu-id="b009a-157">Mer information om priser och erbjudanden finns i erbjudandematrisen för molnåterförsäljare.</span><span class="sxs-lookup"><span data-stu-id="b009a-157">For more information about pricing and offers, refer to the Cloud Reseller offer matrix.</span></span> <span data-ttu-id="b009a-158">Om du avbryter basprenumerationen inaktiveras även eventuella associerade tillägg.</span><span class="sxs-lookup"><span data-stu-id="b009a-158">Suspending the base subscription will also suspend any associated add-ons.</span></span>

<span data-ttu-id="b009a-159">Startdatumen för tillägg följer basprenumerationen och avgifterna beräknas utifrån startdatumet för debitering och slutdatumet för debitering med proportionella avgifter på den första fakturan.</span><span class="sxs-lookup"><span data-stu-id="b009a-159">Start dates for add-ons align to the base subscription and charges are calculated from the Charge start date and Charge end date with pro-rata charges in the first invoice.</span></span> <span data-ttu-id="b009a-160">Mer information finns i [Licensbaserad fakturering.](license-based-billing.md)</span><span class="sxs-lookup"><span data-stu-id="b009a-160">For additional information see, [License-based billing](license-based-billing.md).</span></span>


## <a name="suspend-or-cancel-a-subscription"></a><span data-ttu-id="b009a-161">Pausa eller avbryta en prenumeration</span><span class="sxs-lookup"><span data-stu-id="b009a-161">Suspend or cancel a subscription</span></span>

<span data-ttu-id="b009a-162">Partner kan inaktivera eller avbryta en prenumeration om det begärs av kunden, eller i fall av utebliven betalning eller bedrägeri.</span><span class="sxs-lookup"><span data-stu-id="b009a-162">Partners can suspend or cancel a subscription if requested by the customer, or in cases of nonpayment or fraud.</span></span>

### <a name="suspend-a-subscription"></a><span data-ttu-id="b009a-163">Inaktivera en prenumeration</span><span class="sxs-lookup"><span data-stu-id="b009a-163">Suspend a subscription</span></span>

<span data-ttu-id="b009a-164">När du ändrar statusen för en prenumeration **till Inaktiverad** kan användarna inte logga in eller komma åt tjänster.</span><span class="sxs-lookup"><span data-stu-id="b009a-164">When you change the status of a subscription to **Suspended**, users are not able to sign in or access services.</span></span>

1. <span data-ttu-id="b009a-165">Logga in på instrumentpanelen i [Partnercenter.](https://partner.microsoft.com/dashboard)</span><span class="sxs-lookup"><span data-stu-id="b009a-165">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="b009a-166">I menyn i Partnercenter väljer **du Kunder** och sedan en kund i listan.</span><span class="sxs-lookup"><span data-stu-id="b009a-166">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="b009a-167">Välj den prenumeration som du vill hantera.</span><span class="sxs-lookup"><span data-stu-id="b009a-167">Choose the subscription you want to manage.</span></span>

4. <span data-ttu-id="b009a-168">I avsnittet **Status** väljer du **Tillfälligt avbruten**.</span><span class="sxs-lookup"><span data-stu-id="b009a-168">In the **Status** section, choose **Suspended**.</span></span> <span data-ttu-id="b009a-169">**Skicka** sedan dina ändringar.</span><span class="sxs-lookup"><span data-stu-id="b009a-169">Then **Submit** your changes.</span></span>

5. <span data-ttu-id="b009a-170">Alla data tas bort om inte prenumerationen återaktiveras inom 90 dagar, eller 90 dagar plus antalet dagar mellan den tidpunkt då kontot öppnades och den första faktureringsperioden (högst 120 dagar).</span><span class="sxs-lookup"><span data-stu-id="b009a-170">All data will be deleted unless the subscription is reactivated within 90 days, or 90 days plus the number of days between the time the account was opened and the first billing period (maximum 120 days).</span></span>

<span data-ttu-id="b009a-171">När du inaktiverar en prenumeration anger  datumet under knappen Pausad när prenumerationen upphör att gälla automatiskt om du inte återaktiverar den.</span><span class="sxs-lookup"><span data-stu-id="b009a-171">When you suspend a subscription, the date you see below the **Suspended** button indicates when the subscription would automatically expire if you don't reactivate it.</span></span> 

>[!NOTE]
><span data-ttu-id="b009a-172">CSP-prenumerationer har inte en förfallen period (så som web-direct-prenumerationer gör) då tjänsterna fortfarande fungerar men prenumerationen genererar inga faktureringsavgifter.</span><span class="sxs-lookup"><span data-stu-id="b009a-172">CSP subscriptions don't have an expired period (the way web-direct subscriptions do) during which the services are still working but the subscription doesn't generate any billing charges.</span></span> <span data-ttu-id="b009a-173">CSP-prenumerationer är antingen aktiva eller inaktiverade (eller helt borttagna).</span><span class="sxs-lookup"><span data-stu-id="b009a-173">CSP subscriptions are either active or suspended (or fully deleted).</span></span>

### <a name="cancel-a-subscription"></a><span data-ttu-id="b009a-174">Avbryta en prenumeration</span><span class="sxs-lookup"><span data-stu-id="b009a-174">Cancel a subscription</span></span>

<span data-ttu-id="b009a-175">Du kan avbryta licensbaserade SaaS-prenumerationer från isv-utgivare från tredje part på den kommersiella marknadsplatsen [i Partnercenter.](csp-commercial-marketplace-overview.md)</span><span class="sxs-lookup"><span data-stu-id="b009a-175">You can cancel license-based SaaS subscriptions from third-party ISV publishers within the Partner Center [commercial marketplace](csp-commercial-marketplace-overview.md).</span></span> <span data-ttu-id="b009a-176">Så länge du avbryter inom annulleringsperioden får du en fullständig återbetalning.</span><span class="sxs-lookup"><span data-stu-id="b009a-176">As long as you cancel within the cancellation period, you will receive a full refund.</span></span>

<span data-ttu-id="b009a-177">För ISV-erbjudanden som faktureras månadsvis:</span><span class="sxs-lookup"><span data-stu-id="b009a-177">For ISV offers billed monthly:</span></span>

- <span data-ttu-id="b009a-178">Om du avbryter mindre än 24 timmar efter att du har gjort beställningen får du en fullständig kredit på nästa faktura.</span><span class="sxs-lookup"><span data-stu-id="b009a-178">If you cancel less than 24 hours after you placed the order, you will receive a full credit on the next invoice.</span></span>

- <span data-ttu-id="b009a-179">Om du avbryter senare än 24 timmar efter att du har gjort beställningen schemaläggs annulleringen att ske vid förnyelsen.</span><span class="sxs-lookup"><span data-stu-id="b009a-179">If you cancel later than 24 hours after you placed the order, the cancellation will be scheduled to occur at renewal.</span></span>

<span data-ttu-id="b009a-180">För erbjudanden som faktureras per år:</span><span class="sxs-lookup"><span data-stu-id="b009a-180">For offers billed annually:</span></span>

- <span data-ttu-id="b009a-181">Om du avbryter mindre än 14 dagar efter att du har beställt får du en fullständig kredit på nästa faktura.</span><span class="sxs-lookup"><span data-stu-id="b009a-181">If you cancel less than 14 days after you place the order, you will receive a full credit on the next invoice.</span></span>

- <span data-ttu-id="b009a-182">Om du avbryter senare än 14 dagar efter att du har beställt kommer annulleringen att schemaläggas att ske vid förnyelsen.</span><span class="sxs-lookup"><span data-stu-id="b009a-182">If you cancel later than 14 days after you place the order, the cancellation will be scheduled to occur at renewal.</span></span>

<span data-ttu-id="b009a-183">När dessa perioder är över ser du inte längre alternativet att avbryta prenumerationen.</span><span class="sxs-lookup"><span data-stu-id="b009a-183">After these periods are over, you will no longer see the option to cancel the subscription.</span></span>

> [!NOTE]
> <span data-ttu-id="b009a-184">Användningsbaserade och uppmätta ISV-tjänster från tredje part (som till exempel använder virtuella datorer eller containrar) är inte berättigade till retur.</span><span class="sxs-lookup"><span data-stu-id="b009a-184">Usage-based and metered, third-party ISV services (that use virtual machines or containers, for example) are not eligible for return.</span></span> <span data-ttu-id="b009a-185">Användningsbaserade tjänster kan avetableas som en annulleringsmetod.</span><span class="sxs-lookup"><span data-stu-id="b009a-185">Usage-based services can be de-provisioned as a cancellation method.</span></span> <span data-ttu-id="b009a-186">Eftersom avgifter debiteras efter användning är dessa tjänster inte berättigade till återbetalning.</span><span class="sxs-lookup"><span data-stu-id="b009a-186">Since charges are billed after use, these services are not eligible for a refund.</span></span>

<span data-ttu-id="b009a-187">Så här avbryter du en licensbaserad SaaS-prenumeration från en ISV-utgivare:</span><span class="sxs-lookup"><span data-stu-id="b009a-187">To cancel a license-based SaaS subscription from an ISV publisher, do the following:</span></span>

1. <span data-ttu-id="b009a-188">Logga in på instrumentpanelen i [Partnercenter.](https://partner.microsoft.com/dashboard)</span><span class="sxs-lookup"><span data-stu-id="b009a-188">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="b009a-189">I menyn i Partnercenter väljer **du Kunder** och sedan en kund i listan.</span><span class="sxs-lookup"><span data-stu-id="b009a-189">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="b009a-190">Leta upp den prenumeration som du vill avbryta.</span><span class="sxs-lookup"><span data-stu-id="b009a-190">Locate the subscription you want to cancel.</span></span>

4. <span data-ttu-id="b009a-191">I kolumnen **Status** väljer du **Avbryt**.</span><span class="sxs-lookup"><span data-stu-id="b009a-191">In the **Status** column, select **Cancel**.</span></span> <span data-ttu-id="b009a-192">**Skicka** sedan dina ändringar.</span><span class="sxs-lookup"><span data-stu-id="b009a-192">Then **Submit** your changes.</span></span>

5. <span data-ttu-id="b009a-193">Om en dialogruta visas fyller du i relevant information och väljer sedan **Skicka**.</span><span class="sxs-lookup"><span data-stu-id="b009a-193">If a dialog box appears, fill out any relevant details then select **Submit**.</span></span>

6. <span data-ttu-id="b009a-194">Bekräfta annulleringen genom att välja **Ja, avbryt**.</span><span class="sxs-lookup"><span data-stu-id="b009a-194">To confirm the cancellation, select **Yes, cancel**.</span></span>

> [!NOTE]
> <span data-ttu-id="b009a-195">Du kan också välja att avbryta en prenumeration Azure Marketplace med hjälp av API:er.</span><span class="sxs-lookup"><span data-stu-id="b009a-195">You can also choose to cancel an Azure Marketplace subscription using APIs.</span></span> <span data-ttu-id="b009a-196">Om du vill göra det kan [du läsa Avbryta en Azure Marketplace prenumeration.](/partner-center/develop/cancel-an-azure-marketplace-subscription)</span><span class="sxs-lookup"><span data-stu-id="b009a-196">To do so, see [Cancel an Azure Marketplace subscription](/partner-center/develop/cancel-an-azure-marketplace-subscription).</span></span>

### <a name="choose-whether-to-automatically-renew-a-commercial-marketplace-subscription"></a><span data-ttu-id="b009a-197">Välj om du vill förnya en prenumeration på den kommersiella marknadsplatsen automatiskt</span><span class="sxs-lookup"><span data-stu-id="b009a-197">Choose whether to automatically renew a commercial marketplace subscription</span></span>

<span data-ttu-id="b009a-198">Som standard förnyas prenumerationer automatiskt när prenumerationstiden går ut.</span><span class="sxs-lookup"><span data-stu-id="b009a-198">By default, active subscriptions are set to automatically renew when the subscription period expires.</span></span> <span data-ttu-id="b009a-199">För [prenumerationer på kommersiella marknadsplatsprodukter](csp-commercial-marketplace-overview.md)kan du välja att inte förnya prenumerationen automatiskt.</span><span class="sxs-lookup"><span data-stu-id="b009a-199">For [subscriptions to commercial marketplace products](csp-commercial-marketplace-overview.md), you can optionally choose not to automatically renew the subscription.</span></span>

<span data-ttu-id="b009a-200">Så här stoppar du en aktiv prenumeration på den kommersiella marknadsplatsen från att förnyas automatiskt:</span><span class="sxs-lookup"><span data-stu-id="b009a-200">To stop an active commercial marketplace subscription from automatically renewing:</span></span>

1. <span data-ttu-id="b009a-201">Logga in på instrumentpanelen i [Partnercenter.](https://partner.microsoft.com/dashboard)</span><span class="sxs-lookup"><span data-stu-id="b009a-201">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="b009a-202">I menyn i Partnercenter väljer **du Kunder** och sedan en kund i listan.</span><span class="sxs-lookup"><span data-stu-id="b009a-202">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="b009a-203">Välj **Prenumerationer**.</span><span class="sxs-lookup"><span data-stu-id="b009a-203">Select **Subscriptions**.</span></span> <span data-ttu-id="b009a-204">Här visas alla licensbaserade prenumerationer som du har köpt för kunden.</span><span class="sxs-lookup"><span data-stu-id="b009a-204">This lists any license-based subscriptions you have purchased for the customer.</span></span>

4. <span data-ttu-id="b009a-205">I kolumnen **Prenumeration** väljer du den prenumeration som du vill ändra.</span><span class="sxs-lookup"><span data-stu-id="b009a-205">In the **Subscription** column, select the subscription you want to modify.</span></span>

5. <span data-ttu-id="b009a-206">På sidan med prenumerationsinformation letar du **upp avsnittet Status** och **avmarkerar rutan Förnya** automatiskt.</span><span class="sxs-lookup"><span data-stu-id="b009a-206">In the subscription details page, locate the **Status** section and uncheck the **Auto-renew** box.</span></span>

6. <span data-ttu-id="b009a-207">Välj **Skicka**.</span><span class="sxs-lookup"><span data-stu-id="b009a-207">Select **Submit**.</span></span>

## <a name="next-steps"></a><span data-ttu-id="b009a-208">Nästa steg</span><span class="sxs-lookup"><span data-stu-id="b009a-208">Next steps</span></span>

- [<span data-ttu-id="b009a-209">Köpa produkter på den kommersiella marknadsplatsen för dina kunder</span><span class="sxs-lookup"><span data-stu-id="b009a-209">Purchase commercial marketplace products for your customers</span></span>](csp-commercial-marketplace-purchase.md)

- [<span data-ttu-id="b009a-210">Hantera produkter på den kommersiella marknadsplatsen för dina kunder</span><span class="sxs-lookup"><span data-stu-id="b009a-210">Manage commercial marketplace products for your customers</span></span>](csp-commercial-marketplace-manage.md)

- [<span data-ttu-id="b009a-211">Översikt över kommersiell marknadsplats</span><span class="sxs-lookup"><span data-stu-id="b009a-211">Commercial marketplace overview</span></span>](csp-commercial-marketplace-overview.md)