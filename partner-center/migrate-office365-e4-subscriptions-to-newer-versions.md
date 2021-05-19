---
title: Migrera Office 365 E4-prenumerationer
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Microsoft Office 365 Enterprise E4-versionen dras tillbaka den 7 april 2017. Lär dig hur du migrerar dina kundprenumerationer till nyare versioner av Office 365.
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: f738ddace805838cdf202c23cca8535c11cbdf54
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 05/19/2021
ms.locfileid: "110151567"
---
# <a name="migrate-office-365-e4-subscriptions-to-newer-office-365-versions"></a><span data-ttu-id="6661e-104">Migrera Office 365 E4-prenumerationer till senare Office 365-versioner</span><span class="sxs-lookup"><span data-stu-id="6661e-104">Migrate Office 365 E4 subscriptions to newer Office 365 versions</span></span>

<span data-ttu-id="6661e-105">**Lämpliga roller:** Global | Administratörsbehörighet för användarhantering | Administratörsagent | Försäljningsagent</span><span class="sxs-lookup"><span data-stu-id="6661e-105">**Appropriate roles**: Global admin | User management admin | Admin agent | Sales agent</span></span>

<span data-ttu-id="6661e-106">Office 365 Enterprise E4-planen dras tillbaka från och med den 7 april 2017.</span><span class="sxs-lookup"><span data-stu-id="6661e-106">The Office 365 Enterprise E4 plan is retired, effective April 7, 2017.</span></span> <span data-ttu-id="6661e-107">Du kan inte längre köpa nya Office 365 E4-prenumerationer efter detta datum, och befintliga E4-prenumerationer förnyas inte automatiskt när de upphör att gälla.</span><span class="sxs-lookup"><span data-stu-id="6661e-107">You can no longer purchase new Office 365 E4 subscriptions after this date, and existing E4 subscriptions will not renew automatically when they expire.</span></span>

<span data-ttu-id="6661e-108">När E4-prenumerationer avslutas avbryts de.</span><span class="sxs-lookup"><span data-stu-id="6661e-108">When E4 subscriptions end, they will be canceled.</span></span> <span data-ttu-id="6661e-109">För att säkerställa kontinuitet för kunder bör du föra över kunder med utgående E4-prenumerationer till ett SKU-alternativ som stöds, som anges nedan.</span><span class="sxs-lookup"><span data-stu-id="6661e-109">To ensure continuity for customers, you should transition customers with expiring E4 subscriptions to a supported SKU option, listed below.</span></span> <span data-ttu-id="6661e-110">Vi rekommenderar att du flyttar kunder till nya prenumerationer före prenumerationens årliga slutdatum för att undvika eventuella tjänstavbrott för kunder.</span><span class="sxs-lookup"><span data-stu-id="6661e-110">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span> 

> [!NOTE]  
> <span data-ttu-id="6661e-111">Både kommersiella SKU:er och myndighets-SKU:er för Office 365 Enterprise E4 dras tillbaka.</span><span class="sxs-lookup"><span data-stu-id="6661e-111">Both Office 365 Enterprise E4 commercial and government SKUs are retired.</span></span>
 
<span data-ttu-id="6661e-112">På prenumerationens informationssida har E4-prenumerationens status ändrats till "Upphör att gälla [datum]" från "Förnyas automatiskt [datum]".</span><span class="sxs-lookup"><span data-stu-id="6661e-112">On the subscription's detail page, the E4 subscription status has changed to "Expires on [date]" from "Auto renews on [date]".</span></span> 

<span data-ttu-id="6661e-113">Om du använder API:et (antingen KANT eller Partnercenter) kan du identifiera utgående prenumerationer genom att utvärdera slutdatumet för prenumerationen tillsammans med egenskapen för automatisk förnyelse = Falskt.</span><span class="sxs-lookup"><span data-stu-id="6661e-113">If you use the API (either CREST or Partner Center), you can discover expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.</span></span> 

<span data-ttu-id="6661e-114">E4-prenumerationerna ställs in på automatisk förnyelse =Falskt den 7 april 2017.</span><span class="sxs-lookup"><span data-stu-id="6661e-114">The E4 subscriptions will be set to auto renew=False in April 7, 2017.</span></span> <span data-ttu-id="6661e-115">Du kan när som helst flytta kunder till en ny plan.</span><span class="sxs-lookup"><span data-stu-id="6661e-115">You can move customers to a new plan at any time.</span></span> 

