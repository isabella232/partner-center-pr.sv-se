---
title: Migrera kvalificerade Dynamics 365-prenumerationer
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Lär dig hur du migrerar från kvalificerade, grundläggande Dynamics 365-prenumerationer till en ny prenumeration innan befintliga prenumerationer upphör att gälla.
author: Brentserbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 5ba6992eff64031aed0dafeb5a5010983396ab63
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 05/19/2021
ms.locfileid: "110151652"
---
# <a name="migrate-dynamics-365-and-customer-engagement-plan-from-basic-qualified-offers-to-newer-versions"></a><span data-ttu-id="03525-103">Migrera Dynamics 365 och en plan för kundengagemang från Basic (kvalificerade erbjudanden) till nyare versioner</span><span class="sxs-lookup"><span data-stu-id="03525-103">Migrate Dynamics 365 and Customer Engagement Plan from Basic (qualified offers) to newer versions</span></span>

<span data-ttu-id="03525-104">**Lämpliga roller:** Global | Administratörsbehörighet för användarhantering | Administratörsagent | Försäljningsagent</span><span class="sxs-lookup"><span data-stu-id="03525-104">**Appropriate roles**: Global admin | User management admin | Admin agent | Sales agent</span></span>

<span data-ttu-id="03525-105">Från och med den 1 januari 2019 kan kunder med Prenumerationer på Dynamics 365 for Sales/Customer Engagement från Basic-prenumerationer (kvalificerade erbjudanden) inte längre förnya dessa äldre erbjudanden. befintliga prenumerationer förnyas inte automatiskt när de upphör att gälla.</span><span class="sxs-lookup"><span data-stu-id="03525-105">Effective January 1, 2019, customers with Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offers) subscriptions can no longer renew these legacy offers; existing subscriptions will not renew automatically when they expire.</span></span> <span data-ttu-id="03525-106">På prenumerationens informationssida ändras prenumerationsstatusen till "Upphör att gälla [datum]" från "Förnyas automatiskt [datum]".</span><span class="sxs-lookup"><span data-stu-id="03525-106">On the subscription's detail page, the subscription status will change to "Expires on [date]" from "Auto renews on [date]".</span></span> 

<span data-ttu-id="03525-107">För att säkerställa kontinuitet för kunder bör du föra över dem med utgående prenumerationer till ett alternativ som stöds, som anges nedan.</span><span class="sxs-lookup"><span data-stu-id="03525-107">To ensure continuity for customers, you should transition those with expiring subscriptions to a supported option, listed below.</span></span> <span data-ttu-id="03525-108">Vi rekommenderar att du flyttar kunder till nya prenumerationer före prenumerationens årliga slutdatum för att undvika eventuella tjänstavbrott för kunder.</span><span class="sxs-lookup"><span data-stu-id="03525-108">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span>

<span data-ttu-id="03525-109">Om du använder API:et (antingen KANT eller Partnercenter) kan du hitta prenumerationer som går ut genom att utvärdera slutdatumet för prenumerationen tillsammans med egenskapen för automatisk förnyelse = Falskt.</span><span class="sxs-lookup"><span data-stu-id="03525-109">If you use the API (either CREST or Partner Center), you can find expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.</span></span> <span data-ttu-id="03525-110">Prenumerationerna i fråga ställs in på förnya automatiskt = Falskt den 1 januari 2019.</span><span class="sxs-lookup"><span data-stu-id="03525-110">The subscriptions in question will be set to auto renew=False on January 1, 2019.</span></span> <span data-ttu-id="03525-111">Du kan när som helst flytta kunder till en ny plan.</span><span class="sxs-lookup"><span data-stu-id="03525-111">You can move customers to a new plan at any time.</span></span> 

### <a name="the-dynamics-365-offers-being-retired"></a><span data-ttu-id="03525-112">Dynamics 365-erbjudanden som dras tillbaka</span><span class="sxs-lookup"><span data-stu-id="03525-112">The Dynamics 365 offers being retired</span></span>

