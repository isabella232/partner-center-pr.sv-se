---
title: Meddelanden i mars 2021
description: Mars 2021-meddelanden för Microsoft Partner Center, inklusive nya funktioner, kampanjer, erbjudanden, marknader eller ändringar av befintliga erbjudanden.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: brentserbus
ms.author: brserbus
ms.custom: announcement
ms.localizationpriority: high
ms.date: 04/02/2021
ms.openlocfilehash: 5b8c5f52207a7b9a49d07885a36b61486be45497
ms.sourcegitcommit: 60bbb8f4056120264b769f94431f84d86984c2e9
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/03/2021
ms.locfileid: "106280878"
---
# <a name="march-2021-announcements"></a><span data-ttu-id="d40f8-103">Meddelanden i mars 2021</span><span class="sxs-lookup"><span data-stu-id="d40f8-103">March 2021 announcements</span></span>

<span data-ttu-id="d40f8-104">Den här sidan innehåller meddelandena för Microsoft Partner Center för mars 2021.</span><span class="sxs-lookup"><span data-stu-id="d40f8-104">This page provides the announcements for Microsoft Partner Center for March 2021.</span></span>

________________
## <a name="updated-csp-customer-address-validation-api-now-available-for-testing"></a><a name="18"></a><span data-ttu-id="d40f8-105">Uppdaterat API för kund adress validering för CSP nu tillgängligt för testning</span><span class="sxs-lookup"><span data-stu-id="d40f8-105">Updated CSP customer address validation API now available for testing</span></span>

### <a name="categories"></a><span data-ttu-id="d40f8-106">Kategorier</span><span class="sxs-lookup"><span data-stu-id="d40f8-106">Categories</span></span>

- <span data-ttu-id="d40f8-107">Datum: 2021-03-31</span><span class="sxs-lookup"><span data-stu-id="d40f8-107">Date: 2021-03-31</span></span>
- <span data-ttu-id="d40f8-108">Funktioner</span><span class="sxs-lookup"><span data-stu-id="d40f8-108">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="d40f8-109">Sammanfattning</span><span class="sxs-lookup"><span data-stu-id="d40f8-109">Summary</span></span>

<span data-ttu-id="d40f8-110">Som en del av vårt åtagande att hjälpa partner och kunder att köra verksamheten baserat på förtroende kommer vi att bjuda in partners över hela världen för att testa ändringarna i ValidateAddress-API: et.</span><span class="sxs-lookup"><span data-stu-id="d40f8-110">As part of our commitment to help partners and customers run their business based on trust, we will be inviting partners worldwide to test the changes to the ValidateAddress API.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="d40f8-111">Förverkad mål grupp</span><span class="sxs-lookup"><span data-stu-id="d40f8-111">Impacted audience</span></span>

<span data-ttu-id="d40f8-112">Alla leverantörer av CSP-direkt fakturering och indirekta leverantörer som skapar nya eller uppdaterade befintliga kund adress uppgifter</span><span class="sxs-lookup"><span data-stu-id="d40f8-112">All CSP direct bill partners and indirect providers who create new or update existing customer address details</span></span>

### <a name="details"></a><span data-ttu-id="d40f8-113">Information</span><span class="sxs-lookup"><span data-stu-id="d40f8-113">Details</span></span>

<span data-ttu-id="d40f8-114">Microsoft körs med förtroende.</span><span class="sxs-lookup"><span data-stu-id="d40f8-114">Microsoft runs on trust.</span></span> <span data-ttu-id="d40f8-115">Vi strävar efter att tillhandahålla en kompatibel, säker och säker metod för att skicka in kund adress validering för att agera kund prenumerationer i CSP-programmet.</span><span class="sxs-lookup"><span data-stu-id="d40f8-115">We’re committed to providing a compliant, safe, and secure method of submitting customer address validation for transacting customer subscriptions in the CSP program.</span></span> <span data-ttu-id="d40f8-116">Idag den 31 mars 2021 har vi infört ändringar i ValidateAddress-API: et som vi vill bjuda in dig att testa, innan du fortsätter med ändringarna i juni 2021.</span><span class="sxs-lookup"><span data-stu-id="d40f8-116">Today, March 31, 2021, we have introduced changes to the ValidateAddress API that we’d like to invite you to test, prior to going live with the changes in June 2021.</span></span> 

<span data-ttu-id="d40f8-117">Observera att dessa ändringar påverkar endast ValidateAddress-API: et.</span><span class="sxs-lookup"><span data-stu-id="d40f8-117">Note that these changes affect the ValidateAddress API only.</span></span> <span data-ttu-id="d40f8-118">CreateCustomer-och UpdateBillingProfile-API: er påverkas inte.</span><span class="sxs-lookup"><span data-stu-id="d40f8-118">CreateCustomer and UpdateBillingProfile APIs are not affected.</span></span>

<span data-ttu-id="d40f8-119">Svaret returnerar ett av följande status meddelanden:</span><span class="sxs-lookup"><span data-stu-id="d40f8-119">The response will return one of the following status messages:</span></span>

| <span data-ttu-id="d40f8-120">Status</span><span class="sxs-lookup"><span data-stu-id="d40f8-120">Status</span></span> | <span data-ttu-id="d40f8-121">Beskrivning</span><span class="sxs-lookup"><span data-stu-id="d40f8-121">Description</span></span> | <span data-ttu-id="d40f8-122">Antal föreslagna adresser som returneras</span><span class="sxs-lookup"><span data-stu-id="d40f8-122">Number of suggested addresses returned</span></span> |
|----------|-------------|-------------------|
| <span data-ttu-id="d40f8-123">VerifiedShippable</span><span class="sxs-lookup"><span data-stu-id="d40f8-123">VerifiedShippable</span></span> | <span data-ttu-id="d40f8-124">Adressen verifieras och kan skickas till.</span><span class="sxs-lookup"><span data-stu-id="d40f8-124">Address is verified and can be shipped to.</span></span> | <span data-ttu-id="d40f8-125">Enkel</span><span class="sxs-lookup"><span data-stu-id="d40f8-125">Single</span></span> |
| <span data-ttu-id="d40f8-126">Kontrol</span><span class="sxs-lookup"><span data-stu-id="d40f8-126">Verified</span></span> | <span data-ttu-id="d40f8-127">Adressen har verifierats.</span><span class="sxs-lookup"><span data-stu-id="d40f8-127">Address is verified.</span></span> | <span data-ttu-id="d40f8-128">Enkel</span><span class="sxs-lookup"><span data-stu-id="d40f8-128">Single</span></span> |
| <span data-ttu-id="d40f8-129">InteractionRequired</span><span class="sxs-lookup"><span data-stu-id="d40f8-129">InteractionRequired</span></span> | <span data-ttu-id="d40f8-130">Föreslagen adress (er) har ändrats avsevärt och användar bekräftelsen behöver bekräftas.</span><span class="sxs-lookup"><span data-stu-id="d40f8-130">Suggested address(es) has been changed significantly and needs user confirmation.</span></span> | <span data-ttu-id="d40f8-131">Enkel</span><span class="sxs-lookup"><span data-stu-id="d40f8-131">Single</span></span> |
| <span data-ttu-id="d40f8-132">StreetPartial</span><span class="sxs-lookup"><span data-stu-id="d40f8-132">StreetPartial</span></span> | <span data-ttu-id="d40f8-133">Den gatuadress som anges i adressen är delvis och behöver mer information.</span><span class="sxs-lookup"><span data-stu-id="d40f8-133">The given street in the address is partial and needs more info.</span></span> | <span data-ttu-id="d40f8-134">Flera – högst tre</span><span class="sxs-lookup"><span data-stu-id="d40f8-134">Multiple—maximum of three</span></span>|
| <span data-ttu-id="d40f8-135">PremisesPartial</span><span class="sxs-lookup"><span data-stu-id="d40f8-135">PremisesPartial</span></span> | <span data-ttu-id="d40f8-136">De lokala anläggningarna (build Number, Suite Number osv.) är delvis och behöver mer information.</span><span class="sxs-lookup"><span data-stu-id="d40f8-136">The given premises (building number, suite number, etc.) is partial and needs more info.</span></span> | <span data-ttu-id="d40f8-137">Flera – högst tre</span><span class="sxs-lookup"><span data-stu-id="d40f8-137">Multiple—maximum of three</span></span> |
| <span data-ttu-id="d40f8-138">Flera</span><span class="sxs-lookup"><span data-stu-id="d40f8-138">Multiple</span></span> | <span data-ttu-id="d40f8-139">Det finns flera fält som är partiella i adressen (kan även inkludera StreetPartial och PremisesPartial).</span><span class="sxs-lookup"><span data-stu-id="d40f8-139">There are multiple fields that are partial in the address (potentially also including StreetPartial and PremisesPartial).</span></span> | <span data-ttu-id="d40f8-140">Flera – högst tre</span><span class="sxs-lookup"><span data-stu-id="d40f8-140">Multiple—maximum of three</span></span> |
| <span data-ttu-id="d40f8-141">Inget</span><span class="sxs-lookup"><span data-stu-id="d40f8-141">None</span></span> | <span data-ttu-id="d40f8-142">Adressen är felaktig.</span><span class="sxs-lookup"><span data-stu-id="d40f8-142">Address is incorrect.</span></span> | <span data-ttu-id="d40f8-143">Inget</span><span class="sxs-lookup"><span data-stu-id="d40f8-143">None</span></span> |
| <span data-ttu-id="d40f8-144">NotValidated</span><span class="sxs-lookup"><span data-stu-id="d40f8-144">NotValidated</span></span> | <span data-ttu-id="d40f8-145">Adressen kunde inte skickas genom validerings processen.</span><span class="sxs-lookup"><span data-stu-id="d40f8-145">Address was not able to be sent through the validation process.</span></span>  | <span data-ttu-id="d40f8-146">Inget</span><span class="sxs-lookup"><span data-stu-id="d40f8-146">None</span></span> |

<span data-ttu-id="d40f8-147">När en adress har skickats för att verifieras via ValidateAddress-API: et kommer följande svars schema att returneras:</span><span class="sxs-lookup"><span data-stu-id="d40f8-147">Once an address has been submitted to be validated via the ValidateAddress API, the following response schema will be returned:</span></span>

```csharp

// <summary>
/// Object represents the address validation response.
/// </summary>

public class AddressValidationResponse
{
   /// <summary>
   /// Gets or sets the original address
   /// </summary>
   /// <value>
   /// Original Address
   /// </value>
   public Address OriginalAddress { get; set; }

   /// <summary>
   /// Gets or sets the suggested addresses
   /// </summary>
   /// <value>
   /// Suggested Addresses
   /// </value>
   public List<Address> SuggestedAddresses { get; set; }

   /// <summary>
   /// Gets or sets the validation status
   /// </summary>
   /// <value>
   /// Status
   /// </value>
   public string Status { get; set; }

   /// <summary>
   /// Gets or sets the validation message
   /// </summary>
   /// <value>
   /// Validation Message
   /// </value>
   public string ValidationMessage { get; set; }
   ```

<span data-ttu-id="d40f8-148">Ta en titt på det här exempel svaret.</span><span class="sxs-lookup"><span data-stu-id="d40f8-148">Take a look at this sample response.</span></span> <span data-ttu-id="d40f8-149">Observera att för oss kommer svaret att returnera ytterligare fyrsiffrigt suffix för post nummer linjen om du bara anger fem siffror för post numret.</span><span class="sxs-lookup"><span data-stu-id="d40f8-149">Note that for the US, the response will return an additional four-digit suffix for the postal code line if you only enter five digits for the zip code.</span></span>

```csharp
// IAggregatePartner partnerOperations;
// string customerId;
// s{
"suggested_address": {
    "Country": "US",
    "region": "WA",
    "city": "Redmond",
    "address_line1": "1 Microsoft Way",
    "postal_Code": "98052-8300"
},
"original_address": {
    "Country": "US",
    "region": "WA",
    "city": "Redmond",
    "address_line1": "1 Micro Way",
    "postal_Code": "98052"
},
"status":  "InteractionRequired",
"validation_message": "Address field invalid for property: ‘Street’"
}
```

### <a name="next-steps"></a><span data-ttu-id="d40f8-150">Nästa steg</span><span class="sxs-lookup"><span data-stu-id="d40f8-150">Next steps</span></span>

- <span data-ttu-id="d40f8-151">Dela ditt sandbox-klient-ID med vår ämnes expert (SMF), Ali khaki, som ska ingå i test flygningen så att du kan börja förbereda för uppdateringen.</span><span class="sxs-lookup"><span data-stu-id="d40f8-151">Share your sandbox tenant ID with our subject matter expert (SME), Ali Khaki, to be included in the test flight, so that you can begin preparing for the update.</span></span>

- <span data-ttu-id="d40f8-152">Om du använder en lösning för en kontroll panels leverantör (CPV) bör du kontakta din CPV.</span><span class="sxs-lookup"><span data-stu-id="d40f8-152">If you’re using a control panel vendor (CPV) solution, consult your CPV.</span></span>

### <a name="questions"></a><span data-ttu-id="d40f8-153">Har du några frågor?</span><span class="sxs-lookup"><span data-stu-id="d40f8-153">Questions?</span></span>

<span data-ttu-id="d40f8-154">Om du har några frågor eller behöver support för dina åtgärder med Microsoft, kontakta din partner support Yammer-grupp.</span><span class="sxs-lookup"><span data-stu-id="d40f8-154">If you have any questions or need support for your operations with Microsoft, reach out to your partner support Yammer group.</span></span>

________________
## <a name="new-exchange-admin-center-eac-experience"></a><a name="17"></a><span data-ttu-id="d40f8-155">Ny upplevelse för Exchange administrations Center (UK)</span><span class="sxs-lookup"><span data-stu-id="d40f8-155">New Exchange admin center (EAC) experience</span></span>

### <a name="categories"></a><span data-ttu-id="d40f8-156">Kategorier</span><span class="sxs-lookup"><span data-stu-id="d40f8-156">Categories</span></span>

- <span data-ttu-id="d40f8-157">Datum: 2021-03-29</span><span class="sxs-lookup"><span data-stu-id="d40f8-157">Date: 2021-03-29</span></span>
- <span data-ttu-id="d40f8-158">Funktioner</span><span class="sxs-lookup"><span data-stu-id="d40f8-158">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="d40f8-159">Sammanfattning</span><span class="sxs-lookup"><span data-stu-id="d40f8-159">Summary</span></span>

<span data-ttu-id="d40f8-160">Från och med den 27 april 2021 kommer Exchange administrations Center (UK) att distribuera en ny upplevelse som förbättrar den dagliga effektiviteten för användarna.</span><span class="sxs-lookup"><span data-stu-id="d40f8-160">Starting April 27, 2021, the Exchange admin center (EAC) will roll out a new experience that will improve day-to-day efficiency for users.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="d40f8-161">Förverkad mål grupp</span><span class="sxs-lookup"><span data-stu-id="d40f8-161">Impacted audience</span></span>

<span data-ttu-id="d40f8-162">Delegerade administratörer åtkomst till Exchange via partner Center</span><span class="sxs-lookup"><span data-stu-id="d40f8-162">Delegated admins accessing Exchange through Partner Center</span></span>

### <a name="details"></a><span data-ttu-id="d40f8-163">Information</span><span class="sxs-lookup"><span data-stu-id="d40f8-163">Details</span></span>

<span data-ttu-id="d40f8-164">Från och med den 27 april 2021 kommer partners som navigerar till Exchange via partner Center att omdirigeras till nya UK.</span><span class="sxs-lookup"><span data-stu-id="d40f8-164">Starting April 27, 2021, partners who navigate to Exchange through Partner Center will be redirected to the new EAC.</span></span>

<span data-ttu-id="d40f8-165">Den här nya upplevelsen är för närvarande tillgänglig som en för hands version och administratörer kan aktivera den här funktionen genom att välja växla i det övre högra hörnet i den klassiska UK.</span><span class="sxs-lookup"><span data-stu-id="d40f8-165">This new experience is currently available as a preview, and admins can activate this experience by selecting the toggle on the top right corner within the classic EAC.</span></span> <span data-ttu-id="d40f8-166">De kan också navigera till den nya UKn genom att välja "Prova nu"-banderollen som visas på alla sidor.</span><span class="sxs-lookup"><span data-stu-id="d40f8-166">They can also navigate to the new EAC by selecting the “Try it now” banner that’s displayed on all the pages.</span></span>

<span data-ttu-id="d40f8-167">Fördelarna med nya UK är:</span><span class="sxs-lookup"><span data-stu-id="d40f8-167">Benefits of the new EAC include:</span></span>

- <span data-ttu-id="d40f8-168">Ytterligare insikter, rapporter och aviserings metoder för e-postflöden – relaterade problem.</span><span class="sxs-lookup"><span data-stu-id="d40f8-168">Added insights, reports, and alert mechanisms for mail flow–related issues.</span></span> 

- <span data-ttu-id="d40f8-169">Anpassade instrument paneler för att öka produktiviteten.</span><span class="sxs-lookup"><span data-stu-id="d40f8-169">Personalized dashboards to increase productivity.</span></span>

<span data-ttu-id="d40f8-170">För att hjälpa dig att navigera genom den nya upplevelsen är videor tillgängliga i avsnittet **utbildning &s guide** på den nya UK-upplevelsen.</span><span class="sxs-lookup"><span data-stu-id="d40f8-170">To help you navigate through the new experience, videos are available within the **Training & Guide** section on the new EAC experience.</span></span> <span data-ttu-id="d40f8-171">Du får en översikt över hur du bäst använder den nya portalen.</span><span class="sxs-lookup"><span data-stu-id="d40f8-171">These will give you an overview of how you can best use the new portal.</span></span>

>[!NOTE]
><span data-ttu-id="d40f8-172">Med den här ändringen är den klassiska UK-upplevelsen inte föråldrad.</span><span class="sxs-lookup"><span data-stu-id="d40f8-172">With this change, the classic EAC experience will not be deprecated.</span></span> <span data-ttu-id="d40f8-173">Du får ett meddelande i förväg innan någon ändring implementeras.</span><span class="sxs-lookup"><span data-stu-id="d40f8-173">You will be notified well in advance before any change is implemented.</span></span>

### <a name="next-steps"></a><span data-ttu-id="d40f8-174">Nästa steg</span><span class="sxs-lookup"><span data-stu-id="d40f8-174">Next steps</span></span>

