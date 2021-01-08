---
title: Köp kommersiella Marketplace-erbjudanden
ms.topic: how-to
ms.date: 05/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Lär dig hur CSP-programpartner kan använda Partner Center Marketplace för att göra kund inköp av SaaS-erbjudanden från oberoende program varu leverantörer (ISV).
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 841308d535d4071ee0a8eabf3e70325edea5777c
ms.sourcegitcommit: a78dd3c532860d01867d116bfb4e2c88b84bcd25
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 01/08/2021
ms.locfileid: "97979725"
---
# <a name="purchase-commercial-marketplace-products-for-your-customers-in-partner-center"></a><span data-ttu-id="93610-103">Köp kommersiella Marketplace-produkter för dina kunder i Partner Center</span><span class="sxs-lookup"><span data-stu-id="93610-103">Purchase commercial marketplace products for your customers in Partner Center</span></span>


<span data-ttu-id="93610-104">**Lämpliga roller**</span><span class="sxs-lookup"><span data-stu-id="93610-104">**Appropriate roles**</span></span>

- <span data-ttu-id="93610-105">Global administratör</span><span class="sxs-lookup"><span data-stu-id="93610-105">Global admin</span></span>
- <span data-ttu-id="93610-106">Administratörs agent</span><span class="sxs-lookup"><span data-stu-id="93610-106">Admin agent</span></span>

<span data-ttu-id="93610-107">Som partner i ett CSP-program (Cloud Solution Provider) kan du använda den kommersiella Marketplace för att köpa prenumerationer för dina kunder till vissa SaaS-produkter (Software as a Service) som erbjuds av oberoende program varu leverantörer (ISV).</span><span class="sxs-lookup"><span data-stu-id="93610-107">As a partner in the Cloud Solution Provider (CSP) program, you can use the commercial marketplace to purchase subscriptions for your customers to certain Software as a Service (SaaS) products offered by Independent Software Vendors (ISVs).</span></span>

<span data-ttu-id="93610-108">Genom att erbjuda ISV SaaS-prenumerationer till dina kunder kan du hjälpa företaget att särskilja din verksamhet.</span><span class="sxs-lookup"><span data-stu-id="93610-108">By offering ISV SaaS subscriptions to your customers, you can help differentiate your business.</span></span> <span data-ttu-id="93610-109">Du kan också ge kunderna till gång till program varu paket som åtgärdar sina specifika affärs behov.</span><span class="sxs-lookup"><span data-stu-id="93610-109">You can also give customers access to software bundles that address their specific business needs.</span></span> <span data-ttu-id="93610-110">Du hanterar licenser och prenumerationer för dessa Marketplace SaaS-produkter från ISV-utgivare, precis som du hanterar licenser och prenumerationer för Microsoft-produkter.</span><span class="sxs-lookup"><span data-stu-id="93610-110">You manage licenses and subscriptions for these marketplace SaaS products from ISV publishers just as you manage licenses and subscriptions for Microsoft products.</span></span>

<span data-ttu-id="93610-111">Du kan köpa antingen **licensbaserade** SaaS-prenumerationer eller **användnings baserade** prenumerationer.</span><span class="sxs-lookup"><span data-stu-id="93610-111">You can purchase either **license-based** SaaS subscriptions or **usage-based** subscriptions.</span></span> <span data-ttu-id="93610-112">Mer information om skillnaden mellan licensierad och Använd fakturering finns i [fakturerings grunderna](billing-basics.md).</span><span class="sxs-lookup"><span data-stu-id="93610-112">To learn more about the difference between license-based and usage-based billing, see [Billing basics](billing-basics.md).</span></span>

## <a name="purchase-license-based-and-metered-saas-subscriptions-in-partner-center"></a><span data-ttu-id="93610-113">Köp licensbaserade och avgiftsbelagda SaaS-prenumerationer i Partner Center</span><span class="sxs-lookup"><span data-stu-id="93610-113">Purchase license-based and metered SaaS subscriptions in Partner Center</span></span>

<span data-ttu-id="93610-114">Du köper prenumerationer för licensbaserade eller avgiftsbelagda SaaS-produkter som erbjuds av ISV-utgivare med samma process som du använder för att köpa prenumerationer för Microsoft-produkter.</span><span class="sxs-lookup"><span data-stu-id="93610-114">You purchase subscriptions for license-based or metered SaaS products offered by ISV publishers using the same process you use to purchase subscriptions for Microsoft products.</span></span>

