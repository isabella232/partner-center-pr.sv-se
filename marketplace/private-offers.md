---
title: Privata erbjudanden i Azure Marketplace
description: Lär dig om privata erbjudanden i Azure Marketplace.
ms.prod: marketplace-customer
ms.topic: article
author: Guyshu
ms.author: gushuchm
ms.date: 11/20/2020
ms.openlocfilehash: 055151f0420d642d591554a829dc21b69df84ebd
ms.sourcegitcommit: 1aa43438ad181278052788f15e017f9ae7777943
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 11/21/2020
ms.locfileid: "95007644"
---
# <a name="private-offers-in-azure-marketplace"></a><span data-ttu-id="40124-103">Privata erbjudanden i Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="40124-103">Private offers in Azure Marketplace</span></span>

<span data-ttu-id="40124-104">Privata erbjudanden ger utgivare anpassade planer för vissa kunder.</span><span class="sxs-lookup"><span data-stu-id="40124-104">Private offers are how publishers provide custom plans to specific customers.</span></span> <span data-ttu-id="40124-105">Det här alternativet stöds för närvarande endast i Azure Marketplace-miljön i Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="40124-105">This option is currently supported only in the Azure Marketplace experience in the Azure portal.</span></span> <span data-ttu-id="40124-106">Privata erbjudanden är bara tillgängliga för avgiftsbelagda erbjudanden som kan köpas och installeras direkt från Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="40124-106">Private offers are only available for paid offers that can be purchased and directly installed from the Azure portal.</span></span> <span data-ttu-id="40124-107">Det går inte att skapa privata erbjudanden för konsult tjänster, alla tjänster som har **kontakt mig** som en samtal till åtgärd eller en kostnads fri tjänst, oavsett om den kan installeras från portalen eller inte.</span><span class="sxs-lookup"><span data-stu-id="40124-107">Publisher cannot create private offers for consulting services, any service that has **Contact me** as a call-to-action, or any free service, regardless of whether it can be installed from the portal or not.</span></span>

## <a name="find-private-offers-in-the-azure-portal"></a><span data-ttu-id="40124-108">Hitta privata erbjudanden i Azure Portal</span><span class="sxs-lookup"><span data-stu-id="40124-108">Find private offers in the Azure portal</span></span>

<span data-ttu-id="40124-109">När en partner publicerar ett privat erbjudande, är det bara synligt för berättigade användare i **Marketplace** -avsnittet i Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="40124-109">When a partner publishes a private offer, it is visible only to eligible users in the **Marketplace** section of the Azure portal.</span></span> <span data-ttu-id="40124-110">Dessa användare definieras av prenumerations-ID eller klient-ID, beroende på typen av erbjudande.</span><span class="sxs-lookup"><span data-stu-id="40124-110">These users are defined by subscription ID or tenant ID, depending on the offer type.</span></span> <span data-ttu-id="40124-111">Om du är berättigad till privata erbjudanden finns det två sätt att hitta dem i portalen.</span><span class="sxs-lookup"><span data-stu-id="40124-111">If you are eligible for  private offers, there are two ways to find them in the portal.</span></span>

> [!NOTE]
> <span data-ttu-id="40124-112">Privata erbjudanden är för närvarande inte sökbara eller filtrerings bara (efter kategori) i Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="40124-112">Private offers are currently not searchable or filterable (by category) in the Azure portal.</span></span>

<span data-ttu-id="40124-113">I Azure Portal väljer du **+ skapa en resurs** eller söker efter "Marketplace" för att gå till **Marketplace** -sidan.</span><span class="sxs-lookup"><span data-stu-id="40124-113">In the Azure portal, select **+ Create a resource** or search for “marketplace” to go to the **Marketplace** page.</span></span> <span data-ttu-id="40124-114">Om du är berättigad till privata erbjudanden visas banderollen för **privata erbjudanden** överst på sidan.</span><span class="sxs-lookup"><span data-stu-id="40124-114">If you are eligible for private offers, you will see the **You have private offers available** banner on the top of the page.</span></span> <span data-ttu-id="40124-115">Välj **Visa privata erbjudanden** för att gå till din privata erbjudande sida.</span><span class="sxs-lookup"><span data-stu-id="40124-115">Select **View private offers** to go to your private offers page.</span></span>

