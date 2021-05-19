---
title: Migrera Dynamics 365 Business Edition
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Lär dig hur du migrerar kvalificerade Dynamics 365 Business Edition-erbjudanden till nyare versioner innan de upphör att gälla.
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 8232ab165ea68ebefdfbb30f3ac52c907e1b7278
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 05/19/2021
ms.locfileid: "110151533"
---
# <a name="migrate-dynamics-365-business-edition-offers-to-newer-versions"></a><span data-ttu-id="8b8df-103">Migrera Dynamics 365 Business Edition-erbjudanden till nyare versioner</span><span class="sxs-lookup"><span data-stu-id="8b8df-103">Migrate Dynamics 365 Business Edition Offers to newer versions</span></span>

<span data-ttu-id="8b8df-104">**Lämpliga roller:** Globala | Administratörsbehörighet för | Administratörsagent | Försäljningsagent</span><span class="sxs-lookup"><span data-stu-id="8b8df-104">**Appropriate roles**: Global admin | User management admin | Admin agent | Sales agent</span></span>

<span data-ttu-id="8b8df-105">Från och med 1 januari 2019 kan kunder med Dynamics 365 Business Edition-prenumerationer inte längre förnya till dessa äldre erbjudanden. befintliga prenumerationer förnyas inte automatiskt när de upphör att gälla.</span><span class="sxs-lookup"><span data-stu-id="8b8df-105">Effective January 1, 2019, customers with Dynamics 365 Business Edition subscriptions can no longer renew into these legacy offers; existing subscriptions will not renew automatically when they expire.</span></span> <span data-ttu-id="8b8df-106">På prenumerationens informationssida ändras prenumerationsstatusen till "Upphör [datum]" från "Förnyas automatiskt [datum]".</span><span class="sxs-lookup"><span data-stu-id="8b8df-106">On the subscription's detail page, the subscription status will change to "Expires on [date]" from "Auto renews on [date]".</span></span>

<span data-ttu-id="8b8df-107">För att säkerställa kontinuitet för kunder bör du föra över dem med utgående prenumerationer till ett alternativ som stöds, som anges nedan.</span><span class="sxs-lookup"><span data-stu-id="8b8df-107">To ensure continuity for customers, you should transition those with expiring subscriptions to a supported option, listed below.</span></span> <span data-ttu-id="8b8df-108">Vi rekommenderar att du flyttar kunder till nya prenumerationer före prenumerationens årliga slutdatum för att undvika eventuella tjänstavbrott för kunder.</span><span class="sxs-lookup"><span data-stu-id="8b8df-108">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span>

<span data-ttu-id="8b8df-109">Om du använder API:et (antingen ELLER Partnercenter) kan du hitta utgångna prenumerationer genom att utvärdera slutdatumet för prenumerationen tillsammans med egenskapen förnya automatiskt = Falskt.</span><span class="sxs-lookup"><span data-stu-id="8b8df-109">If you use the API (either CREST or Partner Center), you can find expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.</span></span> <span data-ttu-id="8b8df-110">Prenumerationerna i fråga ställs in på förnya automatiskt = Falskt den 1 januari 2019.</span><span class="sxs-lookup"><span data-stu-id="8b8df-110">The subscriptions in question will be set to auto renew=False on January 1, 2019.</span></span> <span data-ttu-id="8b8df-111">Du kan när som helst flytta kunder till en ny plan.</span><span class="sxs-lookup"><span data-stu-id="8b8df-111">You can move customers to a new plan at any time.</span></span> 

## <a name="the-dynamics-365-business-editions-being-retired"></a><span data-ttu-id="8b8df-112">Dynamics 365 Business Editions dras tillbaka</span><span class="sxs-lookup"><span data-stu-id="8b8df-112">The Dynamics 365 Business Editions being retired</span></span>

