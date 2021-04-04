---
title: Migrera Dynamics 365 Business Edition
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Lär dig hur du migrerar kvalificerade Dynamics 365 Business Edition-erbjudanden till nyare versioner innan de går ut.
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: e83c06c11638bdde508fd27904038bcb6d8c9e9c
ms.sourcegitcommit: f24089cd27b1de6ecf6ddbefb6cbb2d340e144de
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/01/2021
ms.locfileid: "106132646"
---
# <a name="migrate-dynamics-365-business-edition-offers-to-newer-versions"></a><span data-ttu-id="b84a7-103">Migrera Dynamics 365 Business Edition-erbjudanden till nyare versioner</span><span class="sxs-lookup"><span data-stu-id="b84a7-103">Migrate Dynamics 365 Business Edition Offers to newer versions</span></span>

<span data-ttu-id="b84a7-104">**Lämpliga roller**</span><span class="sxs-lookup"><span data-stu-id="b84a7-104">**Appropriate roles**</span></span>

- <span data-ttu-id="b84a7-105">Global administratör</span><span class="sxs-lookup"><span data-stu-id="b84a7-105">Global admin</span></span>
- <span data-ttu-id="b84a7-106">Administratör för användar hantering</span><span class="sxs-lookup"><span data-stu-id="b84a7-106">User management admin</span></span>
- <span data-ttu-id="b84a7-107">Administratörs agent</span><span class="sxs-lookup"><span data-stu-id="b84a7-107">Admin agent</span></span>
- <span data-ttu-id="b84a7-108">Försäljnings agent</span><span class="sxs-lookup"><span data-stu-id="b84a7-108">Sales agent</span></span>

<span data-ttu-id="b84a7-109">Från och med 1 januari 2019 kan kunder med Dynamics 365 Business Edition-prenumerationer inte längre förnyas till de här äldre erbjudandena. befintliga prenumerationer förnyas inte automatiskt när de upphör att gälla.</span><span class="sxs-lookup"><span data-stu-id="b84a7-109">Effective January 1, 2019, customers with Dynamics 365 Business Edition subscriptions can no longer renew into these legacy offers; existing subscriptions will not renew automatically when they expire.</span></span> <span data-ttu-id="b84a7-110">På prenumerationens informations sida ändras prenumerations statusen till "upphör att gälla [datum]" från "Auto Regener på [Date]".</span><span class="sxs-lookup"><span data-stu-id="b84a7-110">On the subscription's detail page, the subscription status will change to "Expires on [date]" from "Auto renews on [date]".</span></span>

<span data-ttu-id="b84a7-111">För att säkerställa kontinuitet för kunderna bör du gå över de med förfallna prenumerationer på ett alternativ som stöds.</span><span class="sxs-lookup"><span data-stu-id="b84a7-111">To ensure continuity for customers, you should transition those with expiring subscriptions to a supported option, listed below.</span></span> <span data-ttu-id="b84a7-112">Vi rekommenderar att du flyttar kunder till nya prenumerationer före prenumerationens årliga slutdatum för att undvika eventuella avbrott i tjänsten för kunderna.</span><span class="sxs-lookup"><span data-stu-id="b84a7-112">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span>

<span data-ttu-id="b84a7-113">Om du använder API: et (topp-eller partner Center) kan du hitta förfallna prenumerationer genom att utvärdera slutdatumet för prenumerationen tillsammans med egenskapen Auto renew = false.</span><span class="sxs-lookup"><span data-stu-id="b84a7-113">If you use the API (either CREST or Partner Center), you can find expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.</span></span> <span data-ttu-id="b84a7-114">Prenumerationerna i fråga kommer att ställas in på automatisk förnyelse = falskt den 1 januari 2019.</span><span class="sxs-lookup"><span data-stu-id="b84a7-114">The subscriptions in question will be set to auto renew=False on January 1, 2019.</span></span> <span data-ttu-id="b84a7-115">Du kan när som helst flytta kunder till en ny plan.</span><span class="sxs-lookup"><span data-stu-id="b84a7-115">You can move customers to a new plan at any time.</span></span> 

