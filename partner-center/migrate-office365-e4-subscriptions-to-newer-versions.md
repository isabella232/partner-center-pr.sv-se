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
ms.openlocfilehash: bbd2aceac62a7e726ed81a78305ea23213c94156
ms.sourcegitcommit: 36a60f672c1c3d6b63fd225d04c5ffa917694ae0
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 07/03/2020
ms.locfileid: "92529179"
---
# <a name="migrate-office-365-e4-subscriptions-to-newer-office-365-versions"></a><span data-ttu-id="8d035-104">Migrera Office 365 E4-prenumerationer till senare Office 365-versioner</span><span class="sxs-lookup"><span data-stu-id="8d035-104">Migrate Office 365 E4 subscriptions to newer Office 365 versions</span></span>

<span data-ttu-id="8d035-105">**Gäller för**</span><span class="sxs-lookup"><span data-stu-id="8d035-105">**Applies to**</span></span>

-  <span data-ttu-id="8d035-106">Partnercenter</span><span class="sxs-lookup"><span data-stu-id="8d035-106">Partner Center</span></span>

<span data-ttu-id="8d035-107">**Lämpliga roller**</span><span class="sxs-lookup"><span data-stu-id="8d035-107">**Appropriate roles**</span></span>
-   <span data-ttu-id="8d035-108">Global administratör</span><span class="sxs-lookup"><span data-stu-id="8d035-108">Global admin</span></span>
-   <span data-ttu-id="8d035-109">Användaradministratör</span><span class="sxs-lookup"><span data-stu-id="8d035-109">User admin</span></span>
-   <span data-ttu-id="8d035-110">Administratörs agent</span><span class="sxs-lookup"><span data-stu-id="8d035-110">Admin agent</span></span>
-   <span data-ttu-id="8d035-111">Försäljnings agent</span><span class="sxs-lookup"><span data-stu-id="8d035-111">Sales agent</span></span>

<span data-ttu-id="8d035-112">Office 365 Enterprise E4 plan dras tillbaka, från och med 7 april 2017.</span><span class="sxs-lookup"><span data-stu-id="8d035-112">The Office 365 Enterprise E4 plan is retired, effective April 7, 2017.</span></span> <span data-ttu-id="8d035-113">Du kan inte längre köpa nya Office 365 E4-prenumerationer efter det här datumet och befintliga E4-prenumerationer kommer inte att förnyas automatiskt när de upphör att gälla.</span><span class="sxs-lookup"><span data-stu-id="8d035-113">You can no longer purchase new Office 365 E4 subscriptions after this date, and existing E4 subscriptions will not renew automatically when they expire.</span></span>

<span data-ttu-id="8d035-114">När E4-prenumerationer slutar, kommer de att avbrytas.</span><span class="sxs-lookup"><span data-stu-id="8d035-114">When E4 subscriptions end, they will be canceled.</span></span> <span data-ttu-id="8d035-115">För att säkerställa kontinuitet för kunderna bör du överföra kunder med att förfalla E4-prenumerationer till ett SKU-alternativ som stöds, som anges nedan.</span><span class="sxs-lookup"><span data-stu-id="8d035-115">To ensure continuity for customers, you should transition customers with expiring E4 subscriptions to a supported SKU option, listed below.</span></span> <span data-ttu-id="8d035-116">Vi rekommenderar att du flyttar kunder till nya prenumerationer före prenumerationens årliga slutdatum för att undvika eventuella avbrott i tjänsten för kunderna.</span><span class="sxs-lookup"><span data-stu-id="8d035-116">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span> 

> [!NOTE]  
> <span data-ttu-id="8d035-117">Både Office 365 Enterprise E4-kommersiella och offentliga SKU: er dras tillbaka.</span><span class="sxs-lookup"><span data-stu-id="8d035-117">Both Office 365 Enterprise E4 commercial and government SKUs are retired.</span></span>
 
<span data-ttu-id="8d035-118">På prenumerationens informations sida har status för E4-prenumerationen ändrats till "upphör att gälla [datum]" från "Auto News på [Date]".</span><span class="sxs-lookup"><span data-stu-id="8d035-118">On the subscription's detail page, the E4 subscription status has changed to "Expires on [date]" from "Auto renews on [date]".</span></span> 

<span data-ttu-id="8d035-119">Om du använder API: et (topp eller partner Center) kan du identifiera prenumerationer som upphör att gälla genom att utvärdera slutdatumet för prenumerationen tillsammans med egenskapen Auto renew = false.</span><span class="sxs-lookup"><span data-stu-id="8d035-119">If you use the API (either CREST or Partner Center), you can discover expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.</span></span> 

