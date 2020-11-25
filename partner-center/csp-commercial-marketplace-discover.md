---
title: Upptäck erbjudanden – kommersiell marknads plats
ms.topic: article
ms.date: 05/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Lär dig hur CSP-partner kan använda Partner Center för att visa eller söka i Marketplace efter SaaS erbjudanden eller priser från oberoende program varu leverantörer (ISV).
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: e89473cf095be4cc87c96f1c2a6d0da224eccedd
ms.sourcegitcommit: f34f2f69e6df4f260479a205d94010cf47987ff2
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 11/25/2020
ms.locfileid: "96038869"
---
# <a name="discover-offers-and-pricing-in-partner-center-commercial-marketplace"></a><span data-ttu-id="3222a-103">Identifiera erbjudanden och priser i Partner Center kommersiell marknads plats</span><span class="sxs-lookup"><span data-stu-id="3222a-103">Discover offers and pricing in Partner Center commercial marketplace</span></span>

<span data-ttu-id="3222a-104">**Gäller för**</span><span class="sxs-lookup"><span data-stu-id="3222a-104">**Applies to**</span></span>

- <span data-ttu-id="3222a-105">Partnercenter</span><span class="sxs-lookup"><span data-stu-id="3222a-105">Partner Center</span></span>
- <span data-ttu-id="3222a-106">Partner i CSP-programmet</span><span class="sxs-lookup"><span data-stu-id="3222a-106">Partners in the CSP program</span></span>

<span data-ttu-id="3222a-107">**Lämpliga roller**</span><span class="sxs-lookup"><span data-stu-id="3222a-107">**Appropriate roles**</span></span>

- <span data-ttu-id="3222a-108">Global administratör</span><span class="sxs-lookup"><span data-stu-id="3222a-108">Global admin</span></span>
- <span data-ttu-id="3222a-109">Administratörs agent</span><span class="sxs-lookup"><span data-stu-id="3222a-109">Admin agent</span></span>

<span data-ttu-id="3222a-110">När oberoende program varu leverantörer (ISV) väljer att publicera ett erbjudande i den kommersiella marknads platsen kan de också avgöra om de vill att erbjudandet ska göras tillgängligt i CSP-programmet.</span><span class="sxs-lookup"><span data-stu-id="3222a-110">When Independent Software Vendors (ISVs) choose to publish an offer in the commercial marketplace, they can also decide if they want the offer to be made available in the CSP program.</span></span> <span data-ttu-id="3222a-111">Om de väljer att sälja erbjudandet via CSP-programmet bör CSP-partners se erbjudandet i Partner Center Marketplace-avsnittet.</span><span class="sxs-lookup"><span data-stu-id="3222a-111">If they choose to sell the offer through the CSP program, CSP partners should see the offer in Partner Center Marketplace area.</span></span>

<span data-ttu-id="3222a-112">Om ett ISV-erbjudande inte visas som du förväntar dig i Partner Center kan det bero på att:</span><span class="sxs-lookup"><span data-stu-id="3222a-112">If an ISV offer does not appear as you expect in Partner Center, it may be because:</span></span>

