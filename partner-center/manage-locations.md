---
title: Hantera platser i ditt partner konto
ms.topic: how-to
ms.date: 04/05/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Lär dig hur du lägger till en ny plats och hur plats MPN ID används i stimulans program, CSP-verksamhet, prenumerationer och andra transaktioner.
author: vinayks
ms.author: vinayks
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 7ca8c866479fbe153c1e0192edd33e8258b9d6e7
ms.sourcegitcommit: 3c26a61982082787bbdaf5d1e92553b26f3a5076
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/06/2021
ms.locfileid: "106441343"
---
# <a name="manage-your-mpn-account-locations-and-add-delete-a-location"></a><span data-ttu-id="7be01-103">Hantera dina MPN-konto platser och lägga till (ta bort) en plats</span><span class="sxs-lookup"><span data-stu-id="7be01-103">Manage your MPN account locations and add (delete) a location</span></span>


<span data-ttu-id="7be01-104">**Lämpliga roller**</span><span class="sxs-lookup"><span data-stu-id="7be01-104">**Appropriate roles**</span></span>

- <span data-ttu-id="7be01-105">Global administratör</span><span class="sxs-lookup"><span data-stu-id="7be01-105">Global admin</span></span>
- <span data-ttu-id="7be01-106">Kontoadministratör</span><span class="sxs-lookup"><span data-stu-id="7be01-106">Account admin</span></span>

<span data-ttu-id="7be01-107">Platsens MPN-ID identifierar varje enskild plats för ditt företag.</span><span class="sxs-lookup"><span data-stu-id="7be01-107">The location MPN ID identifies each specific location of your company.</span></span> <span data-ttu-id="7be01-108">Du kan använda platsens MPN-ID för att registrera dig för stimulans program, till Transact Cloud Solution Provider (CSP) Business och andra affärs transaktioner.</span><span class="sxs-lookup"><span data-stu-id="7be01-108">You use the location MPN ID to enroll in incentive programs, to transact Cloud Solution Provider (CSP) business, and other business transactions.</span></span> <span data-ttu-id="7be01-109">Det globala MPN-ID: t används för icke-transaktionella aktiviteter, till exempel support förfrågningar.</span><span class="sxs-lookup"><span data-stu-id="7be01-109">The global MPN ID is used for non-transactional activities such as support requests.</span></span>

## <a name="the-following-scenario-is-typical"></a><span data-ttu-id="7be01-110">Följande scenario är vanligt:</span><span class="sxs-lookup"><span data-stu-id="7be01-110">The following scenario is typical:</span></span>

<span data-ttu-id="7be01-111">Contoso har sitt globala partner konto (PGA) i Storbritannien.</span><span class="sxs-lookup"><span data-stu-id="7be01-111">Contoso has its Partner global account (PGA) in the UK.</span></span> <span data-ttu-id="7be01-112">PGA är sitt registrerade juridiska företag och det globala MPN-ID: t används för att hantera all icke-transaktionell verksamhet.</span><span class="sxs-lookup"><span data-stu-id="7be01-112">The PGA is their registered legal business, and it's global MPN ID is used for managing all non-transactional business.</span></span> <span data-ttu-id="7be01-113">Contoso har även ett konto för partner lokalisering (PLA) som motsvarar dotter bolag eller divisioner på en annan plats i Storbritannien, Frankrike och USA.</span><span class="sxs-lookup"><span data-stu-id="7be01-113">Contoso also has Partner location accounts (PLA) equivalent to subsidiaries or divisions in another location in the UK, France, and the USA.</span></span> <span data-ttu-id="7be01-114">I MPN-konto strukturen visas dessa PLAs som unika plats MPN-ID: n.</span><span class="sxs-lookup"><span data-stu-id="7be01-114">In the MPN Account structure, these PLAs are represented as unique location MPN IDs.</span></span> <span data-ttu-id="7be01-115">PLAs används för transaktions företag som CSP eller incitaments program.</span><span class="sxs-lookup"><span data-stu-id="7be01-115">The PLAs are used for transactional business such as CSP or incentives programs.</span></span> <span data-ttu-id="7be01-116">Utbetalningar är knutna till vissa platser.</span><span class="sxs-lookup"><span data-stu-id="7be01-116">Payouts are tied to specific locations.</span></span> 

