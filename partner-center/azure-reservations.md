---
title: Sälj kunder Microsoft Azure reservationer
description: Som en moln lösnings leverantör kan du köpa, sälja eller hantera Azure-reservationer för kunder. Använd partner Center, Azure Portal eller partner Center API.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 08/06/2020
ms.openlocfilehash: 9dc92685503fd4b9b05e40337f72e810c1693779
ms.sourcegitcommit: 2d9aab15ddc20cb3d9537e68ace33d36f7d8a250
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 12/02/2020
ms.locfileid: "96534904"
---
# <a name="sell-microsoft-azure-reservations-to-customers-using-partner-center-the-azure-portal-or-apis"></a><span data-ttu-id="fb9e0-104">Sälj Microsoft Azure reservationer till kunder som använder Partner Center, Azure Portal eller API: er</span><span class="sxs-lookup"><span data-stu-id="fb9e0-104">Sell Microsoft Azure reservations to customers using Partner Center, the Azure portal, or APIs</span></span>

<span data-ttu-id="fb9e0-105">**Lämpliga roller**</span><span class="sxs-lookup"><span data-stu-id="fb9e0-105">**Appropriate roles**</span></span>

- <span data-ttu-id="fb9e0-106">Administratörs agent</span><span class="sxs-lookup"><span data-stu-id="fb9e0-106">Admin agent</span></span>
- <span data-ttu-id="fb9e0-107">Global administratör</span><span class="sxs-lookup"><span data-stu-id="fb9e0-107">Global admin</span></span>
- <span data-ttu-id="fb9e0-108">Support agent</span><span class="sxs-lookup"><span data-stu-id="fb9e0-108">Helpdesk agent</span></span>
- <span data-ttu-id="fb9e0-109">Försäljnings agent</span><span class="sxs-lookup"><span data-stu-id="fb9e0-109">Sales agent</span></span>
- <span data-ttu-id="fb9e0-110">Administratör för användar hantering</span><span class="sxs-lookup"><span data-stu-id="fb9e0-110">User management admin</span></span>

<span data-ttu-id="fb9e0-111">Som partner i Cloud Solution Provider-programmet (CSP) kan du köpa, sälja eller hantera Azure-reservationer för kunder.</span><span class="sxs-lookup"><span data-stu-id="fb9e0-111">As a partner in the Cloud Solution Provider program (CSP), you can buy, sell, or manage Azure reservations for customers.</span></span> <span data-ttu-id="fb9e0-112">Använd partner Center, Azure Portal eller partner Center API.</span><span class="sxs-lookup"><span data-stu-id="fb9e0-112">Use Partner Center, the Azure portal, or the Partner Center API.</span></span>

> [!NOTE]
> <span data-ttu-id="fb9e0-113">Den här artikeln gäller endast partner i CSP.</span><span class="sxs-lookup"><span data-stu-id="fb9e0-113">This article applies only to partners in CSP.</span></span> <span data-ttu-id="fb9e0-114">Kunder som använder andra typer av prenumerationer (t. ex. betala per användning, enskilda, Microsoft-kundavtal eller Enterprise-avtal prenumerationer) bör i stället läsa [denna dokumentation om Azure-reservationer](/azure/cost-management-billing/reservations).</span><span class="sxs-lookup"><span data-stu-id="fb9e0-114">Customers using other types of subscriptions (such as, pay-as-you-go, individual, Microsoft Customer Agreement, or Enterprise Agreement subscriptions) should instead read [this Azure reservations documentation](/azure/cost-management-billing/reservations).</span></span>

