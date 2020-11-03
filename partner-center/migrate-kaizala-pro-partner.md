---
title: Migrera Kaizala Pro-prenumerationer till Microsoft365
description: Lär dig hur du migrerar Kaizala Pro-prenumerationer till Microsoft365-eller Office 365-versioner. Läs den här artikeln om du vill ha mer information om att överföra dina kunder.
ms.topic: article
ms.service: partner-dashboard
ms.author: sukumart
author: sukumart
ms.date: 06/01/2020
localization_priority: Normal
ms.openlocfilehash: 0807931ae95b5c7d76f4ad33708cc8014412f55f
ms.sourcegitcommit: 3c45a181ef86b3a4866e97fb50efeae8714ab3f7
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 10/19/2020
ms.locfileid: "92532032"
---
# <a name="migrate-kaizala-pro-standalone-subscriptions-to-microsoft365-or-office-365-versions"></a><span data-ttu-id="3833b-104">Migrera Kaizala Pro fristående prenumerationer till Microsoft365-eller Office 365-versioner</span><span class="sxs-lookup"><span data-stu-id="3833b-104">Migrate Kaizala Pro Standalone subscriptions to Microsoft365 or Office 365 versions</span></span>

<span data-ttu-id="3833b-105">Från och med den 1 juli 2020 avslutas Microsoft Sales of Kaizala Pro standalone service.</span><span class="sxs-lookup"><span data-stu-id="3833b-105">Effective July 1, 2020, Microsoft is ending sales of the Kaizala Pro standalone service.</span></span> <span data-ttu-id="3833b-106">Kunder kommer inte längre att kunna köpa nya Kaizala Pro-prenumerationer efter det här datumet och befintliga Kaizala Pro-prenumerationer förnyas inte automatiskt när de upphör att gälla.</span><span class="sxs-lookup"><span data-stu-id="3833b-106">Customers will no longer be able to purchase new Kaizala Pro subscriptions after this date, and existing Kaizala Pro subscriptions will not renew automatically when they expire.</span></span>

<span data-ttu-id="3833b-107">För att säkerställa kontinuitet för kunderna bör du gå över till kunder med att förfalla Kaizala Pro fristående prenumerationer till ett SKU-alternativ som stöds, som anges nedan.</span><span class="sxs-lookup"><span data-stu-id="3833b-107">To ensure continuity for customers, you should transition customers with expiring Kaizala Pro standalone subscriptions to a supported SKU option, listed below.</span></span> <span data-ttu-id="3833b-108">Vi rekommenderar att du flyttar kunder till nya prenumerationer före prenumerationens årliga slutdatum för att undvika eventuella avbrott i tjänsten för kunderna.</span><span class="sxs-lookup"><span data-stu-id="3833b-108">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span>

<span data-ttu-id="3833b-109">Om du använder API: et (topp eller partner Center) kan du identifiera prenumerationer som upphör att gälla genom att utvärdera slutdatumet för prenumerationen tillsammans med egenskapen för automatisk förnyelse inställd på falskt: `auto renew = False` .</span><span class="sxs-lookup"><span data-stu-id="3833b-109">If you use the API (either CREST or Partner Center), you can discover expiring subscriptions by evaluating the end date of the subscription along with the auto renew property set to false: `auto renew = False`.</span></span>

<span data-ttu-id="3833b-110">E4-prenumerationerna sätts till `auto renew=False` den 1 juli 2020.</span><span class="sxs-lookup"><span data-stu-id="3833b-110">The E4 subscriptions will be set to `auto renew=False` on July 1, 2020.</span></span> <span data-ttu-id="3833b-111">Du kan när som helst flytta kunder till en ny plan.</span><span class="sxs-lookup"><span data-stu-id="3833b-111">You can move customers to a new plan at any time.</span></span>

## <a name="kaizala-pro-standalone-replacement-plans"></a><span data-ttu-id="3833b-112">Kaizala Pro fristående ersättnings planer</span><span class="sxs-lookup"><span data-stu-id="3833b-112">Kaizala Pro Standalone replacement plans</span></span>

