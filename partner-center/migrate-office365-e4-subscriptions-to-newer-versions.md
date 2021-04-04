---
title: Migrera Office 365 E4-prenumerationer
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Microsoft Office 365 Enterprise E4 Edition dras tillbaka den 7 april 2017. Lär dig hur du migrerar kund prenumerationer till nyare versioner av Office 365.
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 8a9662e0ce99fc054149dfbd4149532ce336eff6
ms.sourcegitcommit: f24089cd27b1de6ecf6ddbefb6cbb2d340e144de
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/01/2021
ms.locfileid: "106132629"
---
# <a name="migrate-office-365-e4-subscriptions-to-newer-office-365-versions"></a><span data-ttu-id="c1da3-104">Migrera Office 365 E4-prenumerationer till senare Office 365-versioner</span><span class="sxs-lookup"><span data-stu-id="c1da3-104">Migrate Office 365 E4 subscriptions to newer Office 365 versions</span></span>

<span data-ttu-id="c1da3-105">**Lämpliga roller**</span><span class="sxs-lookup"><span data-stu-id="c1da3-105">**Appropriate roles**</span></span>

- <span data-ttu-id="c1da3-106">Global administratör</span><span class="sxs-lookup"><span data-stu-id="c1da3-106">Global admin</span></span>
- <span data-ttu-id="c1da3-107">Administratör för användar hantering</span><span class="sxs-lookup"><span data-stu-id="c1da3-107">User management admin</span></span>
- <span data-ttu-id="c1da3-108">Administratörs agent</span><span class="sxs-lookup"><span data-stu-id="c1da3-108">Admin agent</span></span>
- <span data-ttu-id="c1da3-109">Försäljnings agent</span><span class="sxs-lookup"><span data-stu-id="c1da3-109">Sales agent</span></span>

<span data-ttu-id="c1da3-110">Office 365 Enterprise E4 plan dras tillbaka, från och med 7 april 2017.</span><span class="sxs-lookup"><span data-stu-id="c1da3-110">The Office 365 Enterprise E4 plan is retired, effective April 7, 2017.</span></span> <span data-ttu-id="c1da3-111">Du kan inte längre köpa nya Office 365 E4-prenumerationer efter det här datumet och befintliga E4-prenumerationer kommer inte att förnyas automatiskt när de upphör att gälla.</span><span class="sxs-lookup"><span data-stu-id="c1da3-111">You can no longer purchase new Office 365 E4 subscriptions after this date, and existing E4 subscriptions will not renew automatically when they expire.</span></span>

<span data-ttu-id="c1da3-112">När E4-prenumerationer slutar, kommer de att avbrytas.</span><span class="sxs-lookup"><span data-stu-id="c1da3-112">When E4 subscriptions end, they will be canceled.</span></span> <span data-ttu-id="c1da3-113">För att säkerställa kontinuitet för kunderna bör du överföra kunder med att förfalla E4-prenumerationer till ett SKU-alternativ som stöds, som anges nedan.</span><span class="sxs-lookup"><span data-stu-id="c1da3-113">To ensure continuity for customers, you should transition customers with expiring E4 subscriptions to a supported SKU option, listed below.</span></span> <span data-ttu-id="c1da3-114">Vi rekommenderar att du flyttar kunder till nya prenumerationer före prenumerationens årliga slutdatum för att undvika eventuella avbrott i tjänsten för kunderna.</span><span class="sxs-lookup"><span data-stu-id="c1da3-114">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span> 

> [!NOTE]  
> <span data-ttu-id="c1da3-115">Både Office 365 Enterprise E4-kommersiella och offentliga SKU: er dras tillbaka.</span><span class="sxs-lookup"><span data-stu-id="c1da3-115">Both Office 365 Enterprise E4 commercial and government SKUs are retired.</span></span>
 