- <span data-ttu-id="8b8df-113">Dynamics 365 for Finance and Operations, Business Edition</span><span class="sxs-lookup"><span data-stu-id="8b8df-113">Dynamics 365 for Finance and Operations, Business edition</span></span>
- <span data-ttu-id="8b8df-114">Dynamics 365 for Team Members, Business Edition</span><span class="sxs-lookup"><span data-stu-id="8b8df-114">Dynamics 365 for Team Members, Business edition</span></span>

## <a name="dynamics-business-central---the-dynamics-365-business-edition-new-offers"></a><span data-ttu-id="8b8df-115">Dynamics Business Central – nya erbjudanden för Dynamics 365 Business Edition</span><span class="sxs-lookup"><span data-stu-id="8b8df-115">Dynamics Business Central - the Dynamics 365 Business Edition new offers</span></span>

<span data-ttu-id="8b8df-116">Med de nya Dynamics Business Central-erbjudandena kan dina kunder ansluta sina ekonomi-, försäljnings-, tjänst- och drifttjänster för att effektivisera affärsprocesser, förbättra kundinteraktioner och fatta bättre beslut.</span><span class="sxs-lookup"><span data-stu-id="8b8df-116">With the new Dynamics Business Central offers, your customers can connect their financials, sales, service, and operations to streamline business processes, improve customer interactions, and make better decisions.</span></span> <span data-ttu-id="8b8df-117">Dynamics 365 Business Central är molnbaserad och tillgänglig endast via Molnlösningsleverantör(CSP) programpartner.</span><span class="sxs-lookup"><span data-stu-id="8b8df-117">Dynamics 365 Business Central is cloud-based and available through Cloud Solution Provider (CSP) program partners only.</span></span>
<span data-ttu-id="8b8df-118">Dynamics 365 Business Edition-kunder är berättigade till rabatterade övergångspriser för de nya Business Central-erbjudandena fram till den 30 juni 2020.</span><span class="sxs-lookup"><span data-stu-id="8b8df-118">Dynamics 365 Business Edition customers are eligible to receive discounted transition pricing for the new Business Central offers until June 30, 2020.</span></span>

## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="8b8df-119">Övergå kunder till nya produktplaner</span><span class="sxs-lookup"><span data-stu-id="8b8df-119">Transition customers to new product plans</span></span>

 <span data-ttu-id="8b8df-120">Att flytta kunder från tillbakadragna SKU:er till nyare kräver följande steg i den här ordningen:</span><span class="sxs-lookup"><span data-stu-id="8b8df-120">Moving customers from retired SKUs to newer ones requires the following steps in this order:</span></span>

- <span data-ttu-id="8b8df-121">Köpa den nya prenumerationen</span><span class="sxs-lookup"><span data-stu-id="8b8df-121">Purchase the new subscription</span></span>
- <span data-ttu-id="8b8df-122">Tilldela om aktuella användarlicenser</span><span class="sxs-lookup"><span data-stu-id="8b8df-122">Reassign current user licenses</span></span>
- <span data-ttu-id="8b8df-123">Avbryta gammal prenumeration</span><span class="sxs-lookup"><span data-stu-id="8b8df-123">Cancel old subscription</span></span>

## <a name="purchase-the-new-plan-for-your-customer"></a><span data-ttu-id="8b8df-124">Köp den nya planen för din kund</span><span class="sxs-lookup"><span data-stu-id="8b8df-124">Purchase the new plan for your customer</span></span>

1. <span data-ttu-id="8b8df-125">Välj **Kunder** i det vänstra navigeringsfältet och välj sedan den kund som du vill flytta till den nya prenumerationen.</span><span class="sxs-lookup"><span data-stu-id="8b8df-125">Select **Customers** from the left nav and then select the customer you want to move to the new subscription.</span></span>
2. <span data-ttu-id="8b8df-126">Välj **Lägg till prenumeration.**</span><span class="sxs-lookup"><span data-stu-id="8b8df-126">Select **Add Subscription**.</span></span>
3. <span data-ttu-id="8b8df-127">Välj den prenumeration som du vill köpa från katalogen (i det här fallet något av alternativen ovan), ange antalet licenser och välj sedan **Skicka.**</span><span class="sxs-lookup"><span data-stu-id="8b8df-127">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span> 