## <a name="office-365-enterprise-e4-edition-replacement-plans"></a><span data-ttu-id="6661e-116">Ersättningsplaner för Office 365 Enterprise E4-versionen</span><span class="sxs-lookup"><span data-stu-id="6661e-116">Office 365 Enterprise E4 edition replacement plans</span></span>

<span data-ttu-id="6661e-117">Du kan välja att behålla samma funktioner med E4 eller så kan dina kunder dra nytta av nyare funktioner i Office 365 och Skype för företag – Online.</span><span class="sxs-lookup"><span data-stu-id="6661e-117">You can choose to maintain the same functionality with E4 or have your customers take advantage of newer features and functionality in Office 365 and Skype for Business Online.</span></span> <span data-ttu-id="6661e-118">Prisinformation finns i prislistan och erbjudandelistan i Partnercenter.</span><span class="sxs-lookup"><span data-stu-id="6661e-118">Pricing details are found on the price list and offer list matrix in Partner Center.</span></span> <span data-ttu-id="6661e-119">Secure Product Enterprise E3 eller Secure Productive Enterprise E5 kan ersättas med följande alternativ för Office 365 Enterprise E3 respektive Office 365 Enterprise E5.</span><span class="sxs-lookup"><span data-stu-id="6661e-119">Secure Product Enterprise E3 or Secure Productive Enterprise E5 may be substituted in the following options for Office 365 Enterprise E3 or Office 365 Enterprise E5 respectively.</span></span>

- <span data-ttu-id="6661e-120">Alternativ 1: Office 365 Enterprise E5</span><span class="sxs-lookup"><span data-stu-id="6661e-120">Option 1: Office 365 Enterprise E5</span></span>

- <span data-ttu-id="6661e-121">Alternativ 2: Office 365 Enterprise E3 + Skype för företag – Cloud PBX</span><span class="sxs-lookup"><span data-stu-id="6661e-121">Option 2: Office 365 Enterprise E3 + Skype for Business Cloud PBX</span></span>

- <span data-ttu-id="6661e-122">Alternativ 3: Office 365 Enterprise E3 + Skype för företag Plus CAL (pris- och funktionsparitet med E4)</span><span class="sxs-lookup"><span data-stu-id="6661e-122">Option 3: Office 365 Enterprise E3 + Skype for Business Plus CAL (price and functionality parity with E4)</span></span>

- <span data-ttu-id="6661e-123">Alternativ 4: Office 365 Enterprise E3</span><span class="sxs-lookup"><span data-stu-id="6661e-123">Option 4: Office 365 Enterprise E3</span></span>


