---
title: Partner intjänad kredit för hanterade tjänster
ms.topic: article
ms.date: 11/30/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Lär dig hur Microsoft partner intjänad kredit (PEC) för hanterade tjänster beräknas och betalas och hur du garanterar att du är berättigad.
author: adamyeh
ms.author: adamyeh
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 97af446c4021e9785833374131eee2f08431b5fe
ms.sourcegitcommit: 4043c791402f0acebee6ede160a135e87fe92493
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 12/01/2020
ms.locfileid: "96474316"
---
# <a name="how-the-partner-earned-credit-is-calculated-and-paid"></a><span data-ttu-id="7339c-103">Hur partnerintjänad kredit beräknas och betalas</span><span class="sxs-lookup"><span data-stu-id="7339c-103">How the partner earned credit is calculated and paid</span></span>

<span data-ttu-id="7339c-104">**Lämpliga roller**</span><span class="sxs-lookup"><span data-stu-id="7339c-104">**Appropriate roles**</span></span>

- <span data-ttu-id="7339c-105">Global administratör</span><span class="sxs-lookup"><span data-stu-id="7339c-105">Global admin</span></span>
- <span data-ttu-id="7339c-106">Användaradministratör</span><span class="sxs-lookup"><span data-stu-id="7339c-106">User admin</span></span>
- <span data-ttu-id="7339c-107">Administratörs agent</span><span class="sxs-lookup"><span data-stu-id="7339c-107">Admin agent</span></span>
- <span data-ttu-id="7339c-108">Faktureringsadministratör</span><span class="sxs-lookup"><span data-stu-id="7339c-108">Billing admin</span></span>
- <span data-ttu-id="7339c-109">Försäljnings agent</span><span class="sxs-lookup"><span data-stu-id="7339c-109">Sales agent</span></span>

<span data-ttu-id="7339c-110">Partner intjänad kredit för hanterade tjänster (PEC) känner av och fördelar partner som äger den dygnet runt IT-operativa styrning och hantering av delar av, eller hela, Azure-miljön för kunderna.</span><span class="sxs-lookup"><span data-stu-id="7339c-110">Partner earned credit for managed services (PEC) recognizes and rewards partners that own the 24x7 IT operational control and management of parts of, or the entire, Azure environment of their customers.</span></span> <span data-ttu-id="7339c-111">Som standard beviljas partner i CSP de nödvändiga åtkomst rättigheterna till kundens prenumeration så att de kan utföra 24 X 7 drifts hantering och kontroll över resurserna i prenumerationen.</span><span class="sxs-lookup"><span data-stu-id="7339c-111">By default, in CSP, partners are granted the necessary access rights to the customer's subscription allowing them to perform 24 X 7 operational management and control of the resources on the subscription.</span></span> <span data-ttu-id="7339c-112">Ytterligare sätt som kunden kan använda för att etablera åtkomst för att agera partner beskrivs i följande avsnitt.</span><span class="sxs-lookup"><span data-stu-id="7339c-112">Additional ways in which customer can provision access for transacting partner is described in the following section.</span></span> <span data-ttu-id="7339c-113">Det månatliga fakturabeloppet är efter av partner intjänad kredit.</span><span class="sxs-lookup"><span data-stu-id="7339c-113">The monthly invoice amount is net of partner earned credit.</span></span> <span data-ttu-id="7339c-114">Partner kan se PEC-information om sina månatliga rekognoseringar-filer.</span><span class="sxs-lookup"><span data-stu-id="7339c-114">Partners can see the PEC details on their monthly recon file.</span></span> <span data-ttu-id="7339c-115">Läs [Hantera prenumerationer och resurser i Azure-prenumerationen](azure-plan-manage.md)för ytterligare sätt som en kund kan använda för att etablera åtkomst för den inhandlande partnern.</span><span class="sxs-lookup"><span data-stu-id="7339c-115">For additional ways in which a customer can provision access for the transacting partner, read [Manage subscriptions and resources under the Azure plan](azure-plan-manage.md).</span></span>

<span data-ttu-id="7339c-116">Läs även [återställa administratörs behörighet för Azure CSP-prenumerationer](revoke-reinstate-csp.md)</span><span class="sxs-lookup"><span data-stu-id="7339c-116">Also read [Reinstate admin privileges for Azure CSP subscriptions](revoke-reinstate-csp.md)</span></span>

