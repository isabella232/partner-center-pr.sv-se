---
title: Partner intjänad kredit för hanterade tjänster
ms.topic: article
ms.date: 12/16/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Lär dig hur Microsoft partner intjänad kredit (PEC) för hanterade tjänster beräknas och betalas och hur du garanterar att du är berättigad.
author: adamyeh
ms.author: adamyeh
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 010f74164b0428a5cd6ffcde5000b52ac6a6993f
ms.sourcegitcommit: d37a3f353426e52dfbbac577b7576f9c3f6d2ddf
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 02/06/2021
ms.locfileid: "99624008"
---
# <a name="how-the-partner-earned-credit-is-calculated-and-paid"></a><span data-ttu-id="68906-103">Hur partnerintjänad kredit beräknas och betalas</span><span class="sxs-lookup"><span data-stu-id="68906-103">How the partner earned credit is calculated and paid</span></span>

<span data-ttu-id="68906-104">**Lämpliga roller**</span><span class="sxs-lookup"><span data-stu-id="68906-104">**Appropriate roles**</span></span>

- <span data-ttu-id="68906-105">Global administratör</span><span class="sxs-lookup"><span data-stu-id="68906-105">Global admin</span></span>
- <span data-ttu-id="68906-106">Användaradministratör</span><span class="sxs-lookup"><span data-stu-id="68906-106">User admin</span></span>
- <span data-ttu-id="68906-107">Administratörs agent</span><span class="sxs-lookup"><span data-stu-id="68906-107">Admin agent</span></span>
- <span data-ttu-id="68906-108">Faktureringsadministratör</span><span class="sxs-lookup"><span data-stu-id="68906-108">Billing admin</span></span>
- <span data-ttu-id="68906-109">Försäljnings agent</span><span class="sxs-lookup"><span data-stu-id="68906-109">Sales agent</span></span>

<span data-ttu-id="68906-110">Partner intjänad kredit för hanterade tjänster (PEC) känner av och fördelar partner som äger den dygnet runt IT-operativa styrning och hantering av delar av, eller hela, Azure-miljön för kunderna.</span><span class="sxs-lookup"><span data-stu-id="68906-110">Partner earned credit for managed services (PEC) recognizes and rewards partners that own the 24x7 IT operational control and management of parts of, or the entire, Azure environment of their customers.</span></span> <span data-ttu-id="68906-111">Som standard beviljas partner i CSP de nödvändiga åtkomst rättigheterna till kundens prenumeration så att de kan utföra 24 X 7 drifts hantering och kontroll över resurserna i prenumerationen.</span><span class="sxs-lookup"><span data-stu-id="68906-111">By default, in CSP, partners are granted the necessary access rights to the customer's subscription allowing them to perform 24 X 7 operational management and control of the resources on the subscription.</span></span> <span data-ttu-id="68906-112">Ytterligare sätt som kunden kan använda för att etablera åtkomst för att agera partner beskrivs i följande avsnitt.</span><span class="sxs-lookup"><span data-stu-id="68906-112">Additional ways in which customer can provision access for transacting partner is described in the following section.</span></span> <span data-ttu-id="68906-113">Det månatliga fakturabeloppet är efter av partner intjänad kredit.</span><span class="sxs-lookup"><span data-stu-id="68906-113">The monthly invoice amount is net of partner earned credit.</span></span> <span data-ttu-id="68906-114">Partner kan se PEC-information om sina månatliga rekognoseringar-filer.</span><span class="sxs-lookup"><span data-stu-id="68906-114">Partners can see the PEC details on their monthly recon file.</span></span> <span data-ttu-id="68906-115">Läs [Hantera prenumerationer och resurser i Azure-prenumerationen](azure-plan-manage.md)för ytterligare sätt som en kund kan använda för att etablera åtkomst för den inhandlande partnern.</span><span class="sxs-lookup"><span data-stu-id="68906-115">For additional ways in which a customer can provision access for the transacting partner, read [Manage subscriptions and resources under the Azure plan](azure-plan-manage.md).</span></span>

<span data-ttu-id="68906-116">Läs även [återställa administratörs behörighet för Azure CSP-prenumerationer](revoke-reinstate-csp.md)</span><span class="sxs-lookup"><span data-stu-id="68906-116">Also read [Reinstate admin privileges for Azure CSP subscriptions](revoke-reinstate-csp.md)</span></span>