- <span data-ttu-id="03525-113">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (kvalificerat erbjudande)</span><span class="sxs-lookup"><span data-stu-id="03525-113">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="03525-114">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (kvalificerat erbjudande) för lärare och lärare</span><span class="sxs-lookup"><span data-stu-id="03525-114">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="03525-115">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (kvalificerat erbjudande) för studenter</span><span class="sxs-lookup"><span data-stu-id="03525-115">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="03525-116">Dynamics 365 for Sales Enterprise Edition (Government Pricing) CRMOL Basic (kvalificerat erbjudande)</span><span class="sxs-lookup"><span data-stu-id="03525-116">Dynamics 365 for Sales Enterprise Edition (Government Pricing) CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="03525-117">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (kvalificerat erbjudande)</span><span class="sxs-lookup"><span data-stu-id="03525-117">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="03525-118">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (kvalificerat erbjudande) för lärare och lärare</span><span class="sxs-lookup"><span data-stu-id="03525-118">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="03525-119">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (kvalificerat erbjudande) för studenter</span><span class="sxs-lookup"><span data-stu-id="03525-119">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="03525-120">Dynamics 365 for Sales Enterprise Edition (Myndighetspriser) från SA för CRM Basic (kvalificerat erbjudande)</span><span class="sxs-lookup"><span data-stu-id="03525-120">Dynamics 365 for Sales Enterprise Edition (Government Pricing) From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="03525-121">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (kvalificerat erbjudande)</span><span class="sxs-lookup"><span data-stu-id="03525-121">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="03525-122">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (kvalificerat erbjudande) för lärare och lärare</span><span class="sxs-lookup"><span data-stu-id="03525-122">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="03525-123">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (kvalificerat erbjudande) för studenter</span><span class="sxs-lookup"><span data-stu-id="03525-123">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="03525-124">Dynamics 365 for Sales Enterprise Edition (Government Pricing) Add-On för CRM Basic (kvalificerat erbjudande)</span><span class="sxs-lookup"><span data-stu-id="03525-124">Dynamics 365 for Sales Enterprise Edition (Government Pricing) Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="03525-125">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (kvalificerat erbjudande)</span><span class="sxs-lookup"><span data-stu-id="03525-125">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="03525-126">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) CRMOL Basic (kvalificerat erbjudande)</span><span class="sxs-lookup"><span data-stu-id="03525-126">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="03525-127">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (kvalificerat erbjudande) för studenter</span><span class="sxs-lookup"><span data-stu-id="03525-127">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="03525-128">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (kvalificerat erbjudande) för lärare och lärare</span><span class="sxs-lookup"><span data-stu-id="03525-128">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="03525-129">Dynamics 365 Customer Engagement Plan Enterprise Edition från SA för CRM Basic (kvalificerat erbjudande)</span><span class="sxs-lookup"><span data-stu-id="03525-129">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="03525-130">Dynamics 365 Customer Engagement Plan Enterprise Edition (Myndighetspriser) från SA för CRM Basic (kvalificerat erbjudande)</span><span class="sxs-lookup"><span data-stu-id="03525-130">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="03525-131">Dynamics 365 Customer Engagement Plan Enterprise Edition från SA för CRM Basic (kvalificerat erbjudande) för studenter</span><span class="sxs-lookup"><span data-stu-id="03525-131">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="03525-132">Dynamics 365 Customer Engagement Plan Enterprise Edition from SA for CRM Basic (kvalificerat erbjudande) för lärare och lärare</span><span class="sxs-lookup"><span data-stu-id="03525-132">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="03525-133">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (kvalificerat erbjudande)</span><span class="sxs-lookup"><span data-stu-id="03525-133">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="03525-134">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) Add-On för CRM Basic (kvalificerat erbjudande)</span><span class="sxs-lookup"><span data-stu-id="03525-134">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="03525-135">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (kvalificerat erbjudande) för studenter</span><span class="sxs-lookup"><span data-stu-id="03525-135">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="03525-136">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (kvalificerat erbjudande) för lärare och lärare</span><span class="sxs-lookup"><span data-stu-id="03525-136">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Faculty</span></span>



