---
title: Bekräfta kund godkännande av Microsofts kund avtal
description: Lär dig hur du bekräftar kund godkännande av Microsofts kund avtal. Det kan vara nödvändigt att beställa Microsoft-produkter och-tjänster för kunder.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: aarzh-AaronZhang
ms.author: v-aarzh
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.date: 06/30/2020
ms.openlocfilehash: f2513213bff38a6296832253a13725ff2508f1f8
ms.sourcegitcommit: 22d79fb31cce852ae809078ea2310ebc80030739
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 12/12/2020
ms.locfileid: "97354618"
---
# <a name="updated-method-to-confirm-customer-acceptance-of-the-microsoft-customer-agreement"></a><span data-ttu-id="c930f-104">Uppdaterad metod för att bekräfta kund godkännande av Microsofts kund avtal</span><span class="sxs-lookup"><span data-stu-id="c930f-104">Updated method to confirm customer acceptance of the Microsoft Customer Agreement</span></span>


<span data-ttu-id="c930f-105">**Lämpliga roller**</span><span class="sxs-lookup"><span data-stu-id="c930f-105">**Appropriate roles**</span></span>

- <span data-ttu-id="c930f-106">Administratörs agent</span><span class="sxs-lookup"><span data-stu-id="c930f-106">Admin agent</span></span>
- <span data-ttu-id="c930f-107">Försäljnings agent</span><span class="sxs-lookup"><span data-stu-id="c930f-107">Sales agent</span></span>

> [!NOTE]
> <span data-ttu-id="c930f-108">Avtals resursen stöds för närvarande av Partner Center i det offentliga Microsoft-molnet.</span><span class="sxs-lookup"><span data-stu-id="c930f-108">The Agreement resource is currently supported by Partner Center in the Microsoft public cloud only.</span></span> <span data-ttu-id="c930f-109">Det gäller inte för:</span><span class="sxs-lookup"><span data-stu-id="c930f-109">It is not applicable to:</span></span>
> * <span data-ttu-id="c930f-110">Partner Center som drivs av 21Vianet</span><span class="sxs-lookup"><span data-stu-id="c930f-110">Partner Center operated by 21Vianet</span></span>
> * <span data-ttu-id="c930f-111">Partnercenter för Microsoft Cloud Tyskland</span><span class="sxs-lookup"><span data-stu-id="c930f-111">Partner Center for Microsoft Cloud Germany</span></span>
> * <span data-ttu-id="c930f-112">Välkommen till Partnercenter för Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="c930f-112">Partner Center for Microsoft Cloud for US Government</span></span>

>[!NOTE]
><span data-ttu-id="c930f-113">Från och med den 31 januari 2020 måste alla kunder, befintliga och nya, signera det nya Microsofts kund avtal.</span><span class="sxs-lookup"><span data-stu-id="c930f-113">As of January 31, 2020, all customers, existing and new, must sign the new Microsoft Customer Agreement.</span></span> <span data-ttu-id="c930f-114">Läs mer i [bekräfta kund godkännande av Microsofts kund avtal](confirm-customer-agreement.md).</span><span class="sxs-lookup"><span data-stu-id="c930f-114">To learn more, read [Confirm customer acceptance of the Microsoft Customer Agreement](confirm-customer-agreement.md).</span></span>

<span data-ttu-id="c930f-115">Som partner måste du inhämta kundens godkännande av Microsofts kund avtal innan du kan beställa Microsofts produkter och tjänster för kunden.</span><span class="sxs-lookup"><span data-stu-id="c930f-115">As a partner, you need to obtain your customer's acceptance of the Microsoft Customer Agreement before you can order Microsoft products and services for that customer.</span></span> <span data-ttu-id="c930f-116">För att bättre hjälpa partners att uppfylla kraven för efterlevnad ber Microsoft partners att bekräfta godkännande genom att tillhandahålla följande information om den person som har godkänt avtalet:</span><span class="sxs-lookup"><span data-stu-id="c930f-116">To better help partners meet compliance requirements, Microsoft asks partners to confirm acceptance by providing the following details regarding the person who accepted the agreement:</span></span>

- <span data-ttu-id="c930f-117">Förnamn</span><span class="sxs-lookup"><span data-stu-id="c930f-117">First name</span></span>

- <span data-ttu-id="c930f-118">Efternamn</span><span class="sxs-lookup"><span data-stu-id="c930f-118">Last name</span></span>

- <span data-ttu-id="c930f-119">E-postadress</span><span class="sxs-lookup"><span data-stu-id="c930f-119">Email address</span></span>

