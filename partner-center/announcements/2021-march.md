---
title: Meddelanden mars 2021
description: Mars 2021-meddelanden för Microsoft Partner Center, inklusive nya funktioner, kampanjer, erbjudanden, marknader eller ändringar i befintliga erbjudanden.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: brentserbus
ms.author: brserbus
ms.custom: announcement
ms.localizationpriority: high
ms.date: 04/02/2021
ms.openlocfilehash: 3d91eb26f98005b92a48c6f242ea4439e42cde05
ms.sourcegitcommit: 22e257d5b334ca8d3fc072f59010a508e1022694
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 05/06/2021
ms.locfileid: "108702883"
---
# <a name="march-2021-announcements"></a><span data-ttu-id="ee09b-103">Meddelanden mars 2021</span><span class="sxs-lookup"><span data-stu-id="ee09b-103">March 2021 announcements</span></span>

<span data-ttu-id="ee09b-104">Den här sidan innehåller meddelanden för Microsoft Partner Center för mars 2021.</span><span class="sxs-lookup"><span data-stu-id="ee09b-104">This page provides the announcements for Microsoft Partner Center for March 2021.</span></span>

## <a name="readiness-changes-to-the-cloud-solution-provider-csp-customer-address-validation-api-going-live-in-june-testing-capability-now-available"></a><a name="18"></a><span data-ttu-id="ee09b-105">Beredskap: Ändringar i CSP Molnlösningsleverantör-API:et för kundadressvalidering går live i juni. nu tillgänglig testfunktion</span><span class="sxs-lookup"><span data-stu-id="ee09b-105">Readiness: Changes to the Cloud Solution Provider (CSP) customer address validation API going live in June; testing capability now available</span></span>

### <a name="categories"></a><span data-ttu-id="ee09b-106">Kategorier</span><span class="sxs-lookup"><span data-stu-id="ee09b-106">Categories</span></span>

- <span data-ttu-id="ee09b-107">Datum: 2021-03-30</span><span class="sxs-lookup"><span data-stu-id="ee09b-107">Date: 2021-03-30</span></span>
- <span data-ttu-id="ee09b-108">Beredskap</span><span class="sxs-lookup"><span data-stu-id="ee09b-108">Readiness</span></span>

### <a name="summary"></a><span data-ttu-id="ee09b-109">Sammanfattning</span><span class="sxs-lookup"><span data-stu-id="ee09b-109">Summary</span></span>

<span data-ttu-id="ee09b-110">För att hjälpa partner och kunder att driva sin verksamhet baserat på förtroende kommer vi att bjuda in partner att testa ändringar i API:et validate address för alla länder över hela världen.</span><span class="sxs-lookup"><span data-stu-id="ee09b-110">To help partners and customers run their business based on trust, we’ll be inviting partners to test changes to the Validate Address API for all countries worldwide.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="ee09b-111">Målgrupp som påverkas</span><span class="sxs-lookup"><span data-stu-id="ee09b-111">Impacted audience</span></span>

<span data-ttu-id="ee09b-112">CSP-direktfaktureringspartner och indirekta leverantörer som skapar nya eller uppdaterar befintliga kunders adressinformation.</span><span class="sxs-lookup"><span data-stu-id="ee09b-112">CSP direct bill partners and indirect providers who create new or update existing customers address details.</span></span>

### <a name="details"></a><span data-ttu-id="ee09b-113">Information</span><span class="sxs-lookup"><span data-stu-id="ee09b-113">Details</span></span>

<span data-ttu-id="ee09b-114">Microsoft körs med förtroende.</span><span class="sxs-lookup"><span data-stu-id="ee09b-114">Microsoft runs on trust.</span></span> <span data-ttu-id="ee09b-115">Vi strävar efter att tillhandahålla en kompatibel, säker och säker metod för validering av kundadresser för att kunna hantera kundprenumerationer i CSP-programmet.</span><span class="sxs-lookup"><span data-stu-id="ee09b-115">We’re committed to providing a compliant, safe, and secure method of customer address validation for transacting customer subscriptions in the CSP program.</span></span> <span data-ttu-id="ee09b-116">Från och med den 31 mars 2021 har vi infört ändringar i API:et Validate Address som vi bjudit in partner att testa innan vi går live med ändringarna i juni 2021.</span><span class="sxs-lookup"><span data-stu-id="ee09b-116">As of March 31, 2021, we’ve introduced changes to the Validate Address API that we invited partners to test, prior to going live with the changes in June 2021.</span></span>

<span data-ttu-id="ee09b-117">Ändringarna påverkar endast API:et validate address.</span><span class="sxs-lookup"><span data-stu-id="ee09b-117">Changes affect the Validate Address API only.</span></span> <span data-ttu-id="ee09b-118">API:er för att skapa kund och uppdatera faktureringsprofil påverkas inte.</span><span class="sxs-lookup"><span data-stu-id="ee09b-118">Create Customer and Update Billing Profile APIs aren’t impacted.</span></span>

<span data-ttu-id="ee09b-119">Svaret returnerar något av följande statusmeddelanden:</span><span class="sxs-lookup"><span data-stu-id="ee09b-119">The response will return one of the following status messages:</span></span>

| <span data-ttu-id="ee09b-120">Status</span><span class="sxs-lookup"><span data-stu-id="ee09b-120">Status</span></span>     | <span data-ttu-id="ee09b-121">Beskrivning</span><span class="sxs-lookup"><span data-stu-id="ee09b-121">Description</span></span> |    <span data-ttu-id="ee09b-122">Antal föreslagna adresser som returneras</span><span class="sxs-lookup"><span data-stu-id="ee09b-122">Number of suggested addresses returned</span></span> |
|-------|---------------|-------------------|
|<span data-ttu-id="ee09b-123">Verifierad leverans</span><span class="sxs-lookup"><span data-stu-id="ee09b-123">Verified shippable</span></span> | <span data-ttu-id="ee09b-124">Adressen är verifierad och kan skickas till.</span><span class="sxs-lookup"><span data-stu-id="ee09b-124">Address is verified and can be shipped to.</span></span> | <span data-ttu-id="ee09b-125">Enkel</span><span class="sxs-lookup"><span data-stu-id="ee09b-125">Single</span></span> |
|<span data-ttu-id="ee09b-126">Verifierat</span><span class="sxs-lookup"><span data-stu-id="ee09b-126">Verified</span></span> | <span data-ttu-id="ee09b-127">Adressen är verifierad.</span><span class="sxs-lookup"><span data-stu-id="ee09b-127">Address is verified.</span></span> | <span data-ttu-id="ee09b-128">Enkel</span><span class="sxs-lookup"><span data-stu-id="ee09b-128">Single</span></span> |
|<span data-ttu-id="ee09b-129">Interaktion krävs</span><span class="sxs-lookup"><span data-stu-id="ee09b-129">Interaction required</span></span> | <span data-ttu-id="ee09b-130">Den föreslagna adressen har ändrats avsevärt och kräver användarbekräftelse.</span><span class="sxs-lookup"><span data-stu-id="ee09b-130">Suggested address has been changed significantly and needs user confirmation.</span></span> | <span data-ttu-id="ee09b-131">Enkel</span><span class="sxs-lookup"><span data-stu-id="ee09b-131">Single</span></span> |
|<span data-ttu-id="ee09b-132">Gatuadress – partiell</span><span class="sxs-lookup"><span data-stu-id="ee09b-132">Street partial</span></span> | <span data-ttu-id="ee09b-133">Den angivna gatuadressen är delvis och behöver mer information.</span><span class="sxs-lookup"><span data-stu-id="ee09b-133">The given street in the address is partial and needs more info.</span></span> | <span data-ttu-id="ee09b-134">Flera – högst tre</span><span class="sxs-lookup"><span data-stu-id="ee09b-134">Multiple—maximum of three</span></span> |
|<span data-ttu-id="ee09b-135">Delvis lokal</span><span class="sxs-lookup"><span data-stu-id="ee09b-135">Premises partial</span></span> | <span data-ttu-id="ee09b-136">De angivna lokalerna (byggnummer, svitnummer och annat) är ofullständiga och behöver mer information.</span><span class="sxs-lookup"><span data-stu-id="ee09b-136">The given premises (building number, suite number, and others) are partial and need more info.</span></span> | <span data-ttu-id="ee09b-137">Flera – högst tre</span><span class="sxs-lookup"><span data-stu-id="ee09b-137">Multiple—maximum of three</span></span> |
|<span data-ttu-id="ee09b-138">Flera</span><span class="sxs-lookup"><span data-stu-id="ee09b-138">Multiple</span></span> | <span data-ttu-id="ee09b-139">Det finns flera fält som är partiella i adressen (eventuellt även delvis gatuadress och delvis lokal).</span><span class="sxs-lookup"><span data-stu-id="ee09b-139">There are multiple fields that are partial in the address (potentially also including street partial and premises partial).</span></span> | <span data-ttu-id="ee09b-140">Flera – högst tre</span><span class="sxs-lookup"><span data-stu-id="ee09b-140">Multiple—maximum of three</span></span> |
|<span data-ttu-id="ee09b-141">Inget</span><span class="sxs-lookup"><span data-stu-id="ee09b-141">None</span></span> | <span data-ttu-id="ee09b-142">Adressen är felaktig.</span><span class="sxs-lookup"><span data-stu-id="ee09b-142">Address is incorrect.</span></span> | <span data-ttu-id="ee09b-143">Inget</span><span class="sxs-lookup"><span data-stu-id="ee09b-143">None</span></span> |
|<span data-ttu-id="ee09b-144">Inte validerat</span><span class="sxs-lookup"><span data-stu-id="ee09b-144">Not validated</span></span> | <span data-ttu-id="ee09b-145">Adressen kunde inte skickas via valideringsprocessen.</span><span class="sxs-lookup"><span data-stu-id="ee09b-145">Address was not able to be sent through the validation process.</span></span> | <span data-ttu-id="ee09b-146">Inget</span><span class="sxs-lookup"><span data-stu-id="ee09b-146">None</span></span> |

<span data-ttu-id="ee09b-147">Amerikanska postkoder returnerar ytterligare 4 siffror + bindestreck , till exempel 12345-6789.</span><span class="sxs-lookup"><span data-stu-id="ee09b-147">US post codes will return an additional 4 digits + hyphen - for example, 12345-6789.</span></span>

<span data-ttu-id="ee09b-148">När en adress har skickats för validering via API:et validate address returneras följande svarsschema:</span><span class="sxs-lookup"><span data-stu-id="ee09b-148">Once an address is submitted for validation via the Validate Address API, the following response schema will be returned:</span></span>

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

<span data-ttu-id="ee09b-149">Ta en titt på det här exempelsvaret.</span><span class="sxs-lookup"><span data-stu-id="ee09b-149">Take a look at this sample response.</span></span> <span data-ttu-id="ee09b-150">Observera att för USA returnerar svaret ytterligare ett fyrsiffrigt suffix för postnummerraden om du bara anger fem siffror för postnumret.</span><span class="sxs-lookup"><span data-stu-id="ee09b-150">Note that for the US, the response will return an additional four-digit suffix for the postal code line if you only enter five digits for the zip code.</span></span>