## <a name="the-dynamics-365-business-editions-being-retired"></a><span data-ttu-id="b84a7-116">Dynamics 365 Business-versionerna dras tillbaka</span><span class="sxs-lookup"><span data-stu-id="b84a7-116">The Dynamics 365 Business Editions being retired</span></span>

- <span data-ttu-id="b84a7-117">Dynamics 365 för finanser och drift, Business Edition</span><span class="sxs-lookup"><span data-stu-id="b84a7-117">Dynamics 365 for Finance and Operations, Business edition</span></span>
- <span data-ttu-id="b84a7-118">Dynamics 365 for Team Members, Business Edition</span><span class="sxs-lookup"><span data-stu-id="b84a7-118">Dynamics 365 for Team Members, Business edition</span></span>

## <a name="dynamics-business-central---the-dynamics-365-business-edition-new-offers"></a><span data-ttu-id="b84a7-119">Dynamics Business Central – Dynamics 365 Business Edition nya erbjudanden</span><span class="sxs-lookup"><span data-stu-id="b84a7-119">Dynamics Business Central - the Dynamics 365 Business Edition new offers</span></span>

<span data-ttu-id="b84a7-120">Med de nya Dynamics Business Central-erbjudandena kan dina kunder ansluta sina finanser, försäljning, tjänster och åtgärder för att effektivisera affärs processerna, förbättra kund interaktioner och fatta bättre beslut.</span><span class="sxs-lookup"><span data-stu-id="b84a7-120">With the new Dynamics Business Central offers, your customers can connect their financials, sales, service, and operations to streamline business processes, improve customer interactions, and make better decisions.</span></span> <span data-ttu-id="b84a7-121">Dynamics 365 Business Central är endast molnbaserad och tillgängligt via program partner för Cloud Solution Provider (CSP).</span><span class="sxs-lookup"><span data-stu-id="b84a7-121">Dynamics 365 Business Central is cloud-based and available through Cloud Solution Provider (CSP) program partners only.</span></span>
<span data-ttu-id="b84a7-122">Dynamics 365 Business Edition-kunder är berättigade till rabatterad över gångs prissättning för de nya företags Central erbjudandena fram till den 30 juni 2020.</span><span class="sxs-lookup"><span data-stu-id="b84a7-122">Dynamics 365 Business Edition customers are eligible to receive discounted transition pricing for the new Business Central offers until June 30, 2020.</span></span>

## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="b84a7-123">Överföra kunder till nya produkt planer</span><span class="sxs-lookup"><span data-stu-id="b84a7-123">Transition customers to new product plans</span></span>

 <span data-ttu-id="b84a7-124">Att flytta kunder från tillbakadragna SKU: er till nyare kräver följande steg i den här ordningen:</span><span class="sxs-lookup"><span data-stu-id="b84a7-124">Moving customers from retired SKUs to newer ones requires the following steps in this order:</span></span>

- <span data-ttu-id="b84a7-125">Köp den nya prenumerationen</span><span class="sxs-lookup"><span data-stu-id="b84a7-125">Purchase the new subscription</span></span>
- <span data-ttu-id="b84a7-126">Tilldela om aktuella användar licenser</span><span class="sxs-lookup"><span data-stu-id="b84a7-126">Reassign current user licenses</span></span>
- <span data-ttu-id="b84a7-127">Avbryt gammal prenumeration</span><span class="sxs-lookup"><span data-stu-id="b84a7-127">Cancel old subscription</span></span>

## <a name="purchase-the-new-plan-for-your-customer"></a><span data-ttu-id="b84a7-128">Köp det nya avtalet för kunden</span><span class="sxs-lookup"><span data-stu-id="b84a7-128">Purchase the new plan for your customer</span></span>

