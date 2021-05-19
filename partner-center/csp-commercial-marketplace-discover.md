---
title: Upptäck erbjudanden – kommersiell marknadsplats
ms.topic: how-to
ms.date: 05/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Lär dig hur CSP-partner kan använda Partnercenter för att visa eller söka på marknadsplatsen efter SaaS-erbjudanden eller priser från oberoende programvaruleverantörer (ISV).
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: ab30f8391df58155c8511dc628b1fefd94c8d768
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 05/19/2021
ms.locfileid: "110147980"
---
# <a name="discover-offers-and-pricing-in-partner-center-commercial-marketplace"></a><span data-ttu-id="304e0-103">Upptäck erbjudanden och priser på den kommersiella marknadsplatsen i Partnercenter</span><span class="sxs-lookup"><span data-stu-id="304e0-103">Discover offers and pricing in Partner Center commercial marketplace</span></span>

<span data-ttu-id="304e0-104">**Lämpliga roller:** Globala | Administratörsagent</span><span class="sxs-lookup"><span data-stu-id="304e0-104">**Appropriate roles**: Global admin | Admin agent</span></span>

<span data-ttu-id="304e0-105">När oberoende programvaruleverantörer väljer att publicera ett erbjudande på den kommersiella marknadsplatsen kan de också avgöra om de vill att erbjudandet ska göras tillgängligt i CSP-programmet.</span><span class="sxs-lookup"><span data-stu-id="304e0-105">When Independent Software Vendors (ISVs) choose to publish an offer in the commercial marketplace, they can also decide if they want the offer to be made available in the CSP program.</span></span> <span data-ttu-id="304e0-106">Om de väljer att sälja erbjudandet via CSP-programmet bör CSP-partner se erbjudandet i Partnercenter Marketplace-området.</span><span class="sxs-lookup"><span data-stu-id="304e0-106">If they choose to sell the offer through the CSP program, CSP partners should see the offer in Partner Center Marketplace area.</span></span>

<span data-ttu-id="304e0-107">Om ett ISV-erbjudande inte visas som förväntat i Partnercenter kan det beror på följande:</span><span class="sxs-lookup"><span data-stu-id="304e0-107">If an ISV offer does not appear as you expect in Partner Center, it may be because:</span></span>

