---
title: Bekräfta kundens samtycke till Microsofts kundavtal
description: Leverantörer av moln lösningar (CSP) behöver bekräfta kund godkännande av Microsofts kund avtal innan de beställer Microsoft-tjänster för kunder.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: aarzh-AaronZhang
ms.author: v-aarzh
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.date: 05/05/2020
ms.openlocfilehash: 423cf1aab281ad8e77e03aa386b43360e1b99b3c
ms.sourcegitcommit: 6b03ff400d1350db9696f9b457fcfe710310c5d3
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 12/03/2020
ms.locfileid: "96570577"
---
# <a name="confirm-customer-acceptance-of-the-microsoft-customer-agreement-in-the-csp-partner-program"></a><span data-ttu-id="f1f36-103">Bekräfta kund godkännande av Microsofts kund avtal i CSP partner-programmet</span><span class="sxs-lookup"><span data-stu-id="f1f36-103">Confirm customer acceptance of the Microsoft Customer Agreement in the CSP partner program</span></span>

<span data-ttu-id="f1f36-104">**Gäller för**</span><span class="sxs-lookup"><span data-stu-id="f1f36-104">**Applies to**</span></span>

- <span data-ttu-id="f1f36-105">Partnercenter</span><span class="sxs-lookup"><span data-stu-id="f1f36-105">Partner Center</span></span>
- <span data-ttu-id="f1f36-106">Microsoft 365 administrations Center</span><span class="sxs-lookup"><span data-stu-id="f1f36-106">Microsoft 365 Admin Center</span></span>

<span data-ttu-id="f1f36-107">**Lämpliga roller**</span><span class="sxs-lookup"><span data-stu-id="f1f36-107">**Appropriate roles**</span></span>

- <span data-ttu-id="f1f36-108">Administratörs agent</span><span class="sxs-lookup"><span data-stu-id="f1f36-108">Admin agent</span></span>
- <span data-ttu-id="f1f36-109">Försäljnings agent</span><span class="sxs-lookup"><span data-stu-id="f1f36-109">Sales agent</span></span>

<span data-ttu-id="f1f36-110">Den 1 oktober 2019 introducerade Microsoft **kund avtalet** till CSP-programmet för att ersätta Microsoft Cloud avtalet.</span><span class="sxs-lookup"><span data-stu-id="f1f36-110">On October 1, 2019, Microsoft introduced the **Microsoft Customer Agreement** to the CSP program to replace the Microsoft Cloud Agreement.</span></span> <span data-ttu-id="f1f36-111">Läs ytterligare [vägledning](indirect-reseller-tasks-in-partner-center.md) för indirekta åter försäljare.</span><span class="sxs-lookup"><span data-stu-id="f1f36-111">Read additional [guidance](indirect-reseller-tasks-in-partner-center.md) for indirect resellers.</span></span> <span data-ttu-id="f1f36-112">För att under lätta migreringen av partner till det nya avtalet, finns båda avtalen i CSP-programmet fram till den 31 januari 2020.</span><span class="sxs-lookup"><span data-stu-id="f1f36-112">To facilitate partners' migration to the new agreement, both agreements coexisted in the CSP program until January 31, 2020.</span></span> <span data-ttu-id="f1f36-113">Från och med den 1 februari 2020 ersatte Microsofts kund avtal Microsoft Cloud avtalet.</span><span class="sxs-lookup"><span data-stu-id="f1f36-113">Starting February 1, 2020, the Microsoft Customer Agreement replaced the Microsoft Cloud Agreement.</span></span>

<span data-ttu-id="f1f36-114">Kunder har två alternativ för att godkänna Microsofts kund avtal.</span><span class="sxs-lookup"><span data-stu-id="f1f36-114">Customers have two options for accepting the Microsoft Customer Agreement.</span></span> 

<span data-ttu-id="f1f36-115">**Alternativ 1**: partner attestering för kund godkännande – partner kan bekräfta kund acceptansen med hjälp av Partner Center API/SDK eller via instrument panelen för partner Center.</span><span class="sxs-lookup"><span data-stu-id="f1f36-115">**Option 1**: Partner attestation of customer acceptance - Partner can confirm customer acceptance using Partner Center API/SDK or through the Partner Center dashboard.</span></span>

<span data-ttu-id="f1f36-116">**Alternativ 2**: Kunddirekt godkännande – partner kan bjuda in kunden via en URL för att granska och godkänna avtalet i Microsoft 365 administrations centret.</span><span class="sxs-lookup"><span data-stu-id="f1f36-116">**Option 2**: Customer direct acceptance - Partner can invite the customer via a URL to review and accept the agreement in the Microsoft 365 Admin Center.</span></span>

## <a name="access-microsoft-customer-agreement-template"></a><span data-ttu-id="f1f36-117">Få åtkomst till Microsofts kundavtals mall</span><span class="sxs-lookup"><span data-stu-id="f1f36-117">Access Microsoft Customer Agreement template</span></span>

