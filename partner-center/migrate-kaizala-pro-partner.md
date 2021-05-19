---
title: Migrera Kaizala Pro-prenumerationer till Microsoft 365
description: Lär dig hur du migrerar Kaizala Pro-prenumerationer till Microsoft 365- eller Office 365-versioner. Läs den här artikeln för mer information om hur du övergår till dina kunder.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
ms.author: sukumart
author: sukumart
ms.date: 06/01/2020
localization_priority: Normal
ms.openlocfilehash: 583e9c40bb8d161c30440f12331dc8dcbf3db417
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 05/19/2021
ms.locfileid: "110146433"
---
# <a name="migrate-kaizala-pro-standalone-subscriptions-to-microsoft-365-or-office-365-versions"></a><span data-ttu-id="c9e16-104">Migrera fristående Kaizala Pro-prenumerationer till Microsoft 365 eller Office 365-versioner</span><span class="sxs-lookup"><span data-stu-id="c9e16-104">Migrate Kaizala Pro Standalone subscriptions to Microsoft 365 or Office 365 versions</span></span>

<span data-ttu-id="c9e16-105">**Lämpliga roller:** Försäljningsagent</span><span class="sxs-lookup"><span data-stu-id="c9e16-105">**Appropriate roles**: Sales agent</span></span>

<span data-ttu-id="c9e16-106">Från och med 1 juli 2020 avslutar Microsoft försäljningen av den fristående Kaizala Pro-tjänsten.</span><span class="sxs-lookup"><span data-stu-id="c9e16-106">Effective July 1, 2020, Microsoft is ending sales of the Kaizala Pro standalone service.</span></span> <span data-ttu-id="c9e16-107">Kunder kommer inte längre att kunna köpa nya Kaizala Pro-prenumerationer efter detta datum, och befintliga Kaizala Pro-prenumerationer förnyas inte automatiskt när de upphör att gälla.</span><span class="sxs-lookup"><span data-stu-id="c9e16-107">Customers will no longer be able to purchase new Kaizala Pro subscriptions after this date, and existing Kaizala Pro subscriptions will not renew automatically when they expire.</span></span>

<span data-ttu-id="c9e16-108">För att säkerställa kontinuitet för kunder bör du övergå till att kunder med fristående Kaizala Pro-prenumerationer upphör att gälla till ett SKU-alternativ som stöds, som anges nedan.</span><span class="sxs-lookup"><span data-stu-id="c9e16-108">To ensure continuity for customers, you should transition customers with expiring Kaizala Pro standalone subscriptions to a supported SKU option, listed below.</span></span> <span data-ttu-id="c9e16-109">Vi rekommenderar att du flyttar kunder till nya prenumerationer före prenumerationens årliga slutdatum för att undvika eventuella tjänstavbrott för kunder.</span><span class="sxs-lookup"><span data-stu-id="c9e16-109">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span>

<span data-ttu-id="c9e16-110">Om du använder API:et (antingenNTINGEN ELLER Partnercenter) kan du identifiera utgående prenumerationer genom att utvärdera slutdatumet för prenumerationen tillsammans med egenskapen för automatisk förnyelse inställd på falskt: `auto renew = False` .</span><span class="sxs-lookup"><span data-stu-id="c9e16-110">If you use the API (either CREST or Partner Center), you can discover expiring subscriptions by evaluating the end date of the subscription along with the auto renew property set to false: `auto renew = False`.</span></span>

<span data-ttu-id="c9e16-111">E4-prenumerationerna anges till `auto renew=False` den 1 juli 2020.</span><span class="sxs-lookup"><span data-stu-id="c9e16-111">The E4 subscriptions will be set to `auto renew=False` on July 1, 2020.</span></span> <span data-ttu-id="c9e16-112">Du kan när som helst flytta kunder till en ny plan.</span><span class="sxs-lookup"><span data-stu-id="c9e16-112">You can move customers to a new plan at any time.</span></span>

## <a name="kaizala-pro-standalone-replacement-plans"></a><span data-ttu-id="c9e16-113">Fristående Kaizala Pro-ersättningsplaner</span><span class="sxs-lookup"><span data-stu-id="c9e16-113">Kaizala Pro Standalone replacement plans</span></span>

