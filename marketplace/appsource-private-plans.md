---
title: Privata planer i Microsoft AppSource
description: Konfigurera privata planer i Microsoft AppSource (Azure Marketplace).
ms.service: marketplace-customer
ms.topic: how-to
author: Guyshu
ms.author: gushuchm
ms.date: 06/08/2021
robots: noindex
ms.openlocfilehash: a392859c1106c747e0e7c696927ef3b25262e411
ms.sourcegitcommit: a576c9606ade59cef7d0b2d5e1584016740d08eb
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/11/2021
ms.locfileid: "112008607"
---
# <a name="private-plans-in-microsoft-appsource"></a><span data-ttu-id="ed093-103">Privata planer i Microsoft AppSource</span><span class="sxs-lookup"><span data-stu-id="ed093-103">Private plans in Microsoft AppSource</span></span>

<span data-ttu-id="ed093-104">Privata planer är hur utgivare tillhandahåller anpassade planer till specifika kunder.</span><span class="sxs-lookup"><span data-stu-id="ed093-104">Private plans are how publishers provide custom plans to specific customers.</span></span> <span data-ttu-id="ed093-105">Det här alternativet är nu tillgängligt i Microsoft AppSource.</span><span class="sxs-lookup"><span data-stu-id="ed093-105">This option is now available in Microsoft AppSource.</span></span> <span data-ttu-id="ed093-106">Privata planer kan säljas på AppSource för SaaS-erbjudanden  (programvara som en tjänst) med call-to-action för Hämta nu.</span><span class="sxs-lookup"><span data-stu-id="ed093-106">Private plans can be sold on AppSource for software as a service (SaaS) offers with the **Get it now** call-to-action.</span></span>

## <a name="ask-your-isv-for-a-private-plan"></a><span data-ttu-id="ed093-107">Be din ISV om en privat plan</span><span class="sxs-lookup"><span data-stu-id="ed093-107">Ask your ISV for a private plan</span></span>

<span data-ttu-id="ed093-108">För att en privat plan ska vara tillgänglig för dig i AppSource måste du kontakta ISV:en direkt och förhandla fram ett anpassat pris och tekniska specifikationer.</span><span class="sxs-lookup"><span data-stu-id="ed093-108">For a private plan to be available to you in AppSource, you need to contact the ISV directly and negotiate a custom price and technical specifications.</span></span> <span data-ttu-id="ed093-109">När villkoren i den privata planen har godkänts skapar ISV:n en plan åt dig och tilldelar den till din organisations klientorganisations-ID, som du måste ange.</span><span class="sxs-lookup"><span data-stu-id="ed093-109">Once the terms of the private plan are agreed to, the ISV will create a plan for you and assign it to your organization’s tenant ID, which you’ll need to provide.</span></span>

### <a name="finding-your-tenant-id"></a><span data-ttu-id="ed093-110">Hitta ditt klientorganisations-ID</span><span class="sxs-lookup"><span data-stu-id="ed093-110">Finding your tenant ID</span></span>

1. <span data-ttu-id="ed093-111">I AppSource, i det övre högra hörnet, väljer du ikonen för din kontoprofil och sedan **Visa klientorganisation.**</span><span class="sxs-lookup"><span data-stu-id="ed093-111">In AppSource, in the upper right corner, select your account profile icon and then **View tenant**.</span></span>
2. <span data-ttu-id="ed093-112">Kopiera klientorganisations-ID:t och ange det till ISV:n.</span><span class="sxs-lookup"><span data-stu-id="ed093-112">Copy the tenant ID and provide it to the ISV.</span></span>

    :::image type="content" source="media/private-offers/find-tenant-id.png" alt-text="Visar hur du hittar ditt klientorganisations-ID.":::

## <a name="find-a-private-plan-in-appsource"></a><span data-ttu-id="ed093-114">Hitta en privat plan i AppSource</span><span class="sxs-lookup"><span data-stu-id="ed093-114">Find a private plan in AppSource</span></span>