<span data-ttu-id="f1f36-118">Du kan manuellt hämta den senaste versionen av Microsoft kund avtals mal len [härifrån.](https://aka.ms/customeragreement)</span><span class="sxs-lookup"><span data-stu-id="f1f36-118">You can manually download the latest version of the Microsoft Customer Agreement template from [here](https://aka.ms/customeragreement).</span></span> <span data-ttu-id="f1f36-119">Microsofts kund avtal är landsspecifika.</span><span class="sxs-lookup"><span data-stu-id="f1f36-119">The Microsoft Customer Agreement is country-specific.</span></span> <span data-ttu-id="f1f36-120">När du begär Microsofts kund avtals mall måste du välja rätt land baserat på kundens plats.</span><span class="sxs-lookup"><span data-stu-id="f1f36-120">When requesting the Microsoft Customer Agreement template, be sure to select the correct country based on the customer's location.</span></span>

## <a name="option-1-confirm-customer-acceptance-in-partner-center"></a><span data-ttu-id="f1f36-121">Alternativ 1: bekräfta kund godkännande i Partner Center</span><span class="sxs-lookup"><span data-stu-id="f1f36-121">Option 1: Confirm customer acceptance in Partner Center</span></span>

<span data-ttu-id="f1f36-122">Partner kan bekräfta kund godkännande av Microsofts kund avtal i Partner Center för nya och befintliga kunder.</span><span class="sxs-lookup"><span data-stu-id="f1f36-122">Partners can confirm customer acceptance of the Microsoft Customer Agreement in Partner Center for new and existing customers.</span></span> <span data-ttu-id="f1f36-123">Åter försäljare kan inte attestera sina kunders räkning och behöver arbeta med sin indirekta leverantör för att få attesteringen slutförd.</span><span class="sxs-lookup"><span data-stu-id="f1f36-123">Resellers cannot attest on behalf of their customers and need to work with their Indirect Provider to get attestation completed.</span></span>

### <a name="confirm-customer-acceptance-for-new-customers"></a><span data-ttu-id="f1f36-124">Bekräfta kund godkännande för nya kunder</span><span class="sxs-lookup"><span data-stu-id="f1f36-124">Confirm customer acceptance for new customers</span></span>

<span data-ttu-id="f1f36-125">När du skapar en ny kund klient i Partner Center kan du använda följande steg för att bekräfta kundens godkännande av Microsofts kund avtal.</span><span class="sxs-lookup"><span data-stu-id="f1f36-125">When you create a new customer tenant in Partner Center, use the following steps to confirm the customer's acceptance of the Microsoft Customer Agreement.</span></span> <span data-ttu-id="f1f36-126">Du måste vara administratörs agent eller försäljnings agent för att kunna utföra dessa steg.</span><span class="sxs-lookup"><span data-stu-id="f1f36-126">You must be an Admin agent or Sales agent to perform these steps.</span></span>

1. <span data-ttu-id="f1f36-127">Välj **kunder** och sedan **ny kund**.</span><span class="sxs-lookup"><span data-stu-id="f1f36-127">Select **Customers**, and then **New customer**.</span></span>

2. <span data-ttu-id="f1f36-128">Under **konto information** anger du information för företaget och den primära kontakten.</span><span class="sxs-lookup"><span data-stu-id="f1f36-128">Under **Account info**, enter information for the company and its primary contact.</span></span>

3. <span data-ttu-id="f1f36-129">Under **Microsoft-avtal** markerar du kryss rutan för att bekräfta att kunden har godkänt Microsofts kund avtal.</span><span class="sxs-lookup"><span data-stu-id="f1f36-129">Under **Microsoft agreement**, select the box to attest that the customer has accepted the Microsoft Customer Agreement.</span></span>

4. <span data-ttu-id="f1f36-130">Ange ett datum under **avtalets godkännande datum**.</span><span class="sxs-lookup"><span data-stu-id="f1f36-130">Under **Agreement acceptance date**, enter the appropriate date.</span></span> <span data-ttu-id="f1f36-131">Du kan inte ange ett framtida datum.</span><span class="sxs-lookup"><span data-stu-id="f1f36-131">You cannot set this to a future date.</span></span>

5. <span data-ttu-id="f1f36-132">Kontrol lera att den primära användar kontakt informationen som visas är korrekt.</span><span class="sxs-lookup"><span data-stu-id="f1f36-132">Make sure that the primary user contact information displayed is correct.</span></span> <span data-ttu-id="f1f36-133">Om den är felaktig väljer du **Uppdatera** och anger korrekt information för den person som har godkänt avtalet.</span><span class="sxs-lookup"><span data-stu-id="f1f36-133">If it's incorrect, select **Update** and enter the accurate information for the person who accepted the agreement.</span></span>

6. <span data-ttu-id="f1f36-134">Välj **Nästa** för att fortsätta skapa kund klienten.</span><span class="sxs-lookup"><span data-stu-id="f1f36-134">Select **Next** to continue creating the customer tenant.</span></span>

   :::image type="content" source="images/mca/newcustomeragreement.jpg" alt-text="Ny kund":::  

### <a name="confirm-customer-acceptance-for-existing-customers"></a><span data-ttu-id="f1f36-136">Bekräfta kund godkännande för befintliga kunder</span><span class="sxs-lookup"><span data-stu-id="f1f36-136">Confirm customer acceptance for existing customers</span></span>

<span data-ttu-id="f1f36-137">Du måste vara administratörs agent eller försäljnings agent för att göra detta:</span><span class="sxs-lookup"><span data-stu-id="f1f36-137">You must be an Admin agent or Sales agent to do this:</span></span>

1. <span data-ttu-id="f1f36-138">Välj **Kunder**.</span><span class="sxs-lookup"><span data-stu-id="f1f36-138">Select **Customers**.</span></span> <span data-ttu-id="f1f36-139">Sök efter och välj kunden.</span><span class="sxs-lookup"><span data-stu-id="f1f36-139">Find and select the customer.</span></span>

2. <span data-ttu-id="f1f36-140">Välj **konto information**.</span><span class="sxs-lookup"><span data-stu-id="f1f36-140">Select **Account info**.</span></span>

3. <span data-ttu-id="f1f36-141">Under **Microsofts kund avtal** väljer du **Uppdatera**.</span><span class="sxs-lookup"><span data-stu-id="f1f36-141">Under **Microsoft Customer Agreement**, select **Update**.</span></span>

4. <span data-ttu-id="f1f36-142">Ange **förnamn**, **efter namn**, **e-postadress** och **telefonnummer** (valfritt) för den person som har godkänt avtalet.</span><span class="sxs-lookup"><span data-stu-id="f1f36-142">Enter the **First name**, **Last name**, **Email address**, and **Phone number** (optional) of the person who accepted the agreement.</span></span> <span data-ttu-id="f1f36-143">Ange ett datum under **avtalets godkännande datum**.</span><span class="sxs-lookup"><span data-stu-id="f1f36-143">Under **Agreement acceptance date**, enter the appropriate date.</span></span> <span data-ttu-id="f1f36-144">Du kan inte ange ett framtida datum.</span><span class="sxs-lookup"><span data-stu-id="f1f36-144">You cannot set this to a future date.</span></span>

5. <span data-ttu-id="f1f36-145">Välj **Spara** och fortsätt.</span><span class="sxs-lookup"><span data-stu-id="f1f36-145">Select **Save** and continue.</span></span>

   :::image type="content" source="images/mcua2-update2.png" alt-text="Befintlig kund":::

### <a name="retrieve-confirmation-of-customer-acceptance"></a><span data-ttu-id="f1f36-147">Hämta bekräftelse av kund godkännande</span><span class="sxs-lookup"><span data-stu-id="f1f36-147">Retrieve confirmation of customer acceptance</span></span>

<span data-ttu-id="f1f36-148">Du kan hämta en bekräftelse på att en befintlig kund har godkänt Microsofts kund avtal med hjälp av följande steg.</span><span class="sxs-lookup"><span data-stu-id="f1f36-148">You can retrieve confirmation that an existing customer has accepted the Microsoft Customer Agreement using the following steps.</span></span> <span data-ttu-id="f1f36-149">Du måste vara administratörs agent eller försäljnings agent för att göra detta.</span><span class="sxs-lookup"><span data-stu-id="f1f36-149">You must be an Admin agent or Sales agent to do this.</span></span>

1. <span data-ttu-id="f1f36-150">Välj **kunder** och leta upp och välj den kund som du vill se.</span><span class="sxs-lookup"><span data-stu-id="f1f36-150">Select **Customers**, and then find and select the customer you want to see.</span></span>

2. <span data-ttu-id="f1f36-151">Välj **konto information**.</span><span class="sxs-lookup"><span data-stu-id="f1f36-151">Select **Account info**.</span></span>

3. <span data-ttu-id="f1f36-152">Under **Microsofts kund avtal** kan du Visa om bekräftelsen har eller inte har tillhandahållits av den här kunden.</span><span class="sxs-lookup"><span data-stu-id="f1f36-152">Under **Microsoft customer agreement**, view if confirmation has or hasn't been provided by this customer.</span></span>

## <a name="confirm-customer-acceptance-using-partner-center-apisdk"></a><span data-ttu-id="f1f36-153">Bekräfta kund godkännande med partner Center API/SDK</span><span class="sxs-lookup"><span data-stu-id="f1f36-153">Confirm customer acceptance using Partner Center API/SDK</span></span>

<span data-ttu-id="f1f36-154">Du kan använda Partner Center API/SDK för att bekräfta kund godkännande av Microsofts kund avtal.</span><span class="sxs-lookup"><span data-stu-id="f1f36-154">You can use Partner Center API/SDK to confirm customer acceptance of the Microsoft Customer Agreement.</span></span> <span data-ttu-id="f1f36-155">Mer information om API/SDK finns i:</span><span class="sxs-lookup"><span data-stu-id="f1f36-155">For details on the API/SDK, refer to:</span></span>

- [<span data-ttu-id="f1f36-156">Hämta avtals-metadata för Microsofts kund avtal</span><span class="sxs-lookup"><span data-stu-id="f1f36-156">Get agreement metadata for the Microsoft Customer Agreement</span></span>](/partner-center/develop/get-customer-agreement-metadata)

- [<span data-ttu-id="f1f36-157">Bekräfta kund godkännande av Microsofts kund avtal</span><span class="sxs-lookup"><span data-stu-id="f1f36-157">Confirm customer acceptance of Microsoft Customer Agreement</span></span>](/partner-center/develop/confirm-customer-consent-customer-agreement)

- [<span data-ttu-id="f1f36-158">Få bekräftelse på kund godkännande av Microsofts kund avtal</span><span class="sxs-lookup"><span data-stu-id="f1f36-158">Get confirmation of customer acceptance of Microsoft Customer Agreement</span></span>](/partner-center/develop/get-confirmation-of-customer-agreement)

- [<span data-ttu-id="f1f36-159">Hämta en nedladdnings länk för Microsofts kund avtals mall</span><span class="sxs-lookup"><span data-stu-id="f1f36-159">Get a download link for the Microsoft Customer Agreement template</span></span>](/partner-center/develop/download-customer-agreement-template)

## <a name="option-2-customer-acceptance-in-microsoft-365-admin-center"></a><span data-ttu-id="f1f36-160">Alternativ 2: kund godkännande i Microsoft 365 administrations Center</span><span class="sxs-lookup"><span data-stu-id="f1f36-160">Option 2: Customer acceptance in Microsoft 365 Admin Center</span></span>

<span data-ttu-id="f1f36-161">Partner kan bjuda in nya och befintliga kunder via en URL för att granska och godkänna avtalet i Microsoft 365 administrations centret.</span><span class="sxs-lookup"><span data-stu-id="f1f36-161">Partners can invite new and existing customers, via a URL, to review and accept the agreement within the Microsoft 365 Admin Center.</span></span> <span data-ttu-id="f1f36-162">I följande avsnitt visas hur du:</span><span class="sxs-lookup"><span data-stu-id="f1f36-162">The next few sections show you how to:</span></span>

- <span data-ttu-id="f1f36-163">Skapa en ny kund och Bjud in kunden att granska och godkänna avtalet.</span><span class="sxs-lookup"><span data-stu-id="f1f36-163">Create a new customer and invite the customer to review and accept the agreement.</span></span>

- <span data-ttu-id="f1f36-164">Bjud in en ny kund att granska och godkänna åter försäljarens relation och avtal.</span><span class="sxs-lookup"><span data-stu-id="f1f36-164">Invite a new customer to review and accept the reseller relationship and agreement.</span></span>

- <span data-ttu-id="f1f36-165">Bjud in en befintlig kund för att granska och godkänna avtalet.</span><span class="sxs-lookup"><span data-stu-id="f1f36-165">Invite an existing customer to review and accept the agreement.</span></span>

>[!NOTE]
> <span data-ttu-id="f1f36-166">Du kan använda [partner Center API/SDK](/partner-center/develop/get-direct-sign-status-of-customer-agreement) för att hämta statusen för kundens direkta godkännande av Microsofts kund avtal.</span><span class="sxs-lookup"><span data-stu-id="f1f36-166">You can use [Partner Center API/SDK](/partner-center/develop/get-direct-sign-status-of-customer-agreement) to get the status of a customer's direct acceptance of the Microsoft Customer Agreement.</span></span>  

## <a name="create-a-new-customer-and-invite-the-customer-to-review-and-accept-the-agreement"></a><span data-ttu-id="f1f36-167">Skapa en ny kund och Bjud in kunden att granska och godkänna avtalet</span><span class="sxs-lookup"><span data-stu-id="f1f36-167">Create a new customer and invite the customer to review and accept the agreement</span></span>

<span data-ttu-id="f1f36-168">Använd följande steg för att skapa en ny kund i Partner Center och sedan bjuda in dem att granska och godkänna Microsofts kund avtal i Microsoft 365 administrations Center.</span><span class="sxs-lookup"><span data-stu-id="f1f36-168">Use the following steps to create a new customer in Partner Center then invite them to review and accept the Microsoft Customer Agreement within Microsoft 365 Admin Center.</span></span>

1. <span data-ttu-id="f1f36-169">Välj **Lägg till kund** på fliken **kunder** i Partner Center.</span><span class="sxs-lookup"><span data-stu-id="f1f36-169">From the **Customers** tab within Partner Center, select **Add customer**.</span></span>

2. <span data-ttu-id="f1f36-170">Under **konto information** anger du information om den nya kunden i alla obligatoriska fält, inklusive kundens företags namn och primär kontakt.</span><span class="sxs-lookup"><span data-stu-id="f1f36-170">Under **Account Info**, enter information about the new customer in all required fields, including the customer's company name and primary contact.</span></span>

3. <span data-ttu-id="f1f36-171">Under **kund avtal** väljer du det första alternativet. **kunden uppmanas att godkänna Microsofts kund avtal i Microsoft 365 administrations Center**.</span><span class="sxs-lookup"><span data-stu-id="f1f36-171">Under **Customer Agreement**, select the first option, **Customer will be asked to accept the Microsoft Customer Agreement in Microsoft 365 Admin Center**.</span></span> <span data-ttu-id="f1f36-172">Fyll i alla andra obligatoriska fält på sidan.</span><span class="sxs-lookup"><span data-stu-id="f1f36-172">Complete any other required fields on the page.</span></span>

4. <span data-ttu-id="f1f36-173">Välj **Nästa: granska** och fortsätt sedan stegen för att skapa kund klienten.</span><span class="sxs-lookup"><span data-stu-id="f1f36-173">Select **Next: Review** then continue the steps to create the customer tenant.</span></span> 

>[!NOTE] 
><span data-ttu-id="f1f36-174">Nya kunder kan inte göra ett nytt inköp förrän de accepterar Microsofts kund avtal.</span><span class="sxs-lookup"><span data-stu-id="f1f36-174">New customers cannot make a new purchase until they accept the Microsoft Customer Agreement.</span></span>  

   :::image type="content" source="images/mca/create-new-customer.jpg" alt-text="Skapa ny kund":::

5. <span data-ttu-id="f1f36-176">När du når **bekräftelse** skärmen i det nya kund arbets flödet sparar du kundens autentiseringsuppgifter.</span><span class="sxs-lookup"><span data-stu-id="f1f36-176">When you reach the **Confirmation** screen in the new customer workflow, save the customer credentials.</span></span> <span data-ttu-id="f1f36-177">Du måste ange autentiseringsuppgifterna för din kund senare.</span><span class="sxs-lookup"><span data-stu-id="f1f36-177">You will need to give these credentials to your customer later.</span></span>

6. <span data-ttu-id="f1f36-178">Utanför Partner Center skapar och skickar du ett e-postmeddelande som bjuder in kunden att godkänna Microsofts kund avtal i Microsoft 365 administrations Center.</span><span class="sxs-lookup"><span data-stu-id="f1f36-178">Outside of Partner Center, create and send an email that invites the customer to accept the Microsoft Customer Agreement in Microsoft 365 Admin Center.</span></span> <span data-ttu-id="f1f36-179">Se till att ta med dessa objekt i e-postmeddelandet:</span><span class="sxs-lookup"><span data-stu-id="f1f36-179">Make sure to include these items in the email:</span></span>

   - <span data-ttu-id="f1f36-180">En länk till denna [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement) (inloggning krävs)</span><span class="sxs-lookup"><span data-stu-id="f1f36-180">A link to this [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement) (Sign-in required)</span></span>

   - <span data-ttu-id="f1f36-181">Kundens autentiseringsuppgifter som du sparade i steg 5.</span><span class="sxs-lookup"><span data-stu-id="f1f36-181">The customer's credentials you saved in Step 5.</span></span>

7. <span data-ttu-id="f1f36-182">Kunden får sedan e-postinbjudan från partnern och välja [URL: en](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement).</span><span class="sxs-lookup"><span data-stu-id="f1f36-182">The customer will then receive the email invite from the partner and select the [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement).</span></span>

8. <span data-ttu-id="f1f36-183">Kunden loggar in i Microsoft 365 administrations Center med hjälp av de kundautentiseringsuppgifter som tidigare togs emot från partnern.</span><span class="sxs-lookup"><span data-stu-id="f1f36-183">The customer signs into Microsoft 365 Admin Center using the customer credentials previously received from the partner.</span></span>

9. <span data-ttu-id="f1f36-184">Kunden kontrollerar sedan rutan för att godkänna Microsofts kund avtal.</span><span class="sxs-lookup"><span data-stu-id="f1f36-184">The customer then checks the box to accept the Microsoft Customer agreement.</span></span>

## <a name="invite-a-new-customer-to-review-and-accept-the-reseller-relationship-and-microsoft-customer-agreement"></a><span data-ttu-id="f1f36-185">Bjud in en ny kund att granska och godkänna åter försäljarens relation och Microsofts kund avtal</span><span class="sxs-lookup"><span data-stu-id="f1f36-185">Invite a new customer to review and accept the reseller relationship and Microsoft Customer Agreement</span></span> 

<span data-ttu-id="f1f36-186">Använd följande steg för att bjuda in en ny kund att granska och godkänna åter försäljarens relation och Microsofts kund avtal.</span><span class="sxs-lookup"><span data-stu-id="f1f36-186">Use the following steps to invite a new customer to review and accept the reseller relationship and the Microsoft Customer Agreement.</span></span> 

1. <span data-ttu-id="f1f36-187">På fliken **kunder** i Partner Center väljer du **begär en åter försäljares Relations** länk.</span><span class="sxs-lookup"><span data-stu-id="f1f36-187">From the **Customers** tab within Partner Center, select **Request a reseller relationship** link.</span></span> 

2. <span data-ttu-id="f1f36-188">En mall för automatisk e-post kommer att skapas, inklusive text och en parametriserad URL som leder kunden till Microsoft 365 administrations Center.</span><span class="sxs-lookup"><span data-stu-id="f1f36-188">An automatic email template will be generated, including text and a parameterized URL that directs the customer to the Microsoft 365 Admin Center.</span></span>

3. <span data-ttu-id="f1f36-189">Du kan anpassa den automatiskt genererade e-postmallen och sedan välja **Kopiera till Urklipp** eller **Öppna i e-post**.</span><span class="sxs-lookup"><span data-stu-id="f1f36-189">You can customize the automatically generated email template and then select **Copy to clipboard** or **Open in email**.</span></span>

4. <span data-ttu-id="f1f36-190">Använd den här e-postmallen för att bjuda in kunden att acceptera **åter försäljarens Relations** förfrågan och **Microsofts kund avtal**.</span><span class="sxs-lookup"><span data-stu-id="f1f36-190">Use this email template to invite the customer to accept **reseller relationship** request and the **Microsoft Customer Agreement**.</span></span> <span data-ttu-id="f1f36-191">(Obs! i e-postinbjudanen ser du till att partnern även innehåller den URL som angavs automatiskt samt de autentiseringsuppgifter för kunden som nyligen har skapats.)</span><span class="sxs-lookup"><span data-stu-id="f1f36-191">(Note: In the email invite, make sure the partner also includes the URL that was automatically provided as well as the customer credentials that were recently created.)</span></span>

   :::image type="content" source="images/mca/createrelationship.png" alt-text="skapa en relation":::

5. <span data-ttu-id="f1f36-193">Kunden tar emot inbjudan via e-post och klickar på URL: en för parametern.</span><span class="sxs-lookup"><span data-stu-id="f1f36-193">Customer receives invite via email and clicks on the parameterized URL.</span></span> 

6. <span data-ttu-id="f1f36-194">Kunden använder autentiseringsuppgifter från partnern i e-postmeddelandet för att logga in på Microsoft 365 administrations Center.</span><span class="sxs-lookup"><span data-stu-id="f1f36-194">Customer uses credentials provided by partner within email to sign into Microsoft 365 Admin Center.</span></span>

7. <span data-ttu-id="f1f36-195">Kunden kontrollerar rutan för att godkänna **åter försäljarens relation** och **Microsofts kund avtal**.</span><span class="sxs-lookup"><span data-stu-id="f1f36-195">Customer checks the box to accept the **reseller relationship** and **Microsoft Customer Agreement**.</span></span> 

8. <span data-ttu-id="f1f36-196">Inom samma URL kan kunden se en lista över olika partners som de arbetar med.</span><span class="sxs-lookup"><span data-stu-id="f1f36-196">Within the same URL, the customer is able to see a consolidated list of different partners they are working with.</span></span> <span data-ttu-id="f1f36-197">De kan välja en partner för att se information.</span><span class="sxs-lookup"><span data-stu-id="f1f36-197">They can select a partner to see details.</span></span>

   :::image type="content" source="images/mca/accept.jpg" alt-text="Godkänna avtal":::


## <a name="invite-an-existing-customer-to-review-and-accept-the-agreement"></a><span data-ttu-id="f1f36-199">Bjud in en befintlig kund för att granska och godkänna avtalet</span><span class="sxs-lookup"><span data-stu-id="f1f36-199">Invite an existing customer to review and accept the agreement</span></span>

<span data-ttu-id="f1f36-200">Använd följande steg för att bjuda in en befintlig kund att granska och godkänna Microsofts kund avtal.</span><span class="sxs-lookup"><span data-stu-id="f1f36-200">Use the following steps to invite an existing customer to review and accept the Microsoft Customer Agreement.</span></span> 

1. <span data-ttu-id="f1f36-201">Skapa kund-e-postmeddelandet med den inbäddade URL: en som bjuder in kunden att godkänna Microsofts kund avtal.</span><span class="sxs-lookup"><span data-stu-id="f1f36-201">Create the customer email with the embedded URL inviting your customer to accept the Microsoft Customer Agreement.</span></span>

2. <span data-ttu-id="f1f36-202">Kunden får inbjudan via e-post och klickar på [URL: en](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement).</span><span class="sxs-lookup"><span data-stu-id="f1f36-202">Your customer receives the invitation via email and clicks the [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement).</span></span> 

3. <span data-ttu-id="f1f36-203">Kunden anger sina autentiseringsuppgifter i Microsoft 365 administrations Center.</span><span class="sxs-lookup"><span data-stu-id="f1f36-203">The customer enters their credentials into Microsoft 365 Admin Center.</span></span>

4. <span data-ttu-id="f1f36-204">Kunden söker i rutan om att godkänna Microsofts kund avtal.</span><span class="sxs-lookup"><span data-stu-id="f1f36-204">Your customer checks the box to accept the Microsoft Customer Agreement.</span></span> 

5. <span data-ttu-id="f1f36-205">I samma URL kan kunden se den konsoliderade listan över olika partners som de arbetar med.</span><span class="sxs-lookup"><span data-stu-id="f1f36-205">Within the same URL, the customer can see the consolidated list of different partners they are working with.</span></span> <span data-ttu-id="f1f36-206">De kan välja en partner för att se information.</span><span class="sxs-lookup"><span data-stu-id="f1f36-206">They can select a partner to see details.</span></span>

   :::image type="content" source="images/mca/customeraccept.png" alt-text="kund":::

>[!NOTE]
><span data-ttu-id="f1f36-208">I vissa fall kanske kunderna inte kan acceptera Microsofts kund avtal direkt.</span><span class="sxs-lookup"><span data-stu-id="f1f36-208">In certain scenarios, customers may not be able to directly accept the Microsoft Customer Agreement.</span></span> <span data-ttu-id="f1f36-209">Mer information om de här situationerna finns i [två scenarier där du behöver intyga för kundens räkning](attest-acceptance-customer-agreement.md).</span><span class="sxs-lookup"><span data-stu-id="f1f36-209">To learn more about these situations, see [Two scenarios where you need to attest on behalf of your customer](attest-acceptance-customer-agreement.md).</span></span>

### <a name="historical-timeline-details"></a><span data-ttu-id="f1f36-210">Information om historisk tids linje</span><span class="sxs-lookup"><span data-stu-id="f1f36-210">Historical timeline details</span></span>

| <span data-ttu-id="f1f36-211">Datum</span><span class="sxs-lookup"><span data-stu-id="f1f36-211">Date</span></span> | <span data-ttu-id="f1f36-212">Gränser</span><span class="sxs-lookup"><span data-stu-id="f1f36-212">Milestone</span></span> | <span data-ttu-id="f1f36-213">Information</span><span class="sxs-lookup"><span data-stu-id="f1f36-213">Details</span></span> |
|------------|------------|--------------------------------|
|<span data-ttu-id="f1f36-214">01 augusti 2019</span><span class="sxs-lookup"><span data-stu-id="f1f36-214">August 01, 2019</span></span>| <span data-ttu-id="f1f36-215">UX-förhandsgranskning som är tillgänglig i sandbox</span><span class="sxs-lookup"><span data-stu-id="f1f36-215">UX preview available in sandbox</span></span>| <span data-ttu-id="f1f36-216">Partner kan bekräfta kund godkännande av Microsofts kund avtal med hjälp av Partner Center-instrumentpanelen i sand Box miljön för KRYPTOGRAFI.</span><span class="sxs-lookup"><span data-stu-id="f1f36-216">Partners can confirm customer acceptance of the Microsoft Customer Agreement using the Partner Center dashboard in the CSP sandbox environment.</span></span> <span data-ttu-id="f1f36-217">Partner med åtkomst till CSP sandbox-miljön för hands versions ändringar av användar upplevelsen.</span><span class="sxs-lookup"><span data-stu-id="f1f36-217">Partners with access to the CSP sandbox environment preview the user experience changes.</span></span> <span data-ttu-id="f1f36-218">Partner utan sandbox-åtkomst kan lära sig mer om ändringarna i det här avsnittet.</span><span class="sxs-lookup"><span data-stu-id="f1f36-218">Partners without sandbox access can learn about the changes in this topic.</span></span>|
|<span data-ttu-id="f1f36-219">September 03 2019</span><span class="sxs-lookup"><span data-stu-id="f1f36-219">September 03, 2019</span></span>|<span data-ttu-id="f1f36-220">API Preview är tillgängligt i begränsat läge.</span><span class="sxs-lookup"><span data-stu-id="f1f36-220">API preview is available in sandbox.</span></span>|<span data-ttu-id="f1f36-221">Partner kan bekräfta kund godkännande av Microsofts kund avtal med hjälp av API för partner Center i sand Box miljö.</span><span class="sxs-lookup"><span data-stu-id="f1f36-221">Partner can confirm customer acceptance of the Microsoft Customer Agreement using Partner Center API in CSP sandbox environment.</span></span> <span data-ttu-id="f1f36-222">API-partner kan använda den här möjligheten för att förhandsgranska API-ändringar och börja arbeta med API-integrering för att stödja det nya avtalet.</span><span class="sxs-lookup"><span data-stu-id="f1f36-222">API partners can use this opportunity to preview the API changes and start working on API integration to support the new agreement.</span></span>|
|<span data-ttu-id="f1f36-223">20 september 2019</span><span class="sxs-lookup"><span data-stu-id="f1f36-223">September 20, 2019</span></span>|<span data-ttu-id="f1f36-224">.NET SDK-förhands granskning är tillgänglig i begränsat läge.</span><span class="sxs-lookup"><span data-stu-id="f1f36-224">.NET SDK preview is available in sandbox.</span></span>|<span data-ttu-id="f1f36-225">Partner kan bekräfta kund godkännande av Microsofts kund avtal med partner Center .NET SDK i sand Box miljö.</span><span class="sxs-lookup"><span data-stu-id="f1f36-225">Partner can confirm customer acceptance of the Microsoft Customer Agreement using Partner Center .NET SDK in CSP sandbox environment.</span></span> <span data-ttu-id="f1f36-226">API-partner kan använda den här möjligheten för att förhandsgranska .NET SDK-ändringar och börja arbeta med API-integrering för att stödja det nya avtalet.</span><span class="sxs-lookup"><span data-stu-id="f1f36-226">API partners can use this opportunity to preview the .NET SDK changes and start working on API integration to support the new agreement.</span></span>|
|<span data-ttu-id="f1f36-227">01 oktober 2019</span><span class="sxs-lookup"><span data-stu-id="f1f36-227">October 01, 2019</span></span>|<span data-ttu-id="f1f36-228">Microsofts kund avtal finns i produktion</span><span class="sxs-lookup"><span data-stu-id="f1f36-228">Microsoft Customer Agreement available in production</span></span>|<span data-ttu-id="f1f36-229">Microsoft presenterar Microsofts kund avtal till CSP-programmet för att ersätta Microsoft Clouds avtalet.</span><span class="sxs-lookup"><span data-stu-id="f1f36-229">Microsoft introduces the Microsoft Customer Agreement to the CSP program to replace the Microsoft Cloud Agreement.</span></span> <span data-ttu-id="f1f36-230">Partner kan bekräfta kund godkännande av Microsofts kund avtal med hjälp av Partner Center-instrumentpanelen och API: et i produktionen.</span><span class="sxs-lookup"><span data-stu-id="f1f36-230">Partners can confirm customer acceptance of the Microsoft Customer Agreement using the Partner Center dashboard and API in production.</span></span> <span data-ttu-id="f1f36-231">Microsoft Cloud avtalet stöds fortfarande i CSP-partnerprogram.</span><span class="sxs-lookup"><span data-stu-id="f1f36-231">The Microsoft Cloud Agreement remains supported within the CSP partner program.</span></span> <span data-ttu-id="f1f36-232">Partner uppmanas dock att börja migrera till Microsofts kund avtal.</span><span class="sxs-lookup"><span data-stu-id="f1f36-232">However, partners are advised to start migrating to the Microsoft Customer Agreement.</span></span> <span data-ttu-id="f1f36-233">Nya inköps-och licens antal ändringar i befintliga prenumerationer kräver partner bekräftelse av antingen Microsofts kund avtal eller Microsoft Cloud avtal.</span><span class="sxs-lookup"><span data-stu-id="f1f36-233">New purchases and license count changes to existing subscriptions will require partner confirmation of either the Microsoft Customer Agreement or the Microsoft Cloud Agreement.</span></span> <span data-ttu-id="f1f36-234">Vissa nya erbjudanden (till exempel den nya Azure-prenumerationen) kräver att du bekräftar Microsofts kund avtal.</span><span class="sxs-lookup"><span data-stu-id="f1f36-234">Certain new offers (for example, the new Azure plan) will require confirmation of the Microsoft Customer Agreement.</span></span>|
|<span data-ttu-id="f1f36-235">31 januari 2020</span><span class="sxs-lookup"><span data-stu-id="f1f36-235">January 31, 2020</span></span>|<span data-ttu-id="f1f36-236">Microsoft Cloud avtalet har tagits bort från produktionen</span><span class="sxs-lookup"><span data-stu-id="f1f36-236">Microsoft Cloud Agreement removed from production</span></span>|<span data-ttu-id="f1f36-237">Microsoft Cloud avtalet godkänns inte längre i CSP-partner programmet.</span><span class="sxs-lookup"><span data-stu-id="f1f36-237">The Microsoft Cloud Agreement is no longer accepted within the CSP partner program.</span></span> <span data-ttu-id="f1f36-238">Nya köp-och licens antal ändringar i befintliga prenumerationer kräver att partnern tillhandahåller en bekräftelse på Microsofts kund avtal.</span><span class="sxs-lookup"><span data-stu-id="f1f36-238">New purchases and license count changes to existing subscriptions will require the partner to provide confirmation of the Microsoft Customer Agreement.</span></span> <span data-ttu-id="f1f36-239">Detta krav gäller för nya kunder och befintliga kunder som tidigare har godkänt Microsoft Cloud avtalet.</span><span class="sxs-lookup"><span data-stu-id="f1f36-239">This requirement applies to new customers and existing customers who may have previously accepted the Microsoft Cloud Agreement.</span></span>|
|<span data-ttu-id="f1f36-240">3 februari 2020</span><span class="sxs-lookup"><span data-stu-id="f1f36-240">February 3, 2020</span></span>|<span data-ttu-id="f1f36-241">Partner har nu möjlighet att bjuda in kunden via en URL för att granska och godkänna avtalet i autentiserade Microsoft 365 administrations Center.</span><span class="sxs-lookup"><span data-stu-id="f1f36-241">Partner now has the option to invite the customer via a URL to review and accept the agreement in authenticated Microsoft 365 Admin Center.</span></span> | <span data-ttu-id="f1f36-242">Kunden kan godkänna Microsofts kund avtal i Microsoft 365 administrations Center.</span><span class="sxs-lookup"><span data-stu-id="f1f36-242">Customer can accept the Microsoft Customer Agreement in Microsoft 365 Admin Center.</span></span> <span data-ttu-id="f1f36-243">Kundens direkta godkännande av avtalet i Microsoft 365 Admin Center bekräftar godkännande av villkor.</span><span class="sxs-lookup"><span data-stu-id="f1f36-243">Customer's direct acceptance of the agreement in Microsoft 365 Admin Center confirms approval of terms.</span></span> 