>[!NOTE]
><span data-ttu-id="7be01-117">Det finns en 1-1-relation mellan en CSP-klient och en MPN plats-ID.</span><span class="sxs-lookup"><span data-stu-id="7be01-117">There is a 1-1 relationship between a CSP tenant and an MPN location ID.</span></span>

:::image type="content" source="images/locations/locations1.png" alt-text="Struktur för MPN-platser":::

## <a name="prerequisites-in-order-to-add-a-new-account-for-a-csp-business"></a><span data-ttu-id="7be01-119">Krav för att lägga till ett nytt konto för en CSP-verksamhet</span><span class="sxs-lookup"><span data-stu-id="7be01-119">Prerequisites in order to add a new account for a CSP business</span></span>

<span data-ttu-id="7be01-120">Om du vill lägga till ett nytt CSP-affärskonto börjar du med att se till att du uppfyller kraven.</span><span class="sxs-lookup"><span data-stu-id="7be01-120">To add a new CSP business account, start by ensuring that you have fulfilled the prerequisites.</span></span>

1. <span data-ttu-id="7be01-121">Du måste ha ett plats MPN-ID i det land där du vill göra CSP-verksamhet.</span><span class="sxs-lookup"><span data-stu-id="7be01-121">You must have a location MPN ID in the country where you want to do CSP business.</span></span> <span data-ttu-id="7be01-122">Om du vill skapa en ny MPN plats läser du "Lägg till en MPN plats" nedan.</span><span class="sxs-lookup"><span data-stu-id="7be01-122">To create a new MPN location, read “Add an MPN location” below.</span></span>
  
