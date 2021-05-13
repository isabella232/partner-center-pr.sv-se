---
title: Överföra En Azure-prenumeration under en Azure-plan till en annan CSP-partner
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Lär dig hur du ändrar Molnlösningsleverantör partner som är associerad med en kunds Azure-prenumerationer under en Azure-plan.
ms.custom: SEOMAY.20
ms.localizationpriority: medium
author: mckennaville
ms.author: mcville
ms.date: 07/29/2020
ms.openlocfilehash: dcacc6da51fe40c7eb05997f5409ef5fadbcf693
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 05/13/2021
ms.locfileid: "109856057"
---
# <a name="transfer-a-customers-azure-plan-subscriptions-to-a-different-partner"></a><span data-ttu-id="d0d5c-103">Överföra en kunds Azure-planprenumerationer till en annan partner</span><span class="sxs-lookup"><span data-stu-id="d0d5c-103">Transfer a customer's Azure plan subscriptions to a different partner</span></span>

<span data-ttu-id="d0d5c-104">**Lämpliga roller:** Kontoadministratörsroller | Försäljningsagent | Faktureringsagent</span><span class="sxs-lookup"><span data-stu-id="d0d5c-104">**Appropriate roles**: Account admin | Sales agent | Billing agent</span></span>

<span data-ttu-id="d0d5c-105">Den här artikeln beskriver hur en kund kan byta azure-prenumerationer under en Azure-plan från en Molnlösningsleverantör (CSP) till en annan.</span><span class="sxs-lookup"><span data-stu-id="d0d5c-105">This article describes how a customer can switch their Azure subscriptions under an Azure plan from one Cloud Solution Provider (CSP) to another.</span></span>

<span data-ttu-id="d0d5c-106">Följ dessa steg om du vill byta en kunds Azure-prenumerationer från en annan partner.</span><span class="sxs-lookup"><span data-stu-id="d0d5c-106">To switch a customer's Azure subscriptions from a different partner, follow these steps.</span></span> <span data-ttu-id="d0d5c-107">Både partnern och kunden har steg att slutföra.</span><span class="sxs-lookup"><span data-stu-id="d0d5c-107">Both the partner and the customer have steps to complete.</span></span>

>[!Note]  
><span data-ttu-id="d0d5c-108">Endast partner med en direkt faktureringsrelation med Microsoft kan komma åt övergångsverktyget.</span><span class="sxs-lookup"><span data-stu-id="d0d5c-108">Only partners with a direct billing relationship with Microsoft can access the transition tooling.</span></span> <span data-ttu-id="d0d5c-109">Indirekta återförsäljare måste samarbeta med sina indirekta leverantörer för att använda det här övergångsverktyget.</span><span class="sxs-lookup"><span data-stu-id="d0d5c-109">Indirect Resellers must work with their Indirect Providers to leverage this transition tool.</span></span>

<span data-ttu-id="d0d5c-110">Kunden måste föra en konversation med båda partnerna (aktuell och framtida) innan det här verktyget används.</span><span class="sxs-lookup"><span data-stu-id="d0d5c-110">The customer must be in conversation with both partners (current and future) prior to this tool being leveraged.</span></span> <span data-ttu-id="d0d5c-111">En offline-konversation måste vara tvungen att undvika förvirring och omsättning.</span><span class="sxs-lookup"><span data-stu-id="d0d5c-111">An offline conversation needs to be had to avoid confusion and churn.</span></span> <span data-ttu-id="d0d5c-112">Dessutom bör partner och kunder förstå dessa överväganden och förutsättningar innan en övergång påbörjas:</span><span class="sxs-lookup"><span data-stu-id="d0d5c-112">In addition, partners and customers should understand these considerations and prerequisites prior to initiating a transition:</span></span>

<span data-ttu-id="d0d5c-113">**Viktiga överväganden:**</span><span class="sxs-lookup"><span data-stu-id="d0d5c-113">**Key considerations:**</span></span>