| <span data-ttu-id="6661e-124">Funktion</span><span class="sxs-lookup"><span data-stu-id="6661e-124">Feature</span></span> | <span data-ttu-id="6661e-125">Alternativ 1</span><span class="sxs-lookup"><span data-stu-id="6661e-125">Option 1</span></span> | <span data-ttu-id="6661e-126">Alternativ 2</span><span class="sxs-lookup"><span data-stu-id="6661e-126">Option 2</span></span> | <span data-ttu-id="6661e-127">Alternativ 3</span><span class="sxs-lookup"><span data-stu-id="6661e-127">Option 3</span></span> | <span data-ttu-id="6661e-128">Alternativ 4</span><span class="sxs-lookup"><span data-stu-id="6661e-128">Option 4</span></span> |
| :---    | :------: |   :---:  |   :---:  |   :---:  |
| <span data-ttu-id="6661e-129">Hämta alla funktioner som ingår i Office 365 Enterprise E4?</span><span class="sxs-lookup"><span data-stu-id="6661e-129">Get all the features included in Office 365 Enterprise E4?</span></span> | <span data-ttu-id="6661e-130">Ja</span><span class="sxs-lookup"><span data-stu-id="6661e-130">Yes</span></span> | <span data-ttu-id="6661e-131">Ja</span><span class="sxs-lookup"><span data-stu-id="6661e-131">Yes</span></span> | <span data-ttu-id="6661e-132">Ja</span><span class="sxs-lookup"><span data-stu-id="6661e-132">Yes</span></span> | <span data-ttu-id="6661e-133">Nej</span><span class="sxs-lookup"><span data-stu-id="6661e-133">No</span></span> |
| <span data-ttu-id="6661e-134">Telefonnummer som hanteras i Office 365?</span><span class="sxs-lookup"><span data-stu-id="6661e-134">Phone numbers managed in Office 365?</span></span> | <span data-ttu-id="6661e-135">Ja</span><span class="sxs-lookup"><span data-stu-id="6661e-135">Yes</span></span> | <span data-ttu-id="6661e-136">Ja</span><span class="sxs-lookup"><span data-stu-id="6661e-136">Yes</span></span> | <span data-ttu-id="6661e-137">Nej</span><span class="sxs-lookup"><span data-stu-id="6661e-137">No</span></span> | <span data-ttu-id="6661e-138">Nej</span><span class="sxs-lookup"><span data-stu-id="6661e-138">No</span></span> |
| <span data-ttu-id="6661e-139">Telefonnummer som hanteras både lokalt och i Office 365 (hybriddistribution)?</span><span class="sxs-lookup"><span data-stu-id="6661e-139">Phone numbers managed both on-premises and in Office 365 (hybrid deployment)?</span></span> | <span data-ttu-id="6661e-140">Ja</span><span class="sxs-lookup"><span data-stu-id="6661e-140">Yes</span></span> | <span data-ttu-id="6661e-141">Ja</span><span class="sxs-lookup"><span data-stu-id="6661e-141">Yes</span></span> | <span data-ttu-id="6661e-142">Nej</span><span class="sxs-lookup"><span data-stu-id="6661e-142">No</span></span> | <span data-ttu-id="6661e-143">Nej</span><span class="sxs-lookup"><span data-stu-id="6661e-143">No</span></span> |
| <span data-ttu-id="6661e-144">Alternativ för att lägga till en pstn-plan för röstsamtal?</span><span class="sxs-lookup"><span data-stu-id="6661e-144">Option to add a PSTN voice calling plan?</span></span> | <span data-ttu-id="6661e-145">Ja</span><span class="sxs-lookup"><span data-stu-id="6661e-145">Yes</span></span> | <span data-ttu-id="6661e-146">Ja</span><span class="sxs-lookup"><span data-stu-id="6661e-146">Yes</span></span> | <span data-ttu-id="6661e-147">Nej</span><span class="sxs-lookup"><span data-stu-id="6661e-147">No</span></span> | <span data-ttu-id="6661e-148">Nej</span><span class="sxs-lookup"><span data-stu-id="6661e-148">No</span></span> |
| <span data-ttu-id="6661e-149">PSTN-konferens?</span><span class="sxs-lookup"><span data-stu-id="6661e-149">PSTN Conferencing?</span></span> | <span data-ttu-id="6661e-150">Ja</span><span class="sxs-lookup"><span data-stu-id="6661e-150">Yes</span></span> | <span data-ttu-id="6661e-151">Nej</span><span class="sxs-lookup"><span data-stu-id="6661e-151">No</span></span> | <span data-ttu-id="6661e-152">Nej</span><span class="sxs-lookup"><span data-stu-id="6661e-152">No</span></span> | <span data-ttu-id="6661e-153">Nej</span><span class="sxs-lookup"><span data-stu-id="6661e-153">No</span></span> |
| <span data-ttu-id="6661e-154">Avancerade verktyg för samarbete, analys och säkerhet?</span><span class="sxs-lookup"><span data-stu-id="6661e-154">Advanced tools for collaboration, analytics, and security?</span></span> | <span data-ttu-id="6661e-155">Ja</span><span class="sxs-lookup"><span data-stu-id="6661e-155">Yes</span></span> | <span data-ttu-id="6661e-156">Nej</span><span class="sxs-lookup"><span data-stu-id="6661e-156">No</span></span> | <span data-ttu-id="6661e-157">Nej</span><span class="sxs-lookup"><span data-stu-id="6661e-157">No</span></span> | <span data-ttu-id="6661e-158">Nej</span><span class="sxs-lookup"><span data-stu-id="6661e-158">No</span></span> |
| <span data-ttu-id="6661e-159">Interaktiva rapporter, instrumentpaneler och datavisualiseringar?</span><span class="sxs-lookup"><span data-stu-id="6661e-159">Interactive reports, dashboards, and data visualizations?</span></span> | <span data-ttu-id="6661e-160">Ja</span><span class="sxs-lookup"><span data-stu-id="6661e-160">Yes</span></span> | <span data-ttu-id="6661e-161">Nej</span><span class="sxs-lookup"><span data-stu-id="6661e-161">No</span></span> | <span data-ttu-id="6661e-162">Nej</span><span class="sxs-lookup"><span data-stu-id="6661e-162">No</span></span> | <span data-ttu-id="6661e-163">Nej</span><span class="sxs-lookup"><span data-stu-id="6661e-163">No</span></span> | 
| <span data-ttu-id="6661e-164">Mer kontroll över datasäkerhet och efterlevnad med inbyggd sekretess, transparens och förfinade användarkontroller?</span><span class="sxs-lookup"><span data-stu-id="6661e-164">More control over data security and compliance with built-in privacy, transparency, and refined user controls?</span></span> | <span data-ttu-id="6661e-165">Ja</span><span class="sxs-lookup"><span data-stu-id="6661e-165">Yes</span></span> | <span data-ttu-id="6661e-166">Nej</span><span class="sxs-lookup"><span data-stu-id="6661e-166">No</span></span> | <span data-ttu-id="6661e-167">Nej</span><span class="sxs-lookup"><span data-stu-id="6661e-167">No</span></span> | <span data-ttu-id="6661e-168">Nej</span><span class="sxs-lookup"><span data-stu-id="6661e-168">No</span></span> | 

## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="6661e-169">Övergå kunder till nya produktplaner</span><span class="sxs-lookup"><span data-stu-id="6661e-169">Transition customers to new product plans</span></span>

<span data-ttu-id="6661e-170">Microsoft erbjuder kontinuerligt nya produkter och tjänster till våra partner.</span><span class="sxs-lookup"><span data-stu-id="6661e-170">Microsoft continuously offers new products and services to our partners.</span></span> <span data-ttu-id="6661e-171">I dessa fall kan du behöva uppgradera kunder till nya tjänster eller migrera sina prenumerationer från SKU:er som så småningom kommer att stängas av.</span><span class="sxs-lookup"><span data-stu-id="6661e-171">In these cases, you may need to upgrade customers to new services or migrate their subscriptions from SKUs that will eventually be shut down.</span></span> <span data-ttu-id="6661e-172">Migrering av kunder från tillbakadragna SKU:er till nyare kräver följande steg:</span><span class="sxs-lookup"><span data-stu-id="6661e-172">Migrating customers from retired SKUs to newer ones requires the following steps:</span></span>

-   <span data-ttu-id="6661e-173">Köpa den nya prenumerationen</span><span class="sxs-lookup"><span data-stu-id="6661e-173">Purchase the new subscription</span></span>
-   <span data-ttu-id="6661e-174">Tilldela om aktuella användarlicenser</span><span class="sxs-lookup"><span data-stu-id="6661e-174">Reassign current user licenses</span></span>
-   <span data-ttu-id="6661e-175">Avbryta den gamla prenumerationen</span><span class="sxs-lookup"><span data-stu-id="6661e-175">Cancel the old subscription</span></span>

<span data-ttu-id="6661e-176">Följ dessa steg om du vill migrera en kunds Office 365 Enterprise E4-prenumeration till något av alternativen i tabellen ovan.</span><span class="sxs-lookup"><span data-stu-id="6661e-176">Follow these steps to migrate a customer's Office 365 Enterprise E4 subscription to one of the options in the table above.</span></span>

### <a name="step-1---purchase-the-new-subscription"></a><span data-ttu-id="6661e-177">Steg 1 – Köp den nya prenumerationen</span><span class="sxs-lookup"><span data-stu-id="6661e-177">Step 1 - Purchase the new subscription</span></span>

1. <span data-ttu-id="6661e-178">I **menyn i Partnercenter** väljer du **Kunder,** väljer den kund som du vill flytta och väljer sedan Lägg **till prenumerationer.**</span><span class="sxs-lookup"><span data-stu-id="6661e-178">From the **Partner Center** menu, select **Customers**, select the customer you wish to move, and then select **Add subscriptions**.</span></span>

2. <span data-ttu-id="6661e-179">Välj den prenumeration som du vill köpa från katalogen (i det här fallet något av alternativen ovan), ange antalet licenser och välj sedan **Skicka.**</span><span class="sxs-lookup"><span data-stu-id="6661e-179">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span>

   <span data-ttu-id="6661e-180">Kunden bör nu ha både gamla och nya prenumerationer, den gamla Office 365 Enterprise E4-prenumerationen och den nya målprenumerationen, till exempel Alternativ 1 – Office 365 Enterprise E5.</span><span class="sxs-lookup"><span data-stu-id="6661e-180">Your customer should now have both old and new subscriptions, the old Office 365 Enterprise E4 subscription and the new 'target' subscription, for example, Option 1 - Office 365 Enterprise E5.</span></span>

