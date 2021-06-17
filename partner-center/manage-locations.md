---
title: Hantera platser i ditt partnerkonto
ms.topic: how-to
ms.date: 05/01/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Lär dig hur du lägger till en ny plats och hur platsens MPN-ID används i incitamentprogram, CSP-företag, prenumerationer och andra transaktioner.
author: vinayks
ms.author: vinayks
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 3d30f250d6635758f3bef8e06c6f57ba0a0be744
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/17/2021
ms.locfileid: "112276832"
---
# <a name="manage-your-mpn-account-locations-and-add-delete-a-location"></a><span data-ttu-id="7840f-103">Hantera dina MPN-kontoplatser och lägg till (ta bort) en plats</span><span class="sxs-lookup"><span data-stu-id="7840f-103">Manage your MPN account locations and add (delete) a location</span></span>


<span data-ttu-id="7840f-104">**Lämpliga roller:** Globala | Kontoadministratör</span><span class="sxs-lookup"><span data-stu-id="7840f-104">**Appropriate roles**: Global admin | Account admin</span></span>

<span data-ttu-id="7840f-105">PLATSENs MPN-ID identifierar varje specifik plats för ditt företag.</span><span class="sxs-lookup"><span data-stu-id="7840f-105">The location MPN ID identifies each specific location of your company.</span></span> <span data-ttu-id="7840f-106">Du använder platsens MPN-ID för att registrera dig för incitamentprogram, för att Molnlösningsleverantör företag (CSP) och andra affärstransaktioner.</span><span class="sxs-lookup"><span data-stu-id="7840f-106">You use the location MPN ID to enroll in incentive programs, to transact Cloud Solution Provider (CSP) business, and other business transactions.</span></span> <span data-ttu-id="7840f-107">Det globala MPN-ID:t används för icke-transaktionella aktiviteter, till exempel supportbegäranden.</span><span class="sxs-lookup"><span data-stu-id="7840f-107">The global MPN ID is used for non-transactional activities such as support requests.</span></span>

## <a name="the-following-scenario-is-typical"></a><span data-ttu-id="7840f-108">Följande scenario är typiskt:</span><span class="sxs-lookup"><span data-stu-id="7840f-108">The following scenario is typical:</span></span>

<span data-ttu-id="7840f-109">Contoso har sitt globala partnerkonto (PGA) i Storbritannien.</span><span class="sxs-lookup"><span data-stu-id="7840f-109">Contoso has its Partner global account (PGA) in the UK.</span></span> <span data-ttu-id="7840f-110">PGA är deras registrerade juridiska verksamhet och dess globala MPN-ID används för att hantera alla icke-transaktionella företag.</span><span class="sxs-lookup"><span data-stu-id="7840f-110">The PGA is their registered legal business, and its global MPN ID is used for managing all non-transactional business.</span></span> <span data-ttu-id="7840f-111">Contoso har också partnerplatskonton (PLA) som motsvarar dotterbolag eller avdelningar på en annan plats i Storbritannien, Frankrike och USA.</span><span class="sxs-lookup"><span data-stu-id="7840f-111">Contoso also has Partner location accounts (PLA) equivalent to subsidiaries or divisions in another location in the UK, France, and the USA.</span></span> <span data-ttu-id="7840f-112">I MPN-kontostrukturen representeras dessa PLA:er som unika MPN-ID:er för platsen.</span><span class="sxs-lookup"><span data-stu-id="7840f-112">In the MPN Account structure, these PLAs are represented as unique location MPN IDs.</span></span> <span data-ttu-id="7840f-113">PLA:erna används för transaktionella företag, till exempel CSP eller incitamentsprogram.</span><span class="sxs-lookup"><span data-stu-id="7840f-113">The PLAs are used for transactional business such as CSP or incentives programs.</span></span> <span data-ttu-id="7840f-114">Utbetalningar är knutna till specifika platser.</span><span class="sxs-lookup"><span data-stu-id="7840f-114">Payouts are tied to specific locations.</span></span> 

>[!NOTE]
><span data-ttu-id="7840f-115">Det finns en 1-1-relation mellan en CSP-klient och ett MPN-plats-ID.</span><span class="sxs-lookup"><span data-stu-id="7840f-115">There is a 1-1 relationship between a CSP tenant and an MPN location ID.</span></span>

:::image type="content" source="images/locations/locations1.png" alt-text="Struktur för MPN-platser.":::