1. <span data-ttu-id="b84a7-129">Välj **kunder** i det vänstra navigerings fältet och välj sedan den kund som du vill flytta till den nya prenumerationen.</span><span class="sxs-lookup"><span data-stu-id="b84a7-129">Select **Customers** from the left nav and then select the customer you want to move to the new subscription.</span></span>
2. <span data-ttu-id="b84a7-130">Välj **Lägg till prenumeration**.</span><span class="sxs-lookup"><span data-stu-id="b84a7-130">Select **Add Subscription**.</span></span>
3. <span data-ttu-id="b84a7-131">Välj den prenumeration som du vill köpa från katalogen (i det här fallet ett av alternativen ovan), ange antalet licenser och välj sedan **Skicka**.</span><span class="sxs-lookup"><span data-stu-id="b84a7-131">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span> 

<span data-ttu-id="b84a7-132">Din kund kommer nu att ha både den gamla och den nya prenumerationen.</span><span class="sxs-lookup"><span data-stu-id="b84a7-132">Your customer will now have both the old subscription and the new one.</span></span> <span data-ttu-id="b84a7-133">Nästa steg är att omtilldela licenser till kundens användare.</span><span class="sxs-lookup"><span data-stu-id="b84a7-133">Your next step is to reassign licenses to the customer's users.</span></span>

1. <span data-ttu-id="b84a7-134">Välj **kunder** i det vänstra navigerings fältet och välj sedan den kund som du flyttar.</span><span class="sxs-lookup"><span data-stu-id="b84a7-134">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="b84a7-135">Välj **användare och licenser**.</span><span class="sxs-lookup"><span data-stu-id="b84a7-135">Select **Users and licenses**.</span></span>
3. <span data-ttu-id="b84a7-136">Om du vill tilldela en licens till en användare igen väljer du användaren och väljer sedan **Hantera licenser**.</span><span class="sxs-lookup"><span data-stu-id="b84a7-136">To reassign a license to a user, select the user and then select **Manage licenses**.</span></span> 
4. <span data-ttu-id="b84a7-137">På sidan **Hantera licenser** avmarkerar du kryss rutan Dynamics 365 för sälj-/kund engagemang från Basic-licens (kvalificerad erbjudande) och väljer en ny service plan för den prenumeration som kunden flyttar till.</span><span class="sxs-lookup"><span data-stu-id="b84a7-137">On the **Manage licenses** page, clear the Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offer) license check box and select a new service plan for the subscription the customer is moving to.</span></span> 
5. <span data-ttu-id="b84a7-138">Välj **Skicka**.</span><span class="sxs-lookup"><span data-stu-id="b84a7-138">Select **Submit**.</span></span> <span data-ttu-id="b84a7-139">Du kommer att göra detta för varje användare som behöver den nya licensen.</span><span class="sxs-lookup"><span data-stu-id="b84a7-139">You will do this for each user who needs the new license.</span></span> 

<span data-ttu-id="b84a7-140">När du har flyttat licenserna till den nya prenumerationen kan du avbryta den gamla prenumerationen.</span><span class="sxs-lookup"><span data-stu-id="b84a7-140">Once you've moved the licenses over to the new subscription, you can cancel the old subscription.</span></span> 

1. <span data-ttu-id="b84a7-141">Välj **kunder** i det vänstra navigerings fältet och välj sedan den kund som du flyttar.</span><span class="sxs-lookup"><span data-stu-id="b84a7-141">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="b84a7-142">På sidan prenumerations information anger du att den gamla prenumerationen har **pausats** och väljer **Skicka**.</span><span class="sxs-lookup"><span data-stu-id="b84a7-142">On the subscription detail page, set the old subscription to **Suspended** and select **Submit**.</span></span>

<span data-ttu-id="b84a7-143">Den gamla prenumerationen är nu inaktive rad och den nya prenumerationen är aktiv.</span><span class="sxs-lookup"><span data-stu-id="b84a7-143">The old subscription is now suspended, and the new subscription is active.</span></span> <span data-ttu-id="b84a7-144">Den inaktiverade prenumerationen kommer att avetableras automatiskt efter 120 dagar.</span><span class="sxs-lookup"><span data-stu-id="b84a7-144">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="b84a7-145">Kunden debiteras inga ytterligare kostnader för den gamla prenumerationen.</span><span class="sxs-lookup"><span data-stu-id="b84a7-145">Your customer will incur no additional costs for the old subscription.</span></span>
