---
title: Överför Azure-prenumerationen under en Azure-prenumeration till en annan CSP-partner
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Lär dig hur du ändrar program partner för Cloud Solution Provider som är associerad med en kunds Azure-prenumerationer under en Azure-plan.
ms.custom: SEOMAY.20
ms.localizationpriority: medium
author: mckennaville
ms.author: mcville
ms.date: 07/29/2020
ms.openlocfilehash: 81f64e117f9e0a4abc817746d11dc9acae887577
ms.sourcegitcommit: 146964ce0cc72bd821692f73f9c0b55e6fefb0fc
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 11/10/2020
ms.locfileid: "94433355"
---
# <a name="transfer-a-customers-azure-plan-subscriptions-to-a-different-partner"></a><span data-ttu-id="6c333-103">Överföra en kunds Azure plan-prenumeration till en annan partner</span><span class="sxs-lookup"><span data-stu-id="6c333-103">Transfer a customer's Azure plan subscriptions to a different partner</span></span>

<span data-ttu-id="6c333-104">**Lämpliga roller**</span><span class="sxs-lookup"><span data-stu-id="6c333-104">**Appropriate roles**</span></span>

- <span data-ttu-id="6c333-105">Partner i CSP-programmet (Cloud Solution Provider)</span><span class="sxs-lookup"><span data-stu-id="6c333-105">Partners in the Cloud Solution Provider (CSP) program</span></span>

<span data-ttu-id="6c333-106">Den här artikeln beskriver hur en kund kan byta sina Azure-prenumerationer under en Azure-plan från en leverantör av moln lösningar till en annan.</span><span class="sxs-lookup"><span data-stu-id="6c333-106">This article describes how a customer can switch their Azure subscriptions under an Azure plan from one Cloud Solution Provider (CSP) to another.</span></span>

<span data-ttu-id="6c333-107">Följ dessa steg om du vill byta en kunds Azure-prenumeration från en annan partner.</span><span class="sxs-lookup"><span data-stu-id="6c333-107">To switch a customer's Azure subscriptions from a different partner, follow these steps.</span></span> <span data-ttu-id="6c333-108">Både partnern och kunden har steg för att slutföra.</span><span class="sxs-lookup"><span data-stu-id="6c333-108">Both the partner and the customer have steps to complete.</span></span>

>[!Note]  
><span data-ttu-id="6c333-109">Endast partner med en direkt fakturerings relation med Microsoft kan komma åt över gångs verktyget.</span><span class="sxs-lookup"><span data-stu-id="6c333-109">Only partners with a direct billing relationship with Microsoft can access the transition tooling.</span></span> <span data-ttu-id="6c333-110">Indirekta åter försäljare måste arbeta med sina indirekta leverantörer för att kunna utnyttja det här över gångs verktyget.</span><span class="sxs-lookup"><span data-stu-id="6c333-110">Indirect Resellers must work with their Indirect Providers to leverage this transition tool.</span></span>

<span data-ttu-id="6c333-111">Kunden måste vara i konversation med båda partnerna (aktuella och framtida) innan det här verktyget utnyttjas.</span><span class="sxs-lookup"><span data-stu-id="6c333-111">The customer must be in conversation with both partners (current and future) prior to this tool being leveraged.</span></span> <span data-ttu-id="6c333-112">En offline-konversation måste ha för att undvika förvirring och omsättning.</span><span class="sxs-lookup"><span data-stu-id="6c333-112">An offline conversation needs to be had to avoid confusion and churn.</span></span> <span data-ttu-id="6c333-113">Dessutom bör partner och kunder förstå dessa överväganden och krav innan en över gång påbörjas:</span><span class="sxs-lookup"><span data-stu-id="6c333-113">In addition, partners and customers should understand these considerations and prerequisites prior to initiating a transition:</span></span>

<span data-ttu-id="6c333-114">**Viktiga överväganden:**</span><span class="sxs-lookup"><span data-stu-id="6c333-114">**Key considerations:**</span></span>