- <span data-ttu-id="d0d5c-114">Azure-reservationer flyttas inte med prenumerationen till en framtida partner</span><span class="sxs-lookup"><span data-stu-id="d0d5c-114">Azure Reservations will not move with the subscription to future partner</span></span>
- <span data-ttu-id="d0d5c-115">CSP-priser för Azure-tjänster under den aktuella partnern kommer inte att övergå</span><span class="sxs-lookup"><span data-stu-id="d0d5c-115">CSP pricing for Azure services under current partner will not transition</span></span>  
- <span data-ttu-id="d0d5c-116">Kundens supportansvar flyttas till framtida partner</span><span class="sxs-lookup"><span data-stu-id="d0d5c-116">Support responsibilities for customer will move to future partner</span></span>
- <span data-ttu-id="d0d5c-117">Faktureringen flyttas till en framtida partner vid tidpunkten för överföringen</span><span class="sxs-lookup"><span data-stu-id="d0d5c-117">Billing and invoicing will move to future partner at time of transfer</span></span>
- <span data-ttu-id="d0d5c-118">Azure Role-Based Access Control (RBAC) påverkas inte av överföringen</span><span class="sxs-lookup"><span data-stu-id="d0d5c-118">Azure Role-Based Access Control (RBAC) is not affected by the transfer</span></span>
- <span data-ttu-id="d0d5c-119">Admin on Behalf Of (AOBO) beviljas inte som standard till den framtida partnern</span><span class="sxs-lookup"><span data-stu-id="d0d5c-119">Admin on Behalf Of (AOBO) will not be granted by default to the future partner</span></span>
- <span data-ttu-id="d0d5c-120">Marketplace-produkter från tredje part överförs så länge produkterna klarar berättigandekontrollen för Marketplace.</span><span class="sxs-lookup"><span data-stu-id="d0d5c-120">Third-party marketplace products will transfer as long as the products pass the Marketplace eligibility check.</span></span>
    - <span data-ttu-id="d0d5c-121">Det finns inga särskilda rabatter eller regionala begränsningar</span><span class="sxs-lookup"><span data-stu-id="d0d5c-121">There are no special discounts or regional restrictions</span></span>
    - <span data-ttu-id="d0d5c-122">Produkterna är inte prenumerationsbaserade</span><span class="sxs-lookup"><span data-stu-id="d0d5c-122">The products are non-subscription based</span></span>
    - <span data-ttu-id="d0d5c-123">Den framtida partnern bör samarbeta med utgivaren för att se till att de finns på listan över tillåtna för distribution av produkten</span><span class="sxs-lookup"><span data-stu-id="d0d5c-123">The future partner should work with the publisher to make sure they are on the allow list for deployment of the product</span></span>
    - <span data-ttu-id="d0d5c-124">Om inte alla dessa villkor uppfylls för att överföra Marketplace-produkterna ska avbrytas, överförs Azure-prenumerationerna och sedan på nytt av Marketplace-produkter med den nya partnern</span><span class="sxs-lookup"><span data-stu-id="d0d5c-124">If not all of these conditions are met in order to transfer the Marketplace products should be canceled, the Azure subscriptions transferred, and then repurchase of Marketplace products with the new partner</span></span>

<span data-ttu-id="d0d5c-125">**Krav:**</span><span class="sxs-lookup"><span data-stu-id="d0d5c-125">**Prerequisites:**</span></span>