<span data-ttu-id="3833b-113">Med de nya planerna kan dina kunder dra nytta av nya funktioner och funktioner i Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="3833b-113">With the new plans, your customers can take advantage of newer features and functionality in Microsoft 365.</span></span> <span data-ttu-id="3833b-114">Pris information finns i matrisen pris lista och erbjudande lista i Partner Center.</span><span class="sxs-lookup"><span data-stu-id="3833b-114">Pricing details are found on the price list and offer list matrix in Partner Center.</span></span>

- <span data-ttu-id="3833b-115">[**Microsoft 365 för företag**](https://www.microsoft.com/microsoft-365/compare-all-microsoft-365-products?&activetab=tab:primaryr2), inklusive:</span><span class="sxs-lookup"><span data-stu-id="3833b-115">[**Microsoft 365 for Business**](https://www.microsoft.com/microsoft-365/compare-all-microsoft-365-products?&activetab=tab:primaryr2), including:</span></span>  
   - <span data-ttu-id="3833b-116">Microsoft 365 Business Basic</span><span class="sxs-lookup"><span data-stu-id="3833b-116">Microsoft 365 Business Basic</span></span>
   - <span data-ttu-id="3833b-117">Microsoft 365 Business Standard</span><span class="sxs-lookup"><span data-stu-id="3833b-117">Microsoft 365 Business Standard</span></span>
   - <span data-ttu-id="3833b-118">Microsoft 365 Business Premium</span><span class="sxs-lookup"><span data-stu-id="3833b-118">Microsoft 365 Business Premium</span></span>
    
- <span data-ttu-id="3833b-119">[**Microsoft 365 för Frontline**](https://www.microsoft.com/microsoft-365/microsoft-365-enterprise-f3?activetab=pivot:overviewtab), inklusive:</span><span class="sxs-lookup"><span data-stu-id="3833b-119">[**Microsoft 365 for Frontline**](https://www.microsoft.com/microsoft-365/microsoft-365-enterprise-f3?activetab=pivot:overviewtab), including:</span></span>
   - <span data-ttu-id="3833b-120">Microsoft 365 F3 (tidigare Microsoft 365 F1) och Office 365 F3</span><span class="sxs-lookup"><span data-stu-id="3833b-120">Microsoft 365 F3 (formerly Microsoft 365 F1) and Office 365 F3</span></span>
    
- <span data-ttu-id="3833b-121">[**Microsoft 365 för företag**](https://www.microsoft.com/microsoft-365/compare-microsoft-365-enterprise-plans), inklusive:</span><span class="sxs-lookup"><span data-stu-id="3833b-121">[**Microsoft 365 for Enterprise**](https://www.microsoft.com/microsoft-365/compare-microsoft-365-enterprise-plans), including:</span></span> 
   - <span data-ttu-id="3833b-122">Office 365 E1</span><span class="sxs-lookup"><span data-stu-id="3833b-122">Office 365 E1</span></span>
   - <span data-ttu-id="3833b-123">Microsoft 365 E3 och Office 365 E3</span><span class="sxs-lookup"><span data-stu-id="3833b-123">Microsoft 365 E3 and Office 365 E3</span></span>
   - <span data-ttu-id="3833b-124">Microsoft 365 E5 och Office 365 E5</span><span class="sxs-lookup"><span data-stu-id="3833b-124">Microsoft 365 E5 and Office 365 E5</span></span>

- <span data-ttu-id="3833b-125">[**Microsoft 365 för utbildning**](https://www.microsoft.com/education/buy-license/microsoft365), inklusive:</span><span class="sxs-lookup"><span data-stu-id="3833b-125">[**Microsoft 365 for Education**](https://www.microsoft.com/education/buy-license/microsoft365), including:</span></span> 
    - <span data-ttu-id="3833b-126">Microsoft 365 a1 och Office 365 a1</span><span class="sxs-lookup"><span data-stu-id="3833b-126">Microsoft 365 A1 and Office 365 A1</span></span>
    - <span data-ttu-id="3833b-127">Microsoft 365 a3 och Office 365 a3</span><span class="sxs-lookup"><span data-stu-id="3833b-127">Microsoft 365 A3 and Office 365 A3</span></span>
    - <span data-ttu-id="3833b-128">Microsoft 365 A5 och Office 365 A5</span><span class="sxs-lookup"><span data-stu-id="3833b-128">Microsoft 365 A5 and Office 365 A5</span></span>

## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="3833b-129">Överföra kunder till nya produkt planer</span><span class="sxs-lookup"><span data-stu-id="3833b-129">Transition customers to new product plans</span></span>

<span data-ttu-id="3833b-130">Microsoft erbjuder kontinuerligt nya produkter och tjänster till våra partner.</span><span class="sxs-lookup"><span data-stu-id="3833b-130">Microsoft continuously offers new products and services to our partners.</span></span> <span data-ttu-id="3833b-131">I dessa fall kan du behöva uppgradera kunder till nya tjänster eller migrera sina prenumerationer från SKU: er som slutligen kommer att stängas av.</span><span class="sxs-lookup"><span data-stu-id="3833b-131">In these cases, you may need to upgrade customers to new services or migrate their subscriptions from SKUs that will eventually be shut down.</span></span> <span data-ttu-id="3833b-132">Migrering av kunder från tillbakadragna SKU: er till nyare kräver följande steg:</span><span class="sxs-lookup"><span data-stu-id="3833b-132">Migrating customers from retired SKUs to newer ones requires the following steps:</span></span>

<span data-ttu-id="3833b-133">A.</span><span class="sxs-lookup"><span data-stu-id="3833b-133">A.</span></span> <span data-ttu-id="3833b-134">Köp den nya prenumerationen</span><span class="sxs-lookup"><span data-stu-id="3833b-134">Purchase the new subscription</span></span>

<span data-ttu-id="3833b-135">B.</span><span class="sxs-lookup"><span data-stu-id="3833b-135">B.</span></span> <span data-ttu-id="3833b-136">Tilldela om aktuella användar licenser</span><span class="sxs-lookup"><span data-stu-id="3833b-136">Reassign current user licenses</span></span>

<span data-ttu-id="3833b-137">C.</span><span class="sxs-lookup"><span data-stu-id="3833b-137">C.</span></span> <span data-ttu-id="3833b-138">Avbryt gammal prenumeration</span><span class="sxs-lookup"><span data-stu-id="3833b-138">Cancel old subscription</span></span>


## <a name="migrate-your-customers-to-new-plans"></a><span data-ttu-id="3833b-139">Migrera dina kunder till nya planer</span><span class="sxs-lookup"><span data-stu-id="3833b-139">Migrate your customers to new plans</span></span>

### <a name="a-purchase-the-new-subscription"></a><span data-ttu-id="3833b-140">A.</span><span class="sxs-lookup"><span data-stu-id="3833b-140">A.</span></span> <span data-ttu-id="3833b-141">Köp den nya prenumerationen</span><span class="sxs-lookup"><span data-stu-id="3833b-141">Purchase the new subscription</span></span>

1. <span data-ttu-id="3833b-142">Om du vill köpa den nya prenumerationen väljer du **kunder** från menyn **partner Center** och väljer kunden som du vill flytta. Välj sedan **Lägg till prenumerationer** .</span><span class="sxs-lookup"><span data-stu-id="3833b-142">To purchase the new subscription, from the **Partner Center** menu, select **Customers** , select the customer you want to move, and then select **Add subscriptions** .</span></span>

2. <span data-ttu-id="3833b-143">Välj den prenumeration som du vill köpa från katalogen (i det här fallet ett av alternativen ovan), ange antalet licenser och välj sedan **Skicka** .</span><span class="sxs-lookup"><span data-stu-id="3833b-143">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit** .</span></span>

<span data-ttu-id="3833b-144">Kunden bör nu ha både gamla och nya prenumerationer, den gamla fristående Kaizala Pro-prenumerationen och den nya mål prenumerationen, till exempel alternativ 1 – Office 365 Enterprise F1.</span><span class="sxs-lookup"><span data-stu-id="3833b-144">Your customer should now have both old and new subscriptions, the old Kaizala Pro Standalone subscription and the new 'target' subscription, for example, Option 1 - Office 365 Enterprise F1.</span></span>

### <a name="b-reassign-current-user-licenses"></a><span data-ttu-id="3833b-145">B.</span><span class="sxs-lookup"><span data-stu-id="3833b-145">B.</span></span> <span data-ttu-id="3833b-146">Tilldela om aktuella användar licenser</span><span class="sxs-lookup"><span data-stu-id="3833b-146">Reassign current user licenses</span></span>

1. <span data-ttu-id="3833b-147">Om du vill tilldela om kundens användares licenser går du till menyn **partner Center** och väljer **kunder** , väljer kunden som du flyttar och väljer sedan **användare och licenser** .</span><span class="sxs-lookup"><span data-stu-id="3833b-147">To reassign the customer's users' licenses, from the **Partner Center** menu, select **Customers** , select the customer you are moving, and then select **Users and licenses** .</span></span> <span data-ttu-id="3833b-148">Sidan kund användare och licenser öppnas.</span><span class="sxs-lookup"><span data-stu-id="3833b-148">The customer's Users and Licenses page opens.</span></span>

2. <span data-ttu-id="3833b-149">Om du vill omtilldela användar licensen väljer du den användare som ska omtilldelas och väljer sedan **Hantera licenser** .</span><span class="sxs-lookup"><span data-stu-id="3833b-149">To reassign user license, select the user to reassign and then select **Manage licenses** .</span></span>

3. <span data-ttu-id="3833b-150">På sidan **Hantera licenser** avmarkerar du kryss rutan Kaizala Pro standalone License och väljer en ny service plan för den prenumeration som kunden flyttar till.</span><span class="sxs-lookup"><span data-stu-id="3833b-150">On the **Manage licenses** page, clear the Kaizala Pro Standalone license check box, and select a new service plan for the subscription the customer is moving to.</span></span>

4.  <span data-ttu-id="3833b-151">Välj **Skicka** .</span><span class="sxs-lookup"><span data-stu-id="3833b-151">Select **Submit** .</span></span> <span data-ttu-id="3833b-152">En bekräftelse sida listar de nya licens tilldelningarna.</span><span class="sxs-lookup"><span data-stu-id="3833b-152">A confirmation page lists the new license assignments.</span></span> <span data-ttu-id="3833b-153">Fortsätt med samma process för andra användare som behöver licens tilldelningar.</span><span class="sxs-lookup"><span data-stu-id="3833b-153">Continue this same process for other users who need license assignments.</span></span>

### <a name="c-cancel-old-subscription"></a><span data-ttu-id="3833b-154">C.</span><span class="sxs-lookup"><span data-stu-id="3833b-154">C.</span></span> <span data-ttu-id="3833b-155">Avbryt gammal prenumeration</span><span class="sxs-lookup"><span data-stu-id="3833b-155">Cancel old subscription</span></span>

<span data-ttu-id="3833b-156">När du har flyttat användar licensen till den nya tjänsten kan du på ett säkert sätt avbryta den tillbakadragna prenumerationen på kund nivå.</span><span class="sxs-lookup"><span data-stu-id="3833b-156">After moving the user license to the new service, you can safely cancel the retired subscription at the customer level.</span></span>

1.  <span data-ttu-id="3833b-157">Från menyn **partner Center** väljer du **kunder** .</span><span class="sxs-lookup"><span data-stu-id="3833b-157">From the **Partner Center** menu, select **Customers** .</span></span> <span data-ttu-id="3833b-158">Välj den kund vars prenumeration du vill avbryta.</span><span class="sxs-lookup"><span data-stu-id="3833b-158">Select the customer whose subscription you are canceling.</span></span>

2.  <span data-ttu-id="3833b-159">På sidan prenumerations information ställer du in prenumerationen på **pausad** .</span><span class="sxs-lookup"><span data-stu-id="3833b-159">In the subscription detail page, set the subscription to **Suspended** .</span></span>

3.  <span data-ttu-id="3833b-160">Välj **Skicka** .</span><span class="sxs-lookup"><span data-stu-id="3833b-160">Select **Submit** .</span></span>

<span data-ttu-id="3833b-161">Den gamla prenumerationen har pausats och den nya prenumerationen är aktiv.</span><span class="sxs-lookup"><span data-stu-id="3833b-161">The old subscription is suspended, and the new subscription is active.</span></span> <span data-ttu-id="3833b-162">Den inaktiverade prenumerationen kommer att avetableras automatiskt efter 120 dagar.</span><span class="sxs-lookup"><span data-stu-id="3833b-162">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="3833b-163">Kunden debiteras inga ytterligare kostnader för den gamla prenumerationen.</span><span class="sxs-lookup"><span data-stu-id="3833b-163">The customer incurs no additional costs for the old subscription.</span></span>