- <span data-ttu-id="6c333-115">Azure Reservations kommer inte att flyttas med prenumerationen till en kommande partner</span><span class="sxs-lookup"><span data-stu-id="6c333-115">Azure Reservations will not move with the subscription to future partner</span></span>
- <span data-ttu-id="6c333-116">CSP-prissättning för Azure-tjänster under den aktuella partnern kommer inte att övergå</span><span class="sxs-lookup"><span data-stu-id="6c333-116">CSP pricing for Azure services under current partner will not transition</span></span>  
- <span data-ttu-id="6c333-117">Support ansvar för kunden kommer att gå över till en kommande partner</span><span class="sxs-lookup"><span data-stu-id="6c333-117">Support responsibilities for customer will move to future partner</span></span>
- <span data-ttu-id="6c333-118">Fakturering och fakturering flyttas till framtida partner vid överförings tillfället</span><span class="sxs-lookup"><span data-stu-id="6c333-118">Billing and invoicing will move to future partner at time of transfer</span></span>
- <span data-ttu-id="6c333-119">Azure Role-Based Access Control (RBAC) påverkas inte av överföringen</span><span class="sxs-lookup"><span data-stu-id="6c333-119">Azure Role-Based Access Control (RBAC) is not affected by the transfer</span></span>
- <span data-ttu-id="6c333-120">Admin på uppdrag av (ADMINISTRATE) beviljas inte som standard till den framtida partnern</span><span class="sxs-lookup"><span data-stu-id="6c333-120">Admin on Behalf Of (AOBO) will not be granted by default to the future partner</span></span>
- <span data-ttu-id="6c333-121">Marketplace-produkter från tredje part överförs så länge produkterna uppfyller kontroll av marknads platsens berättigande.</span><span class="sxs-lookup"><span data-stu-id="6c333-121">Third-party marketplace products will transfer as long as the products pass the Marketplace eligibility check.</span></span>
    - <span data-ttu-id="6c333-122">Det finns inga särskilda rabatter eller regionala begränsningar</span><span class="sxs-lookup"><span data-stu-id="6c333-122">There are no special discounts or regional restrictions</span></span>
    - <span data-ttu-id="6c333-123">Produkterna är icke-prenumerationer baserade</span><span class="sxs-lookup"><span data-stu-id="6c333-123">The products are non-subscription based</span></span>
    - <span data-ttu-id="6c333-124">Den framtida partnern bör arbeta med utgivaren för att se till att de finns med i listan över tillåtna program för distribution av produkten</span><span class="sxs-lookup"><span data-stu-id="6c333-124">The future partner should work with the publisher to make sure they are on the allow-list for deployment of the product</span></span>
    - <span data-ttu-id="6c333-125">Om inte alla dessa villkor uppfylls för att överföra Marketplace-produkterna bör avbrytas de Azure-prenumerationer som överförs, och sedan köpa om Marketplace-produkter med den nya partnern</span><span class="sxs-lookup"><span data-stu-id="6c333-125">If not all of these conditions are met in order to transfer the Marketplace products should be canceled, the Azure subscriptions transferred, and then repurchase of Marketplace products with the new partner</span></span>

<span data-ttu-id="6c333-126">**Krav:**</span><span class="sxs-lookup"><span data-stu-id="6c333-126">**Prerequisites:**</span></span>

- <span data-ttu-id="6c333-127">Kunden engagerar sig av den aktuella CSP-partnern i avsikt att övergå</span><span class="sxs-lookup"><span data-stu-id="6c333-127">Customer engages current CSP partner on their intent to transition</span></span>
- <span data-ttu-id="6c333-128">Framtida CSP-partner arbetar med kunden för att säkerställa att kundernas behov kan uppfyllas</span><span class="sxs-lookup"><span data-stu-id="6c333-128">Future CSP partner works with customer to ensure customer needs can be met</span></span>
- <span data-ttu-id="6c333-129">En framtida CSP-partner upprättar en relation med kunden innan över gången börjar</span><span class="sxs-lookup"><span data-stu-id="6c333-129">Future CSP partner establishes a relationship with customer before transition begins</span></span>  
- <span data-ttu-id="6c333-130">Kunden måste teckna Microsofts kund avtal med en framtida CSP-partner</span><span class="sxs-lookup"><span data-stu-id="6c333-130">Customer must sign Microsoft Customer Agreement with future CSP partner</span></span>
- <span data-ttu-id="6c333-131">Den framtida CSP-partnern måste ha undertecknat Microsoft partner Agreement för att kunna använda det här verktyget</span><span class="sxs-lookup"><span data-stu-id="6c333-131">Future CSP partner must have signed the Microsoft Partner Agreement to use this tool</span></span>

## <a name="customer-tasks-to-be-completed"></a><span data-ttu-id="6c333-132">Kund uppgifter som ska utföras</span><span class="sxs-lookup"><span data-stu-id="6c333-132">Customer tasks to be completed</span></span>