- <span data-ttu-id="d0d5c-126">Kunden engagerar den aktuella CSP-partnern om sin avsikt att övergå</span><span class="sxs-lookup"><span data-stu-id="d0d5c-126">Customer engages current CSP partner on their intent to transition</span></span>
- <span data-ttu-id="d0d5c-127">Framtida CSP-partner samarbetar med kunden för att säkerställa att kundernas behov kan uppfyllas</span><span class="sxs-lookup"><span data-stu-id="d0d5c-127">Future CSP partner works with customer to ensure customer needs can be met</span></span>
- <span data-ttu-id="d0d5c-128">En framtida CSP-partner upprättar en relation med kunden och köper en Azure-plan innan övergången börjar</span><span class="sxs-lookup"><span data-stu-id="d0d5c-128">Future CSP partner establishes a relationship with customer and purchases an Azure plan before the transition begins</span></span>  
- <span data-ttu-id="d0d5c-129">Kunden måste signera Microsoft-kundavtal med en framtida CSP-partner</span><span class="sxs-lookup"><span data-stu-id="d0d5c-129">Customer must sign Microsoft Customer Agreement with future CSP partner</span></span>
- <span data-ttu-id="d0d5c-130">En framtida CSP-partner måste ha signerat Microsoft-partneravtal att använda det här verktyget</span><span class="sxs-lookup"><span data-stu-id="d0d5c-130">Future CSP partner must have signed the Microsoft Partner Agreement to use this tool</span></span>

## <a name="customer-tasks-to-be-completed"></a><span data-ttu-id="d0d5c-131">Kunduppgifter som ska slutföras</span><span class="sxs-lookup"><span data-stu-id="d0d5c-131">Customer tasks to be completed</span></span>

<span data-ttu-id="d0d5c-132">Om du vill överföra en Azure-prenumeration under en Azure-plan måste kunden starta processen genom att kontakta sin aktuella partner.</span><span class="sxs-lookup"><span data-stu-id="d0d5c-132">To transfer an Azure subscription under an Azure plan, the customer must start the process by contacting their current partner.</span></span> <span data-ttu-id="d0d5c-133">De bör samla in den aktuella partnerns företagsnamn och domän så att deras framtida partner kan fylla i formuläret för överföringsbegäran för sin räkning.</span><span class="sxs-lookup"><span data-stu-id="d0d5c-133">They should collect their current partner's company name and domain so their future partner can complete the transfer request form on their behalf.</span></span>

<span data-ttu-id="d0d5c-134">Kunden måste också identifiera de prenumerationer som de vill överföra från den aktuella partnern.</span><span class="sxs-lookup"><span data-stu-id="d0d5c-134">The customer must also identify the subscriptions they wish to transfer from their current partner.</span></span> <span data-ttu-id="d0d5c-135">Du kan inte byta partner för Office 365-, Enterprise Mobility Suite- eller Microsoft Dynamics CRM-prenumerationer.</span><span class="sxs-lookup"><span data-stu-id="d0d5c-135">You can't change partners for Office 365, Enterprise Mobility Suite, or Microsoft Dynamics CRM subscriptions.</span></span>

>[!Note]  
><span data-ttu-id="d0d5c-136">Det är den framtida partnerns ansvar att fylla i formuläret för överföringsbegäran som initierar överföringsprocessen.</span><span class="sxs-lookup"><span data-stu-id="d0d5c-136">It is the future partner's responsibility to complete the transfer request form that initiates the transfer process.</span></span> <span data-ttu-id="d0d5c-137">Microsoft kan inte göra något åt kunden eller den aktuella partnern.</span><span class="sxs-lookup"><span data-stu-id="d0d5c-137">Microsoft cannot intervene on behalf of the customer or the current partner.</span></span> <span data-ttu-id="d0d5c-138">Kunden bör planera ett nära samarbete med sin framtida och nuvarande partner för att övergången ska gå smidigt.</span><span class="sxs-lookup"><span data-stu-id="d0d5c-138">The customer should plan to work closely with their future and current partner to make the transition go smoothly.</span></span>

## <a name="future-partner-tasks-to-be-completed"></a><span data-ttu-id="d0d5c-139">Framtida partneruppgifter som ska slutföras</span><span class="sxs-lookup"><span data-stu-id="d0d5c-139">Future partner tasks to be completed</span></span>