```csharp

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

### <a name="next-steps"></a><span data-ttu-id="ee09b-151">Nästa steg</span><span class="sxs-lookup"><span data-stu-id="ee09b-151">Next steps</span></span>

- <span data-ttu-id="ee09b-152">Dela ditt klientorganisations-ID för sandbox-miljön med ämnesexperten (AliJektki) som ska ingå i testresan, så att du kan börja förbereda dig för uppdateringen.</span><span class="sxs-lookup"><span data-stu-id="ee09b-152">Share your sandbox tenant ID with the subject matter expert (Ali Khaki) to be included in the test flight, so that you can begin preparing for the update.</span></span>

- <span data-ttu-id="ee09b-153">Om du använder en CPV-lösning (Kontrollpanelens leverantör) kan du kontakta din CPV.</span><span class="sxs-lookup"><span data-stu-id="ee09b-153">If you’re using a control panel vendor (CPV) solution, consult your CPV.</span></span>

### <a name="questions"></a><span data-ttu-id="ee09b-154">Har du några frågor?</span><span class="sxs-lookup"><span data-stu-id="ee09b-154">Questions?</span></span>

<span data-ttu-id="ee09b-155">Om du behöver support för din verksamhet med Microsoft kan du kontakta yammer-gruppen som din partner har stöd för.</span><span class="sxs-lookup"><span data-stu-id="ee09b-155">If you need support for your operations with Microsoft, reach out to your partner support Yammer group.</span></span>

### <a name="change-log"></a><span data-ttu-id="ee09b-156">Ändringslogg:</span><span class="sxs-lookup"><span data-stu-id="ee09b-156">Change log:</span></span>

- <span data-ttu-id="ee09b-157">31 mars 2020: Ursprunglig publikation</span><span class="sxs-lookup"><span data-stu-id="ee09b-157">March 31, 2020: Original publication</span></span>

- <span data-ttu-id="ee09b-158">30 april 2021: Uppdateringar för exempelsvar och postnummerinformation</span><span class="sxs-lookup"><span data-stu-id="ee09b-158">April 30, 2021: Updates for sample response and Zip code details</span></span>

________________
## <a name="new-exchange-admin-center-eac-experience"></a><a name="17"></a><span data-ttu-id="ee09b-159">Ny upplevelse för Administrationscenter för Exchange (EAC)</span><span class="sxs-lookup"><span data-stu-id="ee09b-159">New Exchange admin center (EAC) experience</span></span>

### <a name="categories"></a><span data-ttu-id="ee09b-160">Kategorier</span><span class="sxs-lookup"><span data-stu-id="ee09b-160">Categories</span></span>

- <span data-ttu-id="ee09b-161">Datum: 2021-03-29</span><span class="sxs-lookup"><span data-stu-id="ee09b-161">Date: 2021-03-29</span></span>
- <span data-ttu-id="ee09b-162">Funktioner</span><span class="sxs-lookup"><span data-stu-id="ee09b-162">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="ee09b-163">Sammanfattning</span><span class="sxs-lookup"><span data-stu-id="ee09b-163">Summary</span></span>

<span data-ttu-id="ee09b-164">Från och med 27 april 2021 kommer Administrationscenter för Exchange (EAC) att distribuera en ny upplevelse som förbättrar den dagliga effektiviteten för användarna.</span><span class="sxs-lookup"><span data-stu-id="ee09b-164">Starting April 27, 2021, the Exchange admin center (EAC) will roll out a new experience that will improve day-to-day efficiency for users.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="ee09b-165">Målgrupp som påverkas</span><span class="sxs-lookup"><span data-stu-id="ee09b-165">Impacted audience</span></span>

<span data-ttu-id="ee09b-166">Delegerade administratörer som har åtkomst till Exchange via Partnercenter</span><span class="sxs-lookup"><span data-stu-id="ee09b-166">Delegated admins accessing Exchange through Partner Center</span></span>

### <a name="details"></a><span data-ttu-id="ee09b-167">Information</span><span class="sxs-lookup"><span data-stu-id="ee09b-167">Details</span></span>

<span data-ttu-id="ee09b-168">Från och med 27 april 2021 omdirigeras partner som navigerar till Exchange via Partnercenter till den nya EAC:en.</span><span class="sxs-lookup"><span data-stu-id="ee09b-168">Starting April 27, 2021, partners who navigate to Exchange through Partner Center will be redirected to the new EAC.</span></span>

<span data-ttu-id="ee09b-169">Den här nya upplevelsen är för närvarande tillgänglig som en förhandsversion, och administratörer kan aktivera den här funktionen genom att välja växlingsknappen i det övre högra hörnet i den klassiska EAC.</span><span class="sxs-lookup"><span data-stu-id="ee09b-169">This new experience is currently available as a preview, and admins can activate this experience by selecting the toggle on the top right corner within the classic EAC.</span></span> <span data-ttu-id="ee09b-170">De kan också navigera till den nya EAC genom att välja banderollen "Prova nu" som visas på alla sidor.</span><span class="sxs-lookup"><span data-stu-id="ee09b-170">They can also navigate to the new EAC by selecting the “Try it now” banner that’s displayed on all the pages.</span></span>

<span data-ttu-id="ee09b-171">Fördelarna med den nya EAC:en är:</span><span class="sxs-lookup"><span data-stu-id="ee09b-171">Benefits of the new EAC include:</span></span>

- <span data-ttu-id="ee09b-172">Lade till insikter, rapporter och aviseringsmekanismer för e-postflödesrelaterade problem.</span><span class="sxs-lookup"><span data-stu-id="ee09b-172">Added insights, reports, and alert mechanisms for mail flow–related issues.</span></span> 

- <span data-ttu-id="ee09b-173">Anpassade instrumentpaneler för att öka produktiviteten.</span><span class="sxs-lookup"><span data-stu-id="ee09b-173">Personalized dashboards to increase productivity.</span></span>

<span data-ttu-id="ee09b-174">Videor som hjälper dig att navigera i den nya upplevelsen finns i avsnittet **Utbildningsguide & den** nya EAC-upplevelsen.</span><span class="sxs-lookup"><span data-stu-id="ee09b-174">To help you navigate through the new experience, videos are available within the **Training & Guide** section on the new EAC experience.</span></span> <span data-ttu-id="ee09b-175">Dessa ger dig en översikt över hur du bäst kan använda den nya portalen.</span><span class="sxs-lookup"><span data-stu-id="ee09b-175">These will give you an overview of how you can best use the new portal.</span></span>

>[!NOTE]
><span data-ttu-id="ee09b-176">Med den här ändringen kommer den klassiska EAC-upplevelsen inte att bli inaktuell.</span><span class="sxs-lookup"><span data-stu-id="ee09b-176">With this change, the classic EAC experience will not be deprecated.</span></span> <span data-ttu-id="ee09b-177">Du meddelas i god tid innan någon ändring implementeras.</span><span class="sxs-lookup"><span data-stu-id="ee09b-177">You will be notified well in advance before any change is implemented.</span></span>

### <a name="next-steps"></a><span data-ttu-id="ee09b-178">Nästa steg</span><span class="sxs-lookup"><span data-stu-id="ee09b-178">Next steps</span></span>

- <span data-ttu-id="ee09b-179">Kolla in resurserna [om det här avsnittet,](https://partner.microsoft.com/resources/collection/new-exchange-admin-center-experience#/)där du kan visa skärmbilder av den nya upplevelsen.</span><span class="sxs-lookup"><span data-stu-id="ee09b-179">Check out the [resources about this topic](https://partner.microsoft.com/resources/collection/new-exchange-admin-center-experience#/), where you can view screenshots of the new experience.</span></span>

- <span data-ttu-id="ee09b-180">Dela den här informationen med lämpliga intressenter i din organisation.</span><span class="sxs-lookup"><span data-stu-id="ee09b-180">Share this information with the appropriate stakeholders in your organization.</span></span> 

### <a name="questions"></a><span data-ttu-id="ee09b-181">Har du några frågor?</span><span class="sxs-lookup"><span data-stu-id="ee09b-181">Questions?</span></span>

<span data-ttu-id="ee09b-182">Om du har frågor om dessa ändringar kan du kontrollera dina relevanta Yammer-communities.</span><span class="sxs-lookup"><span data-stu-id="ee09b-182">For any questions about these changes, check your relevant Yammer communities.</span></span>

________________
## <a name="microsoft-operations-introducing-the-product-launch-calendar"></a><a name="16"></a><span data-ttu-id="ee09b-183">Microsoft Operations: Introduktion till kalendern för produktlansering</span><span class="sxs-lookup"><span data-stu-id="ee09b-183">Microsoft Operations: Introducing the product launch calendar</span></span>

### <a name="categories"></a><span data-ttu-id="ee09b-184">Kategorier</span><span class="sxs-lookup"><span data-stu-id="ee09b-184">Categories</span></span>

- <span data-ttu-id="ee09b-185">Datum: 2021-03-25</span><span class="sxs-lookup"><span data-stu-id="ee09b-185">Date: 2021-03-25</span></span>
- <span data-ttu-id="ee09b-186">Erbjudanden | Modern arbetsplats</span><span class="sxs-lookup"><span data-stu-id="ee09b-186">Offers | Modern Workplace</span></span>

### <a name="summary"></a><span data-ttu-id="ee09b-187">Sammanfattning</span><span class="sxs-lookup"><span data-stu-id="ee09b-187">Summary</span></span>

<span data-ttu-id="ee09b-188">Som svar på partnerfeedback effektiviserar Microsoft Operations kommunikationen för produktlanseringar.</span><span class="sxs-lookup"><span data-stu-id="ee09b-188">In response to partner feedback, Microsoft Operations will streamline communications for product launches.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="ee09b-189">Påverkad målgrupp</span><span class="sxs-lookup"><span data-stu-id="ee09b-189">Impacted audience</span></span>

<span data-ttu-id="ee09b-190">Molnlösningsleverantör (CSP)-partner</span><span class="sxs-lookup"><span data-stu-id="ee09b-190">Cloud Solution Provider (CSP) partners</span></span>

### <a name="details"></a><span data-ttu-id="ee09b-191">Information</span><span class="sxs-lookup"><span data-stu-id="ee09b-191">Details</span></span>

<span data-ttu-id="ee09b-192">Microsoft strävar efter att kontinuerligt förbättra partnerupplevelserna.</span><span class="sxs-lookup"><span data-stu-id="ee09b-192">Microsoft is committed to continually improving partner experiences.</span></span> <span data-ttu-id="ee09b-193">Vi har fått feedback från dig om att du har fått för många meddelanden från Microsoft, inklusive dubbla meddelanden om produktlanseringar.</span><span class="sxs-lookup"><span data-stu-id="ee09b-193">We’ve had feedback from you that you’ve been receiving too many communications from Microsoft, including duplicate announcements for product launches.</span></span>

<span data-ttu-id="ee09b-194">Som svar på din feedback har Microsoft effektiviserat beredskapsupplevelsen för produktlanseringar för nya och befintliga erbjudanden.</span><span class="sxs-lookup"><span data-stu-id="ee09b-194">In response to your feedback, Microsoft has streamlined the readiness experience for product launches for new and existing offers.</span></span>

<span data-ttu-id="ee09b-195">Vi ger dig nu en enda månatlig vy över produktlanseringar som publicerats i resursgalleriet för driftberedskap.</span><span class="sxs-lookup"><span data-stu-id="ee09b-195">We now provide you with a single monthly view of product launches, published in the Operations readiness resource gallery.</span></span> <span data-ttu-id="ee09b-196">Den här [månatliga kalendervyn för produktlansering](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) ersätter enskilda meddelanden om produktlansering i resursgalleriet för driftberedskap och i Partnercenter-meddelanden.</span><span class="sxs-lookup"><span data-stu-id="ee09b-196">This monthly [product launch calendar view](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) will replace individual product launch communications in the Operations readiness resource gallery and in Partner Center announcements.</span></span>

<span data-ttu-id="ee09b-197">Du kan också komma åt den [här produktlanseringskalendern](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) från [communitysamlingar,](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) [kalendervyer](https://partner.microsoft.com/resources/assets#/?type=collection&search=Calendar&sort=updated)och [CSP-nyhetsbrev.](https://partner.microsoft.com/resources/collection/csp-monthly-update#/)</span><span class="sxs-lookup"><span data-stu-id="ee09b-197">You can also access this [product launch calendar](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) from [community collections](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/), [calendar views](https://partner.microsoft.com/resources/assets#/?type=collection&search=Calendar&sort=updated), and [CSP newsletters](https://partner.microsoft.com/resources/collection/csp-monthly-update#/).</span></span> <span data-ttu-id="ee09b-198">Vi meddelar dig när vi publicerar varje månads kalender för produktlansering med ett meddelande i resursgalleriet för driftberedskap.</span><span class="sxs-lookup"><span data-stu-id="ee09b-198">We’ll notify you when we publish each month’s product launch calendar with an announcement in the Operations readiness resource gallery.</span></span>

<span data-ttu-id="ee09b-199">Du hittar fortfarande information om nya och befintliga erbjudanden i förhandsgransknings- och prislistans ändringsloggar, samt i produktbloggar, licensieringsguider och marknadsföringssidor.</span><span class="sxs-lookup"><span data-stu-id="ee09b-199">You can still find information regarding new and existing offers in the price list preview and price list change logs, as well as in product blogs, licensing guides, and product marketing pages.</span></span>

<span data-ttu-id="ee09b-200">Ändringen gäller för lanseringar för följande produkter:</span><span class="sxs-lookup"><span data-stu-id="ee09b-200">The change will apply to launches for the following products:</span></span>

- <span data-ttu-id="ee09b-201">Lokal Dynamics</span><span class="sxs-lookup"><span data-stu-id="ee09b-201">Dynamics on-premises</span></span>
- <span data-ttu-id="ee09b-202">Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="ee09b-202">Microsoft 365</span></span>
- <span data-ttu-id="ee09b-203">Microsoft Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="ee09b-203">Microsoft Dynamics 365</span></span>
- <span data-ttu-id="ee09b-204">Windows</span><span class="sxs-lookup"><span data-stu-id="ee09b-204">Windows</span></span>
- <span data-ttu-id="ee09b-205">Server</span><span class="sxs-lookup"><span data-stu-id="ee09b-205">Server</span></span>  
- <span data-ttu-id="ee09b-206">Verktyg</span><span class="sxs-lookup"><span data-stu-id="ee09b-206">Tools</span></span>
- <span data-ttu-id="ee09b-207">Teams och Telco</span><span class="sxs-lookup"><span data-stu-id="ee09b-207">Teams and Telco</span></span>

<span data-ttu-id="ee09b-208">Vi fortsätter att skicka specifika meddelanden om produktlanseringar som kräver information om driftberedskap.</span><span class="sxs-lookup"><span data-stu-id="ee09b-208">We’ll continue to send specific announcements for product launches that require Operations readiness details.</span></span>

### <a name="next-steps"></a><span data-ttu-id="ee09b-209">Nästa steg</span><span class="sxs-lookup"><span data-stu-id="ee09b-209">Next steps</span></span>

<span data-ttu-id="ee09b-210">Granska resurserna om det här avsnittet och dela den här informationen med lämpliga intressenter i din organisation.</span><span class="sxs-lookup"><span data-stu-id="ee09b-210">Review the resources about this topic and share this information with the appropriate stakeholders in your organization.</span></span>

### <a name="questions"></a><span data-ttu-id="ee09b-211">Har du några frågor?</span><span class="sxs-lookup"><span data-stu-id="ee09b-211">Questions?</span></span>

<span data-ttu-id="ee09b-212">Om du har fler frågor om dessa erbjudanden kan du läsa dina relevanta Yammer-communities.</span><span class="sxs-lookup"><span data-stu-id="ee09b-212">For any further questions about these offers, check your relevant Yammer communities.</span></span>

________________
## <a name="changes-to-csp-customer-onboarding-requirements"></a><a name="15"></a><span data-ttu-id="ee09b-213">Ändringar av CSP-krav för kund-onboarding</span><span class="sxs-lookup"><span data-stu-id="ee09b-213">Changes to CSP customer onboarding requirements</span></span>

### <a name="categories"></a><span data-ttu-id="ee09b-214">Kategorier</span><span class="sxs-lookup"><span data-stu-id="ee09b-214">Categories</span></span>

- <span data-ttu-id="ee09b-215">Datum: 2021-03-25</span><span class="sxs-lookup"><span data-stu-id="ee09b-215">Date: 2021-03-25</span></span>
- <span data-ttu-id="ee09b-216">Funktioner</span><span class="sxs-lookup"><span data-stu-id="ee09b-216">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="ee09b-217">Sammanfattning</span><span class="sxs-lookup"><span data-stu-id="ee09b-217">Summary</span></span>

<span data-ttu-id="ee09b-218">Som en del av vårt åtagande att hjälpa partner och kunder att driva sin verksamhet baserat på förtroende begär vi ytterligare kundinformation från och med den 25 mars 2021.</span><span class="sxs-lookup"><span data-stu-id="ee09b-218">As part of our commitment to help partners and customers run their business based on trust, we will request additional customer information, effective March 25, 2021.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="ee09b-219">Målgrupp som påverkas</span><span class="sxs-lookup"><span data-stu-id="ee09b-219">Impacted audience</span></span>

<span data-ttu-id="ee09b-220">Molnlösningsleverantör direktfaktureringspartner och indirekta leverantörer som har nya eller befintliga kunder i de länder som anges i nästa avsnitt</span><span class="sxs-lookup"><span data-stu-id="ee09b-220">Cloud Solution Provider (CSP) direct bill partners and indirect providers who have new or existing customers in the countries listed in the next section</span></span>

### <a name="details"></a><span data-ttu-id="ee09b-221">Information</span><span class="sxs-lookup"><span data-stu-id="ee09b-221">Details</span></span>

<span data-ttu-id="ee09b-222">Microsoft körs med förtroende.</span><span class="sxs-lookup"><span data-stu-id="ee09b-222">Microsoft runs on trust.</span></span> <span data-ttu-id="ee09b-223">Vi strävar efter att tillhandahålla en kompatibel, säker och säker metod för kundvalidering för att kunna göra kundprenumerationer i CSP-programmet.</span><span class="sxs-lookup"><span data-stu-id="ee09b-223">We’re committed to providing a compliant, safe, and secure method of customer validation for transacting customer subscriptions in the CSP program.</span></span> <span data-ttu-id="ee09b-224">Den 25 mars 2021 introducerar vi förbättringar av Partner Center API och användargränssnitt som påverkar partner som uppfyller båda följande kriterier:</span><span class="sxs-lookup"><span data-stu-id="ee09b-224">On March 25, 2021, we will be introducing Partner Center API and user interface (UI) enhancements that will affect partners who meet both of the following criteria:</span></span>

1. <span data-ttu-id="ee09b-225">Partnern har en direkt faktureringsrelation med Microsoft (vilket innebär att partnern antingen är en partner för direktfakturering eller en indirekt leverantör).</span><span class="sxs-lookup"><span data-stu-id="ee09b-225">The partner has a direct billing relationship with Microsoft (which means that the partner is either a direct bill partner or an indirect provider).</span></span>

2. <span data-ttu-id="ee09b-226">Partnern gör affärer med nya eller befintliga kunder i följande länder:</span><span class="sxs-lookup"><span data-stu-id="ee09b-226">The partner does business with new or existing customers in the following countries:</span></span>

    - <span data-ttu-id="ee09b-227">Thailand</span><span class="sxs-lookup"><span data-stu-id="ee09b-227">Thailand</span></span>
    - <span data-ttu-id="ee09b-228">Vietnam</span><span class="sxs-lookup"><span data-stu-id="ee09b-228">Vietnam</span></span>
    - <span data-ttu-id="ee09b-229">Turkiet</span><span class="sxs-lookup"><span data-stu-id="ee09b-229">Turkey</span></span>
    - <span data-ttu-id="ee09b-230">Polen</span><span class="sxs-lookup"><span data-stu-id="ee09b-230">Poland</span></span>
    - <span data-ttu-id="ee09b-231">Sydafrika</span><span class="sxs-lookup"><span data-stu-id="ee09b-231">South Africa</span></span>
    - <span data-ttu-id="ee09b-232">Indien</span><span class="sxs-lookup"><span data-stu-id="ee09b-232">India</span></span>
    - <span data-ttu-id="ee09b-233">Brasilien</span><span class="sxs-lookup"><span data-stu-id="ee09b-233">Brazil</span></span>
    - <span data-ttu-id="ee09b-234">Irak</span><span class="sxs-lookup"><span data-stu-id="ee09b-234">Iraq</span></span>
    - <span data-ttu-id="ee09b-235">Myanmar</span><span class="sxs-lookup"><span data-stu-id="ee09b-235">Myanmar</span></span>
    - <span data-ttu-id="ee09b-236">Sydsudan</span><span class="sxs-lookup"><span data-stu-id="ee09b-236">South Sudan</span></span>
    - <span data-ttu-id="ee09b-237">Saudiarabien</span><span class="sxs-lookup"><span data-stu-id="ee09b-237">Saudi Arabia</span></span>
    - <span data-ttu-id="ee09b-238">Förenade Arabemiraten</span><span class="sxs-lookup"><span data-stu-id="ee09b-238">United Arab Emirates</span></span>
    - <span data-ttu-id="ee09b-239">Venezuela</span><span class="sxs-lookup"><span data-stu-id="ee09b-239">Venezuela</span></span>

<span data-ttu-id="ee09b-240">Partner som uppfyller villkoren måste skicka in en kunds företagsregistrerings-ID (kallas även  kundens **organisation INN)** och telefonnummer när de registrera nya kunder eller ändra befintlig kundinformation. </span><span class="sxs-lookup"><span data-stu-id="ee09b-240">Partners who meet the criteria will have to submit a customer's **company registration ID** (also known as the customer's **organization INN**) and **phone number** when they onboard new customers or modify existing customer details.</span></span> <span data-ttu-id="ee09b-241">Dessa partner kan också ange ett **mellannamn** för kunden (valfritt).</span><span class="sxs-lookup"><span data-stu-id="ee09b-241">These partners can also enter an optional **middle name** for the customer.</span></span>

<span data-ttu-id="ee09b-242">Observera att när du lägger till ditt företagsregistrerings-ID bör du använda ditt företagsskatte-ID och inte kundens personliga ID.</span><span class="sxs-lookup"><span data-stu-id="ee09b-242">Note that when you add your company registration ID you should use your business tax ID and not the customer personal ID.</span></span>

<span data-ttu-id="ee09b-243">Partner som gör affärer med nya eller befintliga kunder i följande länder har redan fått en tidigare version i november 2020.</span><span class="sxs-lookup"><span data-stu-id="ee09b-243">Partners who do business with new or existing customers in the following countries have already been onboarded with a previous release in November 2020.</span></span>

- <span data-ttu-id="ee09b-244">Armenien</span><span class="sxs-lookup"><span data-stu-id="ee09b-244">Armenia</span></span>
- <span data-ttu-id="ee09b-245">Azerbajdzjan</span><span class="sxs-lookup"><span data-stu-id="ee09b-245">Azerbaijan</span></span>
- <span data-ttu-id="ee09b-246">Vitryssland</span><span class="sxs-lookup"><span data-stu-id="ee09b-246">Belarus</span></span>
- <span data-ttu-id="ee09b-247">Ungern</span><span class="sxs-lookup"><span data-stu-id="ee09b-247">Hungary</span></span>
- <span data-ttu-id="ee09b-248">Kazakstan</span><span class="sxs-lookup"><span data-stu-id="ee09b-248">Kazakhstan</span></span>
- <span data-ttu-id="ee09b-249">Kirgizistan</span><span class="sxs-lookup"><span data-stu-id="ee09b-249">Kyrgyzstan</span></span>
- <span data-ttu-id="ee09b-250">Moldavien</span><span class="sxs-lookup"><span data-stu-id="ee09b-250">Moldova</span></span>
- <span data-ttu-id="ee09b-251">Ryssland</span><span class="sxs-lookup"><span data-stu-id="ee09b-251">Russia</span></span>
- <span data-ttu-id="ee09b-252">Tadzjikistan</span><span class="sxs-lookup"><span data-stu-id="ee09b-252">Tajikistan</span></span>
- <span data-ttu-id="ee09b-253">Ukraina</span><span class="sxs-lookup"><span data-stu-id="ee09b-253">Ukraine</span></span>
- <span data-ttu-id="ee09b-254">Uzbekistan</span><span class="sxs-lookup"><span data-stu-id="ee09b-254">Uzbekistan</span></span>

<span data-ttu-id="ee09b-255">Partner med kunder i resten av världen kan den 25 mars 2021 ange företagets  **registrerings-ID,** telefonnummer och mellannamn för kunder som valfri information.</span><span class="sxs-lookup"><span data-stu-id="ee09b-255">Partners with customers in the rest of the world will have the ability on March 25, 2021 to enter the **company registration ID**, **phone number**, and **middle name** for customers as optional details.</span></span>

### <a name="next-steps"></a><span data-ttu-id="ee09b-256">Nästa steg</span><span class="sxs-lookup"><span data-stu-id="ee09b-256">Next steps</span></span>

- <span data-ttu-id="ee09b-257">Mer detaljerad vägledning finns i den tekniska dokumentationen och vanliga frågor [och svar i](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/) den dedikerade partnersamlingen.</span><span class="sxs-lookup"><span data-stu-id="ee09b-257">Review the technical documentation and frequently asked questions in the [dedicated partner collection](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/) for more detailed guidance.</span></span>

- <span data-ttu-id="ee09b-258">Förbered för att införliva ändringarna med partnercenter-API:et och webbanvändarupplevelsen.</span><span class="sxs-lookup"><span data-stu-id="ee09b-258">Prepare to incorporate the changes using the Partner Center API and web user experience.</span></span> <span data-ttu-id="ee09b-259">API/SDK:er kommer att vara tillgängliga för testning.</span><span class="sxs-lookup"><span data-stu-id="ee09b-259">API/SDKs will be available for testing.</span></span>

- <span data-ttu-id="ee09b-260">Se till att skicka in ytterligare data när du registrera nya kunder eller ändrar befintlig kundinformation.</span><span class="sxs-lookup"><span data-stu-id="ee09b-260">Make sure to submit the additional data when onboarding new customers or modifying existing customer details.</span></span>

- <span data-ttu-id="ee09b-261">Om du använder en CPV-lösning (Kontrollpanelens leverantör) kan du kontakta din CPV.</span><span class="sxs-lookup"><span data-stu-id="ee09b-261">If you’re using a control panel vendor (CPV) solution, consult your CPV.</span></span>

### <a name="questions"></a><span data-ttu-id="ee09b-262">Har du några frågor?</span><span class="sxs-lookup"><span data-stu-id="ee09b-262">Questions?</span></span>

<span data-ttu-id="ee09b-263">Kontakta skatterådgivaren eller det lokala skattekontoret om du har frågor om den juridiska identifieraren (kallas även INN eller TIN).</span><span class="sxs-lookup"><span data-stu-id="ee09b-263">Contact your tax advisor or local tax office if you have any questions related to the legal identifier (also called INN or TIN).</span></span> <span data-ttu-id="ee09b-264">Microsoft kan inte ge vägledning om skattefrågor.</span><span class="sxs-lookup"><span data-stu-id="ee09b-264">Microsoft cannot provide guidance on tax matters.</span></span>

<span data-ttu-id="ee09b-265">Om du behöver support för din verksamhet med Microsoft öppnar [du en tjänstbegäran.](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=aa679372-d996-73df-e244-cb28bbbf28e8)</span><span class="sxs-lookup"><span data-stu-id="ee09b-265">If you need support in your operations with Microsoft, [open a service request](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=aa679372-d996-73df-e244-cb28bbbf28e8).</span></span>

________________
## <a name="corrections-made-to-march-1-2021-perpetual-software-price-list"></a><a name="14"></a><span data-ttu-id="ee09b-266">Korrigeringar som gjorts för 1 mars 2021 permanent programvaruprislista</span><span class="sxs-lookup"><span data-stu-id="ee09b-266">Corrections made to March 1, 2021 perpetual software price list</span></span>

### <a name="categories"></a><span data-ttu-id="ee09b-267">Kategorier</span><span class="sxs-lookup"><span data-stu-id="ee09b-267">Categories</span></span>

- <span data-ttu-id="ee09b-268">Datum: 2021-03-23</span><span class="sxs-lookup"><span data-stu-id="ee09b-268">Date: 2021-03-23</span></span>
- <span data-ttu-id="ee09b-269">Erbjudanden/marknader</span><span class="sxs-lookup"><span data-stu-id="ee09b-269">Offers/Markets</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="ee09b-270">Påverkad målgrupp</span><span class="sxs-lookup"><span data-stu-id="ee09b-270">Impacted audience</span></span>

<span data-ttu-id="ee09b-271">Indirekta leverantörer och direktfaktureringspartner som använder permanent programvara i Molnlösningsleverantör program</span><span class="sxs-lookup"><span data-stu-id="ee09b-271">Indirect providers and direct bill partners transacting perpetual software in the Cloud Solution Provider program</span></span> 

### <a name="details"></a><span data-ttu-id="ee09b-272">Information</span><span class="sxs-lookup"><span data-stu-id="ee09b-272">Details</span></span>

<span data-ttu-id="ee09b-273">Prislistan för permanent programvara som publicerades den 1 mars 2021 innehöll marknader som inte borde ha funnits där.</span><span class="sxs-lookup"><span data-stu-id="ee09b-273">The price list for perpetual software posted on March 1, 2021 included markets that should not have been there.</span></span> <span data-ttu-id="ee09b-274">Den permanenta programvaruprislistan uppdaterades den 17 mars 2021 med korrigeringarna.</span><span class="sxs-lookup"><span data-stu-id="ee09b-274">The perpetual software price list was updated on March 17, 2021 with the corrections.</span></span> <span data-ttu-id="ee09b-275">De här korrigeringarna gäller endast för:</span><span class="sxs-lookup"><span data-stu-id="ee09b-275">These corrections were only applicable to:</span></span>

- <span data-ttu-id="ee09b-276">Produkt-ID: DF77X4D43RKT</span><span class="sxs-lookup"><span data-stu-id="ee09b-276">Product ID: DF77X4D43RKT</span></span> 
- <span data-ttu-id="ee09b-277">Produktnamn: Windows 10 Home pro-uppgradering för Microsoft 365 företag</span><span class="sxs-lookup"><span data-stu-id="ee09b-277">Product name: Windows 10 Home to Pro Upgrade for Microsoft 365 Business</span></span>
- <span data-ttu-id="ee09b-278">Borttagna eller icke-stödda marknader: AE, AF, AL, AM, AO, BA, BB, BD, BM, BN, BO, BR, BS, BW, BY, BZ, CI, CL, CM, CO, CR, CW, DO, DZ, EC, EG, ET, FJ, FO, GE, GH, GT, HN, IL, IN, IQ, JM, JO, KE, KG, KN, CR, KY, KZ, LB, LK, LY, MA, MC, MD, ME, MN, MO, MU, NA, NG , NI, NP, OM, PA, PE, PH, PK, PR, PY, QA, RS, RU, RW, SG, SN, SV, TH, TJ, TM, TN, TT, TZ, UA, UG, UY, CUS, VE, VN, YE, ZM, ZW</span><span class="sxs-lookup"><span data-stu-id="ee09b-278">Removed or unsupported markets: AE, AF, AL, AM, AO, BA, BB, BD, BH, BM, BN, BO, BR, BS, BW, BY, BZ, CI, CL, CM, CO, CR, CW, DO, DZ, EC, EG, ET, FJ, FO, GE, GH, GT, HN, IL, IN, IQ, JM, JO, KE, KG, KN, KW, KY, KZ, LB, LK, LY, MA, MC, MD, ME, MN, MO, MU, NA, NG, NI, NP, OM, PA, PE, PH, PK, PR, PY, QA, RS, RU, RW, SG, SN, SV, TH, TJ, TM, TN, TT, TZ, UA, UG, UY, UZ, VE, VN, YE, ZM, ZW</span></span>

<span data-ttu-id="ee09b-279">Dessa ändringar gäller endast för ovanstående produkt.</span><span class="sxs-lookup"><span data-stu-id="ee09b-279">These changes only apply to the above product.</span></span> <span data-ttu-id="ee09b-280">Andra produkter hade inga korrigeringar.</span><span class="sxs-lookup"><span data-stu-id="ee09b-280">Other products had no corrections.</span></span> 

### <a name="next-steps-and-resources"></a><span data-ttu-id="ee09b-281">Nästa steg och resurser</span><span class="sxs-lookup"><span data-stu-id="ee09b-281">Next steps and resources</span></span>

- <span data-ttu-id="ee09b-282">Partner som överlappar permanent programvara bör ladda ned den senaste permanenta programvaruprislistan.</span><span class="sxs-lookup"><span data-stu-id="ee09b-282">Partners who transact perpetual software should download the latest perpetual software price list.</span></span>
- <span data-ttu-id="ee09b-283">Se [landskoderna för regionen för](https://docs.microsoft.com/azure/marketplace/commercial-marketplace-co-sell-countries) en användarvänlig mappning av förkortningen på två bokstäver till länder.</span><span class="sxs-lookup"><span data-stu-id="ee09b-283">Consult the [region country codes](https://docs.microsoft.com/azure/marketplace/commercial-marketplace-co-sell-countries) for a friendly mapping of the two letter abbreviation to countries.</span></span>
________________
## <a name="sdk-release-on-net-standard-v1170"></a><a name="13"></a> <span data-ttu-id="ee09b-284">SDK-version på .NET Standard (v1.17.0)</span><span class="sxs-lookup"><span data-stu-id="ee09b-284">SDK Release on .NET Standard (v1.17.0)</span></span>

### <a name="categories"></a><span data-ttu-id="ee09b-285">Kategorier</span><span class="sxs-lookup"><span data-stu-id="ee09b-285">Categories</span></span>

- <span data-ttu-id="ee09b-286">Datum: 2021-03-23</span><span class="sxs-lookup"><span data-stu-id="ee09b-286">Date: 2021-03-23</span></span>

- <span data-ttu-id="ee09b-287">Funktioner</span><span class="sxs-lookup"><span data-stu-id="ee09b-287">Capabilities</span></span>
 
### <a name="impacted-audience"></a><span data-ttu-id="ee09b-288">Målgrupp som påverkas</span><span class="sxs-lookup"><span data-stu-id="ee09b-288">Impacted audience</span></span>

<span data-ttu-id="ee09b-289">Direktfaktureringspartner och indirekta leverantörer som deltar i CSP-programmet som använder Partner Center .NET SDK.</span><span class="sxs-lookup"><span data-stu-id="ee09b-289">Direct Bill partners and Indirect Providers participating in the CSP program who are using the Partner Center .NET SDK.</span></span>

### <a name="details"></a><span data-ttu-id="ee09b-290">Information</span><span class="sxs-lookup"><span data-stu-id="ee09b-290">Details</span></span>

<span data-ttu-id="ee09b-291">Från och med 23 mars 2020 kan partner börja ladda ned versionen av [MicrosoftPartnerCenter.NETSDK (NuGet-| Microsoft.Store.PartnerCenter 1.17.0)](https://www.nuget.org/packages/Microsoft.Store.PartnerCenter/1.17.0), tillsammans med uppdaterade offentliga Partnercenter-SDK [GitHub-exempel](https://github.com/Microsoft/Partner-Center-DotNet-Samples).</span><span class="sxs-lookup"><span data-stu-id="ee09b-291">As of March 23 2020, Partners can start downloading the version of [MicrosoftPartnerCenter.NETSDK (NuGet Gallery | Microsoft.Store.PartnerCenter 1.17.0)](https://www.nuget.org/packages/Microsoft.Store.PartnerCenter/1.17.0), along with updated public Partner Center SDK [GitHub samples](https://github.com/Microsoft/Partner-Center-DotNet-Samples).</span></span> <span data-ttu-id="ee09b-292">Den här versionen innehåller uppdateringar av följande metoder:</span><span class="sxs-lookup"><span data-stu-id="ee09b-292">This version includes updates to the following methods:</span></span>

#### <a name="audit-updated-new-operation-types"></a><span data-ttu-id="ee09b-293">Granska uppdaterad: Nya åtgärdstyper</span><span class="sxs-lookup"><span data-stu-id="ee09b-293">Audit Updated: New operation types</span></span>

<span data-ttu-id="ee09b-294">Nya [åtgärdstyper har lagts](https://docs.microsoft.com/partner-center/develop/auditing-resources) till för att veta när kunden godkänt och avslutat DAP.</span><span class="sxs-lookup"><span data-stu-id="ee09b-294">Added new [operation types](https://docs.microsoft.com/partner-center/develop/auditing-resources) for knowing when the customer approved and terminated DAP.</span></span>

- <span data-ttu-id="ee09b-295">DapAdminRelationshipApproved</span><span class="sxs-lookup"><span data-stu-id="ee09b-295">DapAdminRelationshipApproved</span></span>

- <span data-ttu-id="ee09b-296">DapAdminRelationshipTerminated</span><span class="sxs-lookup"><span data-stu-id="ee09b-296">DapAdminRelationshipTerminated</span></span>

#### <a name="audit-updated-new-resource-and-operation-types"></a><span data-ttu-id="ee09b-297">Granska uppdaterad: Nya resurs- och åtgärdstyper</span><span class="sxs-lookup"><span data-stu-id="ee09b-297">Audit Updated: New resource and operation types</span></span>

<span data-ttu-id="ee09b-298">Nya [resurs- och åtgärdstyper har lagts](https://docs.microsoft.com/partner-center/develop/auditing-resources) till för att stödja scenariot med kundkatalogrollen.</span><span class="sxs-lookup"><span data-stu-id="ee09b-298">Added new [resource and operation types](https://docs.microsoft.com/partner-center/develop/auditing-resources) for supporting the customer directory role scenario.</span></span>

- <span data-ttu-id="ee09b-299">Ny resurstyp: "CustomerDirectoryRole"</span><span class="sxs-lookup"><span data-stu-id="ee09b-299">New resource type “CustomerDirectoryRole”</span></span>

- <span data-ttu-id="ee09b-300">Åtgärdstyperna "AddUserMember" och "RemoveUserMember"</span><span class="sxs-lookup"><span data-stu-id="ee09b-300">Operation types “AddUserMember” and “RemoveUserMember”</span></span>

#### <a name="sdk-updates-to-customer-accounts"></a><span data-ttu-id="ee09b-301">SDK-uppdateringar till kundkonton</span><span class="sxs-lookup"><span data-stu-id="ee09b-301">SDK Updates to customer accounts</span></span>

- <span data-ttu-id="ee09b-302">Stöd för GET /customers/{customer-tenant-id}/directSignedMicrosoftCustomerAgreementStatus</span><span class="sxs-lookup"><span data-stu-id="ee09b-302">Support for GET /customers/{customer-tenant-id}/directSignedMicrosoftCustomerAgreementStatus</span></span>

- <span data-ttu-id="ee09b-303">GET /customers/{customer-tenant-id}/kvalificering</span><span class="sxs-lookup"><span data-stu-id="ee09b-303">GET /customers/{customer-tenant-id}/qualifications</span></span>

- <span data-ttu-id="ee09b-304">POST /customers/{customer_id}/qualifications?code={validationCode}</span><span class="sxs-lookup"><span data-stu-id="ee09b-304">POST /customers/{customer_id}/qualifications?code={validationCode}</span></span>

#### <a name="additional-changes"></a><span data-ttu-id="ee09b-305">Ytterligare ändringar</span><span class="sxs-lookup"><span data-stu-id="ee09b-305">Additional changes</span></span>

<span data-ttu-id="ee09b-306">Följande ändringar introduceras som en del av New Commerce och är för närvarande endast tillgängliga genom inbjudan till partner som ingår i den tekniska förhandsversionen av den nya M365/D365-upplevelsen.</span><span class="sxs-lookup"><span data-stu-id="ee09b-306">The following changes are introduced as part of New Commerce, and are currently available by invitation only to partners who are part of the M365/D365 New Commerce experience technical preview.</span></span> <span data-ttu-id="ee09b-307">Partner som inte är en del av den tekniska förhandsversionen av Ny handel bör inte märka påverkan och bör vara bakåtkompatibla.</span><span class="sxs-lookup"><span data-stu-id="ee09b-307">Partners who are not part of the New Commerce technical preview should not notice impacts and should be backward compatible.</span></span>

- <span data-ttu-id="ee09b-308">Katalogändringar:</span><span class="sxs-lookup"><span data-stu-id="ee09b-308">Catalog Changes:</span></span>

  - <span data-ttu-id="ee09b-309">GET /products/{product-id}/skus/{sku-id}</span><span class="sxs-lookup"><span data-stu-id="ee09b-309">GET /products/{product-id}/skus/{sku-id}</span></span>

- <span data-ttu-id="ee09b-310">Köp och hantera:</span><span class="sxs-lookup"><span data-stu-id="ee09b-310">Purchase and Manage:</span></span>
  - <span data-ttu-id="ee09b-311">GET /customers/{customerId}/subscriptions</span><span class="sxs-lookup"><span data-stu-id="ee09b-311">GET /customers/{customerId}/subscriptions</span></span>
  - <span data-ttu-id="ee09b-312">GET /customers/{customerId}/subscriptions/{subscriptionId}</span><span class="sxs-lookup"><span data-stu-id="ee09b-312">GET /customers/{customerId}/subscriptions/{subscriptionId}</span></span>
  - <span data-ttu-id="ee09b-313">PATCH /customers/{customerId}/subscriptions/{subscriptionId}</span><span class="sxs-lookup"><span data-stu-id="ee09b-313">PATCH /customers/{customerId}/subscriptions/{subscriptionId}</span></span>
  - <span data-ttu-id="ee09b-314">GET /customers/{customerId}/subscriptions/{subscriptionId}/transitioneligibilities</span><span class="sxs-lookup"><span data-stu-id="ee09b-314">GET /customers/{customerId}/subscriptions/{subscriptionId}/transitioneligibilities</span></span>
  - <span data-ttu-id="ee09b-315">GET /customers/{customerId}/subscriptions/{subscriptionId}/transitions</span><span class="sxs-lookup"><span data-stu-id="ee09b-315">GET /customers/{customerId}/subscriptions/{subscriptionId}/transitions</span></span>
  - <span data-ttu-id="ee09b-316">POST /customers/{customerId}/subscriptions/{subscriptionId}/transitions</span><span class="sxs-lookup"><span data-stu-id="ee09b-316">POST /customers/{customerId}/subscriptions/{subscriptionId}/transitions</span></span>

### <a name="next-steps"></a><span data-ttu-id="ee09b-317">Nästa steg</span><span class="sxs-lookup"><span data-stu-id="ee09b-317">Next Steps</span></span>

- <span data-ttu-id="ee09b-318">Ladda ned den senaste [versionen av MicrosoftPartnerCenter.NETSDK (NuGet-| Microsoft.Store.PartnerCenter 1.17.0)](https://www.nuget.org/packages/Microsoft.Store.PartnerCenter/1.17.0)</span><span class="sxs-lookup"><span data-stu-id="ee09b-318">Download the latest version [MicrosoftPartnerCenter.NETSDK (NuGet Gallery | Microsoft.Store.PartnerCenter 1.17.0)](https://www.nuget.org/packages/Microsoft.Store.PartnerCenter/1.17.0)</span></span>
- <span data-ttu-id="ee09b-319">Ladda ned och granska [GitHub-exemplen](https://github.com/Microsoft/Partner-Center-DotNet-Samples)</span><span class="sxs-lookup"><span data-stu-id="ee09b-319">Download and review the [GitHub samples](https://github.com/Microsoft/Partner-Center-DotNet-Samples)</span></span>

________________
## <a name="csp-commercial-marketplace-offer-and-fy21-csp-incentives-for-eligible-offers"></a><a name="12"></a><span data-ttu-id="ee09b-320">CSP Commercial Marketplace-erbjudande och FY21 CSP-incitament för berättigade erbjudanden</span><span class="sxs-lookup"><span data-stu-id="ee09b-320">CSP commercial marketplace offer and FY21 CSP incentives for eligible offers</span></span>

### <a name="categories"></a><span data-ttu-id="ee09b-321">Kategorier</span><span class="sxs-lookup"><span data-stu-id="ee09b-321">Categories</span></span>

- <span data-ttu-id="ee09b-322">Datum: 2021-03-18</span><span class="sxs-lookup"><span data-stu-id="ee09b-322">Date: 2021-03-18</span></span>
- <span data-ttu-id="ee09b-323">Funktioner</span><span class="sxs-lookup"><span data-stu-id="ee09b-323">Capabilities</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="ee09b-324">Påverkad målgrupp</span><span class="sxs-lookup"><span data-stu-id="ee09b-324">Impacted audience</span></span>

<span data-ttu-id="ee09b-325">Indirekta leverantörer och direktfaktureringspartner i Molnlösningsleverantör program</span><span class="sxs-lookup"><span data-stu-id="ee09b-325">Indirect providers and direct bill partners in the Cloud Solution Provider program</span></span> 

### <a name="details"></a><span data-ttu-id="ee09b-326">Information</span><span class="sxs-lookup"><span data-stu-id="ee09b-326">Details</span></span>

<span data-ttu-id="ee09b-327">Indirekta leverantörer och direktfaktureringspartner i Molnlösningsleverantör-programmet kan sälja erbjudanden från tredje part och få incitament för varje kvalificerande tredjepartserbjudande som erbjuds i Partnercenter eller Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="ee09b-327">Indirect providers and direct bill partners in the Cloud Solution Provider program can sell third party offers and earn a rebate incentive for each eligible third-party offer transacted in Partner Center or the Azure portal.</span></span> <span data-ttu-id="ee09b-328">Incitamentet är i form av en kontakt med fakturerad försäljning för de berättigade erbjudandena och är tillgängligt fram till **den 30 juni 2021.**</span><span class="sxs-lookup"><span data-stu-id="ee09b-328">The incentive will be in the form of a rebate on billed sales for the eligible offers and is **available until June 30, 2021**.</span></span>  

<span data-ttu-id="ee09b-329">Fortsätt lära dig mer om denna CSP Commercial Marketplace-erbjudande nedan och kontakta dina kunder idag för att identifiera rätt erbjudanden för att möjliggöra fortsatt framgång och digital omvandling.</span><span class="sxs-lookup"><span data-stu-id="ee09b-329">Continue learning about this CSP Commercial Marketplace Offer incentive below and contact your customers today to identify the right offers to enable their continued success and digital transformation.</span></span>

<span data-ttu-id="ee09b-330">Vi samarbetar med oberoende programvaruleverantörer (ISV: er) för att få de senaste IaaS- och SaaS-lösningarna till marknaden för Microsoft-kunder.</span><span class="sxs-lookup"><span data-stu-id="ee09b-330">We partner with Independent Software Vendors (ISVs) to bring the latest IaaS and SaaS solutions to market for Microsoft customers.</span></span> <span data-ttu-id="ee09b-331">ISV-utgivare har möjlighet att aktivera försäljning av sina erbjudanden via Microsofts partnerkanal.</span><span class="sxs-lookup"><span data-stu-id="ee09b-331">ISV publishers have the option of enabling sales of their offers through the Microsoft partner channel.</span></span> <span data-ttu-id="ee09b-332">Våra incitamentberättigade erbjudanden är indela i två kategorier:</span><span class="sxs-lookup"><span data-stu-id="ee09b-332">Our incentive-eligible offers fall into two categories:</span></span>

- <span data-ttu-id="ee09b-333">Välj SaaS- och IaaS-erbjudanden från tredje part med incentiviserad status för sälj- och säljförsäljning i Azure IP.</span><span class="sxs-lookup"><span data-stu-id="ee09b-333">Select SaaS and IaaS third-party offers with Azure IP co-sell incentivized status.</span></span> 

- <span data-ttu-id="ee09b-334">SaaS-program som är integrerade med Teams eller minst två Microsoft 365 produktivitetsappar, till exempel PowerPoint, Word, Excel, Outlook eller SharePoint.</span><span class="sxs-lookup"><span data-stu-id="ee09b-334">SaaS applications integrated with Teams or at least two Microsoft 365 productivity apps, such as PowerPoint, Word, Excel, Outlook, or SharePoint.</span></span>

### <a name="next-steps-and-resources"></a><span data-ttu-id="ee09b-335">Nästa steg och resurser</span><span class="sxs-lookup"><span data-stu-id="ee09b-335">Next steps and resources</span></span>

- <span data-ttu-id="ee09b-336">Lär dig mer om att [tjäna partnerincitament](https://partner.microsoft.com/membership/partner-incentives) för att sälja berättigade Marketplace-appar för berättigade incitamentappar.</span><span class="sxs-lookup"><span data-stu-id="ee09b-336">Learn about earning [Partner Incentives](https://partner.microsoft.com/membership/partner-incentives) for selling eligible marketplace apps the incentive eligible apps.</span></span> <span data-ttu-id="ee09b-337">Nya erbjudanden läggs till varje månad.</span><span class="sxs-lookup"><span data-stu-id="ee09b-337">New offers are added monthly.</span></span>  
- [<span data-ttu-id="ee09b-338">Molnlösningsleverantör direktfakturering av partnerincitamentresurser</span><span class="sxs-lookup"><span data-stu-id="ee09b-338">Cloud Solution Provider direct bill partner incentive resources</span></span>](https://partner.microsoft.com/asset/collection/cloud-solution-provider-direct-partner-incentive-resources#/)
- [<span data-ttu-id="ee09b-339">Molnlösningsleverantör incitamentresurser för indirekta leverantörer</span><span class="sxs-lookup"><span data-stu-id="ee09b-339">Cloud Solution Provider indirect provider incentive resources</span></span>](https://partner.microsoft.com/asset/collection/cloud-solution-provider-indirect-provider-incentive-resources#/)
- <span data-ttu-id="ee09b-340">Läs den här [presentationen](https://partner.microsoft.com/resources/detail/partner-center-cm-for-csp-overview-pdf) om du vill veta mer om att sälja appar på den kommersiella marknadsplatsen.</span><span class="sxs-lookup"><span data-stu-id="ee09b-340">Review this [presentation](https://partner.microsoft.com/resources/detail/partner-center-cm-for-csp-overview-pdf) to learn more about selling the commercial marketplace apps.</span></span> <span data-ttu-id="ee09b-341">Kolla in ytterligare resurser [här.](https://partner.microsoft.com/resources/collection/partner-center-cm-for-csp-collection#/)</span><span class="sxs-lookup"><span data-stu-id="ee09b-341">Check out additional resources [here](https://partner.microsoft.com/resources/collection/partner-center-cm-for-csp-collection#/).</span></span> 
- <span data-ttu-id="ee09b-342">Utforska katalogen för den kommersiella marknadsplatsen [i Partnercenter](https://docs.microsoft.com/partner-center/csp-commercial-marketplace-discover) [eller Azure Portal](https://ms.portal.azure.com/#home)</span><span class="sxs-lookup"><span data-stu-id="ee09b-342">Explore the commercial marketplace catalog in [Partner Center](https://docs.microsoft.com/partner-center/csp-commercial-marketplace-discover) or [Azure portal](https://ms.portal.azure.com/#home)</span></span>
- <span data-ttu-id="ee09b-343">Använda [API:er](https://docs.microsoft.com/partner-center/develop/create-subscription-azure-marketplace-products#get-a-list-of-offers-for-a-market) för att integrera appar på företagets marknadsplats</span><span class="sxs-lookup"><span data-stu-id="ee09b-343">Use [APIs](https://docs.microsoft.com/partner-center/develop/create-subscription-azure-marketplace-products#get-a-list-of-offers-for-a-market) to integrate apps into your company’s marketplace</span></span>
- <span data-ttu-id="ee09b-344">Kontakta ISV:er som du är intresserad av att göra affärer med</span><span class="sxs-lookup"><span data-stu-id="ee09b-344">Reach out to ISVs you are interested in doing business with</span></span>
- <span data-ttu-id="ee09b-345">Indirekta leverantörer måste integrera med hjälp av API:er och vägleda återförsäljare om vilka appar som ska säljas</span><span class="sxs-lookup"><span data-stu-id="ee09b-345">Indirect providers need to integrate using APIs and guide resellers on which apps to sell</span></span>

### <a name="questions"></a><span data-ttu-id="ee09b-346">Har du några frågor?</span><span class="sxs-lookup"><span data-stu-id="ee09b-346">Questions?</span></span>  

<span data-ttu-id="ee09b-347">I den [här artikeln](https://docs.microsoft.com/partner-center/csp-commercial-marketplace-overview) finns en översikt över den kommersiella marknadsplatsen i Partnercenter.</span><span class="sxs-lookup"><span data-stu-id="ee09b-347">Refer to [this article](https://docs.microsoft.com/partner-center/csp-commercial-marketplace-overview) for an overview of the commercial marketplace in Partner Center.</span></span>

<span data-ttu-id="ee09b-348">Om du behöver ytterligare hjälp kan du skapa en supportbegäran i Partnercenter.</span><span class="sxs-lookup"><span data-stu-id="ee09b-348">If you need additional assistance you can create a support request in Partner Center.</span></span> <span data-ttu-id="ee09b-349">Läs mer på [https://aka.ms/IncentivesSupport](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=1) .</span><span class="sxs-lookup"><span data-stu-id="ee09b-349">Learn more at [https://aka.ms/IncentivesSupport](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=1).</span></span>

________________
## <a name="power-bi-premium-offer-naming-and-prerequisite-update"></a><a name="11"></a><span data-ttu-id="ee09b-350">Power BI Premium för namn och kravuppdatering</span><span class="sxs-lookup"><span data-stu-id="ee09b-350">Power BI Premium offer naming and prerequisite update</span></span>

### <a name="categories"></a><span data-ttu-id="ee09b-351">Kategorier</span><span class="sxs-lookup"><span data-stu-id="ee09b-351">Categories</span></span>

- <span data-ttu-id="ee09b-352">Datum: 2021-03-18</span><span class="sxs-lookup"><span data-stu-id="ee09b-352">Date: 2021-03-18</span></span>
- <span data-ttu-id="ee09b-353">Funktioner</span><span class="sxs-lookup"><span data-stu-id="ee09b-353">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="ee09b-354">Sammanfattning</span><span class="sxs-lookup"><span data-stu-id="ee09b-354">Summary</span></span>

<span data-ttu-id="ee09b-355">Den slutliga prislistan för den 1 april 2021 uppdateras för att förtydliga namngivnings- och/eller kravinformationen för erbjudanden Power BI Premium per användare.</span><span class="sxs-lookup"><span data-stu-id="ee09b-355">The April 1, 2021 final price list will be updated to add clarity to the naming and/or prerequisite information for Power BI Premium Per User offers.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="ee09b-356">Påverkad målgrupp</span><span class="sxs-lookup"><span data-stu-id="ee09b-356">Impacted audience</span></span>

<span data-ttu-id="ee09b-357">Molnlösningsleverantör (CSP) direkta och indirekta partner</span><span class="sxs-lookup"><span data-stu-id="ee09b-357">Cloud Solution Provider (CSP) direct and indirect partners</span></span>

### <a name="details"></a><span data-ttu-id="ee09b-358">Information</span><span class="sxs-lookup"><span data-stu-id="ee09b-358">Details</span></span>

<span data-ttu-id="ee09b-359">Den slutliga prislistan för den 1 april 2021 uppdateras för att förtydliga namngivnings- och/eller kravinformationen för de Power BI Premium per användare.</span><span class="sxs-lookup"><span data-stu-id="ee09b-359">The April 1, 2021 final price list will be updated to add clarity to the naming and/or prerequisite information for Power BI Premium Per User offers.</span></span>

<span data-ttu-id="ee09b-360">Tills den slutliga prislistan har uppdaterats använder du informationen i det här avsnittet för att säkerställa att rätt produkt har beställts.</span><span class="sxs-lookup"><span data-stu-id="ee09b-360">Until the final price list is updated, use the information in this section to ensure that the correct product is ordered.</span></span>

<span data-ttu-id="ee09b-361">Följande information visar den berörda SKU:n och kravinformation.</span><span class="sxs-lookup"><span data-stu-id="ee09b-361">The following details show the affected SKU and prerequisite details.</span></span>

| <span data-ttu-id="ee09b-362">Erbjudandevisningsnamn den 1 mars – förhandsversion av prislista</span><span class="sxs-lookup"><span data-stu-id="ee09b-362">Offer display name on March 1 price list preview</span></span> |  <span data-ttu-id="ee09b-363">Uppdaterad erbjudandevisningsnamn den 1 april slutprislista</span><span class="sxs-lookup"><span data-stu-id="ee09b-363">Updated offer display name on April 1 final price list</span></span>| <span data-ttu-id="ee09b-364">Erbjudande-ID</span><span class="sxs-lookup"><span data-stu-id="ee09b-364">Offer ID</span></span> |
| ------ | ----------- | ----------- |
| <span data-ttu-id="ee09b-365">Power BI Premium per användare Add-On (prissättning för ideell personal)</span><span class="sxs-lookup"><span data-stu-id="ee09b-365">Power BI Premium Per User Add-On (Nonprofit Staff Pricing)</span></span>  |  <span data-ttu-id="ee09b-366">Power BI Premium per Add-On **(Office)** (prissättning för ideell personal)</span><span class="sxs-lookup"><span data-stu-id="ee09b-366">Power BI Premium Per User Add-On **(Office)** (Nonprofit Staff Pricing)</span></span>   | <span data-ttu-id="ee09b-367">31c03289-47ab-4ab0-8df1-03742c127ac6</span><span class="sxs-lookup"><span data-stu-id="ee09b-367">31c03289-47ab-4ab0-8df1-03742c127ac6</span></span>   |

<span data-ttu-id="ee09b-368">Kunder måste ha något av följande förhandskrav för att köpa det här erbjudandet:</span><span class="sxs-lookup"><span data-stu-id="ee09b-368">Customers are required to have any one of the following prerequisites to purchase this offer:</span></span>

| <span data-ttu-id="ee09b-369">Erbjudandets visningsnamn</span><span class="sxs-lookup"><span data-stu-id="ee09b-369">Offer display name</span></span> | <span data-ttu-id="ee09b-370">Erbjudande-ID</span><span class="sxs-lookup"><span data-stu-id="ee09b-370">Offer ID</span></span> |
| ------ | ----------- |
| <span data-ttu-id="ee09b-371">Microsoft 365 E5 (prissättning för ideell personal)</span><span class="sxs-lookup"><span data-stu-id="ee09b-371">Microsoft 365 E5 (Nonprofit Staff Pricing)</span></span>  |  <span data-ttu-id="ee09b-372">31bedf01-9e57-4ece-a53a-d3656a563931</span><span class="sxs-lookup"><span data-stu-id="ee09b-372">31bedf01-9e57-4ece-a53a-d3656a563931</span></span>   |
|   <span data-ttu-id="ee09b-373">Microsoft 365 E5 utan ljudkonferens (prissättning för ideell personal)</span><span class="sxs-lookup"><span data-stu-id="ee09b-373">Microsoft 365 E5 without Audio Conferencing (Nonprofit Staff Pricing)</span></span>|  <span data-ttu-id="ee09b-374">b456810a-c414-4e07-98fc-ef74e8175a09</span><span class="sxs-lookup"><span data-stu-id="ee09b-374">b456810a-c414-4e07-98fc-ef74e8175a09</span></span>|
|   <span data-ttu-id="ee09b-375">Office 365 E5 (prissättning för ideell personal)</span><span class="sxs-lookup"><span data-stu-id="ee09b-375">Office 365 E5 (Nonprofit Staff Pricing)</span></span>| <span data-ttu-id="ee09b-376">ce139fe5-8bd5-47ed-a5be-07c286f8b9e</span><span class="sxs-lookup"><span data-stu-id="ee09b-376">ce139fe5-8bd5-47ed-a5be-07c286f8b9e</span></span>    |
|   <span data-ttu-id="ee09b-377">Utvärderingsversion av Office 365 E5 (prissättning för ideell personal)</span><span class="sxs-lookup"><span data-stu-id="ee09b-377">Office 365 E5 (Nonprofit Staff Pricing) Trial</span></span>|  <span data-ttu-id="ee09b-378">2f192efe-608a-4c9c-9d19-2b0b70b0962e</span><span class="sxs-lookup"><span data-stu-id="ee09b-378">2f192efe-608a-4c9c-9d19-2b0b70b0962e</span></span>|
|   <span data-ttu-id="ee09b-379">Office 365 E5 utan ljudkonferens (prissättning för ideell personal)</span><span class="sxs-lookup"><span data-stu-id="ee09b-379">Office 365 E5 without Audio Conferencing (Nonprofit Staff Pricing)</span></span>|  <span data-ttu-id="ee09b-380">c3897426-9f49-4eaf-9b4d-7d9a1c72aef7</span><span class="sxs-lookup"><span data-stu-id="ee09b-380">c3897426-9f49-4eaf-9b4d-7d9a1c72aef7</span></span>|

<span data-ttu-id="ee09b-381">Följande erbjudande Power BI Premium ett förhandskrav för inköp:</span><span class="sxs-lookup"><span data-stu-id="ee09b-381">The following Power BI Premium offer has a prerequisite required for purchase:</span></span>

| <span data-ttu-id="ee09b-382">Erbjudandets visningsnamn</span><span class="sxs-lookup"><span data-stu-id="ee09b-382">Offer display name</span></span> | <span data-ttu-id="ee09b-383">Erbjudande-ID</span><span class="sxs-lookup"><span data-stu-id="ee09b-383">Offer ID</span></span> |
| ------ | ----------- |
|   <span data-ttu-id="ee09b-384">Power BI Premium per Add-On (prissättning för ideell personal)</span><span class="sxs-lookup"><span data-stu-id="ee09b-384">Power BI Premium Per User Add-On (Nonprofit Staff Pricing)</span></span>|  <span data-ttu-id="ee09b-385">ef0b895b-681b-4026-a5b1-dda182a57d40</span><span class="sxs-lookup"><span data-stu-id="ee09b-385">ef0b895b-681b-4026-a5b1-dda182a57d40</span></span> |

<span data-ttu-id="ee09b-386">Kunder måste ha detta förhandskrav för att kunna köpa det här erbjudandet:</span><span class="sxs-lookup"><span data-stu-id="ee09b-386">Customers are required to have this prerequisite to purchase this offer:</span></span>

| <span data-ttu-id="ee09b-387">Erbjudandets visningsnamn</span><span class="sxs-lookup"><span data-stu-id="ee09b-387">Offer display name</span></span> | <span data-ttu-id="ee09b-388">Erbjudande-ID</span><span class="sxs-lookup"><span data-stu-id="ee09b-388">Offer ID</span></span> |
| ------ |----------|
| <span data-ttu-id="ee09b-389">Power BI Pro (prissättning för ideell personal)</span><span class="sxs-lookup"><span data-stu-id="ee09b-389">Power BI Pro (Nonprofit Staff Pricing)</span></span>  |   <span data-ttu-id="ee09b-390">cabdfc93-5786-4224-bfd3-35d58f833b35</span><span class="sxs-lookup"><span data-stu-id="ee09b-390">cabdfc93-5786-4224-bfd3-35d58f833b35</span></span> |

### <a name="next-steps"></a><span data-ttu-id="ee09b-391">Nästa steg</span><span class="sxs-lookup"><span data-stu-id="ee09b-391">Next steps</span></span>

<span data-ttu-id="ee09b-392">Granska resurserna om det här avsnittet och dela den här informationen med lämpliga intressenter i din organisation.</span><span class="sxs-lookup"><span data-stu-id="ee09b-392">Review the resources about this topic, and share this information with the appropriate stakeholders in your organization.</span></span>  

### <a name="questions"></a><span data-ttu-id="ee09b-393">Har du några frågor?</span><span class="sxs-lookup"><span data-stu-id="ee09b-393">Questions?</span></span>

<span data-ttu-id="ee09b-394">Om du har frågor om dessa erbjudanden kan du kontrollera dina relevanta Yammer-communities.</span><span class="sxs-lookup"><span data-stu-id="ee09b-394">For any questions about these offers, check your relevant Yammer communities.</span></span> 

## <a name="march-price-updates-for-microsoft-365-f3"></a><a name="10"></a> <span data-ttu-id="ee09b-395">Prisuppdateringar mars för Microsoft 365 F3</span><span class="sxs-lookup"><span data-stu-id="ee09b-395">March price updates for Microsoft 365 F3</span></span>

### <a name="categories"></a><span data-ttu-id="ee09b-396">Kategorier</span><span class="sxs-lookup"><span data-stu-id="ee09b-396">Categories</span></span>

- <span data-ttu-id="ee09b-397">Datum: 2021-03-16</span><span class="sxs-lookup"><span data-stu-id="ee09b-397">Date: 2021-03-16</span></span>
- <span data-ttu-id="ee09b-398">Erbjudanden/marknader</span><span class="sxs-lookup"><span data-stu-id="ee09b-398">Offers/Markets</span></span>

### <a name="summary"></a><span data-ttu-id="ee09b-399">Sammanfattning</span><span class="sxs-lookup"><span data-stu-id="ee09b-399">Summary</span></span>

<span data-ttu-id="ee09b-400">Felaktig prissättning för mars 2021 har korrigerats för Microsoft 365 F3 British Pound (GBP) och EURO (EUR).</span><span class="sxs-lookup"><span data-stu-id="ee09b-400">Incorrect March 2021 pricing has been corrected for Microsoft 365 F3 British Pound (GBP) and Euro (EUR).</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="ee09b-401">Målgrupp som påverkas</span><span class="sxs-lookup"><span data-stu-id="ee09b-401">Impacted audience</span></span>

<span data-ttu-id="ee09b-402">Partner som köper Microsoft 365 F3 i Gbit/s eller EUR mellan 1 mars och 17 mars 2021 via programmet Molnlösningsleverantör (CSP).</span><span class="sxs-lookup"><span data-stu-id="ee09b-402">Partners purchasing Microsoft 365 F3 in GBP or EUR between March 1 and March 17, 2021 through the Cloud Solution Provider (CSP) program.</span></span>

### <a name="details"></a><span data-ttu-id="ee09b-403">Information</span><span class="sxs-lookup"><span data-stu-id="ee09b-403">Details</span></span>

<span data-ttu-id="ee09b-404">Microsoft har löst felaktig prissättning för Microsoft 365 F3.</span><span class="sxs-lookup"><span data-stu-id="ee09b-404">Microsoft has resolved incorrect pricing for Microsoft 365 F3.</span></span> <span data-ttu-id="ee09b-405">De felaktiga priserna var för GBP och EUR och endast för erbjudanden som köpts mellan 1 mars och 17 mars 2021.</span><span class="sxs-lookup"><span data-stu-id="ee09b-405">The incorrect prices were for GBP and EUR and only for offers purchased between March 1 and March 17, 2021.</span></span> <span data-ttu-id="ee09b-406">De erbjudanden och valutor som påverkas visas nedan.</span><span class="sxs-lookup"><span data-stu-id="ee09b-406">The impacted offers and currencies are listed below.</span></span> 

| <span data-ttu-id="ee09b-407">Erbjudandets namn</span><span class="sxs-lookup"><span data-stu-id="ee09b-407">Offer name</span></span> | <span data-ttu-id="ee09b-408">Valuta</span><span class="sxs-lookup"><span data-stu-id="ee09b-408">Currency</span></span> | <span data-ttu-id="ee09b-409">Erbjudande-ID</span><span class="sxs-lookup"><span data-stu-id="ee09b-409">Offer ID</span></span> | <span data-ttu-id="ee09b-410">Material-ID</span><span class="sxs-lookup"><span data-stu-id="ee09b-410">Material ID</span></span> |
| ------ |----------- |----------- |----------- |
| <span data-ttu-id="ee09b-411">Microsoft 365 F3 (Fc)</span><span class="sxs-lookup"><span data-stu-id="ee09b-411">Microsoft 365 F3 (Charity)</span></span> | <span data-ttu-id="ee09b-412">GBP</span><span class="sxs-lookup"><span data-stu-id="ee09b-412">GBP</span></span> | <span data-ttu-id="ee09b-413">57b722c2-c435-4bfb-9bc8-80509213a13a</span><span class="sxs-lookup"><span data-stu-id="ee09b-413">57b722c2-c435-4bfb-9bc8-80509213a13a</span></span> | <span data-ttu-id="ee09b-414">AAD-11626</span><span class="sxs-lookup"><span data-stu-id="ee09b-414">AAD-11626</span></span> |
| <span data-ttu-id="ee09b-415">Microsoft 365 F3 (kommersiell)</span><span class="sxs-lookup"><span data-stu-id="ee09b-415">Microsoft 365 F3 (Commercial)</span></span> | <span data-ttu-id="ee09b-416">EUR</span><span class="sxs-lookup"><span data-stu-id="ee09b-416">EUR</span></span>| <span data-ttu-id="ee09b-417">3451a3b0-8cda-44a7-bad7-c30be81c4aaa</span><span class="sxs-lookup"><span data-stu-id="ee09b-417">3451a3b0-8cda-44a7-bad7-c30be81c4aaa</span></span> | <span data-ttu-id="ee09b-418">AAA-89898</span><span class="sxs-lookup"><span data-stu-id="ee09b-418">AAA-89898</span></span> |
 
<span data-ttu-id="ee09b-419">Prislistorna för licensbas för mars och april uppdaterades 16 mars 17:00 Pacific Standard Time.</span><span class="sxs-lookup"><span data-stu-id="ee09b-419">The March and April preview license-base price lists were updated March 16, 5PM pacific standard time.</span></span>

### <a name="next-steps"></a><span data-ttu-id="ee09b-420">Nästa steg</span><span class="sxs-lookup"><span data-stu-id="ee09b-420">Next steps</span></span>

- <span data-ttu-id="ee09b-421">Partner bör ladda ned de aktuella licensbaserade prislistorna på nytt, både mars och aprilförhandsvisningen, med dessa priskorrigeringar om tillämpligt.</span><span class="sxs-lookup"><span data-stu-id="ee09b-421">Partners should redownload the current license-based price lists, both March and the April preview, with these price corrections if applicable.</span></span>  
- <span data-ttu-id="ee09b-422">Microsoft kommer att kontakta berörda partner under de kommande veckorna via e-post för att informera dem om nästa steg som rör korrigering av berörda transaktioner.</span><span class="sxs-lookup"><span data-stu-id="ee09b-422">Microsoft will be contacting impacted partners in the coming weeks via email to inform them of next steps related to correcting affected transactions.</span></span>

### <a name="questions"></a><span data-ttu-id="ee09b-423">Har du några frågor?</span><span class="sxs-lookup"><span data-stu-id="ee09b-423">Questions?</span></span>

<span data-ttu-id="ee09b-424">Om du har fler frågor kan du kontrollera dina relevanta CSP Yammer-communities.</span><span class="sxs-lookup"><span data-stu-id="ee09b-424">For any further questions please check your relevant CSP Yammer communities.</span></span>

________________

## <a name="update-a-legal-company-name-through-partner-center"></a><a name="9"></a> <span data-ttu-id="ee09b-425">Uppdatera ett juridiskt företagsnamn via Partnercenter</span><span class="sxs-lookup"><span data-stu-id="ee09b-425">Update a legal company name through Partner Center</span></span>

### <a name="categories"></a><span data-ttu-id="ee09b-426">Kategorier</span><span class="sxs-lookup"><span data-stu-id="ee09b-426">Categories</span></span>

- <span data-ttu-id="ee09b-427">Datum: 2021-03-16</span><span class="sxs-lookup"><span data-stu-id="ee09b-427">Date: 2021-03-16</span></span>
- <span data-ttu-id="ee09b-428">Skala för & effektivitet</span><span class="sxs-lookup"><span data-stu-id="ee09b-428">Drive Efficiency & Scale</span></span>

### <a name="summary"></a><span data-ttu-id="ee09b-429">Sammanfattning</span><span class="sxs-lookup"><span data-stu-id="ee09b-429">Summary</span></span>

<span data-ttu-id="ee09b-430">Från och med mars 2021 kan Microsoft Partner Network-partner (MPN) och indirekta Molnlösningsleverantör CSP-återförsäljare (CSP) uppdatera sina juridiska företagsnamn via Partnercenter.</span><span class="sxs-lookup"><span data-stu-id="ee09b-430">Starting March 2021, Microsoft Partner Network (MPN) partners and Cloud Solution Provider (CSP) indirect resellers can update their legal company name through Partner Center.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="ee09b-431">Påverkad målgrupp</span><span class="sxs-lookup"><span data-stu-id="ee09b-431">Impacted audience</span></span>

<span data-ttu-id="ee09b-432">MPN-partner och indirekta CSP-återförsäljare (gäller inte CSP-direktfaktureringspartner)</span><span class="sxs-lookup"><span data-stu-id="ee09b-432">MPN partners and CSP indirect resellers (not applicable to CSP direct bill partners)</span></span>

### <a name="details"></a><span data-ttu-id="ee09b-433">Information</span><span class="sxs-lookup"><span data-stu-id="ee09b-433">Details</span></span>

<span data-ttu-id="ee09b-434">Från och med mars 2021 kan MPN-partner och indirekta CSP-återförsäljare uppdatera sitt juridiska företagsnamn via Partnercenter på ett kompatibelt sätt med självbetjäning.</span><span class="sxs-lookup"><span data-stu-id="ee09b-434">Starting March 2021, MPN partners and CSP indirect resellers can update their legal company name through Partner Center in a compliant, self-serve manner.</span></span> <span data-ttu-id="ee09b-435">Med den här nya funktionen behöver partner inte längre skicka en supportbiljett till Partnercenter för att uppdatera företagets namn.</span><span class="sxs-lookup"><span data-stu-id="ee09b-435">With this new feature, partners will no longer need to submit a Partner Center support ticket to update their company name.</span></span> <span data-ttu-id="ee09b-436">Detta sparar mycket tid för partner när de utför dessa aktiviteter.</span><span class="sxs-lookup"><span data-stu-id="ee09b-436">This will save a significant amount of time for partners when performing these activities.</span></span> 

<span data-ttu-id="ee09b-437">Mer information finns i [Uppdatera din juridiska företagsprofil.](../update-your-partner-profile.md#update-your-legal-business-profile)</span><span class="sxs-lookup"><span data-stu-id="ee09b-437">To learn more, see [Update your legal business profile](../update-your-partner-profile.md#update-your-legal-business-profile).</span></span>

>[!NOTE]
><span data-ttu-id="ee09b-438">Se till att företagets namn i din juridiska företagsprofil inte innehåller stavfel och förkortningar och exakt matchar företagets formella registreringsposter för företag.</span><span class="sxs-lookup"><span data-stu-id="ee09b-438">Ensure that the company name in your legal business profile is free of spelling errors and abbreviations, and exactly matches your formal company business registration records.</span></span> <span data-ttu-id="ee09b-439">Mer information om hur du uppdaterar din organisationsprofil finns i [Verifiera din organisationsprofil.](../update-your-partner-profile.md#update-your-legal-business-profile)</span><span class="sxs-lookup"><span data-stu-id="ee09b-439">For more information on updating your organization profile, refer to [Verify your organization profile](../update-your-partner-profile.md#update-your-legal-business-profile).</span></span>

### <a name="next-steps"></a><span data-ttu-id="ee09b-440">Nästa steg</span><span class="sxs-lookup"><span data-stu-id="ee09b-440">Next steps</span></span>

<span data-ttu-id="ee09b-441">Dela den här informationen i din organisation så att rätt team kan granska och uppdatera sina processer.</span><span class="sxs-lookup"><span data-stu-id="ee09b-441">Share this information within your organization so that the appropriate team can review and update their processes.</span></span>

### <a name="questions"></a><span data-ttu-id="ee09b-442">Har du några frågor?</span><span class="sxs-lookup"><span data-stu-id="ee09b-442">Questions?</span></span>

<span data-ttu-id="ee09b-443">Om du har fler frågor kan du kontrollera dina relevanta CSP Yammer-communities.</span><span class="sxs-lookup"><span data-stu-id="ee09b-443">For any further questions please check your relevant CSP Yammer communities.</span></span>

________________
## <a name="update-to-cloud-solution-provider-csp-program-evolution-and-open-license-program-changes"></a><a name="8"></a> <span data-ttu-id="ee09b-444">Uppdatera till Molnlösningsleverantör programutveckling (CSP) och ändringar i Open License-programmet</span><span class="sxs-lookup"><span data-stu-id="ee09b-444">Update to Cloud Solution Provider (CSP) program evolution and Open License program changes</span></span>

### <a name="categories"></a><span data-ttu-id="ee09b-445">Kategorier</span><span class="sxs-lookup"><span data-stu-id="ee09b-445">Categories</span></span>

- <span data-ttu-id="ee09b-446">Datum: 2021-03-15</span><span class="sxs-lookup"><span data-stu-id="ee09b-446">Date: 2021-03-15</span></span>
- <span data-ttu-id="ee09b-447">Funktioner</span><span class="sxs-lookup"><span data-stu-id="ee09b-447">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="ee09b-448">Sammanfattning</span><span class="sxs-lookup"><span data-stu-id="ee09b-448">Summary</span></span>

<span data-ttu-id="ee09b-449">Nya kommersiella och offentliga programvaruerbjudanden kommer till CSP-programmet (Molnlösningsleverantör) tillsammans med ändringar i Open Licensing-programmet.</span><span class="sxs-lookup"><span data-stu-id="ee09b-449">New commercial and public sector perpetual software offers are coming to the Cloud Solution Provider (CSP) program along with changes to the Open Licensing program.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="ee09b-450">Målgrupp som påverkas</span><span class="sxs-lookup"><span data-stu-id="ee09b-450">Impacted audience</span></span>

<span data-ttu-id="ee09b-451">Kommersiella distributörer och hanterade återförsäljare som säljer via Open License-programmet, samt alla CSP-partner som handlar permanent programvara</span><span class="sxs-lookup"><span data-stu-id="ee09b-451">Commercial distributors and managed resellers selling through the Open License program, as well as all CSP partners transacting perpetual software</span></span>

### <a name="details"></a><span data-ttu-id="ee09b-452">Information</span><span class="sxs-lookup"><span data-stu-id="ee09b-452">Details</span></span>

<span data-ttu-id="ee09b-453">I september 2020 presenterade [Microsoft](https://blogs.partner.microsoft.com/mpn/expanding-opportunities-for-partners-in-the-cloud-solution-provider-program/) en serie steg i vår digitala omvandlingsresa för att utöka möjligheterna till partner i CSP-programmet, inklusive tillgängligheten för lokal programvara för partner.</span><span class="sxs-lookup"><span data-stu-id="ee09b-453">In September 2020, Microsoft [announced](https://blogs.partner.microsoft.com/mpn/expanding-opportunities-for-partners-in-the-cloud-solution-provider-program/) a series of steps in our digital transformation journey to expand opportunities to partners in the CSP program, including the availability of on-premises software for partners.</span></span> <span data-ttu-id="ee09b-454">Dessa ändringar gör det möjligt för partner att utöka sin verksamhet och sin räckvidd genom att utnyttja programvarulicenser i CSP och positionera dem för framgång i dagens molnbaserade värld.</span><span class="sxs-lookup"><span data-stu-id="ee09b-454">These changes enable partners to grow their business and extend their reach by leveraging software licenses in CSP, positioning them for success in today’s cloud-first world.</span></span> <span data-ttu-id="ee09b-455">De ger också kundernas övergångar till molnet och ger partner den flexibilitet som krävs för kundernas hybridmolnmiljöer.</span><span class="sxs-lookup"><span data-stu-id="ee09b-455">They also empower customers’ transitions to the cloud and give partners the flexibility needed for customer hybrid cloud environments.</span></span>

<span data-ttu-id="ee09b-456">I fortsättningen på den här digitala omvandlingen presenterar vi följande ändringar:</span><span class="sxs-lookup"><span data-stu-id="ee09b-456">In continuation of this digital transformation, we are announcing the following changes:</span></span>

- <span data-ttu-id="ee09b-457">1 juli 2021: Inga nya SKU:er, produkter eller kampanjer kommer att läggas till i prislistan för Open License-programmet.</span><span class="sxs-lookup"><span data-stu-id="ee09b-457">July 1, 2021:  No new SKUs, products, or promotions will be added to the Open License program price list.</span></span>

- <span data-ttu-id="ee09b-458">7 juli 2021: Två kommersiella erbjudanden, Get Genuine Windows och Visual Studio Professional, och erbjudanden inom den offentliga sektorn (myndigheter, utbildning och ideella organisationer – se [meddelande)](./2020-december.md#9)kommer att läggas till i CSP:s löpande prislista för programvara.</span><span class="sxs-lookup"><span data-stu-id="ee09b-458">July 7, 2021:  Two commercial offers, Get Genuine Windows and Visual Studio Professional, and public sector offers (government, education and nonprofit – see [announcement](./2020-december.md#9)) will be added to the CSP perpetual software price list.</span></span>  <span data-ttu-id="ee09b-459">Prislistan finns i avsnittet Programvara på sidan [Säljpriser >](https://partnercenter.microsoft.com/pcv/sales) & i Partnercenter och publiceras på nytt det här datumet.</span><span class="sxs-lookup"><span data-stu-id="ee09b-459">The price list can be found in the Software section of the [Sell > Pricing & Offers](https://partnercenter.microsoft.com/pcv/sales) page in Partner Center and will be republished on this date.</span></span>

<span data-ttu-id="ee09b-460">Fullständig information om CSP-programutvecklingen och ändringar i Open License-programmet finns i **Nästa steg** nedan.</span><span class="sxs-lookup"><span data-stu-id="ee09b-460">For full details regarding the CSP program evolution and Open License program changes, please see **Next Steps** below.</span></span>

### <a name="next-steps"></a><span data-ttu-id="ee09b-461">Nästa steg:</span><span class="sxs-lookup"><span data-stu-id="ee09b-461">Next Steps:</span></span>

- <span data-ttu-id="ee09b-462">Utveckling av CSP-program: Granska den beständiga [programvaran i Molnlösningsleverantör för programberedskap.](https://partner.microsoft.com/resources/collection/software-in-csp#/)</span><span class="sxs-lookup"><span data-stu-id="ee09b-462">CSP Program evolution:  Review the [Perpetual software in the Cloud Solution Provider program](https://partner.microsoft.com/resources/collection/software-in-csp#/) readiness materials.</span></span> <span data-ttu-id="ee09b-463">Använd [beredskapskartan](https://partner.microsoft.com/resources/detail/software-in-csp-readiness-map-pdf) för att snabbt hitta rätt information för din roll.</span><span class="sxs-lookup"><span data-stu-id="ee09b-463">Use this [readiness map](https://partner.microsoft.com/resources/detail/software-in-csp-readiness-map-pdf) to quickly locate the right information for your role.</span></span>

- <span data-ttu-id="ee09b-464">Öppna Ändringar av licensprogram: Granska [CSP-programutvecklingen och Ändra](https://partner.microsoft.com/resources/collection/csp-open-evolution-to-a-better-experience#/) beredskapsmaterial för Open License Program.</span><span class="sxs-lookup"><span data-stu-id="ee09b-464">Open License program changes:  Review the [CSP program evolution and Open License program changes](https://partner.microsoft.com/resources/collection/csp-open-evolution-to-a-better-experience#/) readiness materials.</span></span> <span data-ttu-id="ee09b-465">Använd [beredskapskartan](https://partner.microsoft.com/resources/detail/csp-open-evolution-to-a-better-experience-readiness-map-pdf) för att snabbt hitta rätt information för din roll.</span><span class="sxs-lookup"><span data-stu-id="ee09b-465">Use this [readiness map](https://partner.microsoft.com/resources/detail/csp-open-evolution-to-a-better-experience-readiness-map-pdf) to quickly locate the right information for your role.</span></span>

### <a name="questions"></a><span data-ttu-id="ee09b-466">Frågor</span><span class="sxs-lookup"><span data-stu-id="ee09b-466">Questions</span></span>

<span data-ttu-id="ee09b-467">Om du har fler frågor kan du kontrollera dina relevanta CSP Yammer-communities.</span><span class="sxs-lookup"><span data-stu-id="ee09b-467">For any further questions please check your relevant CSP Yammer communities.</span></span>

_______________
## <a name="update-to-a-previous-announcement-premium-assessments-an-add-on-to-compliance-manager"></a><a name="7"></a><span data-ttu-id="ee09b-468">Uppdatera till ett tidigare meddelande: Premium Assessments, ett tillägg till Compliance Manager</span><span class="sxs-lookup"><span data-stu-id="ee09b-468">Update to a previous announcement: Premium Assessments, an add-on to Compliance Manager</span></span>

### <a name="categories"></a><span data-ttu-id="ee09b-469">Kategorier</span><span class="sxs-lookup"><span data-stu-id="ee09b-469">Categories</span></span>

- <span data-ttu-id="ee09b-470">Datum: 2021-03-15</span><span class="sxs-lookup"><span data-stu-id="ee09b-470">Date: 2021-03-15</span></span>
- <span data-ttu-id="ee09b-471">Utveckla verksamheten</span><span class="sxs-lookup"><span data-stu-id="ee09b-471">Grow your business</span></span>

### <a name="summary"></a><span data-ttu-id="ee09b-472">Sammanfattning</span><span class="sxs-lookup"><span data-stu-id="ee09b-472">Summary</span></span>

<span data-ttu-id="ee09b-473">Utvärderingserbjudandena bör inte ha listats i prislistan och tas bort.</span><span class="sxs-lookup"><span data-stu-id="ee09b-473">The trial offers shouldn’t have been listed on the price list and will be removed.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="ee09b-474">Målgrupp som påverkas</span><span class="sxs-lookup"><span data-stu-id="ee09b-474">Impacted audience</span></span>

<span data-ttu-id="ee09b-475">Partner som gör en Molnlösningsleverantör</span><span class="sxs-lookup"><span data-stu-id="ee09b-475">Partners transacting through Cloud Solution Provider</span></span>

### <a name="details"></a><span data-ttu-id="ee09b-476">Information</span><span class="sxs-lookup"><span data-stu-id="ee09b-476">Details</span></span>

<span data-ttu-id="ee09b-477">Utvärderingserbjudandena bör inte ha inkluderats i prislistan.</span><span class="sxs-lookup"><span data-stu-id="ee09b-477">The trial offers shouldn’t have been included in the price list.</span></span> <span data-ttu-id="ee09b-478">Dessa tas bort från prislistan 1 maj 2021.</span><span class="sxs-lookup"><span data-stu-id="ee09b-478">These will be removed from the May 1, 2021 price list.</span></span>

<span data-ttu-id="ee09b-479">Det ursprungliga meddelandet finns [här.](./2021-february.md#4)</span><span class="sxs-lookup"><span data-stu-id="ee09b-479">The original announcement is [here](./2021-february.md#4).</span></span>

### <a name="additional-resources"></a><span data-ttu-id="ee09b-480">Ytterligare resurser</span><span class="sxs-lookup"><span data-stu-id="ee09b-480">Additional resources</span></span>

- [<span data-ttu-id="ee09b-481">Microsoft 365 säkerhet och efterlevnad för E5</span><span class="sxs-lookup"><span data-stu-id="ee09b-481">Microsoft 365 E5 security and compliance</span></span>](https://www.microsoft.com/licensing/product-licensing/microsoft-365-enterprise?activetab=m365-enterprise:primaryr5)

- [<span data-ttu-id="ee09b-482">Skapa och hantera utvärderingar i Microsoft Compliance Manager – Microsoft 365 efterlevnad</span><span class="sxs-lookup"><span data-stu-id="ee09b-482">Build and manage assessments in Microsoft Compliance Manager - Microsoft 365 Compliance</span></span>](/microsoft-365/compliance/compliance-manager-assessments)

### <a name="next-steps"></a><span data-ttu-id="ee09b-483">Nästa steg</span><span class="sxs-lookup"><span data-stu-id="ee09b-483">Next steps</span></span>

<span data-ttu-id="ee09b-484">Granska resurserna om det här avsnittet och dela den här informationen med lämpliga intressenter i din organisation.</span><span class="sxs-lookup"><span data-stu-id="ee09b-484">Review the resources about this topic, and share this information with the appropriate stakeholders in your organization.</span></span>

### <a name="questions"></a><span data-ttu-id="ee09b-485">Har du några frågor?</span><span class="sxs-lookup"><span data-stu-id="ee09b-485">Questions?</span></span>

<span data-ttu-id="ee09b-486">Frågor om dessa erbjudanden finns i dina relevanta Yammer-communities.</span><span class="sxs-lookup"><span data-stu-id="ee09b-486">For questions about these offers, check your relevant Yammer communities.</span></span>

________________
## <a name="migrate-your-solutions-from-one-commercial-partner-ocp-go-to-market-gtm-to-the-microsoft-commercial-marketplace"></a><a name="6"></a> <span data-ttu-id="ee09b-487">Migrera dina lösningar från EN kommersiell partner (OCP) till Microsofts kommersiella marknadsplats</span><span class="sxs-lookup"><span data-stu-id="ee09b-487">Migrate your solutions from One Commercial Partner (OCP) go-to market (GTM) to the Microsoft commercial marketplace</span></span>

### <a name="categories"></a><span data-ttu-id="ee09b-488">Kategorier</span><span class="sxs-lookup"><span data-stu-id="ee09b-488">Categories</span></span>

- <span data-ttu-id="ee09b-489">Datum: 2021-03-12</span><span class="sxs-lookup"><span data-stu-id="ee09b-489">Date: 2021-03-12</span></span>
- <span data-ttu-id="ee09b-490">Funktioner</span><span class="sxs-lookup"><span data-stu-id="ee09b-490">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="ee09b-491">Sammanfattning</span><span class="sxs-lookup"><span data-stu-id="ee09b-491">Summary</span></span>

<span data-ttu-id="ee09b-492">Från och med 29 mars 2021 kommer du att få begränsade FUNKTIONER för EN kommersiell partner (OCP) på marknaden (GTM).</span><span class="sxs-lookup"><span data-stu-id="ee09b-492">From March 29, 2021, you will begin to experience limited One Commercial Partner (OCP) go-to market (GTM) capabilities.</span></span> <span data-ttu-id="ee09b-493">Vi rekommenderar att du migrerar dina lösningar till den kommersiella marknadsplatsen i Partnercenter.</span><span class="sxs-lookup"><span data-stu-id="ee09b-493">We encourage you to migrate your solutions to the commercial marketplace in Partner Center.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="ee09b-494">Påverkad målgrupp</span><span class="sxs-lookup"><span data-stu-id="ee09b-494">Impacted audience</span></span>

<span data-ttu-id="ee09b-495">Organisationer som samarbetar med lösningar i OCP GTM</span><span class="sxs-lookup"><span data-stu-id="ee09b-495">Organizations co-selling with solutions in OCP GTM</span></span>

### <a name="details"></a><span data-ttu-id="ee09b-496">Information</span><span class="sxs-lookup"><span data-stu-id="ee09b-496">Details</span></span>

<span data-ttu-id="ee09b-497">I december 2020 påbörjade vi vår resa från Verktyget Microsoft OCP GTM till Microsofts kommersiella marknadsplats i Partnercenter.</span><span class="sxs-lookup"><span data-stu-id="ee09b-497">In December 2020, we started our journey from the Microsoft OCP GTM tool to the Microsoft commercial marketplace in Partner Center.</span></span> <span data-ttu-id="ee09b-498">Den här övergången utökar funktionerna på den kommersiella marknadsplatsen där du kan demonstrera dina lösningar för miljontals kunder, dela affärsmöjligheter med andra Microsoft- och partnerförsäljningar och gemensamt sälja innovativa lösningar.</span><span class="sxs-lookup"><span data-stu-id="ee09b-498">This transition expands the capabilities of the commercial marketplace where you can showcase your solutions to millions of customers, bidirectionally share opportunities with other Microsoft and partner sellers, and jointly sell innovative solutions.</span></span>

<span data-ttu-id="ee09b-499">Nästa milstolpe i övergången sker den 29 mars 2021.</span><span class="sxs-lookup"><span data-stu-id="ee09b-499">The next milestone in the transition will take place on March 29, 2021.</span></span> <span data-ttu-id="ee09b-500">Det är då du börjar uppleva begränsade OCP GTM-funktioner, där vissa fält blir skrivskyddade.</span><span class="sxs-lookup"><span data-stu-id="ee09b-500">That’s when you’ll begin to experience limited OCP GTM capabilities, with some fields becoming read-only.</span></span> <span data-ttu-id="ee09b-501">Om du för närvarande samarbetar med lösningar i OCP GTM rekommenderar vi att du migrerar dina lösningar till den kommersiella marknadsplatsen för att dra nytta av dess funktioner och förenkla din publiceringsupplevelse.</span><span class="sxs-lookup"><span data-stu-id="ee09b-501">If you’re currently co-selling with solutions in OCP GTM, we encourage you to migrate your solutions to the commercial marketplace to take advantage of its capabilities and simplify your publishing experience.</span></span> 

<span data-ttu-id="ee09b-502">Att flytta till den kommersiella marknadsplatsen gör Partner Center till det primära målet för publiceringen av säljförsäljning.</span><span class="sxs-lookup"><span data-stu-id="ee09b-502">Moving to the commercial marketplace makes Partner Center the primary destination for the co-sell publishing experience.</span></span> <span data-ttu-id="ee09b-503">Det är här du kan fortsätta att utveckla din verksamhet genom att ansluta dina lösningar till våra delade kunder via samma kanaler och produktupplevelser som vi använder för Microsoft-produkter.</span><span class="sxs-lookup"><span data-stu-id="ee09b-503">It’s where you can continue to grow your business by connecting your solutions with our shared customers through the same channels and in-product experiences that we use for Microsoft products.</span></span> <span data-ttu-id="ee09b-504">[Läs mer om den kommersiella marknadsplatsen](https://blogs.partner.microsoft.com/mpn/getting-started-with-the-microsoft-commercial-marketplace/).</span><span class="sxs-lookup"><span data-stu-id="ee09b-504">[Learn more about the commercial marketplace](https://blogs.partner.microsoft.com/mpn/getting-started-with-the-microsoft-commercial-marketplace/).</span></span>

### <a name="next-steps"></a><span data-ttu-id="ee09b-505">Nästa steg</span><span class="sxs-lookup"><span data-stu-id="ee09b-505">Next steps</span></span>

- <span data-ttu-id="ee09b-506">Om du ännu inte har flyttat dina lösningar [](/azure/marketplace/co-sell-solution-migration) följer du anvisningarna i övergångsguiden eller visar den stegvisa videokursen för att slutföra alla [migreringsaktiviteter](https://partner.microsoft.com/asset/detail/ocp-gtm-to-the-microsoft-commercial-marketplace-mp4) och börja publicera dina lösningar på den kommersiella marknadsplatsen.</span><span class="sxs-lookup"><span data-stu-id="ee09b-506">If you have not yet moved your solutions, follow the instructions detailed in the [transition guide](/azure/marketplace/co-sell-solution-migration) or view the [step-by-step video tutorial](https://partner.microsoft.com/asset/detail/ocp-gtm-to-the-microsoft-commercial-marketplace-mp4) to complete all migration activities and start publishing your solution(s) in the commercial marketplace.</span></span>

- <span data-ttu-id="ee09b-507">Om du har frågor om den begränsade kapacitetsupplevelsen i OCP GTM kan du se krav på säljförsäljning för publicering på Microsofts kommersiella marknadsplats – vanliga [frågor och svar.](https://partner.microsoft.com/resources/detail/co-sell-requirements-publish-commercial-marketplace-faq-pdf)</span><span class="sxs-lookup"><span data-stu-id="ee09b-507">For questions regarding the limited capability experience in OCP GTM, view the [Co-sell requirements to publish in the Microsoft commercial marketplace FAQ](https://partner.microsoft.com/resources/detail/co-sell-requirements-publish-commercial-marketplace-faq-pdf).</span></span> <span data-ttu-id="ee09b-508">(Se avsnittet "OCP GTM-begränsade funktioner från och med 29 mars 2021.")</span><span class="sxs-lookup"><span data-stu-id="ee09b-508">(See the section “OCP GTM limited capabilities starting March 29, 2021.”)</span></span>

### <a name="questions"></a><span data-ttu-id="ee09b-509">Har du några frågor?</span><span class="sxs-lookup"><span data-stu-id="ee09b-509">Questions?</span></span>

<span data-ttu-id="ee09b-510">Kontakta [supporten](https://partner.microsoft.com/support/?stage=1) om du har frågor eller behöver mer information.</span><span class="sxs-lookup"><span data-stu-id="ee09b-510">Contact [Support](https://partner.microsoft.com/support/?stage=1) if you have any questions or need more information.</span></span>

________________
## <a name="expanding-the-new-commerce-experience-in-the-cloud-solution-provider-csp-program-for-azure-to-russia"></a><a name="5"></a><span data-ttu-id="ee09b-511">Utöka den nya handelsupplevelsen i programmet Molnlösningsleverantör (CSP) för Azure till Ryssland</span><span class="sxs-lookup"><span data-stu-id="ee09b-511">Expanding the new commerce experience in the Cloud Solution Provider (CSP) program for Azure to Russia</span></span>

### <a name="categories"></a><span data-ttu-id="ee09b-512">Kategorier</span><span class="sxs-lookup"><span data-stu-id="ee09b-512">Categories</span></span>

- <span data-ttu-id="ee09b-513">Datum: 2021-03-10</span><span class="sxs-lookup"><span data-stu-id="ee09b-513">Date: 2021-03-10</span></span>
- <span data-ttu-id="ee09b-514">Funktioner</span><span class="sxs-lookup"><span data-stu-id="ee09b-514">Capabilities</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="ee09b-515">Målgrupp som påverkas</span><span class="sxs-lookup"><span data-stu-id="ee09b-515">Impacted audience</span></span>

<span data-ttu-id="ee09b-516">Alla partner i Ryssland går igenom programmet Molnlösningsleverantör (CSP).</span><span class="sxs-lookup"><span data-stu-id="ee09b-516">All partners in Russia transacting through the Cloud Solution Provider (CSP) program.</span></span>

### <a name="details"></a><span data-ttu-id="ee09b-517">Information</span><span class="sxs-lookup"><span data-stu-id="ee09b-517">Details</span></span>

<span data-ttu-id="ee09b-518">Från och med 10 mars 2021 är vi glada över att kunna presentera tillgängligheten för den nya handelsupplevelsen i **CSP för Azure i Ryssland.**</span><span class="sxs-lookup"><span data-stu-id="ee09b-518">Starting March 10 2021, we’re excited to announce the availability of the **new commerce experience in CSP for Azure in Russia**.</span></span> <span data-ttu-id="ee09b-519">Den här upplevelsen effektiviserar och förbättrar kundernas sätt att köpa och använda Azure-tjänster.</span><span class="sxs-lookup"><span data-stu-id="ee09b-519">This experience will streamline and improve the way customers buy and consume Azure services.</span></span> <span data-ttu-id="ee09b-520">Det ger även partner i CSP-programmet en konsekvent vy över Azure-priser över försäljningsork, USD-priser för global konsekvens, anpassning av faktureringsdatum och åtkomst till Azure Cost Management.</span><span class="sxs-lookup"><span data-stu-id="ee09b-520">It will also give partners in the CSP program a consistent view of Azure pricing across sales motions, USD pricing for global consistency, billing date alignment, and access to Azure Cost Management.</span></span>

### <a name="next-steps"></a><span data-ttu-id="ee09b-521">Nästa steg</span><span class="sxs-lookup"><span data-stu-id="ee09b-521">Next steps</span></span>

<span data-ttu-id="ee09b-522">Det finns flera tillgängliga resurser som introducerar den nya Azure-handelsupplevelsen och ger ytterligare information.</span><span class="sxs-lookup"><span data-stu-id="ee09b-522">There are several resources available introducing the new Azure commerce experience and providing additional information.</span></span> <span data-ttu-id="ee09b-523">Hitta de senaste vanliga frågor och svar, decks, video och mer i [CSP Program Updates Resource Gallery](https://partner.microsoft.com/resources/collection/new-azure-experience-in-csp#/).</span><span class="sxs-lookup"><span data-stu-id="ee09b-523">Find the latest FAQs, decks, video and more in the [CSP Program Updates Resource Gallery](https://partner.microsoft.com/resources/collection/new-azure-experience-in-csp#/).</span></span>

________________
## <a name="partner-center-software-license-key-and-download-fulfillment"></a><a name="4"></a><span data-ttu-id="ee09b-524">Partnercenter– programvarulicensnyckel och hämtningsuppfyllelse</span><span class="sxs-lookup"><span data-stu-id="ee09b-524">Partner Center software license key and download fulfillment</span></span>

### <a name="categories"></a><span data-ttu-id="ee09b-525">Kategorier</span><span class="sxs-lookup"><span data-stu-id="ee09b-525">Categories</span></span>

- <span data-ttu-id="ee09b-526">Datum: 2021-03-04</span><span class="sxs-lookup"><span data-stu-id="ee09b-526">Date: 2021-03-04</span></span>
- <span data-ttu-id="ee09b-527">Funktioner</span><span class="sxs-lookup"><span data-stu-id="ee09b-527">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="ee09b-528">Sammanfattning</span><span class="sxs-lookup"><span data-stu-id="ee09b-528">Summary</span></span>

<span data-ttu-id="ee09b-529">Funktionen för nedladdning av programvara och licens för nyckeluppfyllelse i Partnercenter har återställts.</span><span class="sxs-lookup"><span data-stu-id="ee09b-529">The Partner Center software download and license key fulfillment capability has been reinstated.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="ee09b-530">Målgrupp som påverkas</span><span class="sxs-lookup"><span data-stu-id="ee09b-530">Impacted audience</span></span>

<span data-ttu-id="ee09b-531">Alla Molnlösningsleverantör (CSP) som gör permanenta programvarubeställningar och programvarubeställningar för serverprenumeration via Partnercenter</span><span class="sxs-lookup"><span data-stu-id="ee09b-531">All Cloud Solution Provider (CSP) partners transacting perpetual and server subscription software orders through Partner Center</span></span>

### <a name="details"></a><span data-ttu-id="ee09b-532">Information</span><span class="sxs-lookup"><span data-stu-id="ee09b-532">Details</span></span>

<span data-ttu-id="ee09b-533">Som svar på feedback från partnern omvärder vi funktionen för att uppfylla Partnercenter för att hämta programvaru- och licensnycklar för beständiga programvarubeställningar och programvaruordrar för serverprenumeration.</span><span class="sxs-lookup"><span data-stu-id="ee09b-533">In response to partner feedback, we’re reinstating the Partner Center fulfillment capability to obtain software and license keys for perpetual and server subscription software orders.</span></span> <span data-ttu-id="ee09b-534">Den återställs till sitt tidigare tillstånd innan den tas bort den 19 januari 2021.</span><span class="sxs-lookup"><span data-stu-id="ee09b-534">It will be restored to its previous state prior to being removed on January 19, 2021.</span></span> <span data-ttu-id="ee09b-535">(Se [tillkännagivandet](2020-september.md#17).)</span><span class="sxs-lookup"><span data-stu-id="ee09b-535">(See the [announcement](2020-september.md#17).)</span></span>

<span data-ttu-id="ee09b-536">Observera att nycklar för programvarulicens och nedladdningslänkar är värdefulla och eftersökta immateriella tillgångar.</span><span class="sxs-lookup"><span data-stu-id="ee09b-536">Note that software license keys and download links are valuable and highly sought-after intellectual property assets.</span></span> <span data-ttu-id="ee09b-537">Om de läcks kan de snabbt få slut på sina aktiveringsgränser och orsaka en negativ kund- och partnerupplevelse.</span><span class="sxs-lookup"><span data-stu-id="ee09b-537">If leaked, they can quickly be depleted of their activation limits and cause a negative customer and partner experience.</span></span>

### <a name="next-steps"></a><span data-ttu-id="ee09b-538">Nästa steg</span><span class="sxs-lookup"><span data-stu-id="ee09b-538">Next steps</span></span>

<span data-ttu-id="ee09b-539">Granska följande resurser för användningsanvisningar och viktig vägledning om distribution av programvarunyckel:</span><span class="sxs-lookup"><span data-stu-id="ee09b-539">Review the following resources for usage instructions and important guidance on software key distribution:</span></span>

- [<span data-ttu-id="ee09b-540">Sälja lokal programvara via CSP-programmet</span><span class="sxs-lookup"><span data-stu-id="ee09b-540">Sell on-premises software through the CSP program</span></span>](../csp-on-premise-software.md)
- <span data-ttu-id="ee09b-541">[Partner Center New Commerce Operations Guide](https://partner.microsoft.com/resources/detail/partner-center-new-commerce-operations-guide-pdf) (se avsnittet Vägledning om distribution av **programvarunyckel.)**</span><span class="sxs-lookup"><span data-stu-id="ee09b-541">[Partner Center New Commerce Operations Guide](https://partner.microsoft.com/resources/detail/partner-center-new-commerce-operations-guide-pdf) (See the **Guidance on Software Key Distribution** section.)</span></span>

### <a name="questions"></a><span data-ttu-id="ee09b-542">Har du några frågor?</span><span class="sxs-lookup"><span data-stu-id="ee09b-542">Questions?</span></span>

<span data-ttu-id="ee09b-543">Om du har ytterligare frågor om det här meddelandet kan du kontrollera dina relevanta Yammer-communities.</span><span class="sxs-lookup"><span data-stu-id="ee09b-543">If you have any further questions about this notice, check your relevant Yammer communities.</span></span>

________________
## <a name="migrate-your-deals-from-partner-sales-connect-psc-to-partner-center"></a><a name="3"></a><span data-ttu-id="ee09b-544">Migrera dina avtal från Partner Sales Connect (PSC) till Partnercenter</span><span class="sxs-lookup"><span data-stu-id="ee09b-544">Migrate your deals from Partner Sales Connect (PSC) to Partner Center</span></span>

### <a name="categories"></a><span data-ttu-id="ee09b-545">Kategorier</span><span class="sxs-lookup"><span data-stu-id="ee09b-545">Categories</span></span>

- <span data-ttu-id="ee09b-546">Datum: 2021-03-04</span><span class="sxs-lookup"><span data-stu-id="ee09b-546">Date: 2021-03-04</span></span>
- <span data-ttu-id="ee09b-547">Funktioner</span><span class="sxs-lookup"><span data-stu-id="ee09b-547">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="ee09b-548">Sammanfattning</span><span class="sxs-lookup"><span data-stu-id="ee09b-548">Summary</span></span>

<span data-ttu-id="ee09b-549">Partner Sales Connect (PSC) kommer att gå över till skrivskyddade åtkomst från och med 31 mars 2021, så vi hoppas att du ska börja migrera dina avtal från PSC till PartnerCenter.</span><span class="sxs-lookup"><span data-stu-id="ee09b-549">Partner Sales Connect (PSC) will move to read-only access starting March 31, 2021, so we urge you to begin migrating your deals from PSC to Partner Center.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="ee09b-550">Påverkad målgrupp</span><span class="sxs-lookup"><span data-stu-id="ee09b-550">Impacted audience</span></span>

<span data-ttu-id="ee09b-551">Partner med avtal i PSC</span><span class="sxs-lookup"><span data-stu-id="ee09b-551">Partners with deals in PSC</span></span>

### <a name="details"></a><span data-ttu-id="ee09b-552">Information</span><span class="sxs-lookup"><span data-stu-id="ee09b-552">Details</span></span>

<span data-ttu-id="ee09b-553">Som en del av vårt delade engagemang för tillväxt är samförsäljning med **Microsoft** den väg som du kan använda för att bli **upptäckt,** leverera din expertis och utöka ditt kundfotavtryck för positiva kundresultat.</span><span class="sxs-lookup"><span data-stu-id="ee09b-553">As part of our shared commitment to growth, **co-sell with Microsoft** is the path for you to **be discovered, deliver your expertise, and expand your customer footprint** for positive customer outcomes.</span></span> <span data-ttu-id="ee09b-554">Med ett genomsnittligt avtal som är **3,5** gånger snabbare än normalt kan du hantera din säljupplevelse i Partnercenter för att sälja direkt till kunder, partner och Microsoft-försäljningskanaler och hantera hela din hänvisningspipeline på en och samma plats.</span><span class="sxs-lookup"><span data-stu-id="ee09b-554">With an average deal that’s **3.5 times faster** than normal, managing your co-sell experience in Partner Center allows you to sell across the direct customer, partner, and Microsoft seller channels, and manage your entire referral pipeline in one location.</span></span>

<span data-ttu-id="ee09b-555">**PSC** kommer  att gå över till skrivskyddade åtkomst från och med **31 mars 2021,** så vi hoppas att du börjar flytta till Partnercenter och få åtkomst till dessa kapacitetsförbättringar:</span><span class="sxs-lookup"><span data-stu-id="ee09b-555">**PSC** will move to **read-only access** starting **March 31, 2021**, so we urge you to start your move to Partner Center and access these capability improvements:</span></span> 

- <span data-ttu-id="ee09b-556">**Mer exakt routning** av de avtal som du delar med Microsoft till rätt säljare, baserat på vilken typ av hjälp du behöver.</span><span class="sxs-lookup"><span data-stu-id="ee09b-556">**More accurate routing** of the deals that you share with Microsoft to the right seller, based on the type of assistance you need.</span></span>
- <span data-ttu-id="ee09b-557">**Validering av berättigande för** förskottsberättigade avtal för incitamentberättigade lösningar och för att uppfylla kriterierna för ISV Connect-programmet, vilket förenklar godkännandeprocessen och POE-attestation (final proof of execution).</span><span class="sxs-lookup"><span data-stu-id="ee09b-557">**Upfront deal eligibility validation** for incentive-eligible solutions and to meet the ISV Connect program criteria, simplifying the approval process and final proof of execution (POE) attestation.</span></span>
- <span data-ttu-id="ee09b-558">**Smidig användarupplevelse** för att hantera alla dina möjligheter till säljförsäljning och säljkvalificerade leads på ett och samma ställe.</span><span class="sxs-lookup"><span data-stu-id="ee09b-558">**Seamless user experience** to manage all your co-sell opportunities and sales qualified leads in one place.</span></span>

<span data-ttu-id="ee09b-559">Vi har också nyligen lagt till nya funktioner i Partnercenter för att underlätta flytten:</span><span class="sxs-lookup"><span data-stu-id="ee09b-559">We’ve also recently added new features in Partner Center to assist in your move:</span></span>

- [<span data-ttu-id="ee09b-560">Massåtgärder för möjligheter till säljförsäljning</span><span class="sxs-lookup"><span data-stu-id="ee09b-560">Bulk operations for co-sell opportunities</span></span>](../bulk-operations.md)
- <span data-ttu-id="ee09b-561">[Avtalsmigreringsfunktionen](../psc-to-pc.md) (se **avsnittet om PSC-avtalsmigrering.)**</span><span class="sxs-lookup"><span data-stu-id="ee09b-561">[Deal migration feature](../psc-to-pc.md) (See the **PSC Deals migration** section.)</span></span>

<span data-ttu-id="ee09b-562">Med hjälp av säljupplevelsen i Partnercenter får säljteamen mer tid att fokusera på att hjälpa leads och affärsmöjligheter, stänga avtal och skapa varaktiga kundrelationer.</span><span class="sxs-lookup"><span data-stu-id="ee09b-562">Using the co-sell experience in Partner Center, your sales teams will have more time to focus on nurturing leads and opportunities, closing deals, and creating lasting customer relationships.</span></span>

### <a name="next-steps"></a><span data-ttu-id="ee09b-563">Nästa steg</span><span class="sxs-lookup"><span data-stu-id="ee09b-563">Next steps</span></span>

<span data-ttu-id="ee09b-564">Använd [partnercenterövergångsguiden för](../psc-to-pc.md) att gå igenom stegen för att migrera dina avtal från PSC till Partnercenter.</span><span class="sxs-lookup"><span data-stu-id="ee09b-564">Use the Partner Center [transition guide](../psc-to-pc.md) to walk you through the steps to migrate your deals from PSC to Partner Center.</span></span>

### <a name="questions"></a><span data-ttu-id="ee09b-565">Har du några frågor?</span><span class="sxs-lookup"><span data-stu-id="ee09b-565">Questions?</span></span>

<span data-ttu-id="ee09b-566">Kontakta supporten för ytterligare [frågor.](https://partner.microsoft.com/support/?stage=1)</span><span class="sxs-lookup"><span data-stu-id="ee09b-566">For any further questions, contact [Support](https://partner.microsoft.com/support/?stage=1).</span></span>

________________
## <a name="new-microsoft-dynamics-365-products-and-offers-available-on-april-1-2021"></a><a name="2"></a><span data-ttu-id="ee09b-567">Nya Microsoft Dynamics 365-produkter och -erbjudanden är tillgängliga den 1 april 2021</span><span class="sxs-lookup"><span data-stu-id="ee09b-567">New Microsoft Dynamics 365 products and offers available on April 1, 2021</span></span>

### <a name="categories"></a><span data-ttu-id="ee09b-568">Kategorier</span><span class="sxs-lookup"><span data-stu-id="ee09b-568">Categories</span></span>

- <span data-ttu-id="ee09b-569">Datum: 2021-03-04</span><span class="sxs-lookup"><span data-stu-id="ee09b-569">Date: 2021-03-04</span></span>
- <span data-ttu-id="ee09b-570">Funktioner</span><span class="sxs-lookup"><span data-stu-id="ee09b-570">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="ee09b-571">Sammanfattning</span><span class="sxs-lookup"><span data-stu-id="ee09b-571">Summary</span></span>

<span data-ttu-id="ee09b-572">Den 1 april 2021 lanserar Microsoft flera nya produkter och erbjudanden för programmet Molnlösningsleverantör (CSP).</span><span class="sxs-lookup"><span data-stu-id="ee09b-572">On April 1, 2021, Microsoft will be launching several new products and offers for the Cloud Solution Provider (CSP) program.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="ee09b-573">Målgrupp som påverkas</span><span class="sxs-lookup"><span data-stu-id="ee09b-573">Impacted audience</span></span>

<span data-ttu-id="ee09b-574">Alla partner som gör en Molnlösningsleverantör (CSP)</span><span class="sxs-lookup"><span data-stu-id="ee09b-574">All partners transacting through the Cloud Solution Provider (CSP) program</span></span>

### <a name="details"></a><span data-ttu-id="ee09b-575">Information</span><span class="sxs-lookup"><span data-stu-id="ee09b-575">Details</span></span>

<span data-ttu-id="ee09b-576">Den 1 april 2021 lanserar Microsoft följande nya produkter och erbjudanden:</span><span class="sxs-lookup"><span data-stu-id="ee09b-576">On April 1, 2021, Microsoft will be launching the following new products and offers:</span></span>

- <span data-ttu-id="ee09b-577">Power BI Premium per användare</span><span class="sxs-lookup"><span data-stu-id="ee09b-577">Power BI Premium Per User</span></span>
- <span data-ttu-id="ee09b-578">Usl-geo- och segmentexpansion för Customer Voice and Marketing</span><span class="sxs-lookup"><span data-stu-id="ee09b-578">Customer Voice and Marketing USL geo and segment expansion</span></span>

<span data-ttu-id="ee09b-579">**Power BI Premium per användare**</span><span class="sxs-lookup"><span data-stu-id="ee09b-579">**Power BI Premium Per User**</span></span>

<span data-ttu-id="ee09b-580">Microsoft introducerar de första erbjudandena per användare Power BI Premium erbjudanden.</span><span class="sxs-lookup"><span data-stu-id="ee09b-580">Microsoft will introduce the first per-user Power BI Premium offers.</span></span> <span data-ttu-id="ee09b-581">Power BI Premium säljs för närvarande endast i en kapacitetskonstruktion.</span><span class="sxs-lookup"><span data-stu-id="ee09b-581">Power BI Premium is currently sold only in a capacity construct.</span></span> <span data-ttu-id="ee09b-582">Power BI Premium per användare ger åtkomst till business intelligence (BI) och analysfunktioner.</span><span class="sxs-lookup"><span data-stu-id="ee09b-582">Power BI Premium Per User provides access to enterprise business intelligence (BI) and analytics capabilities.</span></span> <span data-ttu-id="ee09b-583">Dess flexibla individuella klientlicensiering riktar sig till små och medelstora företag.</span><span class="sxs-lookup"><span data-stu-id="ee09b-583">Its flexible individual seat licensing caters to small and medium-sized businesses.</span></span>

<span data-ttu-id="ee09b-584">Läs informationen [Power BI om du](/power-platform-release-plan/2020wave2/power-bi/planned-features) vill veta mer om det här erbjudandet.</span><span class="sxs-lookup"><span data-stu-id="ee09b-584">Review the [Power BI release details](/power-platform-release-plan/2020wave2/power-bi/planned-features) to learn more about this offer.</span></span>


<span data-ttu-id="ee09b-585">**Erbjudandeinformation**</span><span class="sxs-lookup"><span data-stu-id="ee09b-585">**Offer details**</span></span>

<span data-ttu-id="ee09b-586">Observera att erbjudandets namn skiljer sig något från förhandsversionen av prislistan.</span><span class="sxs-lookup"><span data-stu-id="ee09b-586">Note that the offer name differs slightly from the price list preview.</span></span>

| <span data-ttu-id="ee09b-587">Erbjudandets namn</span><span class="sxs-lookup"><span data-stu-id="ee09b-587">Offer name</span></span> | <span data-ttu-id="ee09b-588">Erbjudande-ID</span><span class="sxs-lookup"><span data-stu-id="ee09b-588">Offer ID</span></span> |
| ------ |----------- |
| <span data-ttu-id="ee09b-589">Power BI Premium per användare</span><span class="sxs-lookup"><span data-stu-id="ee09b-589">Power BI Premium Per User</span></span> | <span data-ttu-id="ee09b-590">9c810018-9356-4903-95ab-eeb956289290</span><span class="sxs-lookup"><span data-stu-id="ee09b-590">9c810018-9356-4903-95ab-eeb956289290</span></span> | 
| <span data-ttu-id="ee09b-591">Power BI Premium per användare för lärare och lärare</span><span class="sxs-lookup"><span data-stu-id="ee09b-591">Power BI Premium Per User for Faculty</span></span> | <span data-ttu-id="ee09b-592">3affc44f-f372-4ad5-8657-aadd9574fce0</span><span class="sxs-lookup"><span data-stu-id="ee09b-592">3affc44f-f372-4ad5-8657-aadd9574fce0</span></span> | 
| <span data-ttu-id="ee09b-593">Power BI Premium per användare för studenter</span><span class="sxs-lookup"><span data-stu-id="ee09b-593">Power BI Premium Per User for Students</span></span> | <span data-ttu-id="ee09b-594">657eea87-d0b0-4c89-8c8e-9b04395bd940</span><span class="sxs-lookup"><span data-stu-id="ee09b-594">657eea87-d0b0-4c89-8c8e-9b04395bd940</span></span> | 
| <span data-ttu-id="ee09b-595">Power BI Premium per användare (prissättning för ideell personal)</span><span class="sxs-lookup"><span data-stu-id="ee09b-595">Power BI Premium Per User (Nonprofit Staff Pricing)</span></span> | <span data-ttu-id="ee09b-596">7a0a856c-059f-45dd-9d26-ae27992e706a</span><span class="sxs-lookup"><span data-stu-id="ee09b-596">7a0a856c-059f-45dd-9d26-ae27992e706a</span></span> | 
| <span data-ttu-id="ee09b-597">Power BI Premium per användare Add-On</span><span class="sxs-lookup"><span data-stu-id="ee09b-597">Power BI Premium Per User Add-On</span></span> | <span data-ttu-id="ee09b-598">244ff87e-5925-44a0-bf31-cea189719b58</span><span class="sxs-lookup"><span data-stu-id="ee09b-598">244ff87e-5925-44a0-bf31-cea189719b58</span></span> | 
| <span data-ttu-id="ee09b-599">Power BI Premium per Add-On för lärare och lärare</span><span class="sxs-lookup"><span data-stu-id="ee09b-599">Power BI Premium Per User Add-On for Faculty</span></span> | <span data-ttu-id="ee09b-600">5da849bd-b8f7-4340-b4f4-3a9eaeb8987e</span><span class="sxs-lookup"><span data-stu-id="ee09b-600">5da849bd-b8f7-4340-b4f4-3a9eaeb8987e</span></span> | 
| <span data-ttu-id="ee09b-601">Power BI Premium per användare Add-On för studenter</span><span class="sxs-lookup"><span data-stu-id="ee09b-601">Power BI Premium Per User Add-On for Students</span></span> | <span data-ttu-id="ee09b-602">cf62d70d-5af5-422a-bda8-97936402ac8e</span><span class="sxs-lookup"><span data-stu-id="ee09b-602">cf62d70d-5af5-422a-bda8-97936402ac8e</span></span> | 
| <span data-ttu-id="ee09b-603">Power BI Premium per användare Add-On (prissättning för ideell personal)</span><span class="sxs-lookup"><span data-stu-id="ee09b-603">Power BI Premium Per User Add-On (Nonprofit Staff Pricing)</span></span> | <span data-ttu-id="ee09b-604">31c03289-47ab-4ab0-8df1-03742c127ac6</span><span class="sxs-lookup"><span data-stu-id="ee09b-604">31c03289-47ab-4ab0-8df1-03742c127ac6</span></span> | 

<span data-ttu-id="ee09b-605">**Customer Voice and Marketing USL geo and segmentexpansion**</span><span class="sxs-lookup"><span data-stu-id="ee09b-605">**Customer Voice and Marketing USL geo and segment expansion**</span></span>

<span data-ttu-id="ee09b-606">Som en uppföljning till lanseringen i december 2020 har USL-erbjudanden för Dynamics 365 Customer Voice and Marketing ändrats för att lägga till nya länder och fler ideella organisationer och utbildnings-SKU:er.</span><span class="sxs-lookup"><span data-stu-id="ee09b-606">As a follow-up to the December 2020 launch, Dynamics 365 Customer Voice and Marketing USL offers have been changed to add new countries and more nonprofit and educational SKUs.</span></span>

| <span data-ttu-id="ee09b-607">Erbjudandets namn</span><span class="sxs-lookup"><span data-stu-id="ee09b-607">Offer name</span></span> | <span data-ttu-id="ee09b-608">Erbjudande-ID</span><span class="sxs-lookup"><span data-stu-id="ee09b-608">Offer ID</span></span> |
| ------ |----------- |
| <span data-ttu-id="ee09b-609">Dynamics 365 Customer Voice USL (prissättning för ideell personal)</span><span class="sxs-lookup"><span data-stu-id="ee09b-609">Dynamics 365 Customer Voice USL (Nonprofit Staff Pricing)</span></span> | <span data-ttu-id="ee09b-610">7a8642a5-481e-4906-a642-b56dbeeb62a0</span><span class="sxs-lookup"><span data-stu-id="ee09b-610">7a8642a5-481e-4906-a642-b56dbeeb62a0</span></span> |
| <span data-ttu-id="ee09b-611">Dynamics 365 Customer Voice USL för lärare</span><span class="sxs-lookup"><span data-stu-id="ee09b-611">Dynamics 365 Customer Voice USL for Faculty</span></span> | <span data-ttu-id="ee09b-612">85162d70-9676-4cf6-a4bc-a0d6672f2657</span><span class="sxs-lookup"><span data-stu-id="ee09b-612">85162d70-9676-4cf6-a4bc-a0d6672f2657</span></span> |

<span data-ttu-id="ee09b-613">Besök följande sidor om du vill veta mer om dessa erbjudanden:</span><span class="sxs-lookup"><span data-stu-id="ee09b-613">Visit the following pages to find out more about these offers:</span></span>

- [<span data-ttu-id="ee09b-614">Startsida för Dynamics 365 Customer Service Voice</span><span class="sxs-lookup"><span data-stu-id="ee09b-614">Dynamics 365 Customer Service Voice home page</span></span>](https://dynamics.microsoft.com/customer-voice/overview/)
- [<span data-ttu-id="ee09b-615">Startsida för Dynamics 365 Marketing</span><span class="sxs-lookup"><span data-stu-id="ee09b-615">Dynamics 365 Marketing home page</span></span>](https://dynamics.microsoft.com/customer-voice/overview/)

### <a name="next-steps"></a><span data-ttu-id="ee09b-616">Nästa steg</span><span class="sxs-lookup"><span data-stu-id="ee09b-616">Next steps</span></span>

<span data-ttu-id="ee09b-617">Granska resurserna i det här avsnittet och dela den här informationen med lämpliga intressenter i din organisation.</span><span class="sxs-lookup"><span data-stu-id="ee09b-617">Review the resources on this topic, and share this information with the appropriate stakeholders in your organization.</span></span>  

### <a name="questions"></a><span data-ttu-id="ee09b-618">Har du några frågor?</span><span class="sxs-lookup"><span data-stu-id="ee09b-618">Questions?</span></span>

<span data-ttu-id="ee09b-619">Om du har frågor om dessa erbjudanden kan du kontrollera dina relevanta Yammer-communities.</span><span class="sxs-lookup"><span data-stu-id="ee09b-619">For any questions about these offers, check your relevant Yammer communities.</span></span> 

________________
## <a name="microsoft-universal-print-now-available-in-some-suites"></a><a name="1"></a> <span data-ttu-id="ee09b-620">Microsoft Universell utskrift nu tillgängligt i vissa paket</span><span class="sxs-lookup"><span data-stu-id="ee09b-620">Microsoft Universal Print now available in some suites</span></span>

### <a name="categories"></a><span data-ttu-id="ee09b-621">Kategorier</span><span class="sxs-lookup"><span data-stu-id="ee09b-621">Categories</span></span>

- <span data-ttu-id="ee09b-622">Datum: 2021-03-03</span><span class="sxs-lookup"><span data-stu-id="ee09b-622">Date: 2021-03-03</span></span>
- <span data-ttu-id="ee09b-623">Funktioner</span><span class="sxs-lookup"><span data-stu-id="ee09b-623">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="ee09b-624">Sammanfattning</span><span class="sxs-lookup"><span data-stu-id="ee09b-624">Summary</span></span>

<span data-ttu-id="ee09b-625">Microsoft Universell utskrift kommer att vara tillgängligt för att handla inom utvalda Microsoft 365-paket och som ett fristående tillägg från den 1 mars 2021.</span><span class="sxs-lookup"><span data-stu-id="ee09b-625">Microsoft Universal Print will be available to transact within select Microsoft 365 suites and as a standalone add-on from March 1, 2021.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="ee09b-626">Påverkad målgrupp</span><span class="sxs-lookup"><span data-stu-id="ee09b-626">Impacted audience</span></span>

<span data-ttu-id="ee09b-627">Alla partner som gör en Molnlösningsleverantör via CSP-programmet</span><span class="sxs-lookup"><span data-stu-id="ee09b-627">All partners transacting through the Cloud Solution Provider (CSP) program</span></span>

### <a name="details"></a><span data-ttu-id="ee09b-628">Information</span><span class="sxs-lookup"><span data-stu-id="ee09b-628">Details</span></span>

<span data-ttu-id="ee09b-629">[Universell utskrift](https://aka.ms/universalprint) är en Microsoft 365 utskriftstjänst som tar bort behovet av lokala utskriftsservrar och gör det möjligt för Windows-enheter att skriva ut till Azure-registrerade skrivare.</span><span class="sxs-lookup"><span data-stu-id="ee09b-629">[Universal Print](https://aka.ms/universalprint) is a Microsoft 365 print service that removes the need for on-premises print servers, and enables Windows devices to print to Azure-registered printers.</span></span> <span data-ttu-id="ee09b-630">Den kommer att vara tillgänglig för transact från den 1 mars 2021.</span><span class="sxs-lookup"><span data-stu-id="ee09b-630">It will be available to transact from March 1, 2021.</span></span>

<span data-ttu-id="ee09b-631">Arbetare drar nytta av drivrutinslöst utskrift, strömlinjeformad platsbaserad skrivaridentifiering och en intuitiv utskriftsupplevelse utan inlärningskurva.</span><span class="sxs-lookup"><span data-stu-id="ee09b-631">Workers benefit from driverless printing, streamlined location-based printer discovery, and an intuitive printing experience with no learning curve.</span></span> <span data-ttu-id="ee09b-632">Enheter som är anslutna till Azure Active Directory (Azure AD) använder befintliga Azure AD-autentiseringsuppgifter för att skriva ut på ett säkert sätt.</span><span class="sxs-lookup"><span data-stu-id="ee09b-632">Devices that are joined to Azure Active Directory (Azure AD) use existing Azure AD credentials to print securely.</span></span> <span data-ttu-id="ee09b-633">Administratörer hanterar utskrift med hjälp av Azure Portal och kan enkelt ansluta skrivare med inbyggt stöd för Universell utskrift.</span><span class="sxs-lookup"><span data-stu-id="ee09b-633">Administrators manage printing by using the Azure portal, and can easily connect printers with native support for Universal Print.</span></span> <span data-ttu-id="ee09b-634">Universell utskrift kan distribueras med icke-kompatibla skrivare med hjälp av Anslutning för Universell utskrift programvara.</span><span class="sxs-lookup"><span data-stu-id="ee09b-634">Universal Print can be deployed with non-compatible printers by using Universal Print connector software.</span></span>

<span data-ttu-id="ee09b-635">Universell utskrift återfylls vid start till Windows E3, A3, E5 och A5 och Microsoft 365 BP, F3, E3, A3, E5 och A5.</span><span class="sxs-lookup"><span data-stu-id="ee09b-635">Universal Print will be backfilled at launch to Windows E3, A3, E5, and A5, and Microsoft 365 BP, F3, E3, A3, E5, and A5.</span></span>  

<span data-ttu-id="ee09b-636">**Erbjudandeinformation**</span><span class="sxs-lookup"><span data-stu-id="ee09b-636">**Offer details**</span></span>

<span data-ttu-id="ee09b-637">Observera att erbjudandets namn skiljer sig något från förhandsversionen av prislistan.</span><span class="sxs-lookup"><span data-stu-id="ee09b-637">Note that the offer name differs slightly from the price list preview.</span></span>

| <span data-ttu-id="ee09b-638">Erbjudandets namn</span><span class="sxs-lookup"><span data-stu-id="ee09b-638">Offer name</span></span> | <span data-ttu-id="ee09b-639">Erbjudande-ID</span><span class="sxs-lookup"><span data-stu-id="ee09b-639">Offer ID</span></span> | <span data-ttu-id="ee09b-640">Material-ID</span><span class="sxs-lookup"><span data-stu-id="ee09b-640">Material ID</span></span> |
| ------ |----------- |----------- |  
| <span data-ttu-id="ee09b-641">Universell utskrift volymökning (500 jobb) – Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="ee09b-641">Universal Print volume add-on (500 jobs) - Microsoft 365</span></span>  | <span data-ttu-id="ee09b-642">cb131356-45ee-4ae2-8537-873b706c8e75</span><span class="sxs-lookup"><span data-stu-id="ee09b-642">cb131356-45ee-4ae2-8537-873b706c8e75</span></span>     | <span data-ttu-id="ee09b-643">9BI-00004</span><span class="sxs-lookup"><span data-stu-id="ee09b-643">9BI-00004</span></span>   |
| <span data-ttu-id="ee09b-644">Universell utskrift volymökning (500 jobb) för lärare och lärare – Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="ee09b-644">Universal Print volume add-on (500 jobs) for faculty - Microsoft 365</span></span>   | <span data-ttu-id="ee09b-645">477 tb81-9872-43d6-91d3-c72390bfcf49</span><span class="sxs-lookup"><span data-stu-id="ee09b-645">477bee81-9872-43d6-91d3-c72390bfcf49</span></span>   | <span data-ttu-id="ee09b-646">9BK-00004</span><span class="sxs-lookup"><span data-stu-id="ee09b-646">9BK-00004</span></span>   |
| <span data-ttu-id="ee09b-647">Universell utskrift volymökning (500 jobb) – Windows</span><span class="sxs-lookup"><span data-stu-id="ee09b-647">Universal Print volume add-on (500 jobs) - Windows</span></span>    | <span data-ttu-id="ee09b-648">d3ddc493-5741-4e0d-a02d-07edbb0bb72e</span><span class="sxs-lookup"><span data-stu-id="ee09b-648">d3ddc493-5741-4e0d-a02d-07edbb0bb72e</span></span>   | <span data-ttu-id="ee09b-649">9BI-00002</span><span class="sxs-lookup"><span data-stu-id="ee09b-649">9BI-00002</span></span>   |
| <span data-ttu-id="ee09b-650">Universell utskrift volym tillägg (500 jobb) för lärare – Windows</span><span class="sxs-lookup"><span data-stu-id="ee09b-650">Universal Print volume add-on (500 jobs) for faculty - Windows</span></span>   |  <span data-ttu-id="ee09b-651">d0862f05-80f5-4fd4-8432-fe72dd893cc7</span><span class="sxs-lookup"><span data-stu-id="ee09b-651">d0862f05-80f5-4fd4-8432-fe72dd893cc7</span></span>  | <span data-ttu-id="ee09b-652">9BK-00002</span><span class="sxs-lookup"><span data-stu-id="ee09b-652">9BK-00002</span></span>   |

### <a name="next-steps"></a><span data-ttu-id="ee09b-653">Nästa steg</span><span class="sxs-lookup"><span data-stu-id="ee09b-653">Next steps</span></span>

<span data-ttu-id="ee09b-654">Bekanta dig med prislistan och Universell utskrift [översikt](/universal-print/fundamentals/universal-print-whatis).</span><span class="sxs-lookup"><span data-stu-id="ee09b-654">Familiarize yourself with the price list and the [Universal Print overview](/universal-print/fundamentals/universal-print-whatis).</span></span> <span data-ttu-id="ee09b-655">Dela den här informationen med alla lämpliga kontakter i din organisation.</span><span class="sxs-lookup"><span data-stu-id="ee09b-655">Share this information with all appropriate contacts in your organization.</span></span>

### <a name="questions"></a><span data-ttu-id="ee09b-656">Har du några frågor?</span><span class="sxs-lookup"><span data-stu-id="ee09b-656">Questions?</span></span>

<span data-ttu-id="ee09b-657">Om du har frågor om dessa erbjudanden kan du kontrollera dina relevanta Yammer-communities.</span><span class="sxs-lookup"><span data-stu-id="ee09b-657">For any questions about these offers, check your relevant Yammer communities.</span></span>
