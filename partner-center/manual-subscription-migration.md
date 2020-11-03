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
ms.openlocfilehash: 8575d87ab3c4c7970135a87b7ef7564c4fe06232
ms.sourcegitcommit: 7153f0b8c67efd35f58695ca2a7e00e70da1c5e9
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 07/17/2020
ms.locfileid: "92531008"
---
# <a name="migrate-dynamics-365-and-customer-engagement-plan-from-basic-qualified-offers-to-newer-versions"></a><span data-ttu-id="2374c-103">Migrera Dynamics 365 och en plan för kundengagemang från Basic (kvalificerade erbjudanden) till nyare versioner</span><span class="sxs-lookup"><span data-stu-id="2374c-103">Migrate Dynamics 365 and Customer Engagement Plan from Basic (qualified offers) to newer versions</span></span>

<span data-ttu-id="2374c-104">**Gäller för**</span><span class="sxs-lookup"><span data-stu-id="2374c-104">**Applies to**</span></span>

-  <span data-ttu-id="2374c-105">Partnercenter</span><span class="sxs-lookup"><span data-stu-id="2374c-105">Partner Center</span></span>

<span data-ttu-id="2374c-106">**Lämpliga roller**</span><span class="sxs-lookup"><span data-stu-id="2374c-106">**Appropriate roles**</span></span>
-   <span data-ttu-id="2374c-107">Global administratör</span><span class="sxs-lookup"><span data-stu-id="2374c-107">Global admin</span></span>
-   <span data-ttu-id="2374c-108">Användaradministratör</span><span class="sxs-lookup"><span data-stu-id="2374c-108">User admin</span></span>
-   <span data-ttu-id="2374c-109">Administratörs agent</span><span class="sxs-lookup"><span data-stu-id="2374c-109">Admin agent</span></span>
-   <span data-ttu-id="2374c-110">Försäljnings agent</span><span class="sxs-lookup"><span data-stu-id="2374c-110">Sales agent</span></span>

<span data-ttu-id="2374c-111">Från och med den 1 januari 2019 kan kunder med Dynamics 365 för försäljnings-/kund engagemang avtal från Basic-prenumerationer (kvalificerade erbjudanden) inte längre förnya de här äldre erbjudandena. befintliga prenumerationer förnyas inte automatiskt när de upphör att gälla.</span><span class="sxs-lookup"><span data-stu-id="2374c-111">Effective January 1, 2019, customers with Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offers) subscriptions can no longer renew these legacy offers; existing subscriptions will not renew automatically when they expire.</span></span> <span data-ttu-id="2374c-112">På prenumerationens informations sida ändras prenumerations statusen till "upphör att gälla [datum]" från "Auto Regener på [Date]".</span><span class="sxs-lookup"><span data-stu-id="2374c-112">On the subscription's detail page, the subscription status will change to "Expires on [date]" from "Auto renews on [date]".</span></span> 

<span data-ttu-id="2374c-113">För att säkerställa kontinuitet för kunderna bör du gå över de med förfallna prenumerationer på ett alternativ som stöds.</span><span class="sxs-lookup"><span data-stu-id="2374c-113">To ensure continuity for customers, you should transition those with expiring subscriptions to a supported option, listed below.</span></span> <span data-ttu-id="2374c-114">Vi rekommenderar att du flyttar kunder till nya prenumerationer före prenumerationens årliga slutdatum för att undvika eventuella avbrott i tjänsten för kunderna.</span><span class="sxs-lookup"><span data-stu-id="2374c-114">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span>

<span data-ttu-id="2374c-115">Om du använder API: et (topp-eller partner Center) kan du hitta förfallna prenumerationer genom att utvärdera slutdatumet för prenumerationen tillsammans med egenskapen Auto renew = false.</span><span class="sxs-lookup"><span data-stu-id="2374c-115">If you use the API (either CREST or Partner Center), you can find expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.</span></span> <span data-ttu-id="2374c-116">Prenumerationerna i fråga kommer att ställas in på automatisk förnyelse = falskt den 1 januari 2019.</span><span class="sxs-lookup"><span data-stu-id="2374c-116">The subscriptions in question will be set to auto renew=False on Jan 1, 2019.</span></span> <span data-ttu-id="2374c-117">Du kan när som helst flytta kunder till en ny plan.</span><span class="sxs-lookup"><span data-stu-id="2374c-117">You can move customers to a new plan at any time.</span></span> 