<span data-ttu-id="6c333-133">För att överföra en Azure-prenumeration under en Azure-plan måste kunden starta processen genom att kontakta den aktuella partnern.</span><span class="sxs-lookup"><span data-stu-id="6c333-133">To transfer an Azure subscription under an Azure plan, the customer must start the process by contacting their current partner.</span></span> <span data-ttu-id="6c333-134">De bör samla in sin nuvarande partner företags namn och domän så att deras framtids partner kan fylla i formuläret för överförings förfrågan för deras räkning.</span><span class="sxs-lookup"><span data-stu-id="6c333-134">They should collect their current partner's company name and domain so their future partner can complete the transfer request form on their behalf.</span></span>

<span data-ttu-id="6c333-135">Kunden måste också identifiera de prenumerationer som de vill överföra från sin aktuella partner.</span><span class="sxs-lookup"><span data-stu-id="6c333-135">The customer must also identify the subscriptions they wish to transfer from their current partner.</span></span> <span data-ttu-id="6c333-136">Du kan inte ändra partner för Office 365, Enterprise Mobility Suite eller Microsoft Dynamics CRM-prenumerationer.</span><span class="sxs-lookup"><span data-stu-id="6c333-136">You can't change partners for Office 365, Enterprise Mobility Suite, or Microsoft Dynamics CRM subscriptions.</span></span>

>[!Note]  
><span data-ttu-id="6c333-137">Det är den framtida partnerns ansvar att fylla i formuläret för överförings begäran som initierar överförings processen.</span><span class="sxs-lookup"><span data-stu-id="6c333-137">It is the future partner's responsibility to complete the transfer request form that initiates the transfer process.</span></span> <span data-ttu-id="6c333-138">Microsoft kan inte ingripa för kundens räkning eller den aktuella partnern.</span><span class="sxs-lookup"><span data-stu-id="6c333-138">Microsoft cannot intervene on behalf of the customer or the current partner.</span></span> <span data-ttu-id="6c333-139">Kunden bör planera att samar beta med sin framtida och aktuella partner för att få över gången att gå smidigt.</span><span class="sxs-lookup"><span data-stu-id="6c333-139">The customer should plan to work closely with their future and current partner to make the transition go smoothly.</span></span>

## <a name="future-partner-tasks-to-be-completed"></a><span data-ttu-id="6c333-140">Framtida partner aktiviteter som ska slutföras</span><span class="sxs-lookup"><span data-stu-id="6c333-140">Future partner tasks to be completed</span></span>

<span data-ttu-id="6c333-141">Den framtida partnern av prenumerationen måste slutföra ett överförings förfrågnings formulär från Partner Center för att begära en prenumerations överföring:</span><span class="sxs-lookup"><span data-stu-id="6c333-141">The future partner of the subscription needs to complete a transfer request form from Partner Center to request a subscription transfer:</span></span>

1.  <span data-ttu-id="6c333-142">Från menyn Partner Center väljer du **kunder** och väljer sedan den kund som du vill slutföra ett överförings förfrågnings formulär för.</span><span class="sxs-lookup"><span data-stu-id="6c333-142">From the Partner Center menu, select **Customers** , then select the customer you wish to complete a transfer request form on behalf of.</span></span>
2.  <span data-ttu-id="6c333-143">Från menyn kund väljer du **prenumerationer**.</span><span class="sxs-lookup"><span data-stu-id="6c333-143">From the Customer menu, select **Subscriptions**.</span></span>
3.  <span data-ttu-id="6c333-144">Välj avsnittet **överförings förfrågan** .</span><span class="sxs-lookup"><span data-stu-id="6c333-144">Select the **Transfer request** section.</span></span>
4.  <span data-ttu-id="6c333-145">I **avsnittet överförings förfrågan** väljer du **Lägg till ny begäran**.</span><span class="sxs-lookup"><span data-stu-id="6c333-145">From the **Transfer request section** , select **Add new request**.</span></span>

    :::image type="content" source="images/modernazuretransfers/Transferrequestheader.png" alt-text="Avsnittet överföringar":::

5.  <span data-ttu-id="6c333-147">Slutför det **nya formuläret för överförings förfrågan** .</span><span class="sxs-lookup"><span data-stu-id="6c333-147">Complete the **New transfer request** form.</span></span>