## <a name="important-eligibility-and-calculation-information"></a><span data-ttu-id="7339c-117">Viktig information om berättigande och beräkningar</span><span class="sxs-lookup"><span data-stu-id="7339c-117">Important eligibility and calculation information</span></span>

- <span data-ttu-id="7339c-118">Partner bör ha ett aktivt MPN-avtal och en giltig RBAC-roll för att få intjänad kredit för de Azure-tillgångar som de hanterar.</span><span class="sxs-lookup"><span data-stu-id="7339c-118">Partner should have an active MPN agreement and valid RBAC role to receive earned credit for the Azure assets they manage.</span></span> 

- <span data-ttu-id="7339c-119">När det gäller indirekta leverantörer och deras indirekta åter försäljare är den indirekta leverantören berättigad till PEC om antingen den indirekta leverantören eller den indirekta åter försäljaren eller både har drifts kontroll och hantering av kundens Azure-resurser i CSP.</span><span class="sxs-lookup"><span data-stu-id="7339c-119">In the case of indirect providers and their indirect resellers, the indirect provider will be eligible for PEC if either the indirect provider, or the indirect reseller or both have 24x7 operational control and management of the customer's Azure resources in CSP.</span></span>

- <span data-ttu-id="7339c-120">PEC är kopplad till fakturerad (debiterbar) förbrukning av kundens Azure-egendom i CSP som hanteras av partnern.</span><span class="sxs-lookup"><span data-stu-id="7339c-120">PEC is associated to billed (chargeable) consumption of customer's Azure estate in CSP managed by the partner.</span></span> <span data-ttu-id="7339c-121">PEC görs endast tillgängligt för partner i CSP som faktureras av Microsoft (indirekt leverantör och direkt fakturerings partner).</span><span class="sxs-lookup"><span data-stu-id="7339c-121">PEC is made available only to partners in CSP billed by Microsoft (indirect provider and direct bill partner).</span></span> 

