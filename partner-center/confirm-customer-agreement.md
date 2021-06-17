---
title: Så här bekräftar du att kunden har godkänt Microsoft-kundavtal till CSP-programmet
description: Molnlösningsleverantör (CSP)-partner måste bekräfta kundens godkännande av Microsoft-kundavtal innan de beställer Microsoft-tjänster för kunder.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: aarzh-AaronZhang
ms.author: v-aarzh
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.date: 03/24/2021
ms.openlocfilehash: 9deebf3d9aab2d4dc7953da67a7eb17078b3d30c
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/17/2021
ms.locfileid: "112277019"
---
# <a name="how-to-confirm-that-your-customer-has-accepted-the-microsoft-customer-agreement-to-the-csp-program"></a><span data-ttu-id="28a82-103">Så här bekräftar du att kunden har godkänt Microsoft-kundavtal till CSP-programmet</span><span class="sxs-lookup"><span data-stu-id="28a82-103">How to confirm that your customer has accepted the Microsoft Customer Agreement to the CSP program</span></span>

<span data-ttu-id="28a82-104">**Lämpliga roller:** Administratörsagent | Försäljningsagent</span><span class="sxs-lookup"><span data-stu-id="28a82-104">**Appropriate roles**: Admin agent | Sales agent</span></span>


<span data-ttu-id="28a82-105">Kunder har två alternativ för hur de accepterar Microsoft-kundavtal.</span><span class="sxs-lookup"><span data-stu-id="28a82-105">Customers have two options for how they accept the Microsoft Customer Agreement.</span></span>

<span data-ttu-id="28a82-106">**Alternativ 1:** Partner attestation av kundgodkännande – Partner kan bekräfta kundens godkännande via Partner Center API/SDK eller via instrumentpanelen i Partnercenter.</span><span class="sxs-lookup"><span data-stu-id="28a82-106">**Option 1**: Partner attestation of customer acceptance - Partner can confirm customer acceptance using Partner Center API/SDK or through the Partner Center dashboard.</span></span>

<span data-ttu-id="28a82-107">**Alternativ 2:** Direkt godkännande av kund – Partner kan bjuda in kunden via en URL för att granska och godkänna avtalet i Microsoft 365 Administrationscenter.</span><span class="sxs-lookup"><span data-stu-id="28a82-107">**Option 2**: Customer direct acceptance - Partner can invite the customer via a URL to review and accept the agreement in the Microsoft 365 Admin Center.</span></span>

## <a name="access-microsoft-customer-agreement-template"></a><span data-ttu-id="28a82-108">Åtkomst Microsoft-kundavtal mall</span><span class="sxs-lookup"><span data-stu-id="28a82-108">Access Microsoft Customer Agreement template</span></span>

