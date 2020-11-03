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
ms.openlocfilehash: d441d121c28c2762d1f1c71d6f6a1e81d089f99c
ms.sourcegitcommit: 7153f0b8c67efd35f58695ca2a7e00e70da1c5e9
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 07/17/2020
ms.locfileid: "92531005"
---
# <a name="migrate-dynamics-365-business-edition-offers-to-newer-versions"></a><span data-ttu-id="40c80-103">Migrera Dynamics 365 Business Edition-erbjudanden till nyare versioner</span><span class="sxs-lookup"><span data-stu-id="40c80-103">Migrate Dynamics 365 Business Edition Offers to newer versions</span></span>

<span data-ttu-id="40c80-104">**Gäller för**</span><span class="sxs-lookup"><span data-stu-id="40c80-104">**Applies to**</span></span>

- <span data-ttu-id="40c80-105">Partnercenter</span><span class="sxs-lookup"><span data-stu-id="40c80-105">Partner Center</span></span>

<span data-ttu-id="40c80-106">**Lämpliga roller**</span><span class="sxs-lookup"><span data-stu-id="40c80-106">**Appropriate roles**</span></span>
- <span data-ttu-id="40c80-107">Global administratör</span><span class="sxs-lookup"><span data-stu-id="40c80-107">Global admin</span></span>
- <span data-ttu-id="40c80-108">Användaradministratör</span><span class="sxs-lookup"><span data-stu-id="40c80-108">User admin</span></span>
- <span data-ttu-id="40c80-109">Administratörs agent</span><span class="sxs-lookup"><span data-stu-id="40c80-109">Admin agent</span></span>
- <span data-ttu-id="40c80-110">Försäljnings agent</span><span class="sxs-lookup"><span data-stu-id="40c80-110">Sales agent</span></span>

<span data-ttu-id="40c80-111">Från och med 1 januari 2019 kan kunder med Dynamics 365 Business Edition-prenumerationer inte längre förnyas till de här äldre erbjudandena. befintliga prenumerationer förnyas inte automatiskt när de upphör att gälla.</span><span class="sxs-lookup"><span data-stu-id="40c80-111">Effective January 1, 2019, customers with Dynamics 365 Business Edition subscriptions can no longer renew into these legacy offers; existing subscriptions will not renew automatically when they expire.</span></span> <span data-ttu-id="40c80-112">På prenumerationens informations sida ändras prenumerations statusen till "upphör att gälla [datum]" från "Auto Regener på [Date]".</span><span class="sxs-lookup"><span data-stu-id="40c80-112">On the subscription's detail page, the subscription status will change to "Expires on [date]" from "Auto renews on [date]".</span></span>

<span data-ttu-id="40c80-113">För att säkerställa kontinuitet för kunderna bör du gå över de med förfallna prenumerationer på ett alternativ som stöds.</span><span class="sxs-lookup"><span data-stu-id="40c80-113">To ensure continuity for customers, you should transition those with expiring subscriptions to a supported option, listed below.</span></span> <span data-ttu-id="40c80-114">Vi rekommenderar att du flyttar kunder till nya prenumerationer före prenumerationens årliga slutdatum för att undvika eventuella avbrott i tjänsten för kunderna.</span><span class="sxs-lookup"><span data-stu-id="40c80-114">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span>

<span data-ttu-id="40c80-115">Om du använder API: et (topp-eller partner Center) kan du hitta förfallna prenumerationer genom att utvärdera slutdatumet för prenumerationen tillsammans med egenskapen Auto renew = false.</span><span class="sxs-lookup"><span data-stu-id="40c80-115">If you use the API (either CREST or Partner Center), you can find expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.</span></span> <span data-ttu-id="40c80-116">Prenumerationerna i fråga kommer att ställas in på automatisk förnyelse = falskt den 1 januari 2019.</span><span class="sxs-lookup"><span data-stu-id="40c80-116">The subscriptions in question will be set to auto renew=False on Jan 1, 2019.</span></span> <span data-ttu-id="40c80-117">Du kan när som helst flytta kunder till en ny plan.</span><span class="sxs-lookup"><span data-stu-id="40c80-117">You can move customers to a new plan at any time.</span></span> 

