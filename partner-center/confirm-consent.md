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
ms.openlocfilehash: aacca72e9af45b2777364734c2b07dbe8101989d
ms.sourcegitcommit: 22af0997d52a87417b62f44fb0a7d711bec77b35
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 10/19/2020
ms.locfileid: "92532124"
---
# <a name="updated-method-to-confirm-customer-acceptance-of-the-microsoft-customer-agreement"></a><span data-ttu-id="d588d-104">Uppdaterad metod för att bekräfta kund godkännande av Microsofts kund avtal</span><span class="sxs-lookup"><span data-stu-id="d588d-104">Updated method to confirm customer acceptance of the Microsoft Customer Agreement</span></span>

<span data-ttu-id="d588d-105">**Gäller för**</span><span class="sxs-lookup"><span data-stu-id="d588d-105">**Applies to**</span></span>

-  <span data-ttu-id="d588d-106">Partnercenter</span><span class="sxs-lookup"><span data-stu-id="d588d-106">Partner Center</span></span>

<span data-ttu-id="d588d-107">**Lämpliga roller**</span><span class="sxs-lookup"><span data-stu-id="d588d-107">**Appropriate roles**</span></span>

- <span data-ttu-id="d588d-108">Administratörs agent</span><span class="sxs-lookup"><span data-stu-id="d588d-108">Admin agent</span></span>
- <span data-ttu-id="d588d-109">Försäljnings agent</span><span class="sxs-lookup"><span data-stu-id="d588d-109">Sales agent</span></span>

> [!NOTE]
> <span data-ttu-id="d588d-110">Avtals resursen stöds för närvarande av Partner Center i det offentliga Microsoft-molnet.</span><span class="sxs-lookup"><span data-stu-id="d588d-110">The Agreement resource is currently supported by Partner Center in the Microsoft public cloud only.</span></span> <span data-ttu-id="d588d-111">Det gäller inte för:</span><span class="sxs-lookup"><span data-stu-id="d588d-111">It is not applicable to:</span></span>
> * <span data-ttu-id="d588d-112">Partner Center som drivs av 21Vianet</span><span class="sxs-lookup"><span data-stu-id="d588d-112">Partner Center operated by 21Vianet</span></span>
> * <span data-ttu-id="d588d-113">Partner Center för Microsoft Cloud Germany</span><span class="sxs-lookup"><span data-stu-id="d588d-113">Partner Center for Microsoft Cloud Germany</span></span>
> * <span data-ttu-id="d588d-114">Partner Center för Microsoft Cloud för amerikanska myndigheter</span><span class="sxs-lookup"><span data-stu-id="d588d-114">Partner Center for Microsoft Cloud for US Government</span></span>

>[!NOTE]
><span data-ttu-id="d588d-115">Från och med den 31 januari 2020 måste alla kunder, befintliga och nya, signera det nya Microsofts kund avtal.</span><span class="sxs-lookup"><span data-stu-id="d588d-115">As of January 31, 2020, all customers, existing and new, must sign the new Microsoft Customer Agreement.</span></span> <span data-ttu-id="d588d-116">Läs mer i [bekräfta kund godkännande av Microsofts kund avtal](confirm-customer-agreement.md).</span><span class="sxs-lookup"><span data-stu-id="d588d-116">To learn more, read [Confirm customer acceptance of the Microsoft Customer Agreement](confirm-customer-agreement.md).</span></span>

<span data-ttu-id="d588d-117">Som partner måste du inhämta kundens godkännande av Microsofts kund avtal innan du kan beställa Microsofts produkter och tjänster för kunden.</span><span class="sxs-lookup"><span data-stu-id="d588d-117">As a partner, you need to obtain your customer's acceptance of the Microsoft Customer Agreement before you can order Microsoft products and services for that customer.</span></span> <span data-ttu-id="d588d-118">För att bättre hjälpa partners att uppfylla kraven för efterlevnad ber Microsoft partners att bekräfta godkännande genom att tillhandahålla följande information om den person som har godkänt avtalet:</span><span class="sxs-lookup"><span data-stu-id="d588d-118">To better help partners meet compliance requirements, Microsoft asks partners to confirm acceptance by providing the following details regarding the person who accepted the agreement:</span></span>

- <span data-ttu-id="d588d-119">Förnamn</span><span class="sxs-lookup"><span data-stu-id="d588d-119">First name</span></span>

- <span data-ttu-id="d588d-120">Efternamn</span><span class="sxs-lookup"><span data-stu-id="d588d-120">Last name</span></span>