## <a name="prerequisites-in-order-to-add-a-new-account-for-a-csp-business"></a><span data-ttu-id="7840f-117">Krav för att lägga till ett nytt konto för ett CSP-företag</span><span class="sxs-lookup"><span data-stu-id="7840f-117">Prerequisites in order to add a new account for a CSP business</span></span>

<span data-ttu-id="7840f-118">Om du vill lägga till ett nytt CSP-företagskonto börjar du med att se till att du uppfyller kraven.</span><span class="sxs-lookup"><span data-stu-id="7840f-118">To add a new CSP business account, start by ensuring that you have fulfilled the prerequisites.</span></span>

1. <span data-ttu-id="7840f-119">Du måste ha ett PLATS-MPN-ID i det land där du vill göra CSP-verksamheten.</span><span class="sxs-lookup"><span data-stu-id="7840f-119">You must have a location MPN ID in the country where you want to do CSP business.</span></span> <span data-ttu-id="7840f-120">Om du vill skapa en ny MPN-plats läser du "Lägg till en MPN-plats" nedan.</span><span class="sxs-lookup"><span data-stu-id="7840f-120">To create a new MPN location, read “Add an MPN location” below.</span></span>
  
1. <span data-ttu-id="7840f-121">Om du vill skapa en CSP Indirect Reseller registrering kan du läsa [Arbeta med indirekta leverantörer](indirect-reseller-tasks-in-partner-center.md#get-started)</span><span class="sxs-lookup"><span data-stu-id="7840f-121">To create a new CSP Indirect Reseller enrollment, read [Work with Indirect providers](indirect-reseller-tasks-in-partner-center.md#get-started)</span></span> 

>[!NOTE] 
 ><span data-ttu-id="7840f-122">Kom ihåg att logga in med de **nya autentiseringsuppgifterna** för det **nya** CSP-kontot.</span><span class="sxs-lookup"><span data-stu-id="7840f-122">Remember to sign in with the **new** credentials for the **new** CSP account.</span></span> <span data-ttu-id="7840f-123">Använd inte dina befintliga autentiseringsuppgifter eftersom Partnercenter identifierar dig som att du redan har ett konto.</span><span class="sxs-lookup"><span data-stu-id="7840f-123">Don't use your existing credentials as Partner Center will recognize you as already having an account.</span></span>

2. <span data-ttu-id="7840f-124">Godkänn Microsoft-partneravtal och aktivera kontot.</span><span class="sxs-lookup"><span data-stu-id="7840f-124">Accept the Microsoft Partner Agreement and activate the account.</span></span>

1. <span data-ttu-id="7840f-125">Om du vill registrera dig som direktfaktureringspartner läser du [Krav för direktfaktureringspartner](direct-partner-new-requirements.md)</span><span class="sxs-lookup"><span data-stu-id="7840f-125">If you want to enroll as a Direct Bill partner, read [Requirements for Direct Bill partners](direct-partner-new-requirements.md)</span></span>

## <a name="view-and-update-your-mpn-locations"></a><span data-ttu-id="7840f-126">Visa och uppdatera DINA MPN-platser</span><span class="sxs-lookup"><span data-stu-id="7840f-126">View and update your MPN locations</span></span>

1. <span data-ttu-id="7840f-127">Logga in på instrumentpanelen i [Partnercenter med](https://partner.microsoft.com/dashboard/home) dina MPN-kontoautentiseringsuppgifter.</span><span class="sxs-lookup"><span data-stu-id="7840f-127">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard/home) with your MPN account credentials.</span></span> <span data-ttu-id="7840f-128">(Dina MPN-autentiseringsuppgifter kan vara annorlunda än dina CSP-autentiseringsuppgifter)</span><span class="sxs-lookup"><span data-stu-id="7840f-128">(Your MPN credentials may be different from your CSP credentials)</span></span> 
 
1. <span data-ttu-id="7840f-129">Från ikonen **Inställningar** väljer du **Kontoinställningar**, **Organisationsprofil**, **Juridiskt**.</span><span class="sxs-lookup"><span data-stu-id="7840f-129">From the **Settings** icon, select **Account settings**, **Organization profile**, **Legal**.</span></span> 

1. <span data-ttu-id="7840f-130">På fliken **Partner** kontrollerar du att det inte finns något banderollsfelmeddelande där du uppmanas att åtgärda migrerade platser från PMC.</span><span class="sxs-lookup"><span data-stu-id="7840f-130">On the **Partner** tab, verify that there isn't a banner error message asking you to fix migrated locations from PMC.</span></span>  <span data-ttu-id="7840f-131">Om dina platser inte har ställts in korrekt i PMC och ännu inte har gått över till datorn, måste du uppdatera dessa platser.</span><span class="sxs-lookup"><span data-stu-id="7840f-131">If your locations were not set up correctly in PMC, and have not transitioned yet to PC, you need to update those locations.</span></span>

:::image type="content" source="images/locations/location-two.png" alt-text="Skärmbild som visar hur du uppdaterar platsen.":::
 
4.  <span data-ttu-id="7840f-133">På skärmen **Granska PMC-platser** väljer du **Uppdatera**.</span><span class="sxs-lookup"><span data-stu-id="7840f-133">On the **Review PMC locations** screen, select **Update**.</span></span>
<span data-ttu-id="7840f-134">Uppdatera följande fält:</span><span class="sxs-lookup"><span data-stu-id="7840f-134">Update the following fields:</span></span>

- <span data-ttu-id="7840f-135">**Namnfält:** Kontrollera att namnet på företagets plats är korrekt.</span><span class="sxs-lookup"><span data-stu-id="7840f-135">**Name field**: Make sure that the name of the company location is correct.</span></span> <span data-ttu-id="7840f-136">Om ett dubblettfel visas kan du prova att byta från till exempel Contoso till Contoso, Inc.</span><span class="sxs-lookup"><span data-stu-id="7840f-136">If a duplicate error is displayed, try changing from, for example, Contoso to Contoso, Inc.</span></span>

- <span data-ttu-id="7840f-137">**Fältet Juridisk enhet:** Kontrollera att du har valt den juridiska enhet som platsen är kopplad till</span><span class="sxs-lookup"><span data-stu-id="7840f-137">**Legal Entity field**: Make sure that you have chosen the legal entity the location is tied to</span></span>

- <span data-ttu-id="7840f-138">**Adressrad 1 & 2:** Kontrollera att adressen är korrekt</span><span class="sxs-lookup"><span data-stu-id="7840f-138">**Address line 1 & 2 fields**: Make sure that the address is correct</span></span>

- <span data-ttu-id="7840f-139">**Ort & för delstat/provins:** Kontrollera att kombinationen mellan stad och region är korrekt.</span><span class="sxs-lookup"><span data-stu-id="7840f-139">**City & State/Province fields**: Make sure the combination between the city and the state/province is correct.</span></span> <span data-ttu-id="7840f-140">Det finns länder där den nedrullningsbara menyn för att välja Delstat/provins kommer att gälla, och i andra länder måste fältet infogas manuellt.</span><span class="sxs-lookup"><span data-stu-id="7840f-140">There are countries where the dropdown menu for choosing the State/Province will apply, and in other countries that field will need to manually be inserted.</span></span>

- <span data-ttu-id="7840f-141">**Postnummerfält:** Kontrollera att postnummerfältet matchar ditt angivna land, region, ort eller adress.</span><span class="sxs-lookup"><span data-stu-id="7840f-141">**ZIP/ Postal code field**: Make sure the Zip Code field is matching your indicated Country, Region, City, or Address.</span></span>

- <span data-ttu-id="7840f-142">**Primära kontaktinformationsfält:** Kontrollera att fälten för för- och efternamn är ifyllda och att e-postadressen som anges är en e-postadress för arbetet och inte en personlig e-postadress (till exempel @outlook.com , @live.com osv.)</span><span class="sxs-lookup"><span data-stu-id="7840f-142">**Primary contact information fields**: Make sure the first and last name fields are filled and that the e-mail address indicated is a work e-mail address and not a personal one (for example, @outlook.com, @live.com, etc.)</span></span>

- <span data-ttu-id="7840f-143">**Telefonnummerfält:** Kontrollera att Telefonnumret INTE innehåller specialtecken, blanksteg eller landskod.</span><span class="sxs-lookup"><span data-stu-id="7840f-143">**Phone number field**: Make sure that the Phone number does NOT include special characters, spaces, or country code.</span></span> <span data-ttu-id="7840f-144">Värdet som anges i fältet Telefonnummer innehåller alltid högst 10 tecken.</span><span class="sxs-lookup"><span data-stu-id="7840f-144">The value entered in the Phone Number field will always contain a maximum of 10 characters.</span></span>

5. <span data-ttu-id="7840f-145">Om det inte finns något felmeddelande går du till **Inställningar och väljer** **Kontoinställningar,** **Organisationsprofil,** **Identifierare.**</span><span class="sxs-lookup"><span data-stu-id="7840f-145">If there isn't an error message, then from  **Settings**, select  **Account Settings**, **Organization profile**, **Identifiers**.</span></span>

6. <span data-ttu-id="7840f-146">Hitta MPN-ID:t med typen "Plats" som matchar landet för det här CSP-kontot och använd det för att slutföra associationen.</span><span class="sxs-lookup"><span data-stu-id="7840f-146">Find the MPN ID with Type "Location" that matches the country of this CSP account and use it to complete the association.</span></span>

7. <span data-ttu-id="7840f-147">Om du inte hittar platsens MPN-ID som matchar det CSP-konto som du vill använda kan du lägga till en ny plats, vilket skapar ett nytt MPN-ID.</span><span class="sxs-lookup"><span data-stu-id="7840f-147">If you can’t find the location MPN ID that matches the CSP account you want to use, you can add a new location, which will create a new MPN ID.</span></span> <span data-ttu-id="7840f-148">Se **Lägg till en MPN-plats** nedan.</span><span class="sxs-lookup"><span data-stu-id="7840f-148">See **Add an MPN location** below.</span></span>

## <a name="add-an-mpn-location"></a><span data-ttu-id="7840f-149">Lägga till en MPN-plats</span><span class="sxs-lookup"><span data-stu-id="7840f-149">Add an MPN location</span></span>

1. <span data-ttu-id="7840f-150">Logga in med MPN-kontot i Partnercenter.</span><span class="sxs-lookup"><span data-stu-id="7840f-150">Sign in using the MPN account in Partner Center.</span></span> <span data-ttu-id="7840f-151">(Dina MPN-autentiseringsuppgifter kan vara annorlunda än dina CSP-autentiseringsuppgifter.) MPN-kontot ska ha behörigheter som global administratör eller kontoadministratör.</span><span class="sxs-lookup"><span data-stu-id="7840f-151">(Your MPN credentials may be different from your CSP credentials.) The MPN account should have Global Admin or Account Admin privileges.</span></span> 

1. <span data-ttu-id="7840f-152">Från ikonen **Inställningar väljer** du **Kontoinställningar och** sedan **Organisationsprofil.**</span><span class="sxs-lookup"><span data-stu-id="7840f-152">From the **Settings icon**, select the **Account settings** and then select **Organization profile**.</span></span>

2. <span data-ttu-id="7840f-153">Välj **Juridiskt** och sedan, på **fliken Partner,** väljer **du Business locations (Företagsplatser)** och sedan Add a location **(Lägg till en plats).**</span><span class="sxs-lookup"><span data-stu-id="7840f-153">Select **Legal** and then, on the **Partner** tab, select **Business locations,** and select **Add a location.**</span></span>

3. <span data-ttu-id="7840f-154">Ange nödvändig information, inklusive företagsnamn, adress och kontakt för den plats som du vill lägga till i företaget.</span><span class="sxs-lookup"><span data-stu-id="7840f-154">Provide the required details including business name, address, and contact for the location that you want to add to your company.</span></span>
 
1. <span data-ttu-id="7840f-155">Välj **Lägg till plats.**</span><span class="sxs-lookup"><span data-stu-id="7840f-155">Select **Add location**.</span></span> <span data-ttu-id="7840f-156">Detta skapar ett nytt MPN-ID för den nya platsen som du kan använda för CSP-transaktioner och incitament.</span><span class="sxs-lookup"><span data-stu-id="7840f-156">This will create a new MPN ID for the new location that you can use for CSP transactions and incentives.</span></span>

:::image type="content" source="images/legal-biz.png" alt-text="Lägg till en ny juridisk verksamhet.":::

> [!NOTE]
> <span data-ttu-id="7840f-158">När en plats har lagts till i Partnercenter kan du inte ta bort den.</span><span class="sxs-lookup"><span data-stu-id="7840f-158">Once a location is added in Partner Center, you cannot remove it.</span></span> <span data-ttu-id="7840f-159">MPN visas **på** den vänstra menyn i Partnercenter om du har använt rätt MPN-ID för att logga in.</span><span class="sxs-lookup"><span data-stu-id="7840f-159">You will see **MPN** in the left menu of Partner Center if you have used the correct MPN ID to sign in.</span></span>

## <a name="add-the-registration-number-id"></a><span data-ttu-id="7840f-160">Lägg till registreringsnummer-ID:t</span><span class="sxs-lookup"><span data-stu-id="7840f-160">Add the registration number ID</span></span>

<span data-ttu-id="7840f-161">Om du är en indirekt leverantör, partner för direktfakturering eller indirekt återförsäljare och du gör affärer med nya eller befintliga kunder i följande länder måste du ange registrerings-ID-nummer för din verksamhet.</span><span class="sxs-lookup"><span data-stu-id="7840f-161">If you are an Indirect provider, Direct bill partner, or Indirect reseller and you are doing business with new or existing customers in the following countries, you need to provide registration ID numbers for your business.</span></span> <span data-ttu-id="7840f-162">Om landet du gör affärer i inte visas nedan är registrerings-ID valfritt.</span><span class="sxs-lookup"><span data-stu-id="7840f-162">If the country you are doing business in is not listed below, the registration ID is optional.</span></span>

- <span data-ttu-id="7840f-163">Armenien</span><span class="sxs-lookup"><span data-stu-id="7840f-163">Armenia</span></span> 
- <span data-ttu-id="7840f-164">Azerbajdzjan</span><span class="sxs-lookup"><span data-stu-id="7840f-164">Azerbaijan</span></span> 
- <span data-ttu-id="7840f-165">Vitryssland</span><span class="sxs-lookup"><span data-stu-id="7840f-165">Belarus</span></span> 
- <span data-ttu-id="7840f-166">Brasilien</span><span class="sxs-lookup"><span data-stu-id="7840f-166">Brazil</span></span> 
- <span data-ttu-id="7840f-167">Ungern</span><span class="sxs-lookup"><span data-stu-id="7840f-167">Hungary</span></span> 
- <span data-ttu-id="7840f-168">Indien</span><span class="sxs-lookup"><span data-stu-id="7840f-168">India</span></span> 
- <span data-ttu-id="7840f-169">Irak</span><span class="sxs-lookup"><span data-stu-id="7840f-169">Iraq</span></span> 
- <span data-ttu-id="7840f-170">Kazakstan</span><span class="sxs-lookup"><span data-stu-id="7840f-170">Kazakhstan</span></span> 
- <span data-ttu-id="7840f-171">Kirgizistan</span><span class="sxs-lookup"><span data-stu-id="7840f-171">Kyrgyzstan</span></span> 
- <span data-ttu-id="7840f-172">Moldavien</span><span class="sxs-lookup"><span data-stu-id="7840f-172">Moldova</span></span> 
- <span data-ttu-id="7840f-173">Myanmar</span><span class="sxs-lookup"><span data-stu-id="7840f-173">Myanmar</span></span> 
- <span data-ttu-id="7840f-174">Polen</span><span class="sxs-lookup"><span data-stu-id="7840f-174">Poland</span></span> 
- <span data-ttu-id="7840f-175">Ryssland</span><span class="sxs-lookup"><span data-stu-id="7840f-175">Russia</span></span> 
- <span data-ttu-id="7840f-176">Saudiarabien</span><span class="sxs-lookup"><span data-stu-id="7840f-176">Saudi Arabia</span></span> 
- <span data-ttu-id="7840f-177">Sydafrika</span><span class="sxs-lookup"><span data-stu-id="7840f-177">South Africa</span></span> 
- <span data-ttu-id="7840f-178">Sydsudan</span><span class="sxs-lookup"><span data-stu-id="7840f-178">South Sudan</span></span>  
- <span data-ttu-id="7840f-179">Tadzjikistan</span><span class="sxs-lookup"><span data-stu-id="7840f-179">Tajikistan</span></span> 
- <span data-ttu-id="7840f-180">Thailand</span><span class="sxs-lookup"><span data-stu-id="7840f-180">Thailand</span></span>
- <span data-ttu-id="7840f-181">Turkiet</span><span class="sxs-lookup"><span data-stu-id="7840f-181">Turkey</span></span> 
- <span data-ttu-id="7840f-182">Ukraina</span><span class="sxs-lookup"><span data-stu-id="7840f-182">Ukraine</span></span> 
- <span data-ttu-id="7840f-183">Förenade Arabemiraten</span><span class="sxs-lookup"><span data-stu-id="7840f-183">United Arab Emirates</span></span> 
- <span data-ttu-id="7840f-184">Uzbekistan</span><span class="sxs-lookup"><span data-stu-id="7840f-184">Uzbekistan</span></span> 
- <span data-ttu-id="7840f-185">Venezuela</span><span class="sxs-lookup"><span data-stu-id="7840f-185">Venezuela</span></span>
- <span data-ttu-id="7840f-186">Vietnam</span><span class="sxs-lookup"><span data-stu-id="7840f-186">Vietnam</span></span> 


<span data-ttu-id="7840f-187">Mer information finns i Informationen om [registrerings-ID-nummer](reg-number-id.md)</span><span class="sxs-lookup"><span data-stu-id="7840f-187">For more information, read [Registration ID number information](reg-number-id.md)</span></span>

## <a name="delete-a-location"></a><span data-ttu-id="7840f-188">Ta bort en plats</span><span class="sxs-lookup"><span data-stu-id="7840f-188">Delete a location</span></span>

<span data-ttu-id="7840f-189">Om du vill ta bort en plats från ditt konto måste du kontakta [partnersupporten.](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=1af7f3a0-1757-3543-4b6a-c945c3ad187b)</span><span class="sxs-lookup"><span data-stu-id="7840f-189">To delete a location from your account, you will need to contact [Partner Support](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=1af7f3a0-1757-3543-4b6a-c945c3ad187b).</span></span> <span data-ttu-id="7840f-190">Se till att du förstår vilken effekt den här åtgärden har.</span><span class="sxs-lookup"><span data-stu-id="7840f-190">Make sure that you understand the impact this action has.</span></span> <span data-ttu-id="7840f-191">Borttagna platser kan inte hämtas och allt som är kopplat till det specifika MPN-ID:t kommer inte längre att identifieras eller vara aktivt för ditt företag.</span><span class="sxs-lookup"><span data-stu-id="7840f-191">Deleted locations cannot be retrieved and anything tied to that specific MPN ID will no longer be recognized or be active for your company.</span></span>

## <a name="change-country-of-partner-global-account"></a><span data-ttu-id="7840f-192">Ändra land för partnerns globala konto</span><span class="sxs-lookup"><span data-stu-id="7840f-192">Change country of Partner global account</span></span> 

1. <span data-ttu-id="7840f-193">Logga in med MPN-kontot i Partnercenter.</span><span class="sxs-lookup"><span data-stu-id="7840f-193">Sign in using the MPN account in Partner Center.</span></span> <span data-ttu-id="7840f-194">(Dina MPN-autentiseringsuppgifter kan vara annorlunda än dina CSP-autentiseringsuppgifter.) MPN-kontot ska ha behörigheter som global administratör eller kontoadministratör.</span><span class="sxs-lookup"><span data-stu-id="7840f-194">(Your MPN credentials may be different from your CSP credentials.) The MPN account should have Global Admin or Account Admin privileges.</span></span> 

2. <span data-ttu-id="7840f-195">På fliken **Partner** går du till **Företagsplatser** och kontrollerar listan över platser för att se till att den plats som du vill använda som juridisk enhet visas.</span><span class="sxs-lookup"><span data-stu-id="7840f-195">On the **Partner** tab, go to **Business locations** and check the list of locations to ensure that the location you want as your legal entity is listed.</span></span> 
 
1. <span data-ttu-id="7840f-196">Om du vill lägga till en plats klickar du på Lägg till en plats och anger nödvändig information, inklusive företagsnamn, adress och primär kontakt för den plats som du vill lägga till i företaget.</span><span class="sxs-lookup"><span data-stu-id="7840f-196">To add a location, click **Add a location**, and, in the fly out, provide the required details including business name, address, and primary contact for the location that you want to add to your company.</span></span> 
 
1. <span data-ttu-id="7840f-197">Välj **Ändra land** bredvid **listrutan Land/region** och följ stegen.</span><span class="sxs-lookup"><span data-stu-id="7840f-197">Select **Change your country** next to the **Country/region** drop-down list and follow the steps.</span></span> 

:::image type="content" source="images/lbp.png" alt-text="Data om juridiska affärsprofiler samlas in.":::

5. <span data-ttu-id="7840f-199">Välj **Spara**.</span><span class="sxs-lookup"><span data-stu-id="7840f-199">Select **Save**.</span></span>

6. <span data-ttu-id="7840f-200">MPN:s globala kontoland ändras till det nya juridiska landet.</span><span class="sxs-lookup"><span data-stu-id="7840f-200">MPN global account country will be changed to the new legal country.</span></span>
  
## <a name="next-steps"></a><span data-ttu-id="7840f-201">Nästa steg</span><span class="sxs-lookup"><span data-stu-id="7840f-201">Next steps</span></span>

- <span data-ttu-id="7840f-202">Läs mer om [verifieringsprocessen](verification-responses.md).</span><span class="sxs-lookup"><span data-stu-id="7840f-202">Learn about the [verification process](verification-responses.md).</span></span>