<span data-ttu-id="d0d5c-140">Prenumerationens framtida partner måste fylla i ett formulär för överföringsbegäran från Partnercenter för att begära en prenumerationsöverföring:</span><span class="sxs-lookup"><span data-stu-id="d0d5c-140">The future partner of the subscription needs to complete a transfer request form from Partner Center to request a subscription transfer:</span></span>

1.  <span data-ttu-id="d0d5c-141">I menyn i Partnercenter väljer du **Kunder** och väljer sedan den kund som du vill fylla i ett formulär för överföringsbegäran för.</span><span class="sxs-lookup"><span data-stu-id="d0d5c-141">From the Partner Center menu, select **Customers**, then select the customer you wish to complete a transfer request form on behalf of.</span></span>
2.  <span data-ttu-id="d0d5c-142">Välj Prenumerationer på menyn **Kund.**</span><span class="sxs-lookup"><span data-stu-id="d0d5c-142">From the Customer menu, select **Subscriptions**.</span></span>
3.  <span data-ttu-id="d0d5c-143">Välj avsnittet **Överföringsbegäran.**</span><span class="sxs-lookup"><span data-stu-id="d0d5c-143">Select the **Transfer request** section.</span></span>
4.  <span data-ttu-id="d0d5c-144">I avsnittet **Överföringsbegäran väljer** du Lägg **till ny begäran.**</span><span class="sxs-lookup"><span data-stu-id="d0d5c-144">From the **Transfer request section**, select **Add new request**.</span></span>

    :::image type="content" source="images/modernazuretransfers/Transferrequestheader.png" alt-text="Avsnittet Överföringar":::

5.  <span data-ttu-id="d0d5c-146">Fyll i **formuläret Ny överföringsbegäran.**</span><span class="sxs-lookup"><span data-stu-id="d0d5c-146">Complete the **New transfer request** form.</span></span>

6.  <span data-ttu-id="d0d5c-147">Välj **Skicka överföringsbegäran**  >  **Skicka**.</span><span class="sxs-lookup"><span data-stu-id="d0d5c-147">Select **Send transfer request** > **Send**.</span></span>

    :::image type="content" source="images/modernazuretransfers/CompleteTrnasferRequestForm.png" alt-text="Fullständigt formulär för överföringsbegäran":::

7.  <span data-ttu-id="d0d5c-149">Granska bekräftelse av överföringsbegäran</span><span class="sxs-lookup"><span data-stu-id="d0d5c-149">Review Transfer request confirmation</span></span>

    :::image type="content" source="images/modernazuretransfers/TransferPending.png" alt-text="Granska väntande överföring":::

    >[!Note]
    ><span data-ttu-id="d0d5c-151">Den framtida partnern kan avbryta  överföringsbegäran genom att välja Avbryt begäran i det övre högra hörnet endast när statusen för överföringsbegäran är "väntande".</span><span class="sxs-lookup"><span data-stu-id="d0d5c-151">The future partner can cancel the transfer request by selecting **cancel request** in the upper right-hand corner only when the transfer request status is “pending”.</span></span> <span data-ttu-id="d0d5c-152">När statusen för överföringsbegäran är "pågår" eller "klar" går det inte att avbryta.</span><span class="sxs-lookup"><span data-stu-id="d0d5c-152">Once the transfer request status is “in progress” or “complete”, cancellations will not be possible.</span></span>

## <a name="current-partner-tasks-to-be-completed"></a><span data-ttu-id="d0d5c-153">Aktuella partneruppgifter som ska slutföras</span><span class="sxs-lookup"><span data-stu-id="d0d5c-153">Current partner tasks to be completed</span></span>

<span data-ttu-id="d0d5c-154">Den aktuella partnerns administratörsagent för kunden får ett e-postmeddelande om att kunden begär överföring av sina prenumerationer:</span><span class="sxs-lookup"><span data-stu-id="d0d5c-154">The current partner's Admin Agent of the customer will receive an email that their customer is requesting a transfer of their subscriptions:</span></span>

:::image type="content" source="images/modernazuretransfers/SourceReviewEmail.png" alt-text="Genomgång":::

