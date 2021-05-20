---
title: Sälja kunder Microsoft Azure reservationer
description: Som en Molnlösningsleverantör kan du köpa, sälja eller hantera Azure-reservationer för kunder. Använd Partner Center, Azure Portal eller Partner Center-API:et.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 08/06/2020
ms.openlocfilehash: b97cafea9ad2f36718418c7c7cfca5f91ee8849c
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 05/19/2021
ms.locfileid: "110149476"
---
# <a name="sell-microsoft-azure-reservations-to-customers-using-partner-center-the-azure-portal-or-apis"></a><span data-ttu-id="0a1c4-104">Sälja Microsoft Azure reservationer till kunder med partnercenter, Azure Portal eller API:er</span><span class="sxs-lookup"><span data-stu-id="0a1c4-104">Sell Microsoft Azure reservations to customers using Partner Center, the Azure portal, or APIs</span></span>

<span data-ttu-id="0a1c4-105">**Lämpliga roller:** Administratörsagent | Global | Supportagent | Försäljningsagentens | Administratör för användarhantering</span><span class="sxs-lookup"><span data-stu-id="0a1c4-105">**Appropriate roles**: Admin agent | Global admin | Helpdesk agent | Sales agent | User management admin</span></span>

<span data-ttu-id="0a1c4-106">Som partner i Molnlösningsleverantör program (CSP) kan du köpa, sälja eller hantera Azure-reservationer för kunder.</span><span class="sxs-lookup"><span data-stu-id="0a1c4-106">As a partner in the Cloud Solution Provider program (CSP), you can buy, sell, or manage Azure reservations for customers.</span></span> <span data-ttu-id="0a1c4-107">Använd Partner Center, Azure Portal eller Partner Center-API:et.</span><span class="sxs-lookup"><span data-stu-id="0a1c4-107">Use Partner Center, the Azure portal, or the Partner Center API.</span></span>

> [!NOTE]
> <span data-ttu-id="0a1c4-108">Den här artikeln gäller endast för partner i CSP.</span><span class="sxs-lookup"><span data-stu-id="0a1c4-108">This article applies only to partners in CSP.</span></span> <span data-ttu-id="0a1c4-109">Kunder som använder andra typer av prenumerationer (till exempel prenumerationer med användningsbaserade betalning, enskilda prenumerationer, Microsoft-kundavtal- eller Enterprise-avtal) bör i stället läsa dokumentationen om [Azure-reservationer.](/azure/cost-management-billing/reservations)</span><span class="sxs-lookup"><span data-stu-id="0a1c4-109">Customers using other types of subscriptions (such as, pay-as-you-go, individual, Microsoft Customer Agreement, or Enterprise Agreement subscriptions) should instead read [this Azure reservations documentation](/azure/cost-management-billing/reservations).</span></span>

<span data-ttu-id="0a1c4-110">Partner i CSP-programmet kan erbjuda sina kunder Microsoft Azure reservationer.</span><span class="sxs-lookup"><span data-stu-id="0a1c4-110">Partners in the CSP program can offer their customers Microsoft Azure reservations.</span></span> <span data-ttu-id="0a1c4-111">Kunder kan få betydande besparingar när de reserverar i förväg.</span><span class="sxs-lookup"><span data-stu-id="0a1c4-111">Customers can gain significant savings when they reserve in advance.</span></span> <span data-ttu-id="0a1c4-112">Azure-reservationer erbjuder kunderna enkelhet och flexibilitet på följande sätt:</span><span class="sxs-lookup"><span data-stu-id="0a1c4-112">Azure reservations offer customers simplicity and flexibility in the following ways:</span></span>

- <span data-ttu-id="0a1c4-113">Ett eller tre års reservationsvillkor</span><span class="sxs-lookup"><span data-stu-id="0a1c4-113">One or three-year reservation terms</span></span>
- <span data-ttu-id="0a1c4-114">Lätt att komma igång; installationen slutfördes på några sekunder</span><span class="sxs-lookup"><span data-stu-id="0a1c4-114">Easy to get started; setup completed in seconds</span></span>
- <span data-ttu-id="0a1c4-115">Avbryta eller byta ut reserverade instanser när som helst för justerad återbetalning</span><span class="sxs-lookup"><span data-stu-id="0a1c4-115">Cancel or exchange reserved instances at any time for adjusted refund</span></span>
- <span data-ttu-id="0a1c4-116">Hantera användning av reserverade instanser på organisations- eller avdelningsnivå</span><span class="sxs-lookup"><span data-stu-id="0a1c4-116">Manage reserved instances usage at the organizational or individual department level</span></span>

<span data-ttu-id="0a1c4-117">Azure-reservationer kan tilltala kunder på följande sätt:</span><span class="sxs-lookup"><span data-stu-id="0a1c4-117">Azure reservations can appeal to customers in the following ways:</span></span>