## <a name="eligibility"></a><span data-ttu-id="68906-117">Behörighet</span><span class="sxs-lookup"><span data-stu-id="68906-117">Eligibility</span></span>

<span data-ttu-id="68906-118">Följande krav gäller för att få partner företaget intjänade kredit (PEC):</span><span class="sxs-lookup"><span data-stu-id="68906-118">In order to receive the partner earned credit (PEC), the following requirements apply:</span></span> 

- <span data-ttu-id="68906-119">Du måste ha ett aktivt MPN-avtal och en giltig rollbaserad åtkomst kontroll (RBAC) för att få intjänad kredit för de Azure-tillgångar som du hanterar.</span><span class="sxs-lookup"><span data-stu-id="68906-119">You must have an active MPN agreement and valid role-based access control (RBAC) role to receive earned credit for the Azure assets you manage.</span></span>

- <span data-ttu-id="68906-120">Du måste ha dygnet runt drifts kontroll och hantering av kundens Azure-resurser i CSP.</span><span class="sxs-lookup"><span data-stu-id="68906-120">You must have 24x7 operational control and management of the customer's Azure resources in CSP.</span></span> <span data-ttu-id="68906-121">Det innebär att du måste ha administratörs behörighet för kundens Azure-prenumeration, Azure-resurs grupp, Azure-resurs.</span><span class="sxs-lookup"><span data-stu-id="68906-121">This means you must have admin privileges on the customer’s Azure subscription, Azure resource group, Azure resource.</span></span> <span data-ttu-id="68906-122">Om det gäller indirekta leverantörer och deras indirekta åter försäljare är den indirekta leverantören berättigad till PEC om antingen den indirekta leverantören eller den indirekta åter försäljaren eller båda har denna operativa kontroll.</span><span class="sxs-lookup"><span data-stu-id="68906-122">In the case of indirect providers and their indirect resellers, the indirect provider will be eligible for PEC if either the indirect provider or the indirect reseller or both have this operational control.</span></span> <span data-ttu-id="68906-123">Läs mer om det här i [återställa administratörs behörigheter för Azure CSP-prenumerationer](./revoke-reinstate-csp.md).</span><span class="sxs-lookup"><span data-stu-id="68906-123">To learn more about this, see [Reinstate admin privileges for Azure CSP subscriptions](./revoke-reinstate-csp.md).</span></span>