<span data-ttu-id="c9e16-114">Med de nya planerna kan dina kunder dra nytta av nyare funktioner och funktioner i Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="c9e16-114">With the new plans, your customers can take advantage of newer features and functionality in Microsoft 365.</span></span> <span data-ttu-id="c9e16-115">Prisinformation finns i matrisen för prislistan och erbjudandelistan i Partnercenter.</span><span class="sxs-lookup"><span data-stu-id="c9e16-115">Pricing details are found on the price list and offer list matrix in Partner Center.</span></span>

- <span data-ttu-id="c9e16-116">[**Microsoft 365 för företag**](https://www.microsoft.com/microsoft-365/compare-all-microsoft-365-products?&activetab=tab:primaryr2), inklusive:</span><span class="sxs-lookup"><span data-stu-id="c9e16-116">[**Microsoft 365 for Business**](https://www.microsoft.com/microsoft-365/compare-all-microsoft-365-products?&activetab=tab:primaryr2), including:</span></span>  
   - <span data-ttu-id="c9e16-117">Microsoft 365 Business Basic</span><span class="sxs-lookup"><span data-stu-id="c9e16-117">Microsoft 365 Business Basic</span></span>
   - <span data-ttu-id="c9e16-118">Microsoft 365 Business Standard</span><span class="sxs-lookup"><span data-stu-id="c9e16-118">Microsoft 365 Business Standard</span></span>
   - <span data-ttu-id="c9e16-119">Microsoft 365 Business Premium</span><span class="sxs-lookup"><span data-stu-id="c9e16-119">Microsoft 365 Business Premium</span></span>
    
- <span data-ttu-id="c9e16-120">[**Microsoft 365 för Frontline,**](https://www.microsoft.com/microsoft-365/microsoft-365-enterprise-f3?activetab=pivot:overviewtab)inklusive:</span><span class="sxs-lookup"><span data-stu-id="c9e16-120">[**Microsoft 365 for Frontline**](https://www.microsoft.com/microsoft-365/microsoft-365-enterprise-f3?activetab=pivot:overviewtab), including:</span></span>
   - <span data-ttu-id="c9e16-121">Microsoft 365 F3 (tidigare Microsoft 365 F1) och Office 365 F3</span><span class="sxs-lookup"><span data-stu-id="c9e16-121">Microsoft 365 F3 (formerly Microsoft 365 F1) and Office 365 F3</span></span>
    
- <span data-ttu-id="c9e16-122">[**Microsoft 365 för Enterprise**](https://www.microsoft.com/microsoft-365/compare-microsoft-365-enterprise-plans), inklusive:</span><span class="sxs-lookup"><span data-stu-id="c9e16-122">[**Microsoft 365 for Enterprise**](https://www.microsoft.com/microsoft-365/compare-microsoft-365-enterprise-plans), including:</span></span> 
   - <span data-ttu-id="c9e16-123">Office 365 E1</span><span class="sxs-lookup"><span data-stu-id="c9e16-123">Office 365 E1</span></span>
   - <span data-ttu-id="c9e16-124">Microsoft 365 E3 och Office 365 E3</span><span class="sxs-lookup"><span data-stu-id="c9e16-124">Microsoft 365 E3 and Office 365 E3</span></span>
   - <span data-ttu-id="c9e16-125">Microsoft 365 E5 och Office 365 E5</span><span class="sxs-lookup"><span data-stu-id="c9e16-125">Microsoft 365 E5 and Office 365 E5</span></span>

- <span data-ttu-id="c9e16-126">[**Microsoft 365 for Education**](https://www.microsoft.com/education/buy-license/microsoft365), inklusive:</span><span class="sxs-lookup"><span data-stu-id="c9e16-126">[**Microsoft 365 for Education**](https://www.microsoft.com/education/buy-license/microsoft365), including:</span></span> 
    - <span data-ttu-id="c9e16-127">Microsoft 365 A1 och Office 365 A1</span><span class="sxs-lookup"><span data-stu-id="c9e16-127">Microsoft 365 A1 and Office 365 A1</span></span>
    - <span data-ttu-id="c9e16-128">Microsoft 365 A3 och Office 365 A3</span><span class="sxs-lookup"><span data-stu-id="c9e16-128">Microsoft 365 A3 and Office 365 A3</span></span>
    - <span data-ttu-id="c9e16-129">Microsoft 365 A5 och Office 365 A5</span><span class="sxs-lookup"><span data-stu-id="c9e16-129">Microsoft 365 A5 and Office 365 A5</span></span>

## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="c9e16-130">Övergå kunder till nya produktplaner</span><span class="sxs-lookup"><span data-stu-id="c9e16-130">Transition customers to new product plans</span></span>

<span data-ttu-id="c9e16-131">Microsoft erbjuder kontinuerligt nya produkter och tjänster till våra partner.</span><span class="sxs-lookup"><span data-stu-id="c9e16-131">Microsoft continuously offers new products and services to our partners.</span></span> <span data-ttu-id="c9e16-132">I dessa fall kan du behöva uppgradera kunder till nya tjänster eller migrera sina prenumerationer från SKU:er som så småningom kommer att stängas av.</span><span class="sxs-lookup"><span data-stu-id="c9e16-132">In these cases, you may need to upgrade customers to new services or migrate their subscriptions from SKUs that will eventually be shut down.</span></span> <span data-ttu-id="c9e16-133">Migrering av kunder från tillbakadragna SKU:er till nyare kräver följande steg:</span><span class="sxs-lookup"><span data-stu-id="c9e16-133">Migrating customers from retired SKUs to newer ones requires the following steps:</span></span>

<span data-ttu-id="c9e16-134">A.</span><span class="sxs-lookup"><span data-stu-id="c9e16-134">A.</span></span> <span data-ttu-id="c9e16-135">Köpa den nya prenumerationen</span><span class="sxs-lookup"><span data-stu-id="c9e16-135">Purchase the new subscription</span></span>

<span data-ttu-id="c9e16-136">B.</span><span class="sxs-lookup"><span data-stu-id="c9e16-136">B.</span></span> <span data-ttu-id="c9e16-137">Tilldela om aktuella användarlicenser</span><span class="sxs-lookup"><span data-stu-id="c9e16-137">Reassign current user licenses</span></span>

<span data-ttu-id="c9e16-138">C.</span><span class="sxs-lookup"><span data-stu-id="c9e16-138">C.</span></span> <span data-ttu-id="c9e16-139">Avbryta gammal prenumeration</span><span class="sxs-lookup"><span data-stu-id="c9e16-139">Cancel old subscription</span></span>


## <a name="migrate-your-customers-to-new-plans"></a><span data-ttu-id="c9e16-140">Migrera dina kunder till nya planer</span><span class="sxs-lookup"><span data-stu-id="c9e16-140">Migrate your customers to new plans</span></span>

### <a name="a-purchase-the-new-subscription"></a><span data-ttu-id="c9e16-141">A.</span><span class="sxs-lookup"><span data-stu-id="c9e16-141">A.</span></span> <span data-ttu-id="c9e16-142">Köpa den nya prenumerationen</span><span class="sxs-lookup"><span data-stu-id="c9e16-142">Purchase the new subscription</span></span>

1. <span data-ttu-id="c9e16-143">Om du vill köpa den nya prenumerationen går du till **Menyn i Partnercenter** och väljer **Kunder,** väljer den kund som du vill flytta och väljer sedan **Lägg till prenumerationer.**</span><span class="sxs-lookup"><span data-stu-id="c9e16-143">To purchase the new subscription, from the **Partner Center** menu, select **Customers**, select the customer you want to move, and then select **Add subscriptions**.</span></span>

2. <span data-ttu-id="c9e16-144">Välj den prenumeration som du vill köpa från katalogen (i det här fallet något av alternativen ovan), ange antalet licenser och välj sedan **Skicka.**</span><span class="sxs-lookup"><span data-stu-id="c9e16-144">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span>

<span data-ttu-id="c9e16-145">Kunden bör nu ha både gamla och nya prenumerationer, den gamla fristående Kaizala Pro-prenumerationen och den nya målprenumerationen, till exempel Alternativ 1 – Office 365 Enterprise F1.</span><span class="sxs-lookup"><span data-stu-id="c9e16-145">Your customer should now have both old and new subscriptions, the old Kaizala Pro Standalone subscription and the new 'target' subscription, for example, Option 1 - Office 365 Enterprise F1.</span></span>

### <a name="b-reassign-current-user-licenses"></a><span data-ttu-id="c9e16-146">B.</span><span class="sxs-lookup"><span data-stu-id="c9e16-146">B.</span></span> <span data-ttu-id="c9e16-147">Tilldela om aktuella användarlicenser</span><span class="sxs-lookup"><span data-stu-id="c9e16-147">Reassign current user licenses</span></span>

1. <span data-ttu-id="c9e16-148">Om du vill tilldela om kundens användarlicenser går du till **Menyn i Partnercenter,** väljer **Kunder,** väljer den kund som du flyttar och väljer sedan **Användare och licenser.**</span><span class="sxs-lookup"><span data-stu-id="c9e16-148">To reassign the customer's users' licenses, from the **Partner Center** menu, select **Customers**, select the customer you are moving, and then select **Users and licenses**.</span></span> <span data-ttu-id="c9e16-149">Kundens sida Användare och licenser öppnas.</span><span class="sxs-lookup"><span data-stu-id="c9e16-149">The customer's Users and Licenses page opens.</span></span>

2. <span data-ttu-id="c9e16-150">Om du vill tilldela om användarlicensen väljer du den användare som du vill tilldela om och väljer **sedan Hantera licenser.**</span><span class="sxs-lookup"><span data-stu-id="c9e16-150">To reassign user license, select the user to reassign and then select **Manage licenses**.</span></span>

3. <span data-ttu-id="c9e16-151">På sidan **Hantera licenser** avmarkerar du kryssrutan Fristående Licens för Kaizala Pro och väljer en ny tjänstplan för prenumerationen som kunden flyttar till.</span><span class="sxs-lookup"><span data-stu-id="c9e16-151">On the **Manage licenses** page, clear the Kaizala Pro Standalone license check box, and select a new service plan for the subscription the customer is moving to.</span></span>

4.  <span data-ttu-id="c9e16-152">Välj **Skicka**.</span><span class="sxs-lookup"><span data-stu-id="c9e16-152">Select **Submit**.</span></span> <span data-ttu-id="c9e16-153">En bekräftelsesida visar de nya licenstilldelningarna.</span><span class="sxs-lookup"><span data-stu-id="c9e16-153">A confirmation page lists the new license assignments.</span></span> <span data-ttu-id="c9e16-154">Fortsätt samma process för andra användare som behöver licenstilldelningar.</span><span class="sxs-lookup"><span data-stu-id="c9e16-154">Continue this same process for other users who need license assignments.</span></span>

### <a name="c-cancel-old-subscription"></a><span data-ttu-id="c9e16-155">C.</span><span class="sxs-lookup"><span data-stu-id="c9e16-155">C.</span></span> <span data-ttu-id="c9e16-156">Avbryta gammal prenumeration</span><span class="sxs-lookup"><span data-stu-id="c9e16-156">Cancel old subscription</span></span>

<span data-ttu-id="c9e16-157">När du har flyttat användarlicensen till den nya tjänsten kan du på ett säkert sätt avbryta den tillbakadragna prenumerationen på kundnivå.</span><span class="sxs-lookup"><span data-stu-id="c9e16-157">After moving the user license to the new service, you can safely cancel the retired subscription at the customer level.</span></span>

1.  <span data-ttu-id="c9e16-158">I **menyn i Partnercenter** väljer du **Kunder.**</span><span class="sxs-lookup"><span data-stu-id="c9e16-158">From the **Partner Center** menu, select **Customers**.</span></span> <span data-ttu-id="c9e16-159">Välj den kund vars prenumeration du avbryter.</span><span class="sxs-lookup"><span data-stu-id="c9e16-159">Select the customer whose subscription you are canceling.</span></span>

2.  <span data-ttu-id="c9e16-160">På sidan med prenumerationsdetaljer ställer du in prenumerationen på **Pausat.**</span><span class="sxs-lookup"><span data-stu-id="c9e16-160">In the subscription detail page, set the subscription to **Suspended**.</span></span>

3.  <span data-ttu-id="c9e16-161">Välj **Skicka**.</span><span class="sxs-lookup"><span data-stu-id="c9e16-161">Select **Submit**.</span></span>

<span data-ttu-id="c9e16-162">Den gamla prenumerationen pausas och den nya prenumerationen är aktiv.</span><span class="sxs-lookup"><span data-stu-id="c9e16-162">The old subscription is suspended, and the new subscription is active.</span></span> <span data-ttu-id="c9e16-163">Den pausade prenumerationen avetableeras automatiskt efter 120 dagar.</span><span class="sxs-lookup"><span data-stu-id="c9e16-163">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="c9e16-164">Kunden medför inga ytterligare kostnader för den gamla prenumerationen.</span><span class="sxs-lookup"><span data-stu-id="c9e16-164">The customer incurs no additional costs for the old subscription.</span></span>