- <span data-ttu-id="d588d-121">E-postadress</span><span class="sxs-lookup"><span data-stu-id="d588d-121">Email address</span></span>

- <span data-ttu-id="d588d-122">Telefonnummer (valfritt)</span><span class="sxs-lookup"><span data-stu-id="d588d-122">Phone number (optional)</span></span>

- <span data-ttu-id="d588d-123">Datum för godkännande</span><span class="sxs-lookup"><span data-stu-id="d588d-123">Date of acceptance</span></span>

<span data-ttu-id="d588d-124">Direkta fakturerings partner och indirekta leverantörer måste bekräfta kund godkännande av Microsofts kund avtal vid kommunikation via partner Center eller API för partner Center.</span><span class="sxs-lookup"><span data-stu-id="d588d-124">Direct bill partners and Indirect Providers must confirm customer acceptance of the Microsoft Customer Agreement when transacting through Partner Center or Partner Center API.</span></span> <span data-ttu-id="d588d-125">Bekräftelse är *obligatorisk* .</span><span class="sxs-lookup"><span data-stu-id="d588d-125">Confirmation is *mandatory* .</span></span>

<span data-ttu-id="d588d-126">Om ingen bekräftelse anges för en angiven kund:</span><span class="sxs-lookup"><span data-stu-id="d588d-126">If confirmation is not provided for a given customer:</span></span>

- <span data-ttu-id="d588d-127">Du kommer inte att kunna skapa nya beställningar för den här kunden.</span><span class="sxs-lookup"><span data-stu-id="d588d-127">You won't be able to create new orders for this customer.</span></span>

- <span data-ttu-id="d588d-128">Du kommer inte att kunna ändra licens antalet för befintliga licensbaserade prenumerationer för den här kunden.</span><span class="sxs-lookup"><span data-stu-id="d588d-128">You won't be able to change the license count of existing license-based subscriptions for this customer.</span></span>

<span data-ttu-id="d588d-129">Bekräftelse av kund godkännande kan göras via partner Center eller partner Center API.</span><span class="sxs-lookup"><span data-stu-id="d588d-129">Confirmation of customer acceptance can be done via Partner Center or the Partner Center API.</span></span> <span data-ttu-id="d588d-130">Om du vill göra detta via partner Center API, se följande avsnitt:</span><span class="sxs-lookup"><span data-stu-id="d588d-130">To do this through the Partner Center API, see the following topics:</span></span>

- [<span data-ttu-id="d588d-131">Få bekräftelse på kund medgivande</span><span class="sxs-lookup"><span data-stu-id="d588d-131">Get confirmation of customer consent</span></span>](/partner-center/develop/get-confirmation-of-customer-consent)

- [<span data-ttu-id="d588d-132">Hämta avtals metadata</span><span class="sxs-lookup"><span data-stu-id="d588d-132">Get agreement metadata</span></span>](/partner-center/develop/get-agreement-metadata)

- [<span data-ttu-id="d588d-133">Bekräfta kund medgivande</span><span class="sxs-lookup"><span data-stu-id="d588d-133">Confirm customer consent</span></span>](/partner-center/develop/confirm-customer-consent)

<span data-ttu-id="d588d-134">Detta gäller för både produktions-och sandbox-miljöer.</span><span class="sxs-lookup"><span data-stu-id="d588d-134">This applies to both production and sandbox environments.</span></span>

## <a name="confirm-customer-acceptance-for-a-new-customer"></a><span data-ttu-id="d588d-135">Bekräfta kund godkännande för en ny kund</span><span class="sxs-lookup"><span data-stu-id="d588d-135">Confirm customer acceptance for a new customer</span></span>

<span data-ttu-id="d588d-136">Använd följande procedur för att bekräfta kund godkännande när du skapar en ny kund klient i Partner Center.</span><span class="sxs-lookup"><span data-stu-id="d588d-136">Use the following procedure to confirm customer acceptance while you create a new customer tenant in Partner Center.</span></span> <span data-ttu-id="d588d-137">Du måste vara administratörs agent eller försäljnings agent för att göra detta.</span><span class="sxs-lookup"><span data-stu-id="d588d-137">You must be an Admin agent or Sales agent to do this.</span></span>

1. <span data-ttu-id="d588d-138">Välj **kunder** och sedan **ny kund** och välj sedan **konto information** .</span><span class="sxs-lookup"><span data-stu-id="d588d-138">Select **Customers** , and then **New customer** and then select **Account info** .</span></span>

