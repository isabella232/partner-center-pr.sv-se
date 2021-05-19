---
title: Köpa erbjudanden på den kommersiella marknadsplatsen
ms.topic: how-to
ms.date: 05/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Lär dig hur CSP-programpartner kan använda Partner Center Marketplace för att göra kundköp av SaaS-erbjudanden från oberoende programvaruleverantörer (ISV).
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 3f5cf4895fa4d66c65215989d808a1dd18ef9064
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 05/19/2021
ms.locfileid: "110147861"
---
# <a name="purchase-commercial-marketplace-products-for-your-customers-in-partner-center"></a><span data-ttu-id="71650-103">Köpa produkter på den kommersiella marknadsplatsen för dina kunder i Partnercenter</span><span class="sxs-lookup"><span data-stu-id="71650-103">Purchase commercial marketplace products for your customers in Partner Center</span></span>


<span data-ttu-id="71650-104">**Lämpliga roller:** Globala | Administratörsagent</span><span class="sxs-lookup"><span data-stu-id="71650-104">**Appropriate roles**: Global admin | Admin agent</span></span>

<span data-ttu-id="71650-105">Som partner i programmet Molnlösningsleverantör (CSP) kan du använda den kommersiella marknadsplatsen för att köpa prenumerationer för dina kunder till vissa SaaS-produkter (Programvara som en tjänst) som erbjuds av oberoende programvaruleverantörer (ISV:er).</span><span class="sxs-lookup"><span data-stu-id="71650-105">As a partner in the Cloud Solution Provider (CSP) program, you can use the commercial marketplace to purchase subscriptions for your customers to certain Software as a Service (SaaS) products offered by Independent Software Vendors (ISVs).</span></span>

<span data-ttu-id="71650-106">Genom att erbjuda ISV SaaS-prenumerationer till dina kunder kan du hjälpa till att särskilja din verksamhet.</span><span class="sxs-lookup"><span data-stu-id="71650-106">By offering ISV SaaS subscriptions to your customers, you can help differentiate your business.</span></span> <span data-ttu-id="71650-107">Du kan också ge kunderna åtkomst till programvarupaket som tillgodoser deras specifika affärsbehov.</span><span class="sxs-lookup"><span data-stu-id="71650-107">You can also give customers access to software bundles that address their specific business needs.</span></span> <span data-ttu-id="71650-108">Du hanterar licenser och prenumerationer för dessa Marketplace SaaS-produkter från ISV-utgivare på samma sätt som du hanterar licenser och prenumerationer för Microsoft-produkter.</span><span class="sxs-lookup"><span data-stu-id="71650-108">You manage licenses and subscriptions for these marketplace SaaS products from ISV publishers just as you manage licenses and subscriptions for Microsoft products.</span></span>

<span data-ttu-id="71650-109">Du kan köpa **antingen licensbaserade** SaaS-prenumerationer **eller användningsbaserade** prenumerationer.</span><span class="sxs-lookup"><span data-stu-id="71650-109">You can purchase either **license-based** SaaS subscriptions or **usage-based** subscriptions.</span></span> <span data-ttu-id="71650-110">Mer information om skillnaden mellan licensbaserad och användningsbaserad fakturering finns i [Fakturerings grunder.](billing-basics.md)</span><span class="sxs-lookup"><span data-stu-id="71650-110">To learn more about the difference between license-based and usage-based billing, see [Billing basics](billing-basics.md).</span></span>

## <a name="purchase-license-based-and-metered-saas-subscriptions-in-partner-center"></a><span data-ttu-id="71650-111">Köpa licensbaserade och uppmätta SaaS-prenumerationer i Partnercenter</span><span class="sxs-lookup"><span data-stu-id="71650-111">Purchase license-based and metered SaaS subscriptions in Partner Center</span></span>

<span data-ttu-id="71650-112">Du köper prenumerationer för licensbaserade eller uppmätta SaaS-produkter som erbjuds av ISV-utgivare med samma process som du använder för att köpa prenumerationer för Microsoft-produkter.</span><span class="sxs-lookup"><span data-stu-id="71650-112">You purchase subscriptions for license-based or metered SaaS products offered by ISV publishers using the same process you use to purchase subscriptions for Microsoft products.</span></span>