- <span data-ttu-id="3222a-113">ISV valde att inte sälja erbjudandet via CSP-programmet.</span><span class="sxs-lookup"><span data-stu-id="3222a-113">The ISV decided not to sell the offer through the CSP program.</span></span> <span data-ttu-id="3222a-114">Vissa ISV-produkter kan till exempel ha gjorts tillgängliga i andra områden av den kommersiella marknads platsen (till exempel i [Microsoft AppSource](https://appsource.microsoft.com/) och [Azure Marketplace](https://azuremarketplace.microsoft.com/)), men de visas inte för partner i CSP-programmet på Partner Center Marketplace.</span><span class="sxs-lookup"><span data-stu-id="3222a-114">For example, some ISV products may have been made available in other areas of the commercial marketplace (such as in [Microsoft AppSource](https://appsource.microsoft.com/) and [Azure Marketplace](https://azuremarketplace.microsoft.com/)), but may not appear for partners in the CSP program in Partner Center marketplace.</span></span>

- <span data-ttu-id="3222a-115">ISV valde att göra erbjudandet exklusivt till endast ett SELECT-antal CSP-partner.</span><span class="sxs-lookup"><span data-stu-id="3222a-115">The ISV decided to make the offer exclusive to only a select number of CSP partners.</span></span> <span data-ttu-id="3222a-116">Mer information om exklusiva erbjudanden finns längre fram i det här hjälp avsnittet.</span><span class="sxs-lookup"><span data-stu-id="3222a-116">For more information about exclusive offers, see later in this help topic.</span></span>

- <span data-ttu-id="3222a-117">Erbjudande typen kanske inte går att använda i ett läge genom Partner Center eller Azure Portal (t. ex. behållare eller vissa användnings erbjudanden).</span><span class="sxs-lookup"><span data-stu-id="3222a-117">The offer type may not be transactable through Partner Center or Azure portal (e.g. Containers or some usage-based offers).</span></span>

- <span data-ttu-id="3222a-118">Fakturerings landet för dina associerade kunder kanske inte stöds för det här ISV-erbjudandet.</span><span class="sxs-lookup"><span data-stu-id="3222a-118">The billing country of your associated customer(s) may not be supported for this ISV offer.</span></span>

## <a name="view-marketplace-offers-in-partner-center"></a><span data-ttu-id="3222a-119">Visa Marketplace-erbjudanden i Partner Center</span><span class="sxs-lookup"><span data-stu-id="3222a-119">View Marketplace offers in Partner Center</span></span>

<span data-ttu-id="3222a-120">För att visa tillgängliga kommersiella Marketplace-erbjudanden i CSP-programmet:</span><span class="sxs-lookup"><span data-stu-id="3222a-120">To view available commercial marketplace offers in the CSP program:</span></span>

1. <span data-ttu-id="3222a-121">Logga in på Partner Center- [instrumentpanelen](https://partner.microsoft.com/dashboard)och välj **CSP** i den vänstra navigerings menyn.</span><span class="sxs-lookup"><span data-stu-id="3222a-121">Sign into Partner Center [dashboard](https://partner.microsoft.com/dashboard), then select **CSP** from the left navigation menu.</span></span>

2. <span data-ttu-id="3222a-122">Välj **Sälj**, följt av **Marketplace**.</span><span class="sxs-lookup"><span data-stu-id="3222a-122">Select **Sell**, followed by **Marketplace**.</span></span> <span data-ttu-id="3222a-123">Som standard visas produkter av alla typer och kategorier.</span><span class="sxs-lookup"><span data-stu-id="3222a-123">By default, you will see products of all types and categories.</span></span>

3. <span data-ttu-id="3222a-124">Välj ett filter efter typ eller kategori.</span><span class="sxs-lookup"><span data-stu-id="3222a-124">Select a filter by type or category.</span></span> <span data-ttu-id="3222a-125">Du kan också använda **Sök** för att hitta vissa nyckelord, erbjudande namn eller namn på ISV-utgivare.</span><span class="sxs-lookup"><span data-stu-id="3222a-125">You can also use **Search** to find specific keywords, offer names or the names of ISV publishers.</span></span>

4. <span data-ttu-id="3222a-126">Välj ett enskilt produkt erbjudande i listan.</span><span class="sxs-lookup"><span data-stu-id="3222a-126">Select a specific product offer from the list.</span></span> <span data-ttu-id="3222a-127">Detta tar dig till en produkt översikts flik där du kan lära dig mer om erbjudandet.</span><span class="sxs-lookup"><span data-stu-id="3222a-127">This will take you to a product Overview tab where you can learn more about the offer.</span></span> <span data-ttu-id="3222a-128">Informationen på den här fliken kan vara:</span><span class="sxs-lookup"><span data-stu-id="3222a-128">Information on this tab might include:</span></span> 

    - <span data-ttu-id="3222a-129">En beskrivning av produkten eller erbjudandet</span><span class="sxs-lookup"><span data-stu-id="3222a-129">A description of the product or offer</span></span>

    - <span data-ttu-id="3222a-130">Mer information om ISV-utgivaren</span><span class="sxs-lookup"><span data-stu-id="3222a-130">More information about the ISV publisher</span></span>

    - <span data-ttu-id="3222a-131">Länkar till dokumentation eller marknadsförings material som laddas upp av ISV-utgivaren</span><span class="sxs-lookup"><span data-stu-id="3222a-131">Links to documentation or marketing materials uploaded by the ISV publisher</span></span>

    - <span data-ttu-id="3222a-132">Andra möjliga ISV-kontakter för kund support, teknik eller en kontakt för CSP-programmet</span><span class="sxs-lookup"><span data-stu-id="3222a-132">Other possible ISV contacts for customer support, engineering, or a contact for the CSP program</span></span>

5. <span data-ttu-id="3222a-133">Om du vill se mer information om erbjudanden, SKU: er eller priser för erbjudandet väljer du fliken **abonnemang + prissättning** . På den här fliken visas:</span><span class="sxs-lookup"><span data-stu-id="3222a-133">To see more information about an offer's available plans, SKUs, or pricing, select the **Plans + Pricing** tab. This tab will show you:</span></span>

    - <span data-ttu-id="3222a-134">De marknader där det här erbjudandet är tillgängligt för dig</span><span class="sxs-lookup"><span data-stu-id="3222a-134">The markets where this offer is available to you</span></span>

    - <span data-ttu-id="3222a-135">En lista över SKU: er eller planer som är tillgängliga för erbjudandet</span><span class="sxs-lookup"><span data-stu-id="3222a-135">A list of SKUs or plans available for the offer</span></span>

    - <span data-ttu-id="3222a-136">Prissättning för varje SKU eller abonnemang som är tillgängligt</span><span class="sxs-lookup"><span data-stu-id="3222a-136">Pricing for each SKU or Plan available</span></span>

## <a name="view-marketplace-offers-via-partner-center-apis"></a><span data-ttu-id="3222a-137">Visa Marketplace-erbjudanden via API: er för partner Center</span><span class="sxs-lookup"><span data-stu-id="3222a-137">View Marketplace offers via Partner Center APIs</span></span>

<span data-ttu-id="3222a-138">CSP-programpartner kan också använda API: er för att returnera en lista över berättigade erbjudanden.</span><span class="sxs-lookup"><span data-stu-id="3222a-138">CSP program partners can also use APIs to return a list of eligible offers.</span></span> <span data-ttu-id="3222a-139">Berättigade erbjudanden är bara de SaaS ISV-erbjudanden som är tillgängliga för partnern att sälja via partner Center Marketplace.</span><span class="sxs-lookup"><span data-stu-id="3222a-139">Eligible offers will be only those SaaS ISV offers available for the partner to sell via Partner Center marketplace.</span></span> <span data-ttu-id="3222a-140">För partner som använder API: er för att identifiera erbjudanden i katalogen, se rikt linjerna för att [få en lista över erbjudanden för en marknad](/partner-center/develop/create-subscription-azure-marketplace-products#get-a-list-of-offers-for-a-market).</span><span class="sxs-lookup"><span data-stu-id="3222a-140">For partners using APIs to identify offers in the catalog, refer to the guidance to [obtain a list of offers for a market](/partner-center/develop/create-subscription-azure-marketplace-products#get-a-list-of-offers-for-a-market).</span></span>

## <a name="view-the-latest-marketplace-offer-pricing-in-partner-center"></a><span data-ttu-id="3222a-141">Visa den senaste prissättningen för Marketplace i Partner Center</span><span class="sxs-lookup"><span data-stu-id="3222a-141">View the latest Marketplace offer pricing in Partner Center</span></span>

<span data-ttu-id="3222a-142">Följ de här stegen för de senaste pris uppgifter som är associerade med ett erbjudande:</span><span class="sxs-lookup"><span data-stu-id="3222a-142">Follow these steps for the latest pricing details associated with an offer:</span></span>

1. <span data-ttu-id="3222a-143">Logga in på Partner Center- [instrumentpanelen](https://partner.microsoft.com/dashboard)och välj **CSP** i den vänstra navigerings menyn.</span><span class="sxs-lookup"><span data-stu-id="3222a-143">Sign into Partner Center [dashboard](https://partner.microsoft.com/dashboard), then select **CSP** from the left navigation menu.</span></span>

2. <span data-ttu-id="3222a-144">Välj **försäljning** följt av **priser och erbjudanden**.</span><span class="sxs-lookup"><span data-stu-id="3222a-144">Select **Sell**, followed by **Pricing and offers**.</span></span>

3. <span data-ttu-id="3222a-145">Rulla ned till **Marketplace** -avsnittet, Välj en plats och ladda ned **Marketplace-priser**.</span><span class="sxs-lookup"><span data-stu-id="3222a-145">Scroll down to the **Marketplace** section, select a location and download **Marketplace pricing**.</span></span> <span data-ttu-id="3222a-146">Detta genererar ett kalkyl blad med de senaste pris uppgifterna för SaaS, licensbaserade erbjudanden och avgiftsbelagda erbjudanden som är tillgängliga från ISV-utgivare.</span><span class="sxs-lookup"><span data-stu-id="3222a-146">This generates a spreadsheet with the latest pricing data for SaaS, license-based offers and metered offers available from ISV publishers.</span></span> <span data-ttu-id="3222a-147">Vissa priser för Azure-program kan också visas här.</span><span class="sxs-lookup"><span data-stu-id="3222a-147">Some Azure application pricing may also appear here.</span></span> <span data-ttu-id="3222a-148">Den här informationen uppdateras varje dag, så du kan kontrol lera den efter aktuella priser så ofta som du väljer.</span><span class="sxs-lookup"><span data-stu-id="3222a-148">This information is updated daily, so you can check it for current prices as often as you choose.</span></span>

4. <span data-ttu-id="3222a-149">Om en ISV-produkt innehåller en kostnads fri utvärderings period visar kalkyl bladet två rader för produkten:</span><span class="sxs-lookup"><span data-stu-id="3222a-149">If an ISV product includes a free trial period, the spreadsheet will display two rows for that product:</span></span>

    - <span data-ttu-id="3222a-150">En rad visar den kostnads fria utvärderings versionen på noll.</span><span class="sxs-lookup"><span data-stu-id="3222a-150">One row shows the free trial price of zero.</span></span> <span data-ttu-id="3222a-151">Det innebär att en kostnads fri utvärderings period är tillgänglig.</span><span class="sxs-lookup"><span data-stu-id="3222a-151">This means a free trial period is available.</span></span>

    - <span data-ttu-id="3222a-152">Den andra raden visar priset och villkoren som ska gälla när den kostnads fria utvärderings perioden är över.</span><span class="sxs-lookup"><span data-stu-id="3222a-152">The other row shows the price and terms that will apply after the free trial period is over.</span></span>

<span data-ttu-id="3222a-153">Som CSP-programpartner kan du vara berättigad till andra incitament som är kopplade till vissa kommersiella Marketplace-erbjudanden.</span><span class="sxs-lookup"><span data-stu-id="3222a-153">As a CSP program partner, you may be eligible for other incentives associated with certain commercial marketplace offers.</span></span> <span data-ttu-id="3222a-154">Mer information om andra incitament finns i [stimulans guiden för CSP](https://aka.ms/partnerincentives) (kräver CSP-inloggning).</span><span class="sxs-lookup"><span data-stu-id="3222a-154">For more information about other incentives, see the [CSP incentive guide](https://aka.ms/partnerincentives) (requires CSP login).</span></span>

## <a name="learn-about-marketplace-exclusive-offers"></a><span data-ttu-id="3222a-155">Läs om exklusiva erbjudanden för Marketplace</span><span class="sxs-lookup"><span data-stu-id="3222a-155">Learn about marketplace exclusive offers</span></span>

<span data-ttu-id="3222a-156">ISV: er har möjlighet att göra sina erbjudanden tillgängliga enbart för vissa partner i CSP-programmet.</span><span class="sxs-lookup"><span data-stu-id="3222a-156">ISVs have the option to make their offers available only to specific partners in the CSP program.</span></span> <span data-ttu-id="3222a-157">Detta kallas för ett exklusivt erbjudande.</span><span class="sxs-lookup"><span data-stu-id="3222a-157">This is known as an Exclusive offer.</span></span> <span data-ttu-id="3222a-158">Alla partner i CSP-programmet kan fortfarande Visa alla ISV-erbjudanden i partner Centers kommersiella marknads platser, inklusive de som har marker ATS som exklusiva.</span><span class="sxs-lookup"><span data-stu-id="3222a-158">All partners in the CSP program can still view all ISV offers in Partner Center commercial marketplace, including those offers marked Exclusive.</span></span>

<span data-ttu-id="3222a-159">Om ett erbjudande **inte** har marker ATS som exklusiv kan alla partner köpa det erbjudandet (förutsatt att den valda kundens fakturerings land matchar landets tillgänglighet för ISV: s erbjudande).</span><span class="sxs-lookup"><span data-stu-id="3222a-159">If an offer is **not** marked Exclusive, all partners can purchase that offer (assuming the selected customer’s billing country matches the country availability of the ISV's offer).</span></span>

<span data-ttu-id="3222a-160">För alla erbjudanden som marker ATS som exklusiva, kommer dock bara de partner som valts av ISV att kunna köpa det erbjudandet.</span><span class="sxs-lookup"><span data-stu-id="3222a-160">For any offer marked Exclusive, however, only those partners selected by the ISV will be able to purchase that offer.</span></span>

> [!NOTE]
> <span data-ttu-id="3222a-161">Om du ser ett erbjudande som marker ATS som du vill sälja till dina kunder kan du kontakta ISV direkt och be om tillåtelse att sälja erbjudandet exklusivt.</span><span class="sxs-lookup"><span data-stu-id="3222a-161">If you see an offer marked Exclusive that you would like to sell to your customers, reach out to the ISV directly and ask for permission to sell the Exclusive offer.</span></span> <span data-ttu-id="3222a-162">När du visar information om ett exklusivt erbjudande kan du se en kontakt- **ISV** -länk som du kan välja.</span><span class="sxs-lookup"><span data-stu-id="3222a-162">When you view the details of an Exclusive offer, you may see a **Contact ISV** link that you can select.</span></span>

<span data-ttu-id="3222a-163">Läs mer om ISV-upplevelsen på den kommersiella marknads platsen genom att läsa [leverantörer av moln lösningar](/azure/marketplace/cloud-solution-providers).</span><span class="sxs-lookup"><span data-stu-id="3222a-163">To learn more about the ISV experience in the commercial marketplace, read [Cloud Solution Providers](/azure/marketplace/cloud-solution-providers).</span></span>

<span data-ttu-id="3222a-164">Mer information om CSP-upplevelsen på Marketplace finns i [Översikt över kommersiella marknads platser](csp-commercial-marketplace-overview.md).</span><span class="sxs-lookup"><span data-stu-id="3222a-164">For more information on the CSP experience in the marketplace, read [Commercial marketplace overview](csp-commercial-marketplace-overview.md).</span></span>

## <a name="next-steps"></a><span data-ttu-id="3222a-165">Nästa steg</span><span class="sxs-lookup"><span data-stu-id="3222a-165">Next steps</span></span>

- [<span data-ttu-id="3222a-166">Köp kommersiella Marketplace-erbjudanden</span><span class="sxs-lookup"><span data-stu-id="3222a-166">Purchase commercial marketplace offers</span></span>](csp-commercial-marketplace-purchase.md)