2. <span data-ttu-id="d588d-139">Ange information om **företaget** och den **primära kontakten** .</span><span class="sxs-lookup"><span data-stu-id="d588d-139">Enter the information about the **Company** and **Primary contact** .</span></span>

   :::image type="content" source="images/mca/mca1.png" alt-text="Företags information":::

3. <span data-ttu-id="d588d-141">Under **Microsofts kund avtal** väljer **du kunden har accepterat det senaste kund avtalet från Microsoft** .</span><span class="sxs-lookup"><span data-stu-id="d588d-141">Under **Microsoft customer agreement** , select **The customer has accepted the latest Microsoft customer agreement** .</span></span>

4. <span data-ttu-id="d588d-142">Ange ett datum under **avtalets godkännande datum** .</span><span class="sxs-lookup"><span data-stu-id="d588d-142">Under **Agreement acceptance date** , enter the appropriate date.</span></span> <span data-ttu-id="d588d-143">Du kan inte ange ett framtida datum.</span><span class="sxs-lookup"><span data-stu-id="d588d-143">You cannot set this to a future date.</span></span>

5. <span data-ttu-id="d588d-144">Ange information om den användare som tillhandahöll godkännandet.</span><span class="sxs-lookup"><span data-stu-id="d588d-144">Enter the details of the user who provided the acceptance.</span></span>

   :::image type="content" source="images/mca/MCA3.png" alt-text="Lägg till godkännande datum":::

   <span data-ttu-id="d588d-146">Som standard visas den primära kontaktens användar information.</span><span class="sxs-lookup"><span data-stu-id="d588d-146">By default, the primary contact user information is displayed.</span></span> <span data-ttu-id="d588d-147">Om detta inte är korrekt väljer du **Uppdatera** och anger sedan **förnamn** , **efter namn** , **e-postadress** och \* *telefonnummer* (valfritt) för den person som har godkänt avtalet.</span><span class="sxs-lookup"><span data-stu-id="d588d-147">If this isn't correct, select **Update** and then enter the **First name** , **Last name** , **Email address** , and \* *Phone number* (optional) of the person who accepted the agreement.</span></span>

6. <span data-ttu-id="d588d-148">Välj **Nästa** för att fortsätta med de återstående stegen för att skapa kund klienten.</span><span class="sxs-lookup"><span data-stu-id="d588d-148">Select **Next** to continue with the remaining steps to create the customer tenant.</span></span>

## <a name="confirm-customer-acceptance-for-an-existing-customer"></a><span data-ttu-id="d588d-149">Bekräfta kund godkännande för en befintlig kund</span><span class="sxs-lookup"><span data-stu-id="d588d-149">Confirm customer acceptance for an existing customer</span></span>

<span data-ttu-id="d588d-150">Du måste vara administratörs agent eller försäljnings agent för att göra detta.</span><span class="sxs-lookup"><span data-stu-id="d588d-150">You must be an Admin agent or Sales agent to do this.</span></span>

1. <span data-ttu-id="d588d-151">Välj **kunder** och leta upp och välj den kund som du vill se.</span><span class="sxs-lookup"><span data-stu-id="d588d-151">Select **Customers** , and then find and select the customer you want to see.</span></span>

2. <span data-ttu-id="d588d-152">Välj **konto information** .</span><span class="sxs-lookup"><span data-stu-id="d588d-152">Select **Account info** .</span></span>

3. <span data-ttu-id="d588d-153">Under **Microsofts kund avtal** väljer du **Uppdatera** .</span><span class="sxs-lookup"><span data-stu-id="d588d-153">Under **Microsoft customer agreement** , select **Update** .</span></span>

   :::image type="content" source="images/mca/mca4.png" alt-text="Uppdatera":::

4. <span data-ttu-id="d588d-155">Ange **förnamn** , **efter namn** , **e-postadress** och **telefonnummer** (valfritt) för den användare som har godkänt avtalet.</span><span class="sxs-lookup"><span data-stu-id="d588d-155">Enter the **First name** , **Last name** , **Email address** , and **Phone number** (optional) of the user who accepted the agreement.</span></span>

5. <span data-ttu-id="d588d-156">Ange ett datum under **avtalets godkännande datum** .</span><span class="sxs-lookup"><span data-stu-id="d588d-156">Under **Agreement acceptance date** , enter the appropriate date.</span></span> <span data-ttu-id="d588d-157">Du kan inte ange ett framtida datum.</span><span class="sxs-lookup"><span data-stu-id="d588d-157">You cannot set this to a future date.</span></span>