- <span data-ttu-id="c930f-120">Telefonnummer (valfritt)</span><span class="sxs-lookup"><span data-stu-id="c930f-120">Phone number (optional)</span></span>

- <span data-ttu-id="c930f-121">Datum för godkännande</span><span class="sxs-lookup"><span data-stu-id="c930f-121">Date of acceptance</span></span>

<span data-ttu-id="c930f-122">Direkta fakturerings partner och indirekta leverantörer måste bekräfta kund godkännande av Microsofts kund avtal vid kommunikation via partner Center eller API för partner Center.</span><span class="sxs-lookup"><span data-stu-id="c930f-122">Direct bill partners and Indirect Providers must confirm customer acceptance of the Microsoft Customer Agreement when transacting through Partner Center or Partner Center API.</span></span> <span data-ttu-id="c930f-123">Bekräftelse är *obligatorisk*.</span><span class="sxs-lookup"><span data-stu-id="c930f-123">Confirmation is *mandatory*.</span></span>

<span data-ttu-id="c930f-124">Om ingen bekräftelse anges för en angiven kund:</span><span class="sxs-lookup"><span data-stu-id="c930f-124">If confirmation is not provided for a given customer:</span></span>

- <span data-ttu-id="c930f-125">Du kommer inte att kunna skapa nya beställningar för den här kunden.</span><span class="sxs-lookup"><span data-stu-id="c930f-125">You won't be able to create new orders for this customer.</span></span>

- <span data-ttu-id="c930f-126">Du kommer inte att kunna ändra licens antalet för befintliga licensbaserade prenumerationer för den här kunden.</span><span class="sxs-lookup"><span data-stu-id="c930f-126">You won't be able to change the license count of existing license-based subscriptions for this customer.</span></span>

<span data-ttu-id="c930f-127">Bekräftelse av kund godkännande kan göras via partner Center eller partner Center API.</span><span class="sxs-lookup"><span data-stu-id="c930f-127">Confirmation of customer acceptance can be done via Partner Center or the Partner Center API.</span></span> <span data-ttu-id="c930f-128">Om du vill göra detta via partner Center API, se följande avsnitt:</span><span class="sxs-lookup"><span data-stu-id="c930f-128">To do this through the Partner Center API, see the following topics:</span></span>

- [<span data-ttu-id="c930f-129">Få bekräftelse på kund medgivande</span><span class="sxs-lookup"><span data-stu-id="c930f-129">Get confirmation of customer consent</span></span>](/partner-center/develop/get-confirmation-of-customer-consent)

- [<span data-ttu-id="c930f-130">Hämta avtals metadata</span><span class="sxs-lookup"><span data-stu-id="c930f-130">Get agreement metadata</span></span>](/partner-center/develop/get-agreement-metadata)

- [<span data-ttu-id="c930f-131">Bekräfta kund medgivande</span><span class="sxs-lookup"><span data-stu-id="c930f-131">Confirm customer consent</span></span>](/partner-center/develop/confirm-customer-consent)

<span data-ttu-id="c930f-132">Detta gäller för både produktions-och sandbox-miljöer.</span><span class="sxs-lookup"><span data-stu-id="c930f-132">This applies to both production and sandbox environments.</span></span>

## <a name="confirm-customer-acceptance-for-a-new-customer"></a><span data-ttu-id="c930f-133">Bekräfta kund godkännande för en ny kund</span><span class="sxs-lookup"><span data-stu-id="c930f-133">Confirm customer acceptance for a new customer</span></span>

<span data-ttu-id="c930f-134">Använd följande procedur för att bekräfta kund godkännande när du skapar en ny kund klient i Partner Center.</span><span class="sxs-lookup"><span data-stu-id="c930f-134">Use the following procedure to confirm customer acceptance while you create a new customer tenant in Partner Center.</span></span> <span data-ttu-id="c930f-135">Du måste vara administratörs agent eller försäljnings agent för att göra detta.</span><span class="sxs-lookup"><span data-stu-id="c930f-135">You must be an Admin agent or Sales agent to do this.</span></span>

1. <span data-ttu-id="c930f-136">Välj **kunder** och sedan **ny kund** och välj sedan **konto information**.</span><span class="sxs-lookup"><span data-stu-id="c930f-136">Select **Customers**, and then **New customer** and then select **Account info**.</span></span>