<span data-ttu-id="d0d5c-156">Granska och acceptera formuläret för överföringsbegäran från Partnercenter för att slutföra prenumerationsöverföringen.</span><span class="sxs-lookup"><span data-stu-id="d0d5c-156">Review and accept the transfer request form from Partner Center to complete the subscription transfer.</span></span>

>[!Note]  
><span data-ttu-id="d0d5c-157">Om ingen åtgärd vidtas av den aktuella partnern inom 30 dagar upphör begäran att gälla och den framtida partnern har en för att skapa en ny överföringsbegäran.</span><span class="sxs-lookup"><span data-stu-id="d0d5c-157">If no action is taken by the current partner within 30 days the request will expire and the future partner will have a to create a new transfer request.</span></span>

1.  <span data-ttu-id="d0d5c-158">Välj **Granska överföringsbegäran i** e-postmeddelandet ELLER</span><span class="sxs-lookup"><span data-stu-id="d0d5c-158">Select **Review transfer Request** from the email OR</span></span>
1.  <span data-ttu-id="d0d5c-159">I menyn i Partnercenter väljer **du Kunder** och väljer sedan den kund som en överföringsbegäran har skickats för.</span><span class="sxs-lookup"><span data-stu-id="d0d5c-159">From the Partner Center menu, select **Customers**, then select the customer that a transfer request has been submitted on behalf of.</span></span>
2.  <span data-ttu-id="d0d5c-160">Välj Prenumerationer på menyn **Kund.**</span><span class="sxs-lookup"><span data-stu-id="d0d5c-160">From the Customer menu, select **Subscriptions**.</span></span>
3.  <span data-ttu-id="d0d5c-161">Välj avsnittet **Överföringsbegäran.**</span><span class="sxs-lookup"><span data-stu-id="d0d5c-161">Select the **Transfer request** section.</span></span>
4.  <span data-ttu-id="d0d5c-162">Expandera överföringsinformation genom att välja det valda **ID:t för överföringsbegäran** under **Mottagna begäranden**</span><span class="sxs-lookup"><span data-stu-id="d0d5c-162">Expand transfer information by selecting the chosen **Transfer request ID** under **Received requests**</span></span>

:::image type="content" source="images/modernazuretransfers/ReviewRequest.png" alt-text="Överföringsbegäran för källgranskningar":::

5.  <span data-ttu-id="d0d5c-164">Granska överföringsbegäran.</span><span class="sxs-lookup"><span data-stu-id="d0d5c-164">Review transfer request.</span></span> <span data-ttu-id="d0d5c-165">Välj de Azure-prenumerationer som ska överföras.</span><span class="sxs-lookup"><span data-stu-id="d0d5c-165">Select the requested Azure subscriptions to transfer.</span></span>

>[!Note]  
> <span data-ttu-id="d0d5c-166">Observera följande innan du fortsätter: Du kommer inte längre att ha åtkomst till de valda prenumerationerna.</span><span class="sxs-lookup"><span data-stu-id="d0d5c-166">Before proceeding please note: You will no longer have access to the selected subscriptions.</span></span>
> <span data-ttu-id="d0d5c-167">Du faktureras inte för ytterligare användning.</span><span class="sxs-lookup"><span data-stu-id="d0d5c-167">You will not be invoiced for further usage.</span></span>
> <span data-ttu-id="d0d5c-168">Azure-reservationer överförs inte med prenumerationerna.</span><span class="sxs-lookup"><span data-stu-id="d0d5c-168">Azure reservations do not transfer with the subscriptions.</span></span>

6.  <span data-ttu-id="d0d5c-169">Välj sedan **Acceptera och överför** för att slutföra överföringsprocessen.</span><span class="sxs-lookup"><span data-stu-id="d0d5c-169">Then select **Accept and transfer** to complete the transfer process.</span></span>

:::image type="content" source="images/modernazuretransfers/SelectSubs.png" alt-text="Välj prenumerationer som ska överföras under dina Azure-planer":::