6. <span data-ttu-id="d588d-158">Välj **Spara och fortsätt** .</span><span class="sxs-lookup"><span data-stu-id="d588d-158">Select **Save and continue** .</span></span>

## <a name="confirm-customer-acceptance-while-creating-new-order-for-an-existing-customer"></a><span data-ttu-id="d588d-159">Bekräfta kund godkännande när du skapar en ny order för en befintlig kund</span><span class="sxs-lookup"><span data-stu-id="d588d-159">Confirm customer acceptance while creating new order for an existing customer</span></span>

<span data-ttu-id="d588d-160">Om du försöker skapa en ny order för en befintlig kund som du inte har bekräftat tidigare får du ett meddelande om att slutföra bekräftelsen.</span><span class="sxs-lookup"><span data-stu-id="d588d-160">If you try to create a new order for an existing customer who you have not confirmed before, you'll receive a prompt to complete the confirmation.</span></span> <span data-ttu-id="d588d-161">Använd följande procedur för att göra detta.</span><span class="sxs-lookup"><span data-stu-id="d588d-161">Use the following procedure to do this.</span></span>

1. <span data-ttu-id="d588d-162">Ange **förnamn** , **efter namn** , **e-postadress** och **telefonnummer** (valfritt) för den användare som har godkänt avtalet.</span><span class="sxs-lookup"><span data-stu-id="d588d-162">Enter the **First name** , **Last name** , **Email address** , and **Phone number** (optional) of the user who accepted the agreement.</span></span>

2. <span data-ttu-id="d588d-163">Ange ett datum under **avtalets godkännande datum** .</span><span class="sxs-lookup"><span data-stu-id="d588d-163">Under **Agreement acceptance date** , enter the appropriate date.</span></span> <span data-ttu-id="d588d-164">Du kan inte ange ett framtida datum.</span><span class="sxs-lookup"><span data-stu-id="d588d-164">You cannot set this to a future date.</span></span>

3. <span data-ttu-id="d588d-165">Välj **Spara och fortsätt** .</span><span class="sxs-lookup"><span data-stu-id="d588d-165">Select **Save and continue** .</span></span>

## <a name="retrieve-confirmation-of-customer-acceptance-for-an-existing-customer"></a><span data-ttu-id="d588d-166">Hämta bekräftelse av kund godkännande för en befintlig kund</span><span class="sxs-lookup"><span data-stu-id="d588d-166">Retrieve confirmation of customer acceptance for an existing customer</span></span>

<span data-ttu-id="d588d-167">Du kan hämta bekräftelse på kund godkännande för en befintlig kund som du har angett tidigare med hjälp av proceduren nedan.</span><span class="sxs-lookup"><span data-stu-id="d588d-167">You can retrieve confirmation of customer acceptance for an existing customer that you have provided previously using the procedure below.</span></span> <span data-ttu-id="d588d-168">Du måste vara administratörs agent eller försäljnings agent för att göra detta.</span><span class="sxs-lookup"><span data-stu-id="d588d-168">You must be an Admin agent or Sales agent to do this.</span></span>

1. <span data-ttu-id="d588d-169">Välj **kunder** och leta upp och välj den kund som du vill se.</span><span class="sxs-lookup"><span data-stu-id="d588d-169">Select **Customers** , and then find and select the customer you want to see.</span></span>

2. <span data-ttu-id="d588d-170">Välj **konto information** .</span><span class="sxs-lookup"><span data-stu-id="d588d-170">Select **Account info** .</span></span>

3. <span data-ttu-id="d588d-171">Under **Microsofts kund avtal** ser du om en bekräftelse har angetts för kunden.</span><span class="sxs-lookup"><span data-stu-id="d588d-171">Under **Microsoft customer agreement** , you'll see whether or not confirmation has been provided for this customer.</span></span>

## <a name="next-steps"></a><span data-ttu-id="d588d-172">Nästa steg</span><span class="sxs-lookup"><span data-stu-id="d588d-172">Next steps</span></span>

- [<span data-ttu-id="d588d-173">Bekräfta kund godkännande av Microsofts kund avtal i CSP partner-programmet</span><span class="sxs-lookup"><span data-stu-id="d588d-173">Confirm customer acceptance of the Microsoft Customer Agreement in the CSP partner program</span></span>](confirm-customer-agreement.md)

- [<span data-ttu-id="d588d-174">Attestering av godkännande av Microsofts kund avtal för kundens räkning</span><span class="sxs-lookup"><span data-stu-id="d588d-174">Attest acceptance of the Microsoft Customer Agreement on behalf of your customer</span></span>](attest-acceptance-customer-agreement.md)