<span data-ttu-id="ed093-115">Det kan ta upp till 48 timmar efter att ISV:en har publicerat den nya privata planen innan du ser den i AppSource.</span><span class="sxs-lookup"><span data-stu-id="ed093-115">It can take up to 48 hours after the ISV publishes the new private plan before you see it in AppSource.</span></span> <span data-ttu-id="ed093-116">Om du vill hitta privata planer som är associerade med ditt **klientorganisations-ID väljer** du Privata planer (låsikonen) längst upp till höger i AppSource.</span><span class="sxs-lookup"><span data-stu-id="ed093-116">To find private plans associated with your tenant ID, select **Private plans** (Lock icon) at the upper right of AppSource.</span></span>

:::image type="content" source="media/private-offers/lock-icon.png" alt-text="Visar låsikonen (hänglås) i det övre verktygsfältet.":::

<span data-ttu-id="ed093-118">Om du inte är inloggad uppmanas du att göra det i ett meddelande.</span><span class="sxs-lookup"><span data-stu-id="ed093-118">If you are not signed in, a message will prompt you to do so.</span></span> <span data-ttu-id="ed093-119">Du kan sedan köpa de privata planer som är associerade med ditt klientorganisations-ID **på fliken Planer +** priser.</span><span class="sxs-lookup"><span data-stu-id="ed093-119">You can then purchase the private plans associated with your tenant ID on the **Plans + pricing** tab.</span></span>

:::image type="content" source="media/private-offers/plan-pricing-tab.png" alt-text="Visar privata erbjudanden på fliken plan och prissättning.":::

<span data-ttu-id="ed093-121">Om privata planer inte är tillgängliga för din klientorganisation visas ett meddelande om att du inte har några privata planer eller erbjudanden.</span><span class="sxs-lookup"><span data-stu-id="ed093-121">If private plans are not available for your tenant, a message will state that you don’t have any private plans or offers.</span></span>

## <a name="purchase-a-private-plan"></a><span data-ttu-id="ed093-122">Köpa en privat plan</span><span class="sxs-lookup"><span data-stu-id="ed093-122">Purchase a private plan</span></span>

<span data-ttu-id="ed093-123">En ISV kan innehålla en eller flera privata planer i ett erbjudande.</span><span class="sxs-lookup"><span data-stu-id="ed093-123">An ISV can include one or more private plans within an offer.</span></span> <span data-ttu-id="ed093-124">Varje erbjudande kan ha både offentliga och privata planer, men privata planer visas under en separat sida med erbjudanden från ikonen privata erbjudanden (hänglås) längst upp till höger på sidan.</span><span class="sxs-lookup"><span data-stu-id="ed093-124">Each offer can have both public and private plans, but private plans appear under a separate offer listing page accessed from the Private offers icon (padlock) at the upper right of the page.</span></span>

<span data-ttu-id="ed093-125">Tillgängliga privata planer visas på **fliken Planer +** priser. Privata planer har ett blått märke.</span><span class="sxs-lookup"><span data-stu-id="ed093-125">Available private plans display on the **Plans + pricing** tab. Private plans have a distinctive blue badge.</span></span>

:::image type="content" source="media/private-offers/private-plans-badge.png" alt-text="Visar märke för det blå privata erbjudandet bredvid privata erbjudanden.":::

<span data-ttu-id="ed093-127">Om du vill köpa en vald plan väljer **du Hämta nu** och följer stegen.</span><span class="sxs-lookup"><span data-stu-id="ed093-127">To purchase a selected plan, select **Get it now** and follow the steps provided.</span></span>

## <a name="next-steps"></a><span data-ttu-id="ed093-128">Nästa steg</span><span class="sxs-lookup"><span data-stu-id="ed093-128">Next steps</span></span>

- [<span data-ttu-id="ed093-129">Vad är Microsoft AppSource?</span><span class="sxs-lookup"><span data-stu-id="ed093-129">What is Microsoft AppSource?</span></span>](appsource-overview.md)