6.  <span data-ttu-id="6c333-148">Välj **skicka begäran**  >  **Skicka** överföring.</span><span class="sxs-lookup"><span data-stu-id="6c333-148">Select **Send transfer request** > **Send**.</span></span>

    :::image type="content" source="images/modernazuretransfers/CompleteTrnasferRequestForm.png" alt-text="Slutför formulär för överförings förfrågan":::

7.  <span data-ttu-id="6c333-150">Granska bekräftelse av överförings förfrågan</span><span class="sxs-lookup"><span data-stu-id="6c333-150">Review Transfer request confirmation</span></span>

    :::image type="content" source="images/modernazuretransfers/TransferPending.png" alt-text="Granska väntande överföring":::

    >[!Note]
    ><span data-ttu-id="6c333-152">Den framtida partnern kan avbryta överföringsbegäran genom att välja **Cancel Request** i det övre högra hörnet endast när status för överförings förfrågan är "väntar".</span><span class="sxs-lookup"><span data-stu-id="6c333-152">The future partner can cancel the transfer request by selecting **cancel request** in the upper right-hand corner only when the transfer request status is “pending”.</span></span> <span data-ttu-id="6c333-153">När statusen för överförings förfrågan är "pågående" eller "slutförd" går det inte att avbryta.</span><span class="sxs-lookup"><span data-stu-id="6c333-153">Once the transfer request status is “in progress” or “complete”, cancellations will not be possible.</span></span>

## <a name="current-partner-tasks-to-be-completed"></a><span data-ttu-id="6c333-154">Aktuella partner aktiviteter som ska slutföras</span><span class="sxs-lookup"><span data-stu-id="6c333-154">Current partner tasks to be completed</span></span>

<span data-ttu-id="6c333-155">Den aktuella partnerns administratörs agent för kunden får ett e-postmeddelande om att deras kund begär en överföring av sina prenumerationer:</span><span class="sxs-lookup"><span data-stu-id="6c333-155">The current partner's Admin Agent of the customer will receive an email that their customer is requesting a transfer of their subscriptions:</span></span>

:::image type="content" source="images/modernazuretransfers/SourceReviewEmail.png" alt-text="Genomgång":::

<span data-ttu-id="6c333-157">Granska och Godkänn formuläret för överförings förfrågan från Partner Center för att slutföra prenumerations överföringen.</span><span class="sxs-lookup"><span data-stu-id="6c333-157">Review and accept the transfer request form from Partner Center to complete the subscription transfer.</span></span>

>[!Note]  
><span data-ttu-id="6c333-158">Om ingen åtgärd vidtas av den aktuella partnern inom 30 dagar upphör begäran att gälla och den framtida partnern kommer att ha en för att skapa en ny överförings förfrågan.</span><span class="sxs-lookup"><span data-stu-id="6c333-158">If no action is taken by the current partner within 30 days the request will expire and the future partner will have a to create a new transfer request.</span></span>

1.  <span data-ttu-id="6c333-159">Välj **Granska överförings förfrågan** från e-postmeddelandet eller</span><span class="sxs-lookup"><span data-stu-id="6c333-159">Select **Review transfer Request** from the email OR</span></span>
1.  <span data-ttu-id="6c333-160">Från menyn Partner Center väljer du **kunder** och väljer sedan den kund som en överföringsbegäran har skickats åt för.</span><span class="sxs-lookup"><span data-stu-id="6c333-160">From the Partner Center menu, select **Customers** , then select the customer that a transfer request has been submitted on behalf of.</span></span>
2.  <span data-ttu-id="6c333-161">Från menyn kund väljer du **prenumerationer**.</span><span class="sxs-lookup"><span data-stu-id="6c333-161">From the Customer menu, select **Subscriptions**.</span></span>
3.  <span data-ttu-id="6c333-162">Välj avsnittet **överförings förfrågan** .</span><span class="sxs-lookup"><span data-stu-id="6c333-162">Select the **Transfer request** section.</span></span>
4.  <span data-ttu-id="6c333-163">Expandera överförings information genom att välja det valda **överföringsbegäran-ID: t** under **mottagna begär Anden**</span><span class="sxs-lookup"><span data-stu-id="6c333-163">Expand transfer information by selecting the chosen **Transfer request ID** under **Received requests**</span></span>

:::image type="content" source="images/modernazuretransfers/ReviewRequest.png" alt-text="Begäran om käll gransknings överföring":::

5.  <span data-ttu-id="6c333-165">Granska överförings förfrågan.</span><span class="sxs-lookup"><span data-stu-id="6c333-165">Review transfer request.</span></span> <span data-ttu-id="6c333-166">Välj de begärda Azure-prenumerationerna som ska överföras.</span><span class="sxs-lookup"><span data-stu-id="6c333-166">Select the requested Azure subscriptions to transfer.</span></span>