2. <span data-ttu-id="c930f-137">Ange information om **företaget** och den **primära kontakten**.</span><span class="sxs-lookup"><span data-stu-id="c930f-137">Enter the information about the **Company** and **Primary contact**.</span></span>

   :::image type="content" source="images/mca/mca1.png" alt-text="Företags information":::

3. <span data-ttu-id="c930f-139">Under **Microsofts kund avtal** väljer **du kunden har accepterat det senaste kund avtalet från Microsoft**.</span><span class="sxs-lookup"><span data-stu-id="c930f-139">Under **Microsoft customer agreement**, select **The customer has accepted the latest Microsoft customer agreement**.</span></span>

4. <span data-ttu-id="c930f-140">Ange ett datum under **avtalets godkännande datum**.</span><span class="sxs-lookup"><span data-stu-id="c930f-140">Under **Agreement acceptance date**, enter the appropriate date.</span></span> <span data-ttu-id="c930f-141">Du kan inte ange ett framtida datum.</span><span class="sxs-lookup"><span data-stu-id="c930f-141">You cannot set this to a future date.</span></span>

5. <span data-ttu-id="c930f-142">Ange information om den användare som tillhandahöll godkännandet.</span><span class="sxs-lookup"><span data-stu-id="c930f-142">Enter the details of the user who provided the acceptance.</span></span>

   :::image type="content" source="images/mca/MCA3.png" alt-text="Lägg till godkännande datum":::

   <span data-ttu-id="c930f-144">Som standard visas den primära kontaktens användar information.</span><span class="sxs-lookup"><span data-stu-id="c930f-144">By default, the primary contact user information is displayed.</span></span> <span data-ttu-id="c930f-145">Om detta inte är korrekt väljer du **Uppdatera** och anger sedan **förnamn**, **efter namn**, **e-postadress** och \**telefonnummer* (valfritt) för den person som har godkänt avtalet.</span><span class="sxs-lookup"><span data-stu-id="c930f-145">If this isn't correct, select **Update** and then enter the **First name**, **Last name**, **Email address**, and \**Phone number* (optional) of the person who accepted the agreement.</span></span>

6. <span data-ttu-id="c930f-146">Välj **Nästa** för att fortsätta med de återstående stegen för att skapa kund klienten.</span><span class="sxs-lookup"><span data-stu-id="c930f-146">Select **Next** to continue with the remaining steps to create the customer tenant.</span></span>

## <a name="confirm-customer-acceptance-for-an-existing-customer"></a><span data-ttu-id="c930f-147">Bekräfta kund godkännande för en befintlig kund</span><span class="sxs-lookup"><span data-stu-id="c930f-147">Confirm customer acceptance for an existing customer</span></span>

<span data-ttu-id="c930f-148">Du måste vara administratörs agent eller försäljnings agent för att göra detta.</span><span class="sxs-lookup"><span data-stu-id="c930f-148">You must be an Admin agent or Sales agent to do this.</span></span>

1. <span data-ttu-id="c930f-149">Välj **kunder** och leta upp och välj den kund som du vill se.</span><span class="sxs-lookup"><span data-stu-id="c930f-149">Select **Customers**, and then find and select the customer you want to see.</span></span>

2. <span data-ttu-id="c930f-150">Välj **konto information**.</span><span class="sxs-lookup"><span data-stu-id="c930f-150">Select **Account info**.</span></span>

3. <span data-ttu-id="c930f-151">Under **Microsofts kund avtal** väljer du **Uppdatera**.</span><span class="sxs-lookup"><span data-stu-id="c930f-151">Under **Microsoft customer agreement**, select **Update**.</span></span>

   :::image type="content" source="images/mca/mca4.png" alt-text="Uppdatera":::

4. <span data-ttu-id="c930f-153">Ange **förnamn**, **efter namn**, **e-postadress** och **telefonnummer** (valfritt) för den användare som har godkänt avtalet.</span><span class="sxs-lookup"><span data-stu-id="c930f-153">Enter the **First name**, **Last name**, **Email address**, and **Phone number** (optional) of the user who accepted the agreement.</span></span>

5. <span data-ttu-id="c930f-154">Ange ett datum under **avtalets godkännande datum**.</span><span class="sxs-lookup"><span data-stu-id="c930f-154">Under **Agreement acceptance date**, enter the appropriate date.</span></span> <span data-ttu-id="c930f-155">Du kan inte ange ett framtida datum.</span><span class="sxs-lookup"><span data-stu-id="c930f-155">You cannot set this to a future date.</span></span>

6. <span data-ttu-id="c930f-156">Välj **Spara och fortsätt**.</span><span class="sxs-lookup"><span data-stu-id="c930f-156">Select **Save and continue**.</span></span>