<span data-ttu-id="c1da3-116">På prenumerationens informations sida har status för E4-prenumerationen ändrats till "upphör att gälla [datum]" från "Auto News på [Date]".</span><span class="sxs-lookup"><span data-stu-id="c1da3-116">On the subscription's detail page, the E4 subscription status has changed to "Expires on [date]" from "Auto renews on [date]".</span></span> 

<span data-ttu-id="c1da3-117">Om du använder API: et (topp eller partner Center) kan du identifiera prenumerationer som upphör att gälla genom att utvärdera slutdatumet för prenumerationen tillsammans med egenskapen Auto renew = false.</span><span class="sxs-lookup"><span data-stu-id="c1da3-117">If you use the API (either CREST or Partner Center), you can discover expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.</span></span> 

<span data-ttu-id="c1da3-118">E4-prenumerationerna ställs in på automatisk förnyelse = falskt i den 7 april 2017.</span><span class="sxs-lookup"><span data-stu-id="c1da3-118">The E4 subscriptions will be set to auto renew=False in April 7, 2017.</span></span> <span data-ttu-id="c1da3-119">Du kan när som helst flytta kunder till en ny plan.</span><span class="sxs-lookup"><span data-stu-id="c1da3-119">You can move customers to a new plan at any time.</span></span> 

## <a name="office-365-enterprise-e4-edition-replacement-plans"></a><span data-ttu-id="c1da3-120">Ersättnings planer för Office 365 Enterprise E4 Edition</span><span class="sxs-lookup"><span data-stu-id="c1da3-120">Office 365 Enterprise E4 edition replacement plans</span></span>

<span data-ttu-id="c1da3-121">Du kan välja att behålla samma funktioner med E4 eller låta dina kunder dra nytta av nya funktioner i Office 365 och Skype för företag – online.</span><span class="sxs-lookup"><span data-stu-id="c1da3-121">You can choose to maintain the same functionality with E4 or have your customers take advantage of newer features and functionality in Office 365 and Skype for Business Online.</span></span> <span data-ttu-id="c1da3-122">Pris information finns i matrisen pris lista och erbjudande lista i Partner Center.</span><span class="sxs-lookup"><span data-stu-id="c1da3-122">Pricing details are found on the price list and offer list matrix in Partner Center.</span></span> <span data-ttu-id="c1da3-123">Säker produkt Enterprise E3 eller Secure produktiv Enterprise E5 kan ersättas med följande alternativ för Office 365 Enterprise E3 eller Office 365 Enterprise E5.</span><span class="sxs-lookup"><span data-stu-id="c1da3-123">Secure Product Enterprise E3 or Secure Productive Enterprise E5 may be substituted in the following options for Office 365 Enterprise E3 or Office 365 Enterprise E5 respectively.</span></span>

- <span data-ttu-id="c1da3-124">Alternativ 1: Office 365 Enterprise E5</span><span class="sxs-lookup"><span data-stu-id="c1da3-124">Option 1: Office 365 Enterprise E5</span></span>

- <span data-ttu-id="c1da3-125">Alternativ 2: Office 365 Enterprise E3 + Skype för företag Cloud PBX</span><span class="sxs-lookup"><span data-stu-id="c1da3-125">Option 2: Office 365 Enterprise E3 + Skype for Business Cloud PBX</span></span>

- <span data-ttu-id="c1da3-126">Alternativ 3: Office 365 Enterprise E3 + Skype för företag Plus CAL (pris-och funktions paritet med E4)</span><span class="sxs-lookup"><span data-stu-id="c1da3-126">Option 3: Office 365 Enterprise E3 + Skype for Business Plus CAL (price and functionality parity with E4)</span></span>

- <span data-ttu-id="c1da3-127">Alternativ 4: Office 365 Enterprise E3</span><span class="sxs-lookup"><span data-stu-id="c1da3-127">Option 4: Office 365 Enterprise E3</span></span>


