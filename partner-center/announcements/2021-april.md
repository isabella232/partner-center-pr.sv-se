---
title: Meddelanden april 2021
description: April 2021-meddelanden för Microsoft Partner Center, inklusive nya funktioner, kampanjer, erbjudanden, marknader eller ändringar i befintliga erbjudanden.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: brentserbus
ms.author: brserbus
ms.custom:
- announcement
- references_regions
ms.localizationpriority: high
ms.date: 04/29/2021
ms.openlocfilehash: d26d1af994ae9a3f951ee9428ee6fd092b2c91d8
ms.sourcegitcommit: 6c20c3cc4a226cada70c56df295966696affcec8
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/30/2021
ms.locfileid: "108328057"
---
# <a name="april-2021-announcements"></a><span data-ttu-id="86528-103">Meddelanden april 2021</span><span class="sxs-lookup"><span data-stu-id="86528-103">April 2021 announcements</span></span>

<span data-ttu-id="86528-104">Den här sidan innehåller meddelanden för Microsoft Partner Center för april 2021.</span><span class="sxs-lookup"><span data-stu-id="86528-104">This page provides the announcements for Microsoft Partner Center for April 2021.</span></span>

## <a name="readiness-updated-csp-customer-address-validation-api-going-live-in-june-testing-capability-now-available"></a><a name="10"></a><span data-ttu-id="86528-105">Beredskap: Uppdaterade CSP-kundadressvaliderings-API:et går i drift i juni. nu tillgänglig testfunktion</span><span class="sxs-lookup"><span data-stu-id="86528-105">Readiness: Updated CSP customer address validation API going live in June; testing capability now available</span></span>

### <a name="categories"></a><span data-ttu-id="86528-106">Kategorier</span><span class="sxs-lookup"><span data-stu-id="86528-106">Categories</span></span>

- <span data-ttu-id="86528-107">Datum: 2021-04-30</span><span class="sxs-lookup"><span data-stu-id="86528-107">Date: 2021-04-30</span></span>
- <span data-ttu-id="86528-108">Beredskap</span><span class="sxs-lookup"><span data-stu-id="86528-108">Readiness</span></span>

### <a name="summary"></a><span data-ttu-id="86528-109">Sammanfattning</span><span class="sxs-lookup"><span data-stu-id="86528-109">Summary</span></span>

<span data-ttu-id="86528-110">För att hjälpa partner och kunder att driva sin verksamhet baserat på förtroende kommer vi att bjuda in partner att testa ändringar i API:et validate address för alla länder över hela världen.</span><span class="sxs-lookup"><span data-stu-id="86528-110">To help partners and customers run their business based on trust, we’ll be inviting partners to test changes to the Validate Address API for all countries worldwide.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="86528-111">Påverkad målgrupp</span><span class="sxs-lookup"><span data-stu-id="86528-111">Impacted audience</span></span>

<span data-ttu-id="86528-112">CSP-direktfaktureringspartner och indirekta leverantörer som skapar nya eller uppdaterar befintliga kunders adressinformation</span><span class="sxs-lookup"><span data-stu-id="86528-112">CSP direct bill partners and indirect providers who create new or update existing customers’ address details</span></span>

### <a name="details"></a><span data-ttu-id="86528-113">Information</span><span class="sxs-lookup"><span data-stu-id="86528-113">Details</span></span>

<span data-ttu-id="86528-114">Microsoft körs med förtroende.</span><span class="sxs-lookup"><span data-stu-id="86528-114">Microsoft runs on trust.</span></span> <span data-ttu-id="86528-115">Vi strävar efter att tillhandahålla en kompatibel, säker och säker metod för kundadressvalidering för att hantera kundprenumerationer i CSP-programmet.</span><span class="sxs-lookup"><span data-stu-id="86528-115">We’re committed to providing a compliant, safe, and secure method of customer address validation for transacting customer subscriptions in the CSP program.</span></span> <span data-ttu-id="86528-116">Från och med 31 mars 2021 har vi infört ändringar i API:et validate address.</span><span class="sxs-lookup"><span data-stu-id="86528-116">As of March 31, 2021, we have introduced changes to the Validate Address API.</span></span> <span data-ttu-id="86528-117">Vi bjuder in partner att testa API:et före go-live i slutet av juni 2021.</span><span class="sxs-lookup"><span data-stu-id="86528-117">We invite partners to test the API prior to the  go-live at the end of June 2021.</span></span> 

<span data-ttu-id="86528-118">Observera att dessa ändringar endast påverkar API:et verifiera adress.</span><span class="sxs-lookup"><span data-stu-id="86528-118">Note that these changes affect the Validate Address API only.</span></span> <span data-ttu-id="86528-119">API:er för att skapa kund och uppdatera faktureringsprofil påverkas inte.</span><span class="sxs-lookup"><span data-stu-id="86528-119">Create Customer and Update Billing Profile APIs aren’t affected.</span></span> <span data-ttu-id="86528-120">Även om den föreslagna adressen för närvarande inte behöver användas med API:et för att skapa kund rekommenderas det starkt.</span><span class="sxs-lookup"><span data-stu-id="86528-120">Although the suggested address doesn’t currently have to be used with the Create Customer API, it’s highly recommended.</span></span>

<span data-ttu-id="86528-121">Svaret returnerar något av följande statusmeddelanden:</span><span class="sxs-lookup"><span data-stu-id="86528-121">The response will return one of the following status messages:</span></span>

| <span data-ttu-id="86528-122">Status</span><span class="sxs-lookup"><span data-stu-id="86528-122">Status</span></span>     | <span data-ttu-id="86528-123">Beskrivning</span><span class="sxs-lookup"><span data-stu-id="86528-123">Description</span></span> |    <span data-ttu-id="86528-124">Antal föreslagna adresser som returneras</span><span class="sxs-lookup"><span data-stu-id="86528-124">Number of suggested addresses returned</span></span> |
|-------|---------------|-------------------|
|<span data-ttu-id="86528-125">Verifierad shippable</span><span class="sxs-lookup"><span data-stu-id="86528-125">Verified shippable</span></span> | <span data-ttu-id="86528-126">Adressen är verifierad och kan skickas till.</span><span class="sxs-lookup"><span data-stu-id="86528-126">Address is verified and can be shipped to.</span></span> | <span data-ttu-id="86528-127">Enkel</span><span class="sxs-lookup"><span data-stu-id="86528-127">Single</span></span> |
|<span data-ttu-id="86528-128">Verifierat</span><span class="sxs-lookup"><span data-stu-id="86528-128">Verified</span></span> | <span data-ttu-id="86528-129">Adressen är verifierad.</span><span class="sxs-lookup"><span data-stu-id="86528-129">Address is verified.</span></span> | <span data-ttu-id="86528-130">Enkel</span><span class="sxs-lookup"><span data-stu-id="86528-130">Single</span></span> |
|<span data-ttu-id="86528-131">Interaktion krävs</span><span class="sxs-lookup"><span data-stu-id="86528-131">Interaction required</span></span> | <span data-ttu-id="86528-132">Den föreslagna adressen har ändrats avsevärt och kräver användarbekräftelse.</span><span class="sxs-lookup"><span data-stu-id="86528-132">Suggested address has been changed significantly and needs user confirmation.</span></span> | <span data-ttu-id="86528-133">Enkel</span><span class="sxs-lookup"><span data-stu-id="86528-133">Single</span></span> |
|<span data-ttu-id="86528-134">Partiell gatuadress</span><span class="sxs-lookup"><span data-stu-id="86528-134">Street partial</span></span> | <span data-ttu-id="86528-135">Den angivna gatuadressen är delvis och behöver mer information.</span><span class="sxs-lookup"><span data-stu-id="86528-135">The given street in the address is partial and needs more info.</span></span> | <span data-ttu-id="86528-136">Flera – högst tre</span><span class="sxs-lookup"><span data-stu-id="86528-136">Multiple—maximum of three</span></span> |
|<span data-ttu-id="86528-137">Delvis lokal</span><span class="sxs-lookup"><span data-stu-id="86528-137">Premises partial</span></span> | <span data-ttu-id="86528-138">De angivna lokalerna (byggnadsnummer, svitnummer och andra) är ofullständiga och behöver mer information.</span><span class="sxs-lookup"><span data-stu-id="86528-138">The given premises (building number, suite number, and others) are partial and need more info.</span></span> | <span data-ttu-id="86528-139">Flera – högst tre</span><span class="sxs-lookup"><span data-stu-id="86528-139">Multiple—maximum of three</span></span> |
|<span data-ttu-id="86528-140">Flera</span><span class="sxs-lookup"><span data-stu-id="86528-140">Multiple</span></span> | <span data-ttu-id="86528-141">Det finns flera fält som är partiella i adressen (inklusive delvis gatuadress och delvis lokal).</span><span class="sxs-lookup"><span data-stu-id="86528-141">There are multiple fields that are partial in the address (potentially also including street partial and premises partial).</span></span> | <span data-ttu-id="86528-142">Flera – högst tre</span><span class="sxs-lookup"><span data-stu-id="86528-142">Multiple—maximum of three</span></span> |
|<span data-ttu-id="86528-143">Inget</span><span class="sxs-lookup"><span data-stu-id="86528-143">None</span></span> | <span data-ttu-id="86528-144">Adressen är felaktig.</span><span class="sxs-lookup"><span data-stu-id="86528-144">Address is incorrect.</span></span> | <span data-ttu-id="86528-145">Inget</span><span class="sxs-lookup"><span data-stu-id="86528-145">None</span></span> |
|<span data-ttu-id="86528-146">Inte validerat</span><span class="sxs-lookup"><span data-stu-id="86528-146">Not validated</span></span> | <span data-ttu-id="86528-147">Adressen kunde inte skickas via verifieringsprocessen.</span><span class="sxs-lookup"><span data-stu-id="86528-147">Address was not able to be sent through the validation process.</span></span> | <span data-ttu-id="86528-148">Inget</span><span class="sxs-lookup"><span data-stu-id="86528-148">None</span></span> |