<span data-ttu-id="8d035-120">E4-prenumerationerna ställs in på automatisk förnyelse = falskt i den 7 april 2017.</span><span class="sxs-lookup"><span data-stu-id="8d035-120">The E4 subscriptions will be set to auto renew=False in April 7, 2017.</span></span> <span data-ttu-id="8d035-121">Du kan när som helst flytta kunder till en ny plan.</span><span class="sxs-lookup"><span data-stu-id="8d035-121">You can move customers to a new plan at any time.</span></span> 

## <a name="office-365-enterprise-e4-edition-replacement-plans"></a><span data-ttu-id="8d035-122">Ersättnings planer för Office 365 Enterprise E4 Edition</span><span class="sxs-lookup"><span data-stu-id="8d035-122">Office 365 Enterprise E4 edition replacement plans</span></span>

<span data-ttu-id="8d035-123">Du kan välja att behålla samma funktioner med E4 eller låta dina kunder dra nytta av nya funktioner i Office 365 och Skype för företag – online.</span><span class="sxs-lookup"><span data-stu-id="8d035-123">You can choose to maintain the same functionality with E4 or have your customers take advantage of newer features and functionality in Office 365 and Skype for Business Online.</span></span> <span data-ttu-id="8d035-124">Pris information finns i matrisen pris lista och erbjudande lista i Partner Center.</span><span class="sxs-lookup"><span data-stu-id="8d035-124">Pricing details are found on the price list and offer list matrix in Partner Center.</span></span> <span data-ttu-id="8d035-125">Säker produkt Enterprise E3 eller Secure produktiv Enterprise E5 kan ersättas med följande alternativ för Office 365 Enterprise E3 eller Office 365 Enterprise E5.</span><span class="sxs-lookup"><span data-stu-id="8d035-125">Secure Product Enterprise E3 or Secure Productive Enterprise E5 may be substituted in the following options for Office 365 Enterprise E3 or Office 365 Enterprise E5 respectively.</span></span>

- <span data-ttu-id="8d035-126">Alternativ 1: Office 365 Enterprise E5</span><span class="sxs-lookup"><span data-stu-id="8d035-126">Option 1: Office 365 Enterprise E5</span></span>

- <span data-ttu-id="8d035-127">Alternativ 2: Office 365 Enterprise E3 + Skype för företag Cloud PBX</span><span class="sxs-lookup"><span data-stu-id="8d035-127">Option 2: Office 365 Enterprise E3 + Skype for Business Cloud PBX</span></span>

- <span data-ttu-id="8d035-128">Alternativ 3: Office 365 Enterprise E3 + Skype för företag Plus CAL (pris-och funktions paritet med E4)</span><span class="sxs-lookup"><span data-stu-id="8d035-128">Option 3: Office 365 Enterprise E3 + Skype for Business Plus CAL (price and functionality parity with E4)</span></span>

- <span data-ttu-id="8d035-129">Alternativ 4: Office 365 Enterprise E3</span><span class="sxs-lookup"><span data-stu-id="8d035-129">Option 4: Office 365 Enterprise E3</span></span>