7.  <span data-ttu-id="d0d5c-171">Visa bekräftelse på överföringsgodkännande.</span><span class="sxs-lookup"><span data-stu-id="d0d5c-171">View transfer acceptance confirmation.</span></span>

   <span data-ttu-id="d0d5c-172">Nu meddelas den framtida partnern, kunden och den aktuella partnern om den accepterade överföringsbegäran via e-post.</span><span class="sxs-lookup"><span data-stu-id="d0d5c-172">At this point, the future partner, the customer, and current partner will be notified of the accepted transfer request via email.</span></span>

   <span data-ttu-id="d0d5c-173">När övergången har godkänts kan överföringsstatusen vara Väntande i upp till 15 minuter medan systemet uppdateras.</span><span class="sxs-lookup"><span data-stu-id="d0d5c-173">After, the transition has been accepted the transfer status might remain Pending for up to 15 minutes while the system is updated.</span></span> <span data-ttu-id="d0d5c-174">Om det tar längre tid fortsätter systemet att försöka i tre dagar.</span><span class="sxs-lookup"><span data-stu-id="d0d5c-174">If it takes longer, the system will keep trying for three days.</span></span> <span data-ttu-id="d0d5c-175">Om överföringsstatusen fortfarande är Väntande bör partnern skicka en tjänstbegäran.</span><span class="sxs-lookup"><span data-stu-id="d0d5c-175">If the transfer status still remains Pending, the partner should submit a service request.</span></span>

   <span data-ttu-id="d0d5c-176">När överföringen är klar visas de prenumerationer som ingår i begäran i Azure-planen för den framtida partnern och visas inte längre med dig.</span><span class="sxs-lookup"><span data-stu-id="d0d5c-176">Once the transfer is complete, the subscriptions included within the request will appear in the Azure plan of the future partner, and no longer be listed with you.</span></span>

>[!Note]  
><span data-ttu-id="d0d5c-177">För indirekta leverantörer: Informera den indirekta återförsäljaren om att överföringsbegäran har accepterats.</span><span class="sxs-lookup"><span data-stu-id="d0d5c-177">For Indirect Providers: Please inform your Indirect Reseller that the transfer request has been accepted.</span></span>

### <a name="managing-your-transferred-customer-subscriptions"></a><span data-ttu-id="d0d5c-178">Hantera dina överförda kundprenumerationer</span><span class="sxs-lookup"><span data-stu-id="d0d5c-178">Managing your transferred customer subscriptions</span></span>

- <span data-ttu-id="d0d5c-179">Åtkomst till befintliga användare, grupper eller tjänsthuvudnamn som tilldelades med hjälp av Azure RBAC (rollbaserad åtkomstkontroll) påverkas inte under övergången.</span><span class="sxs-lookup"><span data-stu-id="d0d5c-179">Access to existing users, groups, or service principals that were assigned using Azure role-based access control (RBAC) isn't affected during the transition.</span></span> <span data-ttu-id="d0d5c-180">Rollbaserad åtkomstkontroll [i Azure (Azure RBAC)](/azure/role-based-access-control/overview) hjälper kunden att hantera vem som har åtkomst till Azure-resurser, vad de kan göra med dessa resurser och vilka områden de har åtkomst till.</span><span class="sxs-lookup"><span data-stu-id="d0d5c-180">Azure role-based access control [(Azure RBAC)](/azure/role-based-access-control/overview) helps your customer manage who has access to Azure resources, what they can do with those resources, and what areas they have access to.</span></span> <span data-ttu-id="d0d5c-181">Som ny partner får du ingen RBAC-åtkomst till kundens resurser efter prenumerationsöverföringen.</span><span class="sxs-lookup"><span data-stu-id="d0d5c-181">As the new partner you aren't given any RBAC access to your customer’s resources after the subscription transfer.</span></span> <span data-ttu-id="d0d5c-182">Kundens tidigare partner behåller sin RBAC-åtkomst.</span><span class="sxs-lookup"><span data-stu-id="d0d5c-182">Your customer’s previous partner retains their RBAC access.</span></span> <span data-ttu-id="d0d5c-183">Arbeta med kunden för att förstå vem som har insyn i sina prenumerationer och hur du gör önskade ändringar.</span><span class="sxs-lookup"><span data-stu-id="d0d5c-183">Work with your customer to understand who has insight into their subscriptions and how to make any wanted changes.</span></span>