<span data-ttu-id="8b8df-128">Kunden kommer nu att ha både den gamla och den nya.</span><span class="sxs-lookup"><span data-stu-id="8b8df-128">Your customer will now have both the old subscription and the new one.</span></span> <span data-ttu-id="8b8df-129">Nästa steg är att omtilldela licenser till kundens användare.</span><span class="sxs-lookup"><span data-stu-id="8b8df-129">Your next step is to reassign licenses to the customer's users.</span></span>

1. <span data-ttu-id="8b8df-130">Välj **Kunder** i det vänstra navigeringsfältet och välj sedan den kund som du flyttar.</span><span class="sxs-lookup"><span data-stu-id="8b8df-130">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="8b8df-131">Välj **Användare och licenser.**</span><span class="sxs-lookup"><span data-stu-id="8b8df-131">Select **Users and licenses**.</span></span>
3. <span data-ttu-id="8b8df-132">Om du vill tilldela om en licens till en användare väljer du användaren och sedan **Hantera licenser.**</span><span class="sxs-lookup"><span data-stu-id="8b8df-132">To reassign a license to a user, select the user and then select **Manage licenses**.</span></span> 
4. <span data-ttu-id="8b8df-133">På sidan **Hantera licenser** avmarkerar du kryssrutan Dynamics 365 for Sales/Customer Engagement Plan från Basic-licens (kvalificerat erbjudande) och väljer en ny tjänstplan för prenumerationen som kunden flyttar till.</span><span class="sxs-lookup"><span data-stu-id="8b8df-133">On the **Manage licenses** page, clear the Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offer) license check box and select a new service plan for the subscription the customer is moving to.</span></span> 
5. <span data-ttu-id="8b8df-134">Välj **Skicka**.</span><span class="sxs-lookup"><span data-stu-id="8b8df-134">Select **Submit**.</span></span> <span data-ttu-id="8b8df-135">Du gör detta för varje användare som behöver den nya licensen.</span><span class="sxs-lookup"><span data-stu-id="8b8df-135">You will do this for each user who needs the new license.</span></span> 

<span data-ttu-id="8b8df-136">När du har flyttat över licenserna till den nya prenumerationen kan du avbryta den gamla prenumerationen.</span><span class="sxs-lookup"><span data-stu-id="8b8df-136">Once you've moved the licenses over to the new subscription, you can cancel the old subscription.</span></span> 

1. <span data-ttu-id="8b8df-137">Välj **Kunder** i det vänstra navigeringsfältet och välj sedan den kund som du flyttar.</span><span class="sxs-lookup"><span data-stu-id="8b8df-137">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="8b8df-138">På sidan med prenumerationsdetaljer ställer du in den gamla prenumerationen på **Pausad** och väljer **Skicka**.</span><span class="sxs-lookup"><span data-stu-id="8b8df-138">On the subscription detail page, set the old subscription to **Suspended** and select **Submit**.</span></span>

<span data-ttu-id="8b8df-139">Den gamla prenumerationen har nu inaktiverats och den nya prenumerationen är aktiv.</span><span class="sxs-lookup"><span data-stu-id="8b8df-139">The old subscription is now suspended, and the new subscription is active.</span></span> <span data-ttu-id="8b8df-140">Den pausade prenumerationen avetableeras automatiskt efter 120 dagar.</span><span class="sxs-lookup"><span data-stu-id="8b8df-140">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="8b8df-141">Kunden medför inga ytterligare kostnader för den gamla prenumerationen.</span><span class="sxs-lookup"><span data-stu-id="8b8df-141">Your customer will incur no additional costs for the old subscription.</span></span>