>[!Note]  
> <span data-ttu-id="6c333-167">Innan du fortsätter bör du tänka på följande: du kommer inte längre att ha åtkomst till de valda prenumerationerna.</span><span class="sxs-lookup"><span data-stu-id="6c333-167">Before proceeding please note: You will no longer have access to the selected subscriptions.</span></span>
> <span data-ttu-id="6c333-168">Du kommer inte att faktureras för ytterligare användning.</span><span class="sxs-lookup"><span data-stu-id="6c333-168">You will not be invoiced for further usage.</span></span>
> <span data-ttu-id="6c333-169">Azure-reservationer överförs inte med prenumerationerna.</span><span class="sxs-lookup"><span data-stu-id="6c333-169">Azure reservations do not transfer with the subscriptions.</span></span>

6.  <span data-ttu-id="6c333-170">Välj sedan **Godkänn och överför** för att slutföra överförings processen.</span><span class="sxs-lookup"><span data-stu-id="6c333-170">Then select **Accept and transfer** to complete the transfer process.</span></span>

:::image type="content" source="images/modernazuretransfers/SelectSubs.png" alt-text="Välj prenumerationer som ska överföras under dina Azure-planer":::

7.  <span data-ttu-id="6c333-172">Visa bekräftelse av godkännande av överföring.</span><span class="sxs-lookup"><span data-stu-id="6c333-172">View transfer acceptance confirmation.</span></span>

   <span data-ttu-id="6c333-173">I det här läget meddelas den framtida partnern, kunden och den aktuella partnern om den godkända överföringsbegäran via e-post.</span><span class="sxs-lookup"><span data-stu-id="6c333-173">At this point, the future partner, the customer, and current partner will be notified of the accepted transfer request via email.</span></span>

   <span data-ttu-id="6c333-174">Efter att över gången har godkänts kan överförings statusen vara väntande i upp till 15 minuter medan systemet uppdateras.</span><span class="sxs-lookup"><span data-stu-id="6c333-174">After, the transition has been accepted the transfer status might remain Pending for up to 15 minutes while the system is updated.</span></span> <span data-ttu-id="6c333-175">Om det tar längre tid fortsätter systemet att försöka i tre dagar.</span><span class="sxs-lookup"><span data-stu-id="6c333-175">If it takes longer, the system will keep trying for three days.</span></span> <span data-ttu-id="6c333-176">Om överförings statusen fortfarande är väntande bör partnern skicka en tjänstbegäran.</span><span class="sxs-lookup"><span data-stu-id="6c333-176">If the transfer status still remains Pending, the partner should submit a service request.</span></span>

   <span data-ttu-id="6c333-177">När överföringen är klar visas de prenumerationer som ingår i förfrågan i Azure-planen för den framtida partnern och visas inte längre med dig.</span><span class="sxs-lookup"><span data-stu-id="6c333-177">Once the transfer is complete, the subscriptions included within the request will appear in the Azure plan of the future partner, and no longer be listed with you.</span></span>

>[!Note]  
><span data-ttu-id="6c333-178">För indirekta leverantörer: informera din indirekta åter försäljare att överföringsbegäran har accepterats.</span><span class="sxs-lookup"><span data-stu-id="6c333-178">For Indirect Providers: Please inform your Indirect Reseller that the transfer request has been accepted.</span></span>

