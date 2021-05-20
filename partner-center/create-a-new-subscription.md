---
title: Skapa kundprenumerationer i Partnercenter
ms.topic: how-to
ms.date: 05/19/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Lär dig hur du säljer prenumerationer till dina kunder för produkter som publicerats av Microsoft samt SaaS-produkter som publicerats av isv:er från tredje part.
author: BillLinzbach
ms.author: BillLi
ms.custom: SEOAPR.20
ms.localizationpriority: medium
ms.openlocfilehash: 9052954c81ef55a2bfa06778ace651c9d0f9b26f
ms.sourcegitcommit: e0444145d7720df948b9d02ae2469206db48dba5
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 05/19/2021
ms.locfileid: "110201416"
---
# <a name="create-suspend-or-cancel-customer-subscriptions"></a><span data-ttu-id="6f1e2-103">Skapa, pausa eller avbryta kundprenumerationer</span><span class="sxs-lookup"><span data-stu-id="6f1e2-103">Create, suspend, or cancel customer subscriptions</span></span>

<span data-ttu-id="6f1e2-104">**Gäller för**: Partner Center-| Partnercenter för Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="6f1e2-104">**Applies to**: Partner Center | Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="6f1e2-105">**Lämpliga roller:** Administratörsagent | Faktureringsadministratörskonto | Global | Supportagent | Försäljningsagent</span><span class="sxs-lookup"><span data-stu-id="6f1e2-105">**Appropriate roles**: Admin agent | Billing admin | Global admin | Helpdesk agent | Sales agent</span></span>

<span data-ttu-id="6f1e2-106">När du har skapat en post för kunden i Partnercenter kan du sälja dem prenumerationer till produkter i katalogen.</span><span class="sxs-lookup"><span data-stu-id="6f1e2-106">After you've created a record of your customer in the Partner Center, you can sell them subscriptions to products in the catalog.</span></span> <span data-ttu-id="6f1e2-107">Detta omfattar produkter som publicerats av Microsoft och SaaS-produkter (Software as a Service) som publicerats av oberoende programvaruleverantörer (ISV) från tredje part på den [kommersiella marknadsplatsen.](https://azuremarketplace.microsoft.com/marketplace)</span><span class="sxs-lookup"><span data-stu-id="6f1e2-107">This includes products published by Microsoft and Software as a Service (SaaS) products published by third-party Independent Software Vendors (ISVs) to the [commercial marketplace](https://azuremarketplace.microsoft.com/marketplace).</span></span>

<span data-ttu-id="6f1e2-108">Vissa erbjudanden är begränsade till en prenumeration per kund.</span><span class="sxs-lookup"><span data-stu-id="6f1e2-108">Some offers are limited to one subscription per customer.</span></span> <span data-ttu-id="6f1e2-109">Om du vill se en lista över vilka erbjudanden som är begränsade går du till sidan Priser och erbjudanden för Partnercenter.</span><span class="sxs-lookup"><span data-stu-id="6f1e2-109">To see a list of which offers are restricted, visit the Partner Center Pricing and Offers page.</span></span>