:::image type="content" source="media/private-offers/private-offers-banner.png" alt-text="Den banderoll som visas när du har privata erbjudanden tillgängliga.":::

<span data-ttu-id="40124-117">Alternativt kan du även Rulla längst ned på sidan produkt galleri och visa en delmängd av dina privata erbjudanden om du ser annonsen för privata erbjudanden.</span><span class="sxs-lookup"><span data-stu-id="40124-117">Alternately, if you see the private offers banner, you can also scroll to the bottom of the product gallery page and you will see a subset of your private offers.</span></span> <span data-ttu-id="40124-118">Välj länken om du vill **Visa mer** för att gå till din privata erbjudande sida.</span><span class="sxs-lookup"><span data-stu-id="40124-118">Select the link to **See More** to go to your private offers page.</span></span>

:::image type="content" source="media/private-offers/see-more-link.png" alt-text="Visar privata erbjudanden längst ned på skärmen, tillsammans med länken se mer.":::

## <a name="review-private-plans"></a><span data-ttu-id="40124-120">Granska privata planer</span><span class="sxs-lookup"><span data-stu-id="40124-120">Review private plans</span></span>

<span data-ttu-id="40124-121">Ett privat erbjudande är i själva verket en privat plan inom ett erbjudande.</span><span class="sxs-lookup"><span data-stu-id="40124-121">A private offer is actually a private plan within an offer.</span></span> <span data-ttu-id="40124-122">Varje erbjudande kan ha flera planer, både offentliga och privata, men privata planer visas under en separat lista från offentliga planer.</span><span class="sxs-lookup"><span data-stu-id="40124-122">Each offer can have multiple plans, both public and private, but private plans are shown under a separate listing from public plans.</span></span>

<span data-ttu-id="40124-123">Du kan se tillgängliga privata planer på fliken **planer** som marker ATS med ett **eget privat** märke:</span><span class="sxs-lookup"><span data-stu-id="40124-123">You can see the available private plans under the **Plans** tab, marked with a distinctive **Private** badge:</span></span>

:::image type="content" source="media/private-offers/private-badge.png" alt-text="En sida med planer som marker ATS som privata.":::

<span data-ttu-id="40124-125">Om du har mer än en prenumeration visas alla privata erbjudanden som är tillgängliga för alla dina prenumerationer.</span><span class="sxs-lookup"><span data-stu-id="40124-125">If you have more than one subscription, you will see all private offers available for all your subscriptions.</span></span> <span data-ttu-id="40124-126">När du väljer **skapa** dirigeras du till sidan för att skapa resurser för att börja konfigurera din resurs.</span><span class="sxs-lookup"><span data-stu-id="40124-126">When you select **Create**, you are routed to the resource creation page to start configuring your resource.</span></span>

<span data-ttu-id="40124-127">Om du väljer **skapa** och har flera prenumerationer, men inte alla läggs till i den privata planen, kanske din standard prenumeration inte är den prenumeration som är berättigad till det privata erbjudandet.</span><span class="sxs-lookup"><span data-stu-id="40124-127">If you select **Create** and have multiple subscriptions, but not all of them are added to the private plan, your default subscription may not be the subscription eligible for this private offer.</span></span> <span data-ttu-id="40124-128">I det här fallet väljer du rätt prenumeration.</span><span class="sxs-lookup"><span data-stu-id="40124-128">In this case, select the correct subscription.</span></span>

:::image type="content" source="media/private-offers/select-correct-subscription.png" alt-text="Länken som visar att det finns fler privata erbjudanden tillgängliga.":::

## <a name="next-steps"></a><span data-ttu-id="40124-130">Nästa steg</span><span class="sxs-lookup"><span data-stu-id="40124-130">Next steps</span></span>

- [<span data-ttu-id="40124-131">Vad är Azure Marketplace?</span><span class="sxs-lookup"><span data-stu-id="40124-131">What is Azure Marketplace?</span></span>](azure-marketplace-overview.md)