| <span data-ttu-id="c1da3-128">Funktion</span><span class="sxs-lookup"><span data-stu-id="c1da3-128">Feature</span></span> | <span data-ttu-id="c1da3-129">Alternativ 1</span><span class="sxs-lookup"><span data-stu-id="c1da3-129">Option 1</span></span> | <span data-ttu-id="c1da3-130">Alternativ 2</span><span class="sxs-lookup"><span data-stu-id="c1da3-130">Option 2</span></span> | <span data-ttu-id="c1da3-131">Alternativ 3</span><span class="sxs-lookup"><span data-stu-id="c1da3-131">Option 3</span></span> | <span data-ttu-id="c1da3-132">Alternativ 4</span><span class="sxs-lookup"><span data-stu-id="c1da3-132">Option 4</span></span> |
| :---    | :------: |   :---:  |   :---:  |   :---:  |
| <span data-ttu-id="c1da3-133">Hämta alla funktioner som ingår i Office 365 Enterprise E4?</span><span class="sxs-lookup"><span data-stu-id="c1da3-133">Get all the features included in Office 365 Enterprise E4?</span></span> | <span data-ttu-id="c1da3-134">Ja</span><span class="sxs-lookup"><span data-stu-id="c1da3-134">Yes</span></span> | <span data-ttu-id="c1da3-135">Ja</span><span class="sxs-lookup"><span data-stu-id="c1da3-135">Yes</span></span> | <span data-ttu-id="c1da3-136">Ja</span><span class="sxs-lookup"><span data-stu-id="c1da3-136">Yes</span></span> | <span data-ttu-id="c1da3-137">Inga</span><span class="sxs-lookup"><span data-stu-id="c1da3-137">No</span></span> |
| <span data-ttu-id="c1da3-138">Telefonnummer som hanteras i Office 365?</span><span class="sxs-lookup"><span data-stu-id="c1da3-138">Phone numbers managed in Office 365?</span></span> | <span data-ttu-id="c1da3-139">Ja</span><span class="sxs-lookup"><span data-stu-id="c1da3-139">Yes</span></span> | <span data-ttu-id="c1da3-140">Ja</span><span class="sxs-lookup"><span data-stu-id="c1da3-140">Yes</span></span> | <span data-ttu-id="c1da3-141">Inga</span><span class="sxs-lookup"><span data-stu-id="c1da3-141">No</span></span> | <span data-ttu-id="c1da3-142">Inga</span><span class="sxs-lookup"><span data-stu-id="c1da3-142">No</span></span> |
| <span data-ttu-id="c1da3-143">De telefonnummer som hanteras både lokalt och i Office 365 (hybrid distribution)?</span><span class="sxs-lookup"><span data-stu-id="c1da3-143">Phone numbers managed both on-premises and in Office 365 (hybrid deployment)?</span></span> | <span data-ttu-id="c1da3-144">Ja</span><span class="sxs-lookup"><span data-stu-id="c1da3-144">Yes</span></span> | <span data-ttu-id="c1da3-145">Ja</span><span class="sxs-lookup"><span data-stu-id="c1da3-145">Yes</span></span> | <span data-ttu-id="c1da3-146">Inga</span><span class="sxs-lookup"><span data-stu-id="c1da3-146">No</span></span> | <span data-ttu-id="c1da3-147">Inga</span><span class="sxs-lookup"><span data-stu-id="c1da3-147">No</span></span> |
| <span data-ttu-id="c1da3-148">Alternativ för att lägga till en PSTN-röst samtals plan?</span><span class="sxs-lookup"><span data-stu-id="c1da3-148">Option to add a PSTN voice calling plan?</span></span> | <span data-ttu-id="c1da3-149">Ja</span><span class="sxs-lookup"><span data-stu-id="c1da3-149">Yes</span></span> | <span data-ttu-id="c1da3-150">Ja</span><span class="sxs-lookup"><span data-stu-id="c1da3-150">Yes</span></span> | <span data-ttu-id="c1da3-151">Inga</span><span class="sxs-lookup"><span data-stu-id="c1da3-151">No</span></span> | <span data-ttu-id="c1da3-152">Inga</span><span class="sxs-lookup"><span data-stu-id="c1da3-152">No</span></span> |
| <span data-ttu-id="c1da3-153">PSTN-konferens?</span><span class="sxs-lookup"><span data-stu-id="c1da3-153">PSTN Conferencing?</span></span> | <span data-ttu-id="c1da3-154">Ja</span><span class="sxs-lookup"><span data-stu-id="c1da3-154">Yes</span></span> | <span data-ttu-id="c1da3-155">Inga</span><span class="sxs-lookup"><span data-stu-id="c1da3-155">No</span></span> | <span data-ttu-id="c1da3-156">Inga</span><span class="sxs-lookup"><span data-stu-id="c1da3-156">No</span></span> | <span data-ttu-id="c1da3-157">Inga</span><span class="sxs-lookup"><span data-stu-id="c1da3-157">No</span></span> |
| <span data-ttu-id="c1da3-158">Avancerade verktyg för samarbete, analys och säkerhet?</span><span class="sxs-lookup"><span data-stu-id="c1da3-158">Advanced tools for collaboration, analytics, and security?</span></span> | <span data-ttu-id="c1da3-159">Ja</span><span class="sxs-lookup"><span data-stu-id="c1da3-159">Yes</span></span> | <span data-ttu-id="c1da3-160">Inga</span><span class="sxs-lookup"><span data-stu-id="c1da3-160">No</span></span> | <span data-ttu-id="c1da3-161">Inga</span><span class="sxs-lookup"><span data-stu-id="c1da3-161">No</span></span> | <span data-ttu-id="c1da3-162">Inga</span><span class="sxs-lookup"><span data-stu-id="c1da3-162">No</span></span> |
| <span data-ttu-id="c1da3-163">Interaktiva rapporter, instrument paneler och data visualiseringar?</span><span class="sxs-lookup"><span data-stu-id="c1da3-163">Interactive reports, dashboards, and data visualizations?</span></span> | <span data-ttu-id="c1da3-164">Ja</span><span class="sxs-lookup"><span data-stu-id="c1da3-164">Yes</span></span> | <span data-ttu-id="c1da3-165">Inga</span><span class="sxs-lookup"><span data-stu-id="c1da3-165">No</span></span> | <span data-ttu-id="c1da3-166">Inga</span><span class="sxs-lookup"><span data-stu-id="c1da3-166">No</span></span> | <span data-ttu-id="c1da3-167">Inga</span><span class="sxs-lookup"><span data-stu-id="c1da3-167">No</span></span> | 
| <span data-ttu-id="c1da3-168">Mer kontroll över data säkerhet och efterlevnad med inbyggda sekretess-, genomskinlighets-och raffinerade användar kontroller?</span><span class="sxs-lookup"><span data-stu-id="c1da3-168">More control over data security and compliance with built-in privacy, transparency, and refined user controls?</span></span> | <span data-ttu-id="c1da3-169">Ja</span><span class="sxs-lookup"><span data-stu-id="c1da3-169">Yes</span></span> | <span data-ttu-id="c1da3-170">Inga</span><span class="sxs-lookup"><span data-stu-id="c1da3-170">No</span></span> | <span data-ttu-id="c1da3-171">Inga</span><span class="sxs-lookup"><span data-stu-id="c1da3-171">No</span></span> | <span data-ttu-id="c1da3-172">Inga</span><span class="sxs-lookup"><span data-stu-id="c1da3-172">No</span></span> | 

## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="c1da3-173">Överföra kunder till nya produkt planer</span><span class="sxs-lookup"><span data-stu-id="c1da3-173">Transition customers to new product plans</span></span>

<span data-ttu-id="c1da3-174">Microsoft erbjuder kontinuerligt nya produkter och tjänster till våra partner.</span><span class="sxs-lookup"><span data-stu-id="c1da3-174">Microsoft continuously offers new products and services to our partners.</span></span> <span data-ttu-id="c1da3-175">I dessa fall kan du behöva uppgradera kunder till nya tjänster eller migrera sina prenumerationer från SKU: er som slutligen kommer att stängas av.</span><span class="sxs-lookup"><span data-stu-id="c1da3-175">In these cases, you may need to upgrade customers to new services or migrate their subscriptions from SKUs that will eventually be shut down.</span></span> <span data-ttu-id="c1da3-176">Migrering av kunder från tillbakadragna SKU: er till nyare kräver följande steg:</span><span class="sxs-lookup"><span data-stu-id="c1da3-176">Migrating customers from retired SKUs to newer ones requires the following steps:</span></span>

-   <span data-ttu-id="c1da3-177">Köp den nya prenumerationen</span><span class="sxs-lookup"><span data-stu-id="c1da3-177">Purchase the new subscription</span></span>
-   <span data-ttu-id="c1da3-178">Tilldela om aktuella användar licenser</span><span class="sxs-lookup"><span data-stu-id="c1da3-178">Reassign current user licenses</span></span>
-   <span data-ttu-id="c1da3-179">Avbryt den gamla prenumerationen</span><span class="sxs-lookup"><span data-stu-id="c1da3-179">Cancel the old subscription</span></span>

