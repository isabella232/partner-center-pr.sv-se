---
title: Hantera platser i ditt partnerkonto
ms.topic: how-to
ms.date: 05/01/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Lär dig hur du lägger till en ny plats och hur plats-MPN-ID används i incitamentprogram, CSP-företag, prenumerationer och andra transaktioner.
author: vinayks
ms.author: vinayks
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 8a2b4fa8b204b10d5d45c0e1409ab4bc463e272f
ms.sourcegitcommit: 22e257d5b334ca8d3fc072f59010a508e1022694
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 05/06/2021
ms.locfileid: "108702900"
---
# <a name="manage-your-mpn-account-locations-and-add-delete-a-location"></a><span data-ttu-id="1d237-103">Hantera dina MPN-kontoplatser och lägg till (ta bort) en plats</span><span class="sxs-lookup"><span data-stu-id="1d237-103">Manage your MPN account locations and add (delete) a location</span></span>


<span data-ttu-id="1d237-104">**Lämpliga roller**</span><span class="sxs-lookup"><span data-stu-id="1d237-104">**Appropriate roles**</span></span>

- <span data-ttu-id="1d237-105">Global administratör</span><span class="sxs-lookup"><span data-stu-id="1d237-105">Global admin</span></span>
- <span data-ttu-id="1d237-106">Kontoadministratör</span><span class="sxs-lookup"><span data-stu-id="1d237-106">Account admin</span></span>

<span data-ttu-id="1d237-107">Platsens MPN-ID identifierar varje specifik plats för ditt företag.</span><span class="sxs-lookup"><span data-stu-id="1d237-107">The location MPN ID identifies each specific location of your company.</span></span> <span data-ttu-id="1d237-108">Du använder platsens MPN-ID för att registrera dig för incitamentprogram, för att Molnlösningsleverantör(CSP)-företag och andra affärstransaktioner.</span><span class="sxs-lookup"><span data-stu-id="1d237-108">You use the location MPN ID to enroll in incentive programs, to transact Cloud Solution Provider (CSP) business, and other business transactions.</span></span> <span data-ttu-id="1d237-109">Det globala MPN-ID:t används för icke-transaktionella aktiviteter, till exempel supportbegäranden.</span><span class="sxs-lookup"><span data-stu-id="1d237-109">The global MPN ID is used for non-transactional activities such as support requests.</span></span>

## <a name="the-following-scenario-is-typical"></a><span data-ttu-id="1d237-110">Följande scenario är vanligt:</span><span class="sxs-lookup"><span data-stu-id="1d237-110">The following scenario is typical:</span></span>

<span data-ttu-id="1d237-111">Contoso har sitt globala partnerkonto (PGA) i Storbritannien.</span><span class="sxs-lookup"><span data-stu-id="1d237-111">Contoso has its Partner global account (PGA) in the UK.</span></span> <span data-ttu-id="1d237-112">PGA är deras registrerade juridiska verksamhet och dess globala MPN-ID används för att hantera alla icke-transaktionella företag.</span><span class="sxs-lookup"><span data-stu-id="1d237-112">The PGA is their registered legal business, and it's global MPN ID is used for managing all non-transactional business.</span></span> <span data-ttu-id="1d237-113">Contoso har också partnerplatskonton (PLA) som motsvarar dotterbolag eller avdelningar på en annan plats i Storbritannien, Frankrike och USA.</span><span class="sxs-lookup"><span data-stu-id="1d237-113">Contoso also has Partner location accounts (PLA) equivalent to subsidiaries or divisions in another location in the UK, France, and the USA.</span></span> <span data-ttu-id="1d237-114">I MPN-kontostrukturen representeras dessa PLA:er som MPN-ID:er för unika platser.</span><span class="sxs-lookup"><span data-stu-id="1d237-114">In the MPN Account structure, these PLAs are represented as unique location MPN IDs.</span></span> <span data-ttu-id="1d237-115">PLA:erna används för transaktionella företag, till exempel CSP eller incitamentsprogram.</span><span class="sxs-lookup"><span data-stu-id="1d237-115">The PLAs are used for transactional business such as CSP or incentives programs.</span></span> <span data-ttu-id="1d237-116">Utbetalningarna är knutna till specifika platser.</span><span class="sxs-lookup"><span data-stu-id="1d237-116">Payouts are tied to specific locations.</span></span> 