<span data-ttu-id="28a82-109">Du kan ladda ned den senaste versionen av Microsoft-kundavtal [här.](https://aka.ms/customeragreement)</span><span class="sxs-lookup"><span data-stu-id="28a82-109">You can manually download the latest version of the Microsoft Customer Agreement template from [here](https://aka.ms/customeragreement).</span></span> <span data-ttu-id="28a82-110">Den Microsoft-kundavtal är landsspecifik.</span><span class="sxs-lookup"><span data-stu-id="28a82-110">The Microsoft Customer Agreement is country-specific.</span></span> <span data-ttu-id="28a82-111">När du Microsoft-kundavtal mallen måste du välja rätt land baserat på kundens plats.</span><span class="sxs-lookup"><span data-stu-id="28a82-111">When requesting the Microsoft Customer Agreement template, be sure to select the correct country based on the customer's location.</span></span>

## <a name="option-1-confirm-customer-acceptance-in-partner-center"></a><span data-ttu-id="28a82-112">Alternativ 1: Bekräfta kundens godkännande i Partnercenter</span><span class="sxs-lookup"><span data-stu-id="28a82-112">Option 1: Confirm customer acceptance in Partner Center</span></span>

<span data-ttu-id="28a82-113">Direktfaktureringspartner kan bekräfta att kunden godkänner Microsoft-kundavtal i Partnercenter för nya och befintliga kunder.</span><span class="sxs-lookup"><span data-stu-id="28a82-113">Direct bill partners can confirm customer acceptance of the Microsoft Customer Agreement in Partner Center for new and existing customers.</span></span> <span data-ttu-id="28a82-114">Indirekta återförsäljare kan inte intyga för sina kunders räkning och behöver samarbeta med sin indirekta leverantör för att slutföra attestering.</span><span class="sxs-lookup"><span data-stu-id="28a82-114">Indirect resellers cannot attest on behalf of their customers and need to work with their Indirect Provider to get attestation completed.</span></span>

### <a name="confirm-customer-acceptance-for-new-customers"></a><span data-ttu-id="28a82-115">Bekräfta kundens godkännande för nya kunder</span><span class="sxs-lookup"><span data-stu-id="28a82-115">Confirm customer acceptance for new customers</span></span>

<span data-ttu-id="28a82-116">När du skapar en ny kundklientorganisation i Partnercenter använder du följande steg för att bekräfta kundens godkännande av Microsoft-kundavtal.</span><span class="sxs-lookup"><span data-stu-id="28a82-116">When you create a new customer tenant in Partner Center, use the following steps to confirm the customer's acceptance of the Microsoft Customer Agreement.</span></span> <span data-ttu-id="28a82-117">Du måste vara administratörsagent eller försäljningsagent för att utföra de här stegen.</span><span class="sxs-lookup"><span data-stu-id="28a82-117">You must be an Admin agent or Sales agent to perform these steps.</span></span>

1. <span data-ttu-id="28a82-118">Välj **Kunder** och sedan **Ny kund.**</span><span class="sxs-lookup"><span data-stu-id="28a82-118">Select **Customers**, and then **New customer**.</span></span>

2. <span data-ttu-id="28a82-119">Under **Kontoinformation** anger du information för företaget och dess primära kontakt.</span><span class="sxs-lookup"><span data-stu-id="28a82-119">Under **Account info**, enter information for the company and its primary contact.</span></span>

3. <span data-ttu-id="28a82-120">Under **Microsoft-avtal** markerar du rutan för att intyga att kunden har accepterat Microsoft-kundavtal.</span><span class="sxs-lookup"><span data-stu-id="28a82-120">Under **Microsoft agreement**, select the box to attest that the customer has accepted the Microsoft Customer Agreement.</span></span>

4. <span data-ttu-id="28a82-121">Under **Godkännandedatum för avtalet** anger du lämpligt datum.</span><span class="sxs-lookup"><span data-stu-id="28a82-121">Under **Agreement acceptance date**, enter the appropriate date.</span></span> <span data-ttu-id="28a82-122">Du kan inte ange detta till ett framtida datum.</span><span class="sxs-lookup"><span data-stu-id="28a82-122">You cannot set this to a future date.</span></span>

5. <span data-ttu-id="28a82-123">Kontrollera att den primära användarens kontaktuppgifter visas korrekt.</span><span class="sxs-lookup"><span data-stu-id="28a82-123">Make sure that the primary user contact information displayed is correct.</span></span> <span data-ttu-id="28a82-124">Om det är felaktigt väljer du **Uppdatera** och anger korrekt information för den person som godkände avtalet.</span><span class="sxs-lookup"><span data-stu-id="28a82-124">If it's incorrect, select **Update** and enter the accurate information for the person who accepted the agreement.</span></span>

6. <span data-ttu-id="28a82-125">Välj **Nästa för** att fortsätta att skapa kundklientorganisationen.</span><span class="sxs-lookup"><span data-stu-id="28a82-125">Select **Next** to continue creating the customer tenant.</span></span>

   :::image type="content" source="images/mca/newcustomeragreement.jpg" alt-text="Ny kund.":::  

### <a name="confirm-customer-acceptance-for-existing-customers"></a><span data-ttu-id="28a82-127">Bekräfta kundgodkännande för befintliga kunder</span><span class="sxs-lookup"><span data-stu-id="28a82-127">Confirm customer acceptance for existing customers</span></span>

<span data-ttu-id="28a82-128">Du måste vara administratörsagent eller försäljningsagent för att göra detta:</span><span class="sxs-lookup"><span data-stu-id="28a82-128">You must be an Admin agent or Sales agent to do this:</span></span>

1. <span data-ttu-id="28a82-129">Välj **Kunder**.</span><span class="sxs-lookup"><span data-stu-id="28a82-129">Select **Customers**.</span></span> <span data-ttu-id="28a82-130">Leta upp och välj kunden.</span><span class="sxs-lookup"><span data-stu-id="28a82-130">Find and select the customer.</span></span>

2. <span data-ttu-id="28a82-131">Välj **Kontoinformation.**</span><span class="sxs-lookup"><span data-stu-id="28a82-131">Select **Account info**.</span></span>

3. <span data-ttu-id="28a82-132">Under **Microsoft-kundavtal** väljer du **Uppdatera**.</span><span class="sxs-lookup"><span data-stu-id="28a82-132">Under **Microsoft Customer Agreement**, select **Update**.</span></span>

4. <span data-ttu-id="28a82-133">Ange **förnamn,** **efternamn,** **e-postadress** och **telefonnummer (valfritt)** för den person som godkände avtalet.</span><span class="sxs-lookup"><span data-stu-id="28a82-133">Enter the **First name**, **Last name**, **Email address**, and **Phone number** (optional) of the person who accepted the agreement.</span></span> <span data-ttu-id="28a82-134">Under **Godkännandedatum för avtalet** anger du lämpligt datum.</span><span class="sxs-lookup"><span data-stu-id="28a82-134">Under **Agreement acceptance date**, enter the appropriate date.</span></span> <span data-ttu-id="28a82-135">Du kan inte ange detta till ett framtida datum.</span><span class="sxs-lookup"><span data-stu-id="28a82-135">You cannot set this to a future date.</span></span>

5. <span data-ttu-id="28a82-136">Välj **Spara** och fortsätt.</span><span class="sxs-lookup"><span data-stu-id="28a82-136">Select **Save** and continue.</span></span>

   :::image type="content" source="images/mcua2-update2.png" alt-text="Befintlig kund.":::

### <a name="retrieve-confirmation-of-customer-acceptance"></a><span data-ttu-id="28a82-138">Hämta bekräftelse av kundgodkännande</span><span class="sxs-lookup"><span data-stu-id="28a82-138">Retrieve confirmation of customer acceptance</span></span>

<span data-ttu-id="28a82-139">Använd följande steg för att hämta en bekräftelse Microsoft-kundavtal en befintlig kund har accepterat Microsoft-kundavtal.</span><span class="sxs-lookup"><span data-stu-id="28a82-139">To retrieve confirmation that an existing customer has accepted the Microsoft Customer Agreement, use the following steps.</span></span> <span data-ttu-id="28a82-140">Du måste vara administratörsagent eller försäljningsagent för att göra detta.</span><span class="sxs-lookup"><span data-stu-id="28a82-140">You must be an Admin agent or Sales agent to do this.</span></span>

1. <span data-ttu-id="28a82-141">Välj **Kunder** och leta upp och välj sedan den kund som du vill se.</span><span class="sxs-lookup"><span data-stu-id="28a82-141">Select **Customers**, and then find and select the customer you want to see.</span></span>

2. <span data-ttu-id="28a82-142">Välj **Kontoinformation.**</span><span class="sxs-lookup"><span data-stu-id="28a82-142">Select **Account info**.</span></span>

3. <span data-ttu-id="28a82-143">Under **Microsoft-kundavtal** visar du om en bekräftelse har eller inte har tillhandahållits av den här kunden.</span><span class="sxs-lookup"><span data-stu-id="28a82-143">Under **Microsoft customer agreement**, view if confirmation has or hasn't been provided by this customer.</span></span>

## <a name="confirm-customer-acceptance-using-partner-center-apisdk"></a><span data-ttu-id="28a82-144">Bekräfta kundgodkännande med partnercenter-API/SDK</span><span class="sxs-lookup"><span data-stu-id="28a82-144">Confirm customer acceptance using Partner Center API/SDK</span></span>

<span data-ttu-id="28a82-145">Du kan använda Partner Center API/SDK för att bekräfta kundens godkännande av Microsoft-kundavtal.</span><span class="sxs-lookup"><span data-stu-id="28a82-145">You can use Partner Center API/SDK to confirm customer acceptance of the Microsoft Customer Agreement.</span></span> <span data-ttu-id="28a82-146">Mer information om API/SDK finns i:</span><span class="sxs-lookup"><span data-stu-id="28a82-146">For details on the API/SDK, refer to:</span></span>

- [<span data-ttu-id="28a82-147">Hämta avtalsmetadata för Microsoft-kundavtalet</span><span class="sxs-lookup"><span data-stu-id="28a82-147">Get agreement metadata for the Microsoft Customer Agreement</span></span>](/partner-center/develop/get-customer-agreement-metadata)

- [<span data-ttu-id="28a82-148">Bekräfta kundgodkännande av Microsoft-kundavtal</span><span class="sxs-lookup"><span data-stu-id="28a82-148">Confirm customer acceptance of Microsoft Customer Agreement</span></span>](/partner-center/develop/confirm-customer-consent-customer-agreement)

- [<span data-ttu-id="28a82-149">Få bekräftelse på kundgodkännande av Microsoft-kundavtal</span><span class="sxs-lookup"><span data-stu-id="28a82-149">Get confirmation of customer acceptance of Microsoft Customer Agreement</span></span>](/partner-center/develop/get-confirmation-of-customer-agreement)

- [<span data-ttu-id="28a82-150">Hämta en nedladdningslänk för Microsoft-kundavtal mallen</span><span class="sxs-lookup"><span data-stu-id="28a82-150">Get a download link for the Microsoft Customer Agreement template</span></span>](/partner-center/develop/download-customer-agreement-template)

## <a name="option-2-customer-acceptance-in-microsoft-365-admin-center"></a><span data-ttu-id="28a82-151">Alternativ 2: Kundgodkännande i Microsoft 365 Administrationscenter</span><span class="sxs-lookup"><span data-stu-id="28a82-151">Option 2: Customer acceptance in Microsoft 365 Admin Center</span></span>

<span data-ttu-id="28a82-152">Partner kan bjuda in nya och befintliga kunder via en URL för att granska och godkänna avtalet i Microsoft 365 administrationscentret.</span><span class="sxs-lookup"><span data-stu-id="28a82-152">Partners can invite new and existing customers, via a URL, to review and accept the agreement within the Microsoft 365 Admin Center.</span></span> <span data-ttu-id="28a82-153">I följande avsnitt visas hur du:</span><span class="sxs-lookup"><span data-stu-id="28a82-153">The next few sections show you how to:</span></span>

- <span data-ttu-id="28a82-154">Skapa en ny kund och bjud in kunden att granska och godkänna avtalet.</span><span class="sxs-lookup"><span data-stu-id="28a82-154">Create a new customer and invite the customer to review and accept the agreement.</span></span>

- <span data-ttu-id="28a82-155">Bjud in en ny kund att granska och godkänna återförsäljarrelationen och avtalet.</span><span class="sxs-lookup"><span data-stu-id="28a82-155">Invite a new customer to review and accept the reseller relationship and agreement.</span></span>

- <span data-ttu-id="28a82-156">Bjud in en befintlig kund att granska och godkänna avtalet.</span><span class="sxs-lookup"><span data-stu-id="28a82-156">Invite an existing customer to review and accept the agreement.</span></span>

>[!NOTE]
> <span data-ttu-id="28a82-157">Du kan använda [Partner Center API/SDK](/partner-center/develop/get-direct-sign-status-of-customer-agreement) för att få status för en kunds direkta godkännande av Microsoft-kundavtal.</span><span class="sxs-lookup"><span data-stu-id="28a82-157">You can use [Partner Center API/SDK](/partner-center/develop/get-direct-sign-status-of-customer-agreement) to get the status of a customer's direct acceptance of the Microsoft Customer Agreement.</span></span>  

## <a name="create-a-new-customer-and-invite-the-customer-to-review-and-accept-the-agreement"></a><span data-ttu-id="28a82-158">Skapa en ny kund och bjud in kunden att granska och godkänna avtalet</span><span class="sxs-lookup"><span data-stu-id="28a82-158">Create a new customer and invite the customer to review and accept the agreement</span></span>

<span data-ttu-id="28a82-159">Använd följande steg för att skapa en ny kund i Partnercenter och sedan bjuda in dem att granska och godkänna Microsoft-kundavtal i Microsoft 365 Administrationscenter.</span><span class="sxs-lookup"><span data-stu-id="28a82-159">Use the following steps to create a new customer in Partner Center then invite them to review and accept the Microsoft Customer Agreement within Microsoft 365 Admin Center.</span></span>

1. <span data-ttu-id="28a82-160">På fliken **Kunder** i Partnercenter väljer du Lägg **till kund.**</span><span class="sxs-lookup"><span data-stu-id="28a82-160">From the **Customers** tab within Partner Center, select **Add customer**.</span></span>

2. <span data-ttu-id="28a82-161">Under **Kontoinformation** anger du information om den nya kunden i alla obligatoriska fält, inklusive kundens företagsnamn och primära kontakt.</span><span class="sxs-lookup"><span data-stu-id="28a82-161">Under **Account Info**, enter information about the new customer in all required fields, including the customer's company name and primary contact.</span></span>

3. <span data-ttu-id="28a82-162">Under **Kundavtal** väljer **du Customer will be to accept the Microsoft-kundavtal in Microsoft 365 Admin Center**.</span><span class="sxs-lookup"><span data-stu-id="28a82-162">Under **Customer Agreement**, select **Customer will be asked to accept the Microsoft Customer Agreement in Microsoft 365 Admin Center**.</span></span> <span data-ttu-id="28a82-163">Fyll i alla andra obligatoriska fält på sidan.</span><span class="sxs-lookup"><span data-stu-id="28a82-163">Complete any other required fields on the page.</span></span>

4. <span data-ttu-id="28a82-164">Välj **Nästa: Granska och** fortsätt sedan stegen för att skapa kundklientorganisationen.</span><span class="sxs-lookup"><span data-stu-id="28a82-164">Select **Next: Review** then continue the steps to create the customer tenant.</span></span> 

>[!NOTE] 
><span data-ttu-id="28a82-165">Nya kunder kan inte göra ett köp förrän de accepterar Microsoft-kundavtal.</span><span class="sxs-lookup"><span data-stu-id="28a82-165">New customers cannot make a purchase until they accept the Microsoft Customer Agreement.</span></span>  

   :::image type="content" source="images/mca/create-new-customer.jpg" alt-text="Skapa en ny kund.":::

5. <span data-ttu-id="28a82-167">När du når **bekräftelseskärmen i** det nya kundarbetsflödet sparar du kundens autentiseringsuppgifter.</span><span class="sxs-lookup"><span data-stu-id="28a82-167">When you reach the **Confirmation** screen in the new customer workflow, save the customer credentials.</span></span> <span data-ttu-id="28a82-168">Du måste ge dessa autentiseringsuppgifter till kunden senare.</span><span class="sxs-lookup"><span data-stu-id="28a82-168">You will need to give these credentials to your customer later.</span></span>

6. <span data-ttu-id="28a82-169">Utanför Partnercenter skapar och skickar du ett e-postmeddelande som uppmanar kunden att godkänna Microsoft-kundavtal i Microsoft 365 Administrationscenter.</span><span class="sxs-lookup"><span data-stu-id="28a82-169">Outside of Partner Center, create and send an email that invites the customer to accept the Microsoft Customer Agreement in Microsoft 365 Admin Center.</span></span> <span data-ttu-id="28a82-170">Se till att inkludera dessa objekt i e-postmeddelandet:</span><span class="sxs-lookup"><span data-stu-id="28a82-170">Make sure to include these items in the email:</span></span>

   - <span data-ttu-id="28a82-171">En länk till [den här URL:en](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement) (inloggning krävs)</span><span class="sxs-lookup"><span data-stu-id="28a82-171">A link to this [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement) (Sign-in required)</span></span>

   - <span data-ttu-id="28a82-172">Kundens autentiseringsuppgifter som du sparade i steg 5.</span><span class="sxs-lookup"><span data-stu-id="28a82-172">The customer's credentials that you saved in Step 5.</span></span>

7. <span data-ttu-id="28a82-173">Kunden får sedan e-post inbjudning från partnern och väljer [URL:en](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement).</span><span class="sxs-lookup"><span data-stu-id="28a82-173">The customer will then receive the email invite from the partner and select the [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement).</span></span>

8. <span data-ttu-id="28a82-174">Kunden loggar in på Microsoft 365-administrationscentret med de kundautentiseringsuppgifter som du angav.</span><span class="sxs-lookup"><span data-stu-id="28a82-174">The customer signs into Microsoft 365 Admin Center using the customer credentials you provided.</span></span>

9. <span data-ttu-id="28a82-175">Kunden kontrollerar kryssrutan för att godkänna Microsoft-kundavtalet.</span><span class="sxs-lookup"><span data-stu-id="28a82-175">The customer checks the box to accept the Microsoft Customer agreement.</span></span>

## <a name="invite-a-new-customer-to-review-and-accept-the-reseller-relationship-and-microsoft-customer-agreement"></a><span data-ttu-id="28a82-176">Bjud in en ny kund att granska och godkänna återförsäljarrelationen och Microsoft-kundavtal</span><span class="sxs-lookup"><span data-stu-id="28a82-176">Invite a new customer to review and accept the reseller relationship and Microsoft Customer Agreement</span></span> 

<span data-ttu-id="28a82-177">Använd följande steg för att bjuda in en ny kund att granska och godkänna återförsäljarrelationen och Microsoft-kundavtal.</span><span class="sxs-lookup"><span data-stu-id="28a82-177">Use the following steps to invite a new customer to review and accept the reseller relationship and the Microsoft Customer Agreement.</span></span> 

1. <span data-ttu-id="28a82-178">På fliken **Kunder** i Partnercenter väljer du Länken **Begär en återförsäljarrelation.**</span><span class="sxs-lookup"><span data-stu-id="28a82-178">From the **Customers** tab within Partner Center, select **Request a reseller relationship** link.</span></span> 

2. <span data-ttu-id="28a82-179">En automatisk e-postmall genereras, inklusive text och en parametriserad URL som dirigerar kunden Microsoft 365 administrationscentret.</span><span class="sxs-lookup"><span data-stu-id="28a82-179">An automatic email template will be generated, including text and a parameterized URL that directs the customer to the Microsoft 365 Admin Center.</span></span>

3. <span data-ttu-id="28a82-180">Du kan anpassa den automatiskt genererade e-postmallen och sedan välja **Kopiera till Urklipp eller** Öppna i **e-post**.</span><span class="sxs-lookup"><span data-stu-id="28a82-180">You can customize the automatically generated email template and then select **Copy to clipboard** or **Open in email**.</span></span>

4. <span data-ttu-id="28a82-181">Använd den här e-postmallen för att bjuda in kunden **att** godkänna begäran om återförsäljarrelation och **Microsoft-kundavtal**.</span><span class="sxs-lookup"><span data-stu-id="28a82-181">Use this email template to invite the customer to accept **reseller relationship** request and the **Microsoft Customer Agreement**.</span></span> <span data-ttu-id="28a82-182">(Obs! I e-postbjudan kontrollerar du att partnern även innehåller den URL som angavs automatiskt samt de kundautentiseringsuppgifter som nyligen skapades.)</span><span class="sxs-lookup"><span data-stu-id="28a82-182">(Note: In the email invite, make sure the partner also includes the URL that was automatically provided as well as the customer credentials that were recently created.)</span></span>

   :::image type="content" source="images/mca/createrelationship.png" alt-text="skapa en relation.":::

5. <span data-ttu-id="28a82-184">Kunden får inbjudan via e-post och klickar på den parametriserade URL:en.</span><span class="sxs-lookup"><span data-stu-id="28a82-184">Customer receives invite via email and clicks on the parameterized URL.</span></span> 

6. <span data-ttu-id="28a82-185">Kunden använder autentiseringsuppgifter som du anger i e-postmeddelandet för att logga Microsoft 365 administrationscentret.</span><span class="sxs-lookup"><span data-stu-id="28a82-185">Customer uses credentials you provide within email to sign into Microsoft 365 Admin Center.</span></span>

7. <span data-ttu-id="28a82-186">Kunden kontrollerar kryssrutan för att godkänna **återförsäljarrelationen** och **Microsoft-kundavtal**.</span><span class="sxs-lookup"><span data-stu-id="28a82-186">Customer checks the box to accept the **reseller relationship** and **Microsoft Customer Agreement**.</span></span> 

8. <span data-ttu-id="28a82-187">Inom samma URL kan kunden se en samlad lista över olika partner som de arbetar med.</span><span class="sxs-lookup"><span data-stu-id="28a82-187">Within the same URL, the customer is able to see a consolidated list of different partners they are working with.</span></span> <span data-ttu-id="28a82-188">De kan välja en partner för att se information.</span><span class="sxs-lookup"><span data-stu-id="28a82-188">They can select a partner to see details.</span></span>

   :::image type="content" source="images/mca/accept.jpg" alt-text="Godkänn avtalet.":::


## <a name="invite-an-existing-customer-to-review-and-accept-the-agreement"></a><span data-ttu-id="28a82-190">Bjud in en befintlig kund att granska och godkänna avtalet</span><span class="sxs-lookup"><span data-stu-id="28a82-190">Invite an existing customer to review and accept the agreement</span></span>

<span data-ttu-id="28a82-191">Använd följande steg för att bjuda in en befintlig kund att granska och godkänna Microsoft-kundavtal.</span><span class="sxs-lookup"><span data-stu-id="28a82-191">Use the following steps to invite an existing customer to review and accept the Microsoft Customer Agreement.</span></span> 

1. <span data-ttu-id="28a82-192">Skapa kundens e-postadress med den inbäddade URL:en som uppmanar kunden att godkänna Microsoft-kundavtal.</span><span class="sxs-lookup"><span data-stu-id="28a82-192">Create the customer email with the embedded URL inviting your customer to accept the Microsoft Customer Agreement.</span></span>

2. <span data-ttu-id="28a82-193">Kunden får inbjudan via e-post och klickar på [URL:en](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement).</span><span class="sxs-lookup"><span data-stu-id="28a82-193">Your customer receives the invitation via email and clicks the [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement).</span></span> 

3. <span data-ttu-id="28a82-194">Kunden anger sina autentiseringsuppgifter i Microsoft 365 Administrationscenter.</span><span class="sxs-lookup"><span data-stu-id="28a82-194">The customer enters their credentials into Microsoft 365 Admin Center.</span></span>

4. <span data-ttu-id="28a82-195">Kunden kontrollerar rutan för att godkänna Microsoft-kundavtal.</span><span class="sxs-lookup"><span data-stu-id="28a82-195">Your customer checks the box to accept the Microsoft Customer Agreement.</span></span> 

5. <span data-ttu-id="28a82-196">Inom samma URL kan kunden se den konsoliderade listan över olika partner som de arbetar med.</span><span class="sxs-lookup"><span data-stu-id="28a82-196">Within the same URL, the customer can see the consolidated list of different partners they are working with.</span></span> <span data-ttu-id="28a82-197">De kan välja en partner för att se information.</span><span class="sxs-lookup"><span data-stu-id="28a82-197">They can select a partner to see details.</span></span>

   :::image type="content" source="images/mca/customeraccept.png" alt-text="Kunden.":::

>[!NOTE]
><span data-ttu-id="28a82-199">I vissa fall kanske kunderna inte kan godkänna Microsoft-kundavtal.</span><span class="sxs-lookup"><span data-stu-id="28a82-199">In certain scenarios, customers may not be able to directly accept the Microsoft Customer Agreement.</span></span> <span data-ttu-id="28a82-200">Mer information om dessa situationer finns i Två scenarier där du behöver attesta för din kunds räkning nedan.</span><span class="sxs-lookup"><span data-stu-id="28a82-200">To learn more about these situations, read Two scenarios where you need to attest on behalf of your customer, below.</span></span>

## <a name="two-scenarios-where-you-need-to-attest-on-behalf-of-your-customer"></a><span data-ttu-id="28a82-201">Två scenarier där du behöver attesta för din kunds räkning</span><span class="sxs-lookup"><span data-stu-id="28a82-201">Two scenarios where you need to attest on behalf of your customer</span></span>

<span data-ttu-id="28a82-202">Det finns två scenarier där kunder kanske inte kan godkänna Microsoft-kundavtal i Microsoft 365 administrationscenter.</span><span class="sxs-lookup"><span data-stu-id="28a82-202">There are two scenarios where customers may not be able to directly accept the Microsoft Customer Agreement within the Microsoft 365 Admin Center.</span></span>

<span data-ttu-id="28a82-203">**Scenario 1:** En befintlig kund har köpt något av följande via en befintlig partnerrelation: erbjudanden, programvaru- eller programvaruprenumerationer, reserverade instanser eller Azure-plan.</span><span class="sxs-lookup"><span data-stu-id="28a82-203">**Scenario 1**: An existing customer has purchased any of the following through an existing partner relationship: offers, software or software subscriptions, Reserved Instances, or Azure Plan.</span></span> <span data-ttu-id="28a82-204">Kunden försöker nu göra ett nytt köp (exklusive automatisk förnyelse).</span><span class="sxs-lookup"><span data-stu-id="28a82-204">The customer is now attempting to make any new purchase (excluding auto renewal).</span></span> <span data-ttu-id="28a82-205">När kunden klickar på URL:en får de meddelandet "Kontakta din partner för att bekräfta att du godkänner Microsoft-kundavtal".</span><span class="sxs-lookup"><span data-stu-id="28a82-205">When that customer clicks the URL, they will receive the message "Please reach out to your Partner to confirm your acceptance of the Microsoft Customer Agreement."</span></span>  

<span data-ttu-id="28a82-206">**För att** lösa problemet måste du intyga för kundens räkning.</span><span class="sxs-lookup"><span data-stu-id="28a82-206">**To resolve**: You must attest on behalf of the customer.</span></span>

:::image type="content" source="images/mca/accept-scenario-1.png" alt-text="Skärmbild av Microsoft 365 administrationscenter där du uppmanas att kontakta din partner för att bekräfta godkännandet av Microsoft-kundavtal.":::

<span data-ttu-id="28a82-208">**Scenario 2:** En befintlig kund har köpt något av följande erbjudanden, programvaru- och programvaruprenumerationer, reserverade instanser och Azure-plan.</span><span class="sxs-lookup"><span data-stu-id="28a82-208">**Scenario 2**: An existing customer has purchased any of the following offers, software and software subscriptions, Reserved Instances, and Azure Plan.</span></span> <span data-ttu-id="28a82-209">Kunden försöker nu göra ett nytt köp med en ny partner.</span><span class="sxs-lookup"><span data-stu-id="28a82-209">The customer is now attempting to make any new purchase with a new partner.</span></span>

<span data-ttu-id="28a82-210">När kunden klickar på URL:en till Microsoft 365-administrationscentret för att godkänna den nya partnerrelationen och avtalet får de meddelandet "Kontakta din partner för att bekräfta att du godkänner Microsoft-kundavtal".</span><span class="sxs-lookup"><span data-stu-id="28a82-210">When the customer clicks the URL to Microsoft 365 Admin Center to accept the new partner relationship and the agreement, they will receive the message "Please reach out to your Partner to confirm your acceptance of the Microsoft Customer Agreement."</span></span>  

<span data-ttu-id="28a82-211">**För att** lösa problemet måste du intyga för kundens räkning.</span><span class="sxs-lookup"><span data-stu-id="28a82-211">**To resolve**: You must attest on behalf of the customer.</span></span>  

## <a name="confirm-that-a-customer-has-accepted-the-agreement"></a><span data-ttu-id="28a82-212">Bekräfta att en kund har accepterat avtalet</span><span class="sxs-lookup"><span data-stu-id="28a82-212">Confirm that a customer has accepted the agreement</span></span>

<span data-ttu-id="28a82-213">Om du försöker skapa en ny order för en befintlig kund som du inte har bekräftat tidigare får du en uppmaning om att slutföra bekräftelsen.</span><span class="sxs-lookup"><span data-stu-id="28a82-213">If you try to create a new order for an existing customer who you have not confirmed before, you'll receive a prompt to complete the confirmation.</span></span> <span data-ttu-id="28a82-214">Gör detta på följande sätt.</span><span class="sxs-lookup"><span data-stu-id="28a82-214">Use the following procedure to do this.</span></span>

1. <span data-ttu-id="28a82-215">Ange **förnamn,** **efternamn,** **e-postadress** och **telefonnummer (valfritt)** för den användare som godkände avtalet.</span><span class="sxs-lookup"><span data-stu-id="28a82-215">Enter the **First name**, **Last name**, **Email address**, and **Phone number** (optional) of the user who accepted the agreement.</span></span>

2. <span data-ttu-id="28a82-216">Under **Avtalets godkännandedatum** anger du lämpligt datum.</span><span class="sxs-lookup"><span data-stu-id="28a82-216">Under **Agreement acceptance date**, enter the appropriate date.</span></span> <span data-ttu-id="28a82-217">Du kan inte ange detta till ett framtida datum.</span><span class="sxs-lookup"><span data-stu-id="28a82-217">You cannot set this to a future date.</span></span>

3. <span data-ttu-id="28a82-218">Välj **Spara och fortsätt**.</span><span class="sxs-lookup"><span data-stu-id="28a82-218">Select **Save and continue**.</span></span> 

## <a name="next-steps"></a><span data-ttu-id="28a82-219">Nästa steg</span><span class="sxs-lookup"><span data-stu-id="28a82-219">Next steps</span></span>

- [<span data-ttu-id="28a82-220">Verifiera eller uppdatera företagets profilinformation</span><span class="sxs-lookup"><span data-stu-id="28a82-220">Verify or update your company profile information</span></span>](update-your-partner-profile.md)
- [<span data-ttu-id="28a82-221">Microsoft-kundavtal (efter region, språk)</span><span class="sxs-lookup"><span data-stu-id="28a82-221">Microsoft Customer Agreements (by region, language)</span></span>](Agreements.md)