## <a name="the-dynamics-365-business-editions-being-retired"></a><span data-ttu-id="40c80-118">Dynamics 365 Business-versionerna dras tillbaka</span><span class="sxs-lookup"><span data-stu-id="40c80-118">The Dynamics 365 Business Editions being retired</span></span>

- <span data-ttu-id="40c80-119">Dynamics 365 för finanser och drift, Business Edition</span><span class="sxs-lookup"><span data-stu-id="40c80-119">Dynamics 365 for Finance and Operations, Business edition</span></span>
- <span data-ttu-id="40c80-120">Dynamics 365 for Team Members, Business Edition</span><span class="sxs-lookup"><span data-stu-id="40c80-120">Dynamics 365 for Team Members, Business edition</span></span>

## <a name="dynamics-business-central---the-dynamics-365-business-edition-new-offers"></a><span data-ttu-id="40c80-121">Dynamics Business Central – Dynamics 365 Business Edition nya erbjudanden</span><span class="sxs-lookup"><span data-stu-id="40c80-121">Dynamics Business Central - the Dynamics 365 Business Edition new offers</span></span>

<span data-ttu-id="40c80-122">Med de nya Dynamics Business Central-erbjudandena kan dina kunder ansluta sina finanser, försäljning, tjänster och åtgärder för att effektivisera affärs processerna, förbättra kund interaktioner och fatta bättre beslut.</span><span class="sxs-lookup"><span data-stu-id="40c80-122">With the new Dynamics Business Central offers, your customers can connect their financials, sales, service, and operations to streamline business processes, improve customer interactions, and make better decisions.</span></span> <span data-ttu-id="40c80-123">Dynamics 365 Business Central är endast molnbaserad och tillgängligt via program partner för Cloud Solution Provider (CSP).</span><span class="sxs-lookup"><span data-stu-id="40c80-123">Dynamics 365 Business Central is cloud-based and available through Cloud Solution Provider (CSP) program partners only.</span></span>
<span data-ttu-id="40c80-124">Dynamics 365 Business Edition-kunder är berättigade till rabatterad över gångs prissättning för de nya företags Central erbjudandena fram till den 30 juni 2020.</span><span class="sxs-lookup"><span data-stu-id="40c80-124">Dynamics 365 Business Edition customers are eligible to receive discounted transition pricing for the new Business Central offers until June 30, 2020.</span></span>

## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="40c80-125">Överföra kunder till nya produkt planer</span><span class="sxs-lookup"><span data-stu-id="40c80-125">Transition customers to new product plans</span></span>

 <span data-ttu-id="40c80-126">Att flytta kunder från tillbakadragna SKU: er till nyare kräver följande steg i den här ordningen:</span><span class="sxs-lookup"><span data-stu-id="40c80-126">Moving customers from retired SKUs to newer ones requires the following steps in this order:</span></span>

- <span data-ttu-id="40c80-127">Köp den nya prenumerationen</span><span class="sxs-lookup"><span data-stu-id="40c80-127">Purchase the new subscription</span></span>
- <span data-ttu-id="40c80-128">Tilldela om aktuella användar licenser</span><span class="sxs-lookup"><span data-stu-id="40c80-128">Reassign current user licenses</span></span>
- <span data-ttu-id="40c80-129">Avbryt gammal prenumeration</span><span class="sxs-lookup"><span data-stu-id="40c80-129">Cancel old subscription</span></span>

## <a name="purchase-the-new-plan-for-your-customer"></a><span data-ttu-id="40c80-130">Köp det nya avtalet för kunden</span><span class="sxs-lookup"><span data-stu-id="40c80-130">Purchase the new plan for your customer</span></span>