### <a name="step-2---reassign-the-customers-users-licenses"></a><span data-ttu-id="6661e-181">Steg 2 – Tilldela om kundens användarlicenser</span><span class="sxs-lookup"><span data-stu-id="6661e-181">Step 2 - Reassign the customer's users' licenses</span></span>

1. <span data-ttu-id="6661e-182">I **menyn i Partnercenter** väljer **du Kunder,** väljer den kund som du vill flytta och väljer sedan **Användare och licenser.**</span><span class="sxs-lookup"><span data-stu-id="6661e-182">From the **Partner Center** menu, select **Customers**, select the customer you wish to move, and then select **Users and licenses**.</span></span> <span data-ttu-id="6661e-183">Kundens sida Användare och licenser öppnas.</span><span class="sxs-lookup"><span data-stu-id="6661e-183">The customer's Users and Licenses page opens.</span></span>

2. <span data-ttu-id="6661e-184">Om du vill tilldela om användarlicenser väljer du den användare som du vill tilldela om och väljer sedan **Hantera licenser.**</span><span class="sxs-lookup"><span data-stu-id="6661e-184">To reassign user licenses, select the user to reassign and then select **Manage licenses**.</span></span>

3. <span data-ttu-id="6661e-185">På sidan **Hantera licenser** avmarkerar du kryssrutan **Office 365 Enterprise E4-licens** och väljer en ny tjänstplan för prenumerationen som kunden flyttar till.</span><span class="sxs-lookup"><span data-stu-id="6661e-185">On the **Manage licenses** page, clear the **Office 365 Enterprise E4** license check box and select a new service plan for the subscription the customer is moving to.</span></span>

4. <span data-ttu-id="6661e-186">Välj **Skicka**.</span><span class="sxs-lookup"><span data-stu-id="6661e-186">Select **Submit**.</span></span> <span data-ttu-id="6661e-187">En bekräftelsesida visar de nya licenstilldelningarna.</span><span class="sxs-lookup"><span data-stu-id="6661e-187">A confirmation page lists the new license assignments.</span></span>

5. <span data-ttu-id="6661e-188">Fortsätt på samma sätt med andra kundanvändare som behöver licensomtilldeling.</span><span class="sxs-lookup"><span data-stu-id="6661e-188">Continue the same steps with any other customer users that need license reassignment.</span></span>

<span data-ttu-id="6661e-189">När du har flyttat användarlicenserna till den nya tjänsten kan du på ett säkert sätt avbryta den tillbakadragna prenumerationen på den högsta kundnivån.</span><span class="sxs-lookup"><span data-stu-id="6661e-189">After moving the user licenses to the new service, you can safely cancel the retired subscription at the top Customer level.</span></span>

### <a name="step-3---cancel-the-old-subscription"></a><span data-ttu-id="6661e-190">Steg 3 – Avbryt den gamla prenumerationen</span><span class="sxs-lookup"><span data-stu-id="6661e-190">Step 3 - Cancel the old subscription</span></span>

1. <span data-ttu-id="6661e-191">I **menyn i Partnercenter** väljer du **Kunder.**</span><span class="sxs-lookup"><span data-stu-id="6661e-191">From the **Partner Center** menu, select **Customers**.</span></span> <span data-ttu-id="6661e-192">Välj den kund som du vill flytta och välj den prenumeration som du vill avbryta.</span><span class="sxs-lookup"><span data-stu-id="6661e-192">Select the customer you want to move, and select the subscription you want to cancel.</span></span>

2. <span data-ttu-id="6661e-193">På sidan med prenumerationsinformation anger du prenumerationsstatusen Till **Pausad.**</span><span class="sxs-lookup"><span data-stu-id="6661e-193">In the subscription details page, set the subscription status to **Suspended**.</span></span>

3. <span data-ttu-id="6661e-194">Välj **Skicka**.</span><span class="sxs-lookup"><span data-stu-id="6661e-194">Select **Submit**.</span></span>

<span data-ttu-id="6661e-195">Den gamla prenumerationen pausas och den nya prenumerationen är aktiv.</span><span class="sxs-lookup"><span data-stu-id="6661e-195">The old subscription is suspended and the new subscription is active.</span></span> <span data-ttu-id="6661e-196">Den pausade prenumerationen avetableeras automatiskt efter 120 dagar.</span><span class="sxs-lookup"><span data-stu-id="6661e-196">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="6661e-197">Kunden medför inga ytterligare kostnader för den gamla prenumerationen.</span><span class="sxs-lookup"><span data-stu-id="6661e-197">The customer incurs no additional costs for the old subscription.</span></span>



 