<span data-ttu-id="fb9e0-115">Partner i CSP-programmet kan erbjuda sina kunder Microsoft Azure reservationer.</span><span class="sxs-lookup"><span data-stu-id="fb9e0-115">Partners in the CSP program can offer their customers Microsoft Azure reservations.</span></span> <span data-ttu-id="fb9e0-116">Kunder kan få betydande besparingar när de reserverar i förväg.</span><span class="sxs-lookup"><span data-stu-id="fb9e0-116">Customers can gain significant savings when they reserve in advance.</span></span> <span data-ttu-id="fb9e0-117">Azure-reservationer ger kunderna enkelhet och flexibilitet på följande sätt:</span><span class="sxs-lookup"><span data-stu-id="fb9e0-117">Azure reservations offer customers simplicity and flexibility in the following ways:</span></span>

- <span data-ttu-id="fb9e0-118">En eller tre års reservations villkor</span><span class="sxs-lookup"><span data-stu-id="fb9e0-118">One or three-year reservation terms</span></span>
- <span data-ttu-id="fb9e0-119">Lätt att komma igång; installationen slutfördes på några sekunder</span><span class="sxs-lookup"><span data-stu-id="fb9e0-119">Easy to get started; setup completed in seconds</span></span>
- <span data-ttu-id="fb9e0-120">Avbryta eller byta ut reserverade instanser när som helst för justerad åter betalning</span><span class="sxs-lookup"><span data-stu-id="fb9e0-120">Cancel or exchange reserved instances at any time for adjusted refund</span></span>
- <span data-ttu-id="fb9e0-121">Hantera användning av reserverade instanser på organisations-eller individuell avdelnings nivå</span><span class="sxs-lookup"><span data-stu-id="fb9e0-121">Manage reserved instances usage at the organizational or individual department level</span></span>

<span data-ttu-id="fb9e0-122">Azure-reservationer kan överklaga till kunder på följande sätt:</span><span class="sxs-lookup"><span data-stu-id="fb9e0-122">Azure reservations can appeal to customers in the following ways:</span></span>

- <span data-ttu-id="fb9e0-123">Reservationer kan erbjuda betydande besparingar jämfört med PAYG-priser (betala per användning)</span><span class="sxs-lookup"><span data-stu-id="fb9e0-123">Reservations can offer significant savings over pay-as-you-go (PAYG) pricing</span></span>
- <span data-ttu-id="fb9e0-124">Bättre budgetering och prognostisering med förskotts betalning för ett år eller tre års villkor</span><span class="sxs-lookup"><span data-stu-id="fb9e0-124">Better budgeting and forecasting with upfront payment for one-year or three-year terms</span></span>
- <span data-ttu-id="fb9e0-125">Prioriterad beräknings kapacitet i den Azure-region som ligger närmast deras kontor</span><span class="sxs-lookup"><span data-stu-id="fb9e0-125">Prioritized computing capacity in the Azure region closest to their offices</span></span>
- <span data-ttu-id="fb9e0-126">Azure-reservationer ger grunden för lösningar från slut punkt till slut punkt för infrastrukturen i kombination med program vara som Microsoft Windows Server och Azure SQL Database</span><span class="sxs-lookup"><span data-stu-id="fb9e0-126">Azure reservations provide the foundation for end to end infrastructure solutions when combined with software like Microsoft Windows Server and Azure SQL Database</span></span>

>[!NOTE]
> <span data-ttu-id="fb9e0-127">Du kan köpa, sälja och hantera Azure-reservationer i både Partner Center och Azure Portal och med hjälp av Partner Center API.</span><span class="sxs-lookup"><span data-stu-id="fb9e0-127">You can buy, sell, and manage Azure reservations in both the Partner Center and the Azure portal, and using the Partner Center API.</span></span> <span data-ttu-id="fb9e0-128">Du kan också ge dina kunder tillstånd att köpa sina egna Azure-reservationer från en Azure-prenumeration som du har köpt för dem.</span><span class="sxs-lookup"><span data-stu-id="fb9e0-128">You can also give your customers permission to buy their own Azure reservations from an Azure subscription you purchased for them.</span></span> <span data-ttu-id="fb9e0-129">Följ länkarna nedan för att lära dig hur.</span><span class="sxs-lookup"><span data-stu-id="fb9e0-129">Follow the links below to learn how.</span></span>