- <span data-ttu-id="d0d5c-184">Därför är det viktigt att kunden tar bort Azure RBAC-åtkomst för sin tidigare partner och lägger till åtkomst för den nya partnern.</span><span class="sxs-lookup"><span data-stu-id="d0d5c-184">Consequently, it’s important that your customer removes Azure RBAC access for their previous partner and add access for the new partner.</span></span> <span data-ttu-id="d0d5c-185">Mer information om hur kunden ger ny åtkomst finns i [Vad är rollbaserad åtkomstkontroll i Azure (Azure RBAC)?](/azure/role-based-access-control/overview)</span><span class="sxs-lookup"><span data-stu-id="d0d5c-185">For more information about your customer giving new access, see [What is Azure role-based access control (Azure RBAC)?](/azure/role-based-access-control/overview)</span></span> <span data-ttu-id="d0d5c-186">Mer information om hur kunden tar bort din tidigare partners RBAC-åtkomst finns i [Ta bort en rolltilldelning.](/azure/role-based-access-control/role-assignments-portal#remove-a-role-assignment)</span><span class="sxs-lookup"><span data-stu-id="d0d5c-186">For more information about your customer removing your previous partner’s RBAC access, see [Remove a role assignment](/azure/role-based-access-control/role-assignments-portal#remove-a-role-assignment).</span></span>

- <span data-ttu-id="d0d5c-187">Dessutom får du inte automatiskt [AOBO-åtkomst (Admin on Behalf Of)](https://channel9.msdn.com/Series/cspdev/Module-11-Admin-On-Behalf-Of-AOBO) till dina prenumerationer.</span><span class="sxs-lookup"><span data-stu-id="d0d5c-187">Additionally, you don’t automatically get [Admin on Behalf Of (AOBO)](https://channel9.msdn.com/Series/cspdev/Module-11-Admin-On-Behalf-Of-AOBO) access to your subscriptions.</span></span> <span data-ttu-id="d0d5c-188">AOBO är nödvändigt för att partner ska kunna hantera sina kunders Azure-prenumerationer åt dem.</span><span class="sxs-lookup"><span data-stu-id="d0d5c-188">AOBO is necessary for partner’s to manage their customer’s Azure subscriptions on their behalf.</span></span> <span data-ttu-id="d0d5c-189">Mer information om Azure-behörigheter finns i [Skaffa behörigheter för att hantera en kunds tjänst eller prenumeration.](./customers-revoke-admin-privileges.md)</span><span class="sxs-lookup"><span data-stu-id="d0d5c-189">For more information about Azure privileges, see [Obtain permissions to manage a customer’s service or subscription.](./customers-revoke-admin-privileges.md)</span></span>

## <a name="next-steps"></a><span data-ttu-id="d0d5c-190">Nästa steg:</span><span class="sxs-lookup"><span data-stu-id="d0d5c-190">Next steps:</span></span>

- [<span data-ttu-id="d0d5c-191">(Azure RBAC)</span><span class="sxs-lookup"><span data-stu-id="d0d5c-191">(Azure RBAC)</span></span>](/azure/role-based-access-control/overview)
- [<span data-ttu-id="d0d5c-192">Få behörighet att hantera en kunds tjänst eller prenumeration.</span><span class="sxs-lookup"><span data-stu-id="d0d5c-192">Obtain permissions to manage a customer’s service or subscription.</span></span>](./customers-revoke-admin-privileges.md)