- <span data-ttu-id="0a1c4-118">Reservationer kan ge betydande besparingar i prissättningen för betala per användning (PAYG)</span><span class="sxs-lookup"><span data-stu-id="0a1c4-118">Reservations can offer significant savings over pay-as-you-go (PAYG) pricing</span></span>
- <span data-ttu-id="0a1c4-119">Bättre budgetering och prognostiserade prognoser med förskottsbetalning för ett eller tre år</span><span class="sxs-lookup"><span data-stu-id="0a1c4-119">Better budgeting and forecasting with upfront payment for one-year or three-year terms</span></span>
- <span data-ttu-id="0a1c4-120">Prioriterad databehandlingskapacitet i Den Azure-region som är närmast deras kontor</span><span class="sxs-lookup"><span data-stu-id="0a1c4-120">Prioritized computing capacity in the Azure region closest to their offices</span></span>
- <span data-ttu-id="0a1c4-121">Azure-reservationer utgör grunden för hela infrastrukturlösningar i kombination med programvara som Microsoft Windows Server och Azure SQL Database</span><span class="sxs-lookup"><span data-stu-id="0a1c4-121">Azure reservations provide the foundation for end to end infrastructure solutions when combined with software like Microsoft Windows Server and Azure SQL Database</span></span>

>[!NOTE]
> <span data-ttu-id="0a1c4-122">Du kan köpa, sälja och hantera Azure-reservationer i både Partnercenter och Azure Portal och med partnercenter-API:et.</span><span class="sxs-lookup"><span data-stu-id="0a1c4-122">You can buy, sell, and manage Azure reservations in both the Partner Center and the Azure portal, and using the Partner Center API.</span></span> <span data-ttu-id="0a1c4-123">Du kan också ge dina kunder behörighet att köpa sina egna Azure-reservationer från en Azure-prenumeration som du har köpt åt dem.</span><span class="sxs-lookup"><span data-stu-id="0a1c4-123">You can also give your customers permission to buy their own Azure reservations from an Azure subscription you purchased for them.</span></span> <span data-ttu-id="0a1c4-124">Följ länkarna nedan för att lära dig hur du gör.</span><span class="sxs-lookup"><span data-stu-id="0a1c4-124">Follow the links below to learn how.</span></span>

## <a name="azure-reservations-resources"></a><span data-ttu-id="0a1c4-125">Resurser för Azure-reservationer</span><span class="sxs-lookup"><span data-stu-id="0a1c4-125">Azure reservations resources</span></span>

|<span data-ttu-id="0a1c4-126">**För information om**</span><span class="sxs-lookup"><span data-stu-id="0a1c4-126">**For information about**</span></span>   |<span data-ttu-id="0a1c4-127">**Läs detta**</span><span class="sxs-lookup"><span data-stu-id="0a1c4-127">**Read this**</span></span>    |
|:-----------------------------|:-----------------|
| <span data-ttu-id="0a1c4-128">Dokumentation om Azure-reservationer för dina kunder</span><span class="sxs-lookup"><span data-stu-id="0a1c4-128">Azure reservations documentation for your customers</span></span> | [<span data-ttu-id="0a1c4-129">Vad är Azure-reservationer?</span><span class="sxs-lookup"><span data-stu-id="0a1c4-129">What are Azure reservations?</span></span>](/azure/billing/billing-save-compute-costs-reservations)
|<span data-ttu-id="0a1c4-130">Köpa Azure-reservationer för dina kunder i Partnercenter</span><span class="sxs-lookup"><span data-stu-id="0a1c4-130">Purchasing Azure reservations for your customers in Partner Center</span></span>   |[<span data-ttu-id="0a1c4-131">Köpa Azure-reservationer</span><span class="sxs-lookup"><span data-stu-id="0a1c4-131">Buy Azure reservations</span></span>](azure-reservations-buying.md)
|<span data-ttu-id="0a1c4-132">Hantera Azure-reservationer i Partnercenter</span><span class="sxs-lookup"><span data-stu-id="0a1c4-132">Managing Azure reservations in Partner Center</span></span> | [<span data-ttu-id="0a1c4-133">Hantera Azure-reservationer i Partnercenter</span><span class="sxs-lookup"><span data-stu-id="0a1c4-133">Managing Azure reservations in Partner Center</span></span>](azure-reservations-manage.md)
|<span data-ttu-id="0a1c4-134">Fastställa rätt VM-storlek och verifiera kundens VM-användning</span><span class="sxs-lookup"><span data-stu-id="0a1c4-134">Determining the correct VM size and verifying customer VM usage</span></span>   |[<span data-ttu-id="0a1c4-135">VM-storlek för maximal användning av Azure-reservationer</span><span class="sxs-lookup"><span data-stu-id="0a1c4-135">VM sizing for maximum Azure reservation usage</span></span>](azure-usage.md)   |
|<span data-ttu-id="0a1c4-136">Köpa Azure-reservationer med partnercenter-API:et</span><span class="sxs-lookup"><span data-stu-id="0a1c4-136">Purchasing Azure reservations using the Partner Center API</span></span> | <span data-ttu-id="0a1c4-137">[Köp Azure Reserved VM Instances](/partner-center/develop/purchase-azure-reservations) i utvecklardokumentationen för Partnercenter</span><span class="sxs-lookup"><span data-stu-id="0a1c4-137">[Purchase Azure Reserved VM Instances](/partner-center/develop/purchase-azure-reservations) in the Partner Center developer documentation</span></span>   |
|<span data-ttu-id="0a1c4-138">Ge kunderna tillstånd att köpa sina egna Azure-reservationer från din CSP-prenumeration.</span><span class="sxs-lookup"><span data-stu-id="0a1c4-138">Giving customers permission to buy their own Azure reservations from your CSP subscription.</span></span> | [<span data-ttu-id="0a1c4-139">Ge kunderna behörighet att köpa sina egna Azure-reservationer</span><span class="sxs-lookup"><span data-stu-id="0a1c4-139">Give customers permission to buy their own Azure reservations</span></span>](give-customers-permission.md)   |