>[!NOTE]
><span data-ttu-id="1d237-117">Det finns en 1-1-relation mellan en CSP-klient och ett MPN-plats-ID.</span><span class="sxs-lookup"><span data-stu-id="1d237-117">There is a 1-1 relationship between a CSP tenant and an MPN location ID.</span></span>

:::image type="content" source="images/locations/locations1.png" alt-text="Strukturen för MPN-platser":::

## <a name="prerequisites-in-order-to-add-a-new-account-for-a-csp-business"></a><span data-ttu-id="1d237-119">Krav för att kunna lägga till ett nytt konto för en CSP-verksamhet</span><span class="sxs-lookup"><span data-stu-id="1d237-119">Prerequisites in order to add a new account for a CSP business</span></span>

<span data-ttu-id="1d237-120">Om du vill lägga till ett nytt CSP-företagskonto börjar du med att se till att du uppfyller kraven.</span><span class="sxs-lookup"><span data-stu-id="1d237-120">To add a new CSP business account, start by ensuring that you have fulfilled the prerequisites.</span></span>

1. <span data-ttu-id="1d237-121">Du måste ha ett PLATS-MPN-ID i det land där du vill göra CSP-verksamhet.</span><span class="sxs-lookup"><span data-stu-id="1d237-121">You must have a location MPN ID in the country where you want to do CSP business.</span></span> <span data-ttu-id="1d237-122">Om du vill skapa en ny MPN-plats läser du "Lägg till en MPN-plats" nedan.</span><span class="sxs-lookup"><span data-stu-id="1d237-122">To create a new MPN location, read “Add an MPN location” below.</span></span>
  