1. <span data-ttu-id="7be01-123">Om du vill skapa en ny CSP indirekt åter försäljares registrering, Läs [arbeta med indirekta leverantörer](indirect-reseller-tasks-in-partner-center.md#get-started)</span><span class="sxs-lookup"><span data-stu-id="7be01-123">To create a new CSP Indirect Reseller enrollment, read [Work with Indirect providers](indirect-reseller-tasks-in-partner-center.md#get-started)</span></span> 

>[!NOTE] 
 ><span data-ttu-id="7be01-124">Kom ihåg att logga in med de **nya** autentiseringsuppgifterna för det **nya** CSP-kontot.</span><span class="sxs-lookup"><span data-stu-id="7be01-124">Remember to sign in with the **new** credentials for the **new** CSP account.</span></span> <span data-ttu-id="7be01-125">Använd inte dina befintliga autentiseringsuppgifter eftersom Partner Center känner igen att du redan har ett konto.</span><span class="sxs-lookup"><span data-stu-id="7be01-125">Don't use your existing credentials as Partner Center will recognize you as already having an account.</span></span>

2. <span data-ttu-id="7be01-126">Godkänn Microsoft partner Agreement och aktivera kontot.</span><span class="sxs-lookup"><span data-stu-id="7be01-126">Accept the Microsoft Partner Agreement and activate the account.</span></span>

1. <span data-ttu-id="7be01-127">Läs [krav för direkt fakturerings](direct-partner-new-requirements.md) partner om du vill registrera dig som en direkt fakturerings partner</span><span class="sxs-lookup"><span data-stu-id="7be01-127">If you want to enroll as a Direct Bill partner, read [Requirements for Direct Bill partners](direct-partner-new-requirements.md)</span></span>

## <a name="view-your-mpn-locations"></a><span data-ttu-id="7be01-128">Visa dina MPN-platser</span><span class="sxs-lookup"><span data-stu-id="7be01-128">View your MPN locations</span></span>

1. <span data-ttu-id="7be01-129">Logga in på [instrument panelen](https://partner.microsoft.com/dashboard/home) för partner Center med dina MPN-kontoautentiseringsuppgifter.</span><span class="sxs-lookup"><span data-stu-id="7be01-129">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard/home) with your MPN account credentials.</span></span> <span data-ttu-id="7be01-130">(Dina MPN-autentiseringsuppgifter kan skilja sig från dina autentiseringsuppgifter för CSP)</span><span class="sxs-lookup"><span data-stu-id="7be01-130">(Your MPN credentials may be different from your CSP credentials)</span></span> 
 
1. <span data-ttu-id="7be01-131">I **inställnings** ikonen väljer du **konto inställningar**, **organisations profil**, **Legal**.</span><span class="sxs-lookup"><span data-stu-id="7be01-131">From the **Settings** icon, select **Account settings**, **Organization profile**, **Legal**.</span></span> 

1. <span data-ttu-id="7be01-132">På fliken **partner** kontrollerar du att det inte finns ett informations fel meddelande som ber dig att åtgärda migrerade platser från PMC.</span><span class="sxs-lookup"><span data-stu-id="7be01-132">On the **Partner** tab, verify that there isn't a banner error message asking you to fix migrated locations from PMC.</span></span>  <span data-ttu-id="7be01-133">Om dina platser inte har ställts in korrekt i PMC och inte har övergått till dator än PC måste du uppdatera dessa platser.</span><span class="sxs-lookup"><span data-stu-id="7be01-133">If your locations were not set up correctly in PMC, and have not transitioned yet to PC, you need to update those locations.</span></span>

:::image type="content" source="images/locations/location-two.png" alt-text="Skärm bild visar hur du uppdaterar platsen.":::
 
4.  <span data-ttu-id="7be01-135">På skärmen **Granska PMC-platser** väljer du **Uppdatera**.</span><span class="sxs-lookup"><span data-stu-id="7be01-135">On the **Review PMC locations** screen, select **Update**.</span></span>
<span data-ttu-id="7be01-136">Uppdatera följande fält:</span><span class="sxs-lookup"><span data-stu-id="7be01-136">Update the following fields:</span></span>

- <span data-ttu-id="7be01-137">**Namnfält**: kontrol lera att namnet på företags platsen är korrekt.</span><span class="sxs-lookup"><span data-stu-id="7be01-137">**Name field**: Make sure that the name of the company location is correct.</span></span> <span data-ttu-id="7be01-138">Om ett duplicerat fel visas kan du försöka ändra från, till exempel contoso till contoso, Inc.</span><span class="sxs-lookup"><span data-stu-id="7be01-138">If a duplicate error is displayed, try changing from, for example, Contoso to Contoso, Inc.</span></span>

- <span data-ttu-id="7be01-139">**Fält för juridisk person**: kontrol lera att du har valt den juridiska personen som platsen är kopplad till</span><span class="sxs-lookup"><span data-stu-id="7be01-139">**Legal Entity field**: Make sure that you have chosen the legal entity the location is tied to</span></span>

- <span data-ttu-id="7be01-140">**Adress rad 1 & 2 fält**: kontrol lera att adressen är korrekt</span><span class="sxs-lookup"><span data-stu-id="7be01-140">**Address line 1 & 2 fields**: Make sure that the address is correct</span></span>

- <span data-ttu-id="7be01-141">**Fälten ort & delstat/provins**: se till att kombinationen mellan staden och regionen är korrekt.</span><span class="sxs-lookup"><span data-stu-id="7be01-141">**City & State/Province fields**: Make sure the combination between the city and the state/province is correct.</span></span> <span data-ttu-id="7be01-142">Det finns länder där List menyn för att välja delstat/provins ska tillämpas och i andra länder måste fältet infogas manuellt.</span><span class="sxs-lookup"><span data-stu-id="7be01-142">There are countries where the dropdown menu for choosing the State/Province will apply, and in other countries that field will need to manually be inserted.</span></span>

- <span data-ttu-id="7be01-143">**Fält för post** nummer: kontrol lera att post nummer fältet matchar ditt angivna land, region, ort eller adress.</span><span class="sxs-lookup"><span data-stu-id="7be01-143">**ZIP/ Postal code field**: Make sure the Zip Code field is matching your indicated Country, Region, City, or Address.</span></span>

- <span data-ttu-id="7be01-144">**Fält för primär kontakt information**: se till att fälten för första och sista namn är fyllda och att den angivna e-postadressen är en e-postadress för arbetet och inte en personlig (t @outlook.com . ex., @live.com osv.)</span><span class="sxs-lookup"><span data-stu-id="7be01-144">**Primary contact information fields**: Make sure the first and last name fields are filled and that the e-mail address indicated is a work e-mail address and not a personal one (for example, @outlook.com, @live.com, etc.)</span></span>

- <span data-ttu-id="7be01-145">**Telefonnummer fält**: kontrol lera att telefonnumret inte innehåller specialtecken, mellanslag eller landskod.</span><span class="sxs-lookup"><span data-stu-id="7be01-145">**Phone number field**: Make sure that the Phone number does NOT include special characters, spaces, or country code.</span></span> <span data-ttu-id="7be01-146">Värdet som anges i fältet telefonnummer får alltid innehålla högst 10 tecken.</span><span class="sxs-lookup"><span data-stu-id="7be01-146">The value entered in the Phone Number field will always contain a maximum of 10 characters.</span></span>

5. <span data-ttu-id="7be01-147">Om det inte finns något fel meddelande väljer du **konto inställningar**, **organisations profil** och **identifierare** i **Inställningar**.</span><span class="sxs-lookup"><span data-stu-id="7be01-147">If there isn't an error message, then from  **Settings**, select  **Account Settings**, **Organization profile**, **Identifiers**.</span></span>

6. <span data-ttu-id="7be01-148">Hitta MPN-ID: t med typen "location" som matchar landet för det här CSP-kontot och Använd det för att slutföra associationen.</span><span class="sxs-lookup"><span data-stu-id="7be01-148">Find the MPN ID with Type "Location" that matches the country of this CSP account and use it to complete the association.</span></span>

7. <span data-ttu-id="7be01-149">Om du inte hittar platsens MPN-ID som matchar det CSP-konto som du vill använda, kan du lägga till en ny plats, vilket skapar ett nytt MPN-ID.</span><span class="sxs-lookup"><span data-stu-id="7be01-149">If you can’t find the location MPN ID that matches the CSP account you want to use, you can add a new location, which will create a new MPN ID.</span></span> <span data-ttu-id="7be01-150">Se **lägga till en MPN plats** nedan.</span><span class="sxs-lookup"><span data-stu-id="7be01-150">See **Add an MPN location** below.</span></span>

## <a name="add-an-mpn-location"></a><span data-ttu-id="7be01-151">Lägg till en MPN-plats</span><span class="sxs-lookup"><span data-stu-id="7be01-151">Add an MPN location</span></span>

1. <span data-ttu-id="7be01-152">Logga in med MPN-kontot i Partner Center.</span><span class="sxs-lookup"><span data-stu-id="7be01-152">Sign in using the MPN account in Partner Center.</span></span> <span data-ttu-id="7be01-153">(Dina MPN-autentiseringsuppgifter kan skilja sig från dina autentiseringsuppgifter för din CSP).</span><span class="sxs-lookup"><span data-stu-id="7be01-153">(Your MPN credentials may be different from your CSP credentials) .</span></span> <span data-ttu-id="7be01-154">MPN-kontot ska ha global administratör eller konto administratörs behörighet.</span><span class="sxs-lookup"><span data-stu-id="7be01-154">The MPN account should have Global Admin or Account Admin privileges.</span></span> 

1. <span data-ttu-id="7be01-155">Från **inställnings ikonen** väljer du **konto inställningarna** och väljer sedan **organisations profil**.</span><span class="sxs-lookup"><span data-stu-id="7be01-155">From the **Settings icon**, select the **Account settings** and then select **Organization profile**.</span></span>

2. <span data-ttu-id="7be01-156">Välj **juridiskt** och sedan på fliken **partner** väljer du **företags platser** och klickar på **Lägg till en plats.**</span><span class="sxs-lookup"><span data-stu-id="7be01-156">Select **Legal** and then, on the **Partner** tab, select **Business locations,** and click on **Add a location.**</span></span>

3. <span data-ttu-id="7be01-157">Ange nödvändig information, inklusive företags namn, adress och kontakt för den plats som du vill lägga till i företaget.</span><span class="sxs-lookup"><span data-stu-id="7be01-157">Provide the required details including business name, address, and contact for the location that you want to add to your company.</span></span>
 
1. <span data-ttu-id="7be01-158">Klicka på **Lägg till plats**.</span><span class="sxs-lookup"><span data-stu-id="7be01-158">Click **Add location**.</span></span> <span data-ttu-id="7be01-159">Då skapas ett nytt MPN-ID för den nya platsen som du kan använda för CSP-transaktioner och-incitament.</span><span class="sxs-lookup"><span data-stu-id="7be01-159">This will create a new MPN ID for the new location which you can use for CSP transactions and incentives.</span></span>

:::image type="content" source="images/legal-biz.png" alt-text="Lägg till en ny juridisk verksamhet":::

> [!NOTE]
> <span data-ttu-id="7be01-161">När en plats har lagts till i Partner Center kan du inte ta bort den.</span><span class="sxs-lookup"><span data-stu-id="7be01-161">Once a location is added in Partner Center, you cannot remove it.</span></span> <span data-ttu-id="7be01-162">Du kommer att se **MPN** på den vänstra menyn i Partner Center om du har använt rätt MPN-ID för att logga in.</span><span class="sxs-lookup"><span data-stu-id="7be01-162">You will see **MPN** in the left menu of Partner Center if you have used the correct MPN ID to sign in.</span></span>


## <a name="delete-a-location"></a><span data-ttu-id="7be01-163">Ta bort en plats</span><span class="sxs-lookup"><span data-stu-id="7be01-163">Delete a location</span></span>

<span data-ttu-id="7be01-164">Om du vill ta bort en plats från ditt konto måste du kontakta [partner support](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=1af7f3a0-1757-3543-4b6a-c945c3ad187b).</span><span class="sxs-lookup"><span data-stu-id="7be01-164">To delete a location from your account, you will need to contact [Partner Support](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=1af7f3a0-1757-3543-4b6a-c945c3ad187b).</span></span> <span data-ttu-id="7be01-165">Se till att du förstår den påverkan den här åtgärden har.</span><span class="sxs-lookup"><span data-stu-id="7be01-165">Make sure that you understand the impact this action has.</span></span> <span data-ttu-id="7be01-166">Det går inte att hämta borttagna platser och något som är knutet till det aktuella MPN-ID: t kan inte längre identifieras eller vara aktivt för ditt företag.</span><span class="sxs-lookup"><span data-stu-id="7be01-166">Deleted locations cannot be retrieved and anything tied to that specific MPN id will no longer be recognized or be active for your company.</span></span>

## <a name="change-country-of-partner-global-account"></a><span data-ttu-id="7be01-167">Ändra land för globalt partner konto</span><span class="sxs-lookup"><span data-stu-id="7be01-167">Change country of Partner global account</span></span> 

1. <span data-ttu-id="7be01-168">Logga in med MPN-kontot i Partner Center.</span><span class="sxs-lookup"><span data-stu-id="7be01-168">Sign in using the MPN account in Partner Center.</span></span> <span data-ttu-id="7be01-169">(Dina MPN-autentiseringsuppgifter kan skilja sig från dina autentiseringsuppgifter för din CSP).</span><span class="sxs-lookup"><span data-stu-id="7be01-169">(Your MPN credentials may be different from your CSP credentials) .</span></span> <span data-ttu-id="7be01-170">MPN-kontot ska ha global administratör eller konto administratörs behörighet.</span><span class="sxs-lookup"><span data-stu-id="7be01-170">The MPN account should have Global Admin or Account Admin privileges.</span></span> 

2. <span data-ttu-id="7be01-171">På fliken **partner** går du till **företags platser** och kontrollerar listan över platser för att se till att den plats som du vill använda som juridisk person visas.</span><span class="sxs-lookup"><span data-stu-id="7be01-171">On the **Partner** tab, go to **Business locations** and check the list of locations to ensure that the location you want as your legal entity is listed.</span></span> 
 
1. <span data-ttu-id="7be01-172">Om du vill lägga till en plats klickar du på **Lägg till en plats** och anger den information som krävs, till exempel företags namn, adress och primär kontakt för den plats som du vill lägga till i företaget.</span><span class="sxs-lookup"><span data-stu-id="7be01-172">To add a location, click **Add a location**, and, in the fly out, provide the required details including business name, address, and primary contact for the location that you want to add to your company.</span></span> 
 
1. <span data-ttu-id="7be01-173">Välj **ändra ditt land** bredvid List rutan **land/region** och följ stegen.</span><span class="sxs-lookup"><span data-stu-id="7be01-173">Select **Change your country** next to the **Country/region** drop-down and follow the steps.</span></span> 

:::image type="content" source="images/lbp.png" alt-text="Information om juridisk företags profil, flyg ut":::

5. <span data-ttu-id="7be01-175">Klicka på **Spara**.</span><span class="sxs-lookup"><span data-stu-id="7be01-175">Click **Save**.</span></span>

6. <span data-ttu-id="7be01-176">MPN globalt konto land kommer att ändras till det nya juridiska landet.</span><span class="sxs-lookup"><span data-stu-id="7be01-176">MPN global account country will be changed to the new legal country.</span></span>
  
## <a name="next-steps"></a><span data-ttu-id="7be01-177">Nästa steg</span><span class="sxs-lookup"><span data-stu-id="7be01-177">Next steps</span></span>

- <span data-ttu-id="7be01-178">Lär dig mer om [verifierings processen](verification-responses.md).</span><span class="sxs-lookup"><span data-stu-id="7be01-178">Learn about the [verification process](verification-responses.md).</span></span>