1. <span data-ttu-id="40c80-131">Välj **kunder** i det vänstra navigerings fältet och välj sedan den kund som du vill flytta till den nya prenumerationen.</span><span class="sxs-lookup"><span data-stu-id="40c80-131">Select **Customers** from the left nav and then select the customer you want to move to the new subscription.</span></span>
2. <span data-ttu-id="40c80-132">Välj **Lägg till prenumeration** .</span><span class="sxs-lookup"><span data-stu-id="40c80-132">Select **Add Subscription** .</span></span>
3. <span data-ttu-id="40c80-133">Välj den prenumeration som du vill köpa från katalogen (i det här fallet ett av alternativen ovan), ange antalet licenser och välj sedan **Skicka** .</span><span class="sxs-lookup"><span data-stu-id="40c80-133">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit** .</span></span> 

<span data-ttu-id="40c80-134">Din kund kommer nu att ha både den gamla och den nya prenumerationen.</span><span class="sxs-lookup"><span data-stu-id="40c80-134">Your customer will now have both the old subscription and the new one.</span></span> <span data-ttu-id="40c80-135">Nästa steg är att omtilldela licenser till kundens användare.</span><span class="sxs-lookup"><span data-stu-id="40c80-135">Your next step is to reassign licenses to the customer's users.</span></span>

1. <span data-ttu-id="40c80-136">Välj **kunder** i det vänstra navigerings fältet och välj sedan den kund som du flyttar.</span><span class="sxs-lookup"><span data-stu-id="40c80-136">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="40c80-137">Välj **användare och licenser** .</span><span class="sxs-lookup"><span data-stu-id="40c80-137">Select **Users and licenses** .</span></span>
3. <span data-ttu-id="40c80-138">Om du vill tilldela en licens till en användare igen väljer du användaren och väljer sedan **Hantera licenser** .</span><span class="sxs-lookup"><span data-stu-id="40c80-138">To reassign a license to a user, select the user and then select **Manage licenses** .</span></span> 
4. <span data-ttu-id="40c80-139">På sidan **Hantera licenser** avmarkerar du kryss rutan Dynamics 365 för sälj-/kund engagemang från Basic-licens (kvalificerad erbjudande) och väljer en ny service plan för den prenumeration som kunden flyttar till.</span><span class="sxs-lookup"><span data-stu-id="40c80-139">On the **Manage licenses** page, clear the Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offer) license check box and select a new service plan for the subscription the customer is moving to.</span></span> 
5. <span data-ttu-id="40c80-140">Välj **Skicka** .</span><span class="sxs-lookup"><span data-stu-id="40c80-140">Select **Submit** .</span></span> <span data-ttu-id="40c80-141">Du kommer att göra detta för varje användare som behöver den nya licensen.</span><span class="sxs-lookup"><span data-stu-id="40c80-141">You will do this for each user who needs the new license.</span></span> 

<span data-ttu-id="40c80-142">När du har flyttat licenserna till den nya prenumerationen kan du avbryta den gamla prenumerationen.</span><span class="sxs-lookup"><span data-stu-id="40c80-142">Once you've moved the licenses over to the new subscription you can cancel the old subscription.</span></span> 

1. <span data-ttu-id="40c80-143">Välj **kunder** i det vänstra navigerings fältet och välj sedan den kund som du flyttar.</span><span class="sxs-lookup"><span data-stu-id="40c80-143">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="40c80-144">På sidan prenumerations information anger du att den gamla prenumerationen har **pausats** och väljer **Skicka** .</span><span class="sxs-lookup"><span data-stu-id="40c80-144">On the subscription detail page, set the old subscription to **Suspended** and select **Submit** .</span></span>

<span data-ttu-id="40c80-145">Den gamla prenumerationen är nu inaktive rad och den nya prenumerationen är aktiv.</span><span class="sxs-lookup"><span data-stu-id="40c80-145">The old subscription is now suspended, and the new subscription is active.</span></span> <span data-ttu-id="40c80-146">Den inaktiverade prenumerationen kommer att avetableras automatiskt efter 120 dagar.</span><span class="sxs-lookup"><span data-stu-id="40c80-146">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="40c80-147">Kunden debiteras inga ytterligare kostnader för den gamla prenumerationen.</span><span class="sxs-lookup"><span data-stu-id="40c80-147">Your customer will incur no additional costs for the old subscription.</span></span>
