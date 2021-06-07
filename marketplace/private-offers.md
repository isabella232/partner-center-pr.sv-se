---
title: Privata erbjudanden i Azure Marketplace
description: Läs mer om privata erbjudanden i Azure Marketplace.
ms.service: marketplace-customer
ms.topic: article
author: Guyshu
ms.author: gushuchm
ms.date: 06/03/2021
ms.openlocfilehash: 55d0716b183e9e8905e631447e547396d6f55404
ms.sourcegitcommit: 9cb6bc9df20540f812b7932f88e520976c1aa85a
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/06/2021
ms.locfileid: "111534147"
---
# <a name="private-plans-in-azure-marketplace"></a><span data-ttu-id="7a92b-103">Privata planer i Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="7a92b-103">Private plans in Azure Marketplace</span></span>

<span data-ttu-id="7a92b-104">Privata planer är hur utgivare tillhandahåller anpassade planer till specifika kunder.</span><span class="sxs-lookup"><span data-stu-id="7a92b-104">Private plans are how publishers provide custom plans to specific customers.</span></span> <span data-ttu-id="7a92b-105">Privata abonnemang är endast tillgängliga för betalda erbjudanden som kan köpas och installeras direkt från Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="7a92b-105">Private plans are only available for paid offers that can be purchased and directly installed from the Azure portal.</span></span> <span data-ttu-id="7a92b-106">Utgivare kan inte skapa privata planer för  konsulttjänster, tjänster som har Kontakta mig som en call-to-action eller någon kostnadsfri tjänst, oavsett om de kan installeras från portalen eller inte.</span><span class="sxs-lookup"><span data-stu-id="7a92b-106">Publishers cannot create private plans for consulting services, any service that has **Contact me** as a call-to-action, or any free service, regardless of whether it can be installed from the portal or not.</span></span>

## <a name="find-private-plans-in-the-azure-portal"></a><span data-ttu-id="7a92b-107">Hitta privata planer i Azure Portal</span><span class="sxs-lookup"><span data-stu-id="7a92b-107">Find private plans in the Azure portal</span></span>

<span data-ttu-id="7a92b-108">När en partner publicerar en privat plan visas den bara för berättigade användare i **Avsnittet Marketplace** i Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="7a92b-108">When a partner publishes a private plan, it is visible only to eligible users in the **Marketplace** section of the Azure portal.</span></span> <span data-ttu-id="7a92b-109">Dessa användare definieras av prenumerations-ID eller klientorganisations-ID, beroende på erbjudandetyp.</span><span class="sxs-lookup"><span data-stu-id="7a92b-109">These users are defined by subscription ID or tenant ID, depending on the offer type.</span></span> <span data-ttu-id="7a92b-110">Om du är berättigad till privata planer finns det två sätt att hitta dem i portalen.</span><span class="sxs-lookup"><span data-stu-id="7a92b-110">If you are eligible for private plans, there are two ways to find them in the portal.</span></span>

> [!NOTE]
> <span data-ttu-id="7a92b-111">Privata planer är sökbara men inte filtrerbara (efter kategori) i Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="7a92b-111">Private plans are searchable but not filterable (by category) in the Azure portal.</span></span>

<span data-ttu-id="7a92b-112">I den Azure Portal väljer du **+ Skapa en resurs** eller söker efter "marketplace" för att gå till **Marketplace-sidan.**</span><span class="sxs-lookup"><span data-stu-id="7a92b-112">In the Azure portal, select **+ Create a resource** or search for “marketplace” to go to the **Marketplace** page.</span></span> <span data-ttu-id="7a92b-113">Om du är berättigad till privata planer visas banderollen Du har **tillgängliga privata** planer överst på sidan.</span><span class="sxs-lookup"><span data-stu-id="7a92b-113">If you are eligible for private plans, you will see the **You have private plans available** banner on the top of the page.</span></span> <span data-ttu-id="7a92b-114">Välj **Visa privata erbjudanden + planer för** att gå till sidan för dina privata planer.</span><span class="sxs-lookup"><span data-stu-id="7a92b-114">Select **View private offers + plans** to go to your private plans page.</span></span>

:::image type="content" source="media/private-offers/private-offers-banner.png" alt-text="Banderollen som visas när du har privata planer tillgängliga.":::

## <a name="review-private-plans"></a><span data-ttu-id="7a92b-116">Granska privata planer</span><span class="sxs-lookup"><span data-stu-id="7a92b-116">Review private plans</span></span>

<span data-ttu-id="7a92b-117">En privat plan är en del av flera planer i ett erbjudande.</span><span class="sxs-lookup"><span data-stu-id="7a92b-117">A private plan is part of several plans in an offer.</span></span> <span data-ttu-id="7a92b-118">Varje erbjudande kan ha flera planer, både offentliga och privata, men privata planer visas under en separat lista från offentliga planer.</span><span class="sxs-lookup"><span data-stu-id="7a92b-118">Each offer can have multiple plans, both public and private, but private plans are shown under a separate listing from public plans.</span></span>

<span data-ttu-id="7a92b-119">Du kan se tillgängliga privata planer under fliken **Planer,** markerade med ett privat **märke:**</span><span class="sxs-lookup"><span data-stu-id="7a92b-119">You can see the available private plans under the **Plans** tab, marked with a distinctive **Private** badge:</span></span>

:::image type="content" source="media/private-offers/private-badge.png" alt-text="En sida med planer markerade som Privata.":::

<span data-ttu-id="7a92b-121">Om du har fler än en prenumeration visas alla privata abonnemang som är tillgängliga för alla dina prenumerationer.</span><span class="sxs-lookup"><span data-stu-id="7a92b-121">If you have more than one subscription, you will see all private plans available for all your subscriptions.</span></span> <span data-ttu-id="7a92b-122">När du väljer **Skapa** dirigeras du till sidan för resursskapande för att börja konfigurera resursen.</span><span class="sxs-lookup"><span data-stu-id="7a92b-122">When you select **Create**, you are routed to the resource creation page to start configuring your resource.</span></span>

<span data-ttu-id="7a92b-123">Om du väljer **Skapa** och har flera prenumerationer, men inte alla läggs till i den privata planen, kanske din standardprenumeration inte är den prenumeration som är berättigad för den här privata planen.</span><span class="sxs-lookup"><span data-stu-id="7a92b-123">If you select **Create** and have multiple subscriptions, but not all of them are added to the private plan, your default subscription may not be the subscription eligible for this private plan.</span></span> <span data-ttu-id="7a92b-124">I det här fallet väljer du rätt prenumeration.</span><span class="sxs-lookup"><span data-stu-id="7a92b-124">In this case, select the correct subscription.</span></span>

:::image type="content" source="media/private-offers/select-correct-subscription.png" alt-text="Länken som visar att det finns fler privata planer tillgängliga.":::

## <a name="next-steps"></a><span data-ttu-id="7a92b-126">Nästa steg</span><span class="sxs-lookup"><span data-stu-id="7a92b-126">Next steps</span></span>

- [<span data-ttu-id="7a92b-127">Vad är Azure Marketplace?</span><span class="sxs-lookup"><span data-stu-id="7a92b-127">What is Azure Marketplace?</span></span>](azure-marketplace-overview.md)