<span data-ttu-id="93610-115">Om du vill köpa en licensierad eller avgiftsbelagd SaaS-prenumeration i Partner Center, se [skapa, pausa eller annullera kund prenumerationer](create-a-new-subscription.md#create-a-new-subscription).</span><span class="sxs-lookup"><span data-stu-id="93610-115">To purchase a license-based or metered SaaS subscription in Partner Center, see [Create, suspend, or cancel customer subscriptions](create-a-new-subscription.md#create-a-new-subscription).</span></span>

<span data-ttu-id="93610-116">Du kan också använda [API: er för partner Center](/partner-center/develop/) för att skapa prenumerationer på kommersiella marknads platser för dina kunder.</span><span class="sxs-lookup"><span data-stu-id="93610-116">You can also use [Partner Center APIs](/partner-center/develop/) to create commercial marketplace subscriptions for your customers.</span></span> <span data-ttu-id="93610-117">(Mer information om hur du använder API: er för partner Center finns i [skapa en prenumeration för kommersiella Marketplace-produkter](/partner-center/develop/create-subscription-azure-marketplace-products).)</span><span class="sxs-lookup"><span data-stu-id="93610-117">(For more info on using Partner Center APIs, see [Create a subscription for commercial marketplace products](/partner-center/develop/create-subscription-azure-marketplace-products).)</span></span>

>[!IMPORTANT]
> <span data-ttu-id="93610-118">Som partner i CSP-programmet kan du köpa **licensbaserade** eller **avgiftsbelagda** SaaS-prenumerationer från ISV-utgivare i Partner Center.</span><span class="sxs-lookup"><span data-stu-id="93610-118">As a partner in the CSP program, you can purchase **license-based** or **metered** SaaS subscriptions from ISV publishers within Partner Center.</span></span> <span data-ttu-id="93610-119">Det innebär att du kan köpa alla **licensbaserade** eller **avgiftsbelagda** SaaS-erbjudanden som ISV-utgivaren har gjort tillgängligt för dig, inklusive [exklusiva erbjudanden](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) som du har åtkomst till.</span><span class="sxs-lookup"><span data-stu-id="93610-119">This means you can purchase any **license-based** or **metered** SaaS offer the ISV publisher has made available to you, including [exclusive offers](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) to which you have access.</span></span> <span data-ttu-id="93610-120">För att köpa eller hantera andra erbjudanden från kommersiella Marketplace från ISV: er (till exempel användnings erbjudanden som rör Azure-program, behållare eller virtuella datorer) måste du gå till [Azure Portal](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="93610-120">To purchase or manage other, commercial marketplace offers from ISVs (such as usage-based offers involving Azure applications, Containers or VMs), you must go to the [Azure portal](https://portal.azure.com/).</span></span>

## <a name="purchase-usage-based-subscriptions-in-the-azure-portal"></a><span data-ttu-id="93610-121">Köp användnings prenumerationer i Azure Portal</span><span class="sxs-lookup"><span data-stu-id="93610-121">Purchase usage-based subscriptions in the Azure portal</span></span>

<span data-ttu-id="93610-122">Till skillnad från SaaS-prenumerationer från tredjeparts ISV-utgivare kräver användnings-baserade prenumerationer först en kund som har en Azure-prenumeration.</span><span class="sxs-lookup"><span data-stu-id="93610-122">In contrast to license-based SaaS subscriptions from third-party ISV publishers, usage-based subscriptions first require a customer to have an Azure subscription.</span></span> <span data-ttu-id="93610-123">Fakturering för kommersiell marknads plats är användnings baserade resurser under kundens Azure-prenumeration.</span><span class="sxs-lookup"><span data-stu-id="93610-123">Billing for commercial marketplace, usage-based resources falls under the customer's Azure subscription.</span></span> <span data-ttu-id="93610-124">När kunden har en Azure-prenumeration kan en partner i CSP-programmet följa de här stegen för att köpa en prenumeration på kommersiell marknads plats för dem:</span><span class="sxs-lookup"><span data-stu-id="93610-124">Once your customer has an Azure subscription, a partner in the CSP program can follow these steps to purchase a commercial marketplace subscription for them:</span></span>

1. <span data-ttu-id="93610-125">Logga in på Partner Center- [instrumentpanelen](https://partner.microsoft.com/dashboard)och välj sedan **kunder** på menyn till vänster.</span><span class="sxs-lookup"><span data-stu-id="93610-125">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard), then select **Customers** from the left-hand menu.</span></span>

2. <span data-ttu-id="93610-126">Välj den specifika kunden och välj sedan **prenumerationer**.</span><span class="sxs-lookup"><span data-stu-id="93610-126">Select the specific customer, then select **Subscriptions**.</span></span>  

3. <span data-ttu-id="93610-127">Under de **användnings baserade prenumerationerna** väljer du **alla resurser**.</span><span class="sxs-lookup"><span data-stu-id="93610-127">Under the **Usage-based subscriptions**, select **All resources**.</span></span> <span data-ttu-id="93610-128">Då går du till hanterings portalen för Azure.</span><span class="sxs-lookup"><span data-stu-id="93610-128">This takes you to the Azure Management portal.</span></span>

4. <span data-ttu-id="93610-129">I hanterings portalen för Azure väljer du **skapa en resurs** i den vänstra menyn.</span><span class="sxs-lookup"><span data-stu-id="93610-129">In the Azure Management portal, select **Create a resource** from the left-hand menu.</span></span>

5. <span data-ttu-id="93610-130">Välj **Se alla** överst i listan Azure Marketplace.</span><span class="sxs-lookup"><span data-stu-id="93610-130">Select **See all** at the top of the Azure Marketplace list.</span></span>

6. <span data-ttu-id="93610-131">Om du vill begränsa listan använder du filter överst i Marketplace-listan.</span><span class="sxs-lookup"><span data-stu-id="93610-131">To narrow your list, use filters at the top of the Marketplace list.</span></span> <span data-ttu-id="93610-132">Du kan till exempel välja **Microsoft** eller **partner** i list rutan **utgivare** om du bara vill visa erbjudanden från Microsoft eller från en ISV-utgivare.</span><span class="sxs-lookup"><span data-stu-id="93610-132">For example, you can select **Microsoft** or **Partner** from the **Publisher** dropdown list to view only offers from Microsoft or those from an ISV publisher.</span></span>

7. <span data-ttu-id="93610-133">Välj ett Special erbjudande och välj sedan **skapa**.</span><span class="sxs-lookup"><span data-stu-id="93610-133">Choose a specific offer, then select **Create**.</span></span>

## <a name="next-steps"></a><span data-ttu-id="93610-134">Nästa steg</span><span class="sxs-lookup"><span data-stu-id="93610-134">Next steps</span></span>

- [<span data-ttu-id="93610-135">Hantera kommersiella Marketplace-erbjudanden</span><span class="sxs-lookup"><span data-stu-id="93610-135">Manage commercial marketplace offers</span></span>](csp-commercial-marketplace-purchase.md)