### <a name="the-dynamics-365-offers-being-retired"></a><span data-ttu-id="2374c-118">Dynamics 365-erbjudanden som dras tillbaka</span><span class="sxs-lookup"><span data-stu-id="2374c-118">The Dynamics 365 offers being retired</span></span>

- <span data-ttu-id="2374c-119">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (kvalificerat erbjudande)</span><span class="sxs-lookup"><span data-stu-id="2374c-119">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="2374c-120">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (kvalificerat erbjudande) för lärare</span><span class="sxs-lookup"><span data-stu-id="2374c-120">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="2374c-121">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (kvalificerat erbjudande) för studenter</span><span class="sxs-lookup"><span data-stu-id="2374c-121">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="2374c-122">Dynamics 365 for Sales Enterprise Edition (myndighets prissättning) CRMOL Basic (kvalificerat erbjudande)</span><span class="sxs-lookup"><span data-stu-id="2374c-122">Dynamics 365 for Sales Enterprise Edition (Government Pricing) CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="2374c-123">Dynamics 365 för Sales Enterprise Edition från SA för CRM Basic (kvalificerat erbjudande)</span><span class="sxs-lookup"><span data-stu-id="2374c-123">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="2374c-124">Dynamics 365 för Sales Enterprise Edition från SA för CRM Basic (kvalificerat erbjudande) för lärare</span><span class="sxs-lookup"><span data-stu-id="2374c-124">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="2374c-125">Dynamics 365 för Sales Enterprise Edition från SA för CRM Basic (kvalificerat erbjudande) för studenter</span><span class="sxs-lookup"><span data-stu-id="2374c-125">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="2374c-126">Dynamics 365 for Sales Enterprise Edition (myndighets priser) från SA för CRM Basic (kvalificerat erbjudande)</span><span class="sxs-lookup"><span data-stu-id="2374c-126">Dynamics 365 for Sales Enterprise Edition (Government Pricing) From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="2374c-127">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (kvalificerat erbjudande)</span><span class="sxs-lookup"><span data-stu-id="2374c-127">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="2374c-128">Dynamics 365 for Sales Enterprise Edition Add-On för CRM Basic (kvalificerat erbjudande) för lärare</span><span class="sxs-lookup"><span data-stu-id="2374c-128">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="2374c-129">Dynamics 365 for Sales Enterprise Edition Add-On för CRM Basic (kvalificerat erbjudande) för studenter</span><span class="sxs-lookup"><span data-stu-id="2374c-129">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="2374c-130">Dynamics 365 for Sales Enterprise Edition (myndighets prissättning) Add-On för CRM Basic (kvalificerat erbjudande)</span><span class="sxs-lookup"><span data-stu-id="2374c-130">Dynamics 365 for Sales Enterprise Edition (Government Pricing) Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="2374c-131">Dynamics 365 Customer Engagement plan Enterprise Edition CRMOL Basic (kvalificerat erbjudande)</span><span class="sxs-lookup"><span data-stu-id="2374c-131">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="2374c-132">Dynamics 365 Customer Engagement plan Enterprise Edition (myndighets priser) CRMOL Basic (kvalificerat erbjudande)</span><span class="sxs-lookup"><span data-stu-id="2374c-132">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="2374c-133">Dynamics 365 Customer Engagement plan Enterprise Edition CRMOL Basic (kvalificerat erbjudande) för studenter</span><span class="sxs-lookup"><span data-stu-id="2374c-133">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="2374c-134">Dynamics 365 Customer Engagement plan Enterprise Edition CRMOL Basic (kvalificerat erbjudande) för lärare</span><span class="sxs-lookup"><span data-stu-id="2374c-134">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="2374c-135">Dynamics 365 kund engagemang plan Enterprise Edition från SA för CRM Basic (kvalificerat erbjudande)</span><span class="sxs-lookup"><span data-stu-id="2374c-135">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="2374c-136">Dynamics 365 Customer Engagement plan Enterprise Edition (prissättning för myndigheter) från SA för CRM Basic (kvalificerat erbjudande)</span><span class="sxs-lookup"><span data-stu-id="2374c-136">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="2374c-137">Dynamics 365 Customer Engagement plan Enterprise Edition från SA för CRM Basic (kvalificerat erbjudande) för studenter</span><span class="sxs-lookup"><span data-stu-id="2374c-137">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="2374c-138">Dynamics 365 Customer Engagement plan Enterprise Edition från SA för CRM Basic (kvalificerade erbjudanden) för lärare</span><span class="sxs-lookup"><span data-stu-id="2374c-138">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="2374c-139">Dynamics 365 Customer Engagement plan Enterprise Edition Add-On for CRM Basic (kvalificerat erbjudande)</span><span class="sxs-lookup"><span data-stu-id="2374c-139">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="2374c-140">Dynamics 365 Customer Engagement plan Enterprise Edition (myndighets prissättning) Add-On för CRM Basic (kvalificerat erbjudande)</span><span class="sxs-lookup"><span data-stu-id="2374c-140">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="2374c-141">Dynamics 365 Customer Engagement plan Enterprise Edition Add-On for CRM Basic (kvalificerat erbjudande) för studenter</span><span class="sxs-lookup"><span data-stu-id="2374c-141">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="2374c-142">Dynamics 365 Customer Engagement plan Enterprise Edition Add-On for CRM Basic (kvalificerade erbjudanden) för lärare</span><span class="sxs-lookup"><span data-stu-id="2374c-142">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Faculty</span></span>