<span data-ttu-id="71650-113">Om du vill köpa en licensbaserad eller uppmätt SaaS-prenumeration i Partnercenter kan du läsa [Skapa, pausa eller avbryta kundprenumerationer.](create-a-new-subscription.md#create-a-new-subscription)</span><span class="sxs-lookup"><span data-stu-id="71650-113">To purchase a license-based or metered SaaS subscription in Partner Center, see [Create, suspend, or cancel customer subscriptions](create-a-new-subscription.md#create-a-new-subscription).</span></span>

<span data-ttu-id="71650-114">Du kan också använda [Partner Center-API:er för](/partner-center/develop/) att skapa prenumerationer på den kommersiella marknadsplatsen för dina kunder.</span><span class="sxs-lookup"><span data-stu-id="71650-114">You can also use [Partner Center APIs](/partner-center/develop/) to create commercial marketplace subscriptions for your customers.</span></span> <span data-ttu-id="71650-115">(Mer information om hur du använder Partner Center-API:er finns i [Skapa en prenumeration för produkter på den kommersiella marknadsplatsen](/partner-center/develop/create-subscription-azure-marketplace-products).)</span><span class="sxs-lookup"><span data-stu-id="71650-115">(For more info on using Partner Center APIs, see [Create a subscription for commercial marketplace products](/partner-center/develop/create-subscription-azure-marketplace-products).)</span></span>

>[!IMPORTANT]
> <span data-ttu-id="71650-116">Som partner i CSP-programmet kan du köpa  licensbaserade eller uppmätta SaaS-prenumerationer från **ISV-utgivare** i Partnercenter.</span><span class="sxs-lookup"><span data-stu-id="71650-116">As a partner in the CSP program, you can purchase **license-based** or **metered** SaaS subscriptions from ISV publishers within Partner Center.</span></span> <span data-ttu-id="71650-117">Det innebär att du kan köpa alla licensbaserade eller **uppmätta** SaaS-erbjudanden [](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) som **ISV-utgivaren** har gjort tillgängliga för dig, inklusive exklusiva erbjudanden som du har åtkomst till.</span><span class="sxs-lookup"><span data-stu-id="71650-117">This means you can purchase any **license-based** or **metered** SaaS offer the ISV publisher has made available to you, including [exclusive offers](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) to which you have access.</span></span> <span data-ttu-id="71650-118">Om du vill köpa eller hantera andra erbjudanden på den kommersiella marknadsplatsen från ISV:er (till exempel användningsbaserade erbjudanden som rör Azure-program, containrar eller virtuella datorer) måste du [gå till Azure Portal](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="71650-118">To purchase or manage other, commercial marketplace offers from ISVs (such as usage-based offers involving Azure applications, Containers or VMs), you must go to the [Azure portal](https://portal.azure.com/).</span></span>

## <a name="purchase-usage-based-subscriptions-in-the-azure-portal"></a><span data-ttu-id="71650-119">Köpa användningsbaserade prenumerationer i Azure Portal</span><span class="sxs-lookup"><span data-stu-id="71650-119">Purchase usage-based subscriptions in the Azure portal</span></span>

<span data-ttu-id="71650-120">Till skillnad från licensbaserade SaaS-prenumerationer från tredjeparts ISV-utgivare kräver användningsbaserade prenumerationer först att kunden har en Azure-prenumeration.</span><span class="sxs-lookup"><span data-stu-id="71650-120">In contrast to license-based SaaS subscriptions from third-party ISV publishers, usage-based subscriptions first require a customer to have an Azure subscription.</span></span> <span data-ttu-id="71650-121">Fakturering för den kommersiella marknadsplatsen, användningsbaserade resurser faller under kundens Azure-prenumeration.</span><span class="sxs-lookup"><span data-stu-id="71650-121">Billing for commercial marketplace, usage-based resources falls under the customer's Azure subscription.</span></span> <span data-ttu-id="71650-122">När kunden har en Azure-prenumeration kan en partner i CSP-programmet följa dessa steg för att köpa en prenumeration på den kommersiella marknadsplatsen för dem:</span><span class="sxs-lookup"><span data-stu-id="71650-122">Once your customer has an Azure subscription, a partner in the CSP program can follow these steps to purchase a commercial marketplace subscription for them:</span></span>

1. <span data-ttu-id="71650-123">Logga in på [instrumentpanelen i Partnercenter](https://partner.microsoft.com/dashboard)och **välj** sedan Kunder på den vänstra menyn.</span><span class="sxs-lookup"><span data-stu-id="71650-123">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard), then select **Customers** from the left-hand menu.</span></span>

2. <span data-ttu-id="71650-124">Välj den specifika kunden och välj sedan **Prenumerationer.**</span><span class="sxs-lookup"><span data-stu-id="71650-124">Select the specific customer, then select **Subscriptions**.</span></span>  

3. <span data-ttu-id="71650-125">Under **Användningsbaserade prenumerationer väljer** du **Alla resurser**.</span><span class="sxs-lookup"><span data-stu-id="71650-125">Under the **Usage-based subscriptions**, select **All resources**.</span></span> <span data-ttu-id="71650-126">Då kommer du till Azure-hanteringsportalen.</span><span class="sxs-lookup"><span data-stu-id="71650-126">This takes you to the Azure Management portal.</span></span>

4. <span data-ttu-id="71650-127">I Azure-hanteringsportalen **väljer du Skapa en** resurs på den vänstra menyn.</span><span class="sxs-lookup"><span data-stu-id="71650-127">In the Azure Management portal, select **Create a resource** from the left-hand menu.</span></span>

5. <span data-ttu-id="71650-128">Välj **Visa alla** överst i listan Azure Marketplace listan.</span><span class="sxs-lookup"><span data-stu-id="71650-128">Select **See all** at the top of the Azure Marketplace list.</span></span>

6. <span data-ttu-id="71650-129">Om du vill begränsa listan använder du filter överst i Marketplace-listan.</span><span class="sxs-lookup"><span data-stu-id="71650-129">To narrow your list, use filters at the top of the Marketplace list.</span></span> <span data-ttu-id="71650-130">Du kan till exempel välja **Microsoft** eller **Partner** i listrutan **Utgivare** om du bara vill visa erbjudanden från Microsoft eller från en ISV-utgivare.</span><span class="sxs-lookup"><span data-stu-id="71650-130">For example, you can select **Microsoft** or **Partner** from the **Publisher** dropdown list to view only offers from Microsoft or those from an ISV publisher.</span></span>

7. <span data-ttu-id="71650-131">Välj ett specifikt erbjudande och välj sedan **Skapa.**</span><span class="sxs-lookup"><span data-stu-id="71650-131">Choose a specific offer, then select **Create**.</span></span>

## <a name="next-steps"></a><span data-ttu-id="71650-132">Nästa steg</span><span class="sxs-lookup"><span data-stu-id="71650-132">Next steps</span></span>

- [<span data-ttu-id="71650-133">Hantera erbjudanden på den kommersiella marknadsplatsen</span><span class="sxs-lookup"><span data-stu-id="71650-133">Manage commercial marketplace offers</span></span>](csp-commercial-marketplace-purchase.md)