>[!IMPORTANT]
> <span data-ttu-id="6f1e2-110">Som partner i CSP-programmet kan du köpa  licensbaserade eller uppmätta SaaS-prenumerationer från **ISV-utgivare** i Partnercenter.</span><span class="sxs-lookup"><span data-stu-id="6f1e2-110">As a partner in the CSP program, you can purchase **license-based** or **metered** SaaS subscriptions from ISV publishers within Partner Center.</span></span> <span data-ttu-id="6f1e2-111">Det innebär att du kan köpa alla licensbaserade eller **uppmätta** SaaS-erbjudanden [](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) som **ISV-utgivaren** har gjort tillgängliga för dig, inklusive exklusiva erbjudanden som du har åtkomst till.</span><span class="sxs-lookup"><span data-stu-id="6f1e2-111">This means you can purchase any **license-based** or **metered** SaaS offer the ISV publisher has made available to you, including [exclusive offers](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) to which you have access.</span></span> <span data-ttu-id="6f1e2-112">Om du vill köpa eller hantera andra erbjudanden på den kommersiella marknadsplatsen från ISV:er (till exempel användningsbaserade erbjudanden som rör Azure-program, containrar eller virtuella datorer) måste du [gå till Azure Portal](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="6f1e2-112">To purchase or manage other, commercial marketplace offers from ISVs (such as usage-based offers involving Azure applications, Containers or VMs), you must go to the [Azure portal](https://portal.azure.com/).</span></span>

>[!NOTE]
><span data-ttu-id="6f1e2-113">Alla datum och tider i Partnercenter anges i utc-tidsstandarden (Universal Time Coordinated).</span><span class="sxs-lookup"><span data-stu-id="6f1e2-113">All dates and times in Partner Center are given in the Universal Time Coordinated (UTC) time standard.</span></span> <span data-ttu-id="6f1e2-114">Detta kan skilja sig med upp till 24 timmar från din lokala tid.</span><span class="sxs-lookup"><span data-stu-id="6f1e2-114">This can differ by up to 24 hours from your local time.</span></span>

## <a name="create-a-new-subscription"></a><span data-ttu-id="6f1e2-115">Skapa en ny prenumeration</span><span class="sxs-lookup"><span data-stu-id="6f1e2-115">Create a new subscription</span></span>

1. <span data-ttu-id="6f1e2-116">Logga in på [instrumentpanelen i Partnercenter](https://partner.microsoft.com/dashboard).</span><span class="sxs-lookup"><span data-stu-id="6f1e2-116">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="6f1e2-117">I menyn i Partnercenter väljer **du Kunder** och sedan en kund i listan.</span><span class="sxs-lookup"><span data-stu-id="6f1e2-117">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="6f1e2-118">Välj **Lägg till prenumeration.**</span><span class="sxs-lookup"><span data-stu-id="6f1e2-118">Select **Add subscription**.</span></span> <span data-ttu-id="6f1e2-119">På **fliken Onlinetjänster** visas alla tillgängliga SaaS-erbjudanden på Marketplace.</span><span class="sxs-lookup"><span data-stu-id="6f1e2-119">The **Online Services** tab will show all available Marketplace SaaS offers.</span></span>

4. <span data-ttu-id="6f1e2-120">Om du bara vill se vissa typer av prenumerationer gör du val i de tillgängliga filtren:</span><span class="sxs-lookup"><span data-stu-id="6f1e2-120">To see only certain types of subscriptions, make selections in the available filters:</span></span>
   - <span data-ttu-id="6f1e2-121">**Utgivare:** Välj **Microsoft om** du bara vill se erbjudanden från Microsoft eller Partner om **du vill** se produkter från den kommersiella marknadsplatsen som publicerats av ISV:er.</span><span class="sxs-lookup"><span data-stu-id="6f1e2-121">**Publisher**: Choose **Microsoft** to see only offers from Microsoft, or **Partner** to see commercial marketplace products published by ISVs.</span></span>
   - <span data-ttu-id="6f1e2-122">**Faktureringstyp:** Välj vilken typ av prenumerationsfakturering du vill använda: **Licens** eller **Användning.**</span><span class="sxs-lookup"><span data-stu-id="6f1e2-122">**Billing type**: Select the type of subscription billing you want to use: **License** or **Usage**.</span></span> <span data-ttu-id="6f1e2-123">Se [Licensbaserad fakturering för](license-based-billing.md) information som hjälper dig att välja mellan månatlig och årlig faktureringsfrekvens.</span><span class="sxs-lookup"><span data-stu-id="6f1e2-123">See [License-based billing](license-based-billing.md) for information that will help you decide between the monthly and annual billing frequency.</span></span>
   - <span data-ttu-id="6f1e2-124">**Kategori:** Välj **Företag,** **Litet företag** eller **Utvärderingsversion.**</span><span class="sxs-lookup"><span data-stu-id="6f1e2-124">**Category**: Choose **Enterprise**, **Small business**, or **Trial**.</span></span> <span data-ttu-id="6f1e2-125">Information om utvärderingsprenumerationer finns i Offer your customers trials of Microsoft products (Erbjuda [kunderna utvärderingsversioner av Microsoft-produkter).](offer-your-customers-trials-of-microsoft-products.md)</span><span class="sxs-lookup"><span data-stu-id="6f1e2-125">For info about trial subscriptions, see [Offer your customers trials of Microsoft products](offer-your-customers-trials-of-microsoft-products.md).</span></span>

5. <span data-ttu-id="6f1e2-126">Välj de produktprenumerationer som du vill köpa för din kund.</span><span class="sxs-lookup"><span data-stu-id="6f1e2-126">Select the product subscriptions you want to purchase for your customer.</span></span> <span data-ttu-id="6f1e2-127">Vilka produkter du ser beror på typen av kundsegment (utbildning, myndigheter osv.) och vilka filter du har tillämpat.</span><span class="sxs-lookup"><span data-stu-id="6f1e2-127">The products you see depend on the type of customer segment (education, government, etc.) and the filters you have applied.</span></span> <span data-ttu-id="6f1e2-128">Vissa erbjudanden som visas på Marketplace kanske inte alltid är tillgängliga för en specifik kund eller en specifik CSP-partner.</span><span class="sxs-lookup"><span data-stu-id="6f1e2-128">Some offers shown on the Marketplace may not always be available to a specific customer or a specific CSP partner.</span></span> <span data-ttu-id="6f1e2-129">Det kan vara så här:</span><span class="sxs-lookup"><span data-stu-id="6f1e2-129">This can be because:</span></span>

   - <span data-ttu-id="6f1e2-130">Kunden har redan en prenumeration på produkten och tillåts bara en</span><span class="sxs-lookup"><span data-stu-id="6f1e2-130">The customer already has a subscription to that product and is only allowed one</span></span>

   - <span data-ttu-id="6f1e2-131">Kundens prenumeration kan ha inaktiverats (I det här fallet kan du återaktivera prenumerationen i stället för att köpa en ny.)</span><span class="sxs-lookup"><span data-stu-id="6f1e2-131">The customer's subscription may have been suspended (In this case, you can reactivate the subscription rather than purchase a new one.)</span></span>

   - <span data-ttu-id="6f1e2-132">För ISV SaaS-erbjudanden kan det finnas några orsaker till varför erbjudandet inte är tillgängligt att köpa: ISV:en kanske inte stöder kundens faktureringsland eller region; ISV:en kan ha valt att inte göra erbjudandet tillgängligt via CSP-programmet, eller så kan ISV:en ha gjort erbjudandet [exklusivt](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) för vissa CSP-partner.</span><span class="sxs-lookup"><span data-stu-id="6f1e2-132">For ISV SaaS offers, there may be a few reasons why the offer is not available to purchase: The ISV may not support the customer's billing country or region; the ISV may have chosen not to make the offer available through the CSP program; or, the ISV may have made the offer [exclusive](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) to only certain CSP partners.</span></span> <span data-ttu-id="6f1e2-133">ISV-erbjudandet kanske inte heller kan göras via Partnercenter (till exempel containrar eller vissa användningsbaserade erbjudanden).</span><span class="sxs-lookup"><span data-stu-id="6f1e2-133">The ISV offer may also not be transactable through the Partner Center (for example, containers or some usage-based offers).</span></span>  

6. <span data-ttu-id="6f1e2-134">För varje prenumeration som du vill lägga till anger du antalet licenser (om det behövs) och väljer Lägg **till i kundvagn.**</span><span class="sxs-lookup"><span data-stu-id="6f1e2-134">For each subscription you want to add, enter the number of licenses (if needed) and select **Add to cart**.</span></span>

7. <span data-ttu-id="6f1e2-135">När du är klar med att lägga till prenumerationer väljer **du Granska** och granskar din beställning.</span><span class="sxs-lookup"><span data-stu-id="6f1e2-135">When you are finished adding subscriptions, select **Review** and review your order.</span></span>

8. <span data-ttu-id="6f1e2-136">När du har granskat dina beställningar och är redo att köpa prenumerationerna väljer du **Köp.**</span><span class="sxs-lookup"><span data-stu-id="6f1e2-136">Once you've reviewed your orders and are ready to purchase these subscriptions, select **Buy**.</span></span>

9. <span data-ttu-id="6f1e2-137">När du har köpt en prenumeration för en kund sker följande:</span><span class="sxs-lookup"><span data-stu-id="6f1e2-137">After you buy a subscription for a customer, the following will occur:</span></span>

    - <span data-ttu-id="6f1e2-138">Du kan granska eller redigera prenumerationen genom att välja prenumerationsnamnet på kundens **prenumerationssida.**</span><span class="sxs-lookup"><span data-stu-id="6f1e2-138">You can review or edit the subscription by selecting the subscription name from that customer's **Subscriptions** page.</span></span> <span data-ttu-id="6f1e2-139">Härifrån kan du välja tilläggslicenser om det finns några, ändra antalet licenser eller pausa prenumerationen.</span><span class="sxs-lookup"><span data-stu-id="6f1e2-139">From here, you can select add-on licenses if any are available, change the quantity of licenses, or suspend the subscription.</span></span>

    <span data-ttu-id="6f1e2-140">**För ISV SaaS-prenumerationer (licensbaserade och uppmätta):**</span><span class="sxs-lookup"><span data-stu-id="6f1e2-140">**For ISV SaaS (license-based and metered) subscriptions:**</span></span>
    - <span data-ttu-id="6f1e2-141">Du får en länk till ISV-utgivarens webbplats.</span><span class="sxs-lookup"><span data-stu-id="6f1e2-141">You will receive a link to the ISV publisher's site.</span></span> <span data-ttu-id="6f1e2-142">Den här länken hjälper dig att slutföra distributionen eller kontokonfigurationen av kundens prenumeration.</span><span class="sxs-lookup"><span data-stu-id="6f1e2-142">This link should help you complete the deployment or account setup of the customer's subscription.</span></span>
      
    >[!NOTE]
    > <span data-ttu-id="6f1e2-143">Varken du eller kunden får ett e-postmeddelande med instruktioner för att slutföra kontouppsättningen/etableringen för den här typen av ISV-prenumeration.)</span><span class="sxs-lookup"><span data-stu-id="6f1e2-143">Neither you nor your customer will receive an email with instructions to complete account set up/provisioning for this type of ISV subscription.)</span></span>

    - <span data-ttu-id="6f1e2-144">Om din prenumeration har en 30-dagars kostnadsfri utvärderingsversion tillämpas den kostnadsfria utvärderingsperioden automatiskt.</span><span class="sxs-lookup"><span data-stu-id="6f1e2-144">If your subscription comes with a 30-day free trial, the free trial period will be applied automatically.</span></span> <span data-ttu-id="6f1e2-145">Som partner i CSP-programmet kan du inte undanta den kostnadsfria utvärderingsperioden för erbjudanden som du köper till kunder.</span><span class="sxs-lookup"><span data-stu-id="6f1e2-145">As a partner in the CSP program, you cannot waive the free trial period on offers you purchase for customers.</span></span> <span data-ttu-id="6f1e2-146">När den kostnadsfria utvärderingsperioden har avslutats börjar prenumerationsperioden och prenumerationen konverteras till betald status.</span><span class="sxs-lookup"><span data-stu-id="6f1e2-146">Once the free trial period ends, the subscription term will begin and the subscription will convert to paid status.</span></span> <span data-ttu-id="6f1e2-147">Prenumerationen förnyas sedan automatiskt enligt samma schema.</span><span class="sxs-lookup"><span data-stu-id="6f1e2-147">The subscription will then auto-renew according to the same schedule.</span></span>
   
## <a name="update-subscriptions-with-add-ons"></a><span data-ttu-id="6f1e2-148">Uppdatera prenumerationer med tillägg</span><span class="sxs-lookup"><span data-stu-id="6f1e2-148">Update subscriptions with add-ons</span></span> 

<span data-ttu-id="6f1e2-149">För att kunna köpa ett tillägg måste kunden först ha en aktiv basprenumeration.</span><span class="sxs-lookup"><span data-stu-id="6f1e2-149">To purchase an add-on, the customer must first have an active base subscription.</span></span>  <span data-ttu-id="6f1e2-150">Det går inte att köpa tillägg via katalogen.</span><span class="sxs-lookup"><span data-stu-id="6f1e2-150">You can't purchase add-ons through the catalog.</span></span>

1. <span data-ttu-id="6f1e2-151">Logga in på instrumentpanelen i [Partnercenter.](https://partner.microsoft.com/dashboard)</span><span class="sxs-lookup"><span data-stu-id="6f1e2-151">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="6f1e2-152">I menyn i Partnercenter väljer **du Kunder** och sedan en kund i listan.</span><span class="sxs-lookup"><span data-stu-id="6f1e2-152">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="6f1e2-153">Välj den prenumeration som du vill hantera.</span><span class="sxs-lookup"><span data-stu-id="6f1e2-153">Choose the subscription you want to manage.</span></span>

4. <span data-ttu-id="6f1e2-154">Under **avsnittet Status** finns en lista över tillgängliga tillägg för prenumerationen.</span><span class="sxs-lookup"><span data-stu-id="6f1e2-154">Below the **Status** section, are a list of available Add-ons for the subscription.</span></span>  

5. <span data-ttu-id="6f1e2-155">Uppdatera antalet licenser för varje nödvändigt tillägg.</span><span class="sxs-lookup"><span data-stu-id="6f1e2-155">Update the quantity of licenses for each required Add-on.</span></span> <span data-ttu-id="6f1e2-156">**Skicka** sedan dina ändringar.</span><span class="sxs-lookup"><span data-stu-id="6f1e2-156">Then **Submit** your changes.</span></span>

<span data-ttu-id="6f1e2-157">Möjligheten att köpa tillägg via Partnercenter är endast tillgänglig för direkta fakturerade och indirekta leverantörer.</span><span class="sxs-lookup"><span data-stu-id="6f1e2-157">The ability to purchase add-ons through Partner Center is only available to direct bill and indirect providers.</span></span>
<span data-ttu-id="6f1e2-158">Endast berättigade tillägg visas baserat på grundkraven och regional tillgänglighet.</span><span class="sxs-lookup"><span data-stu-id="6f1e2-158">Only eligible add-ons are displayed based on the base requirements and regional availability.</span></span> <span data-ttu-id="6f1e2-159">Mer information om priser och erbjudanden finns i erbjudandematrisen för molnåterförsäljare.</span><span class="sxs-lookup"><span data-stu-id="6f1e2-159">For more information about pricing and offers, refer to the Cloud Reseller offer matrix.</span></span> <span data-ttu-id="6f1e2-160">Om du avbryter basprenumerationen inaktiveras även eventuella associerade tillägg.</span><span class="sxs-lookup"><span data-stu-id="6f1e2-160">Suspending the base subscription will also suspend any associated add-ons.</span></span>

<span data-ttu-id="6f1e2-161">Startdatumen för tillägg följer basprenumerationen och avgifterna beräknas utifrån startdatumet för debitering och slutdatumet för debitering med proportionella avgifter på den första fakturan.</span><span class="sxs-lookup"><span data-stu-id="6f1e2-161">Start dates for add-ons align to the base subscription and charges are calculated from the Charge start date and Charge end date with pro-rata charges in the first invoice.</span></span> <span data-ttu-id="6f1e2-162">Mer information finns i [Licensbaserad fakturering.](license-based-billing.md)</span><span class="sxs-lookup"><span data-stu-id="6f1e2-162">For additional information see, [License-based billing](license-based-billing.md).</span></span>


## <a name="suspend-or-cancel-a-subscription"></a><span data-ttu-id="6f1e2-163">Pausa eller avbryta en prenumeration</span><span class="sxs-lookup"><span data-stu-id="6f1e2-163">Suspend or cancel a subscription</span></span>

<span data-ttu-id="6f1e2-164">Partner kan inaktivera eller avbryta en prenumeration om det begärs av kunden, eller i fall av utebliven betalning eller bedrägeri.</span><span class="sxs-lookup"><span data-stu-id="6f1e2-164">Partners can suspend or cancel a subscription if requested by the customer, or in cases of nonpayment or fraud.</span></span>

### <a name="suspend-a-subscription"></a><span data-ttu-id="6f1e2-165">Inaktivera en prenumeration</span><span class="sxs-lookup"><span data-stu-id="6f1e2-165">Suspend a subscription</span></span>

<span data-ttu-id="6f1e2-166">När du ändrar statusen för en prenumeration **till Inaktiverad** kan användarna inte logga in eller komma åt tjänster.</span><span class="sxs-lookup"><span data-stu-id="6f1e2-166">When you change the status of a subscription to **Suspended**, users are not able to sign in or access services.</span></span>

1. <span data-ttu-id="6f1e2-167">Logga in på instrumentpanelen i [Partnercenter.](https://partner.microsoft.com/dashboard)</span><span class="sxs-lookup"><span data-stu-id="6f1e2-167">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="6f1e2-168">I menyn i Partnercenter väljer **du Kunder** och sedan en kund i listan.</span><span class="sxs-lookup"><span data-stu-id="6f1e2-168">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="6f1e2-169">Välj den prenumeration som du vill hantera.</span><span class="sxs-lookup"><span data-stu-id="6f1e2-169">Choose the subscription you want to manage.</span></span>

4. <span data-ttu-id="6f1e2-170">I avsnittet **Status** väljer du **Tillfälligt avbruten**.</span><span class="sxs-lookup"><span data-stu-id="6f1e2-170">In the **Status** section, choose **Suspended**.</span></span> <span data-ttu-id="6f1e2-171">**Skicka** sedan dina ändringar.</span><span class="sxs-lookup"><span data-stu-id="6f1e2-171">Then **Submit** your changes.</span></span>

5. <span data-ttu-id="6f1e2-172">Alla data tas bort om inte prenumerationen återaktiveras inom 90 dagar, eller 90 dagar plus antalet dagar mellan den tidpunkt då kontot öppnades och den första faktureringsperioden (högst 120 dagar).</span><span class="sxs-lookup"><span data-stu-id="6f1e2-172">All data will be deleted unless the subscription is reactivated within 90 days, or 90 days plus the number of days between the time the account was opened and the first billing period (maximum 120 days).</span></span>

<span data-ttu-id="6f1e2-173">När du pausar en prenumeration anger  det datum som visas under knappen Pausad när prenumerationen upphör att gälla automatiskt om du inte återaktiverar den.</span><span class="sxs-lookup"><span data-stu-id="6f1e2-173">When you suspend a subscription, the date you see below the **Suspended** button indicates when the subscription would automatically expire if you don't reactivate it.</span></span> 

>[!NOTE]
><span data-ttu-id="6f1e2-174">CSP-prenumerationer har inte någon utgången period (så som web-direct-prenumerationer gör) när tjänsterna fortfarande fungerar men prenumerationen genererar inga faktureringsavgifter.</span><span class="sxs-lookup"><span data-stu-id="6f1e2-174">CSP subscriptions don't have an expired period (the way web-direct subscriptions do) during which the services are still working but the subscription doesn't generate any billing charges.</span></span> <span data-ttu-id="6f1e2-175">CSP-prenumerationer är antingen aktiva eller inaktiverade (eller helt borttagna).</span><span class="sxs-lookup"><span data-stu-id="6f1e2-175">CSP subscriptions are either active or suspended (or fully deleted).</span></span>

### <a name="cancel-a-subscription"></a><span data-ttu-id="6f1e2-176">Avbryta en prenumeration</span><span class="sxs-lookup"><span data-stu-id="6f1e2-176">Cancel a subscription</span></span>

<span data-ttu-id="6f1e2-177">Du kan avbryta licensbaserade SaaS-prenumerationer från tredjeparts-ISV-utgivare på den kommersiella marknadsplatsen [i Partnercenter.](csp-commercial-marketplace-overview.md)</span><span class="sxs-lookup"><span data-stu-id="6f1e2-177">You can cancel license-based SaaS subscriptions from third-party ISV publishers within the Partner Center [commercial marketplace](csp-commercial-marketplace-overview.md).</span></span> <span data-ttu-id="6f1e2-178">Så länge du avbryter inom annulleringsperioden får du en fullständig återbetalning.</span><span class="sxs-lookup"><span data-stu-id="6f1e2-178">As long as you cancel within the cancellation period, you will receive a full refund.</span></span>

<span data-ttu-id="6f1e2-179">För ISV-erbjudanden som faktureras månadsvis:</span><span class="sxs-lookup"><span data-stu-id="6f1e2-179">For ISV offers billed monthly:</span></span>

- <span data-ttu-id="6f1e2-180">Om du avbryter mindre än 24 timmar efter att du har gjort beställningen får du en fullständig kredit på nästa faktura.</span><span class="sxs-lookup"><span data-stu-id="6f1e2-180">If you cancel less than 24 hours after you placed the order, you will receive a full credit on the next invoice.</span></span>

- <span data-ttu-id="6f1e2-181">Om du avbryter senare än 24 timmar efter att du har gjort beställningen schemaläggs annulleringen att ske vid förnyelsen.</span><span class="sxs-lookup"><span data-stu-id="6f1e2-181">If you cancel later than 24 hours after you placed the order, the cancellation will be scheduled to occur at renewal.</span></span>

<span data-ttu-id="6f1e2-182">För erbjudanden som faktureras per år:</span><span class="sxs-lookup"><span data-stu-id="6f1e2-182">For offers billed annually:</span></span>

- <span data-ttu-id="6f1e2-183">Om du avbryter mindre än 14 dagar efter att du har beställt får du en fullständig kredit på nästa faktura.</span><span class="sxs-lookup"><span data-stu-id="6f1e2-183">If you cancel less than 14 days after you place the order, you will receive a full credit on the next invoice.</span></span>

- <span data-ttu-id="6f1e2-184">Om du avbryter senare än 14 dagar efter att du har beställt kommer annulleringen att ske vid förnyelsen.</span><span class="sxs-lookup"><span data-stu-id="6f1e2-184">If you cancel later than 14 days after you place the order, the cancellation will be scheduled to occur at renewal.</span></span>

<span data-ttu-id="6f1e2-185">När dessa perioder är över visas inte längre alternativet att avbryta prenumerationen.</span><span class="sxs-lookup"><span data-stu-id="6f1e2-185">After these periods are over, you will no longer see the option to cancel the subscription.</span></span>

> [!NOTE]
> <span data-ttu-id="6f1e2-186">Användningsbaserade och uppmätta ISV-tjänster från tredje part (som till exempel använder virtuella datorer eller containrar) är inte berättigade till retur.</span><span class="sxs-lookup"><span data-stu-id="6f1e2-186">Usage-based and metered, third-party ISV services (that use virtual machines or containers, for example) are not eligible for return.</span></span> <span data-ttu-id="6f1e2-187">Användningsbaserade tjänster kan avetableas som en annulleringsmetod.</span><span class="sxs-lookup"><span data-stu-id="6f1e2-187">Usage-based services can be de-provisioned as a cancellation method.</span></span> <span data-ttu-id="6f1e2-188">Eftersom avgifter debiteras efter användning är dessa tjänster inte berättigade till återbetalning.</span><span class="sxs-lookup"><span data-stu-id="6f1e2-188">Since charges are billed after use, these services are not eligible for a refund.</span></span>

<span data-ttu-id="6f1e2-189">Så här avbryter du en licensbaserad SaaS-prenumeration från en ISV-utgivare:</span><span class="sxs-lookup"><span data-stu-id="6f1e2-189">To cancel a license-based SaaS subscription from an ISV publisher, do the following:</span></span>

1. <span data-ttu-id="6f1e2-190">Logga in på instrumentpanelen i [Partnercenter.](https://partner.microsoft.com/dashboard)</span><span class="sxs-lookup"><span data-stu-id="6f1e2-190">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="6f1e2-191">I menyn i Partnercenter väljer **du Kunder** och sedan en kund i listan.</span><span class="sxs-lookup"><span data-stu-id="6f1e2-191">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="6f1e2-192">Leta upp den prenumeration som du vill avbryta.</span><span class="sxs-lookup"><span data-stu-id="6f1e2-192">Locate the subscription you want to cancel.</span></span>

4. <span data-ttu-id="6f1e2-193">I kolumnen **Status** väljer du **Avbryt.**</span><span class="sxs-lookup"><span data-stu-id="6f1e2-193">In the **Status** column, select **Cancel**.</span></span> <span data-ttu-id="6f1e2-194">**Skicka** sedan dina ändringar.</span><span class="sxs-lookup"><span data-stu-id="6f1e2-194">Then **Submit** your changes.</span></span>

5. <span data-ttu-id="6f1e2-195">Om en dialogruta visas fyller du i relevant information och väljer sedan **Skicka**.</span><span class="sxs-lookup"><span data-stu-id="6f1e2-195">If a dialog box appears, fill out any relevant details then select **Submit**.</span></span>

6. <span data-ttu-id="6f1e2-196">Bekräfta annulleringen genom att välja **Ja, avbryt**.</span><span class="sxs-lookup"><span data-stu-id="6f1e2-196">To confirm the cancellation, select **Yes, cancel**.</span></span>

> [!NOTE]
> <span data-ttu-id="6f1e2-197">Du kan också välja att avbryta en prenumeration Azure Marketplace med hjälp av API:er.</span><span class="sxs-lookup"><span data-stu-id="6f1e2-197">You can also choose to cancel an Azure Marketplace subscription using APIs.</span></span> <span data-ttu-id="6f1e2-198">Det gör du genom att läsa [Avbryt en Azure Marketplace prenumeration.](/partner-center/develop/cancel-an-azure-marketplace-subscription)</span><span class="sxs-lookup"><span data-stu-id="6f1e2-198">To do so, see [Cancel an Azure Marketplace subscription](/partner-center/develop/cancel-an-azure-marketplace-subscription).</span></span>

### <a name="choose-whether-to-automatically-renew-a-commercial-marketplace-subscription"></a><span data-ttu-id="6f1e2-199">Välj om du vill förnya en prenumeration på den kommersiella marknadsplatsen automatiskt</span><span class="sxs-lookup"><span data-stu-id="6f1e2-199">Choose whether to automatically renew a commercial marketplace subscription</span></span>

<span data-ttu-id="6f1e2-200">Som standard förnyas prenumerationer automatiskt när prenumerationstiden går ut.</span><span class="sxs-lookup"><span data-stu-id="6f1e2-200">By default, active subscriptions are set to automatically renew when the subscription period expires.</span></span> <span data-ttu-id="6f1e2-201">För [prenumerationer på produkter på den kommersiella](csp-commercial-marketplace-overview.md)marknadsplatsen kan du välja att inte förnya prenumerationen automatiskt.</span><span class="sxs-lookup"><span data-stu-id="6f1e2-201">For [subscriptions to commercial marketplace products](csp-commercial-marketplace-overview.md), you can optionally choose not to automatically renew the subscription.</span></span>

<span data-ttu-id="6f1e2-202">Så här stoppar du en aktiv prenumeration på den kommersiella marknadsplatsen från att förnyas automatiskt:</span><span class="sxs-lookup"><span data-stu-id="6f1e2-202">To stop an active commercial marketplace subscription from automatically renewing:</span></span>

1. <span data-ttu-id="6f1e2-203">Logga in på instrumentpanelen i [Partnercenter.](https://partner.microsoft.com/dashboard)</span><span class="sxs-lookup"><span data-stu-id="6f1e2-203">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="6f1e2-204">I menyn i Partnercenter väljer **du Kunder** och sedan en kund i listan.</span><span class="sxs-lookup"><span data-stu-id="6f1e2-204">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="6f1e2-205">Välj **Prenumerationer**.</span><span class="sxs-lookup"><span data-stu-id="6f1e2-205">Select **Subscriptions**.</span></span> <span data-ttu-id="6f1e2-206">Här visas alla licensbaserade prenumerationer som du har köpt för kunden.</span><span class="sxs-lookup"><span data-stu-id="6f1e2-206">This lists any license-based subscriptions you have purchased for the customer.</span></span>

4. <span data-ttu-id="6f1e2-207">I kolumnen **Prenumeration** väljer du den prenumeration som du vill ändra.</span><span class="sxs-lookup"><span data-stu-id="6f1e2-207">In the **Subscription** column, select the subscription you want to modify.</span></span>

5. <span data-ttu-id="6f1e2-208">På sidan med prenumerationsinformation letar du upp **avsnittet Status** och **avmarkerar rutan Förnya** automatiskt.</span><span class="sxs-lookup"><span data-stu-id="6f1e2-208">In the subscription details page, locate the **Status** section and uncheck the **Auto-renew** box.</span></span>

6. <span data-ttu-id="6f1e2-209">Välj **Skicka**.</span><span class="sxs-lookup"><span data-stu-id="6f1e2-209">Select **Submit**.</span></span>

## <a name="next-steps"></a><span data-ttu-id="6f1e2-210">Nästa steg</span><span class="sxs-lookup"><span data-stu-id="6f1e2-210">Next steps</span></span>

- [<span data-ttu-id="6f1e2-211">Köpa produkter på den kommersiella marknadsplatsen för dina kunder</span><span class="sxs-lookup"><span data-stu-id="6f1e2-211">Purchase commercial marketplace products for your customers</span></span>](csp-commercial-marketplace-purchase.md)

- [<span data-ttu-id="6f1e2-212">Hantera produkter på den kommersiella marknadsplatsen för dina kunder</span><span class="sxs-lookup"><span data-stu-id="6f1e2-212">Manage commercial marketplace products for your customers</span></span>](csp-commercial-marketplace-manage.md)

- [<span data-ttu-id="6f1e2-213">Översikt över kommersiell marknadsplats</span><span class="sxs-lookup"><span data-stu-id="6f1e2-213">Commercial marketplace overview</span></span>](csp-commercial-marketplace-overview.md)