- <span data-ttu-id="304e0-108">ISV:en valde att inte sälja erbjudandet via CSP-programmet.</span><span class="sxs-lookup"><span data-stu-id="304e0-108">The ISV decided not to sell the offer through the CSP program.</span></span> <span data-ttu-id="304e0-109">Vissa ISV-produkter kan till exempel ha gjorts tillgängliga i andra områden på den kommersiella marknadsplatsen (till exempel [i Microsoft AppSource](https://appsource.microsoft.com/) och [Azure Marketplace](https://azuremarketplace.microsoft.com/)), men de kanske inte visas för partner i CSP-programmet på Partner Center Marketplace.</span><span class="sxs-lookup"><span data-stu-id="304e0-109">For example, some ISV products may have been made available in other areas of the commercial marketplace (such as in [Microsoft AppSource](https://appsource.microsoft.com/) and [Azure Marketplace](https://azuremarketplace.microsoft.com/)), but may not appear for partners in the CSP program in Partner Center marketplace.</span></span>

- <span data-ttu-id="304e0-110">ISV:en bestämde sig för att göra erbjudandet exklusivt för ett visst antal CSP-partner.</span><span class="sxs-lookup"><span data-stu-id="304e0-110">The ISV decided to make the offer exclusive to only a select number of CSP partners.</span></span> <span data-ttu-id="304e0-111">Mer information om exklusiva erbjudanden finns längre fram i det här hjälpavsnittet.</span><span class="sxs-lookup"><span data-stu-id="304e0-111">For more information about exclusive offers, see later in this help topic.</span></span>

- <span data-ttu-id="304e0-112">Erbjudandetypen kanske inte kan användas via Partnercenter eller Azure Portal (t.ex. containrar eller vissa användningsbaserade erbjudanden).</span><span class="sxs-lookup"><span data-stu-id="304e0-112">The offer type may not be transactable through Partner Center or Azure portal (e.g. Containers or some usage-based offers).</span></span>

- <span data-ttu-id="304e0-113">Faktureringsland för dina associerade kunder kanske inte stöds för det här ISV-erbjudandet.</span><span class="sxs-lookup"><span data-stu-id="304e0-113">The billing country of your associated customer(s) may not be supported for this ISV offer.</span></span>

## <a name="view-marketplace-offers-in-partner-center"></a><span data-ttu-id="304e0-114">Visa Marketplace-erbjudanden i Partnercenter</span><span class="sxs-lookup"><span data-stu-id="304e0-114">View Marketplace offers in Partner Center</span></span>

<span data-ttu-id="304e0-115">Så här visar du tillgängliga erbjudanden på den kommersiella marknadsplatsen i CSP-programmet:</span><span class="sxs-lookup"><span data-stu-id="304e0-115">To view available commercial marketplace offers in the CSP program:</span></span>

1. <span data-ttu-id="304e0-116">Logga in på instrumentpanelen [i Partnercenter](https://partner.microsoft.com/dashboard)och välj **CSP** på den vänstra navigeringsmenyn.</span><span class="sxs-lookup"><span data-stu-id="304e0-116">Sign into Partner Center [dashboard](https://partner.microsoft.com/dashboard), then select **CSP** from the left navigation menu.</span></span>

2. <span data-ttu-id="304e0-117">Välj **Sälj** följt av **Marketplace.**</span><span class="sxs-lookup"><span data-stu-id="304e0-117">Select **Sell**, followed by **Marketplace**.</span></span> <span data-ttu-id="304e0-118">Som standard visas produkter av alla typer och kategorier.</span><span class="sxs-lookup"><span data-stu-id="304e0-118">By default, you will see products of all types and categories.</span></span>

3. <span data-ttu-id="304e0-119">Välj ett filter efter typ eller kategori.</span><span class="sxs-lookup"><span data-stu-id="304e0-119">Select a filter by type or category.</span></span> <span data-ttu-id="304e0-120">Du kan också använda **Sök för** att hitta specifika nyckelord, erbjudandenamn eller namnen på ISV-utgivare.</span><span class="sxs-lookup"><span data-stu-id="304e0-120">You can also use **Search** to find specific keywords, offer names or the names of ISV publishers.</span></span>

4. <span data-ttu-id="304e0-121">Välj ett specifikt produkterbjudande i listan.</span><span class="sxs-lookup"><span data-stu-id="304e0-121">Select a specific product offer from the list.</span></span> <span data-ttu-id="304e0-122">Då kommer du till produktöversiktsfliken där du kan lära dig mer om erbjudandet.</span><span class="sxs-lookup"><span data-stu-id="304e0-122">This will take you to a product Overview tab where you can learn more about the offer.</span></span> <span data-ttu-id="304e0-123">Informationen på den här fliken kan vara:</span><span class="sxs-lookup"><span data-stu-id="304e0-123">Information on this tab might include:</span></span> 

    - <span data-ttu-id="304e0-124">En beskrivning av produkten eller erbjudandet</span><span class="sxs-lookup"><span data-stu-id="304e0-124">A description of the product or offer</span></span>

    - <span data-ttu-id="304e0-125">Mer information om ISV-utgivaren</span><span class="sxs-lookup"><span data-stu-id="304e0-125">More information about the ISV publisher</span></span>

    - <span data-ttu-id="304e0-126">Länkar till dokumentation eller marknadsföringsmaterial som laddats upp av ISV-utgivaren</span><span class="sxs-lookup"><span data-stu-id="304e0-126">Links to documentation or marketing materials uploaded by the ISV publisher</span></span>

    - <span data-ttu-id="304e0-127">Andra möjliga ISV-kontakter för kundsupport, teknik eller en kontakt för CSP-programmet</span><span class="sxs-lookup"><span data-stu-id="304e0-127">Other possible ISV contacts for customer support, engineering, or a contact for the CSP program</span></span>

5. <span data-ttu-id="304e0-128">Om du vill se mer information om ett erbjudandes tillgängliga planer, SKU:er eller priser väljer du **fliken Planer +** priser. På den här fliken visas:</span><span class="sxs-lookup"><span data-stu-id="304e0-128">To see more information about an offer's available plans, SKUs, or pricing, select the **Plans + Pricing** tab. This tab will show you:</span></span>

    - <span data-ttu-id="304e0-129">De marknader där det här erbjudandet är tillgängligt för dig</span><span class="sxs-lookup"><span data-stu-id="304e0-129">The markets where this offer is available to you</span></span>

    - <span data-ttu-id="304e0-130">En lista över SKU:er eller planer som är tillgängliga för erbjudandet</span><span class="sxs-lookup"><span data-stu-id="304e0-130">A list of SKUs or plans available for the offer</span></span>

    - <span data-ttu-id="304e0-131">Prissättning för varje tillgänglig SKU eller plan</span><span class="sxs-lookup"><span data-stu-id="304e0-131">Pricing for each SKU or Plan available</span></span>

## <a name="view-marketplace-offers-via-partner-center-apis"></a><span data-ttu-id="304e0-132">Visa Marketplace-erbjudanden via Partner Center-API:er</span><span class="sxs-lookup"><span data-stu-id="304e0-132">View Marketplace offers via Partner Center APIs</span></span>

<span data-ttu-id="304e0-133">CSP-programpartner kan också använda API:er för att returnera en lista över berättigade erbjudanden.</span><span class="sxs-lookup"><span data-stu-id="304e0-133">CSP program partners can also use APIs to return a list of eligible offers.</span></span> <span data-ttu-id="304e0-134">Berättigade erbjudanden är endast de SaaS ISV-erbjudanden som är tillgängliga för partnern att sälja via Partner Center Marketplace.</span><span class="sxs-lookup"><span data-stu-id="304e0-134">Eligible offers will be only those SaaS ISV offers available for the partner to sell via Partner Center marketplace.</span></span> <span data-ttu-id="304e0-135">För partner som använder API:er för att identifiera erbjudanden i katalogen kan du gå till vägledningen för [att hämta en lista över erbjudanden för en marknad.](/partner-center/develop/create-subscription-azure-marketplace-products#get-a-list-of-offers-for-a-market)</span><span class="sxs-lookup"><span data-stu-id="304e0-135">For partners using APIs to identify offers in the catalog, refer to the guidance to [obtain a list of offers for a market](/partner-center/develop/create-subscription-azure-marketplace-products#get-a-list-of-offers-for-a-market).</span></span>

## <a name="view-the-latest-marketplace-offer-pricing-in-partner-center"></a><span data-ttu-id="304e0-136">Visa de senaste priserna för Marketplace-erbjudanden i Partnercenter</span><span class="sxs-lookup"><span data-stu-id="304e0-136">View the latest Marketplace offer pricing in Partner Center</span></span>

<span data-ttu-id="304e0-137">Följ de här stegen för den senaste prisinformationen som är associerad med ett erbjudande:</span><span class="sxs-lookup"><span data-stu-id="304e0-137">Follow these steps for the latest pricing details associated with an offer:</span></span>

1. <span data-ttu-id="304e0-138">Logga in på [instrumentpanelen i Partnercenter](https://partner.microsoft.com/dashboard)och välj **CSP** på den vänstra navigeringsmenyn.</span><span class="sxs-lookup"><span data-stu-id="304e0-138">Sign into Partner Center [dashboard](https://partner.microsoft.com/dashboard), then select **CSP** from the left navigation menu.</span></span>

2. <span data-ttu-id="304e0-139">Välj **Sälj** följt av **Priser och erbjudanden.**</span><span class="sxs-lookup"><span data-stu-id="304e0-139">Select **Sell**, followed by **Pricing and offers**.</span></span>

3. <span data-ttu-id="304e0-140">Rulla ned till **avsnittet Marketplace,** välj en plats och ladda ned **Marketplace-priser.**</span><span class="sxs-lookup"><span data-stu-id="304e0-140">Scroll down to the **Marketplace** section, select a location and download **Marketplace pricing**.</span></span> <span data-ttu-id="304e0-141">Detta genererar ett kalkylblad med de senaste prisdata för SaaS, licensbaserade erbjudanden och uppmätta erbjudanden som är tillgängliga från ISV-utgivare.</span><span class="sxs-lookup"><span data-stu-id="304e0-141">This generates a spreadsheet with the latest pricing data for SaaS, license-based offers and metered offers available from ISV publishers.</span></span> <span data-ttu-id="304e0-142">Vissa priser för Azure-program kan också visas här.</span><span class="sxs-lookup"><span data-stu-id="304e0-142">Some Azure application pricing may also appear here.</span></span> <span data-ttu-id="304e0-143">Den här informationen uppdateras dagligen, så du kan kontrollera den för aktuella priser så ofta du väljer.</span><span class="sxs-lookup"><span data-stu-id="304e0-143">This information is updated daily, so you can check it for current prices as often as you choose.</span></span>

4. <span data-ttu-id="304e0-144">Om en ISV-produkt innehåller en kostnadsfri utvärderingsperiod visar kalkylbladet två rader för den produkten:</span><span class="sxs-lookup"><span data-stu-id="304e0-144">If an ISV product includes a free trial period, the spreadsheet will display two rows for that product:</span></span>

    - <span data-ttu-id="304e0-145">En rad visar priset för den kostnadsfria utvärderingsversionen på noll.</span><span class="sxs-lookup"><span data-stu-id="304e0-145">One row shows the free trial price of zero.</span></span> <span data-ttu-id="304e0-146">Det innebär att en kostnadsfri utvärderingsperiod är tillgänglig.</span><span class="sxs-lookup"><span data-stu-id="304e0-146">This means a free trial period is available.</span></span>

    - <span data-ttu-id="304e0-147">Den andra raden visar det pris och de villkor som gäller när den kostnadsfria utvärderingsperioden är slut.</span><span class="sxs-lookup"><span data-stu-id="304e0-147">The other row shows the price and terms that will apply after the free trial period is over.</span></span>

<span data-ttu-id="304e0-148">Som CSP-programpartner kan du vara berättigad till andra incitament som är associerade med vissa erbjudanden på den kommersiella marknadsplatsen.</span><span class="sxs-lookup"><span data-stu-id="304e0-148">As a CSP program partner, you may be eligible for other incentives associated with certain commercial marketplace offers.</span></span> <span data-ttu-id="304e0-149">Mer information om andra incitament finns i [CSP-incitamentguiden (kräver](https://aka.ms/partnerincentives) CSP-inloggning).</span><span class="sxs-lookup"><span data-stu-id="304e0-149">For more information about other incentives, see the [CSP incentive guide](https://aka.ms/partnerincentives) (requires CSP login).</span></span>

## <a name="learn-about-marketplace-exclusive-offers"></a><span data-ttu-id="304e0-150">Läs mer om marketplace-exklusiva erbjudanden</span><span class="sxs-lookup"><span data-stu-id="304e0-150">Learn about marketplace exclusive offers</span></span>

<span data-ttu-id="304e0-151">ISV:er har möjlighet att endast göra sina erbjudanden tillgängliga för specifika partner i CSP-programmet.</span><span class="sxs-lookup"><span data-stu-id="304e0-151">ISVs have the option to make their offers available only to specific partners in the CSP program.</span></span> <span data-ttu-id="304e0-152">Detta kallas för ett exklusivt erbjudande.</span><span class="sxs-lookup"><span data-stu-id="304e0-152">This is known as an Exclusive offer.</span></span> <span data-ttu-id="304e0-153">Alla partner i CSP-programmet kan fortfarande visa alla ISV-erbjudanden på den kommersiella marknadsplatsen i Partnercenter, inklusive de erbjudanden som har markerats som Exklusiva.</span><span class="sxs-lookup"><span data-stu-id="304e0-153">All partners in the CSP program can still view all ISV offers in Partner Center commercial marketplace, including those offers marked Exclusive.</span></span>

<span data-ttu-id="304e0-154">Om ett erbjudande inte **är** markerat som Exklusivt kan alla partner köpa erbjudandet (förutsatt att den valda kundens faktureringsland matchar land tillgängligheten för ISV:ns erbjudande).</span><span class="sxs-lookup"><span data-stu-id="304e0-154">If an offer is **not** marked Exclusive, all partners can purchase that offer (assuming the selected customer’s billing country matches the country availability of the ISV's offer).</span></span>

<span data-ttu-id="304e0-155">För ett erbjudande som är markerat som Exklusivt kan dock endast de partner som väljs av ISV:en köpa erbjudandet.</span><span class="sxs-lookup"><span data-stu-id="304e0-155">For any offer marked Exclusive, however, only those partners selected by the ISV will be able to purchase that offer.</span></span>

> [!NOTE]
> <span data-ttu-id="304e0-156">Om du ser ett erbjudande som är markerat som Exklusivt som du vill sälja till dina kunder kan du kontakta ISV direkt och be om tillstånd att sälja det exklusiva erbjudandet.</span><span class="sxs-lookup"><span data-stu-id="304e0-156">If you see an offer marked Exclusive that you would like to sell to your customers, reach out to the ISV directly and ask for permission to sell the Exclusive offer.</span></span> <span data-ttu-id="304e0-157">När du visar information om ett exklusivt erbjudande kan du se en **kontakt-ISV-länk** som du kan välja.</span><span class="sxs-lookup"><span data-stu-id="304e0-157">When you view the details of an Exclusive offer, you may see a **Contact ISV** link that you can select.</span></span>

<span data-ttu-id="304e0-158">Mer information om ISV-upplevelsen på den kommersiella marknadsplatsen finns i [Molnlösningsleverantörer.](/azure/marketplace/cloud-solution-providers)</span><span class="sxs-lookup"><span data-stu-id="304e0-158">To learn more about the ISV experience in the commercial marketplace, read [Cloud Solution Providers](/azure/marketplace/cloud-solution-providers).</span></span>

<span data-ttu-id="304e0-159">Mer information om CSP-upplevelsen på marketplace finns i Översikt [över kommersiell marknadsplats.](csp-commercial-marketplace-overview.md)</span><span class="sxs-lookup"><span data-stu-id="304e0-159">For more information on the CSP experience in the marketplace, read [Commercial marketplace overview](csp-commercial-marketplace-overview.md).</span></span>

## <a name="next-steps"></a><span data-ttu-id="304e0-160">Nästa steg</span><span class="sxs-lookup"><span data-stu-id="304e0-160">Next steps</span></span>

- [<span data-ttu-id="304e0-161">Köpa erbjudanden på den kommersiella marknadsplatsen</span><span class="sxs-lookup"><span data-stu-id="304e0-161">Purchase commercial marketplace offers</span></span>](csp-commercial-marketplace-purchase.md)