1. <span data-ttu-id="1d237-123">Om du vill skapa en CSP Indirect Reseller registrering kan du läsa [Arbeta med indirekta leverantörer](indirect-reseller-tasks-in-partner-center.md#get-started)</span><span class="sxs-lookup"><span data-stu-id="1d237-123">To create a new CSP Indirect Reseller enrollment, read [Work with Indirect providers](indirect-reseller-tasks-in-partner-center.md#get-started)</span></span> 

>[!NOTE] 
 ><span data-ttu-id="1d237-124">Kom ihåg att logga in med de **nya autentiseringsuppgifterna** för det **nya** CSP-kontot.</span><span class="sxs-lookup"><span data-stu-id="1d237-124">Remember to sign in with the **new** credentials for the **new** CSP account.</span></span> <span data-ttu-id="1d237-125">Använd inte dina befintliga autentiseringsuppgifter eftersom Partnercenter identifierar dig som att du redan har ett konto.</span><span class="sxs-lookup"><span data-stu-id="1d237-125">Don't use your existing credentials as Partner Center will recognize you as already having an account.</span></span>

2. <span data-ttu-id="1d237-126">Godkänn Microsoft-partneravtal och aktivera kontot.</span><span class="sxs-lookup"><span data-stu-id="1d237-126">Accept the Microsoft Partner Agreement and activate the account.</span></span>

1. <span data-ttu-id="1d237-127">Om du vill registrera dig som direktfaktureringspartner läser du [Krav för direktfaktureringspartner](direct-partner-new-requirements.md)</span><span class="sxs-lookup"><span data-stu-id="1d237-127">If you want to enroll as a Direct Bill partner, read [Requirements for Direct Bill partners](direct-partner-new-requirements.md)</span></span>

## <a name="view-and-update-your-mpn-locations"></a><span data-ttu-id="1d237-128">Visa och uppdatera DINA MPN-platser</span><span class="sxs-lookup"><span data-stu-id="1d237-128">View and update your MPN locations</span></span>

1. <span data-ttu-id="1d237-129">Logga in på instrumentpanelen i [Partnercenter med](https://partner.microsoft.com/dashboard/home) dina MPN-kontoautentiseringsuppgifter.</span><span class="sxs-lookup"><span data-stu-id="1d237-129">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard/home) with your MPN account credentials.</span></span> <span data-ttu-id="1d237-130">(Dina MPN-autentiseringsuppgifter kan vara annorlunda än dina CSP-autentiseringsuppgifter)</span><span class="sxs-lookup"><span data-stu-id="1d237-130">(Your MPN credentials may be different from your CSP credentials)</span></span> 
 
1. <span data-ttu-id="1d237-131">Från ikonen **Inställningar** väljer du **Kontoinställningar,** **Organisationsprofil,** **Juridiskt.**</span><span class="sxs-lookup"><span data-stu-id="1d237-131">From the **Settings** icon, select **Account settings**, **Organization profile**, **Legal**.</span></span> 

1. <span data-ttu-id="1d237-132">På fliken **Partner** kontrollerar du att det inte finns något banderollsfelmeddelande där du uppmanas att åtgärda migrerade platser från PMC.</span><span class="sxs-lookup"><span data-stu-id="1d237-132">On the **Partner** tab, verify that there isn't a banner error message asking you to fix migrated locations from PMC.</span></span>  <span data-ttu-id="1d237-133">Om dina platser inte har ställts in korrekt i PMC och ännu inte har gått över till datorn, måste du uppdatera dessa platser.</span><span class="sxs-lookup"><span data-stu-id="1d237-133">If your locations were not set up correctly in PMC, and have not transitioned yet to PC, you need to update those locations.</span></span>

:::image type="content" source="images/locations/location-two.png" alt-text="Skärmbild som visar hur du uppdaterar platsen.":::
 
4.  <span data-ttu-id="1d237-135">På skärmen **Granska PMC-platser** väljer du **Uppdatera**.</span><span class="sxs-lookup"><span data-stu-id="1d237-135">On the **Review PMC locations** screen, select **Update**.</span></span>
<span data-ttu-id="1d237-136">Uppdatera följande fält:</span><span class="sxs-lookup"><span data-stu-id="1d237-136">Update the following fields:</span></span>

- <span data-ttu-id="1d237-137">**Namnfält:** Kontrollera att namnet på företagets plats är korrekt.</span><span class="sxs-lookup"><span data-stu-id="1d237-137">**Name field**: Make sure that the name of the company location is correct.</span></span> <span data-ttu-id="1d237-138">Om ett dubblettfel visas kan du prova att byta från till exempel Contoso till Contoso, Inc.</span><span class="sxs-lookup"><span data-stu-id="1d237-138">If a duplicate error is displayed, try changing from, for example, Contoso to Contoso, Inc.</span></span>

- <span data-ttu-id="1d237-139">**Fältet Juridisk enhet:** Kontrollera att du har valt den juridiska enhet som platsen är kopplad till</span><span class="sxs-lookup"><span data-stu-id="1d237-139">**Legal Entity field**: Make sure that you have chosen the legal entity the location is tied to</span></span>

- <span data-ttu-id="1d237-140">**Adressrad 1 & 2:** Kontrollera att adressen är korrekt</span><span class="sxs-lookup"><span data-stu-id="1d237-140">**Address line 1 & 2 fields**: Make sure that the address is correct</span></span>

- <span data-ttu-id="1d237-141">**Ort & för delstat/provins:** Kontrollera att kombinationen mellan stad och region är korrekt.</span><span class="sxs-lookup"><span data-stu-id="1d237-141">**City & State/Province fields**: Make sure the combination between the city and the state/province is correct.</span></span> <span data-ttu-id="1d237-142">Det finns länder där listrutemenyn för att välja Delstat/provins kommer att gälla, och i andra länder måste fältet infogas manuellt.</span><span class="sxs-lookup"><span data-stu-id="1d237-142">There are countries where the dropdown menu for choosing the State/Province will apply, and in other countries that field will need to manually be inserted.</span></span>

- <span data-ttu-id="1d237-143">**Postnummerfält:** Kontrollera att postnummerfältet matchar ditt angivna land, region, ort eller adress.</span><span class="sxs-lookup"><span data-stu-id="1d237-143">**ZIP/ Postal code field**: Make sure the Zip Code field is matching your indicated Country, Region, City, or Address.</span></span>

- <span data-ttu-id="1d237-144">**Fält med primär** kontaktinformation: Kontrollera att fälten för för- och efternamn är ifyllda och att e-postadressen som anges är en e-postadress för arbetet och inte en personlig e-postadress (till exempel @outlook.com , @live.com osv.)</span><span class="sxs-lookup"><span data-stu-id="1d237-144">**Primary contact information fields**: Make sure the first and last name fields are filled and that the e-mail address indicated is a work e-mail address and not a personal one (for example, @outlook.com, @live.com, etc.)</span></span>

- <span data-ttu-id="1d237-145">**Fältet Telefonnummer:** Kontrollera att Telefonnumret INTE innehåller specialtecken, blanksteg eller landskod.</span><span class="sxs-lookup"><span data-stu-id="1d237-145">**Phone number field**: Make sure that the Phone number does NOT include special characters, spaces, or country code.</span></span> <span data-ttu-id="1d237-146">Värdet som anges i fältet Telefonnummer innehåller alltid högst 10 tecken.</span><span class="sxs-lookup"><span data-stu-id="1d237-146">The value entered in the Phone Number field will always contain a maximum of 10 characters.</span></span>

5. <span data-ttu-id="1d237-147">Om det inte finns något felmeddelande går du till Inställningar **och väljer** **Kontoinställningar,** **Organisationsprofil,** **Identifierare.**</span><span class="sxs-lookup"><span data-stu-id="1d237-147">If there isn't an error message, then from  **Settings**, select  **Account Settings**, **Organization profile**, **Identifiers**.</span></span>

6. <span data-ttu-id="1d237-148">Hitta MPN-ID:t med typen "Plats" som matchar landet för det här CSP-kontot och använd det för att slutföra associationen.</span><span class="sxs-lookup"><span data-stu-id="1d237-148">Find the MPN ID with Type "Location" that matches the country of this CSP account and use it to complete the association.</span></span>

7. <span data-ttu-id="1d237-149">Om du inte hittar platsens MPN-ID som matchar det CSP-konto som du vill använda kan du lägga till en ny plats, vilket skapar ett nytt MPN-ID.</span><span class="sxs-lookup"><span data-stu-id="1d237-149">If you can’t find the location MPN ID that matches the CSP account you want to use, you can add a new location, which will create a new MPN ID.</span></span> <span data-ttu-id="1d237-150">Se **Lägg till en MPN-plats** nedan.</span><span class="sxs-lookup"><span data-stu-id="1d237-150">See **Add an MPN location** below.</span></span>

## <a name="add-an-mpn-location"></a><span data-ttu-id="1d237-151">Lägga till en MPN-plats</span><span class="sxs-lookup"><span data-stu-id="1d237-151">Add an MPN location</span></span>

1. <span data-ttu-id="1d237-152">Logga in med MPN-kontot i Partnercenter.</span><span class="sxs-lookup"><span data-stu-id="1d237-152">Sign in using the MPN account in Partner Center.</span></span> <span data-ttu-id="1d237-153">(Dina MPN-autentiseringsuppgifter kan vara annorlunda än dina CSP-autentiseringsuppgifter).</span><span class="sxs-lookup"><span data-stu-id="1d237-153">(Your MPN credentials may be different from your CSP credentials) .</span></span> <span data-ttu-id="1d237-154">MPN-kontot ska ha behörighet som global administratör eller kontoadministratör.</span><span class="sxs-lookup"><span data-stu-id="1d237-154">The MPN account should have Global Admin or Account Admin privileges.</span></span> 

1. <span data-ttu-id="1d237-155">Från ikonen **Inställningar väljer** du **Kontoinställningar och** sedan **Organisationsprofil.**</span><span class="sxs-lookup"><span data-stu-id="1d237-155">From the **Settings icon**, select the **Account settings** and then select **Organization profile**.</span></span>

2. <span data-ttu-id="1d237-156">Välj **Juridiskt** och sedan På fliken **Partner** väljer du **Företagsplatser** och klickar på Lägg **till en plats.**</span><span class="sxs-lookup"><span data-stu-id="1d237-156">Select **Legal** and then, on the **Partner** tab, select **Business locations,** and click on **Add a location.**</span></span>

3. <span data-ttu-id="1d237-157">Ange nödvändig information, inklusive företagsnamn, adress och kontakt för den plats som du vill lägga till i företaget.</span><span class="sxs-lookup"><span data-stu-id="1d237-157">Provide the required details including business name, address, and contact for the location that you want to add to your company.</span></span>
 
1. <span data-ttu-id="1d237-158">Klicka **på Lägg till plats.**</span><span class="sxs-lookup"><span data-stu-id="1d237-158">Click **Add location**.</span></span> <span data-ttu-id="1d237-159">Detta skapar ett nytt MPN-ID för den nya platsen som du kan använda för CSP-transaktioner och incitament.</span><span class="sxs-lookup"><span data-stu-id="1d237-159">This will create a new MPN ID for the new location which you can use for CSP transactions and incentives.</span></span>

:::image type="content" source="images/legal-biz.png" alt-text="Lägga till ett nytt juridiskt företag":::

> [!NOTE]
> <span data-ttu-id="1d237-161">När en plats har lagts till i Partnercenter kan du inte ta bort den.</span><span class="sxs-lookup"><span data-stu-id="1d237-161">Once a location is added in Partner Center, you cannot remove it.</span></span> <span data-ttu-id="1d237-162">MPN **visas på** den vänstra menyn i Partnercenter om du har använt rätt MPN-ID för att logga in.</span><span class="sxs-lookup"><span data-stu-id="1d237-162">You will see **MPN** in the left menu of Partner Center if you have used the correct MPN ID to sign in.</span></span>

## <a name="add-the-registration-number-id"></a><span data-ttu-id="1d237-163">Lägg till registreringsnummer-ID:t</span><span class="sxs-lookup"><span data-stu-id="1d237-163">Add the registration number ID</span></span>

<span data-ttu-id="1d237-164">Om du är en indirekt leverantör, partner för direktfakturering eller indirekt återförsäljare och du gör affärer med nya eller befintliga kunder i följande länder måste du ange registrerings-ID-nummer för din verksamhet.</span><span class="sxs-lookup"><span data-stu-id="1d237-164">If you are an Indirect provider, Direct bill partner, or Indirect reseller and you are doing business with new or existing customers in the following countries, you need to provide registration ID numbers for your business.</span></span> <span data-ttu-id="1d237-165">Om landet du gör affärer i inte visas nedan är registrerings-ID valfritt.</span><span class="sxs-lookup"><span data-stu-id="1d237-165">If the country you are doing business in is not listed below, the registration ID is optional.</span></span>

- <span data-ttu-id="1d237-166">Armenien</span><span class="sxs-lookup"><span data-stu-id="1d237-166">Armenia</span></span> 
- <span data-ttu-id="1d237-167">Azerbajdzjan</span><span class="sxs-lookup"><span data-stu-id="1d237-167">Azerbaijan</span></span> 
- <span data-ttu-id="1d237-168">Vitryssland</span><span class="sxs-lookup"><span data-stu-id="1d237-168">Belarus</span></span> 
- <span data-ttu-id="1d237-169">Brasilien</span><span class="sxs-lookup"><span data-stu-id="1d237-169">Brazil</span></span> 
- <span data-ttu-id="1d237-170">Ungern</span><span class="sxs-lookup"><span data-stu-id="1d237-170">Hungary</span></span> 
- <span data-ttu-id="1d237-171">Indien</span><span class="sxs-lookup"><span data-stu-id="1d237-171">India</span></span> 
- <span data-ttu-id="1d237-172">Irak</span><span class="sxs-lookup"><span data-stu-id="1d237-172">Iraq</span></span> 
- <span data-ttu-id="1d237-173">Kazakstan</span><span class="sxs-lookup"><span data-stu-id="1d237-173">Kazakhstan</span></span> 
- <span data-ttu-id="1d237-174">Kirgizistan</span><span class="sxs-lookup"><span data-stu-id="1d237-174">Kyrgyzstan</span></span> 
- <span data-ttu-id="1d237-175">Moldavien</span><span class="sxs-lookup"><span data-stu-id="1d237-175">Moldova</span></span> 
- <span data-ttu-id="1d237-176">Myanmar</span><span class="sxs-lookup"><span data-stu-id="1d237-176">Myanmar</span></span> 
- <span data-ttu-id="1d237-177">Polen</span><span class="sxs-lookup"><span data-stu-id="1d237-177">Poland</span></span> 
- <span data-ttu-id="1d237-178">Ryssland</span><span class="sxs-lookup"><span data-stu-id="1d237-178">Russia</span></span> 
- <span data-ttu-id="1d237-179">Saudiarabien</span><span class="sxs-lookup"><span data-stu-id="1d237-179">Saudi Arabia</span></span> 
- <span data-ttu-id="1d237-180">Sydafrika</span><span class="sxs-lookup"><span data-stu-id="1d237-180">South Africa</span></span> 
- <span data-ttu-id="1d237-181">Sydsudan</span><span class="sxs-lookup"><span data-stu-id="1d237-181">South Sudan</span></span>  
- <span data-ttu-id="1d237-182">Tadzjikistan</span><span class="sxs-lookup"><span data-stu-id="1d237-182">Tajikistan</span></span> 
- <span data-ttu-id="1d237-183">Thailand</span><span class="sxs-lookup"><span data-stu-id="1d237-183">Thailand</span></span>
- <span data-ttu-id="1d237-184">Turkiet</span><span class="sxs-lookup"><span data-stu-id="1d237-184">Turkey</span></span> 
- <span data-ttu-id="1d237-185">Ukraina</span><span class="sxs-lookup"><span data-stu-id="1d237-185">Ukraine</span></span> 
- <span data-ttu-id="1d237-186">Förenade Arabemiraten</span><span class="sxs-lookup"><span data-stu-id="1d237-186">United Arab Emirates</span></span> 
- <span data-ttu-id="1d237-187">Uzbekistan</span><span class="sxs-lookup"><span data-stu-id="1d237-187">Uzbekistan</span></span> 
- <span data-ttu-id="1d237-188">Venezuela</span><span class="sxs-lookup"><span data-stu-id="1d237-188">Venezuela</span></span>
- <span data-ttu-id="1d237-189">Vietnam</span><span class="sxs-lookup"><span data-stu-id="1d237-189">Vietnam</span></span> 


<span data-ttu-id="1d237-190">Mer information finns i Informationen om [registrerings-ID-nummer](reg-number-id.md)</span><span class="sxs-lookup"><span data-stu-id="1d237-190">For more information, read [Registration ID number information](reg-number-id.md)</span></span>

## <a name="delete-a-location"></a><span data-ttu-id="1d237-191">Ta bort en plats</span><span class="sxs-lookup"><span data-stu-id="1d237-191">Delete a location</span></span>

<span data-ttu-id="1d237-192">Om du vill ta bort en plats från ditt konto måste du kontakta [partnersupporten.](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=1af7f3a0-1757-3543-4b6a-c945c3ad187b)</span><span class="sxs-lookup"><span data-stu-id="1d237-192">To delete a location from your account, you will need to contact [Partner Support](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=1af7f3a0-1757-3543-4b6a-c945c3ad187b).</span></span> <span data-ttu-id="1d237-193">Se till att du förstår vilken effekt den här åtgärden har.</span><span class="sxs-lookup"><span data-stu-id="1d237-193">Make sure that you understand the impact this action has.</span></span> <span data-ttu-id="1d237-194">Borttagna platser kan inte hämtas och allt som är kopplat till det specifika MPN-ID:t kommer inte längre att identifieras eller vara aktivt för ditt företag.</span><span class="sxs-lookup"><span data-stu-id="1d237-194">Deleted locations cannot be retrieved and anything tied to that specific MPN id will no longer be recognized or be active for your company.</span></span>

## <a name="change-country-of-partner-global-account"></a><span data-ttu-id="1d237-195">Ändra land för partnerns globala konto</span><span class="sxs-lookup"><span data-stu-id="1d237-195">Change country of Partner global account</span></span> 

1. <span data-ttu-id="1d237-196">Logga in med MPN-kontot i Partnercenter.</span><span class="sxs-lookup"><span data-stu-id="1d237-196">Sign in using the MPN account in Partner Center.</span></span> <span data-ttu-id="1d237-197">(Dina MPN-autentiseringsuppgifter kan vara annorlunda än dina CSP-autentiseringsuppgifter).</span><span class="sxs-lookup"><span data-stu-id="1d237-197">(Your MPN credentials may be different from your CSP credentials) .</span></span> <span data-ttu-id="1d237-198">MPN-kontot ska ha behörigheter som global administratör eller kontoadministratör.</span><span class="sxs-lookup"><span data-stu-id="1d237-198">The MPN account should have Global Admin or Account Admin privileges.</span></span> 

2. <span data-ttu-id="1d237-199">På fliken **Partner** går du till **Företagsplatser** och kontrollerar listan över platser för att se till att den plats som du vill ha som juridisk enhet visas.</span><span class="sxs-lookup"><span data-stu-id="1d237-199">On the **Partner** tab, go to **Business locations** and check the list of locations to ensure that the location you want as your legal entity is listed.</span></span> 
 
1. <span data-ttu-id="1d237-200">Om du vill lägga till en plats klickar du på Lägg till en plats och anger nödvändig information, inklusive företagsnamn, adress och primär kontakt för den plats som du vill lägga till i företaget.</span><span class="sxs-lookup"><span data-stu-id="1d237-200">To add a location, click **Add a location**, and, in the fly out, provide the required details including business name, address, and primary contact for the location that you want to add to your company.</span></span> 
 
1. <span data-ttu-id="1d237-201">Välj **Ändra land** bredvid **listrutan Land/region** och följ stegen.</span><span class="sxs-lookup"><span data-stu-id="1d237-201">Select **Change your country** next to the **Country/region** drop-down and follow the steps.</span></span> 

:::image type="content" source="images/lbp.png" alt-text="Data om juridiska affärsprofiler har utfällt":::

5. <span data-ttu-id="1d237-203">Klicka på **Spara**.</span><span class="sxs-lookup"><span data-stu-id="1d237-203">Click **Save**.</span></span>

6. <span data-ttu-id="1d237-204">MPN:s globala kontoland ändras till det nya juridiska landet.</span><span class="sxs-lookup"><span data-stu-id="1d237-204">MPN global account country will be changed to the new legal country.</span></span>
  
## <a name="next-steps"></a><span data-ttu-id="1d237-205">Nästa steg</span><span class="sxs-lookup"><span data-stu-id="1d237-205">Next steps</span></span>

- <span data-ttu-id="1d237-206">Läs mer om [verifieringsprocessen](verification-responses.md).</span><span class="sxs-lookup"><span data-stu-id="1d237-206">Learn about the [verification process](verification-responses.md).</span></span>