| <span data-ttu-id="8d035-130">Funktion</span><span class="sxs-lookup"><span data-stu-id="8d035-130">Feature</span></span> | <span data-ttu-id="8d035-131">Alternativ 1</span><span class="sxs-lookup"><span data-stu-id="8d035-131">Option 1</span></span> | <span data-ttu-id="8d035-132">Alternativ 2</span><span class="sxs-lookup"><span data-stu-id="8d035-132">Option 2</span></span> | <span data-ttu-id="8d035-133">Alternativ 3</span><span class="sxs-lookup"><span data-stu-id="8d035-133">Option 3</span></span> | <span data-ttu-id="8d035-134">Alternativ 4</span><span class="sxs-lookup"><span data-stu-id="8d035-134">Option 4</span></span> |
| :---    | :------: |   :---:  |   :---:  |   :---:  |
| <span data-ttu-id="8d035-135">Hämta alla funktioner som ingår i Office 365 Enterprise E4?</span><span class="sxs-lookup"><span data-stu-id="8d035-135">Get all the features included in Office 365 Enterprise E4?</span></span> | <span data-ttu-id="8d035-136">Ja</span><span class="sxs-lookup"><span data-stu-id="8d035-136">Yes</span></span> | <span data-ttu-id="8d035-137">Ja</span><span class="sxs-lookup"><span data-stu-id="8d035-137">Yes</span></span> | <span data-ttu-id="8d035-138">Ja</span><span class="sxs-lookup"><span data-stu-id="8d035-138">Yes</span></span> | <span data-ttu-id="8d035-139">Nej</span><span class="sxs-lookup"><span data-stu-id="8d035-139">No</span></span> |
| <span data-ttu-id="8d035-140">Telefonnummer som hanteras i Office 365?</span><span class="sxs-lookup"><span data-stu-id="8d035-140">Phone numbers managed in Office 365?</span></span> | <span data-ttu-id="8d035-141">Ja</span><span class="sxs-lookup"><span data-stu-id="8d035-141">Yes</span></span> | <span data-ttu-id="8d035-142">Ja</span><span class="sxs-lookup"><span data-stu-id="8d035-142">Yes</span></span> | <span data-ttu-id="8d035-143">Nej</span><span class="sxs-lookup"><span data-stu-id="8d035-143">No</span></span> | <span data-ttu-id="8d035-144">Nej</span><span class="sxs-lookup"><span data-stu-id="8d035-144">No</span></span> |
| <span data-ttu-id="8d035-145">De telefonnummer som hanteras både lokalt och i Office 365 (hybrid distribution)?</span><span class="sxs-lookup"><span data-stu-id="8d035-145">Phone numbers managed both on-premises and in Office 365 (hybrid deployment)?</span></span> | <span data-ttu-id="8d035-146">Ja</span><span class="sxs-lookup"><span data-stu-id="8d035-146">Yes</span></span> | <span data-ttu-id="8d035-147">Ja</span><span class="sxs-lookup"><span data-stu-id="8d035-147">Yes</span></span> | <span data-ttu-id="8d035-148">Nej</span><span class="sxs-lookup"><span data-stu-id="8d035-148">No</span></span> | <span data-ttu-id="8d035-149">Nej</span><span class="sxs-lookup"><span data-stu-id="8d035-149">No</span></span> |
| <span data-ttu-id="8d035-150">Alternativ för att lägga till en PSTN-röst samtals plan?</span><span class="sxs-lookup"><span data-stu-id="8d035-150">Option to add a PSTN voice calling plan?</span></span> | <span data-ttu-id="8d035-151">Ja</span><span class="sxs-lookup"><span data-stu-id="8d035-151">Yes</span></span> | <span data-ttu-id="8d035-152">Ja</span><span class="sxs-lookup"><span data-stu-id="8d035-152">Yes</span></span> | <span data-ttu-id="8d035-153">Nej</span><span class="sxs-lookup"><span data-stu-id="8d035-153">No</span></span> | <span data-ttu-id="8d035-154">Nej</span><span class="sxs-lookup"><span data-stu-id="8d035-154">No</span></span> |
| <span data-ttu-id="8d035-155">PSTN-konferens?</span><span class="sxs-lookup"><span data-stu-id="8d035-155">PSTN Conferencing?</span></span> | <span data-ttu-id="8d035-156">Ja</span><span class="sxs-lookup"><span data-stu-id="8d035-156">Yes</span></span> | <span data-ttu-id="8d035-157">Nej</span><span class="sxs-lookup"><span data-stu-id="8d035-157">No</span></span> | <span data-ttu-id="8d035-158">Nej</span><span class="sxs-lookup"><span data-stu-id="8d035-158">No</span></span> | <span data-ttu-id="8d035-159">Nej</span><span class="sxs-lookup"><span data-stu-id="8d035-159">No</span></span> |
| <span data-ttu-id="8d035-160">Avancerade verktyg för samarbete, analys och säkerhet?</span><span class="sxs-lookup"><span data-stu-id="8d035-160">Advanced tools for collaboration, analytics, and security?</span></span> | <span data-ttu-id="8d035-161">Ja</span><span class="sxs-lookup"><span data-stu-id="8d035-161">Yes</span></span> | <span data-ttu-id="8d035-162">Nej</span><span class="sxs-lookup"><span data-stu-id="8d035-162">No</span></span> | <span data-ttu-id="8d035-163">Nej</span><span class="sxs-lookup"><span data-stu-id="8d035-163">No</span></span> | <span data-ttu-id="8d035-164">Nej</span><span class="sxs-lookup"><span data-stu-id="8d035-164">No</span></span> |
| <span data-ttu-id="8d035-165">Interaktiva rapporter, instrument paneler och data visualiseringar?</span><span class="sxs-lookup"><span data-stu-id="8d035-165">Interactive reports, dashboards, and data visualizations?</span></span> | <span data-ttu-id="8d035-166">Ja</span><span class="sxs-lookup"><span data-stu-id="8d035-166">Yes</span></span> | <span data-ttu-id="8d035-167">Nej</span><span class="sxs-lookup"><span data-stu-id="8d035-167">No</span></span> | <span data-ttu-id="8d035-168">Nej</span><span class="sxs-lookup"><span data-stu-id="8d035-168">No</span></span> | <span data-ttu-id="8d035-169">Nej</span><span class="sxs-lookup"><span data-stu-id="8d035-169">No</span></span> | 
| <span data-ttu-id="8d035-170">Mer kontroll över data säkerhet och efterlevnad med inbyggda sekretess-, genomskinlighets-och raffinerade användar kontroller?</span><span class="sxs-lookup"><span data-stu-id="8d035-170">More control over data security and compliance with built-in privacy, transparency, and refined user controls?</span></span> | <span data-ttu-id="8d035-171">Ja</span><span class="sxs-lookup"><span data-stu-id="8d035-171">Yes</span></span> | <span data-ttu-id="8d035-172">Nej</span><span class="sxs-lookup"><span data-stu-id="8d035-172">No</span></span> | <span data-ttu-id="8d035-173">Nej</span><span class="sxs-lookup"><span data-stu-id="8d035-173">No</span></span> | <span data-ttu-id="8d035-174">Nej</span><span class="sxs-lookup"><span data-stu-id="8d035-174">No</span></span> | 

## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="8d035-175">Överföra kunder till nya produkt planer</span><span class="sxs-lookup"><span data-stu-id="8d035-175">Transition customers to new product plans</span></span>

<span data-ttu-id="8d035-176">Microsoft erbjuder kontinuerligt nya produkter och tjänster till våra partner.</span><span class="sxs-lookup"><span data-stu-id="8d035-176">Microsoft continuously offers new products and services to our partners.</span></span> <span data-ttu-id="8d035-177">I dessa fall kan du behöva uppgradera kunder till nya tjänster eller migrera sina prenumerationer från SKU: er som slutligen kommer att stängas av.</span><span class="sxs-lookup"><span data-stu-id="8d035-177">In these cases, you may need to upgrade customers to new services or migrate their subscriptions from SKUs that will eventually be shut down.</span></span> <span data-ttu-id="8d035-178">Migrering av kunder från tillbakadragna SKU: er till nyare kräver följande steg:</span><span class="sxs-lookup"><span data-stu-id="8d035-178">Migrating customers from retired SKUs to newer ones requires the following steps:</span></span>

-   <span data-ttu-id="8d035-179">Köp den nya prenumerationen</span><span class="sxs-lookup"><span data-stu-id="8d035-179">Purchase the new subscription</span></span>
-   <span data-ttu-id="8d035-180">Tilldela om aktuella användar licenser</span><span class="sxs-lookup"><span data-stu-id="8d035-180">Reassign current user licenses</span></span>
-   <span data-ttu-id="8d035-181">Avbryt den gamla prenumerationen</span><span class="sxs-lookup"><span data-stu-id="8d035-181">Cancel the old subscription</span></span>

<span data-ttu-id="8d035-182">Följ dessa steg om du vill migrera en kunds Office 365 Enterprise E4-prenumeration till något av alternativen i tabellen ovan.</span><span class="sxs-lookup"><span data-stu-id="8d035-182">Follow these steps to migrate a customer's Office 365 Enterprise E4 subscription to one of the options in the table above.</span></span>

### <a name="step-1---purchase-the-new-subscription"></a><span data-ttu-id="8d035-183">Steg 1 – Köp den nya prenumerationen</span><span class="sxs-lookup"><span data-stu-id="8d035-183">Step 1 - Purchase the new subscription</span></span>

1. <span data-ttu-id="8d035-184">Från menyn **partner Center** väljer du **kunder** , väljer kunden som du vill flytta och väljer sedan **Lägg till prenumerationer** .</span><span class="sxs-lookup"><span data-stu-id="8d035-184">From the **Partner Center** menu, select **Customers** , select the customer you wish to move, and then select **Add subscriptions** .</span></span>

2. <span data-ttu-id="8d035-185">Välj den prenumeration som du vill köpa från katalogen (i det här fallet ett av alternativen ovan), ange antalet licenser och välj sedan **Skicka** .</span><span class="sxs-lookup"><span data-stu-id="8d035-185">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit** .</span></span>

   <span data-ttu-id="8d035-186">Kunden bör nu ha både gamla och nya prenumerationer, den gamla Office 365 Enterprise E4-prenumerationen och den nya mål prenumerationen, till exempel alternativ 1-Office 365 Enterprise E5.</span><span class="sxs-lookup"><span data-stu-id="8d035-186">Your customer should now have both old and new subscriptions, the old Office 365 Enterprise E4 subscription and the new 'target' subscription, for example, Option 1 - Office 365 Enterprise E5.</span></span>