- <span data-ttu-id="d40f8-175">Kolla in [resurserna om det här avsnittet](https://partner.microsoft.com/resources/collection/new-exchange-admin-center-experience#/)där du kan visa skärm dum par av den nya upplevelsen.</span><span class="sxs-lookup"><span data-stu-id="d40f8-175">Check out the [resources about this topic](https://partner.microsoft.com/resources/collection/new-exchange-admin-center-experience#/), where you can view screenshots of the new experience.</span></span>

- <span data-ttu-id="d40f8-176">Dela den här informationen med lämpliga intressenter i din organisation.</span><span class="sxs-lookup"><span data-stu-id="d40f8-176">Share this information with the appropriate stakeholders in your organization.</span></span> 

### <a name="questions"></a><span data-ttu-id="d40f8-177">Har du några frågor?</span><span class="sxs-lookup"><span data-stu-id="d40f8-177">Questions?</span></span>

<span data-ttu-id="d40f8-178">Om du har frågor om dessa ändringar kan du kontrol lera dina relevanta Yammer-communities.</span><span class="sxs-lookup"><span data-stu-id="d40f8-178">For any questions about these changes, check your relevant Yammer communities.</span></span>

________________
## <a name="microsoft-operations-introducing-the-product-launch-calendar"></a><a name="16"></a><span data-ttu-id="d40f8-179">Microsoft-åtgärder: Introduktion till produkt lanserings kalender</span><span class="sxs-lookup"><span data-stu-id="d40f8-179">Microsoft Operations: Introducing the product launch calendar</span></span>

### <a name="categories"></a><span data-ttu-id="d40f8-180">Kategorier</span><span class="sxs-lookup"><span data-stu-id="d40f8-180">Categories</span></span>

- <span data-ttu-id="d40f8-181">Datum: 2021-03-25</span><span class="sxs-lookup"><span data-stu-id="d40f8-181">Date: 2021-03-25</span></span>
- <span data-ttu-id="d40f8-182">Erbjudanden | Modern arbets plats</span><span class="sxs-lookup"><span data-stu-id="d40f8-182">Offers | Modern Workplace</span></span>

### <a name="summary"></a><span data-ttu-id="d40f8-183">Sammanfattning</span><span class="sxs-lookup"><span data-stu-id="d40f8-183">Summary</span></span>

<span data-ttu-id="d40f8-184">Microsoft-åtgärder kommer att effektivisera kommunikationen för produkt lanseringar som svar på feedback från partnern.</span><span class="sxs-lookup"><span data-stu-id="d40f8-184">In response to partner feedback, Microsoft Operations will streamline communications for product launches.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="d40f8-185">Förverkad mål grupp</span><span class="sxs-lookup"><span data-stu-id="d40f8-185">Impacted audience</span></span>

<span data-ttu-id="d40f8-186">Leverantörer av moln lösnings leverantörer (CSP)</span><span class="sxs-lookup"><span data-stu-id="d40f8-186">Cloud Solution Provider (CSP) partners</span></span>

### <a name="details"></a><span data-ttu-id="d40f8-187">Information</span><span class="sxs-lookup"><span data-stu-id="d40f8-187">Details</span></span>

<span data-ttu-id="d40f8-188">Microsoft strävar efter att ständigt förbättra partner upplevelserna.</span><span class="sxs-lookup"><span data-stu-id="d40f8-188">Microsoft is committed to continually improving partner experiences.</span></span> <span data-ttu-id="d40f8-189">Vi har haft feedback från dig att du har fått för många meddelanden från Microsoft, inklusive dubbla meddelanden för produkt lansering.</span><span class="sxs-lookup"><span data-stu-id="d40f8-189">We’ve had feedback from you that you’ve been receiving too many communications from Microsoft, including duplicate announcements for product launches.</span></span>

<span data-ttu-id="d40f8-190">Som svar på din feedback har Microsoft effektiviserat beredskaps upplevelsen för produkt lanseringar för nya och befintliga erbjudanden.</span><span class="sxs-lookup"><span data-stu-id="d40f8-190">In response to your feedback, Microsoft has streamlined the readiness experience for product launches for new and existing offers.</span></span>

<span data-ttu-id="d40f8-191">Nu ger vi dig en enda månatlig visning av produkt lanseringar som publiceras i resurs galleriet för drift beredskap.</span><span class="sxs-lookup"><span data-stu-id="d40f8-191">We now provide you with a single monthly view of product launches, published in the Operations readiness resource gallery.</span></span> <span data-ttu-id="d40f8-192">Den här månads [kalendern för produkt lansering](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) ersätter enskilda produkt lanserings kommunikation i resurs galleriet för drift beredskap och i Partner Center-meddelanden.</span><span class="sxs-lookup"><span data-stu-id="d40f8-192">This monthly [product launch calendar view](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) will replace individual product launch communications in the Operations readiness resource gallery and in Partner Center announcements.</span></span>

<span data-ttu-id="d40f8-193">Du kan också komma åt den här [produkt lanserings kalendern](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) från [Community-samlingar](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/), [kalendervyer](https://partner.microsoft.com/resources/assets#/?type=collection&search=Calendar&sort=updated)och [kryptografiproviders nyhets brev](https://partner.microsoft.com/resources/collection/csp-monthly-update#/).</span><span class="sxs-lookup"><span data-stu-id="d40f8-193">You can also access this [product launch calendar](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) from [community collections](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/), [calendar views](https://partner.microsoft.com/resources/assets#/?type=collection&search=Calendar&sort=updated), and [CSP newsletters](https://partner.microsoft.com/resources/collection/csp-monthly-update#/).</span></span> <span data-ttu-id="d40f8-194">Vi meddelar dig när vi publicerar varje månads produkt lanserings kalender med ett meddelande i resurs galleriet för drift beredskap.</span><span class="sxs-lookup"><span data-stu-id="d40f8-194">We’ll notify you when we publish each month’s product launch calendar with an announcement in the Operations readiness resource gallery.</span></span>

<span data-ttu-id="d40f8-195">Du kan fortfarande hitta information om nya och befintliga erbjudanden i pris listans för hands versions-och pris listans ändrings loggar, samt i produkt Bloggar, licens guider och produkt marknadsförings sidor.</span><span class="sxs-lookup"><span data-stu-id="d40f8-195">You can still find information regarding new and existing offers in the price list preview and price list change logs, as well as in product blogs, licensing guides, and product marketing pages.</span></span>

<span data-ttu-id="d40f8-196">Ändringen gäller för lanseringar för följande produkter:</span><span class="sxs-lookup"><span data-stu-id="d40f8-196">The change will apply to launches for the following products:</span></span>

- <span data-ttu-id="d40f8-197">Lokalt Dynamics</span><span class="sxs-lookup"><span data-stu-id="d40f8-197">Dynamics on-premises</span></span>
- <span data-ttu-id="d40f8-198">Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="d40f8-198">Microsoft 365</span></span>
- <span data-ttu-id="d40f8-199">Microsoft Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="d40f8-199">Microsoft Dynamics 365</span></span>
- <span data-ttu-id="d40f8-200">Windows</span><span class="sxs-lookup"><span data-stu-id="d40f8-200">Windows</span></span>
- <span data-ttu-id="d40f8-201">Server</span><span class="sxs-lookup"><span data-stu-id="d40f8-201">Server</span></span>  
- <span data-ttu-id="d40f8-202">Verktyg</span><span class="sxs-lookup"><span data-stu-id="d40f8-202">Tools</span></span>
- <span data-ttu-id="d40f8-203">Team och Telco</span><span class="sxs-lookup"><span data-stu-id="d40f8-203">Teams and Telco</span></span>

<span data-ttu-id="d40f8-204">Vi kommer att fortsätta att skicka vissa meddelanden om produkt lanseringar som kräver information om drift beredskap.</span><span class="sxs-lookup"><span data-stu-id="d40f8-204">We’ll continue to send specific announcements for product launches that require Operations readiness details.</span></span>

### <a name="next-steps"></a><span data-ttu-id="d40f8-205">Nästa steg</span><span class="sxs-lookup"><span data-stu-id="d40f8-205">Next steps</span></span>

<span data-ttu-id="d40f8-206">Granska resurserna om det här avsnittet och dela den här informationen med lämpliga intressenter i din organisation.</span><span class="sxs-lookup"><span data-stu-id="d40f8-206">Review the resources about this topic and share this information with the appropriate stakeholders in your organization.</span></span>

### <a name="questions"></a><span data-ttu-id="d40f8-207">Har du några frågor?</span><span class="sxs-lookup"><span data-stu-id="d40f8-207">Questions?</span></span>

<span data-ttu-id="d40f8-208">Om du har fler frågor om dessa erbjudanden kan du kontrol lera dina relevanta Yammer-communities.</span><span class="sxs-lookup"><span data-stu-id="d40f8-208">For any further questions about these offers, check your relevant Yammer communities.</span></span>

________________
## <a name="changes-to-csp-customer-onboarding-requirements"></a><a name="15"></a><span data-ttu-id="d40f8-209">Ändringar av CSP-kundens onboarding-krav</span><span class="sxs-lookup"><span data-stu-id="d40f8-209">Changes to CSP customer onboarding requirements</span></span>

### <a name="categories"></a><span data-ttu-id="d40f8-210">Kategorier</span><span class="sxs-lookup"><span data-stu-id="d40f8-210">Categories</span></span>

- <span data-ttu-id="d40f8-211">Datum: 2021-03-25</span><span class="sxs-lookup"><span data-stu-id="d40f8-211">Date: 2021-03-25</span></span>
- <span data-ttu-id="d40f8-212">Funktioner</span><span class="sxs-lookup"><span data-stu-id="d40f8-212">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="d40f8-213">Sammanfattning</span><span class="sxs-lookup"><span data-stu-id="d40f8-213">Summary</span></span>

<span data-ttu-id="d40f8-214">Som en del av vårt åtagande att hjälpa partner och kunder att köra verksamheten baserat på förtroende kommer vi att begära ytterligare kund information, från och med den 25 mars 2021.</span><span class="sxs-lookup"><span data-stu-id="d40f8-214">As part of our commitment to help partners and customers run their business based on trust, we will request additional customer information, effective March 25, 2021.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="d40f8-215">Förverkad mål grupp</span><span class="sxs-lookup"><span data-stu-id="d40f8-215">Impacted audience</span></span>

<span data-ttu-id="d40f8-216">Cloud Solution Provider (CSP) direkta fakturerings partner och indirekta leverantörer som har nya eller befintliga kunder i de länder som anges i nästa avsnitt</span><span class="sxs-lookup"><span data-stu-id="d40f8-216">Cloud Solution Provider (CSP) direct bill partners and indirect providers who have new or existing customers in the countries listed in the next section</span></span>

### <a name="details"></a><span data-ttu-id="d40f8-217">Information</span><span class="sxs-lookup"><span data-stu-id="d40f8-217">Details</span></span>

<span data-ttu-id="d40f8-218">Microsoft körs med förtroende.</span><span class="sxs-lookup"><span data-stu-id="d40f8-218">Microsoft runs on trust.</span></span> <span data-ttu-id="d40f8-219">Vi strävar efter att tillhandahålla en kompatibel, säker och säker metod för kund validering för att agera kund prenumerationer i CSP-programmet.</span><span class="sxs-lookup"><span data-stu-id="d40f8-219">We’re committed to providing a compliant, safe, and secure method of customer validation for transacting customer subscriptions in the CSP program.</span></span> <span data-ttu-id="d40f8-220">Den 25 mars 2021 kommer vi att introduktion till API: er och användar gränssnitts förbättringar i Partner Center som påverkar partner som uppfyller båda följande kriterier:</span><span class="sxs-lookup"><span data-stu-id="d40f8-220">On March 25, 2021, we will be introducing Partner Center API and user interface (UI) enhancements that will affect partners who meet both of the following criteria:</span></span>

1. <span data-ttu-id="d40f8-221">Partnern har en direkt fakturerings relation med Microsoft (vilket innebär att partnern antingen är en direkt fakturerings partner eller en indirekt Provider).</span><span class="sxs-lookup"><span data-stu-id="d40f8-221">The partner has a direct billing relationship with Microsoft (which means that the partner is either a direct bill partner or an indirect provider).</span></span>

2. <span data-ttu-id="d40f8-222">Partnern gör affärer med nya eller befintliga kunder i följande länder:</span><span class="sxs-lookup"><span data-stu-id="d40f8-222">The partner does business with new or existing customers in the following countries:</span></span>

    - <span data-ttu-id="d40f8-223">Thailand</span><span class="sxs-lookup"><span data-stu-id="d40f8-223">Thailand</span></span>
    - <span data-ttu-id="d40f8-224">Vietnam</span><span class="sxs-lookup"><span data-stu-id="d40f8-224">Vietnam</span></span>
    - <span data-ttu-id="d40f8-225">Turkiet</span><span class="sxs-lookup"><span data-stu-id="d40f8-225">Turkey</span></span>
    - <span data-ttu-id="d40f8-226">Polen</span><span class="sxs-lookup"><span data-stu-id="d40f8-226">Poland</span></span>
    - <span data-ttu-id="d40f8-227">Sydafrika</span><span class="sxs-lookup"><span data-stu-id="d40f8-227">South Africa</span></span>
    - <span data-ttu-id="d40f8-228">Indien</span><span class="sxs-lookup"><span data-stu-id="d40f8-228">India</span></span>
    - <span data-ttu-id="d40f8-229">Brasilien</span><span class="sxs-lookup"><span data-stu-id="d40f8-229">Brazil</span></span>
    - <span data-ttu-id="d40f8-230">Irak</span><span class="sxs-lookup"><span data-stu-id="d40f8-230">Iraq</span></span>
    - <span data-ttu-id="d40f8-231">Myanmar</span><span class="sxs-lookup"><span data-stu-id="d40f8-231">Myanmar</span></span>
    - <span data-ttu-id="d40f8-232">Sydsudan</span><span class="sxs-lookup"><span data-stu-id="d40f8-232">South Sudan</span></span>
    - <span data-ttu-id="d40f8-233">Saudiarabien</span><span class="sxs-lookup"><span data-stu-id="d40f8-233">Saudi Arabia</span></span>
    - <span data-ttu-id="d40f8-234">Förenade Arabemiraten</span><span class="sxs-lookup"><span data-stu-id="d40f8-234">United Arab Emirates</span></span>
    - <span data-ttu-id="d40f8-235">Venezuela</span><span class="sxs-lookup"><span data-stu-id="d40f8-235">Venezuela</span></span>

<span data-ttu-id="d40f8-236">Partner som uppfyller kriterierna måste skicka in en kunds **företags registrerings-ID** (även kallat kundens **organisations Inn**) och **telefonnummer** när de utsätter nya kunder eller modifierar befintlig kund information.</span><span class="sxs-lookup"><span data-stu-id="d40f8-236">Partners who meet the criteria will have to submit a customer's **company registration ID** (also known as the customer's **organization INN**) and **phone number** when they onboard new customers or modify existing customer details.</span></span> <span data-ttu-id="d40f8-237">Dessa partner kan också ange ett **mellannamn** för kunden (valfritt).</span><span class="sxs-lookup"><span data-stu-id="d40f8-237">These partners can also enter an optional **middle name** for the customer.</span></span>

<span data-ttu-id="d40f8-238">Observera att när du lägger till ditt företags registrerings-ID bör du använda företagets skatte-ID och inte kundens personliga ID.</span><span class="sxs-lookup"><span data-stu-id="d40f8-238">Note that when you add your company registration ID you should use your business tax ID and not the customer personal ID.</span></span>

<span data-ttu-id="d40f8-239">Partner som gör affärer med nya eller befintliga kunder i följande länder har redan publicerats med en tidigare version i november 2020.</span><span class="sxs-lookup"><span data-stu-id="d40f8-239">Partners who do business with new or existing customers in the following countries have already been onboarded with a previous release in November 2020.</span></span>

- <span data-ttu-id="d40f8-240">Armenien</span><span class="sxs-lookup"><span data-stu-id="d40f8-240">Armenia</span></span>
- <span data-ttu-id="d40f8-241">Azerbajdzjan</span><span class="sxs-lookup"><span data-stu-id="d40f8-241">Azerbaijan</span></span>
- <span data-ttu-id="d40f8-242">Vitryssland</span><span class="sxs-lookup"><span data-stu-id="d40f8-242">Belarus</span></span>
- <span data-ttu-id="d40f8-243">Ungern</span><span class="sxs-lookup"><span data-stu-id="d40f8-243">Hungary</span></span>
- <span data-ttu-id="d40f8-244">Kazakstan</span><span class="sxs-lookup"><span data-stu-id="d40f8-244">Kazakhstan</span></span>
- <span data-ttu-id="d40f8-245">Kirgizistan</span><span class="sxs-lookup"><span data-stu-id="d40f8-245">Kyrgyzstan</span></span>
- <span data-ttu-id="d40f8-246">Moldavien</span><span class="sxs-lookup"><span data-stu-id="d40f8-246">Moldova</span></span>
- <span data-ttu-id="d40f8-247">Ryssland</span><span class="sxs-lookup"><span data-stu-id="d40f8-247">Russia</span></span>
- <span data-ttu-id="d40f8-248">Tadzjikistan</span><span class="sxs-lookup"><span data-stu-id="d40f8-248">Tajikistan</span></span>
- <span data-ttu-id="d40f8-249">Ukraina</span><span class="sxs-lookup"><span data-stu-id="d40f8-249">Ukraine</span></span>
- <span data-ttu-id="d40f8-250">Uzbekistan</span><span class="sxs-lookup"><span data-stu-id="d40f8-250">Uzbekistan</span></span>

<span data-ttu-id="d40f8-251">Partner med kunder i resten av världen kommer att ha möjlighet den 25 mars 2021 att ange **företagets registrerings-ID**, **telefonnummer** och **mellan namn** för kunder som valfri information.</span><span class="sxs-lookup"><span data-stu-id="d40f8-251">Partners with customers in the rest of the world will have the ability on March 25, 2021 to enter the **company registration ID**, **phone number**, and **middle name** for customers as optional details.</span></span>

### <a name="next-steps"></a><span data-ttu-id="d40f8-252">Nästa steg</span><span class="sxs-lookup"><span data-stu-id="d40f8-252">Next steps</span></span>

- <span data-ttu-id="d40f8-253">Läs igenom den tekniska dokumentationen och vanliga frågor och svar i den [dedikerade partner samlingen](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/) för mer detaljerad vägledning.</span><span class="sxs-lookup"><span data-stu-id="d40f8-253">Review the technical documentation and frequently asked questions in the [dedicated partner collection](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/) for more detailed guidance.</span></span>

- <span data-ttu-id="d40f8-254">Förbered för att införliva ändringarna med partner Center API och webb användar upplevelsen.</span><span class="sxs-lookup"><span data-stu-id="d40f8-254">Prepare to incorporate the changes using the Partner Center API and web user experience.</span></span> <span data-ttu-id="d40f8-255">API/SDK: er kommer att vara tillgängliga för testning.</span><span class="sxs-lookup"><span data-stu-id="d40f8-255">API/SDKs will be available for testing.</span></span>

- <span data-ttu-id="d40f8-256">Se till att skicka in ytterligare data när du registrerar nya kunder eller ändrar befintlig kund information.</span><span class="sxs-lookup"><span data-stu-id="d40f8-256">Make sure to submit the additional data when onboarding new customers or modifying existing customer details.</span></span>

- <span data-ttu-id="d40f8-257">Om du använder en lösning för en kontroll panels leverantör (CPV) bör du kontakta din CPV.</span><span class="sxs-lookup"><span data-stu-id="d40f8-257">If you’re using a control panel vendor (CPV) solution, consult your CPV.</span></span>

### <a name="questions"></a><span data-ttu-id="d40f8-258">Har du några frågor?</span><span class="sxs-lookup"><span data-stu-id="d40f8-258">Questions?</span></span>

<span data-ttu-id="d40f8-259">Kontakta din skatte rådgivare eller ditt lokala skatte kontor om du har frågor som rör juridisk identifierare (även kallat INN eller tenn).</span><span class="sxs-lookup"><span data-stu-id="d40f8-259">Contact your tax advisor or local tax office if you have any questions related to the legal identifier (also called INN or TIN).</span></span> <span data-ttu-id="d40f8-260">Microsoft kan inte ge vägledning om skatte frågor.</span><span class="sxs-lookup"><span data-stu-id="d40f8-260">Microsoft cannot provide guidance on tax matters.</span></span>

<span data-ttu-id="d40f8-261">Om du behöver stöd för dina åtgärder med Microsoft [öppnar du en tjänstbegäran](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=aa679372-d996-73df-e244-cb28bbbf28e8).</span><span class="sxs-lookup"><span data-stu-id="d40f8-261">If you need support in your operations with Microsoft, [open a service request](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=aa679372-d996-73df-e244-cb28bbbf28e8).</span></span>

________________
## <a name="corrections-made-to-march-1-2021-perpetual-software-price-list"></a><a name="14"></a><span data-ttu-id="d40f8-262">Korrigeringar gjorda till den 1 mars 2021-pris listan för beständig program vara</span><span class="sxs-lookup"><span data-stu-id="d40f8-262">Corrections made to March 1, 2021 perpetual software price list</span></span>

### <a name="categories"></a><span data-ttu-id="d40f8-263">Kategorier</span><span class="sxs-lookup"><span data-stu-id="d40f8-263">Categories</span></span>

- <span data-ttu-id="d40f8-264">Datum: 2021-03-23</span><span class="sxs-lookup"><span data-stu-id="d40f8-264">Date: 2021-03-23</span></span>
- <span data-ttu-id="d40f8-265">Erbjudanden/marknader</span><span class="sxs-lookup"><span data-stu-id="d40f8-265">Offers/Markets</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="d40f8-266">Förverkad mål grupp</span><span class="sxs-lookup"><span data-stu-id="d40f8-266">Impacted audience</span></span>

<span data-ttu-id="d40f8-267">Indirekta leverantörer och direkta fakturerings partner som agerar med beständig program vara i Cloud Solution Provider-programmet</span><span class="sxs-lookup"><span data-stu-id="d40f8-267">Indirect providers and direct bill partners transacting perpetual software in the Cloud Solution Provider program</span></span> 

### <a name="details"></a><span data-ttu-id="d40f8-268">Information</span><span class="sxs-lookup"><span data-stu-id="d40f8-268">Details</span></span>

<span data-ttu-id="d40f8-269">Pris listan för beständig program vara som publicerades den 1 mars 2021 ingår marknader som inte borde ha funnits där.</span><span class="sxs-lookup"><span data-stu-id="d40f8-269">The price list for perpetual software posted on March 1, 2021 included markets that should not have been there.</span></span> <span data-ttu-id="d40f8-270">Pris listan för beständig program vara uppdaterades den 17 mars 2021 med korrigeringarna.</span><span class="sxs-lookup"><span data-stu-id="d40f8-270">The perpetual software price list was updated on March 17, 2021 with the corrections.</span></span> <span data-ttu-id="d40f8-271">Dessa korrigeringar gäller endast:</span><span class="sxs-lookup"><span data-stu-id="d40f8-271">These corrections were only applicable to:</span></span>

- <span data-ttu-id="d40f8-272">Produkt-ID: DF77X4D43RKT</span><span class="sxs-lookup"><span data-stu-id="d40f8-272">Product ID: DF77X4D43RKT</span></span> 
- <span data-ttu-id="d40f8-273">Produkt namn: Windows 10 Home till Pro-uppgradering för Microsoft 365 Business</span><span class="sxs-lookup"><span data-stu-id="d40f8-273">Product name: Windows 10 Home to Pro Upgrade for Microsoft 365 Business</span></span>
- <span data-ttu-id="d40f8-274">Borttagna eller ej stödda marknader: AE, AF, AL, AM, AO, BA, BB, BD, BH, BM, BN, BO, BR, BS, BW, BZ, CI, CL, CM, CO, CR, FV, DZ, EG, tex, ET, FJ, FO, GE, Last, GT, HN, IL, i, SWEETIQ, JM, Eva, KE, KG, KN, KW, KY, KZ, LB, LK, LY, MA, MC, MD, MN, MO, MK, NA , NI, NP, OM, PA, PE, PH, PK, PR, PY, FRÅGOR OCH SVAR, RS, RU, RW, TG, SN, SA, TH, TJ, TM, TN, TT, TZ, UA, ΜG, UY, UZ, VE, VN, JULEN, ZM, ZW</span><span class="sxs-lookup"><span data-stu-id="d40f8-274">Removed or unsupported markets: AE, AF, AL, AM, AO, BA, BB, BD, BH, BM, BN, BO, BR, BS, BW, BY, BZ, CI, CL, CM, CO, CR, CW, DO, DZ, EC, EG, ET, FJ, FO, GE, GH, GT, HN, IL, IN, IQ, JM, JO, KE, KG, KN, KW, KY, KZ, LB, LK, LY, MA, MC, MD, ME, MN, MO, MU, NA, NG, NI, NP, OM, PA, PE, PH, PK, PR, PY, QA, RS, RU, RW, SG, SN, SV, TH, TJ, TM, TN, TT, TZ, UA, UG, UY, UZ, VE, VN, YE, ZM, ZW</span></span>

<span data-ttu-id="d40f8-275">Dessa ändringar gäller endast för produkten ovan.</span><span class="sxs-lookup"><span data-stu-id="d40f8-275">These changes only apply to the above product.</span></span> <span data-ttu-id="d40f8-276">Andra produkter hade inga ändringar.</span><span class="sxs-lookup"><span data-stu-id="d40f8-276">Other products had no corrections.</span></span> 

### <a name="next-steps-and-resources"></a><span data-ttu-id="d40f8-277">Nästa steg och resurser</span><span class="sxs-lookup"><span data-stu-id="d40f8-277">Next steps and resources</span></span>

- <span data-ttu-id="d40f8-278">Partner som har en Transact-beständig program vara bör ladda ned den senaste pris listan för beständig program vara.</span><span class="sxs-lookup"><span data-stu-id="d40f8-278">Partners who transact perpetual software should download the latest perpetual software price list.</span></span>
- <span data-ttu-id="d40f8-279">Se [lands koderna för regioner](https://docs.microsoft.com/azure/marketplace/commercial-marketplace-co-sell-countries) för en egen mappning av den två bokstavs förkortningen till länder.</span><span class="sxs-lookup"><span data-stu-id="d40f8-279">Consult the [region country codes](https://docs.microsoft.com/azure/marketplace/commercial-marketplace-co-sell-countries) for a friendly mapping of the two letter abbreviation to countries.</span></span>
________________
## <a name="sdk-release-on-net-standard-v1170"></a><a name="13"></a> <span data-ttu-id="d40f8-280">SDK-version på .NET standard (v 1.17.0)</span><span class="sxs-lookup"><span data-stu-id="d40f8-280">SDK Release on .NET Standard (v1.17.0)</span></span>

### <a name="categories"></a><span data-ttu-id="d40f8-281">Kategorier</span><span class="sxs-lookup"><span data-stu-id="d40f8-281">Categories</span></span>

- <span data-ttu-id="d40f8-282">Datum: 2021-03-23</span><span class="sxs-lookup"><span data-stu-id="d40f8-282">Date: 2021-03-23</span></span>

- <span data-ttu-id="d40f8-283">Funktioner</span><span class="sxs-lookup"><span data-stu-id="d40f8-283">Capabilities</span></span>
 
### <a name="impacted-audience"></a><span data-ttu-id="d40f8-284">Förverkad mål grupp</span><span class="sxs-lookup"><span data-stu-id="d40f8-284">Impacted audience</span></span>

<span data-ttu-id="d40f8-285">Direkta fakturerings partner och indirekta leverantörer som deltar i CSP-programmet som använder Partner Center .NET SDK.</span><span class="sxs-lookup"><span data-stu-id="d40f8-285">Direct Bill partners and Indirect Providers participating in the CSP program who are using the Partner Center .NET SDK.</span></span>

### <a name="details"></a><span data-ttu-id="d40f8-286">Information</span><span class="sxs-lookup"><span data-stu-id="d40f8-286">Details</span></span>

<span data-ttu-id="d40f8-287">Från och med mars 23 2020 kan partners börja hämta versionen av [MicrosoftPartnerCenter. NETSDK (NuGet Galleri | Microsoft. Store. PartnerCenter 1.17.0)](https://www.nuget.org/packages/Microsoft.Store.PartnerCenter/1.17.0)tillsammans med uppdaterade offentliga partners Center SDK [GitHub-exempel](https://github.com/Microsoft/Partner-Center-DotNet-Samples).</span><span class="sxs-lookup"><span data-stu-id="d40f8-287">As of March 23 2020, Partners can start downloading the version of [MicrosoftPartnerCenter.NETSDK (NuGet Gallery | Microsoft.Store.PartnerCenter 1.17.0)](https://www.nuget.org/packages/Microsoft.Store.PartnerCenter/1.17.0), along with updated public Partner Center SDK [GitHub samples](https://github.com/Microsoft/Partner-Center-DotNet-Samples).</span></span> <span data-ttu-id="d40f8-288">Den här versionen innehåller uppdateringar av följande metoder:</span><span class="sxs-lookup"><span data-stu-id="d40f8-288">This version includes updates to the following methods:</span></span>

#### <a name="audit-updated-new-operation-types"></a><span data-ttu-id="d40f8-289">Granskning uppdaterad: nya åtgärds typer</span><span class="sxs-lookup"><span data-stu-id="d40f8-289">Audit Updated: New operation types</span></span>

<span data-ttu-id="d40f8-290">Nya [Åtgärds typer](https://docs.microsoft.com/partner-center/develop/auditing-resources) har lagts till för att veta när kunden godkände och avslutade DAP.</span><span class="sxs-lookup"><span data-stu-id="d40f8-290">Added new [operation types](https://docs.microsoft.com/partner-center/develop/auditing-resources) for knowing when the customer approved and terminated DAP.</span></span>

- <span data-ttu-id="d40f8-291">DapAdminRelationshipApproved</span><span class="sxs-lookup"><span data-stu-id="d40f8-291">DapAdminRelationshipApproved</span></span>

- <span data-ttu-id="d40f8-292">DapAdminRelationshipTerminated</span><span class="sxs-lookup"><span data-stu-id="d40f8-292">DapAdminRelationshipTerminated</span></span>

#### <a name="audit-updated-new-resource-and-operation-types"></a><span data-ttu-id="d40f8-293">Granskning uppdaterad: nya resurs-och åtgärds typer</span><span class="sxs-lookup"><span data-stu-id="d40f8-293">Audit Updated: New resource and operation types</span></span>

<span data-ttu-id="d40f8-294">Nya [resurs-och åtgärds typer](https://docs.microsoft.com/partner-center/develop/auditing-resources) har lagts till för att stödja scenariot för kund katalog roller.</span><span class="sxs-lookup"><span data-stu-id="d40f8-294">Added new [resource and operation types](https://docs.microsoft.com/partner-center/develop/auditing-resources) for supporting the customer directory role scenario.</span></span>

- <span data-ttu-id="d40f8-295">Ny resurs typ "CustomerDirectoryRole"</span><span class="sxs-lookup"><span data-stu-id="d40f8-295">New resource type “CustomerDirectoryRole”</span></span>

- <span data-ttu-id="d40f8-296">Åtgärds typer "AddUserMember" och "RemoveUserMember"</span><span class="sxs-lookup"><span data-stu-id="d40f8-296">Operation types “AddUserMember” and “RemoveUserMember”</span></span>

#### <a name="sdk-updates-to-customer-accounts"></a><span data-ttu-id="d40f8-297">SDK-uppdateringar till kund konton</span><span class="sxs-lookup"><span data-stu-id="d40f8-297">SDK Updates to customer accounts</span></span>

- <span data-ttu-id="d40f8-298">Stöd för GET/customers/{customer-tenant-id}/directSignedMicrosoftCustomerAgreementStatus</span><span class="sxs-lookup"><span data-stu-id="d40f8-298">Support for GET /customers/{customer-tenant-id}/directSignedMicrosoftCustomerAgreementStatus</span></span>

- <span data-ttu-id="d40f8-299">Hämta/Customers/{Customer-Tenant-ID}/Qualifications</span><span class="sxs-lookup"><span data-stu-id="d40f8-299">GET /customers/{customer-tenant-id}/qualifications</span></span>

- <span data-ttu-id="d40f8-300">PUBLICERA/Customers/{customer_id}/Qualifications? Code = {validationCode}</span><span class="sxs-lookup"><span data-stu-id="d40f8-300">POST /customers/{customer_id}/qualifications?code={validationCode}</span></span>

#### <a name="additional-changes"></a><span data-ttu-id="d40f8-301">Ytterligare ändringar</span><span class="sxs-lookup"><span data-stu-id="d40f8-301">Additional changes</span></span>

<span data-ttu-id="d40f8-302">Följande ändringar införs som en del av New Commerce och är för närvarande endast tillgängliga genom inbjudan till partner som är en del av M365/D365 nya Commerce Experience Technical Preview.</span><span class="sxs-lookup"><span data-stu-id="d40f8-302">The following changes are introduced as part of New Commerce, and are currently available by invitation only to partners who are part of the M365/D365 New Commerce experience technical preview.</span></span> <span data-ttu-id="d40f8-303">Partner som inte ingår i den nya Commerce Technical Preview bör inte märkas och bör vara bakåtkompatibla.</span><span class="sxs-lookup"><span data-stu-id="d40f8-303">Partners who are not part of the New Commerce technical preview should not notice impacts and should be backward compatible.</span></span>

- <span data-ttu-id="d40f8-304">Katalog ändringar:</span><span class="sxs-lookup"><span data-stu-id="d40f8-304">Catalog Changes:</span></span>

  - <span data-ttu-id="d40f8-305">Hämta/Products/{Product-ID}/SKUs/{SKU-ID}</span><span class="sxs-lookup"><span data-stu-id="d40f8-305">GET /products/{product-id}/skus/{sku-id}</span></span>

- <span data-ttu-id="d40f8-306">Köp och hantera:</span><span class="sxs-lookup"><span data-stu-id="d40f8-306">Purchase and Manage:</span></span>
  - <span data-ttu-id="d40f8-307">Hämta/customers/{customerId}/subscriptions</span><span class="sxs-lookup"><span data-stu-id="d40f8-307">GET /customers/{customerId}/subscriptions</span></span>
  - <span data-ttu-id="d40f8-308">Hämta/customers/{customerId}/subscriptions/{subscriptionId}</span><span class="sxs-lookup"><span data-stu-id="d40f8-308">GET /customers/{customerId}/subscriptions/{subscriptionId}</span></span>
  - <span data-ttu-id="d40f8-309">KORRIGERINGs/customers/{customerId}/subscriptions/{subscriptionId}</span><span class="sxs-lookup"><span data-stu-id="d40f8-309">PATCH /customers/{customerId}/subscriptions/{subscriptionId}</span></span>
  - <span data-ttu-id="d40f8-310">Hämta/customers/{customerId}/subscriptions/{subscriptionId}/transitioneligibilities</span><span class="sxs-lookup"><span data-stu-id="d40f8-310">GET /customers/{customerId}/subscriptions/{subscriptionId}/transitioneligibilities</span></span>
  - <span data-ttu-id="d40f8-311">Hämta/customers/{customerId}/subscriptions/{subscriptionId}/transitions</span><span class="sxs-lookup"><span data-stu-id="d40f8-311">GET /customers/{customerId}/subscriptions/{subscriptionId}/transitions</span></span>
  - <span data-ttu-id="d40f8-312">PUBLICERA/customers/{customerId}/subscriptions/{subscriptionId}/transitions</span><span class="sxs-lookup"><span data-stu-id="d40f8-312">POST /customers/{customerId}/subscriptions/{subscriptionId}/transitions</span></span>

### <a name="next-steps"></a><span data-ttu-id="d40f8-313">Nästa steg</span><span class="sxs-lookup"><span data-stu-id="d40f8-313">Next Steps</span></span>

- <span data-ttu-id="d40f8-314">Ladda ned den senaste versionen [MicrosoftPartnerCenter. NETSDK (NuGet Gallery | Microsoft. Store. PartnerCenter 1.17.0)](https://www.nuget.org/packages/Microsoft.Store.PartnerCenter/1.17.0)</span><span class="sxs-lookup"><span data-stu-id="d40f8-314">Download the latest version [MicrosoftPartnerCenter.NETSDK (NuGet Gallery | Microsoft.Store.PartnerCenter 1.17.0)](https://www.nuget.org/packages/Microsoft.Store.PartnerCenter/1.17.0)</span></span>
- <span data-ttu-id="d40f8-315">Hämta och granska [GitHub-exemplen](https://github.com/Microsoft/Partner-Center-DotNet-Samples)</span><span class="sxs-lookup"><span data-stu-id="d40f8-315">Download and review the [GitHub samples](https://github.com/Microsoft/Partner-Center-DotNet-Samples)</span></span>

________________
## <a name="csp-commercial-marketplace-offer-and-fy21-csp-incentives-for-eligible-offers"></a><a name="12"></a><span data-ttu-id="d40f8-316">Erbjudande om kommersiella Marketplace-erbjudanden och FY21 för berättigade erbjudanden</span><span class="sxs-lookup"><span data-stu-id="d40f8-316">CSP commercial marketplace offer and FY21 CSP incentives for eligible offers</span></span>

### <a name="categories"></a><span data-ttu-id="d40f8-317">Kategorier</span><span class="sxs-lookup"><span data-stu-id="d40f8-317">Categories</span></span>

- <span data-ttu-id="d40f8-318">Datum: 2021-03-18</span><span class="sxs-lookup"><span data-stu-id="d40f8-318">Date: 2021-03-18</span></span>
- <span data-ttu-id="d40f8-319">Funktioner</span><span class="sxs-lookup"><span data-stu-id="d40f8-319">Capabilities</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="d40f8-320">Förverkad mål grupp</span><span class="sxs-lookup"><span data-stu-id="d40f8-320">Impacted audience</span></span>

<span data-ttu-id="d40f8-321">Indirekta leverantörer och direkta fakturerings partner i Cloud Solution Provider-programmet</span><span class="sxs-lookup"><span data-stu-id="d40f8-321">Indirect providers and direct bill partners in the Cloud Solution Provider program</span></span> 

### <a name="details"></a><span data-ttu-id="d40f8-322">Information</span><span class="sxs-lookup"><span data-stu-id="d40f8-322">Details</span></span>

<span data-ttu-id="d40f8-323">Indirekta leverantörer och direkta fakturerings partner i Cloud Solution Provider-programmet kan sälja tredje parts erbjudanden och få rabatt incitament för varje berättigad tredje parts erbjudande i Partner Center eller Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="d40f8-323">Indirect providers and direct bill partners in the Cloud Solution Provider program can sell third party offers and earn a rebate incentive for each eligible third-party offer transacted in Partner Center or the Azure portal.</span></span> <span data-ttu-id="d40f8-324">Stimulans beloppet är i form av en rabatt på fakturerad försäljning för berättigade erbjudanden och är **tillgänglig fram till den 30 juni 2021**.</span><span class="sxs-lookup"><span data-stu-id="d40f8-324">The incentive will be in the form of a rebate on billed sales for the eligible offers and is **available until June 30, 2021**.</span></span>  

<span data-ttu-id="d40f8-325">Fortsätt att lära dig det här erbjudandet om erbjudandet om marknads plats erbjudande nedan och kontakta kunderna idag för att identifiera de rätta erbjudandena för att möjliggöra fortsatt lyckad och digital omvandling.</span><span class="sxs-lookup"><span data-stu-id="d40f8-325">Continue learning about this CSP Commercial Marketplace Offer incentive below and contact your customers today to identify the right offers to enable their continued success and digital transformation.</span></span>

<span data-ttu-id="d40f8-326">Vi samarbetar med oberoende program varu leverantörer (ISV) för att få de senaste IaaS-och SaaS-lösningarna till marknaden för Microsoft-kunder.</span><span class="sxs-lookup"><span data-stu-id="d40f8-326">We partner with Independent Software Vendors (ISVs) to bring the latest IaaS and SaaS solutions to market for Microsoft customers.</span></span> <span data-ttu-id="d40f8-327">ISV-utgivare kan välja att aktivera försäljning av sina erbjudanden via Microsoft Partner Channel.</span><span class="sxs-lookup"><span data-stu-id="d40f8-327">ISV publishers have the option of enabling sales of their offers through the Microsoft partner channel.</span></span> <span data-ttu-id="d40f8-328">Våra incitaments berättigade erbjudanden delas in i två kategorier:</span><span class="sxs-lookup"><span data-stu-id="d40f8-328">Our incentive-eligible offers fall into two categories:</span></span>

- <span data-ttu-id="d40f8-329">Välj SaaS-och IaaS-erbjudanden från tredje part med Azure IP Co-Sälj motiverade status.</span><span class="sxs-lookup"><span data-stu-id="d40f8-329">Select SaaS and IaaS third-party offers with Azure IP co-sell incentivized status.</span></span> 

- <span data-ttu-id="d40f8-330">SaaS-program som är integrerade med team eller minst två Microsoft 365 produktivitets appar, till exempel PowerPoint, Word, Excel, Outlook eller SharePoint.</span><span class="sxs-lookup"><span data-stu-id="d40f8-330">SaaS applications integrated with Teams or at least two Microsoft 365 productivity apps, such as PowerPoint, Word, Excel, Outlook, or SharePoint.</span></span>

### <a name="next-steps-and-resources"></a><span data-ttu-id="d40f8-331">Nästa steg och resurser</span><span class="sxs-lookup"><span data-stu-id="d40f8-331">Next steps and resources</span></span>

- <span data-ttu-id="d40f8-332">Lär dig om bidrags [partner incitament](https://partner.microsoft.com/membership/partner-incentives) för att sälja berättigade Marketplace-appar till de incitament som är berättigade till appar.</span><span class="sxs-lookup"><span data-stu-id="d40f8-332">Learn about earning [Partner Incentives](https://partner.microsoft.com/membership/partner-incentives) for selling eligible marketplace apps the incentive eligible apps.</span></span> <span data-ttu-id="d40f8-333">Nya erbjudanden läggs till varje månad.</span><span class="sxs-lookup"><span data-stu-id="d40f8-333">New offers are added monthly.</span></span>  
- [<span data-ttu-id="d40f8-334">Vår leverantör av moln lösningar direkt fakturerings partner stimulans resurser</span><span class="sxs-lookup"><span data-stu-id="d40f8-334">Cloud Solution Provider direct bill partner incentive resources</span></span>](https://partner.microsoft.com/asset/collection/cloud-solution-provider-direct-partner-incentive-resources#/)
- [<span data-ttu-id="d40f8-335">Moln lösnings leverantörs tjänst för indirekt leverantörs stimulans</span><span class="sxs-lookup"><span data-stu-id="d40f8-335">Cloud Solution Provider indirect provider incentive resources</span></span>](https://partner.microsoft.com/asset/collection/cloud-solution-provider-indirect-provider-incentive-resources#/)
- <span data-ttu-id="d40f8-336">Läs igenom den här [presentationen](https://partner.microsoft.com/resources/detail/partner-center-cm-for-csp-overview-pdf) om du vill veta mer om hur du säljer kommersiella Marketplace-appar.</span><span class="sxs-lookup"><span data-stu-id="d40f8-336">Review this [presentation](https://partner.microsoft.com/resources/detail/partner-center-cm-for-csp-overview-pdf) to learn more about selling the commercial marketplace apps.</span></span> <span data-ttu-id="d40f8-337">Kolla in ytterligare resurser [här](https://partner.microsoft.com/resources/collection/partner-center-cm-for-csp-collection#/).</span><span class="sxs-lookup"><span data-stu-id="d40f8-337">Check out additional resources [here](https://partner.microsoft.com/resources/collection/partner-center-cm-for-csp-collection#/).</span></span> 
- <span data-ttu-id="d40f8-338">Utforska den kommersiella Marketplace-katalogen i [partner Center](https://docs.microsoft.com/partner-center/csp-commercial-marketplace-discover) eller [Azure Portal](https://ms.portal.azure.com/#home)</span><span class="sxs-lookup"><span data-stu-id="d40f8-338">Explore the commercial marketplace catalog in [Partner Center](https://docs.microsoft.com/partner-center/csp-commercial-marketplace-discover) or [Azure portal](https://ms.portal.azure.com/#home)</span></span>
- <span data-ttu-id="d40f8-339">Använd [API: er](https://docs.microsoft.com/partner-center/develop/create-subscription-azure-marketplace-products#get-a-list-of-offers-for-a-market) för att integrera appar i ditt företags marknads plats</span><span class="sxs-lookup"><span data-stu-id="d40f8-339">Use [APIs](https://docs.microsoft.com/partner-center/develop/create-subscription-azure-marketplace-products#get-a-list-of-offers-for-a-market) to integrate apps into your company’s marketplace</span></span>
- <span data-ttu-id="d40f8-340">Kontakta ISV: er som du är intresse rad av att göra affärer med</span><span class="sxs-lookup"><span data-stu-id="d40f8-340">Reach out to ISVs you are interested in doing business with</span></span>
- <span data-ttu-id="d40f8-341">Indirekta leverantörer måste integreras med API: er och guide åter försäljare där appar kan säljas</span><span class="sxs-lookup"><span data-stu-id="d40f8-341">Indirect providers need to integrate using APIs and guide resellers on which apps to sell</span></span>

### <a name="questions"></a><span data-ttu-id="d40f8-342">Har du några frågor?</span><span class="sxs-lookup"><span data-stu-id="d40f8-342">Questions?</span></span>  

<span data-ttu-id="d40f8-343">I [den här artikeln](https://docs.microsoft.com/partner-center/csp-commercial-marketplace-overview) hittar du en översikt över den kommersiella marknads platsen i Partner Center.</span><span class="sxs-lookup"><span data-stu-id="d40f8-343">Refer to [this article](https://docs.microsoft.com/partner-center/csp-commercial-marketplace-overview) for an overview of the commercial marketplace in Partner Center.</span></span>

<span data-ttu-id="d40f8-344">Om du behöver ytterligare hjälp kan du skapa en supportbegäran i Partner Center.</span><span class="sxs-lookup"><span data-stu-id="d40f8-344">If you need additional assistance you can create a support request in Partner Center.</span></span> <span data-ttu-id="d40f8-345">Läs mer på [https://aka.ms/IncentivesSupport](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=1) .</span><span class="sxs-lookup"><span data-stu-id="d40f8-345">Learn more at [https://aka.ms/IncentivesSupport](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=1).</span></span>

________________
## <a name="power-bi-premium-offer-naming-and-prerequisite-update"></a><a name="11"></a><span data-ttu-id="d40f8-346">Power BI Premium erbjuder namngivning och nödvändig uppdatering</span><span class="sxs-lookup"><span data-stu-id="d40f8-346">Power BI Premium offer naming and prerequisite update</span></span>

### <a name="categories"></a><span data-ttu-id="d40f8-347">Kategorier</span><span class="sxs-lookup"><span data-stu-id="d40f8-347">Categories</span></span>

- <span data-ttu-id="d40f8-348">Datum: 2021-03-18</span><span class="sxs-lookup"><span data-stu-id="d40f8-348">Date: 2021-03-18</span></span>
- <span data-ttu-id="d40f8-349">Funktioner</span><span class="sxs-lookup"><span data-stu-id="d40f8-349">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="d40f8-350">Sammanfattning</span><span class="sxs-lookup"><span data-stu-id="d40f8-350">Summary</span></span>

<span data-ttu-id="d40f8-351">Den slutgiltiga pris listan 1 april 2021 kommer att uppdateras för att lägga till klarhet i namngivnings-och/eller nödvändig information för Power BI Premium per användare-erbjudanden.</span><span class="sxs-lookup"><span data-stu-id="d40f8-351">The April 1, 2021 final price list will be updated to add clarity to the naming and/or prerequisite information for Power BI Premium Per User offers.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="d40f8-352">Förverkad mål grupp</span><span class="sxs-lookup"><span data-stu-id="d40f8-352">Impacted audience</span></span>

<span data-ttu-id="d40f8-353">Leverantörer av moln lösningar (CSP), direkta och indirekta partner</span><span class="sxs-lookup"><span data-stu-id="d40f8-353">Cloud Solution Provider (CSP) direct and indirect partners</span></span>

### <a name="details"></a><span data-ttu-id="d40f8-354">Information</span><span class="sxs-lookup"><span data-stu-id="d40f8-354">Details</span></span>

<span data-ttu-id="d40f8-355">Den slutgiltiga pris listan 1 april 2021 kommer att uppdateras för att lägga till klarhet i namngivnings-och/eller nödvändig information för Power BI Premium per användare-erbjudanden.</span><span class="sxs-lookup"><span data-stu-id="d40f8-355">The April 1, 2021 final price list will be updated to add clarity to the naming and/or prerequisite information for Power BI Premium Per User offers.</span></span>

<span data-ttu-id="d40f8-356">Innan den slutgiltiga pris listan har uppdaterats kan du använda informationen i det här avsnittet för att se till att rätt produkt beställs.</span><span class="sxs-lookup"><span data-stu-id="d40f8-356">Until the final price list is updated, use the information in this section to ensure that the correct product is ordered.</span></span>

<span data-ttu-id="d40f8-357">Följande information visar den berörda SKU: n och nödvändig information.</span><span class="sxs-lookup"><span data-stu-id="d40f8-357">The following details show the affected SKU and prerequisite details.</span></span>

| <span data-ttu-id="d40f8-358">Visnings namn för erbjudande 1 mars för hands version av pris lista</span><span class="sxs-lookup"><span data-stu-id="d40f8-358">Offer display name on March 1 price list preview</span></span> |  <span data-ttu-id="d40f8-359">Uppdaterat erbjudandets visnings namn den 1 april, slutgiltiga pris listan</span><span class="sxs-lookup"><span data-stu-id="d40f8-359">Updated offer display name on April 1 final price list</span></span>| <span data-ttu-id="d40f8-360">Erbjudande-ID</span><span class="sxs-lookup"><span data-stu-id="d40f8-360">Offer ID</span></span> |
| ------ | ----------- | ----------- |
| <span data-ttu-id="d40f8-361">Power BI Premium per användare Add-On (prissättning i ideell personal)</span><span class="sxs-lookup"><span data-stu-id="d40f8-361">Power BI Premium Per User Add-On (Nonprofit Staff Pricing)</span></span>  |  <span data-ttu-id="d40f8-362">Power BI Premium per användare Add-On **(Office)** (prissättning i ideell personal)</span><span class="sxs-lookup"><span data-stu-id="d40f8-362">Power BI Premium Per User Add-On **(Office)** (Nonprofit Staff Pricing)</span></span>   | <span data-ttu-id="d40f8-363">31c03289-47ab-4ab0-8df1-03742c127ac6</span><span class="sxs-lookup"><span data-stu-id="d40f8-363">31c03289-47ab-4ab0-8df1-03742c127ac6</span></span>   |

<span data-ttu-id="d40f8-364">Kunder måste ha något av följande krav för att köpa erbjudandet:</span><span class="sxs-lookup"><span data-stu-id="d40f8-364">Customers are required to have any one of the following prerequisites to purchase this offer:</span></span>

| <span data-ttu-id="d40f8-365">Erbjudandets visnings namn</span><span class="sxs-lookup"><span data-stu-id="d40f8-365">Offer display name</span></span> | <span data-ttu-id="d40f8-366">Erbjudande-ID</span><span class="sxs-lookup"><span data-stu-id="d40f8-366">Offer ID</span></span> |
| ------ | ----------- |
| <span data-ttu-id="d40f8-367">Microsoft 365 E5 (pris för ideell personal)</span><span class="sxs-lookup"><span data-stu-id="d40f8-367">Microsoft 365 E5 (Nonprofit Staff Pricing)</span></span>  |  <span data-ttu-id="d40f8-368">31bedf01-9e57-4ece-a53a-d3656a563931</span><span class="sxs-lookup"><span data-stu-id="d40f8-368">31bedf01-9e57-4ece-a53a-d3656a563931</span></span>   |
|   <span data-ttu-id="d40f8-369">Microsoft 365 E5 utan ljud konferens (pris för ideell personal)</span><span class="sxs-lookup"><span data-stu-id="d40f8-369">Microsoft 365 E5 without Audio Conferencing (Nonprofit Staff Pricing)</span></span>|  <span data-ttu-id="d40f8-370">b456810a-c414-4e07-98fc-ef74e8175a09</span><span class="sxs-lookup"><span data-stu-id="d40f8-370">b456810a-c414-4e07-98fc-ef74e8175a09</span></span>|
|   <span data-ttu-id="d40f8-371">Office 365 E5-pris (ideell personal)</span><span class="sxs-lookup"><span data-stu-id="d40f8-371">Office 365 E5 (Nonprofit Staff Pricing)</span></span>| <span data-ttu-id="d40f8-372">ce139fe5-8bd5-47ed-a5be-07c286f8b9e</span><span class="sxs-lookup"><span data-stu-id="d40f8-372">ce139fe5-8bd5-47ed-a5be-07c286f8b9e</span></span>    |
|   <span data-ttu-id="d40f8-373">Utvärderings version av Office 365 E5 (ideell personal)</span><span class="sxs-lookup"><span data-stu-id="d40f8-373">Office 365 E5 (Nonprofit Staff Pricing) Trial</span></span>|  <span data-ttu-id="d40f8-374">2f192efe-608a-4c9c-9d19-2b0b70b0962e</span><span class="sxs-lookup"><span data-stu-id="d40f8-374">2f192efe-608a-4c9c-9d19-2b0b70b0962e</span></span>|
|   <span data-ttu-id="d40f8-375">Office 365 E5 utan ljud konferens (pris för ideell personal)</span><span class="sxs-lookup"><span data-stu-id="d40f8-375">Office 365 E5 without Audio Conferencing (Nonprofit Staff Pricing)</span></span>|  <span data-ttu-id="d40f8-376">c3897426-9f49-4eaf-9b4d-7d9a1c72aef7</span><span class="sxs-lookup"><span data-stu-id="d40f8-376">c3897426-9f49-4eaf-9b4d-7d9a1c72aef7</span></span>|

<span data-ttu-id="d40f8-377">Följande Power BI Premiums erbjudande måste ha ett krav för köp:</span><span class="sxs-lookup"><span data-stu-id="d40f8-377">The following Power BI Premium offer has a prerequisite required for purchase:</span></span>

| <span data-ttu-id="d40f8-378">Erbjudandets visnings namn</span><span class="sxs-lookup"><span data-stu-id="d40f8-378">Offer display name</span></span> | <span data-ttu-id="d40f8-379">Erbjudande-ID</span><span class="sxs-lookup"><span data-stu-id="d40f8-379">Offer ID</span></span> |
| ------ | ----------- |
|   <span data-ttu-id="d40f8-380">Power BI Premium per användare Add-On (prissättning i ideell personal)</span><span class="sxs-lookup"><span data-stu-id="d40f8-380">Power BI Premium Per User Add-On (Nonprofit Staff Pricing)</span></span>|  <span data-ttu-id="d40f8-381">ef0b895b-681B-4026-a5b1-dda182a57d40</span><span class="sxs-lookup"><span data-stu-id="d40f8-381">ef0b895b-681b-4026-a5b1-dda182a57d40</span></span> |

<span data-ttu-id="d40f8-382">Kunder måste ha denna förutsättning för att kunna köpa detta erbjudande:</span><span class="sxs-lookup"><span data-stu-id="d40f8-382">Customers are required to have this prerequisite to purchase this offer:</span></span>

| <span data-ttu-id="d40f8-383">Erbjudandets visnings namn</span><span class="sxs-lookup"><span data-stu-id="d40f8-383">Offer display name</span></span> | <span data-ttu-id="d40f8-384">Erbjudande-ID</span><span class="sxs-lookup"><span data-stu-id="d40f8-384">Offer ID</span></span> |
| ------ |----------|
| <span data-ttu-id="d40f8-385">Power BI Pro (pris för ideell personal)</span><span class="sxs-lookup"><span data-stu-id="d40f8-385">Power BI Pro (Nonprofit Staff Pricing)</span></span>  |   <span data-ttu-id="d40f8-386">cabdfc93-5786-4224-bfd3-35d58f833b35</span><span class="sxs-lookup"><span data-stu-id="d40f8-386">cabdfc93-5786-4224-bfd3-35d58f833b35</span></span> |

### <a name="next-steps"></a><span data-ttu-id="d40f8-387">Nästa steg</span><span class="sxs-lookup"><span data-stu-id="d40f8-387">Next steps</span></span>

<span data-ttu-id="d40f8-388">Granska resurserna om det här avsnittet och dela den här informationen med lämpliga intressenter i din organisation.</span><span class="sxs-lookup"><span data-stu-id="d40f8-388">Review the resources about this topic, and share this information with the appropriate stakeholders in your organization.</span></span>  

### <a name="questions"></a><span data-ttu-id="d40f8-389">Har du några frågor?</span><span class="sxs-lookup"><span data-stu-id="d40f8-389">Questions?</span></span>

<span data-ttu-id="d40f8-390">Om du har frågor om dessa erbjudanden kan du kontrol lera dina relevanta Yammer-communities.</span><span class="sxs-lookup"><span data-stu-id="d40f8-390">For any questions about these offers, check your relevant Yammer communities.</span></span> 

## <a name="march-price-updates-for-microsoft-365-f3"></a><a name="10"></a> <span data-ttu-id="d40f8-391">Pris uppdateringar i mars för Microsoft 365 F3</span><span class="sxs-lookup"><span data-stu-id="d40f8-391">March price updates for Microsoft 365 F3</span></span>

### <a name="categories"></a><span data-ttu-id="d40f8-392">Kategorier</span><span class="sxs-lookup"><span data-stu-id="d40f8-392">Categories</span></span>

- <span data-ttu-id="d40f8-393">Datum: 2021-03-16</span><span class="sxs-lookup"><span data-stu-id="d40f8-393">Date: 2021-03-16</span></span>
- <span data-ttu-id="d40f8-394">Erbjudanden/marknader</span><span class="sxs-lookup"><span data-stu-id="d40f8-394">Offers/Markets</span></span>

### <a name="summary"></a><span data-ttu-id="d40f8-395">Sammanfattning</span><span class="sxs-lookup"><span data-stu-id="d40f8-395">Summary</span></span>

<span data-ttu-id="d40f8-396">Felaktigt mars 2021-pris har korrigerats för Microsoft 365 F3 Storbritannien (GBP) och euro (EUR).</span><span class="sxs-lookup"><span data-stu-id="d40f8-396">Incorrect March 2021 pricing has been corrected for Microsoft 365 F3 British Pound (GBP) and Euro (EUR).</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="d40f8-397">Förverkad mål grupp</span><span class="sxs-lookup"><span data-stu-id="d40f8-397">Impacted audience</span></span>

<span data-ttu-id="d40f8-398">Partner köper Microsoft 365 F3 i GBP eller EUR mellan 1 mars och 17 mars 2021 med hjälp av CSP-programmet (Cloud Solution Provider).</span><span class="sxs-lookup"><span data-stu-id="d40f8-398">Partners purchasing Microsoft 365 F3 in GBP or EUR between March 1 and March 17, 2021 through the Cloud Solution Provider (CSP) program.</span></span>

### <a name="details"></a><span data-ttu-id="d40f8-399">Information</span><span class="sxs-lookup"><span data-stu-id="d40f8-399">Details</span></span>

<span data-ttu-id="d40f8-400">Microsoft har löst felaktig prissättning för Microsoft 365 F3.</span><span class="sxs-lookup"><span data-stu-id="d40f8-400">Microsoft has resolved incorrect pricing for Microsoft 365 F3.</span></span> <span data-ttu-id="d40f8-401">De felaktiga priserna var för GBP och EUR och endast för erbjudanden som köpts mellan 1 mars och 17 mars 2021.</span><span class="sxs-lookup"><span data-stu-id="d40f8-401">The incorrect prices were for GBP and EUR and only for offers purchased between March 1 and March 17, 2021.</span></span> <span data-ttu-id="d40f8-402">De påverkade erbjudandena och valutorna visas nedan.</span><span class="sxs-lookup"><span data-stu-id="d40f8-402">The impacted offers and currencies are listed below.</span></span> 

| <span data-ttu-id="d40f8-403">Erbjudandets namn</span><span class="sxs-lookup"><span data-stu-id="d40f8-403">Offer name</span></span> | <span data-ttu-id="d40f8-404">Valuta</span><span class="sxs-lookup"><span data-stu-id="d40f8-404">Currency</span></span> | <span data-ttu-id="d40f8-405">Erbjudande-ID</span><span class="sxs-lookup"><span data-stu-id="d40f8-405">Offer ID</span></span> | <span data-ttu-id="d40f8-406">Material-ID</span><span class="sxs-lookup"><span data-stu-id="d40f8-406">Material ID</span></span> |
| ------ |----------- |----------- |----------- |
| <span data-ttu-id="d40f8-407">Microsoft 365 F3 (välgörenhet)</span><span class="sxs-lookup"><span data-stu-id="d40f8-407">Microsoft 365 F3 (Charity)</span></span> | <span data-ttu-id="d40f8-408">GBP</span><span class="sxs-lookup"><span data-stu-id="d40f8-408">GBP</span></span> | <span data-ttu-id="d40f8-409">57b722c2-c435-4bfb-9bc8-80509213a13a</span><span class="sxs-lookup"><span data-stu-id="d40f8-409">57b722c2-c435-4bfb-9bc8-80509213a13a</span></span> | <span data-ttu-id="d40f8-410">AAD-11626</span><span class="sxs-lookup"><span data-stu-id="d40f8-410">AAD-11626</span></span> |
| <span data-ttu-id="d40f8-411">Microsoft 365 F3 (kommersiell)</span><span class="sxs-lookup"><span data-stu-id="d40f8-411">Microsoft 365 F3 (Commercial)</span></span> | <span data-ttu-id="d40f8-412">EUR</span><span class="sxs-lookup"><span data-stu-id="d40f8-412">EUR</span></span>| <span data-ttu-id="d40f8-413">3451a3b0-8cda-44a7-bad7-c30be81c4aaa</span><span class="sxs-lookup"><span data-stu-id="d40f8-413">3451a3b0-8cda-44a7-bad7-c30be81c4aaa</span></span> | <span data-ttu-id="d40f8-414">AAA-89898</span><span class="sxs-lookup"><span data-stu-id="d40f8-414">AAA-89898</span></span> |
 
<span data-ttu-id="d40f8-415">Licensen för för hands versionen av mars och april har uppdaterats 16 mars, 17 Pacific, normal tid.</span><span class="sxs-lookup"><span data-stu-id="d40f8-415">The March and April preview license-base price lists were updated March 16, 5PM pacific standard time.</span></span>

### <a name="next-steps"></a><span data-ttu-id="d40f8-416">Nästa steg</span><span class="sxs-lookup"><span data-stu-id="d40f8-416">Next steps</span></span>

- <span data-ttu-id="d40f8-417">Partner bör hämta de aktuella licensbaserade pris listorna, både mars och för hands versionen av april, med dessa pris korrigeringar om det är tillämpligt.</span><span class="sxs-lookup"><span data-stu-id="d40f8-417">Partners should redownload the current license-based price lists, both March and the April preview, with these price corrections if applicable.</span></span>  
- <span data-ttu-id="d40f8-418">Microsoft kontaktar berörda partner i kommande veckor via e-post för att informera dem om nästa steg som rör korrigering av berörda transaktioner.</span><span class="sxs-lookup"><span data-stu-id="d40f8-418">Microsoft will be contacting impacted partners in the coming weeks via email to inform them of next steps related to correcting affected transactions.</span></span>

### <a name="questions"></a><span data-ttu-id="d40f8-419">Har du några frågor?</span><span class="sxs-lookup"><span data-stu-id="d40f8-419">Questions?</span></span>

<span data-ttu-id="d40f8-420">Om du behöver fler frågor kontrollerar du dina relevanta CSP-communities.</span><span class="sxs-lookup"><span data-stu-id="d40f8-420">For any further questions please check your relevant CSP Yammer communities.</span></span>

________________

## <a name="update-a-legal-company-name-through-partner-center"></a><a name="9"></a> <span data-ttu-id="d40f8-421">Uppdatera ett juridiskt företags namn via partner Center</span><span class="sxs-lookup"><span data-stu-id="d40f8-421">Update a legal company name through Partner Center</span></span>

### <a name="categories"></a><span data-ttu-id="d40f8-422">Kategorier</span><span class="sxs-lookup"><span data-stu-id="d40f8-422">Categories</span></span>

- <span data-ttu-id="d40f8-423">Datum: 2021-03-16</span><span class="sxs-lookup"><span data-stu-id="d40f8-423">Date: 2021-03-16</span></span>
- <span data-ttu-id="d40f8-424">& skala för enhets effektivitet</span><span class="sxs-lookup"><span data-stu-id="d40f8-424">Drive Efficiency & Scale</span></span>

### <a name="summary"></a><span data-ttu-id="d40f8-425">Sammanfattning</span><span class="sxs-lookup"><span data-stu-id="d40f8-425">Summary</span></span>

<span data-ttu-id="d40f8-426">Från och med 2021 mars, Microsoft Partner Network (MPN) partner och indirekt åter försäljare av moln lösnings leverantör kan uppdatera sitt juridiska företags namn via partner Center.</span><span class="sxs-lookup"><span data-stu-id="d40f8-426">Starting March 2021, Microsoft Partner Network (MPN) partners and Cloud Solution Provider (CSP) indirect resellers can update their legal company name through Partner Center.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="d40f8-427">Förverkad mål grupp</span><span class="sxs-lookup"><span data-stu-id="d40f8-427">Impacted audience</span></span>

<span data-ttu-id="d40f8-428">MPN-partner och indirekta CSP-åter försäljare (gäller inte för CSP direkt fakturerings partner)</span><span class="sxs-lookup"><span data-stu-id="d40f8-428">MPN partners and CSP indirect resellers (not applicable to CSP direct bill partners)</span></span>

### <a name="details"></a><span data-ttu-id="d40f8-429">Information</span><span class="sxs-lookup"><span data-stu-id="d40f8-429">Details</span></span>

<span data-ttu-id="d40f8-430">Från och med 2021 mars kan MPN-partner och indirekta CSP-återförsäljare uppdatera sitt juridiska företags namn via partner Center på ett kompatibelt och självständigt sätt.</span><span class="sxs-lookup"><span data-stu-id="d40f8-430">Starting March 2021, MPN partners and CSP indirect resellers can update their legal company name through Partner Center in a compliant, self-serve manner.</span></span> <span data-ttu-id="d40f8-431">Med den här nya funktionen behöver partners inte längre skicka ett support ärende för partner Center för att uppdatera företagets namn.</span><span class="sxs-lookup"><span data-stu-id="d40f8-431">With this new feature, partners will no longer need to submit a Partner Center support ticket to update their company name.</span></span> <span data-ttu-id="d40f8-432">Detta sparar en betydande del av tiden för partner när du utför dessa aktiviteter.</span><span class="sxs-lookup"><span data-stu-id="d40f8-432">This will save a significant amount of time for partners when performing these activities.</span></span> 

<span data-ttu-id="d40f8-433">Mer information finns i [Uppdatera din juridiska företags profil](../update-your-partner-profile.md#update-your-legal-business-profile).</span><span class="sxs-lookup"><span data-stu-id="d40f8-433">To learn more, see [Update your legal business profile](../update-your-partner-profile.md#update-your-legal-business-profile).</span></span>

>[!NOTE]
><span data-ttu-id="d40f8-434">Se till att företags namnet i din juridiska företags profil är fritt från stavfel och förkortningar, och exakt matchar dina formella företags registrerings poster.</span><span class="sxs-lookup"><span data-stu-id="d40f8-434">Ensure that the company name in your legal business profile is free of spelling errors and abbreviations, and exactly matches your formal company business registration records.</span></span> <span data-ttu-id="d40f8-435">Mer information om hur du uppdaterar din organisations profil finns i [Verifiera din organisations profil](../update-your-partner-profile.md#update-your-legal-business-profile).</span><span class="sxs-lookup"><span data-stu-id="d40f8-435">For more information on updating your organization profile, refer to [Verify your organization profile](../update-your-partner-profile.md#update-your-legal-business-profile).</span></span>

### <a name="next-steps"></a><span data-ttu-id="d40f8-436">Nästa steg</span><span class="sxs-lookup"><span data-stu-id="d40f8-436">Next steps</span></span>

<span data-ttu-id="d40f8-437">Dela den här informationen i din organisation så att rätt team kan granska och uppdatera sina processer.</span><span class="sxs-lookup"><span data-stu-id="d40f8-437">Share this information within your organization so that the appropriate team can review and update their processes.</span></span>

### <a name="questions"></a><span data-ttu-id="d40f8-438">Har du några frågor?</span><span class="sxs-lookup"><span data-stu-id="d40f8-438">Questions?</span></span>

<span data-ttu-id="d40f8-439">Om du behöver fler frågor kontrollerar du dina relevanta CSP-communities.</span><span class="sxs-lookup"><span data-stu-id="d40f8-439">For any further questions please check your relevant CSP Yammer communities.</span></span>

________________
## <a name="update-to-cloud-solution-provider-csp-program-evolution-and-open-license-program-changes"></a><a name="8"></a> <span data-ttu-id="d40f8-440">Uppdatera till program utveckling i Cloud Solution Provider (CSP) och öppna licens programs ändringar</span><span class="sxs-lookup"><span data-stu-id="d40f8-440">Update to Cloud Solution Provider (CSP) program evolution and Open License program changes</span></span>

### <a name="categories"></a><span data-ttu-id="d40f8-441">Kategorier</span><span class="sxs-lookup"><span data-stu-id="d40f8-441">Categories</span></span>

- <span data-ttu-id="d40f8-442">Datum: 2021-03-15</span><span class="sxs-lookup"><span data-stu-id="d40f8-442">Date: 2021-03-15</span></span>
- <span data-ttu-id="d40f8-443">Funktioner</span><span class="sxs-lookup"><span data-stu-id="d40f8-443">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="d40f8-444">Sammanfattning</span><span class="sxs-lookup"><span data-stu-id="d40f8-444">Summary</span></span>

<span data-ttu-id="d40f8-445">Nya program varor från kommersiell och offentlig sektor kommer till program vara från Cloud Solution Provider (CSP) tillsammans med ändringar i Open License-programmet.</span><span class="sxs-lookup"><span data-stu-id="d40f8-445">New commercial and public sector perpetual software offers are coming to the Cloud Solution Provider (CSP) program along with changes to the Open Licensing program.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="d40f8-446">Förverkad mål grupp</span><span class="sxs-lookup"><span data-stu-id="d40f8-446">Impacted audience</span></span>

<span data-ttu-id="d40f8-447">Kommersiella åter försäljare och hanterade åter försäljare som säljer genom Open License-programmet, samt alla CSP-partner som agerar beständig program vara</span><span class="sxs-lookup"><span data-stu-id="d40f8-447">Commercial distributors and managed resellers selling through the Open License program, as well as all CSP partners transacting perpetual software</span></span>

### <a name="details"></a><span data-ttu-id="d40f8-448">Information</span><span class="sxs-lookup"><span data-stu-id="d40f8-448">Details</span></span>

<span data-ttu-id="d40f8-449">I september 2020 [presenterade](https://blogs.partner.microsoft.com/mpn/expanding-opportunities-for-partners-in-the-cloud-solution-provider-program/) Microsoft en serie steg i vår digitala omvandlings resa för att utöka möjligheterna till partner i CSP-programmet, inklusive tillgängligheten för lokala program för partner.</span><span class="sxs-lookup"><span data-stu-id="d40f8-449">In September 2020, Microsoft [announced](https://blogs.partner.microsoft.com/mpn/expanding-opportunities-for-partners-in-the-cloud-solution-provider-program/) a series of steps in our digital transformation journey to expand opportunities to partners in the CSP program, including the availability of on-premises software for partners.</span></span> <span data-ttu-id="d40f8-450">De här ändringarna gör det möjligt för partner att växa sin verksamhet och utöka sin räckvidd genom att använda program varu licenser i CSP och placera dem på framgång i dagens moln – första världen.</span><span class="sxs-lookup"><span data-stu-id="d40f8-450">These changes enable partners to grow their business and extend their reach by leveraging software licenses in CSP, positioning them for success in today’s cloud-first world.</span></span> <span data-ttu-id="d40f8-451">De ger också kunderna till gång till molnet och ger partner den flexibilitet som krävs för kundernas hybrid moln miljöer.</span><span class="sxs-lookup"><span data-stu-id="d40f8-451">They also empower customers’ transitions to the cloud and give partners the flexibility needed for customer hybrid cloud environments.</span></span>

<span data-ttu-id="d40f8-452">Vi presenterar följande ändringar i fortsättningen på den här digitala omvandlingen:</span><span class="sxs-lookup"><span data-stu-id="d40f8-452">In continuation of this digital transformation, we are announcing the following changes:</span></span>

- <span data-ttu-id="d40f8-453">1 juli 2021: inga nya SKU: er, produkter eller kampanjer läggs till i pris listan öppna licens program.</span><span class="sxs-lookup"><span data-stu-id="d40f8-453">July 1, 2021:  No new SKUs, products, or promotions will be added to the Open License program price list.</span></span>

- <span data-ttu-id="d40f8-454">7 juli 2021: två kommersiella erbjudanden, få äkta Windows-och Visual Studio Professional-erbjudanden och offentliga sektor erbjudanden (myndigheter, utbildning och icke-vinst – se [meddelande](./2020-december.md#9)) läggs till i listan med program varu pris listan med kryptografiprovider.</span><span class="sxs-lookup"><span data-stu-id="d40f8-454">July 7, 2021:  Two commercial offers, Get Genuine Windows and Visual Studio Professional, and public sector offers (government, education and nonprofit – see [announcement](./2020-december.md#9)) will be added to the CSP perpetual software price list.</span></span>  <span data-ttu-id="d40f8-455">Pris listan finns i avsnittet program vara på sidan [sälj > priser för pris &](https://partnercenter.microsoft.com/pcv/sales) i Partner Center och kommer att publiceras på detta datum igen.</span><span class="sxs-lookup"><span data-stu-id="d40f8-455">The price list can be found in the Software section of the [Sell > Pricing & Offers](https://partnercenter.microsoft.com/pcv/sales) page in Partner Center and will be republished on this date.</span></span>

<span data-ttu-id="d40f8-456">Fullständig information om hur du kan utveckla CSP-program och öppna licens program ändringar finns i **Nästa steg** nedan.</span><span class="sxs-lookup"><span data-stu-id="d40f8-456">For full details regarding the CSP program evolution and Open License program changes, please see **Next Steps** below.</span></span>

### <a name="next-steps"></a><span data-ttu-id="d40f8-457">Nästa steg:</span><span class="sxs-lookup"><span data-stu-id="d40f8-457">Next Steps:</span></span>

- <span data-ttu-id="d40f8-458">Utveckling av CSP-program: granska den ständiga [program varan i Cloud solution providers program](https://partner.microsoft.com/resources/collection/software-in-csp#/) beredskap material.</span><span class="sxs-lookup"><span data-stu-id="d40f8-458">CSP Program evolution:  Review the [Perpetual software in the Cloud Solution Provider program](https://partner.microsoft.com/resources/collection/software-in-csp#/) readiness materials.</span></span> <span data-ttu-id="d40f8-459">Använd den här [beredskaps kartan](https://partner.microsoft.com/resources/detail/software-in-csp-readiness-map-pdf) för att snabbt hitta rätt information för din roll.</span><span class="sxs-lookup"><span data-stu-id="d40f8-459">Use this [readiness map](https://partner.microsoft.com/resources/detail/software-in-csp-readiness-map-pdf) to quickly locate the right information for your role.</span></span>

- <span data-ttu-id="d40f8-460">Öppna licens program ändringar: granska [CSP-programmets utveckling och öppna licens programmet ändrar](https://partner.microsoft.com/resources/collection/csp-open-evolution-to-a-better-experience#/) beredskaps material.</span><span class="sxs-lookup"><span data-stu-id="d40f8-460">Open License program changes:  Review the [CSP program evolution and Open License program changes](https://partner.microsoft.com/resources/collection/csp-open-evolution-to-a-better-experience#/) readiness materials.</span></span> <span data-ttu-id="d40f8-461">Använd den här [beredskaps kartan](https://partner.microsoft.com/resources/detail/csp-open-evolution-to-a-better-experience-readiness-map-pdf) för att snabbt hitta rätt information för din roll.</span><span class="sxs-lookup"><span data-stu-id="d40f8-461">Use this [readiness map](https://partner.microsoft.com/resources/detail/csp-open-evolution-to-a-better-experience-readiness-map-pdf) to quickly locate the right information for your role.</span></span>

### <a name="questions"></a><span data-ttu-id="d40f8-462">Frågor</span><span class="sxs-lookup"><span data-stu-id="d40f8-462">Questions</span></span>

<span data-ttu-id="d40f8-463">Om du behöver fler frågor kontrollerar du dina relevanta CSP-communities.</span><span class="sxs-lookup"><span data-stu-id="d40f8-463">For any further questions please check your relevant CSP Yammer communities.</span></span>

_______________
## <a name="update-to-a-previous-announcement-premium-assessments-an-add-on-to-compliance-manager"></a><a name="7"></a><span data-ttu-id="d40f8-464">Uppdatera till ett tidigare meddelande: Premium-utvärderingar, ett tillägg till Compliance Manager</span><span class="sxs-lookup"><span data-stu-id="d40f8-464">Update to a previous announcement: Premium Assessments, an add-on to Compliance Manager</span></span>

### <a name="categories"></a><span data-ttu-id="d40f8-465">Kategorier</span><span class="sxs-lookup"><span data-stu-id="d40f8-465">Categories</span></span>

- <span data-ttu-id="d40f8-466">Datum: 2021-03-15</span><span class="sxs-lookup"><span data-stu-id="d40f8-466">Date: 2021-03-15</span></span>
- <span data-ttu-id="d40f8-467">Utveckla verksamheten</span><span class="sxs-lookup"><span data-stu-id="d40f8-467">Grow your business</span></span>

### <a name="summary"></a><span data-ttu-id="d40f8-468">Sammanfattning</span><span class="sxs-lookup"><span data-stu-id="d40f8-468">Summary</span></span>

<span data-ttu-id="d40f8-469">Utvärderings versionen har inte listats i pris listan och kommer att tas bort.</span><span class="sxs-lookup"><span data-stu-id="d40f8-469">The trial offers shouldn’t have been listed on the price list and will be removed.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="d40f8-470">Förverkad mål grupp</span><span class="sxs-lookup"><span data-stu-id="d40f8-470">Impacted audience</span></span>

<span data-ttu-id="d40f8-471">Partner som agerar via Cloud Solution Provider</span><span class="sxs-lookup"><span data-stu-id="d40f8-471">Partners transacting through Cloud Solution Provider</span></span>

### <a name="details"></a><span data-ttu-id="d40f8-472">Information</span><span class="sxs-lookup"><span data-stu-id="d40f8-472">Details</span></span>

<span data-ttu-id="d40f8-473">Utvärderings versionen får inte ha inkluderats i pris listan.</span><span class="sxs-lookup"><span data-stu-id="d40f8-473">The trial offers shouldn’t have been included in the price list.</span></span> <span data-ttu-id="d40f8-474">De kommer att tas bort från pris listan 1 maj 2021.</span><span class="sxs-lookup"><span data-stu-id="d40f8-474">These will be removed from the May 1, 2021 price list.</span></span>

<span data-ttu-id="d40f8-475">Det ursprungliga meddelandet är [här](./2021-february.md#4).</span><span class="sxs-lookup"><span data-stu-id="d40f8-475">The original announcement is [here](./2021-february.md#4).</span></span>

### <a name="additional-resources"></a><span data-ttu-id="d40f8-476">Ytterligare resurser</span><span class="sxs-lookup"><span data-stu-id="d40f8-476">Additional resources</span></span>

- [<span data-ttu-id="d40f8-477">Microsoft 365 E5-säkerhet och efterlevnad</span><span class="sxs-lookup"><span data-stu-id="d40f8-477">Microsoft 365 E5 security and compliance</span></span>](https://www.microsoft.com/licensing/product-licensing/microsoft-365-enterprise?activetab=m365-enterprise:primaryr5)

- [<span data-ttu-id="d40f8-478">Bygga och hantera utvärderingar i Microsoft Compliance Manager – Microsoft 365 efterlevnad</span><span class="sxs-lookup"><span data-stu-id="d40f8-478">Build and manage assessments in Microsoft Compliance Manager - Microsoft 365 Compliance</span></span>](/microsoft-365/compliance/compliance-manager-assessments)

### <a name="next-steps"></a><span data-ttu-id="d40f8-479">Nästa steg</span><span class="sxs-lookup"><span data-stu-id="d40f8-479">Next steps</span></span>

<span data-ttu-id="d40f8-480">Granska resurserna om det här avsnittet och dela den här informationen med lämpliga intressenter i din organisation.</span><span class="sxs-lookup"><span data-stu-id="d40f8-480">Review the resources about this topic, and share this information with the appropriate stakeholders in your organization.</span></span>

### <a name="questions"></a><span data-ttu-id="d40f8-481">Har du några frågor?</span><span class="sxs-lookup"><span data-stu-id="d40f8-481">Questions?</span></span>

<span data-ttu-id="d40f8-482">Om du har frågor om dessa erbjudanden kan du kontrol lera dina relevanta Yammer-communities.</span><span class="sxs-lookup"><span data-stu-id="d40f8-482">For questions about these offers, check your relevant Yammer communities.</span></span>

________________
## <a name="migrate-your-solutions-from-one-commercial-partner-ocp-go-to-market-gtm-to-the-microsoft-commercial-marketplace"></a><a name="6"></a> <span data-ttu-id="d40f8-483">Migrera dina lösningar från en kommersiell partner (OCP) go-to-Marketing (GTM) till Microsofts kommersiella marknads plats</span><span class="sxs-lookup"><span data-stu-id="d40f8-483">Migrate your solutions from One Commercial Partner (OCP) go-to market (GTM) to the Microsoft commercial marketplace</span></span>

### <a name="categories"></a><span data-ttu-id="d40f8-484">Kategorier</span><span class="sxs-lookup"><span data-stu-id="d40f8-484">Categories</span></span>

- <span data-ttu-id="d40f8-485">Datum: 2021-03-12</span><span class="sxs-lookup"><span data-stu-id="d40f8-485">Date: 2021-03-12</span></span>
- <span data-ttu-id="d40f8-486">Funktioner</span><span class="sxs-lookup"><span data-stu-id="d40f8-486">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="d40f8-487">Sammanfattning</span><span class="sxs-lookup"><span data-stu-id="d40f8-487">Summary</span></span>

<span data-ttu-id="d40f8-488">Från och med den 29 mars 2021 kommer du att börja uppleva begränsade en OCP-funktion (kommersiell partner) (GTM).</span><span class="sxs-lookup"><span data-stu-id="d40f8-488">From March 29, 2021, you will begin to experience limited One Commercial Partner (OCP) go-to market (GTM) capabilities.</span></span> <span data-ttu-id="d40f8-489">Vi rekommenderar att du migrerar dina lösningar till den kommersiella marknads platsen i Partner Center.</span><span class="sxs-lookup"><span data-stu-id="d40f8-489">We encourage you to migrate your solutions to the commercial marketplace in Partner Center.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="d40f8-490">Förverkad mål grupp</span><span class="sxs-lookup"><span data-stu-id="d40f8-490">Impacted audience</span></span>

<span data-ttu-id="d40f8-491">Organisationer som samsäljs med lösningar i OCP-GTM</span><span class="sxs-lookup"><span data-stu-id="d40f8-491">Organizations co-selling with solutions in OCP GTM</span></span>

### <a name="details"></a><span data-ttu-id="d40f8-492">Information</span><span class="sxs-lookup"><span data-stu-id="d40f8-492">Details</span></span>

<span data-ttu-id="d40f8-493">I december 2020 startade vi vår resa från Microsoft OCP GTM-verktyget till Microsofts kommersiella marknads plats i Partner Center.</span><span class="sxs-lookup"><span data-stu-id="d40f8-493">In December 2020, we started our journey from the Microsoft OCP GTM tool to the Microsoft commercial marketplace in Partner Center.</span></span> <span data-ttu-id="d40f8-494">Den här över gången utökar funktionerna i den kommersiella marknads platsen där du kan presentera dina lösningar på miljon tals kunder, som dubbelriktat delar affärs möjligheter med andra Microsoft-och partner-säljare, och gemensamt säljer innovativa lösningar.</span><span class="sxs-lookup"><span data-stu-id="d40f8-494">This transition expands the capabilities of the commercial marketplace where you can showcase your solutions to millions of customers, bidirectionally share opportunities with other Microsoft and partner sellers, and jointly sell innovative solutions.</span></span>

<span data-ttu-id="d40f8-495">Nästa mil stolpe i över gången kommer att ske den 29 mars 2021.</span><span class="sxs-lookup"><span data-stu-id="d40f8-495">The next milestone in the transition will take place on March 29, 2021.</span></span> <span data-ttu-id="d40f8-496">Det är när du börjar uppleva begränsade OCP GTM-funktioner, och vissa fält blir skrivskyddade.</span><span class="sxs-lookup"><span data-stu-id="d40f8-496">That’s when you’ll begin to experience limited OCP GTM capabilities, with some fields becoming read-only.</span></span> <span data-ttu-id="d40f8-497">Om du för närvarande samverkar med lösningar i OCP GTM, rekommenderar vi att du migrerar dina lösningar till den kommersiella marknaden för att dra nytta av dess funktioner och förenkla publicerings upplevelsen.</span><span class="sxs-lookup"><span data-stu-id="d40f8-497">If you’re currently co-selling with solutions in OCP GTM, we encourage you to migrate your solutions to the commercial marketplace to take advantage of its capabilities and simplify your publishing experience.</span></span> 

<span data-ttu-id="d40f8-498">Om du flyttar till den kommersiella marknads platsen blir partner Center det främsta målet för publicerings upplevelsen i Co-försäljningen.</span><span class="sxs-lookup"><span data-stu-id="d40f8-498">Moving to the commercial marketplace makes Partner Center the primary destination for the co-sell publishing experience.</span></span> <span data-ttu-id="d40f8-499">Det är här du kan fortsätta att växa din verksamhet genom att ansluta dina lösningar till våra delade kunder via samma kanaler och produkt upplevelser som vi använder för Microsoft-produkter.</span><span class="sxs-lookup"><span data-stu-id="d40f8-499">It’s where you can continue to grow your business by connecting your solutions with our shared customers through the same channels and in-product experiences that we use for Microsoft products.</span></span> <span data-ttu-id="d40f8-500">[Läs mer om den kommersiella marknads platsen](https://blogs.partner.microsoft.com/mpn/getting-started-with-the-microsoft-commercial-marketplace/).</span><span class="sxs-lookup"><span data-stu-id="d40f8-500">[Learn more about the commercial marketplace](https://blogs.partner.microsoft.com/mpn/getting-started-with-the-microsoft-commercial-marketplace/).</span></span>

### <a name="next-steps"></a><span data-ttu-id="d40f8-501">Nästa steg</span><span class="sxs-lookup"><span data-stu-id="d40f8-501">Next steps</span></span>

- <span data-ttu-id="d40f8-502">Om du inte har flyttat dina lösningar än följer du instruktionerna som beskrivs i [över gångs guiden](/azure/marketplace/co-sell-solution-migration) eller visar [själv studie kursen](https://partner.microsoft.com/asset/detail/ocp-gtm-to-the-microsoft-commercial-marketplace-mp4) för att slutföra alla migreringsåtgärder och börja publicera dina lösningar på den kommersiella Marketplace.</span><span class="sxs-lookup"><span data-stu-id="d40f8-502">If you have not yet moved your solutions, follow the instructions detailed in the [transition guide](/azure/marketplace/co-sell-solution-migration) or view the [step-by-step video tutorial](https://partner.microsoft.com/asset/detail/ocp-gtm-to-the-microsoft-commercial-marketplace-mp4) to complete all migration activities and start publishing your solution(s) in the commercial marketplace.</span></span>

- <span data-ttu-id="d40f8-503">Om du har frågor om den begränsade kapacitets upplevelsen i OCP-GTM kan du Visa [samförsäljnings kraven för att publicera på vanliga frågor och svar om Microsoft kommersiella Marketplace](https://partner.microsoft.com/resources/detail/co-sell-requirements-publish-commercial-marketplace-faq-pdf).</span><span class="sxs-lookup"><span data-stu-id="d40f8-503">For questions regarding the limited capability experience in OCP GTM, view the [Co-sell requirements to publish in the Microsoft commercial marketplace FAQ](https://partner.microsoft.com/resources/detail/co-sell-requirements-publish-commercial-marketplace-faq-pdf).</span></span> <span data-ttu-id="d40f8-504">(Mer information finns i avsnittet "OCP GTM Limited capabilitity Started 29 mars 2021.")</span><span class="sxs-lookup"><span data-stu-id="d40f8-504">(See the section “OCP GTM limited capabilities starting March 29, 2021.”)</span></span>

### <a name="questions"></a><span data-ttu-id="d40f8-505">Har du några frågor?</span><span class="sxs-lookup"><span data-stu-id="d40f8-505">Questions?</span></span>

<span data-ttu-id="d40f8-506">Kontakta [supporten](https://partner.microsoft.com/support/?stage=1) om du har några frågor eller behöver mer information.</span><span class="sxs-lookup"><span data-stu-id="d40f8-506">Contact [Support](https://partner.microsoft.com/support/?stage=1) if you have any questions or need more information.</span></span>

________________
## <a name="expanding-the-new-commerce-experience-in-the-cloud-solution-provider-csp-program-for-azure-to-russia"></a><a name="5"></a><span data-ttu-id="d40f8-507">Expandera den nya Commerce-upplevelsen i Cloud Solution Provider (CSP)-programmet för Azure till Ryssland</span><span class="sxs-lookup"><span data-stu-id="d40f8-507">Expanding the new commerce experience in the Cloud Solution Provider (CSP) program for Azure to Russia</span></span>

### <a name="categories"></a><span data-ttu-id="d40f8-508">Kategorier</span><span class="sxs-lookup"><span data-stu-id="d40f8-508">Categories</span></span>

- <span data-ttu-id="d40f8-509">Datum: 2021-03-10</span><span class="sxs-lookup"><span data-stu-id="d40f8-509">Date: 2021-03-10</span></span>
- <span data-ttu-id="d40f8-510">Funktioner</span><span class="sxs-lookup"><span data-stu-id="d40f8-510">Capabilities</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="d40f8-511">Förverkad mål grupp</span><span class="sxs-lookup"><span data-stu-id="d40f8-511">Impacted audience</span></span>

<span data-ttu-id="d40f8-512">Alla partner i Ryssland går igenom programmet för Cloud Solution Provider (CSP).</span><span class="sxs-lookup"><span data-stu-id="d40f8-512">All partners in Russia transacting through the Cloud Solution Provider (CSP) program.</span></span>

### <a name="details"></a><span data-ttu-id="d40f8-513">Information</span><span class="sxs-lookup"><span data-stu-id="d40f8-513">Details</span></span>

<span data-ttu-id="d40f8-514">Från och med den 10 2021 mars är vi glada att kunna meddela att den **nya Commerce-upplevelsen i CSP för Azure i Ryssland** är tillgänglig.</span><span class="sxs-lookup"><span data-stu-id="d40f8-514">Starting March 10 2021, we’re excited to announce the availability of the **new commerce experience in CSP for Azure in Russia**.</span></span> <span data-ttu-id="d40f8-515">Den här upplevelsen kommer att effektivisera och förbättra hur kunderna köper och använder Azure-tjänster.</span><span class="sxs-lookup"><span data-stu-id="d40f8-515">This experience will streamline and improve the way customers buy and consume Azure services.</span></span> <span data-ttu-id="d40f8-516">Det ger också partner i CSP-programmet en konsekvent vy över Azures priser i Sälj rörelserna, priset USD för global konsekvens, justering av fakturerings datum och åtkomst till Azure Cost Management.</span><span class="sxs-lookup"><span data-stu-id="d40f8-516">It will also give partners in the CSP program a consistent view of Azure pricing across sales motions, USD pricing for global consistency, billing date alignment, and access to Azure Cost Management.</span></span>

### <a name="next-steps"></a><span data-ttu-id="d40f8-517">Nästa steg</span><span class="sxs-lookup"><span data-stu-id="d40f8-517">Next steps</span></span>

<span data-ttu-id="d40f8-518">Det finns flera tillgängliga resurser som introducerar den nya Azure Commerce-upplevelsen och ger ytterligare information.</span><span class="sxs-lookup"><span data-stu-id="d40f8-518">There are several resources available introducing the new Azure commerce experience and providing additional information.</span></span> <span data-ttu-id="d40f8-519">Hitta de senaste frågorna, kortlek, video och mycket mer i [CSP-programmet uppdateringar resurs Galleri](https://partner.microsoft.com/resources/collection/new-azure-experience-in-csp#/).</span><span class="sxs-lookup"><span data-stu-id="d40f8-519">Find the latest FAQs, decks, video and more in the [CSP Program Updates Resource Gallery](https://partner.microsoft.com/resources/collection/new-azure-experience-in-csp#/).</span></span>

________________
## <a name="partner-center-software-license-key-and-download-fulfillment"></a><a name="4"></a><span data-ttu-id="d40f8-520">Partner Center licens nyckel för program vara och hämtnings klara</span><span class="sxs-lookup"><span data-stu-id="d40f8-520">Partner Center software license key and download fulfillment</span></span>

### <a name="categories"></a><span data-ttu-id="d40f8-521">Kategorier</span><span class="sxs-lookup"><span data-stu-id="d40f8-521">Categories</span></span>

- <span data-ttu-id="d40f8-522">Datum: 2021-03-04</span><span class="sxs-lookup"><span data-stu-id="d40f8-522">Date: 2021-03-04</span></span>
- <span data-ttu-id="d40f8-523">Funktioner</span><span class="sxs-lookup"><span data-stu-id="d40f8-523">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="d40f8-524">Sammanfattning</span><span class="sxs-lookup"><span data-stu-id="d40f8-524">Summary</span></span>

<span data-ttu-id="d40f8-525">Hämtningen av Partner Center-program varan och licens nyckelns uppfyllelse funktion har återställts.</span><span class="sxs-lookup"><span data-stu-id="d40f8-525">The Partner Center software download and license key fulfillment capability has been reinstated.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="d40f8-526">Förverkad mål grupp</span><span class="sxs-lookup"><span data-stu-id="d40f8-526">Impacted audience</span></span>

<span data-ttu-id="d40f8-527">Alla leverantörer av moln lösnings leverantörer (CSP) samverkar med program varu beställningar för beständig och Server prenumeration via partner Center</span><span class="sxs-lookup"><span data-stu-id="d40f8-527">All Cloud Solution Provider (CSP) partners transacting perpetual and server subscription software orders through Partner Center</span></span>

### <a name="details"></a><span data-ttu-id="d40f8-528">Information</span><span class="sxs-lookup"><span data-stu-id="d40f8-528">Details</span></span>

<span data-ttu-id="d40f8-529">Som svar på feedback från partnern är vi återinför för att få program vara och licens nycklar för program varu beställningar med beständig och Server prenumeration.</span><span class="sxs-lookup"><span data-stu-id="d40f8-529">In response to partner feedback, we’re reinstating the Partner Center fulfillment capability to obtain software and license keys for perpetual and server subscription software orders.</span></span> <span data-ttu-id="d40f8-530">Det kommer att återställas till sitt tidigare tillstånd innan det tas bort den 19 januari 2021.</span><span class="sxs-lookup"><span data-stu-id="d40f8-530">It will be restored to its previous state prior to being removed on January 19, 2021.</span></span> <span data-ttu-id="d40f8-531">(Se [meddelandet](2020-september.md#17).)</span><span class="sxs-lookup"><span data-stu-id="d40f8-531">(See the [announcement](2020-september.md#17).)</span></span>

<span data-ttu-id="d40f8-532">Observera att program licens nycklar och nedladdnings länkar är värdefulla och har sökts efter efter immateriella till gångar.</span><span class="sxs-lookup"><span data-stu-id="d40f8-532">Note that software license keys and download links are valuable and highly sought-after intellectual property assets.</span></span> <span data-ttu-id="d40f8-533">Om de läcker ut kan de snabbt bli uttömda sina aktiverings gränser och orsaka en negativ kund-och partner upplevelse.</span><span class="sxs-lookup"><span data-stu-id="d40f8-533">If leaked, they can quickly be depleted of their activation limits and cause a negative customer and partner experience.</span></span>

### <a name="next-steps"></a><span data-ttu-id="d40f8-534">Nästa steg</span><span class="sxs-lookup"><span data-stu-id="d40f8-534">Next steps</span></span>

<span data-ttu-id="d40f8-535">Läs följande resurser för användnings instruktioner och viktig vägledning om program varu nyckel distribution:</span><span class="sxs-lookup"><span data-stu-id="d40f8-535">Review the following resources for usage instructions and important guidance on software key distribution:</span></span>

- [<span data-ttu-id="d40f8-536">Sälja lokal program vara via CSP-programmet</span><span class="sxs-lookup"><span data-stu-id="d40f8-536">Sell on-premises software through the CSP program</span></span>](../csp-on-premise-software.md)
- <span data-ttu-id="d40f8-537">[Partner Center New Commerce Operations Guide](https://partner.microsoft.com/resources/detail/partner-center-new-commerce-operations-guide-pdf) (se avsnittet **vägledning om distribution av program varu nycklar** ).</span><span class="sxs-lookup"><span data-stu-id="d40f8-537">[Partner Center New Commerce Operations Guide](https://partner.microsoft.com/resources/detail/partner-center-new-commerce-operations-guide-pdf) (See the **Guidance on Software Key Distribution** section.)</span></span>

### <a name="questions"></a><span data-ttu-id="d40f8-538">Har du några frågor?</span><span class="sxs-lookup"><span data-stu-id="d40f8-538">Questions?</span></span>

<span data-ttu-id="d40f8-539">Om du har ytterligare frågor om det här meddelandet kan du kontrol lera dina relevanta Yammer-communities.</span><span class="sxs-lookup"><span data-stu-id="d40f8-539">If you have any further questions about this notice, check your relevant Yammer communities.</span></span>

________________
## <a name="migrate-your-deals-from-partner-sales-connect-psc-to-partner-center"></a><a name="3"></a><span data-ttu-id="d40f8-540">Migrera dina avtal från partner Sales Connect (PSC) till Partner Center</span><span class="sxs-lookup"><span data-stu-id="d40f8-540">Migrate your deals from Partner Sales Connect (PSC) to Partner Center</span></span>

### <a name="categories"></a><span data-ttu-id="d40f8-541">Kategorier</span><span class="sxs-lookup"><span data-stu-id="d40f8-541">Categories</span></span>

- <span data-ttu-id="d40f8-542">Datum: 2021-03-04</span><span class="sxs-lookup"><span data-stu-id="d40f8-542">Date: 2021-03-04</span></span>
- <span data-ttu-id="d40f8-543">Funktioner</span><span class="sxs-lookup"><span data-stu-id="d40f8-543">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="d40f8-544">Sammanfattning</span><span class="sxs-lookup"><span data-stu-id="d40f8-544">Summary</span></span>

<span data-ttu-id="d40f8-545">Partner Sales Connect (PSC) flyttas till skrivskyddad åtkomst från den 31 mars 2021, så vi uppmanar dig att börja migrera dina avtal från PSC till Partner Center.</span><span class="sxs-lookup"><span data-stu-id="d40f8-545">Partner Sales Connect (PSC) will move to read-only access starting March 31, 2021, so we urge you to begin migrating your deals from PSC to Partner Center.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="d40f8-546">Förverkad mål grupp</span><span class="sxs-lookup"><span data-stu-id="d40f8-546">Impacted audience</span></span>

<span data-ttu-id="d40f8-547">Partner med avtal i PSC</span><span class="sxs-lookup"><span data-stu-id="d40f8-547">Partners with deals in PSC</span></span>

### <a name="details"></a><span data-ttu-id="d40f8-548">Information</span><span class="sxs-lookup"><span data-stu-id="d40f8-548">Details</span></span>

<span data-ttu-id="d40f8-549">Som en del av vårt gemensamma åtagande att växa, är **samförsäljning med Microsoft** att du kan **identifiera, leverera dina kunskaper och utöka dina kunders** behov av positiva kund resultat.</span><span class="sxs-lookup"><span data-stu-id="d40f8-549">As part of our shared commitment to growth, **co-sell with Microsoft** is the path for you to **be discovered, deliver your expertise, and expand your customer footprint** for positive customer outcomes.</span></span> <span data-ttu-id="d40f8-550">Med ett genomsnittligt avtal som är **3,5 gånger snabbare** än vanligt, kan du med hantera din samkunds upplevelse i Partner Center sälja över den direkta kunden, partnern och Microsofts försäljnings kanaler och hantera hela din Hänvisnings pipeline på en plats.</span><span class="sxs-lookup"><span data-stu-id="d40f8-550">With an average deal that’s **3.5 times faster** than normal, managing your co-sell experience in Partner Center allows you to sell across the direct customer, partner, and Microsoft seller channels, and manage your entire referral pipeline in one location.</span></span>

<span data-ttu-id="d40f8-551">**PSC** kommer att flyttas till **skrivskyddad åtkomst** från den **31 mars 2021**, så vi uppmanar dig att påbörja din flytt till Partner Center och få till gång till dessa förbättringar:</span><span class="sxs-lookup"><span data-stu-id="d40f8-551">**PSC** will move to **read-only access** starting **March 31, 2021**, so we urge you to start your move to Partner Center and access these capability improvements:</span></span> 

- <span data-ttu-id="d40f8-552">**Mer exakt routning** av de avtal som du delar med Microsoft till den högra säljaren, baserat på vilken typ av hjälp du behöver.</span><span class="sxs-lookup"><span data-stu-id="d40f8-552">**More accurate routing** of the deals that you share with Microsoft to the right seller, based on the type of assistance you need.</span></span>
- <span data-ttu-id="d40f8-553">Krav **verifiering för direkt** behandling för incitaments berättigade lösningar och för att uppfylla kraven på ISV Connect-program, vilket fören klar godkännande processen och det slutliga Poe-attesteringen (proof of Execution).</span><span class="sxs-lookup"><span data-stu-id="d40f8-553">**Upfront deal eligibility validation** for incentive-eligible solutions and to meet the ISV Connect program criteria, simplifying the approval process and final proof of execution (POE) attestation.</span></span>
- <span data-ttu-id="d40f8-554">**Smidig användar upplevelse** för att hantera alla dina samförsäljnings möjligheter och Sälj kvalificerade leads på ett och samma ställe.</span><span class="sxs-lookup"><span data-stu-id="d40f8-554">**Seamless user experience** to manage all your co-sell opportunities and sales qualified leads in one place.</span></span>

<span data-ttu-id="d40f8-555">Vi har också nyligen lagt till nya funktioner i Partner Center som hjälper dig att flytta:</span><span class="sxs-lookup"><span data-stu-id="d40f8-555">We’ve also recently added new features in Partner Center to assist in your move:</span></span>

- [<span data-ttu-id="d40f8-556">Mass åtgärder för samförsäljnings möjligheter</span><span class="sxs-lookup"><span data-stu-id="d40f8-556">Bulk operations for co-sell opportunities</span></span>](../bulk-operations.md)
- <span data-ttu-id="d40f8-557">[Funktionen](../psc-to-pc.md) för att migrera en funktion (se avsnittet **PSC-migrering** .)</span><span class="sxs-lookup"><span data-stu-id="d40f8-557">[Deal migration feature](../psc-to-pc.md) (See the **PSC Deals migration** section.)</span></span>

<span data-ttu-id="d40f8-558">Med hjälp av co-Sales-upplevelsen i Partner Center får Sälj teamen mer tid på att fokusera på Nurturing-leads och affärs möjligheter, avsluta avtal och skapa långsiktiga kund relationer.</span><span class="sxs-lookup"><span data-stu-id="d40f8-558">Using the co-sell experience in Partner Center, your sales teams will have more time to focus on nurturing leads and opportunities, closing deals, and creating lasting customer relationships.</span></span>

### <a name="next-steps"></a><span data-ttu-id="d40f8-559">Nästa steg</span><span class="sxs-lookup"><span data-stu-id="d40f8-559">Next steps</span></span>

<span data-ttu-id="d40f8-560">Använd [över gångs guiden](../psc-to-pc.md) för partner Center för att gå igenom stegen för att migrera dina avtal från PSC till Partner Center.</span><span class="sxs-lookup"><span data-stu-id="d40f8-560">Use the Partner Center [transition guide](../psc-to-pc.md) to walk you through the steps to migrate your deals from PSC to Partner Center.</span></span>

### <a name="questions"></a><span data-ttu-id="d40f8-561">Har du några frågor?</span><span class="sxs-lookup"><span data-stu-id="d40f8-561">Questions?</span></span>

<span data-ttu-id="d40f8-562">Kontakta [supporten](https://partner.microsoft.com/support/?stage=1)om du vill ha fler frågor.</span><span class="sxs-lookup"><span data-stu-id="d40f8-562">For any further questions, contact [Support](https://partner.microsoft.com/support/?stage=1).</span></span>

________________
## <a name="new-microsoft-dynamics-365-products-and-offers-available-on-april-1-2021"></a><a name="2"></a><span data-ttu-id="d40f8-563">Nya Microsoft Dynamics 365-produkter och erbjudanden som är tillgängliga den 1 april 2021</span><span class="sxs-lookup"><span data-stu-id="d40f8-563">New Microsoft Dynamics 365 products and offers available on April 1, 2021</span></span>

### <a name="categories"></a><span data-ttu-id="d40f8-564">Kategorier</span><span class="sxs-lookup"><span data-stu-id="d40f8-564">Categories</span></span>

- <span data-ttu-id="d40f8-565">Datum: 2021-03-04</span><span class="sxs-lookup"><span data-stu-id="d40f8-565">Date: 2021-03-04</span></span>
- <span data-ttu-id="d40f8-566">Funktioner</span><span class="sxs-lookup"><span data-stu-id="d40f8-566">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="d40f8-567">Sammanfattning</span><span class="sxs-lookup"><span data-stu-id="d40f8-567">Summary</span></span>

<span data-ttu-id="d40f8-568">Den 1 april 2021 kommer Microsoft att lansera flera nya produkter och erbjudanden för Cloud Solution Provider (CSP)-programmet.</span><span class="sxs-lookup"><span data-stu-id="d40f8-568">On April 1, 2021, Microsoft will be launching several new products and offers for the Cloud Solution Provider (CSP) program.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="d40f8-569">Förverkad mål grupp</span><span class="sxs-lookup"><span data-stu-id="d40f8-569">Impacted audience</span></span>

<span data-ttu-id="d40f8-570">Alla partner som går via program varan för Cloud Solution Provider (CSP)</span><span class="sxs-lookup"><span data-stu-id="d40f8-570">All partners transacting through the Cloud Solution Provider (CSP) program</span></span>

### <a name="details"></a><span data-ttu-id="d40f8-571">Information</span><span class="sxs-lookup"><span data-stu-id="d40f8-571">Details</span></span>

<span data-ttu-id="d40f8-572">Den 1 april 2021 kommer Microsoft att lansera följande nya produkter och erbjudanden:</span><span class="sxs-lookup"><span data-stu-id="d40f8-572">On April 1, 2021, Microsoft will be launching the following new products and offers:</span></span>

- <span data-ttu-id="d40f8-573">Power BI Premium per användare</span><span class="sxs-lookup"><span data-stu-id="d40f8-573">Power BI Premium Per User</span></span>
- <span data-ttu-id="d40f8-574">Kund röst och marknadsföring dem Geo-och segment expansion</span><span class="sxs-lookup"><span data-stu-id="d40f8-574">Customer Voice and Marketing USL geo and segment expansion</span></span>

<span data-ttu-id="d40f8-575">**Power BI Premium per användare**</span><span class="sxs-lookup"><span data-stu-id="d40f8-575">**Power BI Premium Per User**</span></span>

<span data-ttu-id="d40f8-576">Microsoft kommer att introducera de första Power BI Premium erbjudandena per användare.</span><span class="sxs-lookup"><span data-stu-id="d40f8-576">Microsoft will introduce the first per-user Power BI Premium offers.</span></span> <span data-ttu-id="d40f8-577">Power BI Premium säljs för närvarande endast i en kapacitets konstruktion.</span><span class="sxs-lookup"><span data-stu-id="d40f8-577">Power BI Premium is currently sold only in a capacity construct.</span></span> <span data-ttu-id="d40f8-578">Power BI Premium per användare ger till gång till Enterprise-Business Intelligence (BI) och analys funktioner.</span><span class="sxs-lookup"><span data-stu-id="d40f8-578">Power BI Premium Per User provides access to enterprise business intelligence (BI) and analytics capabilities.</span></span> <span data-ttu-id="d40f8-579">Den flexibla enskilda klient licensieringen tillgodoser små och medel stora företag.</span><span class="sxs-lookup"><span data-stu-id="d40f8-579">Its flexible individual seat licensing caters to small and medium-sized businesses.</span></span>

<span data-ttu-id="d40f8-580">Läs mer om det här erbjudandet i [Power BI versions informationen](/power-platform-release-plan/2020wave2/power-bi/planned-features) .</span><span class="sxs-lookup"><span data-stu-id="d40f8-580">Review the [Power BI release details](/power-platform-release-plan/2020wave2/power-bi/planned-features) to learn more about this offer.</span></span>


<span data-ttu-id="d40f8-581">**Erbjudande information**</span><span class="sxs-lookup"><span data-stu-id="d40f8-581">**Offer details**</span></span>

<span data-ttu-id="d40f8-582">Observera att namnet på erbjudandet skiljer sig något från för hands versionen av pris listan.</span><span class="sxs-lookup"><span data-stu-id="d40f8-582">Note that the offer name differs slightly from the price list preview.</span></span>

| <span data-ttu-id="d40f8-583">Erbjudandets namn</span><span class="sxs-lookup"><span data-stu-id="d40f8-583">Offer name</span></span> | <span data-ttu-id="d40f8-584">Erbjudande-ID</span><span class="sxs-lookup"><span data-stu-id="d40f8-584">Offer ID</span></span> |
| ------ |----------- |
| <span data-ttu-id="d40f8-585">Power BI Premium per användare</span><span class="sxs-lookup"><span data-stu-id="d40f8-585">Power BI Premium Per User</span></span> | <span data-ttu-id="d40f8-586">9c810018-9356-4903-95ab-eeb956289290</span><span class="sxs-lookup"><span data-stu-id="d40f8-586">9c810018-9356-4903-95ab-eeb956289290</span></span> | 
| <span data-ttu-id="d40f8-587">Power BI Premium per användare för lärare</span><span class="sxs-lookup"><span data-stu-id="d40f8-587">Power BI Premium Per User for Faculty</span></span> | <span data-ttu-id="d40f8-588">3affc44f-f372-4ad5-8657-aadd9574fce0</span><span class="sxs-lookup"><span data-stu-id="d40f8-588">3affc44f-f372-4ad5-8657-aadd9574fce0</span></span> | 
| <span data-ttu-id="d40f8-589">Power BI Premium per användare för studenter</span><span class="sxs-lookup"><span data-stu-id="d40f8-589">Power BI Premium Per User for Students</span></span> | <span data-ttu-id="d40f8-590">657eea87-d0b0-4c89-8c8e-9b04395bd940</span><span class="sxs-lookup"><span data-stu-id="d40f8-590">657eea87-d0b0-4c89-8c8e-9b04395bd940</span></span> | 
| <span data-ttu-id="d40f8-591">Power BI Premium per användare (prissättning i ideell personal)</span><span class="sxs-lookup"><span data-stu-id="d40f8-591">Power BI Premium Per User (Nonprofit Staff Pricing)</span></span> | <span data-ttu-id="d40f8-592">7a0a856c-059f-45dd-9d26-ae27992e706a</span><span class="sxs-lookup"><span data-stu-id="d40f8-592">7a0a856c-059f-45dd-9d26-ae27992e706a</span></span> | 
| <span data-ttu-id="d40f8-593">Power BI Premium per användare Add-On</span><span class="sxs-lookup"><span data-stu-id="d40f8-593">Power BI Premium Per User Add-On</span></span> | <span data-ttu-id="d40f8-594">244ff87e-5925-44a0-bf31-cea189719b58</span><span class="sxs-lookup"><span data-stu-id="d40f8-594">244ff87e-5925-44a0-bf31-cea189719b58</span></span> | 
| <span data-ttu-id="d40f8-595">Power BI Premium per användare Add-On för lärare</span><span class="sxs-lookup"><span data-stu-id="d40f8-595">Power BI Premium Per User Add-On for Faculty</span></span> | <span data-ttu-id="d40f8-596">5da849bd-b8f7-4340-b4f4-3a9eaeb8987e</span><span class="sxs-lookup"><span data-stu-id="d40f8-596">5da849bd-b8f7-4340-b4f4-3a9eaeb8987e</span></span> | 
| <span data-ttu-id="d40f8-597">Power BI Premium per användare Add-On för studenter</span><span class="sxs-lookup"><span data-stu-id="d40f8-597">Power BI Premium Per User Add-On for Students</span></span> | <span data-ttu-id="d40f8-598">cf62d70d-5af5-422a-bda8-97936402ac8e</span><span class="sxs-lookup"><span data-stu-id="d40f8-598">cf62d70d-5af5-422a-bda8-97936402ac8e</span></span> | 
| <span data-ttu-id="d40f8-599">Power BI Premium per användare Add-On (prissättning i ideell personal)</span><span class="sxs-lookup"><span data-stu-id="d40f8-599">Power BI Premium Per User Add-On (Nonprofit Staff Pricing)</span></span> | <span data-ttu-id="d40f8-600">31c03289-47ab-4ab0-8df1-03742c127ac6</span><span class="sxs-lookup"><span data-stu-id="d40f8-600">31c03289-47ab-4ab0-8df1-03742c127ac6</span></span> | 

<span data-ttu-id="d40f8-601">**Kund röst och marknadsföring dem Geo-och segment expansion**</span><span class="sxs-lookup"><span data-stu-id="d40f8-601">**Customer Voice and Marketing USL geo and segment expansion**</span></span>

<span data-ttu-id="d40f8-602">Som en uppföljning till lanseringen av december 2020 har Dynamics 365 Customer Voice och Marketing dem-erbjudanden ändrats för att lägga till nya länder och fler ideella och utbildnings-SKU: er.</span><span class="sxs-lookup"><span data-stu-id="d40f8-602">As a follow-up to the December 2020 launch, Dynamics 365 Customer Voice and Marketing USL offers have been changed to add new countries and more nonprofit and educational SKUs.</span></span>

| <span data-ttu-id="d40f8-603">Erbjudandets namn</span><span class="sxs-lookup"><span data-stu-id="d40f8-603">Offer name</span></span> | <span data-ttu-id="d40f8-604">Erbjudande-ID</span><span class="sxs-lookup"><span data-stu-id="d40f8-604">Offer ID</span></span> |
| ------ |----------- |
| <span data-ttu-id="d40f8-605">Dynamics 365 Customer Voice-dem (pris för ideell personal)</span><span class="sxs-lookup"><span data-stu-id="d40f8-605">Dynamics 365 Customer Voice USL (Nonprofit Staff Pricing)</span></span> | <span data-ttu-id="d40f8-606">7a8642a5-481e-4906-a642-b56dbeeb62a0</span><span class="sxs-lookup"><span data-stu-id="d40f8-606">7a8642a5-481e-4906-a642-b56dbeeb62a0</span></span> |
| <span data-ttu-id="d40f8-607">Dynamics 365 Customer Voice-dem för lärare</span><span class="sxs-lookup"><span data-stu-id="d40f8-607">Dynamics 365 Customer Voice USL for Faculty</span></span> | <span data-ttu-id="d40f8-608">85162d70-9676-4cf6-a4bc-a0d6672f2657</span><span class="sxs-lookup"><span data-stu-id="d40f8-608">85162d70-9676-4cf6-a4bc-a0d6672f2657</span></span> |

<span data-ttu-id="d40f8-609">Besök följande sidor för att få mer information om dessa erbjudanden:</span><span class="sxs-lookup"><span data-stu-id="d40f8-609">Visit the following pages to find out more about these offers:</span></span>

- [<span data-ttu-id="d40f8-610">Dynamics 365-röstens start sida för kund service</span><span class="sxs-lookup"><span data-stu-id="d40f8-610">Dynamics 365 Customer Service Voice home page</span></span>](https://dynamics.microsoft.com/customer-voice/overview/)
- [<span data-ttu-id="d40f8-611">Start sida för Dynamics 365-marknadsföring</span><span class="sxs-lookup"><span data-stu-id="d40f8-611">Dynamics 365 Marketing home page</span></span>](https://dynamics.microsoft.com/customer-voice/overview/)

### <a name="next-steps"></a><span data-ttu-id="d40f8-612">Nästa steg</span><span class="sxs-lookup"><span data-stu-id="d40f8-612">Next steps</span></span>

<span data-ttu-id="d40f8-613">Granska resurserna i det här avsnittet och dela den här informationen med lämpliga intressenter i din organisation.</span><span class="sxs-lookup"><span data-stu-id="d40f8-613">Review the resources on this topic, and share this information with the appropriate stakeholders in your organization.</span></span>  

### <a name="questions"></a><span data-ttu-id="d40f8-614">Har du några frågor?</span><span class="sxs-lookup"><span data-stu-id="d40f8-614">Questions?</span></span>

<span data-ttu-id="d40f8-615">Om du har frågor om dessa erbjudanden kan du kontrol lera dina relevanta Yammer-communities.</span><span class="sxs-lookup"><span data-stu-id="d40f8-615">For any questions about these offers, check your relevant Yammer communities.</span></span> 

________________
## <a name="microsoft-universal-print-now-available-in-some-suites"></a><a name="1"></a> <span data-ttu-id="d40f8-616">Microsoft Universal Print finns nu i vissa paket</span><span class="sxs-lookup"><span data-stu-id="d40f8-616">Microsoft Universal Print now available in some suites</span></span>

### <a name="categories"></a><span data-ttu-id="d40f8-617">Kategorier</span><span class="sxs-lookup"><span data-stu-id="d40f8-617">Categories</span></span>

- <span data-ttu-id="d40f8-618">Datum: 2021-03-33</span><span class="sxs-lookup"><span data-stu-id="d40f8-618">Date: 2021-03-33</span></span>
- <span data-ttu-id="d40f8-619">Funktioner</span><span class="sxs-lookup"><span data-stu-id="d40f8-619">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="d40f8-620">Sammanfattning</span><span class="sxs-lookup"><span data-stu-id="d40f8-620">Summary</span></span>

<span data-ttu-id="d40f8-621">Microsoft Universal Print är tillgängligt för Transact i SELECT Microsoft 365 Suites och som ett fristående tillägg från den 1 mars 2021.</span><span class="sxs-lookup"><span data-stu-id="d40f8-621">Microsoft Universal Print will be available to transact within select Microsoft 365 suites and as a standalone add-on from March 1, 2021.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="d40f8-622">Förverkad mål grupp</span><span class="sxs-lookup"><span data-stu-id="d40f8-622">Impacted audience</span></span>

<span data-ttu-id="d40f8-623">Alla partner som går via program varan för Cloud Solution Provider (CSP)</span><span class="sxs-lookup"><span data-stu-id="d40f8-623">All partners transacting through the Cloud Solution Provider (CSP) program</span></span>

### <a name="details"></a><span data-ttu-id="d40f8-624">Information</span><span class="sxs-lookup"><span data-stu-id="d40f8-624">Details</span></span>

<span data-ttu-id="d40f8-625">[Universal Print](https://aka.ms/universalprint) är en Microsoft 365 utskrifts tjänst som tar bort behovet av lokala utskrifts servrar och gör det möjligt för Windows-enheter att skriva ut till Azure-registrerade skrivare.</span><span class="sxs-lookup"><span data-stu-id="d40f8-625">[Universal Print](https://aka.ms/universalprint) is a Microsoft 365 print service that removes the need for on-premises print servers, and enables Windows devices to print to Azure-registered printers.</span></span> <span data-ttu-id="d40f8-626">Den kommer att vara tillgänglig för Transact från den 1 mars 2021.</span><span class="sxs-lookup"><span data-stu-id="d40f8-626">It will be available to transact from March 1, 2021.</span></span>

<span data-ttu-id="d40f8-627">Arbets tagarna har nytta av driv rutins utskrift, strömlinjeformad plats-baserad skrivar identifiering och en intuitiv utskrifts upplevelse utan inlärnings kurva.</span><span class="sxs-lookup"><span data-stu-id="d40f8-627">Workers benefit from driverless printing, streamlined location-based printer discovery, and an intuitive printing experience with no learning curve.</span></span> <span data-ttu-id="d40f8-628">Enheter som är anslutna till Azure Active Directory (Azure AD) använder befintliga Azure AD-autentiseringsuppgifter för att skriva ut på ett säkert sätt.</span><span class="sxs-lookup"><span data-stu-id="d40f8-628">Devices that are joined to Azure Active Directory (Azure AD) use existing Azure AD credentials to print securely.</span></span> <span data-ttu-id="d40f8-629">Administratörer hanterar utskriften med hjälp av Azure Portal och kan enkelt ansluta skrivare med inbyggt stöd för universell utskrift.</span><span class="sxs-lookup"><span data-stu-id="d40f8-629">Administrators manage printing by using the Azure portal, and can easily connect printers with native support for Universal Print.</span></span> <span data-ttu-id="d40f8-630">Universell utskrift kan distribueras med icke-kompatibla skrivare med hjälp av Universal Print Connector-programvara.</span><span class="sxs-lookup"><span data-stu-id="d40f8-630">Universal Print can be deployed with non-compatible printers by using Universal Print connector software.</span></span>

<span data-ttu-id="d40f8-631">Universal Print kommer att fyllas i vid lanseringen till Windows E3, A3, E5 och A5 och Microsoft 365 BP, F3, E3, A3, E5 och A5.</span><span class="sxs-lookup"><span data-stu-id="d40f8-631">Universal Print will be backfilled at launch to Windows E3, A3, E5, and A5, and Microsoft 365 BP, F3, E3, A3, E5, and A5.</span></span>  

<span data-ttu-id="d40f8-632">**Erbjudande information**</span><span class="sxs-lookup"><span data-stu-id="d40f8-632">**Offer details**</span></span>

<span data-ttu-id="d40f8-633">Observera att namnet på erbjudandet skiljer sig något från för hands versionen av pris listan.</span><span class="sxs-lookup"><span data-stu-id="d40f8-633">Note that the offer name differs slightly from the price list preview.</span></span>

| <span data-ttu-id="d40f8-634">Erbjudandets namn</span><span class="sxs-lookup"><span data-stu-id="d40f8-634">Offer name</span></span> | <span data-ttu-id="d40f8-635">Erbjudande-ID</span><span class="sxs-lookup"><span data-stu-id="d40f8-635">Offer ID</span></span> | <span data-ttu-id="d40f8-636">Material-ID</span><span class="sxs-lookup"><span data-stu-id="d40f8-636">Material ID</span></span> |
| ------ |----------- |----------- |  
| <span data-ttu-id="d40f8-637">Tillägg för universell utskrifts volym (500 jobb) – Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="d40f8-637">Universal Print volume add-on (500 jobs) - Microsoft 365</span></span>  | <span data-ttu-id="d40f8-638">cb131356-45ee-4ae2-8537-873b706c8e75</span><span class="sxs-lookup"><span data-stu-id="d40f8-638">cb131356-45ee-4ae2-8537-873b706c8e75</span></span>     | <span data-ttu-id="d40f8-639">9BI-00004</span><span class="sxs-lookup"><span data-stu-id="d40f8-639">9BI-00004</span></span>   |
| <span data-ttu-id="d40f8-640">Tillägg för universell utskrifts volym (500 jobb) för lärare – Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="d40f8-640">Universal Print volume add-on (500 jobs) for faculty - Microsoft 365</span></span>   | <span data-ttu-id="d40f8-641">477bee81-9872-43d6-91d3-c72390bfcf49</span><span class="sxs-lookup"><span data-stu-id="d40f8-641">477bee81-9872-43d6-91d3-c72390bfcf49</span></span>   | <span data-ttu-id="d40f8-642">9BK-00004</span><span class="sxs-lookup"><span data-stu-id="d40f8-642">9BK-00004</span></span>   |
| <span data-ttu-id="d40f8-643">Tillägg för universell utskrifts volym (500 jobb) – Windows</span><span class="sxs-lookup"><span data-stu-id="d40f8-643">Universal Print volume add-on (500 jobs) - Windows</span></span>    | <span data-ttu-id="d40f8-644">d3ddc493-5741-4e0d-a02d-07edbb0bb72e</span><span class="sxs-lookup"><span data-stu-id="d40f8-644">d3ddc493-5741-4e0d-a02d-07edbb0bb72e</span></span>   | <span data-ttu-id="d40f8-645">9BI-00002</span><span class="sxs-lookup"><span data-stu-id="d40f8-645">9BI-00002</span></span>   |
| <span data-ttu-id="d40f8-646">Tillägg för universell utskrifts volym (500 jobb) för lärare – Windows</span><span class="sxs-lookup"><span data-stu-id="d40f8-646">Universal Print volume add-on (500 jobs) for faculty - Windows</span></span>   |  <span data-ttu-id="d40f8-647">d0862f05-80f5-4fd4-8432-fe72dd893cc7</span><span class="sxs-lookup"><span data-stu-id="d40f8-647">d0862f05-80f5-4fd4-8432-fe72dd893cc7</span></span>  | <span data-ttu-id="d40f8-648">9BK-00002</span><span class="sxs-lookup"><span data-stu-id="d40f8-648">9BK-00002</span></span>   |

### <a name="next-steps"></a><span data-ttu-id="d40f8-649">Nästa steg</span><span class="sxs-lookup"><span data-stu-id="d40f8-649">Next steps</span></span>

<span data-ttu-id="d40f8-650">Bekanta dig med pris listan och [Översikt över universell utskrift](/universal-print/fundamentals/universal-print-whatis).</span><span class="sxs-lookup"><span data-stu-id="d40f8-650">Familiarize yourself with the price list and the [Universal Print overview](/universal-print/fundamentals/universal-print-whatis).</span></span> <span data-ttu-id="d40f8-651">Dela den här informationen med alla lämpliga kontakter i din organisation.</span><span class="sxs-lookup"><span data-stu-id="d40f8-651">Share this information with all appropriate contacts in your organization.</span></span>

### <a name="questions"></a><span data-ttu-id="d40f8-652">Har du några frågor?</span><span class="sxs-lookup"><span data-stu-id="d40f8-652">Questions?</span></span>

<span data-ttu-id="d40f8-653">Om du har frågor om dessa erbjudanden kan du kontrol lera dina relevanta Yammer-communities.</span><span class="sxs-lookup"><span data-stu-id="d40f8-653">For any questions about these offers, check your relevant Yammer communities.</span></span>
