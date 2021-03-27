---
title: Så här bekräftar du att kunden har godkänt Microsofts kund avtal med CSP-programmet
description: Leverantörer av moln lösningar (CSP) behöver bekräfta kund godkännande av Microsofts kund avtal innan de beställer Microsoft-tjänster för kunder.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: aarzh-AaronZhang
ms.author: v-aarzh
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.date: 03/24/2021
ms.openlocfilehash: ebb52a3a8223d3b1101e3a8e78728fcc167e25e3
ms.sourcegitcommit: a691d4cbe144a8fd71e344fd293cc658ac11d6f3
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/27/2021
ms.locfileid: "105633786"
---
# <a name="how-to-confirm-that-your-customer-has-accepted-the-microsoft-customer-agreement-to-the-csp-program"></a><span data-ttu-id="bc33b-103">Så här bekräftar du att kunden har godkänt Microsofts kund avtal med CSP-programmet</span><span class="sxs-lookup"><span data-stu-id="bc33b-103">How to confirm that your customer has accepted the Microsoft Customer Agreement to the CSP program</span></span>

<span data-ttu-id="bc33b-104">**Lämpliga roller**</span><span class="sxs-lookup"><span data-stu-id="bc33b-104">**Appropriate roles**</span></span>

- <span data-ttu-id="bc33b-105">Administratörs agent</span><span class="sxs-lookup"><span data-stu-id="bc33b-105">Admin agent</span></span>
- <span data-ttu-id="bc33b-106">Försäljnings agent</span><span class="sxs-lookup"><span data-stu-id="bc33b-106">Sales agent</span></span>


<span data-ttu-id="bc33b-107">Kunder har två alternativ för hur de godkänner Microsofts kund avtal.</span><span class="sxs-lookup"><span data-stu-id="bc33b-107">Customers have two options for how they accept the Microsoft Customer Agreement.</span></span>

<span data-ttu-id="bc33b-108">**Alternativ 1**: partner attestering för kund godkännande – partner kan bekräfta kund acceptansen med hjälp av Partner Center API/SDK eller via instrument panelen för partner Center.</span><span class="sxs-lookup"><span data-stu-id="bc33b-108">**Option 1**: Partner attestation of customer acceptance - Partner can confirm customer acceptance using Partner Center API/SDK or through the Partner Center dashboard.</span></span>

<span data-ttu-id="bc33b-109">**Alternativ 2**: Kunddirekt godkännande – partner kan bjuda in kunden via en URL för att granska och godkänna avtalet i Microsoft 365 administrations centret.</span><span class="sxs-lookup"><span data-stu-id="bc33b-109">**Option 2**: Customer direct acceptance - Partner can invite the customer via a URL to review and accept the agreement in the Microsoft 365 Admin Center.</span></span>

## <a name="access-microsoft-customer-agreement-template"></a><span data-ttu-id="bc33b-110">Få åtkomst till Microsofts kundavtals mall</span><span class="sxs-lookup"><span data-stu-id="bc33b-110">Access Microsoft Customer Agreement template</span></span>