- <span data-ttu-id="68906-124">Utöver kraven ovan gäller PEC endast för tjänster som anges i prissättningen för Azure-abonnemang, som du kan exportera från pris sidan för [Azure-prenumerationen](https://partner.microsoft.com/commerce/sales) .</span><span class="sxs-lookup"><span data-stu-id="68906-124">In addition to the requirements above, PEC is only applicable to services listed in the Azure plan consumption pricing, which you can export from the [Azure plan pricing](https://partner.microsoft.com/commerce/sales) page.</span></span>

- <span data-ttu-id="68906-125">PEC gäller **inte** för följande tjänster:</span><span class="sxs-lookup"><span data-stu-id="68906-125">PEC is **not** applicable to the following services:</span></span>
    - <span data-ttu-id="68906-126">Azure plan-reservationer</span><span class="sxs-lookup"><span data-stu-id="68906-126">Azure Plan reservations</span></span>
    - <span data-ttu-id="68906-127">Produkter från tredje part som identifieras som tredje part i kolumnen Taggar i pris för Azure plan-förbrukning</span><span class="sxs-lookup"><span data-stu-id="68906-127">Third-party products identified as Third Party in the Tags column of the Azure plan consumption price</span></span>
    - <span data-ttu-id="68906-128">Produkter i pris listan för Marketplace</span><span class="sxs-lookup"><span data-stu-id="68906-128">Products in the Marketplace price list</span></span>
    - [<span data-ttu-id="68906-129">Virtual Machines för Azure-plats</span><span class="sxs-lookup"><span data-stu-id="68906-129">Azure Spot Virtual Machines</span></span>](https://partner.microsoft.com/resources/collection/azure-spot-in-csp#/)

- <span data-ttu-id="68906-130">PEC är intjänad på Azure-resursnivå.</span><span class="sxs-lookup"><span data-stu-id="68906-130">PEC is earned down to the Azure resource level.</span></span> <span data-ttu-id="68906-131">Om du har giltig åtkomst på antingen prenumerations-eller resurs grupps nivå får du PEC genom att varje resurs som slås samman till den högre enheten.</span><span class="sxs-lookup"><span data-stu-id="68906-131">If you have valid access at either the subscription or resource group level, each resource that rolls up to the higher entity will earn PEC.</span></span>

- <span data-ttu-id="68906-132">Information om PEC finns också på sidan för [Azure Cost Management](/azure/cost-management-billing/costs/get-started-partners) .</span><span class="sxs-lookup"><span data-stu-id="68906-132">Details on PEC are also available on the [Azure Cost management](/azure/cost-management-billing/costs/get-started-partners) page.</span></span>

### <a name="calculation"></a><span data-ttu-id="68906-133">Beräkning</span><span class="sxs-lookup"><span data-stu-id="68906-133">Calculation</span></span>

<span data-ttu-id="68906-134">PEC beräknas dagligen och kan visas i den dagliga användnings filen och en månads faktura rekognoseringar-fil.</span><span class="sxs-lookup"><span data-stu-id="68906-134">PEC is calculated daily and can be viewed in the daily usage file and monthly invoice recon file.</span></span> <span data-ttu-id="68906-135">En partner (indirekt provider eller indirekt åter försäljare) måste ha åtkomst för hela dagen (dygnet runt) för att säkerställa att de får PEC.</span><span class="sxs-lookup"><span data-stu-id="68906-135">A partner (indirect provider or indirect reseller) must have access for the entire day (24x7) to ensure they earn PEC.</span></span> <span data-ttu-id="68906-136">PEC beräknas dagligen på de hanterade Azure-resurserna.</span><span class="sxs-lookup"><span data-stu-id="68906-136">PEC is calculated on a daily basis on the managed Azure assets.</span></span> <span data-ttu-id="68906-137">Partner som bevarar beständig privilegie rad åtkomst under månaden (åtkomstscope) och för alla tillgängliga resurser (åtkomstscope) kommer att få fullständig PEC.</span><span class="sxs-lookup"><span data-stu-id="68906-137">Partners retaining persistent privileged access through the month (span of access) and for all the eligible resources (scope of access) will earn full PEC.</span></span> <span data-ttu-id="68906-138">Omfångs-och span-reducering ger lägre PEC-pris för månaden.</span><span class="sxs-lookup"><span data-stu-id="68906-138">Scope and span reduction will result in lower PEC rate for the month.</span></span> <span data-ttu-id="68906-139">Dagligt klassificerad användnings fil visas dagligen på en Azure-till gång, oavsett om PEC används eller inte.</span><span class="sxs-lookup"><span data-stu-id="68906-139">Daily rated usage file shows on a daily basis on an Azure asset, whether PEC is applied or not.</span></span> <span data-ttu-id="68906-140">Partner kan också registrera aviseringar för att övervaka ändringar i beständig privilegie rad åtkomst.</span><span class="sxs-lookup"><span data-stu-id="68906-140">Partners can also enroll in alerts to monitor changes to persistent privileged access.</span></span>

## <a name="azure-cost-management"></a><span data-ttu-id="68906-141">Azure Cost Management</span><span class="sxs-lookup"><span data-stu-id="68906-141">Azure Cost Management</span></span>

<span data-ttu-id="68906-142">Azure Cost Management (ACM) med hjälp av kostnads analys kan du som partner se de kostnader som har fått fördelen med PEC.</span><span class="sxs-lookup"><span data-stu-id="68906-142">Azure Cost Management (ACM) using Cost Analysis enables you as a partner to view the costs that have received the benefit of PEC.</span></span>  

1. <span data-ttu-id="68906-143">Logga in på partner klienten i [Azure Portal](https://portal.azure.com)och välj **Cost Management + fakturering**.</span><span class="sxs-lookup"><span data-stu-id="68906-143">In the [Azure portal](https://portal.azure.com), sign into your partner tenant and select **Cost Management + Billing**.</span></span>

2. <span data-ttu-id="68906-144">Välj **kostnads hantering**</span><span class="sxs-lookup"><span data-stu-id="68906-144">Select **Cost management**</span></span>

3. <span data-ttu-id="68906-145">Välj **kostnads analys**</span><span class="sxs-lookup"><span data-stu-id="68906-145">Select **Cost Analysis**</span></span>

   <span data-ttu-id="68906-146">I vyn kostnads analys visas kostnaderna för ditt fakturerings konto för alla tjänster som köpts och förbrukas enligt de priser som du betalar för Microsoft.</span><span class="sxs-lookup"><span data-stu-id="68906-146">The Cost Analysis view will display the costs for your billing account, for all the services purchased and consumed at the prices that you pay Microsoft.</span></span>

4. <span data-ttu-id="68906-147">Välj **PartnerEarnedCreditApplied** i list rutan i ett pivot-diagram för att Visa kostnader där PEC har tillämpats.</span><span class="sxs-lookup"><span data-stu-id="68906-147">Select **PartnerEarnedCreditApplied** in the drop down on a pivot chart to see costs that have PEC applied.</span></span> <span data-ttu-id="68906-148">När **PartnerEarnedCreditApplied** -egenskapen är true, har den tillhör ande kostnaden nytta av partner intjänade kredit.</span><span class="sxs-lookup"><span data-stu-id="68906-148">When **PartnerEarnedCreditApplied** property is True, the associated cost has the benefit of the partner earned credit.</span></span> 

   <span data-ttu-id="68906-149">När PartnerEarnedCreditApplied-egenskapen har värdet false har den tillhör ande kostnaden inte uppfyllt den nödvändiga behörigheten för krediten eller så är den köpta tjänsten inte berättigad till partner intjänad kredit.</span><span class="sxs-lookup"><span data-stu-id="68906-149">When the PartnerEarnedCreditApplied property is False, the associated cost has not met the required eligibility for the credit or the service purchased is not eligible for partner earned credit.</span></span>

   >[!NOTE] 
   ><span data-ttu-id="68906-150">Normalt tar användningen av tjänster 8-24 timmar innan den visas i **Cost Management** och PEC-krediterna visas inom 48 timmar från tiden för åtkomst i Azure Cost Management.</span><span class="sxs-lookup"><span data-stu-id="68906-150">Typically, usage for services takes 8-24 hours to appear in **Cost Management** and the PEC credits will appear within 48 hours from time of access in Azure Cost Management.</span></span>

5. <span data-ttu-id="68906-151">Du kan också gruppera efter och filtrera efter, egenskapen **PartnerEarnedCreditApplied** med hjälp av **Group by och lägga till** filter funktioner för att öka detalj nivån för kostnader som har PEC och kostnader som inte har använts.</span><span class="sxs-lookup"><span data-stu-id="68906-151">You can also group by, and filter by, the **PartnerEarnedCreditApplied** property using the **Group by and Add** filter features to drill into costs that have PEC and the costs that have no PEC applied.</span></span>

## <a name="next-steps"></a><span data-ttu-id="68906-152">Nästa steg</span><span class="sxs-lookup"><span data-stu-id="68906-152">Next steps</span></span>

- [<span data-ttu-id="68906-153">Partner intjänad kredit – översikt</span><span class="sxs-lookup"><span data-stu-id="68906-153">Partner earned credit - overview</span></span>](partner-earned-credit.md)

- <span data-ttu-id="68906-154">Detaljerade exempel på intjänade kredit beräkningar för partner finns i pris listan som du kan komma åt via instrument panelen för partner Center (inloggning krävs).</span><span class="sxs-lookup"><span data-stu-id="68906-154">Detailed examples of partner earned credit calculations are located on the price list which you can reach through the Partner Center dashboard (sign-in required).</span></span>

- [<span data-ttu-id="68906-155">Flytta till Azure plan – kom igång</span><span class="sxs-lookup"><span data-stu-id="68906-155">Move to Azure plan - get started</span></span>](azure-plan-get-started.md)

- [<span data-ttu-id="68906-156">Hantera prenumerationer och resurser under Azure-planen</span><span class="sxs-lookup"><span data-stu-id="68906-156">Manage subscriptions and resources under the Azure plan</span></span>](azure-plan-manage.md)

- [<span data-ttu-id="68906-157">Återkalla eller Omtillstånd administratörs behörighet för Azure CSP-prenumerationer</span><span class="sxs-lookup"><span data-stu-id="68906-157">Revoke or re-instate admin privileges for Azure CSP subscriptions</span></span>](revoke-reinstate-csp.md)