### <a name="managing-your-transferred-customer-subscriptions"></a><span data-ttu-id="6c333-179">Hantera dina överförda kund prenumerationer</span><span class="sxs-lookup"><span data-stu-id="6c333-179">Managing your transferred customer subscriptions</span></span>
- <span data-ttu-id="6c333-180">Åtkomst till befintliga användare, grupper eller tjänsthuvudnamn som tilldelades med hjälp av Azure RBAC (rollbaserad åtkomstkontroll) påverkas inte under övergången.</span><span class="sxs-lookup"><span data-stu-id="6c333-180">Access to existing users, groups, or service principals that were assigned using Azure role-based access control (RBAC) isn't affected during the transition.</span></span> <span data-ttu-id="6c333-181">Azure rollbaserad åtkomst kontroll [(Azure RBAC)](/azure/role-based-access-control/overview) hjälper din kund att hantera vem som har åtkomst till Azure-resurser, vad de kan göra med dessa resurser och vilka områden de har åtkomst till.</span><span class="sxs-lookup"><span data-stu-id="6c333-181">Azure role-based access control [(Azure RBAC)](/azure/role-based-access-control/overview) helps your customer manage who has access to Azure resources, what they can do with those resources, and what areas they have access to.</span></span> <span data-ttu-id="6c333-182">Som den nya partnern får du inga RBAC-åtkomst till kundens resurser efter prenumerations överföringen.</span><span class="sxs-lookup"><span data-stu-id="6c333-182">As the new partner you aren't given any RBAC access to your customer’s resources after the subscription transfer.</span></span> <span data-ttu-id="6c333-183">Din kunds tidigare partner behåller sin RBAC-åtkomst.</span><span class="sxs-lookup"><span data-stu-id="6c333-183">Your customer’s previous partner retains their RBAC access.</span></span> <span data-ttu-id="6c333-184">Arbeta med kunden för att förstå vem som har insikt i sina prenumerationer och hur du gör de ändringar som önskas.</span><span class="sxs-lookup"><span data-stu-id="6c333-184">Work with your customer to understand who has insight into their subscriptions and how to make any wanted changes.</span></span>

- <span data-ttu-id="6c333-185">Det är därför viktigt att kunden tar bort Azure RBAC-åtkomst för sin tidigare partner och lägger till åtkomst för den nya partnern.</span><span class="sxs-lookup"><span data-stu-id="6c333-185">Consequently, it’s important that your customer removes Azure RBAC access for their previous partner and add access for the new partner.</span></span> <span data-ttu-id="6c333-186">Mer information om din kund ger ny åtkomst finns i [Vad är Azures rollbaserad åtkomst kontroll (Azure RBAC)?](/azure/role-based-access-control/overview)</span><span class="sxs-lookup"><span data-stu-id="6c333-186">For more information about your customer giving new access, see [What is Azure role-based access control (Azure RBAC)?](/azure/role-based-access-control/overview)</span></span> <span data-ttu-id="6c333-187">Mer information om din kund som tar bort din tidigare partners RBAC-åtkomst finns i [ta bort en roll tilldelning](/azure/role-based-access-control/role-assignments-portal#remove-a-role-assignment).</span><span class="sxs-lookup"><span data-stu-id="6c333-187">For more information about your customer removing your previous partner’s RBAC access, see [Remove a role assignment](/azure/role-based-access-control/role-assignments-portal#remove-a-role-assignment).</span></span>

- <span data-ttu-id="6c333-188">Dessutom får du inte automatiskt [Administratörer på uppdrag av (administrate)](https://channel9.msdn.com/Series/cspdev/Module-11-Admin-On-Behalf-Of-AOBO) åtkomst till dina prenumerationer.</span><span class="sxs-lookup"><span data-stu-id="6c333-188">Additionally, you don’t automatically get [Admin on Behalf Of (AOBO)](https://channel9.msdn.com/Series/cspdev/Module-11-Admin-On-Behalf-Of-AOBO) access to your subscriptions.</span></span> <span data-ttu-id="6c333-189">ADMINISTRATE krävs för att partner ska kunna hantera sina kunders Azure-prenumerationer för deras räkning.</span><span class="sxs-lookup"><span data-stu-id="6c333-189">AOBO is necessary for partner’s to manage their customer’s Azure subscriptions on their behalf.</span></span> <span data-ttu-id="6c333-190">Mer information om Azure-behörigheter finns i [Hämta behörigheter för att hantera en kunds tjänst eller prenumeration.](./customers-revoke-admin-privileges.md)</span><span class="sxs-lookup"><span data-stu-id="6c333-190">For more information about Azure privileges, see [Obtain permissions to manage a customer’s service or subscription.](./customers-revoke-admin-privileges.md)</span></span>

## <a name="next-steps"></a><span data-ttu-id="6c333-191">Nästa steg:</span><span class="sxs-lookup"><span data-stu-id="6c333-191">Next steps:</span></span>

- [<span data-ttu-id="6c333-192">(Azure RBAC)</span><span class="sxs-lookup"><span data-stu-id="6c333-192">(Azure RBAC)</span></span>](/azure/role-based-access-control/overview)
- [<span data-ttu-id="6c333-193">Få behörighet att hantera en kunds tjänst eller prenumeration.</span><span class="sxs-lookup"><span data-stu-id="6c333-193">Obtain permissions to manage a customer’s service or subscription.</span></span>](./customers-revoke-admin-privileges.md)