## <a name="dynamics-365-for-sales-customer-engagement-plan-from-basic-qualified-offers-replacement-plans"></a><span data-ttu-id="03525-137">Dynamics 365 for Sales/Customer Engagement-plan från grundläggande (kvalificerade erbjudanden) ersättningsplaner</span><span class="sxs-lookup"><span data-stu-id="03525-137">Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offers) replacement plans</span></span>

<span data-ttu-id="03525-138">**Tillbakadragna erbjudanden**</span><span class="sxs-lookup"><span data-stu-id="03525-138">**Retired offers**</span></span>   

- <span data-ttu-id="03525-139">Dynamics 365 for Sales från CRM Basic eller CRMOL Basic (kvalificerat erbjudande)</span><span class="sxs-lookup"><span data-stu-id="03525-139">Dynamics 365 for Sales from CRM Basic or CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="03525-140">Dynamics 365 Customer Engagement-plan från CRM Basic eller CRMOL Basic (kvalificerat erbjudande)</span><span class="sxs-lookup"><span data-stu-id="03525-140">Dynamics 365 Customer Engagement Plan from CRM Basic or CRMOL Basic (Qualified Offer)</span></span>

<span data-ttu-id="03525-141">**Ersättningsalternativ**</span><span class="sxs-lookup"><span data-stu-id="03525-141">**Replacement options**</span></span>
- <span data-ttu-id="03525-142">Dynamics 365 for Sales Professional (NY)</span><span class="sxs-lookup"><span data-stu-id="03525-142">Dynamics 365 for Sales Professional (NEW)</span></span>
- <span data-ttu-id="03525-143">Dynamics 365 for Sales Professional (NY)</span><span class="sxs-lookup"><span data-stu-id="03525-143">Dynamics 365 for Sales Professional (NEW)</span></span>
- <span data-ttu-id="03525-144">Dynamics 365 for Customer Service</span><span class="sxs-lookup"><span data-stu-id="03525-144">Dynamics 365 for Customer Service</span></span>
- <span data-ttu-id="03525-145">Dynamics 365 Customer Engagement-plan eller</span><span class="sxs-lookup"><span data-stu-id="03525-145">Dynamics 365 Customer Engagement Plan or</span></span>
- <span data-ttu-id="03525-146">Dynamics 365-teammedlemmar</span><span class="sxs-lookup"><span data-stu-id="03525-146">Dynamics 365 Team Members</span></span>



## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="03525-147">Övergå kunder till nya produktplaner</span><span class="sxs-lookup"><span data-stu-id="03525-147">Transition customers to new product plans</span></span>

<span data-ttu-id="03525-148">Att flytta kunder från tillbakadragna SKU:er till nyare kräver följande steg i den här ordningen:</span><span class="sxs-lookup"><span data-stu-id="03525-148">Moving customers from retired SKUs to newer ones requires the following steps in this order:</span></span>

- <span data-ttu-id="03525-149">Köpa den nya prenumerationen</span><span class="sxs-lookup"><span data-stu-id="03525-149">Purchase the new subscription</span></span>
- <span data-ttu-id="03525-150">Tilldela om aktuella användarlicenser</span><span class="sxs-lookup"><span data-stu-id="03525-150">Reassign current user licenses</span></span>
- <span data-ttu-id="03525-151">Avbryta gammal prenumeration</span><span class="sxs-lookup"><span data-stu-id="03525-151">Cancel old subscription</span></span>

## <a name="purchase-the-new-plan-for-your-customer"></a><span data-ttu-id="03525-152">Köp den nya planen för din kund</span><span class="sxs-lookup"><span data-stu-id="03525-152">Purchase the new plan for your customer</span></span>