<span data-ttu-id="86528-149">Amerikanska postkoder returnerar ytterligare fyra siffror + bindestreck, till exempel 12345-6789.</span><span class="sxs-lookup"><span data-stu-id="86528-149">US post codes will return an additional four digits + hyphen, for example, 12345-6789.</span></span>

### <a name="next-steps"></a><span data-ttu-id="86528-150">Nästa steg</span><span class="sxs-lookup"><span data-stu-id="86528-150">Next steps</span></span>

- <span data-ttu-id="86528-151">Mer detaljerad vägledning finns i den tekniska dokumentationen och vanliga frågor [och svar i](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/) den dedikerade partnersamlingen.</span><span class="sxs-lookup"><span data-stu-id="86528-151">Review the technical documentation and frequently asked questions in the [dedicated partner collection](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/) for more detailed guidance.</span></span>
- <span data-ttu-id="86528-152">Förbered för att införliva ändringarna med partnercenter-API:et och webbanvändarupplevelsen.</span><span class="sxs-lookup"><span data-stu-id="86528-152">Prepare to incorporate the changes using the Partner Center API and web user experience.</span></span> 
- <span data-ttu-id="86528-153">Dela ditt sandbox-klientorganisations-ID med ämnesexperten (Ali Firmwareki) som ska ingå i testresan, så att du kan börja förbereda dig för uppdateringen.</span><span class="sxs-lookup"><span data-stu-id="86528-153">Share your sandbox tenant ID with the subject matter expert (Ali Khaki) to be included in the test flight, so that you can begin preparing for the update.</span></span> 
- <span data-ttu-id="86528-154">Om du använder en CPV-lösning (Kontrollpanelen) bör du kontakta din CPV.</span><span class="sxs-lookup"><span data-stu-id="86528-154">If you’re using a control panel vendor (CPV) solution, consult your CPV.</span></span>

### <a name="questions"></a><span data-ttu-id="86528-155">Har du några frågor?</span><span class="sxs-lookup"><span data-stu-id="86528-155">Questions?</span></span>

<span data-ttu-id="86528-156">Om du behöver support för dina åtgärder med Microsoft kan du kontakta din yammer-grupp för partnersupport eller öppna en [tjänstbegäran.](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=aa679372-d996-73df-e244-cb28bbbf28e8)</span><span class="sxs-lookup"><span data-stu-id="86528-156">If you need support for your operations with Microsoft, reach out to your partner support Yammer group or open a [service request](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=aa679372-d996-73df-e244-cb28bbbf28e8).</span></span>

_______________
## <a name="new-location-for-partner-center-api-swagger-documentation"></a><a name="9"></a><span data-ttu-id="86528-157">Ny plats för Swagger-dokumentation för Partner Center API</span><span class="sxs-lookup"><span data-stu-id="86528-157">New location for Partner Center API Swagger documentation</span></span>

### <a name="categories"></a><span data-ttu-id="86528-158">Kategorier</span><span class="sxs-lookup"><span data-stu-id="86528-158">Categories</span></span>

- <span data-ttu-id="86528-159">Datum: 2021-04-26</span><span class="sxs-lookup"><span data-stu-id="86528-159">Date: 2021-04-26</span></span>
- <span data-ttu-id="86528-160">Funktioner</span><span class="sxs-lookup"><span data-stu-id="86528-160">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="86528-161">Sammanfattning</span><span class="sxs-lookup"><span data-stu-id="86528-161">Summary</span></span>