## <a name="azure-reservations-resources"></a><span data-ttu-id="fb9e0-130">Resurser för Azure-reservationer</span><span class="sxs-lookup"><span data-stu-id="fb9e0-130">Azure reservations resources</span></span>

|<span data-ttu-id="fb9e0-131">**För information om**</span><span class="sxs-lookup"><span data-stu-id="fb9e0-131">**For information about**</span></span>   |<span data-ttu-id="fb9e0-132">**Läs detta**</span><span class="sxs-lookup"><span data-stu-id="fb9e0-132">**Read this**</span></span>    |
|:-----------------------------|:-----------------|
| <span data-ttu-id="fb9e0-133">Dokumentation om Azure-reservationer för dina kunder</span><span class="sxs-lookup"><span data-stu-id="fb9e0-133">Azure reservations documentation for your customers</span></span> | [<span data-ttu-id="fb9e0-134">Vad är Azure-reservationer?</span><span class="sxs-lookup"><span data-stu-id="fb9e0-134">What are Azure reservations?</span></span>](/azure/billing/billing-save-compute-costs-reservations)
|<span data-ttu-id="fb9e0-135">Köpa Azure-reservationer för dina kunder i Partner Center</span><span class="sxs-lookup"><span data-stu-id="fb9e0-135">Purchasing Azure reservations for your customers in Partner Center</span></span>   |[<span data-ttu-id="fb9e0-136">Köp Azure-reservationer</span><span class="sxs-lookup"><span data-stu-id="fb9e0-136">Buy Azure reservations</span></span>](azure-reservations-buying.md)
|<span data-ttu-id="fb9e0-137">Hantera Azure-reservationer i Partner Center</span><span class="sxs-lookup"><span data-stu-id="fb9e0-137">Managing Azure reservations in Partner Center</span></span> | [<span data-ttu-id="fb9e0-138">Hantera Azure-reservationer i Partner Center</span><span class="sxs-lookup"><span data-stu-id="fb9e0-138">Managing Azure reservations in Partner Center</span></span>](azure-reservations-manage.md)
|<span data-ttu-id="fb9e0-139">Fastställa rätt VM-storlek och verifiera kunds VM-användning</span><span class="sxs-lookup"><span data-stu-id="fb9e0-139">Determining the correct VM size and verifying customer VM usage</span></span>   |[<span data-ttu-id="fb9e0-140">Storlek på virtuell dator för maximal användning av Azure-reservationer</span><span class="sxs-lookup"><span data-stu-id="fb9e0-140">VM sizing for maximum Azure reservation usage</span></span>](azure-usage.md)   |
|<span data-ttu-id="fb9e0-141">Köpa Azure-reservationer med partner Center API</span><span class="sxs-lookup"><span data-stu-id="fb9e0-141">Purchasing Azure reservations using the Partner Center API</span></span> | <span data-ttu-id="fb9e0-142">[Köp Azure Reserved VM instances](/partner-center/develop/purchase-azure-reservations) i dokumentationen för partner Center-utvecklare</span><span class="sxs-lookup"><span data-stu-id="fb9e0-142">[Purchase Azure Reserved VM Instances](/partner-center/develop/purchase-azure-reservations) in the Partner Center developer documentation</span></span>   |
|<span data-ttu-id="fb9e0-143">Ge kunderna tillstånd att köpa sina egna Azure-reservationer från din CSP-prenumeration.</span><span class="sxs-lookup"><span data-stu-id="fb9e0-143">Giving customers permission to buy their own Azure reservations from your CSP subscription.</span></span> | [<span data-ttu-id="fb9e0-144">Ge kunderna tillstånd att köpa sina egna Azure-reservationer</span><span class="sxs-lookup"><span data-stu-id="fb9e0-144">Give customers permission to buy their own Azure reservations</span></span>](give-customers-permission.md)   |