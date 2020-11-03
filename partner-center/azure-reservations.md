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
ms.openlocfilehash: 317d1f0295b79b79bf06f1091ae365bc7012b749
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/22/2020
ms.locfileid: "92531628"
---
# <a name="sell-microsoft-azure-reservations-to-customers-using-partner-center-the-azure-portal-or-apis"></a><span data-ttu-id="86408-104">Sälj Microsoft Azure reservationer till kunder som använder Partner Center, Azure Portal eller API: er</span><span class="sxs-lookup"><span data-stu-id="86408-104">Sell Microsoft Azure reservations to customers using Partner Center, the Azure portal, or APIs</span></span>

<span data-ttu-id="86408-105">**Gäller för**</span><span class="sxs-lookup"><span data-stu-id="86408-105">**Applies to**</span></span>

- <span data-ttu-id="86408-106">Partnercenter</span><span class="sxs-lookup"><span data-stu-id="86408-106">Partner Center</span></span>
- <span data-ttu-id="86408-107">Microsoft Azure-portalen</span><span class="sxs-lookup"><span data-stu-id="86408-107">Microsoft Azure portal</span></span>
- <span data-ttu-id="86408-108">Partner i CSP-programmet</span><span class="sxs-lookup"><span data-stu-id="86408-108">Partners in the CSP program</span></span>

<span data-ttu-id="86408-109">**Lämpliga roller**</span><span class="sxs-lookup"><span data-stu-id="86408-109">**Appropriate roles**</span></span>

- <span data-ttu-id="86408-110">Administratörs agent</span><span class="sxs-lookup"><span data-stu-id="86408-110">Admin agent</span></span>
- <span data-ttu-id="86408-111">Global administratör</span><span class="sxs-lookup"><span data-stu-id="86408-111">Global admin</span></span>
- <span data-ttu-id="86408-112">Support agent</span><span class="sxs-lookup"><span data-stu-id="86408-112">Helpdesk agent</span></span>
- <span data-ttu-id="86408-113">Försäljnings agent</span><span class="sxs-lookup"><span data-stu-id="86408-113">Sales agent</span></span>
- <span data-ttu-id="86408-114">Administratör för användar hantering</span><span class="sxs-lookup"><span data-stu-id="86408-114">User management admin</span></span>

> [!NOTE]
> <span data-ttu-id="86408-115">Den här artikeln gäller endast partner i Cloud Solution Provider (CSP)-programmet.</span><span class="sxs-lookup"><span data-stu-id="86408-115">This article applies only to partners in the Cloud Solution Provider (CSP) program.</span></span> <span data-ttu-id="86408-116">Kunder som använder andra typer av prenumerationer (t. ex. betala per användning, enskilda, Microsoft-kundavtal eller Enterprise-avtal prenumerationer) bör i stället läsa [denna dokumentation om Azure-reservationer](/azure/cost-management-billing/reservations).</span><span class="sxs-lookup"><span data-stu-id="86408-116">Customers using other types of subscriptions (such as, pay-as-you-go, individual, Microsoft Customer Agreement, or Enterprise Agreement subscriptions) should instead read [this Azure reservations documentation](/azure/cost-management-billing/reservations).</span></span>

<span data-ttu-id="86408-117">Partner i CSP-programmet kan erbjuda sina kunder Microsoft Azure reservationer.</span><span class="sxs-lookup"><span data-stu-id="86408-117">Partners in the CSP program can offer their customers Microsoft Azure reservations.</span></span> <span data-ttu-id="86408-118">Kunder kan få betydande besparingar när de reserverar i förväg.</span><span class="sxs-lookup"><span data-stu-id="86408-118">Customers can gain significant savings when they reserve in advance.</span></span> <span data-ttu-id="86408-119">Azure-reservationer ger kunderna enkelhet och flexibilitet på följande sätt:</span><span class="sxs-lookup"><span data-stu-id="86408-119">Azure reservations offer customers simplicity and flexibility in the following ways:</span></span>

- <span data-ttu-id="86408-120">En eller tre års reservations villkor</span><span class="sxs-lookup"><span data-stu-id="86408-120">One or three-year reservation terms</span></span>
- <span data-ttu-id="86408-121">Lätt att komma igång; installationen slutfördes på några sekunder</span><span class="sxs-lookup"><span data-stu-id="86408-121">Easy to get started; setup completed in seconds</span></span>
- <span data-ttu-id="86408-122">Avbryta eller byta ut reserverade instanser när som helst för justerad åter betalning</span><span class="sxs-lookup"><span data-stu-id="86408-122">Cancel or exchange reserved instances at any time for adjusted refund</span></span>
- <span data-ttu-id="86408-123">Hantera användning av reserverade instanser på organisations-eller individuell avdelnings nivå</span><span class="sxs-lookup"><span data-stu-id="86408-123">Manage reserved instances usage at the organizational or individual department level</span></span>

<span data-ttu-id="86408-124">Azure-reservationer kan överklaga till kunder på följande sätt:</span><span class="sxs-lookup"><span data-stu-id="86408-124">Azure reservations can appeal to customers in the following ways:</span></span>