## <a name="confirm-customer-acceptance-while-creating-new-order-for-an-existing-customer"></a><span data-ttu-id="c930f-157">Bekräfta kund godkännande när du skapar en ny order för en befintlig kund</span><span class="sxs-lookup"><span data-stu-id="c930f-157">Confirm customer acceptance while creating new order for an existing customer</span></span>

<span data-ttu-id="c930f-158">Om du försöker skapa en ny order för en befintlig kund som du inte har bekräftat tidigare får du ett meddelande om att slutföra bekräftelsen.</span><span class="sxs-lookup"><span data-stu-id="c930f-158">If you try to create a new order for an existing customer who you have not confirmed before, you'll receive a prompt to complete the confirmation.</span></span> <span data-ttu-id="c930f-159">Använd följande procedur för att göra detta.</span><span class="sxs-lookup"><span data-stu-id="c930f-159">Use the following procedure to do this.</span></span>

1. <span data-ttu-id="c930f-160">Ange **förnamn**, **efter namn**, **e-postadress** och **telefonnummer** (valfritt) för den användare som har godkänt avtalet.</span><span class="sxs-lookup"><span data-stu-id="c930f-160">Enter the **First name**, **Last name**, **Email address**, and **Phone number** (optional) of the user who accepted the agreement.</span></span>

2. <span data-ttu-id="c930f-161">Ange ett datum under **avtalets godkännande datum**.</span><span class="sxs-lookup"><span data-stu-id="c930f-161">Under **Agreement acceptance date**, enter the appropriate date.</span></span> <span data-ttu-id="c930f-162">Du kan inte ange ett framtida datum.</span><span class="sxs-lookup"><span data-stu-id="c930f-162">You cannot set this to a future date.</span></span>

3. <span data-ttu-id="c930f-163">Välj **Spara och fortsätt**.</span><span class="sxs-lookup"><span data-stu-id="c930f-163">Select **Save and continue**.</span></span>

## <a name="retrieve-confirmation-of-customer-acceptance-for-an-existing-customer"></a><span data-ttu-id="c930f-164">Hämta bekräftelse av kund godkännande för en befintlig kund</span><span class="sxs-lookup"><span data-stu-id="c930f-164">Retrieve confirmation of customer acceptance for an existing customer</span></span>

<span data-ttu-id="c930f-165">Du kan hämta bekräftelse på kund godkännande för en befintlig kund som du har angett tidigare med hjälp av proceduren nedan.</span><span class="sxs-lookup"><span data-stu-id="c930f-165">You can retrieve confirmation of customer acceptance for an existing customer that you have provided previously using the procedure below.</span></span> <span data-ttu-id="c930f-166">Du måste vara administratörs agent eller försäljnings agent för att göra detta.</span><span class="sxs-lookup"><span data-stu-id="c930f-166">You must be an Admin agent or Sales agent to do this.</span></span>

1. <span data-ttu-id="c930f-167">Välj **kunder** och leta upp och välj den kund som du vill se.</span><span class="sxs-lookup"><span data-stu-id="c930f-167">Select **Customers**, and then find and select the customer you want to see.</span></span>

2. <span data-ttu-id="c930f-168">Välj **konto information**.</span><span class="sxs-lookup"><span data-stu-id="c930f-168">Select **Account info**.</span></span>

3. <span data-ttu-id="c930f-169">Under **Microsofts kund avtal** ser du om en bekräftelse har angetts för kunden.</span><span class="sxs-lookup"><span data-stu-id="c930f-169">Under **Microsoft customer agreement**, you'll see whether or not confirmation has been provided for this customer.</span></span>

## <a name="next-steps"></a><span data-ttu-id="c930f-170">Nästa steg</span><span class="sxs-lookup"><span data-stu-id="c930f-170">Next steps</span></span>

- [<span data-ttu-id="c930f-171">Bekräfta kund godkännande av Microsofts kund avtal i CSP partner-programmet</span><span class="sxs-lookup"><span data-stu-id="c930f-171">Confirm customer acceptance of the Microsoft Customer Agreement in the CSP partner program</span></span>](confirm-customer-agreement.md)

- [<span data-ttu-id="c930f-172">Attestering av godkännande av Microsofts kund avtal för kundens räkning</span><span class="sxs-lookup"><span data-stu-id="c930f-172">Attest acceptance of the Microsoft Customer Agreement on behalf of your customer</span></span>](attest-acceptance-customer-agreement.md)