## <a name="dynamics-365-for-sales-customer-engagement-plan-from-basic-qualified-offers-replacement-plans"></a><span data-ttu-id="2374c-143">Dynamics 365 för sälj-/kund engagemang-plan från Basic (kvalificerade erbjudanden) ersättnings planer</span><span class="sxs-lookup"><span data-stu-id="2374c-143">Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offers) replacement plans</span></span>

<span data-ttu-id="2374c-144">**Återkallade erbjudanden**</span><span class="sxs-lookup"><span data-stu-id="2374c-144">**Retired offers**</span></span>   

- <span data-ttu-id="2374c-145">Dynamics 365 för försäljning från CRM Basic eller CRMOL Basic (kvalificerat erbjudande)</span><span class="sxs-lookup"><span data-stu-id="2374c-145">Dynamics 365 for Sales from CRM Basic or CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="2374c-146">Dynamics 365 kund engagemang plan från CRM Basic eller CRMOL Basic (kvalificerat erbjudande)</span><span class="sxs-lookup"><span data-stu-id="2374c-146">Dynamics 365 Customer Engagement Plan from CRM Basic or CRMOL Basic (Qualified Offer)</span></span>

<span data-ttu-id="2374c-147">**Ersättnings alternativ**</span><span class="sxs-lookup"><span data-stu-id="2374c-147">**Replacement options**</span></span>
- <span data-ttu-id="2374c-148">Dynamics 365 for Sales Professional (ny)</span><span class="sxs-lookup"><span data-stu-id="2374c-148">Dynamics 365 for Sales Professional (NEW)</span></span>
- <span data-ttu-id="2374c-149">Dynamics 365 for Sales Professional (ny)</span><span class="sxs-lookup"><span data-stu-id="2374c-149">Dynamics 365 for Sales Professional (NEW)</span></span>
- <span data-ttu-id="2374c-150">Dynamics 365 for Customer Service</span><span class="sxs-lookup"><span data-stu-id="2374c-150">Dynamics 365 for Customer Service</span></span>
- <span data-ttu-id="2374c-151">Dynamics 365 kund engagemang plan eller</span><span class="sxs-lookup"><span data-stu-id="2374c-151">Dynamics 365 Customer Engagement Plan or</span></span>
- <span data-ttu-id="2374c-152">Dynamics 365-team medlemmar</span><span class="sxs-lookup"><span data-stu-id="2374c-152">Dynamics 365 Team Members</span></span>



## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="2374c-153">Överföra kunder till nya produkt planer</span><span class="sxs-lookup"><span data-stu-id="2374c-153">Transition customers to new product plans</span></span>

<span data-ttu-id="2374c-154">Att flytta kunder från tillbakadragna SKU: er till nyare kräver följande steg i den här ordningen:</span><span class="sxs-lookup"><span data-stu-id="2374c-154">Moving customers from retired SKUs to newer ones requires the following steps in this order:</span></span>

- <span data-ttu-id="2374c-155">Köp den nya prenumerationen</span><span class="sxs-lookup"><span data-stu-id="2374c-155">Purchase the new subscription</span></span>
- <span data-ttu-id="2374c-156">Tilldela om aktuella användar licenser</span><span class="sxs-lookup"><span data-stu-id="2374c-156">Reassign current user licenses</span></span>
- <span data-ttu-id="2374c-157">Avbryt gammal prenumeration</span><span class="sxs-lookup"><span data-stu-id="2374c-157">Cancel old subscription</span></span>

## <a name="purchase-the-new-plan-for-your-customer"></a><span data-ttu-id="2374c-158">Köp det nya avtalet för kunden</span><span class="sxs-lookup"><span data-stu-id="2374c-158">Purchase the new plan for your customer</span></span>