1. <span data-ttu-id="03525-153">Välj **Kunder** i det vänstra navigeringsfältet och välj sedan den kund som du vill flytta till den nya prenumerationen.</span><span class="sxs-lookup"><span data-stu-id="03525-153">Select **Customers** from the left nav and then select the customer you want to move to the new subscription.</span></span>
2. <span data-ttu-id="03525-154">Välj **Lägg till prenumeration.**</span><span class="sxs-lookup"><span data-stu-id="03525-154">Select **Add Subscription**.</span></span>
3. <span data-ttu-id="03525-155">Välj den prenumeration som du vill köpa från katalogen (i det här fallet något av alternativen ovan), ange antalet licenser och välj sedan **Skicka.**</span><span class="sxs-lookup"><span data-stu-id="03525-155">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span> 

<span data-ttu-id="03525-156">Kunden kommer nu att ha både den gamla och den nya.</span><span class="sxs-lookup"><span data-stu-id="03525-156">Your customer will now have both the old subscription and the new one.</span></span> <span data-ttu-id="03525-157">Nästa steg är att omtilldela licenser till kundens användare.</span><span class="sxs-lookup"><span data-stu-id="03525-157">Your next step is to reassign licenses to the customer's users.</span></span>

1. <span data-ttu-id="03525-158">Välj **Kunder** i det vänstra navigeringsfältet och välj sedan den kund som du flyttar.</span><span class="sxs-lookup"><span data-stu-id="03525-158">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="03525-159">Välj **Användare och licenser.**</span><span class="sxs-lookup"><span data-stu-id="03525-159">Select **Users and licenses**.</span></span>
3. <span data-ttu-id="03525-160">Om du vill tilldela om en licens till en användare väljer du användaren och sedan **Hantera licenser.**</span><span class="sxs-lookup"><span data-stu-id="03525-160">To reassign a license to a user, select the user and then select **Manage licenses**.</span></span> 
4. <span data-ttu-id="03525-161">På sidan **Hantera licenser** avmarkerar du kryssrutan Dynamics 365 for Sales/Customer Engagement Plan från Basic-licens (kvalificerat erbjudande) och väljer en ny tjänstplan för prenumerationen som kunden flyttar till.</span><span class="sxs-lookup"><span data-stu-id="03525-161">On the **Manage licenses** page, clear the Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offer) license check box and select a new service plan for the subscription the customer is moving to.</span></span> 
5. <span data-ttu-id="03525-162">Välj **Skicka**.</span><span class="sxs-lookup"><span data-stu-id="03525-162">Select **Submit**.</span></span> <span data-ttu-id="03525-163">Du gör detta för varje användare som behöver den nya licensen.</span><span class="sxs-lookup"><span data-stu-id="03525-163">You will do this for each user who needs the new license.</span></span> 

<span data-ttu-id="03525-164">När du har flyttat över licenserna till den nya prenumerationen kan du avbryta den gamla prenumerationen.</span><span class="sxs-lookup"><span data-stu-id="03525-164">Once you've moved the licenses over to the new subscription, you can cancel the old subscription.</span></span> 

1. <span data-ttu-id="03525-165">Välj **Kunder** i det vänstra navigeringsfältet och välj sedan den kund som du flyttar.</span><span class="sxs-lookup"><span data-stu-id="03525-165">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="03525-166">På sidan med prenumerationsdetaljer anger du den gamla prenumerationen till **Pausad** och väljer **Skicka**.</span><span class="sxs-lookup"><span data-stu-id="03525-166">On the subscription detail page, set the old subscription to **Suspended** and select **Submit**.</span></span>

<span data-ttu-id="03525-167">Den gamla prenumerationen har nu inaktiverats och den nya prenumerationen är aktiv.</span><span class="sxs-lookup"><span data-stu-id="03525-167">The old subscription is now suspended, and the new subscription is active.</span></span> <span data-ttu-id="03525-168">Den pausade prenumerationen avetableeras automatiskt efter 120 dagar.</span><span class="sxs-lookup"><span data-stu-id="03525-168">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="03525-169">Kunden medför inga ytterligare kostnader för den gamla prenumerationen.</span><span class="sxs-lookup"><span data-stu-id="03525-169">Your customer will incur no additional costs for the old subscription.</span></span>
 

 