<span data-ttu-id="c1da3-180">Följ dessa steg om du vill migrera en kunds Office 365 Enterprise E4-prenumeration till något av alternativen i tabellen ovan.</span><span class="sxs-lookup"><span data-stu-id="c1da3-180">Follow these steps to migrate a customer's Office 365 Enterprise E4 subscription to one of the options in the table above.</span></span>

### <a name="step-1---purchase-the-new-subscription"></a><span data-ttu-id="c1da3-181">Steg 1 – Köp den nya prenumerationen</span><span class="sxs-lookup"><span data-stu-id="c1da3-181">Step 1 - Purchase the new subscription</span></span>

1. <span data-ttu-id="c1da3-182">Från menyn **partner Center** väljer du **kunder**, väljer kunden som du vill flytta och väljer sedan **Lägg till prenumerationer**.</span><span class="sxs-lookup"><span data-stu-id="c1da3-182">From the **Partner Center** menu, select **Customers**, select the customer you wish to move, and then select **Add subscriptions**.</span></span>

2. <span data-ttu-id="c1da3-183">Välj den prenumeration som du vill köpa från katalogen (i det här fallet ett av alternativen ovan), ange antalet licenser och välj sedan **Skicka**.</span><span class="sxs-lookup"><span data-stu-id="c1da3-183">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span>

   <span data-ttu-id="c1da3-184">Kunden bör nu ha både gamla och nya prenumerationer, den gamla Office 365 Enterprise E4-prenumerationen och den nya mål prenumerationen, till exempel alternativ 1-Office 365 Enterprise E5.</span><span class="sxs-lookup"><span data-stu-id="c1da3-184">Your customer should now have both old and new subscriptions, the old Office 365 Enterprise E4 subscription and the new 'target' subscription, for example, Option 1 - Office 365 Enterprise E5.</span></span>

### <a name="step-2---reassign-the-customers-users-licenses"></a><span data-ttu-id="c1da3-185">Steg 2 – tilldela om kundens användares licenser</span><span class="sxs-lookup"><span data-stu-id="c1da3-185">Step 2 - Reassign the customer's users' licenses</span></span>

1. <span data-ttu-id="c1da3-186">Från menyn **partner Center** väljer du **kunder**, väljer kunden som du vill flytta och väljer sedan **användare och licenser**.</span><span class="sxs-lookup"><span data-stu-id="c1da3-186">From the **Partner Center** menu, select **Customers**, select the customer you wish to move, and then select **Users and licenses**.</span></span> <span data-ttu-id="c1da3-187">Sidan kund användare och licenser öppnas.</span><span class="sxs-lookup"><span data-stu-id="c1da3-187">The customer's Users and Licenses page opens.</span></span>