1. <span data-ttu-id="2374c-159">Välj **kunder** i det vänstra navigerings fältet och välj sedan den kund som du vill flytta till den nya prenumerationen.</span><span class="sxs-lookup"><span data-stu-id="2374c-159">Select **Customers** from the left nav and then select the customer you want to move to the new subscription.</span></span>
2. <span data-ttu-id="2374c-160">Välj **Lägg till prenumeration** .</span><span class="sxs-lookup"><span data-stu-id="2374c-160">Select **Add Subscription** .</span></span>
3. <span data-ttu-id="2374c-161">Välj den prenumeration som du vill köpa från katalogen (i det här fallet ett av alternativen ovan), ange antalet licenser och välj sedan **Skicka** .</span><span class="sxs-lookup"><span data-stu-id="2374c-161">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit** .</span></span> 

<span data-ttu-id="2374c-162">Din kund kommer nu att ha både den gamla och den nya prenumerationen.</span><span class="sxs-lookup"><span data-stu-id="2374c-162">Your customer will now have both the old subscription and the new one.</span></span> <span data-ttu-id="2374c-163">Nästa steg är att omtilldela licenser till kundens användare.</span><span class="sxs-lookup"><span data-stu-id="2374c-163">Your next step is to reassign licenses to the customer's users.</span></span>

1. <span data-ttu-id="2374c-164">Välj **kunder** i det vänstra navigerings fältet och välj sedan den kund som du flyttar.</span><span class="sxs-lookup"><span data-stu-id="2374c-164">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="2374c-165">Välj **användare och licenser** .</span><span class="sxs-lookup"><span data-stu-id="2374c-165">Select **Users and licenses** .</span></span>
3. <span data-ttu-id="2374c-166">Om du vill tilldela en licens till en användare igen väljer du användaren och väljer sedan **Hantera licenser** .</span><span class="sxs-lookup"><span data-stu-id="2374c-166">To reassign a license to a user, select the user and then select **Manage licenses** .</span></span> 
4. <span data-ttu-id="2374c-167">På sidan **Hantera licenser** avmarkerar du kryss rutan Dynamics 365 för sälj-/kund engagemang från Basic-licens (kvalificerad erbjudande) och väljer en ny service plan för den prenumeration som kunden flyttar till.</span><span class="sxs-lookup"><span data-stu-id="2374c-167">On the **Manage licenses** page, clear the Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offer) license check box and select a new service plan for the subscription the customer is moving to.</span></span> 
5. <span data-ttu-id="2374c-168">Välj **Skicka** .</span><span class="sxs-lookup"><span data-stu-id="2374c-168">Select **Submit** .</span></span> <span data-ttu-id="2374c-169">Du kommer att göra detta för varje användare som behöver den nya licensen.</span><span class="sxs-lookup"><span data-stu-id="2374c-169">You will do this for each user who needs the new license.</span></span> 

<span data-ttu-id="2374c-170">När du har flyttat licenserna till den nya prenumerationen kan du avbryta den gamla prenumerationen.</span><span class="sxs-lookup"><span data-stu-id="2374c-170">Once you've moved the licenses over to the new subscription you can cancel the old subscription.</span></span> 

1. <span data-ttu-id="2374c-171">Välj **kunder** i det vänstra navigerings fältet och välj sedan den kund som du flyttar.</span><span class="sxs-lookup"><span data-stu-id="2374c-171">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="2374c-172">På sidan prenumerations information anger du att den gamla prenumerationen har **pausats** och väljer **Skicka** .</span><span class="sxs-lookup"><span data-stu-id="2374c-172">On the subscription detail page, set the old subscription to **Suspended** and select **Submit** .</span></span>

<span data-ttu-id="2374c-173">Den gamla prenumerationen är nu inaktive rad och den nya prenumerationen är aktiv.</span><span class="sxs-lookup"><span data-stu-id="2374c-173">The old subscription is now suspended, and the new subscription is active.</span></span> <span data-ttu-id="2374c-174">Den inaktiverade prenumerationen kommer att avetableras automatiskt efter 120 dagar.</span><span class="sxs-lookup"><span data-stu-id="2374c-174">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="2374c-175">Kunden debiteras inga ytterligare kostnader för den gamla prenumerationen.</span><span class="sxs-lookup"><span data-stu-id="2374c-175">Your customer will incur no additional costs for the old subscription.</span></span>
 

 