- <span data-ttu-id="86408-125">Reservationer kan erbjuda betydande besparingar jämfört med PAYG-priser (betala per användning)</span><span class="sxs-lookup"><span data-stu-id="86408-125">Reservations can offer significant savings over pay-as-you-go (PAYG) pricing</span></span>
- <span data-ttu-id="86408-126">Bättre budgetering och prognostisering med förskotts betalning för ett år eller tre års villkor</span><span class="sxs-lookup"><span data-stu-id="86408-126">Better budgeting and forecasting with upfront payment for one-year or three-year terms</span></span>
- <span data-ttu-id="86408-127">Prioriterad beräknings kapacitet i den Azure-region som ligger närmast deras kontor</span><span class="sxs-lookup"><span data-stu-id="86408-127">Prioritized computing capacity in the Azure region closest to their offices</span></span>
- <span data-ttu-id="86408-128">Azure-reservationer ger grunden för lösningar från slut punkt till slut punkt för infrastrukturen i kombination med program vara som Microsoft Windows Server och Azure SQL Database</span><span class="sxs-lookup"><span data-stu-id="86408-128">Azure reservations provide the foundation for end to end infrastructure solutions when combined with software like Microsoft Windows Server and Azure SQL Database</span></span>

>[!NOTE]
> <span data-ttu-id="86408-129">Du kan köpa, sälja och hantera Azure-reservationer i både Partner Center och Azure Portal och med hjälp av Partner Center API.</span><span class="sxs-lookup"><span data-stu-id="86408-129">You can buy, sell, and manage Azure reservations in both the Partner Center and the Azure portal, and using the Partner Center API.</span></span> <span data-ttu-id="86408-130">Du kan också ge dina kunder tillstånd att köpa sina egna Azure-reservationer från en Azure-prenumeration som du har köpt för dem.</span><span class="sxs-lookup"><span data-stu-id="86408-130">You can also give your customers permission to buy their own Azure reservations from an Azure subscription you purchased for them.</span></span> <span data-ttu-id="86408-131">Följ länkarna nedan för att lära dig hur.</span><span class="sxs-lookup"><span data-stu-id="86408-131">Follow the links below to learn how.</span></span>

## <a name="azure-reservations-resources"></a><span data-ttu-id="86408-132">Resurser för Azure-reservationer</span><span class="sxs-lookup"><span data-stu-id="86408-132">Azure reservations resources</span></span>

|<span data-ttu-id="86408-133">**För information om**</span><span class="sxs-lookup"><span data-stu-id="86408-133">**For information about**</span></span>   |<span data-ttu-id="86408-134">**Läs detta**</span><span class="sxs-lookup"><span data-stu-id="86408-134">**Read this**</span></span>    |
|:-----------------------------|:-----------------|
| <span data-ttu-id="86408-135">Dokumentation om Azure-reservationer för dina kunder</span><span class="sxs-lookup"><span data-stu-id="86408-135">Azure reservations documentation for your customers</span></span> | [<span data-ttu-id="86408-136">Vad är Azure-reservationer?</span><span class="sxs-lookup"><span data-stu-id="86408-136">What are Azure reservations?</span></span>](/azure/billing/billing-save-compute-costs-reservations)
|<span data-ttu-id="86408-137">Köpa Azure-reservationer för dina kunder i Partner Center</span><span class="sxs-lookup"><span data-stu-id="86408-137">Purchasing Azure reservations for your customers in Partner Center</span></span>   |[<span data-ttu-id="86408-138">Köp Azure-reservationer</span><span class="sxs-lookup"><span data-stu-id="86408-138">Buy Azure reservations</span></span>](azure-reservations-buying.md)
|<span data-ttu-id="86408-139">Hantera Azure-reservationer i Partner Center</span><span class="sxs-lookup"><span data-stu-id="86408-139">Managing Azure reservations in Partner Center</span></span> | [<span data-ttu-id="86408-140">Hantera Azure-reservationer i Partner Center</span><span class="sxs-lookup"><span data-stu-id="86408-140">Managing Azure reservations in Partner Center</span></span>](azure-reservations-manage.md)
|<span data-ttu-id="86408-141">Fastställa rätt VM-storlek och verifiera kunds VM-användning</span><span class="sxs-lookup"><span data-stu-id="86408-141">Determining the correct VM size and verifying customer VM usage</span></span>   |[<span data-ttu-id="86408-142">Storlek på virtuell dator för maximal användning av Azure-reservationer</span><span class="sxs-lookup"><span data-stu-id="86408-142">VM sizing for maximum Azure reservation usage</span></span>](azure-usage.md)   |
|<span data-ttu-id="86408-143">Köpa Azure-reservationer med partner Center API</span><span class="sxs-lookup"><span data-stu-id="86408-143">Purchasing Azure reservations using the Partner Center API</span></span> | <span data-ttu-id="86408-144">[Köp Azure Reserved VM instances](/partner-center/develop/purchase-azure-reservations) i dokumentationen för partner Center-utvecklare</span><span class="sxs-lookup"><span data-stu-id="86408-144">[Purchase Azure Reserved VM Instances](/partner-center/develop/purchase-azure-reservations) in the Partner Center developer documentation</span></span>   |
|<span data-ttu-id="86408-145">Ge kunderna tillstånd att köpa sina egna Azure-reservationer från din CSP-prenumeration.</span><span class="sxs-lookup"><span data-stu-id="86408-145">Giving customers permission to buy their own Azure reservations from your CSP subscription.</span></span> | [<span data-ttu-id="86408-146">Ge kunderna tillstånd att köpa sina egna Azure-reservationer</span><span class="sxs-lookup"><span data-stu-id="86408-146">Give customers permission to buy their own Azure reservations</span></span>](give-customers-permission.md)   |