2. <span data-ttu-id="c1da3-188">Om du vill omtilldela användar licenser väljer du den användare som ska omtilldelas och väljer sedan **Hantera licenser**.</span><span class="sxs-lookup"><span data-stu-id="c1da3-188">To reassign user licenses, select the user to reassign and then select **Manage licenses**.</span></span>

3. <span data-ttu-id="c1da3-189">På sidan **Hantera licenser** avmarkerar du kryss rutan **Office 365 Enterprise E4** -licens och väljer en ny service plan för den prenumeration som kunden flyttar till.</span><span class="sxs-lookup"><span data-stu-id="c1da3-189">On the **Manage licenses** page, clear the **Office 365 Enterprise E4** license check box and select a new service plan for the subscription the customer is moving to.</span></span>

4. <span data-ttu-id="c1da3-190">Välj **Skicka**.</span><span class="sxs-lookup"><span data-stu-id="c1da3-190">Select **Submit**.</span></span> <span data-ttu-id="c1da3-191">En bekräftelse sida listar de nya licens tilldelningarna.</span><span class="sxs-lookup"><span data-stu-id="c1da3-191">A confirmation page lists the new license assignments.</span></span>

5. <span data-ttu-id="c1da3-192">Fortsätt på samma sätt med andra kund användare som behöver omtilldela licenser.</span><span class="sxs-lookup"><span data-stu-id="c1da3-192">Continue the same steps with any other customer users that need license reassignment.</span></span>

<span data-ttu-id="c1da3-193">När du har flyttat användar licenserna till den nya tjänsten kan du på ett säkert sätt avbryta den tillbakadragna prenumerationen på den översta kund nivån.</span><span class="sxs-lookup"><span data-stu-id="c1da3-193">After moving the user licenses to the new service, you can safely cancel the retired subscription at the top Customer level.</span></span>

### <a name="step-3---cancel-the-old-subscription"></a><span data-ttu-id="c1da3-194">Steg 3 – Avbryt den gamla prenumerationen</span><span class="sxs-lookup"><span data-stu-id="c1da3-194">Step 3 - Cancel the old subscription</span></span>

1. <span data-ttu-id="c1da3-195">Från menyn **partner Center** väljer du **kunder**.</span><span class="sxs-lookup"><span data-stu-id="c1da3-195">From the **Partner Center** menu, select **Customers**.</span></span> <span data-ttu-id="c1da3-196">Välj den kund som du vill flytta och välj den prenumeration som du vill avbryta.</span><span class="sxs-lookup"><span data-stu-id="c1da3-196">Select the customer you want to move, and select the subscription you want to cancel.</span></span>

2. <span data-ttu-id="c1da3-197">På sidan prenumerations information anger du prenumerations statusen **pausad**.</span><span class="sxs-lookup"><span data-stu-id="c1da3-197">In the subscription details page, set the subscription status to **Suspended**.</span></span>

3. <span data-ttu-id="c1da3-198">Välj **Skicka**.</span><span class="sxs-lookup"><span data-stu-id="c1da3-198">Select **Submit**.</span></span>

<span data-ttu-id="c1da3-199">Den gamla prenumerationen har pausats och den nya prenumerationen är aktiv.</span><span class="sxs-lookup"><span data-stu-id="c1da3-199">The old subscription is suspended and the new subscription is active.</span></span> <span data-ttu-id="c1da3-200">Den inaktiverade prenumerationen kommer att avetableras automatiskt efter 120 dagar.</span><span class="sxs-lookup"><span data-stu-id="c1da3-200">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="c1da3-201">Kunden debiteras inga ytterligare kostnader för den gamla prenumerationen.</span><span class="sxs-lookup"><span data-stu-id="c1da3-201">The customer incurs no additional costs for the old subscription.</span></span>



 