### <a name="step-2---reassign-the-customers-users-licenses"></a><span data-ttu-id="8d035-187">Steg 2 – tilldela om kundens användares licenser</span><span class="sxs-lookup"><span data-stu-id="8d035-187">Step 2 - Reassign the customer's users' licenses</span></span>

1. <span data-ttu-id="8d035-188">Från menyn **partner Center** väljer du **kunder** , väljer kunden som du vill flytta och väljer sedan **användare och licenser** .</span><span class="sxs-lookup"><span data-stu-id="8d035-188">From the **Partner Center** menu, select **Customers** , select the customer you wish to move, and then select **Users and licenses** .</span></span> <span data-ttu-id="8d035-189">Sidan kund användare och licenser öppnas.</span><span class="sxs-lookup"><span data-stu-id="8d035-189">The customer's Users and Licenses page opens.</span></span>

2. <span data-ttu-id="8d035-190">Om du vill tilldela användar licenser igen väljer du den användare som ska omtilldelas och väljer sedan **Hantera licenser** .</span><span class="sxs-lookup"><span data-stu-id="8d035-190">To re-assign user licenses, select the user to reassign and then select **Manage licenses** .</span></span>

3. <span data-ttu-id="8d035-191">På sidan **Hantera licenser** avmarkerar du kryss rutan **Office 365 Enterprise E4** -licens och väljer en ny service plan för den prenumeration som kunden flyttar till.</span><span class="sxs-lookup"><span data-stu-id="8d035-191">On the **Manage licenses** page, clear the **Office 365 Enterprise E4** license check box and select a new service plan for the subscription the customer is moving to.</span></span>

4. <span data-ttu-id="8d035-192">Välj **Skicka** .</span><span class="sxs-lookup"><span data-stu-id="8d035-192">Select **Submit** .</span></span> <span data-ttu-id="8d035-193">En bekräftelse sida listar de nya licens tilldelningarna.</span><span class="sxs-lookup"><span data-stu-id="8d035-193">A confirmation page lists the new license assignments.</span></span>

5. <span data-ttu-id="8d035-194">Fortsätt på samma sätt med andra kund användare som behöver omtilldela licenser.</span><span class="sxs-lookup"><span data-stu-id="8d035-194">Continue the same steps with any other customer users that need license reassignment.</span></span>

<span data-ttu-id="8d035-195">När du har flyttat användar licenserna till den nya tjänsten kan du på ett säkert sätt avbryta den tillbakadragna prenumerationen på den översta kund nivån.</span><span class="sxs-lookup"><span data-stu-id="8d035-195">After moving the user licenses to the new service, you can safely cancel the retired subscription at the top Customer level.</span></span>

### <a name="step-3---cancel-the-old-subscription"></a><span data-ttu-id="8d035-196">Steg 3 – Avbryt den gamla prenumerationen</span><span class="sxs-lookup"><span data-stu-id="8d035-196">Step 3 - Cancel the old subscription</span></span>

1. <span data-ttu-id="8d035-197">Från menyn **partner Center** väljer du **kunder** .</span><span class="sxs-lookup"><span data-stu-id="8d035-197">From the **Partner Center** menu, select **Customers** .</span></span> <span data-ttu-id="8d035-198">Välj den kund som du vill flytta och välj den prenumeration som du vill avbryta.</span><span class="sxs-lookup"><span data-stu-id="8d035-198">Select the customer you want to move, and select the subscription you want to cancel.</span></span>

2. <span data-ttu-id="8d035-199">På sidan prenumerations information anger du prenumerations statusen **pausad** .</span><span class="sxs-lookup"><span data-stu-id="8d035-199">In the subscription details page, set the subscription status to **Suspended** .</span></span>

3. <span data-ttu-id="8d035-200">Välj **Skicka** .</span><span class="sxs-lookup"><span data-stu-id="8d035-200">Select **Submit** .</span></span>

<span data-ttu-id="8d035-201">Den gamla prenumerationen har pausats och den nya prenumerationen är aktiv.</span><span class="sxs-lookup"><span data-stu-id="8d035-201">The old subscription is suspended and the new subscription is active.</span></span> <span data-ttu-id="8d035-202">Den inaktiverade prenumerationen kommer att avetableras automatiskt efter 120 dagar.</span><span class="sxs-lookup"><span data-stu-id="8d035-202">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="8d035-203">Kunden debiteras inga ytterligare kostnader för den gamla prenumerationen.</span><span class="sxs-lookup"><span data-stu-id="8d035-203">The customer incurs no additional costs for the old subscription.</span></span>



 