<span data-ttu-id="86528-162">Partner Center API Swagger-dokument har migrerats från den tidigare [Webbplatsen för Swagger-dokumentation](https://apidocs.microsoft.com/services/partnercenter) till en [ny Swagger-dokumentationswebbplats.](https://docs.microsoft.com/rest/api/partner-center-rest/)</span><span class="sxs-lookup"><span data-stu-id="86528-162">Partner Center API Swagger documents have been migrated from the [previous Swagger Documentation site](https://apidocs.microsoft.com/services/partnercenter) to a [new Swagger Documentation site](https://docs.microsoft.com/rest/api/partner-center-rest/).</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="86528-163">Påverkad målgrupp</span><span class="sxs-lookup"><span data-stu-id="86528-163">Impacted audience</span></span>

<span data-ttu-id="86528-164">Direktfaktureringspartner och indirekta leverantörer som deltar i Molnlösningsleverantör-programmet (CSP) som använder Partner Center-API:erna</span><span class="sxs-lookup"><span data-stu-id="86528-164">Direct bill partners and Indirect Providers participating in the Cloud Solution Provider (CSP) program who are using the Partner Center APIs</span></span>

### <a name="details"></a><span data-ttu-id="86528-165">Information</span><span class="sxs-lookup"><span data-stu-id="86528-165">Details</span></span>

<span data-ttu-id="86528-166">Från och med 26 april 2021 finns Partner Center API Swagger-dokumentationen, inklusive Rest API-innehåll, på en [ny webbplats.](https://docs.microsoft.com/rest/api/partner-center-rest/)</span><span class="sxs-lookup"><span data-stu-id="86528-166">As of April 26, 2021 the Partner Center API Swagger documentation, including Rest API content, is located on a [new site](https://docs.microsoft.com/rest/api/partner-center-rest/).</span></span> <span data-ttu-id="86528-167">Den gamla webbplatsen är otillgänglig efter flera veckor.</span><span class="sxs-lookup"><span data-stu-id="86528-167">The old site will be inaccessible after several weeks.</span></span>

### <a name="benefits"></a><span data-ttu-id="86528-168">Fördelar</span><span class="sxs-lookup"><span data-stu-id="86528-168">Benefits</span></span>

<span data-ttu-id="86528-169">Swagger-dokumentationen för Partnercenter-API:et tillhandahåller **en Try It-funktion.**</span><span class="sxs-lookup"><span data-stu-id="86528-169">The Partner Center API Swagger documentation will provide a **Try It** function.</span></span> <span data-ttu-id="86528-170">Om du vill använda den här funktionen måste du ha en bearer-token som du kan generera genom att följa stegen i [Partner Center-autentisering.](https://docs.microsoft.com/partner-center/develop/partner-center-authentication#app--user-authentication)</span><span class="sxs-lookup"><span data-stu-id="86528-170">To use this function, you’ll need to have a Bearer Token, which you can generate by following the steps listed in [Partner Center Authentication](https://docs.microsoft.com/partner-center/develop/partner-center-authentication#app--user-authentication).</span></span>

### <a name="next-steps"></a><span data-ttu-id="86528-171">Nästa steg</span><span class="sxs-lookup"><span data-stu-id="86528-171">Next steps</span></span>

<span data-ttu-id="86528-172">Dela den här informationen i din organisation så att rätt team kan granska och uppdatera sina processer.</span><span class="sxs-lookup"><span data-stu-id="86528-172">Share this information within your organization so that the appropriate team can review and update their processes.</span></span>

### <a name="questions"></a><span data-ttu-id="86528-173">Har du några frågor?</span><span class="sxs-lookup"><span data-stu-id="86528-173">Questions?</span></span>

<span data-ttu-id="86528-174">Frågor om dessa erbjudanden finns i dina relevanta Yammer-communities.</span><span class="sxs-lookup"><span data-stu-id="86528-174">For questions about these offers, check your relevant Yammer communities.</span></span>

________________
## <a name="cloud-solution-provider-csp-software-return-period-policy-and-download-link-expiry-notice"></a><a name="8"></a><span data-ttu-id="86528-175">Molnlösningsleverantör (CSP) princip för programvarureturperiod och förfallomeddelande om nedladdningslänk</span><span class="sxs-lookup"><span data-stu-id="86528-175">Cloud Solution Provider (CSP) software return period policy and download link expiry notice</span></span>

### <a name="categories"></a><span data-ttu-id="86528-176">Kategorier</span><span class="sxs-lookup"><span data-stu-id="86528-176">Categories</span></span>

- <span data-ttu-id="86528-177">Datum: 2021-04-21</span><span class="sxs-lookup"><span data-stu-id="86528-177">Date: 2021-04-21</span></span>
- <span data-ttu-id="86528-178">Funktioner</span><span class="sxs-lookup"><span data-stu-id="86528-178">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="86528-179">Sammanfattning</span><span class="sxs-lookup"><span data-stu-id="86528-179">Summary</span></span>

<span data-ttu-id="86528-180">Det finns ändringar i CSP-principen för programvarureturperiod och nedladdningslänken upphör att gälla.</span><span class="sxs-lookup"><span data-stu-id="86528-180">There are changes to the CSP software return period policy and download link expiry.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="86528-181">Påverkad målgrupp</span><span class="sxs-lookup"><span data-stu-id="86528-181">Impacted audience</span></span>

<span data-ttu-id="86528-182">Partner som gör permanenta programvaru- eller programvaruprenumerationserbjudanden i CSP</span><span class="sxs-lookup"><span data-stu-id="86528-182">Partners transacting perpetual software or software subscription offers in CSP</span></span>

### <a name="details"></a><span data-ttu-id="86528-183">Information</span><span class="sxs-lookup"><span data-stu-id="86528-183">Details</span></span>

<span data-ttu-id="86528-184">Observera följande viktiga meddelanden om löpande programvaru- och programvaruprenumerationsköp via Partnercenter:</span><span class="sxs-lookup"><span data-stu-id="86528-184">Note the following important notifications regarding perpetual software and software subscription purchases through Partner Center:</span></span>

#### <a name="software-return-period-policy"></a><span data-ttu-id="86528-185">Princip för programvarureturperiod</span><span class="sxs-lookup"><span data-stu-id="86528-185">Software return period policy</span></span>

<span data-ttu-id="86528-186">Från den 1 juni 2021 ändras returperioden för programvaruerbjudanden i CSP enligt vad som anges i Microsoft-partneravtal (MPA) från 60 dagar från orderdatumet till 30 dagar från orderdatumet.</span><span class="sxs-lookup"><span data-stu-id="86528-186">From June 1, 2021, the return period for software offers in CSP, as stated in the Microsoft Partner Agreement (MPA), will change from 60 days from order date to 30 days from order date.</span></span>

<span data-ttu-id="86528-187">När en beställning av ett programvaruerbjudande har skickats har partnern 30 dagar från orderdatumet för att skicka eventuella ändringar till en sådan beställning:</span><span class="sxs-lookup"><span data-stu-id="86528-187">After an order for a software offer is submitted, partners will have 30 days from the order date to submit any revisions to such order:</span></span>

- <span data-ttu-id="86528-188">Alla permanent programvarulicens som returneras inom 30-dagars returperioden får en fullständig kredit av det betalda inköpspriset.</span><span class="sxs-lookup"><span data-stu-id="86528-188">Any perpetual software license returned within the 30-day return period will receive a full credit of the paid purchase price.</span></span>

- <span data-ttu-id="86528-189">Alla produkter för programvaruprenumeration som returneras inom 30-dagars returperioden får en pronomenterad kredit av det betalda inköpspriset.</span><span class="sxs-lookup"><span data-stu-id="86528-189">Any software subscription product returned within the 30-day return period will receive a prorated credit of the paid purchase price.</span></span>

<span data-ttu-id="86528-190">Det här meddelandet är en uppföljning av vår e-postkommunikation som skickades december 2020 och april 2021 till alla CSP-partner angående returperioden och andra uppdateringar av MPA.</span><span class="sxs-lookup"><span data-stu-id="86528-190">This message is a follow-up to our email communications sent on December 2020 and April 2021 to all CSP partners regarding the return period and other updates to the MPA.</span></span> <span data-ttu-id="86528-191">Se dessa meddelanden för fullständig information om ändringar som påverkar MPA.</span><span class="sxs-lookup"><span data-stu-id="86528-191">Refer to those notices for full details regarding changes affecting the MPA.</span></span>

#### <a name="software-download-link-expiry"></a><span data-ttu-id="86528-192">Länk för nedladdning av programvara upphör att gälla</span><span class="sxs-lookup"><span data-stu-id="86528-192">Software download link expiry</span></span>

<span data-ttu-id="86528-193">Från och med 3 juni 2021 har nedladdningslänkarna för programvara för beständiga programvaru- och programvaruprenumerationsköp via Partnercenter ett förfallodatum på fem dagar från den första nedladdningen.</span><span class="sxs-lookup"><span data-stu-id="86528-193">From June 3, 2021, the software download links for perpetual software and software subscription product purchases through Partner Center will have an expiration date of five days from the initial download.</span></span> <span data-ttu-id="86528-194">Förfalloperioden gäller för alla inköp före 3 juni 2021, samt den eller efter 3 juni 2021.</span><span class="sxs-lookup"><span data-stu-id="86528-194">The expiry period will apply to all purchases before June 3, 2021, as well as on or after June 3, 2021.</span></span>

### <a name="next-steps"></a><span data-ttu-id="86528-195">Nästa steg</span><span class="sxs-lookup"><span data-stu-id="86528-195">Next steps</span></span>

<span data-ttu-id="86528-196">Granska [CSP-returperioden och vanliga frågor och svar om nedladdningslänkens](https://partner.microsoft.com/resources/detail/csp-software-return-period-download-expiry-faq-pdf)upphörande och informera alla lämpliga team i din organisation om dessa ändringar:</span><span class="sxs-lookup"><span data-stu-id="86528-196">Review the [CSP return period and download link expiry FAQ](https://partner.microsoft.com/resources/detail/csp-software-return-period-download-expiry-faq-pdf), and inform all appropriate teams within your organization of these changes:</span></span>

### <a name="questions"></a><span data-ttu-id="86528-197">Har du några frågor?</span><span class="sxs-lookup"><span data-stu-id="86528-197">Questions?</span></span>

<span data-ttu-id="86528-198">Om du har frågor om dessa erbjudanden kan du kontrollera dina relevanta Yammer-communities.</span><span class="sxs-lookup"><span data-stu-id="86528-198">For questions about these offers, check your relevant Yammer communities.</span></span>

________________
## <a name="open-licensing-program-transitioning-resellers-to-the-cloud-solution-provider-csp-program"></a><a name="7"></a><span data-ttu-id="86528-199">Open Licensing Program: Övergångsåterförsäljare till Molnlösningsleverantör (CSP)-programmet</span><span class="sxs-lookup"><span data-stu-id="86528-199">Open Licensing program: Transitioning resellers to the Cloud Solution Provider (CSP) program</span></span>

### <a name="categories"></a><span data-ttu-id="86528-200">Kategorier</span><span class="sxs-lookup"><span data-stu-id="86528-200">Categories</span></span>

- <span data-ttu-id="86528-201">Datum: 2021-04-19</span><span class="sxs-lookup"><span data-stu-id="86528-201">Date: 2021-04-19</span></span>
- <span data-ttu-id="86528-202">Utveckla din verksamhet</span><span class="sxs-lookup"><span data-stu-id="86528-202">Grow Your Business</span></span>

### <a name="summary"></a><span data-ttu-id="86528-203">Sammanfattning</span><span class="sxs-lookup"><span data-stu-id="86528-203">Summary</span></span>

<span data-ttu-id="86528-204">Den här kommunikationen beskriver hur du förbereder för de ändringar som snart kommer till Open Licensing-programmet.</span><span class="sxs-lookup"><span data-stu-id="86528-204">This communication details how to prepare for the changes that are coming soon to the Open Licensing program.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="86528-205">Målgrupp som påverkas</span><span class="sxs-lookup"><span data-stu-id="86528-205">Impacted audience</span></span>

<span data-ttu-id="86528-206">CSP- och Open License-partner</span><span class="sxs-lookup"><span data-stu-id="86528-206">CSP and Open License partners</span></span>

### <a name="details"></a><span data-ttu-id="86528-207">Information</span><span class="sxs-lookup"><span data-stu-id="86528-207">Details</span></span>

<span data-ttu-id="86528-208">2020 meddelade [Microsoft](https://blogs.partner.microsoft.com/mpn/general-availability-of-perpetual-software-licenses-in-the-cloud-solution-provider-program/) att permanenta programvarulicenser kommer att vara allmänt tillgängliga för partner och kunder via programmet Molnlösningsleverantör (CSP).</span><span class="sxs-lookup"><span data-stu-id="86528-208">In 2020, Microsoft [announced](https://blogs.partner.microsoft.com/mpn/general-availability-of-perpetual-software-licenses-in-the-cloud-solution-provider-program/) that perpetual software licenses will be broadly available to partners and customers through the Cloud Solution Provider (CSP) program.</span></span> <span data-ttu-id="86528-209">Den första milstolpen nåddes i januari 2021, när kommersiella permanenta programvaruerbjudanden blev tillgängliga.</span><span class="sxs-lookup"><span data-stu-id="86528-209">The first milestone was reached in January 2021, when commercial perpetual software offers became available.</span></span> <span data-ttu-id="86528-210">Nästa viktiga milstolpe sker i juli 2021 när erbjudanden [inom den offentliga sektorn](https://aka.ms/openlicensepublicsector) blir tillgängliga.</span><span class="sxs-lookup"><span data-stu-id="86528-210">The next key milestone will happen in July 2021, when [public sector](https://aka.ms/openlicensepublicsector) offers become available.</span></span> <span data-ttu-id="86528-211">Vi har [också](https://blogs.partner.microsoft.com/mpn/expanding-opportunities-for-partners-in-the-cloud-solution-provider-program/) meddelat att från och med den 1 januari 2022 kan inga nya inköp eller förnyelser av Software Assurance eller onlinetjänster göras via Open License-programmet.</span><span class="sxs-lookup"><span data-stu-id="86528-211">We also [communicated](https://blogs.partner.microsoft.com/mpn/expanding-opportunities-for-partners-in-the-cloud-solution-provider-program/) that effective January 1, 2022, no new software license purchases or renewals of Software Assurance or online services can be made through the Open License program.</span></span>

<span data-ttu-id="86528-212">Övergången av permanent programvara till CSP-programmet i den nya handelsupplevelsen hjälper partner att utöka möjligheterna att erbjuda olika lösningar och hanterade tjänster.</span><span class="sxs-lookup"><span data-stu-id="86528-212">The transition of perpetual software to the CSP program in the new commerce experience will help partners to expand the opportunities to offer diverse solutions and managed services.</span></span> <span data-ttu-id="86528-213">Detta påskyndar även kundernas övergång till molnet.</span><span class="sxs-lookup"><span data-stu-id="86528-213">This will also accelerate customers’ transition to the cloud.</span></span>  <span data-ttu-id="86528-214">För att säkerställa en smidig övergång för både våra partner och kunder har vi gjort dessa justeringar och material för att påskynda den här digitala omvandlingen:</span><span class="sxs-lookup"><span data-stu-id="86528-214">To help ensure a smooth transition for both our partners and customers, we’ve made these adjustments and materials to accelerate this digital transformation:</span></span>

#### <a name="april-2021"></a><span data-ttu-id="86528-215">April 2021</span><span class="sxs-lookup"><span data-stu-id="86528-215">April 2021</span></span>

<span data-ttu-id="86528-216">[Nu tillgängligt:](https://partner.microsoft.com/resources/collection/reseller-open-license-to-csp-transition-materials#/)Open License-to-CSP transition materials for resellers (Öppna licens-till-CSP-övergångsmaterial för återförsäljare)</span><span class="sxs-lookup"><span data-stu-id="86528-216">[Now available](https://partner.microsoft.com/resources/collection/reseller-open-license-to-csp-transition-materials#/): Open License-to-CSP transition materials for resellers</span></span>

#### <a name="july-2021"></a><span data-ttu-id="86528-217">Juli 2021</span><span class="sxs-lookup"><span data-stu-id="86528-217">July 2021</span></span>

##### <a name="csp"></a><span data-ttu-id="86528-218">CSP</span><span class="sxs-lookup"><span data-stu-id="86528-218">CSP</span></span>

- <span data-ttu-id="86528-219">1 juli: Permanent programvarulicenser är tillgängliga för kunder inom den offentliga sektorn</span><span class="sxs-lookup"><span data-stu-id="86528-219">July 1: Perpetual software licenses available to public sector customers</span></span>

- <span data-ttu-id="86528-220">7 juli: Visual Studio Pro och Skaffa äkta Windows-avtal för beständiga programvarulicenser som är tillgängliga för alla segment</span><span class="sxs-lookup"><span data-stu-id="86528-220">July 7: Visual Studio Pro and Get Genuine Windows Agreement  perpetual software licenses available to all segments</span></span>

##### <a name="open-value"></a><span data-ttu-id="86528-221">Öppet värde</span><span class="sxs-lookup"><span data-stu-id="86528-221">Open Value</span></span>

- <span data-ttu-id="86528-222">1 juli: Ytterligare SKU:er är tillgängliga i Open Value-programmet för utbildning och ideell verksamhet, vilket ger liknande erbjudanden som Open License-programmet</span><span class="sxs-lookup"><span data-stu-id="86528-222">July 1: Additional SKUs available in the Open Value program for education and nonprofit, providing similar offers to the Open License program</span></span>

##### <a name="open-license"></a><span data-ttu-id="86528-223">Öppna licens</span><span class="sxs-lookup"><span data-stu-id="86528-223">Open License</span></span>

- <span data-ttu-id="86528-224">1 juli: Microsoft kommer inte längre att lansera nya erbjudanden i Open License-programmet.</span><span class="sxs-lookup"><span data-stu-id="86528-224">July 1: Microsoft will no longer launch new offers in the Open License program.</span></span>

#### <a name="january-2022"></a><span data-ttu-id="86528-225">Januari 2022</span><span class="sxs-lookup"><span data-stu-id="86528-225">January 2022</span></span>

- <span data-ttu-id="86528-226">1 januari: Inga nya köp eller förnyelser kan göras via Open License-programmet</span><span class="sxs-lookup"><span data-stu-id="86528-226">January 1: No new purchases or renewals can be made through the Open License program</span></span>

### <a name="next-steps"></a><span data-ttu-id="86528-227">Nästa steg</span><span class="sxs-lookup"><span data-stu-id="86528-227">Next steps</span></span>

#### <a name="csp-indirect-providers"></a><span data-ttu-id="86528-228">Indirekta CSP-leverantörer</span><span class="sxs-lookup"><span data-stu-id="86528-228">CSP indirect providers</span></span>

<span data-ttu-id="86528-229">Använd de kommande månaderna för att hjälpa Open License-återförsäljare att orientera sig i CSP-programmet genom att delta i partner-community-evenemang och använda övergångsmaterial för öppen licens till CSP för återförsäljare:</span><span class="sxs-lookup"><span data-stu-id="86528-229">Use the coming months to help Open License resellers orient into the CSP program by attending partner community events and using the Open License-to-CSP transition materials for resellers:</span></span>

- <span data-ttu-id="86528-230">[Open License-to-CSP](https://partner.microsoft.com/resources/collection/reseller-open-license-to-csp-transition-materials#/)transition materials for resellers –Customizable overview presentation, email template, CSP indirect reseller onboarding guide, and more to help you drive the adoption for your resellers at scale.</span><span class="sxs-lookup"><span data-stu-id="86528-230">[Open License-to-CSP transition materials for resellers](https://partner.microsoft.com/resources/collection/reseller-open-license-to-csp-transition-materials#/)—Customizable overview presentation, email template, CSP indirect reseller onboarding guide, and more to help you drive the adoption for your resellers at scale.</span></span>

- <span data-ttu-id="86528-231">[CSP Partner Community Events](https://globalpbocomm.eventbuilder.com/GlobalCSP) som värdar för Microsoft Business Operations.</span><span class="sxs-lookup"><span data-stu-id="86528-231">[CSP Partner Community Events](https://globalpbocomm.eventbuilder.com/GlobalCSP) hosted by Microsoft Business Operations.</span></span>  <span data-ttu-id="86528-232">Delta i de olika sessionerna för att lära dig grunderna i CSP (CSP Fundamentals) eller håll dig uppdaterad och ställ frågor om programvara i CSP (Q&A Sessions).</span><span class="sxs-lookup"><span data-stu-id="86528-232">Join the various sessions to learn CSP basics (CSP Fundamentals) or stay up to date, and ask questions regarding Software in CSP (Q&A Sessions).</span></span>

- <span data-ttu-id="86528-233">(Kommer snart) Utbildningssession som fokuserar på indirekt CSP-återförsäljare som värd för Microsoft Business Operations.</span><span class="sxs-lookup"><span data-stu-id="86528-233">(Coming soon) CSP indirect reseller–focused training session hosted by Microsoft Business Operations.</span></span>

#### <a name="open-license-resellers"></a><span data-ttu-id="86528-234">Open License-återförsäljare</span><span class="sxs-lookup"><span data-stu-id="86528-234">Open License resellers</span></span>

- <span data-ttu-id="86528-235">Om din organisation inte är registrerad i CSP-programmet kontaktar du återförsäljaren för information om hur du kommer igång.</span><span class="sxs-lookup"><span data-stu-id="86528-235">If your organization isn’t currently enrolled in the CSP program, contact your distributor for information on how to get started.</span></span> <span data-ttu-id="86528-236">Anslut med en indirekt leverantör [här.](https://partner.microsoft.com/membership/cloud-solution-provider/find-a-provider)</span><span class="sxs-lookup"><span data-stu-id="86528-236">Connect with an indirect provider [here](https://partner.microsoft.com/membership/cloud-solution-provider/find-a-provider).</span></span>

- <span data-ttu-id="86528-237">Om din organisation redan har registrerats i CSP-programmet kan du läsa mer om permanent programvara i CSP [här.](https://partner.microsoft.com/resources/collection/software-in-csp)</span><span class="sxs-lookup"><span data-stu-id="86528-237">If your organization is already enrolled in the CSP program, learn more about perpetual software in CSP [here](https://partner.microsoft.com/resources/collection/software-in-csp).</span></span>

### <a name="questions"></a><span data-ttu-id="86528-238">Har du några frågor?</span><span class="sxs-lookup"><span data-stu-id="86528-238">Questions?</span></span>

<span data-ttu-id="86528-239">Mer information om dessa erbjudanden finns i dina relevanta Yammer-communities.</span><span class="sxs-lookup"><span data-stu-id="86528-239">For further questions about these offers, check your relevant Yammer communities.</span></span>

________________
## <a name="now-live-global-promo-readiness-guide"></a><a name="6"></a><span data-ttu-id="86528-240">Nu live: Guide för global kampanjberedskap</span><span class="sxs-lookup"><span data-stu-id="86528-240">Now live: Global promo readiness guide</span></span>

### <a name="categories"></a><span data-ttu-id="86528-241">Kategorier</span><span class="sxs-lookup"><span data-stu-id="86528-241">Categories</span></span>

- <span data-ttu-id="86528-242">Datum: 2021-04-16</span><span class="sxs-lookup"><span data-stu-id="86528-242">Date: 2021-04-16</span></span>
- <span data-ttu-id="86528-243">Funktioner</span><span class="sxs-lookup"><span data-stu-id="86528-243">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="86528-244">Sammanfattning</span><span class="sxs-lookup"><span data-stu-id="86528-244">Summary</span></span>

<span data-ttu-id="86528-245">Launch Readiness har publicerat en ny [global kampanjberedskapsguide](https://partner.microsoft.com/resources/detail/operations-promo-guide-pdf) i resursgalleriet för driftberedskap.</span><span class="sxs-lookup"><span data-stu-id="86528-245">Launch Readiness has published a new [global promo readiness guide](https://partner.microsoft.com/resources/detail/operations-promo-guide-pdf) on the Operations Readiness resource gallery.</span></span> <span data-ttu-id="86528-246">Den här guiden innehåller en samlad vy över alla aktiva [globala kampanjer.](https://partner.microsoft.com/resources/collection/global-promo-readiness-guide-collection#/)</span><span class="sxs-lookup"><span data-stu-id="86528-246">This guide provides a consolidated view of all active [global promotions](https://partner.microsoft.com/resources/collection/global-promo-readiness-guide-collection#/).</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="86528-247">Målgrupp som påverkas</span><span class="sxs-lookup"><span data-stu-id="86528-247">Impacted audience</span></span>

<span data-ttu-id="86528-248">Alla partner för volymlicensiering (VL), Dynamics Price List (DPL) Molnlösningsleverantör (CSP)</span><span class="sxs-lookup"><span data-stu-id="86528-248">All Volume Licensing (VL), Dynamics Price List (DPL), and Cloud Solution Provider (CSP) partners</span></span>

### <a name="details"></a><span data-ttu-id="86528-249">Information</span><span class="sxs-lookup"><span data-stu-id="86528-249">Details</span></span>

<span data-ttu-id="86528-250">Microsoft-partner har delat med oss om behovet av att tillhandahålla en samlad vy över alla globala kampanjer med kompletterande information.</span><span class="sxs-lookup"><span data-stu-id="86528-250">Microsoft partners have shared with us the need to provide a consolidated view of all global promotions with supporting details.</span></span> <span data-ttu-id="86528-251">Du ville ha den här konsoliderade guiden för att hjälpa dig att använda kampanjer med tillförsikt att all tillgänglig information är lättillgänglig på en central och praktisk plats.</span><span class="sxs-lookup"><span data-stu-id="86528-251">You wanted this consolidated guide to help you use promotions with the confidence that all the available information will be readily accessible in a central and convenient location.</span></span>

<span data-ttu-id="86528-252">Från och med april 2021 uppdaterar Microsoft den här guiden månadsvis och den kommer att vara tillgänglig i en dedikerad samling global kampanjberedskapsguide i resursgalleriet för operationsberedskap.</span><span class="sxs-lookup"><span data-stu-id="86528-252">Beginning in April 2021, Microsoft will update this guide on a monthly basis, and it will be available in a dedicated Global Promo Readiness Guide collection in the Operations Readiness resource gallery.</span></span>

<span data-ttu-id="86528-253">Länkar till den här guiden kommer också att ingå i följande samlingar:</span><span class="sxs-lookup"><span data-stu-id="86528-253">Links to this guide will also be included in the following collections:</span></span>

- <span data-ttu-id="86528-254">[Starta kalendersamlingen](https://partner.microsoft.com/resources/collection/csp-announcement-calendar#/), som ger en centraliserad vy över kommande ändringar och uppskjutningar.</span><span class="sxs-lookup"><span data-stu-id="86528-254">[Launch calendar collection](https://partner.microsoft.com/resources/collection/csp-announcement-calendar#/), which provides a centralized view of upcoming changes and launches.</span></span>

- <span data-ttu-id="86528-255">[Community-samlingar](https://partner.microsoft.com/resources/collection/april-2021-csp-partner-community-content#/), som innehåller stödmaterial för våra månatliga partnersamtal, med fokus på kommande ändringar och aktuella ämnen av driftsmässiga intresse.</span><span class="sxs-lookup"><span data-stu-id="86528-255">[Community collections](https://partner.microsoft.com/resources/collection/april-2021-csp-partner-community-content#/), which contain supporting materials for our monthly partner calls, highlighting upcoming changes and timely topics of operational interest.</span></span>

- <span data-ttu-id="86528-256">[Nyhetsbrev för partner,](https://partner.microsoft.com/resources/collection/csp-monthly-update#/)till exempel månadsuppdatering för CSP</span><span class="sxs-lookup"><span data-stu-id="86528-256">[Partner newsletters](https://partner.microsoft.com/resources/collection/csp-monthly-update#/), such as CSP Monthly Update</span></span>

<span data-ttu-id="86528-257">Som en månatlig påminnelse kommer vi också att publicera ett Partnercenter-meddelande med varje nytt ärende i guiden för global kampanjberedskap.</span><span class="sxs-lookup"><span data-stu-id="86528-257">As a monthly reminder, we will also publish a Partner Center announcement with each new issue of the global promo readiness guide.</span></span>

### <a name="next-steps"></a><span data-ttu-id="86528-258">Nästa steg</span><span class="sxs-lookup"><span data-stu-id="86528-258">Next steps</span></span>

<span data-ttu-id="86528-259">I början av varje månad hittar du den senaste guiden för global [kampanjberedskap](https://partner.microsoft.com/resources/detail/operations-promo-guide-pdf) i [resursgalleriet för driftberedskap.](https://partner.microsoft.com/resources)</span><span class="sxs-lookup"><span data-stu-id="86528-259">At the start of each month, you will find the latest [global promo readiness guide](https://partner.microsoft.com/resources/detail/operations-promo-guide-pdf) in the [Operations Readiness resource gallery](https://partner.microsoft.com/resources).</span></span>

<span data-ttu-id="86528-260">Dela den här informationen med lämpliga kontakter i dina organisationer och berätta för oss hur användbar guiden är genom "Var den här sidan användbar?"</span><span class="sxs-lookup"><span data-stu-id="86528-260">Share this information with the appropriate contacts in your organizations and let us know how helpful the guide is through the “Was this page helpful?”</span></span> <span data-ttu-id="86528-261">i slutet av varje sida.</span><span class="sxs-lookup"><span data-stu-id="86528-261">button at the end of each page.</span></span>

________________
## <a name="april-cloud-solution-provider-csp-community-update-and-reminders"></a><a name="5"></a><span data-ttu-id="86528-262">Community-Molnlösningsleverantör april Molnlösningsleverantör (CSP) och påminnelser</span><span class="sxs-lookup"><span data-stu-id="86528-262">April Cloud Solution Provider (CSP) community update and reminders</span></span>

### <a name="categories"></a><span data-ttu-id="86528-263">Kategorier</span><span class="sxs-lookup"><span data-stu-id="86528-263">Categories</span></span>

- <span data-ttu-id="86528-264">Datum: 2021-04-16</span><span class="sxs-lookup"><span data-stu-id="86528-264">Date: 2021-04-16</span></span>
- <span data-ttu-id="86528-265">Community-| Inbjudningar och påminnelser</span><span class="sxs-lookup"><span data-stu-id="86528-265">Community | Invites and reminders</span></span>

### <a name="summary"></a><span data-ttu-id="86528-266">Sammanfattning</span><span class="sxs-lookup"><span data-stu-id="86528-266">Summary</span></span>

<span data-ttu-id="86528-267">CSP community-resurser är tillgängliga på begäran och uppdateras varje månad för att hålla dig informerad och förberedd för ändringar i CSP-programmet.</span><span class="sxs-lookup"><span data-stu-id="86528-267">CSP community resources are available on demand and updated monthly to keep you informed and prepared for change in the CSP program.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="86528-268">Påverkad målgrupp</span><span class="sxs-lookup"><span data-stu-id="86528-268">Impacted audience</span></span>

<span data-ttu-id="86528-269">CSP-direktfaktureringspartner och indirekta leverantörer</span><span class="sxs-lookup"><span data-stu-id="86528-269">CSP direct bill partners and indirect providers</span></span>

### <a name="details"></a><span data-ttu-id="86528-270">Information</span><span class="sxs-lookup"><span data-stu-id="86528-270">Details</span></span>

<span data-ttu-id="86528-271">Den här månaden innehåller resurserna följande viktiga avsnitt:</span><span class="sxs-lookup"><span data-stu-id="86528-271">This month, the resources include the following key topics:</span></span>

- [<span data-ttu-id="86528-272">Uppdatering av CSP-programutveckling och ändringar i Open License-programmet</span><span class="sxs-lookup"><span data-stu-id="86528-272">Update to CSP program evolution and Open License program changes</span></span>](https://partner.microsoft.com/resources/collection/csp-open-evolution-to-a-better-experience#/)

- [<span data-ttu-id="86528-273">Ändringar av CSP-kundernas registreringskrav i vissa regioner</span><span class="sxs-lookup"><span data-stu-id="86528-273">Changes to CSP customer onboarding requirements in certain regions</span></span>](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/)

- [<span data-ttu-id="86528-274">Nytt format för den nya PDF-fakturan för handel i CSP-programmet</span><span class="sxs-lookup"><span data-stu-id="86528-274">New format for the new commerce PDF invoice in the CSP program</span></span>](https://partner.microsoft.com/resources/collection/introducing-new-format-for-the-new-commerce-invoice-in-csp#/)

<span data-ttu-id="86528-275">I [CSP-communitysamlingen](https://partner.microsoft.com/resources/collection/april-2021-csp-partner-community-content#/)hittar du:</span><span class="sxs-lookup"><span data-stu-id="86528-275">Within the [CSP community collection](https://partner.microsoft.com/resources/collection/april-2021-csp-partner-community-content#/), you’ll find:</span></span>

- <span data-ttu-id="86528-276">Det nedladdningsbara [nyhetsbrevet CSP Monthly Update](https://partner.microsoft.com/resources/detail/csp-monthly-update-april-2021-global), som sammanställer de senaste CSP-meddelandena, uppdateringarna, händelserna och påminnelserna i ett lättläst dokument.</span><span class="sxs-lookup"><span data-stu-id="86528-276">The downloadable [CSP Monthly Update newsletter](https://partner.microsoft.com/resources/detail/csp-monthly-update-april-2021-global), which aggregates recent CSP announcements, updates, events, and reminders in an easy-to-read document.</span></span>

- <span data-ttu-id="86528-277">[CSP-meddelandekalendern](https://partner.microsoft.com/resources/detail/csp-announcement-calendar-april-2021), som ger en tidslinjevy över kommande ändringar som påverkar programmet.</span><span class="sxs-lookup"><span data-stu-id="86528-277">The [CSP Announcement Calendar](https://partner.microsoft.com/resources/detail/csp-announcement-calendar-april-2021), which provides a timeline view of upcoming changes affecting the program.</span></span>

- <span data-ttu-id="86528-278">Den nya [kalendern för produktlansering,](https://partner.microsoft.com/resources/detail/product-launch-calendar-april-pdf)där du kan se kommande produktlanseringar och erbjudanden.</span><span class="sxs-lookup"><span data-stu-id="86528-278">The new [product launch calendar](https://partner.microsoft.com/resources/detail/product-launch-calendar-april-pdf), where you can view upcoming product launches and offers.</span></span>

- <span data-ttu-id="86528-279">[CSP startar uppdateringsresurser](https://partner.microsoft.com/resources/collection/april-2021-csp-launch-topics-collection#/) med lätt att använda innehåll om viktiga operativa ändringar.</span><span class="sxs-lookup"><span data-stu-id="86528-279">[CSP launch update resources](https://partner.microsoft.com/resources/collection/april-2021-csp-launch-topics-collection#/) with easy-to-consume content on key operational changes.</span></span>

- <span data-ttu-id="86528-280">[Uppdaterare och påminnelser om](https://partner.microsoft.com/resources/detail/csp-april-2021-refreshers-and-reminders-pdf) viktiga CSP-ämnen som tar emot intresse och frågor.</span><span class="sxs-lookup"><span data-stu-id="86528-280">[Refreshers and reminders](https://partner.microsoft.com/resources/detail/csp-april-2021-refreshers-and-reminders-pdf) on key CSP topics receiving interest and queries.</span></span>

#### <a name="csp-community-call-qas"></a><span data-ttu-id="86528-281">CSP Community Call Q&As</span><span class="sxs-lookup"><span data-stu-id="86528-281">CSP Community Call Q&As</span></span>

<span data-ttu-id="86528-282">Community Call Q&As are available to help you with questions related to upcoming changes.</span><span class="sxs-lookup"><span data-stu-id="86528-282">Community Call Q&As are available to help you with questions related to upcoming changes.</span></span> <span data-ttu-id="86528-283">Registrera dig nu för CSP Community Call Q&As som äger rum i april, maj och juni.</span><span class="sxs-lookup"><span data-stu-id="86528-283">Register now for CSP Community Call Q&As that are taking place in April, May, and June.</span></span> <span data-ttu-id="86528-284">Dessa fokuserar på de senaste uppskjutningar, viktiga uppdateringar och påminnelser.</span><span class="sxs-lookup"><span data-stu-id="86528-284">These will focus on the latest launches, important refreshers, and reminders.</span></span>

<span data-ttu-id="86528-285">[Registrera dig här.](https://globalpbocomm.eventbuilder.com/GlobalCSP)</span><span class="sxs-lookup"><span data-stu-id="86528-285">[Register here](https://globalpbocomm.eventbuilder.com/GlobalCSP).</span></span>

### <a name="next-steps"></a><span data-ttu-id="86528-286">Nästa steg</span><span class="sxs-lookup"><span data-stu-id="86528-286">Next steps</span></span>

<span data-ttu-id="86528-287">Granska communityresurserna och registrera dig för Community Call Q&A.</span><span class="sxs-lookup"><span data-stu-id="86528-287">Review the community resources and register for the Community Call Q&A.</span></span>

<span data-ttu-id="86528-288">För att säkerställa att du får ut mesta av Community Call Q&A granskar du communityinnehållet på begäran och skickar dina frågor upp till 48 timmar före samtalet.</span><span class="sxs-lookup"><span data-stu-id="86528-288">To ensure that you get the most from the Community Call Q&A, review the on-demand community content and submit your questions up to 48 hours before the call.</span></span>

### <a name="questions"></a><span data-ttu-id="86528-289">Har du några frågor?</span><span class="sxs-lookup"><span data-stu-id="86528-289">Questions?</span></span>

<span data-ttu-id="86528-290">Det månatliga CSP Community Call Q&A är den bästa platsen för frågor som rör ändringar i CSP-programmet.</span><span class="sxs-lookup"><span data-stu-id="86528-290">The monthly CSP Community Call Q&A is the best place for questions related to changes in the CSP program.</span></span> <span data-ttu-id="86528-291">Granska materialet varje månad och skicka dina frågor i förväg så att vi kan ägna sessionen åt de ämnen som är viktigast för dig.</span><span class="sxs-lookup"><span data-stu-id="86528-291">Each month, review the material and submit your questions in advance so that we can spend the session on the topics that are most important to you.</span></span>

<span data-ttu-id="86528-292">Kontakta supporten för [mer information.](https://partner.microsoft.com/dashboard/support/csp/servicerequests/create?category=csp)</span><span class="sxs-lookup"><span data-stu-id="86528-292">For more information, contact [Support](https://partner.microsoft.com/dashboard/support/csp/servicerequests/create?category=csp).</span></span>

________________
## <a name="reminder-deprecation-of-get-qualification-on-may-4-2021"></a><a name="4"></a><span data-ttu-id="86528-293">Påminnelse: Utfasning av GET-kvalificering den 4 maj 2021</span><span class="sxs-lookup"><span data-stu-id="86528-293">Reminder: Deprecation of GET qualification on May 4, 2021</span></span>

### <a name="categories"></a><span data-ttu-id="86528-294">Kategorier</span><span class="sxs-lookup"><span data-stu-id="86528-294">Categories</span></span>

- <span data-ttu-id="86528-295">Datum: 2021-04-09</span><span class="sxs-lookup"><span data-stu-id="86528-295">Date: 2021-04-09</span></span>
- <span data-ttu-id="86528-296">Funktioner</span><span class="sxs-lookup"><span data-stu-id="86528-296">Capabilities</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="86528-297">Målgrupp som påverkas</span><span class="sxs-lookup"><span data-stu-id="86528-297">Impacted audience</span></span>

<span data-ttu-id="86528-298">Partner som säljer erbjudandena Academic, Nonprofit och Government Community Cloud (GCC) via Molnlösningsleverantör med partnercenter-API:et</span><span class="sxs-lookup"><span data-stu-id="86528-298">Partners selling Academic, Nonprofit, and Government Community Cloud (GCC) offers through the Cloud Solution Provider program using the Partner Center API</span></span>

### <a name="details"></a><span data-ttu-id="86528-299">Information</span><span class="sxs-lookup"><span data-stu-id="86528-299">Details</span></span>

<span data-ttu-id="86528-300">Det här meddelandet är en uppföljning av förbättringarna i Partnercenter [som släpptes i december.](https://docs.microsoft.com/partner-center/announcements/2020-december#1)</span><span class="sxs-lookup"><span data-stu-id="86528-300">This announcement is a follow-up to the Partner Center [enhancements released in December](https://docs.microsoft.com/partner-center/announcements/2020-december#1).</span></span> <span data-ttu-id="86528-301">Som en del av den versionen distribuerades nya GET- och POST-kvalificerings-API:er och därför kommer den befintliga GET-kvalificeringen att dras tillbaka den 4 maj 2021.</span><span class="sxs-lookup"><span data-stu-id="86528-301">As part of that release, new GET and POST Qualifications APIs were deployed and, as a result, the existing GET qualification will be retired by May 4, 2021.</span></span> <span data-ttu-id="86528-302">Då måste du ha gått över till att använda de nya API:erna för POST Partner Center i inköpserbjudanden för Education och det nya GET-api:et för kvalificering för att köpa förkvalificerade erbjudanden för ideella organisationer och GCC.</span><span class="sxs-lookup"><span data-stu-id="86528-302">By that time, you’ll need to have transitioned to using the new POST Partner Center APIs in purchase Education offers, and the new GET qualifications API to purchase prequalified Nonprofit and GCC offers.</span></span>

### <a name="next-steps"></a><span data-ttu-id="86528-303">Nästa steg</span><span class="sxs-lookup"><span data-stu-id="86528-303">Next steps</span></span>

- <span data-ttu-id="86528-304">Uppdatera till de nya API:erna för en lyckad övergång i rätt tid.</span><span class="sxs-lookup"><span data-stu-id="86528-304">Update to the new APIs for a successful and timely transition.</span></span>

- <span data-ttu-id="86528-305">Granska de nya partnercenter-API-ändringarna och guiden i resurserna för driftberedskap: Förbättringar av [kundvalideringsprocessen](https://partner.microsoft.com/resources/collection/partner-center-edu-validation-enhancements#/)i Partner Center Education.</span><span class="sxs-lookup"><span data-stu-id="86528-305">Review the new Partner Center API changes and Guide in the Operations Readiness resources: [Partner Center Education customer validation process enhancements](https://partner.microsoft.com/resources/collection/partner-center-edu-validation-enhancements#/).</span></span>

- <span data-ttu-id="86528-306">Dela den här informationen med lämpliga team i din organisation och med dina återförsäljare för att hjälpa dem att förbereda sig för dessa ändringar.</span><span class="sxs-lookup"><span data-stu-id="86528-306">Share this information with the appropriate teams within your organization and with your resellers to help them prepare for these changes.</span></span>

### <a name="questions"></a><span data-ttu-id="86528-307">Har du några frågor?</span><span class="sxs-lookup"><span data-stu-id="86528-307">Questions?</span></span>

<span data-ttu-id="86528-308">Om du har frågor om det här meddelandet kontaktar du [supporten för Partnercenter.](https://partner.microsoft.com/dashboard/support/referrals/servicerequests?category=referrals)</span><span class="sxs-lookup"><span data-stu-id="86528-308">For any questions related to this notification, contact [Partner Center support](https://partner.microsoft.com/dashboard/support/referrals/servicerequests?category=referrals).</span></span>

### <a name="change-log"></a><span data-ttu-id="86528-309">Ändringslogg</span><span class="sxs-lookup"><span data-stu-id="86528-309">Change log</span></span>

- <span data-ttu-id="86528-310">April: Påminnelse om kommande utfasning av GET-kvalificering</span><span class="sxs-lookup"><span data-stu-id="86528-310">April: Reminder of upcoming deprecation of GET qualification</span></span> 
- <span data-ttu-id="86528-311">Februari: Uppdaterade tidslinjer för utfasning av GET & PUT-kvalificeringar</span><span class="sxs-lookup"><span data-stu-id="86528-311">February: Updated timelines for deprecation of GET & PUT qualifications</span></span>
- <span data-ttu-id="86528-312">Januari: Påminnelse om kommande utfasningar av GET & PUT-utbildning</span><span class="sxs-lookup"><span data-stu-id="86528-312">January: Reminder of upcoming deprecations of GET & PUT qualifications</span></span>

________________
## <a name="new-format-for-the-new-commerce-pdf-invoice-in-csp"></a><a name="3"></a><span data-ttu-id="86528-313">Nytt format för den nya PDF-fakturan för handel i CSP</span><span class="sxs-lookup"><span data-stu-id="86528-313">New format for the new commerce PDF invoice in CSP</span></span>

### <a name="categories"></a><span data-ttu-id="86528-314">Kategorier</span><span class="sxs-lookup"><span data-stu-id="86528-314">Categories</span></span>

- <span data-ttu-id="86528-315">Datum: 2021-04-05</span><span class="sxs-lookup"><span data-stu-id="86528-315">Date: 2021-04-05</span></span>
- <span data-ttu-id="86528-316">Funktioner</span><span class="sxs-lookup"><span data-stu-id="86528-316">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="86528-317">Sammanfattning</span><span class="sxs-lookup"><span data-stu-id="86528-317">Summary</span></span>

<span data-ttu-id="86528-318">Microsoft introducerar ett nytt format för den nya PDF-fakturan för handel i Molnlösningsleverantör-programmet (CSP) för att visa faktureringsinformation efter produktinformation i stället för SKU-beskrivning.</span><span class="sxs-lookup"><span data-stu-id="86528-318">Microsoft is introducing a new format for the new commerce PDF invoice in the Cloud Solution Provider (CSP) program to display billing details by product detail instead of SKU description.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="86528-319">Påverkad målgrupp</span><span class="sxs-lookup"><span data-stu-id="86528-319">Impacted audience</span></span>

<span data-ttu-id="86528-320">Partner som gör en överträdelse via CSP-programmet</span><span class="sxs-lookup"><span data-stu-id="86528-320">Partners transacting through the CSP program</span></span>

### <a name="details"></a><span data-ttu-id="86528-321">Information</span><span class="sxs-lookup"><span data-stu-id="86528-321">Details</span></span>

<span data-ttu-id="86528-322">Från och med maj 2021 introducerar Microsoft ett nytt format för den nya PDF-fakturan för handel i CSP-programmet för att visa faktureringsinformation efter produktinformation i stället för SKU-beskrivning.</span><span class="sxs-lookup"><span data-stu-id="86528-322">Starting May 2021, Microsoft is introducing a new format for the new commerce PDF invoice in the CSP program to display billing details by product detail instead of SKU description.</span></span> <span data-ttu-id="86528-323">Med den här nya uppdateringen kommer vi att aggregera radobjekten efter produkttyp samtidigt som vi visar varje produkt på en enskild rad.</span><span class="sxs-lookup"><span data-stu-id="86528-323">With this new update, we will be aggregating the line items by product type while displaying every product on an individual line.</span></span>

<span data-ttu-id="86528-324">Partner kommer att märka att ändringen börjar gälla på fakturan för faktureringsperioden mellan 1 april 2021 och 30 april 2021.</span><span class="sxs-lookup"><span data-stu-id="86528-324">Partners will notice this change coming into effect in their May invoice for the billing period between April 1, 2021 and April 30, 2021.</span></span> <span data-ttu-id="86528-325">De berörda erbjudandena är Microsoft Azure Reserverad instans, Azure-prenumerationer (Azure-plan) och Marketplace.</span><span class="sxs-lookup"><span data-stu-id="86528-325">The affected offers are Microsoft Azure Reserved Instance, Azure subscriptions (Azure plan), and Marketplace.</span></span>

<span data-ttu-id="86528-326">Eventuella begäranden om kreditrefakturering som görs efter att fakturaformatet har uppdaterats genereras i det nya formatet.</span><span class="sxs-lookup"><span data-stu-id="86528-326">Any credit-rebill requests made after the invoice format has been updated will be generated in the new format.</span></span>

#### <a name="partner-benefits"></a><span data-ttu-id="86528-327">Partnerförmåner</span><span class="sxs-lookup"><span data-stu-id="86528-327">Partner benefits</span></span>

<span data-ttu-id="86528-328">Den här uppdateringen kommer att erbjuda följande förbättringar av faktureringsupplevelsen för partner:</span><span class="sxs-lookup"><span data-stu-id="86528-328">This update will offer the following improvements to the invoicing experience for partners:</span></span>

- <span data-ttu-id="86528-329">Minskad fakturastorlek samtidigt som kritiska data bevaras</span><span class="sxs-lookup"><span data-stu-id="86528-329">Reduced invoice size while retaining critical data</span></span>

- <span data-ttu-id="86528-330">Anpassning av formatet till branschstandarderna för kompakta och användarvänliga fakturor</span><span class="sxs-lookup"><span data-stu-id="86528-330">Alignment of the format to the industry standards for compact and user-friendly invoices</span></span> 

<span data-ttu-id="86528-331">Följande element påverkas inte:</span><span class="sxs-lookup"><span data-stu-id="86528-331">The following elements will not be affected:</span></span>

- <span data-ttu-id="86528-332">Sidan Med faktureringssammanfattning på PDF-fakturan</span><span class="sxs-lookup"><span data-stu-id="86528-332">Billing summary page on the invoice PDF</span></span>

- <span data-ttu-id="86528-333">Befintliga fakturerings-API:er</span><span class="sxs-lookup"><span data-stu-id="86528-333">Existing invoicing APIs</span></span>

- <span data-ttu-id="86528-334">Avstämningsfiler (rekognoseringsfiler kan användas för att hämta detaljerade data.)</span><span class="sxs-lookup"><span data-stu-id="86528-334">Reconciliation files (Recon files can be used for retrieving granular data.)</span></span> 

- <span data-ttu-id="86528-335">Fakturor för användnings- och licensbaserade avgifter</span><span class="sxs-lookup"><span data-stu-id="86528-335">Usage and license-based charges invoices</span></span>

### <a name="next-steps"></a><span data-ttu-id="86528-336">Nästa steg</span><span class="sxs-lookup"><span data-stu-id="86528-336">Next steps</span></span>

<span data-ttu-id="86528-337">Granska informationen om det här avsnittet i [resursgalleriet för driftberedskap](https://partner.microsoft.com/resources/collection/introducing-new-format-for-the-new-commerce-invoice-in-csp#/) på Microsofts partnerwebbplats.</span><span class="sxs-lookup"><span data-stu-id="86528-337">Review the information about this topic in the [Operations Readiness resource gallery](https://partner.microsoft.com/resources/collection/introducing-new-format-for-the-new-commerce-invoice-in-csp#/) on the Microsoft partner website.</span></span> <span data-ttu-id="86528-338">Mer information om fakturerings- och skatteämnen som faktureringsresurser, fakturor, CSP-fakturering och skatter finns i [avsnittet Fakturering](https://docs.microsoft.com/partner-center/billing) i Partnercenter.</span><span class="sxs-lookup"><span data-stu-id="86528-338">For more information about billing and tax topics including billing resources, invoices, CSP billing, and taxes, visit the [Billing section](https://docs.microsoft.com/partner-center/billing) in Partner Center.</span></span>

________________
## <a name="changes-to-the-cloud-solution-provider-csp-customer-onboarding-requirements"></a><a name="2"></a><span data-ttu-id="86528-339">Ändringar i CSP Molnlösningsleverantör-kundernas registreringskrav</span><span class="sxs-lookup"><span data-stu-id="86528-339">Changes to the Cloud Solution Provider (CSP) customer onboarding requirements</span></span>

### <a name="categories"></a><span data-ttu-id="86528-340">Kategorier</span><span class="sxs-lookup"><span data-stu-id="86528-340">Categories</span></span>

- <span data-ttu-id="86528-341">Datum: 2021-04-02</span><span class="sxs-lookup"><span data-stu-id="86528-341">Date: 2021-04-02</span></span>
- <span data-ttu-id="86528-342">Erbjudanden/marknader</span><span class="sxs-lookup"><span data-stu-id="86528-342">Offers/Markets</span></span>

### <a name="summary"></a><span data-ttu-id="86528-343">Sammanfattning</span><span class="sxs-lookup"><span data-stu-id="86528-343">Summary</span></span>

<span data-ttu-id="86528-344">Som en del av vårt åtagande att hjälpa partner och kunder att driva sin verksamhet baserat på förtroende begär vi ytterligare kundinformation från och med den 25 mars 2021.</span><span class="sxs-lookup"><span data-stu-id="86528-344">As part of our commitment to help partners and customers run their business based on trust, we will request additional customer information, effective March 25, 2021.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="86528-345">Målgrupp som påverkas</span><span class="sxs-lookup"><span data-stu-id="86528-345">Impacted audience</span></span>

<span data-ttu-id="86528-346">CSP-direktfaktureringspartner och indirekta leverantörer som har nya eller befintliga kunder i de länder som anges i nästa avsnitt</span><span class="sxs-lookup"><span data-stu-id="86528-346">CSP direct bill partners and indirect providers who have new or existing customers in the countries listed in the next section</span></span>

### <a name="details"></a><span data-ttu-id="86528-347">Information</span><span class="sxs-lookup"><span data-stu-id="86528-347">Details</span></span>

<span data-ttu-id="86528-348">Microsoft körs med förtroende.</span><span class="sxs-lookup"><span data-stu-id="86528-348">Microsoft runs on trust.</span></span> <span data-ttu-id="86528-349">Vi strävar efter att tillhandahålla en kompatibel, säker och säker metod för kundvalidering för att kunna göra kundprenumerationer i CSP-programmet.</span><span class="sxs-lookup"><span data-stu-id="86528-349">We’re committed to providing a compliant, safe, and secure method of customer validation for transacting customer subscriptions in the CSP program.</span></span> <span data-ttu-id="86528-350">Den 25 mars 2021 introducerar vi förbättringar av Partner Center API och användargränssnitt som påverkar partner som uppfyller båda följande kriterier:</span><span class="sxs-lookup"><span data-stu-id="86528-350">On March 25, 2021, we will be introducing Partner Center API and user interface (UI) enhancements that will affect partners who meet both of the following criteria:</span></span>

- <span data-ttu-id="86528-351">Partnern har en direkt faktureringsrelation med Microsoft (vilket innebär att partnern antingen är en partner för direktfakturering eller en indirekt leverantör).</span><span class="sxs-lookup"><span data-stu-id="86528-351">The partner has a direct billing relationship with Microsoft (which means that the partner is either a direct bill partner or an indirect provider).</span></span>

- <span data-ttu-id="86528-352">Partnern gör affärer med nya eller befintliga kunder i följande länder:</span><span class="sxs-lookup"><span data-stu-id="86528-352">The partner does business with new or existing customers in the following countries:</span></span>

    - <span data-ttu-id="86528-353">Thailand</span><span class="sxs-lookup"><span data-stu-id="86528-353">Thailand</span></span>
    - <span data-ttu-id="86528-354">Vietnam</span><span class="sxs-lookup"><span data-stu-id="86528-354">Vietnam</span></span>
    - <span data-ttu-id="86528-355">Turkiet</span><span class="sxs-lookup"><span data-stu-id="86528-355">Turkey</span></span>
    - <span data-ttu-id="86528-356">Polen</span><span class="sxs-lookup"><span data-stu-id="86528-356">Poland</span></span>
    - <span data-ttu-id="86528-357">Sydafrika</span><span class="sxs-lookup"><span data-stu-id="86528-357">South Africa</span></span>
    - <span data-ttu-id="86528-358">Indien</span><span class="sxs-lookup"><span data-stu-id="86528-358">India</span></span>
    - <span data-ttu-id="86528-359">Brasilien</span><span class="sxs-lookup"><span data-stu-id="86528-359">Brazil</span></span>
    - <span data-ttu-id="86528-360">Irak</span><span class="sxs-lookup"><span data-stu-id="86528-360">Iraq</span></span>
    - <span data-ttu-id="86528-361">Myanmar</span><span class="sxs-lookup"><span data-stu-id="86528-361">Myanmar</span></span>
    - <span data-ttu-id="86528-362">Sydsudan</span><span class="sxs-lookup"><span data-stu-id="86528-362">South Sudan</span></span>
    - <span data-ttu-id="86528-363">Saudiarabien</span><span class="sxs-lookup"><span data-stu-id="86528-363">Saudi Arabia</span></span>
    - <span data-ttu-id="86528-364">Förenade Arabemiraten</span><span class="sxs-lookup"><span data-stu-id="86528-364">United Arab Emirates</span></span>
    - <span data-ttu-id="86528-365">Venezuela</span><span class="sxs-lookup"><span data-stu-id="86528-365">Venezuela</span></span>

<span data-ttu-id="86528-366">Partner som uppfyller villkoren måste skicka en kunds företagsregistrerings-ID (kallas även kundens organisation INN) och telefonnummer nästa gång de uppdaterar eller skapar en prenumeration för kunden.</span><span class="sxs-lookup"><span data-stu-id="86528-366">Partners who meet the criteria will have to submit a customer's company registration ID (also known as the customer's organization INN) and phone number when they next update or create a subscription for that customer.</span></span> <span data-ttu-id="86528-367">Dessa partner kan också ange ett mellannamn för kunden (valfritt).</span><span class="sxs-lookup"><span data-stu-id="86528-367">These partners can also enter an optional middle name for the customer.</span></span>

<span data-ttu-id="86528-368">Observera att när du lägger till ditt företagsregistrerings-ID bör du använda ditt företagsskatte-ID och inte kundens personliga ID.</span><span class="sxs-lookup"><span data-stu-id="86528-368">Note that when you add your company registration ID you should use your business tax ID and not the customer personal ID.</span></span>

<span data-ttu-id="86528-369">Partner som gör affärer med nya eller befintliga kunder i följande länder har redan fått en tidigare version i november 2020.</span><span class="sxs-lookup"><span data-stu-id="86528-369">Partners who do business with new or existing customers in the following countries have already been onboarded with a previous release in November 2020.</span></span>

- <span data-ttu-id="86528-370">Armenien</span><span class="sxs-lookup"><span data-stu-id="86528-370">Armenia</span></span>
- <span data-ttu-id="86528-371">Azerbajdzjan</span><span class="sxs-lookup"><span data-stu-id="86528-371">Azerbaijan</span></span>
- <span data-ttu-id="86528-372">Vitryssland</span><span class="sxs-lookup"><span data-stu-id="86528-372">Belarus</span></span>
- <span data-ttu-id="86528-373">Ungern</span><span class="sxs-lookup"><span data-stu-id="86528-373">Hungary</span></span>
- <span data-ttu-id="86528-374">Kazakstan</span><span class="sxs-lookup"><span data-stu-id="86528-374">Kazakhstan</span></span>
- <span data-ttu-id="86528-375">Kirgizistan</span><span class="sxs-lookup"><span data-stu-id="86528-375">Kyrgyzstan</span></span>
- <span data-ttu-id="86528-376">Moldavien</span><span class="sxs-lookup"><span data-stu-id="86528-376">Moldova</span></span>
- <span data-ttu-id="86528-377">Ryssland</span><span class="sxs-lookup"><span data-stu-id="86528-377">Russia</span></span>
- <span data-ttu-id="86528-378">Tadzjikistan</span><span class="sxs-lookup"><span data-stu-id="86528-378">Tajikistan</span></span>
- <span data-ttu-id="86528-379">Ukraina</span><span class="sxs-lookup"><span data-stu-id="86528-379">Ukraine</span></span>
- <span data-ttu-id="86528-380">Uzbekistan</span><span class="sxs-lookup"><span data-stu-id="86528-380">Uzbekistan</span></span>

<span data-ttu-id="86528-381">Partner med kunder i resten av världen kommer att ha möjlighet i slutet av mars 2021 att ange företagets registrerings-ID, telefonnummer och mellannamn för kunder som valfri information.</span><span class="sxs-lookup"><span data-stu-id="86528-381">Partners with customers in the rest of the world will have the ability at the end of March 2021 to enter the company registration ID, phone number, and middle name for customers as optional details.</span></span>

### <a name="next-steps"></a><span data-ttu-id="86528-382">Nästa steg</span><span class="sxs-lookup"><span data-stu-id="86528-382">Next steps</span></span>

- <span data-ttu-id="86528-383">Mer detaljerad vägledning finns i den tekniska dokumentationen och vanliga frågor och svar [i](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/) den dedikerade partnersamlingen.</span><span class="sxs-lookup"><span data-stu-id="86528-383">Review the technical documentation and frequently asked questions in the dedicated [partner collection](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/) for more detailed guidance.</span></span>
- <span data-ttu-id="86528-384">Förbered för att införliva ändringarna med partnercenter-API:et och webbanvändarupplevelsen.</span><span class="sxs-lookup"><span data-stu-id="86528-384">Prepare to incorporate the changes using Partner Center API and web user experience.</span></span> <span data-ttu-id="86528-385">API/SDK:er kommer att vara tillgängliga för testning.</span><span class="sxs-lookup"><span data-stu-id="86528-385">API/SDKs will be available for testing.</span></span>
- <span data-ttu-id="86528-386">Se till att skicka in ytterligare data när du registrera nya kunder eller ändrar befintlig kundinformation.</span><span class="sxs-lookup"><span data-stu-id="86528-386">Make sure to submit the additional data when onboarding new customers or modifying existing customer details.</span></span>
- <span data-ttu-id="86528-387">Om du använder en CPV-lösning (Kontrollpanelens leverantör) kan du kontakta din CPV.</span><span class="sxs-lookup"><span data-stu-id="86528-387">If you’re using a control panel vendor (CPV) solution, consult your CPV.</span></span>

### <a name="questions"></a><span data-ttu-id="86528-388">Har du några frågor?</span><span class="sxs-lookup"><span data-stu-id="86528-388">Questions?</span></span>

<span data-ttu-id="86528-389">Kontakta skatterådgivaren eller det lokala skattekontoret om du har frågor som rör id:t för företagsregistrering (kallas även INN eller TIN).</span><span class="sxs-lookup"><span data-stu-id="86528-389">Contact your tax advisor or local tax office if you have any questions related to the company registration ID (also called INN or TIN).</span></span> <span data-ttu-id="86528-390">Microsoft kan inte ge vägledning om skattefrågor.</span><span class="sxs-lookup"><span data-stu-id="86528-390">Microsoft cannot provide guidance on tax matters.</span></span>

<span data-ttu-id="86528-391">Om du behöver support för dina åtgärder med Microsoft öppnar du en [tjänstbegäran.](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=aa679372-d996-73df-e244-cb28bbbf28e8)</span><span class="sxs-lookup"><span data-stu-id="86528-391">If you need support with your operations with Microsoft, open a [service request](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=aa679372-d996-73df-e244-cb28bbbf28e8).</span></span>

## <a name="view-this-months-product-launches-and-offers"></a><a name="1"></a><span data-ttu-id="86528-392">Visa den här månadens produktlanseringar och erbjudanden</span><span class="sxs-lookup"><span data-stu-id="86528-392">View this month’s product launches and offers</span></span>

### <a name="categories"></a><span data-ttu-id="86528-393">Kategorier</span><span class="sxs-lookup"><span data-stu-id="86528-393">Categories</span></span>

- <span data-ttu-id="86528-394">Datum: 2021-04-01</span><span class="sxs-lookup"><span data-stu-id="86528-394">Date: 2021-04-01</span></span>
- <span data-ttu-id="86528-395">Funktioner</span><span class="sxs-lookup"><span data-stu-id="86528-395">Capabilities</span></span>
 
### <a name="summary"></a><span data-ttu-id="86528-396">Sammanfattning</span><span class="sxs-lookup"><span data-stu-id="86528-396">Summary</span></span>

<span data-ttu-id="86528-397">Produktlanseringskalendern för april 2021 publiceras nu.</span><span class="sxs-lookup"><span data-stu-id="86528-397">The April 2021 product launch calendar is now published.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="86528-398">Påverkad målgrupp</span><span class="sxs-lookup"><span data-stu-id="86528-398">Impacted audience</span></span>

<span data-ttu-id="86528-399">Alla partner som gör en Molnlösningsleverantör via CSP-programmet</span><span class="sxs-lookup"><span data-stu-id="86528-399">All partners transacting through the Cloud Solution Provider (CSP) program</span></span>

### <a name="details"></a><span data-ttu-id="86528-400">Information</span><span class="sxs-lookup"><span data-stu-id="86528-400">Details</span></span>

<span data-ttu-id="86528-401">Produktlanseringskalendern för [april](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) 2021 är nu tillgänglig i resursgalleriet för driftberedskap.</span><span class="sxs-lookup"><span data-stu-id="86528-401">The April 2021 [product launch calendar](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) is now available in the Operations readiness resource gallery.</span></span> <span data-ttu-id="86528-402">Visa kommande produktlanseringar och erbjudanden här.</span><span class="sxs-lookup"><span data-stu-id="86528-402">View the upcoming product launches and offers here.</span></span>

### <a name="next-steps"></a><span data-ttu-id="86528-403">Nästa steg</span><span class="sxs-lookup"><span data-stu-id="86528-403">Next steps</span></span>

<span data-ttu-id="86528-404">Granska kalendern [för produktlansering](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/)och dela informationen med lämpliga intressenter i din organisation.</span><span class="sxs-lookup"><span data-stu-id="86528-404">Review the [product launch calendar](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/), and share the information with the appropriate stakeholders in your organization.</span></span>  

### <a name="questions"></a><span data-ttu-id="86528-405">Har du några frågor?</span><span class="sxs-lookup"><span data-stu-id="86528-405">Questions?</span></span>

<span data-ttu-id="86528-406">Om du har fler frågor om dessa erbjudanden kan du läsa dina relevanta Yammer-communities.</span><span class="sxs-lookup"><span data-stu-id="86528-406">For any further questions about these offers, check your relevant Yammer communities.</span></span>