- <span data-ttu-id="7339c-122">Berättigade tjänster: partner intjänad kredit är tillämplig på tjänster som anges i **prissättningen för Azure-abonnemang** som partner kan exportera från pris sidan för [Azure-prenumerationen](https://partner.microsoft.com/commerce/sales) .</span><span class="sxs-lookup"><span data-stu-id="7339c-122">Eligible services: Partner earned credit is applicable to services listed in the **Azure plan consumption pricing** which partners can export from the [Azure plan pricing](https://partner.microsoft.com/commerce/sales) page.</span></span> 

- <span data-ttu-id="7339c-123">Ej berättigade tjänster: partner intjänad kredit är \**_inte_* _ tillämplig på följande:</span><span class="sxs-lookup"><span data-stu-id="7339c-123">Ineligible services: Partner earned credit is \**_not_* _ applicable to the following:</span></span>
    - <span data-ttu-id="7339c-124">Azure plan-reservationer</span><span class="sxs-lookup"><span data-stu-id="7339c-124">Azure Plan reservations</span></span>
    - <span data-ttu-id="7339c-125">Produkter från tredje part som identifieras som en *tredje part*\* i **kolumnen Taggar** i priset för Azure plan-förbrukning</span><span class="sxs-lookup"><span data-stu-id="7339c-125">Third-party products identified as _ *Third Party*\* in the **Tags column** of the Azure plan consumption price</span></span>    
    - <span data-ttu-id="7339c-126">Produkter i pris listan för Marketplace</span><span class="sxs-lookup"><span data-stu-id="7339c-126">Products in the Marketplace price list</span></span>
   - [<span data-ttu-id="7339c-127">Virtual Machines för Azure-plats</span><span class="sxs-lookup"><span data-stu-id="7339c-127">Azure Spot Virtual Machines</span></span>](https://partner.microsoft.com/resources/collection/azure-spot-in-csp#/)

- <span data-ttu-id="7339c-128">PEC beräknas dagligen och kan visas i den dagliga användnings filen och en månads faktura rekognoseringar-fil.</span><span class="sxs-lookup"><span data-stu-id="7339c-128">PEC is calculated daily and can be viewed in the daily usage file and monthly invoice recon file.</span></span> <span data-ttu-id="7339c-129">En partner (indirekt provider eller indirekt åter försäljare) måste ha åtkomst för hela dagen (dygnet runt) för att säkerställa att de får PEC.</span><span class="sxs-lookup"><span data-stu-id="7339c-129">A partner (indirect provider or indirect reseller) must have access for the entire day (24x7) to ensure they earn PEC.</span></span> <span data-ttu-id="7339c-130">PEC beräknas dagligen på de hanterade Azure-resurserna.</span><span class="sxs-lookup"><span data-stu-id="7339c-130">PEC is calculated on daily basis on the managed Azure assets.</span></span> <span data-ttu-id="7339c-131">Högsta PEC för en viss fakturerings period (månad) är 15%.</span><span class="sxs-lookup"><span data-stu-id="7339c-131">The maximum PEC for a given billing period (Month) is 15%.</span></span> <span data-ttu-id="7339c-132">Partner som bevarar beständig privilegie rad åtkomst under månaden (omfånget för åtkomst) och för alla berättigade resurser (åtkomstscope) får fullständig PEC på 15%.</span><span class="sxs-lookup"><span data-stu-id="7339c-132">Partners retaining persistent privileged access through the month(span of access) and for all the eligible resources (scope of access) will earn full PEC of 15%.</span></span> <span data-ttu-id="7339c-133">Omfångs-och span-reducering ger lägre PEC-pris för månaden.</span><span class="sxs-lookup"><span data-stu-id="7339c-133">Scope and span reduction will result in lower PEC rate for the month.</span></span> <span data-ttu-id="7339c-134">Dagligt klassificerad användnings fil visas på daglig basis på en Azure-till gång oavsett om PEC används eller inte.</span><span class="sxs-lookup"><span data-stu-id="7339c-134">Daily rated usage file shows on daily basis on an Azure asset whether PEC is applied or not.</span></span> <span data-ttu-id="7339c-135">Partner kan också registrera sig i aviseringar för att upptäcka om det finns ändringar i beständig privilegie rad åtkomst.</span><span class="sxs-lookup"><span data-stu-id="7339c-135">Partners can also enroll in alerts to detect if there are changes to persistent privileged access.</span></span>

- <span data-ttu-id="7339c-136">PEC är intjänad på Azure-resursnivå.</span><span class="sxs-lookup"><span data-stu-id="7339c-136">PEC is earned down to the Azure resource level.</span></span> <span data-ttu-id="7339c-137">Om partnern har giltig åtkomst till prenumerationen eller resurs grupps nivån får varje resurs som har rollen upp till den högre enheten PEC.</span><span class="sxs-lookup"><span data-stu-id="7339c-137">If the partner has valid access at the subscription, or resource group level, each resource that roles up to the higher entity will earn PEC.</span></span>  

- <span data-ttu-id="7339c-138">PEC-information kommer också att vara tillgänglig i [Azure Cost Management](/azure/cost-management-billing/costs/get-started-partners)</span><span class="sxs-lookup"><span data-stu-id="7339c-138">PEC details will also be available on [Azure Cost management](/azure/cost-management-billing/costs/get-started-partners)</span></span>

## <a name="azure-cost-management"></a><span data-ttu-id="7339c-139">Azure Cost Management</span><span class="sxs-lookup"><span data-stu-id="7339c-139">Azure Cost Management</span></span>

<span data-ttu-id="7339c-140">Azure Cost Management (ACM) med hjälp av kostnads analys kan du som partner se de kostnader som har fått fördelen med PEC.</span><span class="sxs-lookup"><span data-stu-id="7339c-140">Azure Cost Management (ACM) using Cost Analysis enables you as a partner to view the costs that have received the benefit of PEC.</span></span>  

1. <span data-ttu-id="7339c-141">Logga in på partner klienten i [Azure Portal](https://portal.azure.com)och välj **Cost Management + fakturering**.</span><span class="sxs-lookup"><span data-stu-id="7339c-141">In the [Azure portal](https://portal.azure.com), sign into your partner tenant and select **Cost Management + Billing**.</span></span>

2. <span data-ttu-id="7339c-142">Välj **kostnads hantering**</span><span class="sxs-lookup"><span data-stu-id="7339c-142">Select **Cost management**</span></span>

3. <span data-ttu-id="7339c-143">Välj **kostnads analys**</span><span class="sxs-lookup"><span data-stu-id="7339c-143">Select **Cost Analysis**</span></span>

   <span data-ttu-id="7339c-144">I vyn kostnads analys visas kostnaderna för ditt fakturerings konto för alla tjänster som köpts och förbrukas enligt de priser som du betalar för Microsoft.</span><span class="sxs-lookup"><span data-stu-id="7339c-144">The Cost Analysis view will display the costs for your billing account, for all the services purchased and consumed at the prices that you pay Microsoft.</span></span>

4. <span data-ttu-id="7339c-145">Välj **PartnerEarnedCreditApplied** i list rutan i ett pivot-diagram för att Visa kostnader där PEC har tillämpats.</span><span class="sxs-lookup"><span data-stu-id="7339c-145">Select **PartnerEarnedCreditApplied** in the drop down on a pivot chart to see costs that have PEC applied.</span></span> <span data-ttu-id="7339c-146">När **PartnerEarnedCreditApplied** -egenskapen är true, har den tillhör ande kostnaden nytta av partner intjänade kredit.</span><span class="sxs-lookup"><span data-stu-id="7339c-146">When **PartnerEarnedCreditApplied** property is True, the associated cost has the benefit of the partner earned credit.</span></span> 

<span data-ttu-id="7339c-147">När PartnerEarnedCreditApplied-egenskapen har värdet false har den tillhör ande kostnaden inte uppfyllt den nödvändiga behörigheten för krediten eller så är den köpta tjänsten inte berättigad till partner intjänad kredit.</span><span class="sxs-lookup"><span data-stu-id="7339c-147">When the PartnerEarnedCreditApplied property is False, the associated cost has not met the required eligibility for the credit or the service purchased is not eligible for partner earned credit.</span></span>

>[!NOTE] 
><span data-ttu-id="7339c-148">Normalt tar användningen av tjänster 8-24 timmar innan den visas i **Cost Management** och PEC-krediterna visas inom 48 timmar från tiden för åtkomst i Azure Cost Management.</span><span class="sxs-lookup"><span data-stu-id="7339c-148">Typically, usage for services takes 8-24 hours to appear in **Cost Management** and the PEC credits will appear within 48 hours from time of access in Azure Cost Management.</span></span>

5. <span data-ttu-id="7339c-149">Du kan också gruppera efter och filtrera efter, egenskapen **PartnerEarnedCreditApplied** med hjälp av **Group by och lägga till** filter funktioner för att öka detalj nivån för kostnader som har PEC och kostnader som inte har använts.</span><span class="sxs-lookup"><span data-stu-id="7339c-149">You can also group by, and filter by, the **PartnerEarnedCreditApplied** property using the **Group by and Add** filter features to drill into costs that have PEC and the costs that have no PEC applied.</span></span>

## <a name="next-steps"></a><span data-ttu-id="7339c-150">Nästa steg</span><span class="sxs-lookup"><span data-stu-id="7339c-150">Next steps</span></span>

- [<span data-ttu-id="7339c-151">Partner intjänad kredit – översikt</span><span class="sxs-lookup"><span data-stu-id="7339c-151">Partner earned credit - overview</span></span>](partner-earned-credit.md)

- <span data-ttu-id="7339c-152">Detaljerade exempel på intjänade kredit beräkningar för partner finns i pris listan som du kan komma åt via instrument panelen för partner Center (inloggning krävs).</span><span class="sxs-lookup"><span data-stu-id="7339c-152">Detailed examples of partner earned credit calculations are located on the price list which you can reach through the Partner Center dashboard (sign-in required).</span></span>

- [<span data-ttu-id="7339c-153">Flytta till Azure plan – kom igång</span><span class="sxs-lookup"><span data-stu-id="7339c-153">Move to Azure plan - get started</span></span>](azure-plan-get-started.md)

- [<span data-ttu-id="7339c-154">Hantera prenumerationer och resurser under Azure-planen</span><span class="sxs-lookup"><span data-stu-id="7339c-154">Manage subscriptions and resources under the Azure plan</span></span>](azure-plan-manage.md)

- [<span data-ttu-id="7339c-155">Återkalla eller Omtillstånd administratörs behörighet för Azure CSP-prenumerationer</span><span class="sxs-lookup"><span data-stu-id="7339c-155">Revoke or re-instate admin privileges for Azure CSP subscriptions</span></span>](revoke-reinstate-csp.md)