<span data-ttu-id="bc33b-111">Du kan manuellt hämta den senaste versionen av Microsoft kund avtals mal len [härifrån.](https://aka.ms/customeragreement)</span><span class="sxs-lookup"><span data-stu-id="bc33b-111">You can manually download the latest version of the Microsoft Customer Agreement template from [here](https://aka.ms/customeragreement).</span></span> <span data-ttu-id="bc33b-112">Microsofts kund avtal är landsspecifika.</span><span class="sxs-lookup"><span data-stu-id="bc33b-112">The Microsoft Customer Agreement is country-specific.</span></span> <span data-ttu-id="bc33b-113">När du begär Microsofts kund avtals mall måste du välja rätt land baserat på kundens plats.</span><span class="sxs-lookup"><span data-stu-id="bc33b-113">When requesting the Microsoft Customer Agreement template, be sure to select the correct country based on the customer's location.</span></span>

## <a name="option-1-confirm-customer-acceptance-in-partner-center"></a><span data-ttu-id="bc33b-114">Alternativ 1: bekräfta kund godkännande i Partner Center</span><span class="sxs-lookup"><span data-stu-id="bc33b-114">Option 1: Confirm customer acceptance in Partner Center</span></span>

<span data-ttu-id="bc33b-115">Direkt fakturerings partner kan bekräfta kund godkännande av Microsofts kund avtal i Partner Center för nya och befintliga kunder.</span><span class="sxs-lookup"><span data-stu-id="bc33b-115">Direct bill partners can confirm customer acceptance of the Microsoft Customer Agreement in Partner Center for new and existing customers.</span></span> <span data-ttu-id="bc33b-116">Indirekta åter försäljare kan inte attestera sina kunders räkning och behöver arbeta med sin indirekta leverantör för att få attesteringen slutförd.</span><span class="sxs-lookup"><span data-stu-id="bc33b-116">Indirect resellers cannot attest on behalf of their customers and need to work with their Indirect Provider to get attestation completed.</span></span>

### <a name="confirm-customer-acceptance-for-new-customers"></a><span data-ttu-id="bc33b-117">Bekräfta kund godkännande för nya kunder</span><span class="sxs-lookup"><span data-stu-id="bc33b-117">Confirm customer acceptance for new customers</span></span>

<span data-ttu-id="bc33b-118">När du skapar en ny kund klient i Partner Center kan du använda följande steg för att bekräfta kundens godkännande av Microsofts kund avtal.</span><span class="sxs-lookup"><span data-stu-id="bc33b-118">When you create a new customer tenant in Partner Center, use the following steps to confirm the customer's acceptance of the Microsoft Customer Agreement.</span></span> <span data-ttu-id="bc33b-119">Du måste vara administratörs agent eller försäljnings agent för att kunna utföra dessa steg.</span><span class="sxs-lookup"><span data-stu-id="bc33b-119">You must be an Admin agent or Sales agent to perform these steps.</span></span>

1. <span data-ttu-id="bc33b-120">Välj **kunder** och sedan **ny kund**.</span><span class="sxs-lookup"><span data-stu-id="bc33b-120">Select **Customers**, and then **New customer**.</span></span>

2. <span data-ttu-id="bc33b-121">Under **konto information** anger du information för företaget och den primära kontakten.</span><span class="sxs-lookup"><span data-stu-id="bc33b-121">Under **Account info**, enter information for the company and its primary contact.</span></span>

3. <span data-ttu-id="bc33b-122">Under **Microsoft-avtal** markerar du kryss rutan för att bekräfta att kunden har godkänt Microsofts kund avtal.</span><span class="sxs-lookup"><span data-stu-id="bc33b-122">Under **Microsoft agreement**, select the box to attest that the customer has accepted the Microsoft Customer Agreement.</span></span>

4. <span data-ttu-id="bc33b-123">Ange ett datum under **avtalets godkännande datum**.</span><span class="sxs-lookup"><span data-stu-id="bc33b-123">Under **Agreement acceptance date**, enter the appropriate date.</span></span> <span data-ttu-id="bc33b-124">Du kan inte ange ett framtida datum.</span><span class="sxs-lookup"><span data-stu-id="bc33b-124">You cannot set this to a future date.</span></span>

5. <span data-ttu-id="bc33b-125">Kontrol lera att den primära användar kontakt informationen som visas är korrekt.</span><span class="sxs-lookup"><span data-stu-id="bc33b-125">Make sure that the primary user contact information displayed is correct.</span></span> <span data-ttu-id="bc33b-126">Om den är felaktig väljer du **Uppdatera** och anger korrekt information för den person som har godkänt avtalet.</span><span class="sxs-lookup"><span data-stu-id="bc33b-126">If it's incorrect, select **Update** and enter the accurate information for the person who accepted the agreement.</span></span>

6. <span data-ttu-id="bc33b-127">Välj **Nästa** för att fortsätta skapa kund klienten.</span><span class="sxs-lookup"><span data-stu-id="bc33b-127">Select **Next** to continue creating the customer tenant.</span></span>

   :::image type="content" source="images/mca/newcustomeragreement.jpg" alt-text="Ny kund":::  

### <a name="confirm-customer-acceptance-for-existing-customers"></a><span data-ttu-id="bc33b-129">Bekräfta kund godkännande för befintliga kunder</span><span class="sxs-lookup"><span data-stu-id="bc33b-129">Confirm customer acceptance for existing customers</span></span>

<span data-ttu-id="bc33b-130">Du måste vara administratörs agent eller försäljnings agent för att göra detta:</span><span class="sxs-lookup"><span data-stu-id="bc33b-130">You must be an Admin agent or Sales agent to do this:</span></span>

1. <span data-ttu-id="bc33b-131">Välj **Kunder**.</span><span class="sxs-lookup"><span data-stu-id="bc33b-131">Select **Customers**.</span></span> <span data-ttu-id="bc33b-132">Sök efter och välj kunden.</span><span class="sxs-lookup"><span data-stu-id="bc33b-132">Find and select the customer.</span></span>

2. <span data-ttu-id="bc33b-133">Välj **konto information**.</span><span class="sxs-lookup"><span data-stu-id="bc33b-133">Select **Account info**.</span></span>

3. <span data-ttu-id="bc33b-134">Under **Microsofts kund avtal** väljer du **Uppdatera**.</span><span class="sxs-lookup"><span data-stu-id="bc33b-134">Under **Microsoft Customer Agreement**, select **Update**.</span></span>

4. <span data-ttu-id="bc33b-135">Ange **förnamn**, **efter namn**, **e-postadress** och **telefonnummer** (valfritt) för den person som har godkänt avtalet.</span><span class="sxs-lookup"><span data-stu-id="bc33b-135">Enter the **First name**, **Last name**, **Email address**, and **Phone number** (optional) of the person who accepted the agreement.</span></span> <span data-ttu-id="bc33b-136">Ange ett datum under **avtalets godkännande datum**.</span><span class="sxs-lookup"><span data-stu-id="bc33b-136">Under **Agreement acceptance date**, enter the appropriate date.</span></span> <span data-ttu-id="bc33b-137">Du kan inte ange ett framtida datum.</span><span class="sxs-lookup"><span data-stu-id="bc33b-137">You cannot set this to a future date.</span></span>

5. <span data-ttu-id="bc33b-138">Välj **Spara** och fortsätt.</span><span class="sxs-lookup"><span data-stu-id="bc33b-138">Select **Save** and continue.</span></span>

   :::image type="content" source="images/mcua2-update2.png" alt-text="Befintlig kund":::

### <a name="retrieve-confirmation-of-customer-acceptance"></a><span data-ttu-id="bc33b-140">Hämta bekräftelse av kund godkännande</span><span class="sxs-lookup"><span data-stu-id="bc33b-140">Retrieve confirmation of customer acceptance</span></span>

<span data-ttu-id="bc33b-141">Följ stegen nedan om du vill hämta en bekräftelse på att en befintlig kund har godkänt Microsofts kund avtal.</span><span class="sxs-lookup"><span data-stu-id="bc33b-141">To retrieve confirmation that an existing customer has accepted the Microsoft Customer Agreement, use the following steps.</span></span> <span data-ttu-id="bc33b-142">Du måste vara administratörs agent eller försäljnings agent för att göra detta.</span><span class="sxs-lookup"><span data-stu-id="bc33b-142">You must be an Admin agent or Sales agent to do this.</span></span>

1. <span data-ttu-id="bc33b-143">Välj **kunder** och leta upp och välj den kund som du vill se.</span><span class="sxs-lookup"><span data-stu-id="bc33b-143">Select **Customers**, and then find and select the customer you want to see.</span></span>

2. <span data-ttu-id="bc33b-144">Välj **konto information**.</span><span class="sxs-lookup"><span data-stu-id="bc33b-144">Select **Account info**.</span></span>

3. <span data-ttu-id="bc33b-145">Under **Microsofts kund avtal** kan du Visa om bekräftelsen har eller inte har tillhandahållits av den här kunden.</span><span class="sxs-lookup"><span data-stu-id="bc33b-145">Under **Microsoft customer agreement**, view if confirmation has or hasn't been provided by this customer.</span></span>

## <a name="confirm-customer-acceptance-using-partner-center-apisdk"></a><span data-ttu-id="bc33b-146">Bekräfta kund godkännande med partner Center API/SDK</span><span class="sxs-lookup"><span data-stu-id="bc33b-146">Confirm customer acceptance using Partner Center API/SDK</span></span>

<span data-ttu-id="bc33b-147">Du kan använda Partner Center API/SDK för att bekräfta kund godkännande av Microsofts kund avtal.</span><span class="sxs-lookup"><span data-stu-id="bc33b-147">You can use Partner Center API/SDK to confirm customer acceptance of the Microsoft Customer Agreement.</span></span> <span data-ttu-id="bc33b-148">Mer information om API/SDK finns i:</span><span class="sxs-lookup"><span data-stu-id="bc33b-148">For details on the API/SDK, refer to:</span></span>

- [<span data-ttu-id="bc33b-149">Hämta avtalsmetadata för Microsoft-kundavtalet</span><span class="sxs-lookup"><span data-stu-id="bc33b-149">Get agreement metadata for the Microsoft Customer Agreement</span></span>](/partner-center/develop/get-customer-agreement-metadata)

- [<span data-ttu-id="bc33b-150">Bekräfta kundgodkännande av Microsoft-kundavtal</span><span class="sxs-lookup"><span data-stu-id="bc33b-150">Confirm customer acceptance of Microsoft Customer Agreement</span></span>](/partner-center/develop/confirm-customer-consent-customer-agreement)

- [<span data-ttu-id="bc33b-151">Få bekräftelse på kundgodkännande av Microsoft-kundavtal</span><span class="sxs-lookup"><span data-stu-id="bc33b-151">Get confirmation of customer acceptance of Microsoft Customer Agreement</span></span>](/partner-center/develop/get-confirmation-of-customer-agreement)

- [<span data-ttu-id="bc33b-152">Hämta en nedladdnings länk för Microsofts kund avtals mall</span><span class="sxs-lookup"><span data-stu-id="bc33b-152">Get a download link for the Microsoft Customer Agreement template</span></span>](/partner-center/develop/download-customer-agreement-template)

## <a name="option-2-customer-acceptance-in-microsoft-365-admin-center"></a><span data-ttu-id="bc33b-153">Alternativ 2: kund godkännande i Microsoft 365 administrations Center</span><span class="sxs-lookup"><span data-stu-id="bc33b-153">Option 2: Customer acceptance in Microsoft 365 Admin Center</span></span>

<span data-ttu-id="bc33b-154">Partner kan bjuda in nya och befintliga kunder via en URL för att granska och godkänna avtalet i Microsoft 365 administrations centret.</span><span class="sxs-lookup"><span data-stu-id="bc33b-154">Partners can invite new and existing customers, via a URL, to review and accept the agreement within the Microsoft 365 Admin Center.</span></span> <span data-ttu-id="bc33b-155">I följande avsnitt visas hur du:</span><span class="sxs-lookup"><span data-stu-id="bc33b-155">The next few sections show you how to:</span></span>

- <span data-ttu-id="bc33b-156">Skapa en ny kund och Bjud in kunden att granska och godkänna avtalet.</span><span class="sxs-lookup"><span data-stu-id="bc33b-156">Create a new customer and invite the customer to review and accept the agreement.</span></span>

- <span data-ttu-id="bc33b-157">Bjud in en ny kund att granska och godkänna åter försäljarens relation och avtal.</span><span class="sxs-lookup"><span data-stu-id="bc33b-157">Invite a new customer to review and accept the reseller relationship and agreement.</span></span>

- <span data-ttu-id="bc33b-158">Bjud in en befintlig kund för att granska och godkänna avtalet.</span><span class="sxs-lookup"><span data-stu-id="bc33b-158">Invite an existing customer to review and accept the agreement.</span></span>

>[!NOTE]
> <span data-ttu-id="bc33b-159">Du kan använda [partner Center API/SDK](/partner-center/develop/get-direct-sign-status-of-customer-agreement) för att hämta statusen för kundens direkta godkännande av Microsofts kund avtal.</span><span class="sxs-lookup"><span data-stu-id="bc33b-159">You can use [Partner Center API/SDK](/partner-center/develop/get-direct-sign-status-of-customer-agreement) to get the status of a customer's direct acceptance of the Microsoft Customer Agreement.</span></span>  

## <a name="create-a-new-customer-and-invite-the-customer-to-review-and-accept-the-agreement"></a><span data-ttu-id="bc33b-160">Skapa en ny kund och Bjud in kunden att granska och godkänna avtalet</span><span class="sxs-lookup"><span data-stu-id="bc33b-160">Create a new customer and invite the customer to review and accept the agreement</span></span>

<span data-ttu-id="bc33b-161">Använd följande steg för att skapa en ny kund i Partner Center och sedan bjuda in dem att granska och godkänna Microsofts kund avtal i Microsoft 365 administrations Center.</span><span class="sxs-lookup"><span data-stu-id="bc33b-161">Use the following steps to create a new customer in Partner Center then invite them to review and accept the Microsoft Customer Agreement within Microsoft 365 Admin Center.</span></span>

1. <span data-ttu-id="bc33b-162">Välj **Lägg till kund** på fliken **kunder** i Partner Center.</span><span class="sxs-lookup"><span data-stu-id="bc33b-162">From the **Customers** tab within Partner Center, select **Add customer**.</span></span>

2. <span data-ttu-id="bc33b-163">Under **konto information** anger du information om den nya kunden i alla obligatoriska fält, inklusive kundens företags namn och primär kontakt.</span><span class="sxs-lookup"><span data-stu-id="bc33b-163">Under **Account Info**, enter information about the new customer in all required fields, including the customer's company name and primary contact.</span></span>

3. <span data-ttu-id="bc33b-164">Under **kund avtal** väljer **du kund för att bli ombedd att godkänna Microsofts kund avtal i Microsoft 365 administrations Center**.</span><span class="sxs-lookup"><span data-stu-id="bc33b-164">Under **Customer Agreement**, select **Customer will be asked to accept the Microsoft Customer Agreement in Microsoft 365 Admin Center**.</span></span> <span data-ttu-id="bc33b-165">Fyll i alla andra obligatoriska fält på sidan.</span><span class="sxs-lookup"><span data-stu-id="bc33b-165">Complete any other required fields on the page.</span></span>

4. <span data-ttu-id="bc33b-166">Välj **Nästa: granska** och fortsätt sedan stegen för att skapa kund klienten.</span><span class="sxs-lookup"><span data-stu-id="bc33b-166">Select **Next: Review** then continue the steps to create the customer tenant.</span></span> 

>[!NOTE] 
><span data-ttu-id="bc33b-167">Nya kunder kan inte göra ett köp förrän de accepterar Microsofts kund avtal.</span><span class="sxs-lookup"><span data-stu-id="bc33b-167">New customers cannot make a purchase until they accept the Microsoft Customer Agreement.</span></span>  

   :::image type="content" source="images/mca/create-new-customer.jpg" alt-text="Skapa ny kund":::

5. <span data-ttu-id="bc33b-169">När du når **bekräftelse** skärmen i det nya kund arbets flödet sparar du kundens autentiseringsuppgifter.</span><span class="sxs-lookup"><span data-stu-id="bc33b-169">When you reach the **Confirmation** screen in the new customer workflow, save the customer credentials.</span></span> <span data-ttu-id="bc33b-170">Du måste ange autentiseringsuppgifterna för din kund senare.</span><span class="sxs-lookup"><span data-stu-id="bc33b-170">You will need to give these credentials to your customer later.</span></span>

6. <span data-ttu-id="bc33b-171">Utanför Partner Center skapar och skickar du ett e-postmeddelande som bjuder in kunden att godkänna Microsofts kund avtal i Microsoft 365 administrations Center.</span><span class="sxs-lookup"><span data-stu-id="bc33b-171">Outside of Partner Center, create and send an email that invites the customer to accept the Microsoft Customer Agreement in Microsoft 365 Admin Center.</span></span> <span data-ttu-id="bc33b-172">Se till att ta med dessa objekt i e-postmeddelandet:</span><span class="sxs-lookup"><span data-stu-id="bc33b-172">Make sure to include these items in the email:</span></span>

   - <span data-ttu-id="bc33b-173">En länk till denna [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement) (inloggning krävs)</span><span class="sxs-lookup"><span data-stu-id="bc33b-173">A link to this [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement) (Sign-in required)</span></span>

   - <span data-ttu-id="bc33b-174">Kundens autentiseringsuppgifter som du sparade i steg 5.</span><span class="sxs-lookup"><span data-stu-id="bc33b-174">The customer's credentials that you saved in Step 5.</span></span>

7. <span data-ttu-id="bc33b-175">Kunden får sedan e-postinbjudan från partnern och välja [URL: en](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement).</span><span class="sxs-lookup"><span data-stu-id="bc33b-175">The customer will then receive the email invite from the partner and select the [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement).</span></span>

8. <span data-ttu-id="bc33b-176">Kunden loggar in i Microsoft 365 administrations Center med hjälp av de kundautentiseringsuppgifter som du har angett.</span><span class="sxs-lookup"><span data-stu-id="bc33b-176">The customer signs into Microsoft 365 Admin Center using the customer credentials you provided.</span></span>

9. <span data-ttu-id="bc33b-177">Kunden kontrollerar rutan för att godkänna Microsofts kund avtal.</span><span class="sxs-lookup"><span data-stu-id="bc33b-177">The customer checks the box to accept the Microsoft Customer agreement.</span></span>

## <a name="invite-a-new-customer-to-review-and-accept-the-reseller-relationship-and-microsoft-customer-agreement"></a><span data-ttu-id="bc33b-178">Bjud in en ny kund att granska och godkänna åter försäljarens relation och Microsofts kund avtal</span><span class="sxs-lookup"><span data-stu-id="bc33b-178">Invite a new customer to review and accept the reseller relationship and Microsoft Customer Agreement</span></span> 

<span data-ttu-id="bc33b-179">Använd följande steg för att bjuda in en ny kund att granska och godkänna åter försäljarens relation och Microsofts kund avtal.</span><span class="sxs-lookup"><span data-stu-id="bc33b-179">Use the following steps to invite a new customer to review and accept the reseller relationship and the Microsoft Customer Agreement.</span></span> 

1. <span data-ttu-id="bc33b-180">På fliken **kunder** i Partner Center väljer du **begär en åter försäljares Relations** länk.</span><span class="sxs-lookup"><span data-stu-id="bc33b-180">From the **Customers** tab within Partner Center, select **Request a reseller relationship** link.</span></span> 

2. <span data-ttu-id="bc33b-181">En mall för automatisk e-post kommer att skapas, inklusive text och en parametriserad URL som leder kunden till Microsoft 365 administrations Center.</span><span class="sxs-lookup"><span data-stu-id="bc33b-181">An automatic email template will be generated, including text and a parameterized URL that directs the customer to the Microsoft 365 Admin Center.</span></span>

3. <span data-ttu-id="bc33b-182">Du kan anpassa den automatiskt genererade e-postmallen och sedan välja **Kopiera till Urklipp** eller **Öppna i e-post**.</span><span class="sxs-lookup"><span data-stu-id="bc33b-182">You can customize the automatically generated email template and then select **Copy to clipboard** or **Open in email**.</span></span>

4. <span data-ttu-id="bc33b-183">Använd den här e-postmallen för att bjuda in kunden att acceptera **åter försäljarens Relations** förfrågan och **Microsofts kund avtal**.</span><span class="sxs-lookup"><span data-stu-id="bc33b-183">Use this email template to invite the customer to accept **reseller relationship** request and the **Microsoft Customer Agreement**.</span></span> <span data-ttu-id="bc33b-184">(Obs! i e-postinbjudanen ser du till att partnern även innehåller den URL som angavs automatiskt samt de autentiseringsuppgifter för kunden som nyligen har skapats.)</span><span class="sxs-lookup"><span data-stu-id="bc33b-184">(Note: In the email invite, make sure the partner also includes the URL that was automatically provided as well as the customer credentials that were recently created.)</span></span>

   :::image type="content" source="images/mca/createrelationship.png" alt-text="skapa en relation":::

5. <span data-ttu-id="bc33b-186">Kunden tar emot inbjudan via e-post och klickar på URL: en för parametern.</span><span class="sxs-lookup"><span data-stu-id="bc33b-186">Customer receives invite via email and clicks on the parameterized URL.</span></span> 

6. <span data-ttu-id="bc33b-187">Kunden använder autentiseringsuppgifter som du anger i e-postmeddelandet för att logga in på Microsoft 365 administrations Center.</span><span class="sxs-lookup"><span data-stu-id="bc33b-187">Customer uses credentials you provide within email to sign into Microsoft 365 Admin Center.</span></span>

7. <span data-ttu-id="bc33b-188">Kunden kontrollerar rutan för att godkänna **åter försäljarens relation** och **Microsofts kund avtal**.</span><span class="sxs-lookup"><span data-stu-id="bc33b-188">Customer checks the box to accept the **reseller relationship** and **Microsoft Customer Agreement**.</span></span> 

8. <span data-ttu-id="bc33b-189">Inom samma URL kan kunden se en lista över olika partners som de arbetar med.</span><span class="sxs-lookup"><span data-stu-id="bc33b-189">Within the same URL, the customer is able to see a consolidated list of different partners they are working with.</span></span> <span data-ttu-id="bc33b-190">De kan välja en partner för att se information.</span><span class="sxs-lookup"><span data-stu-id="bc33b-190">They can select a partner to see details.</span></span>

   :::image type="content" source="images/mca/accept.jpg" alt-text="Godkänna avtal":::


## <a name="invite-an-existing-customer-to-review-and-accept-the-agreement"></a><span data-ttu-id="bc33b-192">Bjud in en befintlig kund för att granska och godkänna avtalet</span><span class="sxs-lookup"><span data-stu-id="bc33b-192">Invite an existing customer to review and accept the agreement</span></span>

<span data-ttu-id="bc33b-193">Använd följande steg för att bjuda in en befintlig kund att granska och godkänna Microsofts kund avtal.</span><span class="sxs-lookup"><span data-stu-id="bc33b-193">Use the following steps to invite an existing customer to review and accept the Microsoft Customer Agreement.</span></span> 

1. <span data-ttu-id="bc33b-194">Skapa kund-e-postmeddelandet med den inbäddade URL: en som bjuder in kunden att godkänna Microsofts kund avtal.</span><span class="sxs-lookup"><span data-stu-id="bc33b-194">Create the customer email with the embedded URL inviting your customer to accept the Microsoft Customer Agreement.</span></span>

2. <span data-ttu-id="bc33b-195">Kunden får inbjudan via e-post och klickar på [URL: en](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement).</span><span class="sxs-lookup"><span data-stu-id="bc33b-195">Your customer receives the invitation via email and clicks the [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement).</span></span> 

3. <span data-ttu-id="bc33b-196">Kunden anger sina autentiseringsuppgifter i Microsoft 365 administrations Center.</span><span class="sxs-lookup"><span data-stu-id="bc33b-196">The customer enters their credentials into Microsoft 365 Admin Center.</span></span>

4. <span data-ttu-id="bc33b-197">Kunden söker i rutan om att godkänna Microsofts kund avtal.</span><span class="sxs-lookup"><span data-stu-id="bc33b-197">Your customer checks the box to accept the Microsoft Customer Agreement.</span></span> 

5. <span data-ttu-id="bc33b-198">I samma URL kan kunden se den konsoliderade listan över olika partners som de arbetar med.</span><span class="sxs-lookup"><span data-stu-id="bc33b-198">Within the same URL, the customer can see the consolidated list of different partners they are working with.</span></span> <span data-ttu-id="bc33b-199">De kan välja en partner för att se information.</span><span class="sxs-lookup"><span data-stu-id="bc33b-199">They can select a partner to see details.</span></span>

   :::image type="content" source="images/mca/customeraccept.png" alt-text="kund":::

>[!NOTE]
><span data-ttu-id="bc33b-201">I vissa fall kanske kunderna inte kan acceptera Microsofts kund avtal direkt.</span><span class="sxs-lookup"><span data-stu-id="bc33b-201">In certain scenarios, customers may not be able to directly accept the Microsoft Customer Agreement.</span></span> <span data-ttu-id="bc33b-202">Läs mer om dessa situationer i två scenarier där du behöver intyga för kundens räkning, nedan.</span><span class="sxs-lookup"><span data-stu-id="bc33b-202">To learn more about these situations, read Two scenarios where you need to attest on behalf of your customer, below.</span></span>

## <a name="two-scenarios-where-you-need-to-attest-on-behalf-of-your-customer"></a><span data-ttu-id="bc33b-203">Två scenarier där du behöver intyga för kundens räkning</span><span class="sxs-lookup"><span data-stu-id="bc33b-203">Two scenarios where you need to attest on behalf of your customer</span></span>

<span data-ttu-id="bc33b-204">Det finns två scenarier där kunder kanske inte kan acceptera Microsofts kund avtal direkt i Microsoft 365 administrations Center.</span><span class="sxs-lookup"><span data-stu-id="bc33b-204">There are two scenarios where customers may not be able to directly accept the Microsoft Customer Agreement within the Microsoft 365 Admin Center.</span></span>

<span data-ttu-id="bc33b-205">**Scenario 1**: en befintlig kund har köpt något av följande via en befintlig partner relation: erbjudanden, program vara eller program vara, reserverade instanser eller Azure-abonnemang.</span><span class="sxs-lookup"><span data-stu-id="bc33b-205">**Scenario 1**: An existing customer has purchased any of the following through an existing partner relationship: offers, software or software subscriptions, Reserved Instances, or Azure Plan.</span></span> <span data-ttu-id="bc33b-206">Kunden försöker nu att göra ett nytt köp (exklusive automatisk förnyelse).</span><span class="sxs-lookup"><span data-stu-id="bc33b-206">The customer is now attempting to make any new purchase (excluding auto renewal).</span></span> <span data-ttu-id="bc33b-207">När kunden klickar på webb adressen visas meddelandet "kontakta din partner för att bekräfta ditt godkännande av Microsofts kund avtal."</span><span class="sxs-lookup"><span data-stu-id="bc33b-207">When that customer clicks the URL, they will receive the message "Please reach out to your Partner to confirm your acceptance of the Microsoft Customer Agreement."</span></span>  

<span data-ttu-id="bc33b-208">**För att lösa**: du måste attestera för kundens räkning.</span><span class="sxs-lookup"><span data-stu-id="bc33b-208">**To resolve**: You must attest on behalf of the customer.</span></span>

:::image type="content" source="images/mca/accept-scenario-1.png" alt-text="Skärm bild av sidan Microsoft 365 administrations Center där du uppmanas att kontakta din partner för att bekräfta godkännande av Microsofts kund avtal.":::

<span data-ttu-id="bc33b-210">**Scenario 2**: en befintlig kund har köpt någon av följande erbjudanden, program-och program varu prenumerationer, reserverade instanser och Azure-abonnemang.</span><span class="sxs-lookup"><span data-stu-id="bc33b-210">**Scenario 2**: An existing customer has purchased any of the following offers, software and software subscriptions, Reserved Instances, and Azure Plan.</span></span> <span data-ttu-id="bc33b-211">Kunden försöker nu att göra ett nytt köp med en ny partner.</span><span class="sxs-lookup"><span data-stu-id="bc33b-211">The customer is now attempting to make any new purchase with a new partner.</span></span>

<span data-ttu-id="bc33b-212">När kunden klickar på URL: en för att Microsoft 365 administrations Center för att godkänna den nya partner relationen och avtalet, får han eller hon meddelandet "kontakta din partner för att bekräfta ditt godkännande av Microsofts kund avtal."</span><span class="sxs-lookup"><span data-stu-id="bc33b-212">When the customer clicks the URL to Microsoft 365 Admin Center to accept the new partner relationship and the agreement, they will receive the message "Please reach out to your Partner to confirm your acceptance of the Microsoft Customer Agreement."</span></span>  

<span data-ttu-id="bc33b-213">**För att lösa**: du måste attestera för kundens räkning.</span><span class="sxs-lookup"><span data-stu-id="bc33b-213">**To resolve**: You must attest on behalf of the customer.</span></span>  

## <a name="confirm-that-a-customer-has-accepted-the-agreement"></a><span data-ttu-id="bc33b-214">Bekräfta att en kund har godkänt avtalet</span><span class="sxs-lookup"><span data-stu-id="bc33b-214">Confirm that a customer has accepted the agreement</span></span>

<span data-ttu-id="bc33b-215">Om du försöker skapa en ny order för en befintlig kund som du inte har bekräftat tidigare får du ett meddelande om att slutföra bekräftelsen.</span><span class="sxs-lookup"><span data-stu-id="bc33b-215">If you try to create a new order for an existing customer who you have not confirmed before, you'll receive a prompt to complete the confirmation.</span></span> <span data-ttu-id="bc33b-216">Använd följande procedur för att göra detta.</span><span class="sxs-lookup"><span data-stu-id="bc33b-216">Use the following procedure to do this.</span></span>

1. <span data-ttu-id="bc33b-217">Ange **förnamn**, **efter namn**, **e-postadress** och **telefonnummer** (valfritt) för den användare som har godkänt avtalet.</span><span class="sxs-lookup"><span data-stu-id="bc33b-217">Enter the **First name**, **Last name**, **Email address**, and **Phone number** (optional) of the user who accepted the agreement.</span></span>

2. <span data-ttu-id="bc33b-218">Ange ett datum under **avtalets godkännande datum**.</span><span class="sxs-lookup"><span data-stu-id="bc33b-218">Under **Agreement acceptance date**, enter the appropriate date.</span></span> <span data-ttu-id="bc33b-219">Du kan inte ange ett framtida datum.</span><span class="sxs-lookup"><span data-stu-id="bc33b-219">You cannot set this to a future date.</span></span>

3. <span data-ttu-id="bc33b-220">Välj **Spara och fortsätt**.</span><span class="sxs-lookup"><span data-stu-id="bc33b-220">Select **Save and continue**.</span></span> 

## <a name="next-steps"></a><span data-ttu-id="bc33b-221">Nästa steg</span><span class="sxs-lookup"><span data-stu-id="bc33b-221">Next steps</span></span>

- [<span data-ttu-id="bc33b-222">Verifiera eller uppdatera företagets profil information</span><span class="sxs-lookup"><span data-stu-id="bc33b-222">Verify or update your company profile information</span></span>](update-your-partner-profile.md)
- [<span data-ttu-id="bc33b-223">Microsoft-kundavtal (efter region, språk)</span><span class="sxs-lookup"><span data-stu-id="bc33b-223">Microsoft Customer Agreements (by region, language)</span></span>](Agreements.md)
