---
title: Hantera platser i ditt partner konto
ms.topic: how-to
ms.date: 01/26/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Lär dig hur du lägger till en ny plats och hur plats MPN ID används i stimulans program, CSP-verksamhet, prenumerationer och andra transaktioner.
author: vinayks
ms.author: vinayks
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 21d82fc3ec4470d4941d3ca7436089d3e892439e
ms.sourcegitcommit: 81017727107a907bf1f3246097b51667d7c5fb18
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 01/30/2021
ms.locfileid: "99098898"
---
# <a name="manage-your-mpn-account-locations-and-add-a-new-location"></a><span data-ttu-id="3b916-103">Hantera dina MPN-konto platser och Lägg till en ny plats</span><span class="sxs-lookup"><span data-stu-id="3b916-103">Manage your MPN account locations and add a new location</span></span>


<span data-ttu-id="3b916-104">**Lämpliga roller**</span><span class="sxs-lookup"><span data-stu-id="3b916-104">**Appropriate roles**</span></span>

- <span data-ttu-id="3b916-105">Global administratör</span><span class="sxs-lookup"><span data-stu-id="3b916-105">Global admin</span></span>
- <span data-ttu-id="3b916-106">Kontoadministratör</span><span class="sxs-lookup"><span data-stu-id="3b916-106">Account admin</span></span>

<span data-ttu-id="3b916-107">Platsens MPN-ID identifierar varje enskild plats för ditt företag.</span><span class="sxs-lookup"><span data-stu-id="3b916-107">The location MPN ID identifies each specific location of your company.</span></span> <span data-ttu-id="3b916-108">Du kan använda platsens MPN-ID för att registrera dig för stimulans program, till Transact Cloud Solution Provider (CSP) Business och andra affärs transaktioner.</span><span class="sxs-lookup"><span data-stu-id="3b916-108">You use the location MPN ID to enroll in incentive programs, to transact Cloud Solution Provider (CSP) business, and other business transactions.</span></span> <span data-ttu-id="3b916-109">Det globala MPN-ID: t används för icke-transaktionella aktiviteter, till exempel support förfrågningar.</span><span class="sxs-lookup"><span data-stu-id="3b916-109">The global MPN ID is used for non-transactional activities such as support requests.</span></span>

## <a name="the-following-is-a-typical-scenario"></a><span data-ttu-id="3b916-110">Följande är ett typiskt scenario:</span><span class="sxs-lookup"><span data-stu-id="3b916-110">The following is a typical scenario:</span></span>

<span data-ttu-id="3b916-111">Contoso har sitt globala partner konto (PGA) i Storbritannien.</span><span class="sxs-lookup"><span data-stu-id="3b916-111">Contoso has its Partner global account (PGA) in the UK.</span></span> <span data-ttu-id="3b916-112">Detta är deras registrerade juridiska verksamhet och det globala MPN-ID används för att hantera all icke-transaktionell verksamhet.</span><span class="sxs-lookup"><span data-stu-id="3b916-112">This is their registered legal business, and it's global MPN ID is used for managing all non-transactional business.</span></span> <span data-ttu-id="3b916-113">Contoso har även ett konto för partner lokalisering (PLA) som motsvarar dotter bolag eller divisioner på en annan plats i Storbritannien, Frankrike och USA.</span><span class="sxs-lookup"><span data-stu-id="3b916-113">Contoso also has Partner location accounts (PLA) equivalent to subsidiaries or divisions in another location in the UK, France, and the USA.</span></span> <span data-ttu-id="3b916-114">I MPN-konto strukturen visas dessa PLAs som unika plats MPN-ID: n.</span><span class="sxs-lookup"><span data-stu-id="3b916-114">In the MPN Account structure, these PLAs are represented as unique location MPN IDs.</span></span> <span data-ttu-id="3b916-115">PLAs används för transaktions företag som CSP eller incitaments program.</span><span class="sxs-lookup"><span data-stu-id="3b916-115">The PLAs are used for transactional business such as CSP or incentives programs.</span></span> <span data-ttu-id="3b916-116">Utbetalningar är knutna till vissa platser.</span><span class="sxs-lookup"><span data-stu-id="3b916-116">Payouts are tied to specific locations.</span></span> 

>[!NOTE]
><span data-ttu-id="3b916-117">Det finns en 1-1-relation mellan en CSP-klient och en MPN plats-ID.</span><span class="sxs-lookup"><span data-stu-id="3b916-117">There is a 1-1 relationship between a CSP tenant and an MPN location ID.</span></span>

:::image type="content" source="images/locations/locations1.png" alt-text="Struktur för MPN-platser":::

## <a name="prerequisites-in-order-to-add-a-new-account-for-a-csp-business"></a><span data-ttu-id="3b916-119">Krav för att lägga till ett nytt konto för en CSP-verksamhet</span><span class="sxs-lookup"><span data-stu-id="3b916-119">Prerequisites in order to add a new account for a CSP business</span></span>

<span data-ttu-id="3b916-120">Om du vill lägga till ett nytt CSP-affärskonto börjar du med att se till att du uppfyller kraven.</span><span class="sxs-lookup"><span data-stu-id="3b916-120">To add a new CSP business account, start by ensuring that you have fulfilled the prerequisites.</span></span>

1. <span data-ttu-id="3b916-121">Du måste ha ett plats MPN-ID i det land där du vill göra CSP-verksamhet.</span><span class="sxs-lookup"><span data-stu-id="3b916-121">You must have a location MPN ID in the country where you want to do CSP business.</span></span> <span data-ttu-id="3b916-122">Om du vill skapa en ny MPN plats läser du "Lägg till en MPN plats" nedan.</span><span class="sxs-lookup"><span data-stu-id="3b916-122">To create a new MPN location, read “Add an MPN location” below.</span></span>
  
1. <span data-ttu-id="3b916-123">Om du vill skapa en ny CSP indirekt åter försäljares registrering, Läs [arbeta med indirekta leverantörer](indirect-reseller-tasks-in-partner-center.md#get-started)</span><span class="sxs-lookup"><span data-stu-id="3b916-123">To create a new CSP Indirect Reseller enrollment, read [Work with Indirect providers](indirect-reseller-tasks-in-partner-center.md#get-started)</span></span> 

>[!NOTE] 
 ><span data-ttu-id="3b916-124">Kom ihåg att logga in med de **nya** autentiseringsuppgifterna för det **nya** CSP-kontot.</span><span class="sxs-lookup"><span data-stu-id="3b916-124">Remember to sign in with the **new** credentials for the **new** CSP account.</span></span> <span data-ttu-id="3b916-125">Använd inte dina befintliga autentiseringsuppgifter eftersom Partner Center känner igen att du redan har ett konto.</span><span class="sxs-lookup"><span data-stu-id="3b916-125">Don't use your existing credentials as Partner Center will recognize you as already having an account.</span></span>

2. <span data-ttu-id="3b916-126">Godkänn Microsoft partner Agreement och aktivera kontot.</span><span class="sxs-lookup"><span data-stu-id="3b916-126">Accept the Microsoft Partner Agreement and activate the account.</span></span>

## <a name="view-your-mpn-locations"></a><span data-ttu-id="3b916-127">Visa dina MPN-platser</span><span class="sxs-lookup"><span data-stu-id="3b916-127">View your MPN locations</span></span>

1. <span data-ttu-id="3b916-128">Logga in på [instrument panelen](https://partner.microsoft.com/dashboard/home) för partner Center med dina MPN-kontoautentiseringsuppgifter.</span><span class="sxs-lookup"><span data-stu-id="3b916-128">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard/home) with your MPN account credentials.</span></span> <span data-ttu-id="3b916-129">(Dina MPN-autentiseringsuppgifter kan skilja sig från dina autentiseringsuppgifter för CSP)</span><span class="sxs-lookup"><span data-stu-id="3b916-129">(Your MPN credentials may be different from your CSP credentials)</span></span> 
 
1. <span data-ttu-id="3b916-130">I **inställnings** ikonen väljer du **konto inställningar**, **organisations profil**, **Legal**.</span><span class="sxs-lookup"><span data-stu-id="3b916-130">From the **Settings** icon, select **Account settings**, **Organization profile**, **Legal**.</span></span> 

1. <span data-ttu-id="3b916-131">På fliken **partner** kontrollerar du att det inte finns något informations fel meddelande som ber dig att åtgärda migrerade platser från PMC.</span><span class="sxs-lookup"><span data-stu-id="3b916-131">On the **Partner** tab verify that there isn't a banner error message asking you to fix migrated locations from PMC.</span></span> <span data-ttu-id="3b916-132">Följ anvisningarna och åtgärda dessa platser.</span><span class="sxs-lookup"><span data-stu-id="3b916-132">If there is, follow instructions and fix those locations.</span></span> 

3. <span data-ttu-id="3b916-133">Om det inte finns något fel meddelande väljer du **konto inställningar**, **organisations profil** och **identifierare** i **Inställningar**.</span><span class="sxs-lookup"><span data-stu-id="3b916-133">If there isn't an error message, then from  **Settings**, select  **Account Settings**, **Organization profile**, **Identifiers**.</span></span>

4. <span data-ttu-id="3b916-134">Hitta MPN-ID: t med typen "location" som stämmer överens med det här CSP-kontots land och Använd det för att söka efter och slutföra associationen.</span><span class="sxs-lookup"><span data-stu-id="3b916-134">Find the MPN ID with Type "Location" that matches the country of this CSP account and use it to search below and complete association.</span></span>

5. <span data-ttu-id="3b916-135">Om du inte hittar platsens MPN-ID som matchar det CSP-konto som du vill använda, kan du lägga till en ny plats som skapar ett nytt MPN-ID.</span><span class="sxs-lookup"><span data-stu-id="3b916-135">If you can’t find the location MPN ID that matches the CSP account you want to use, you can add a new location which will create a new MPN ID.</span></span> <span data-ttu-id="3b916-136">Se **lägga till en MPN plats** nedan.</span><span class="sxs-lookup"><span data-stu-id="3b916-136">See **Add an MPN location** below.</span></span>

## <a name="add-an-mpn-location"></a><span data-ttu-id="3b916-137">Lägg till en MPN-plats</span><span class="sxs-lookup"><span data-stu-id="3b916-137">Add an MPN location</span></span>

1. <span data-ttu-id="3b916-138">Logga in med MPN-kontot i Partner Center.</span><span class="sxs-lookup"><span data-stu-id="3b916-138">Sign in using the MPN account in Partner Center.</span></span> <span data-ttu-id="3b916-139">(Dina MPN-autentiseringsuppgifter kan skilja sig från dina autentiseringsuppgifter för din CSP).</span><span class="sxs-lookup"><span data-stu-id="3b916-139">(Your MPN credentials may be different from your CSP credentials) .</span></span> <span data-ttu-id="3b916-140">MPN-kontot ska ha global administratör eller konto administratörs behörighet.</span><span class="sxs-lookup"><span data-stu-id="3b916-140">The MPN account should have Global Admin or Account Admin privileges.</span></span> 

1. <span data-ttu-id="3b916-141">Från **inställnings ikonen** väljer du **konto inställningarna** och väljer sedan **organisations profil**.</span><span class="sxs-lookup"><span data-stu-id="3b916-141">From the **Settings icon**, select the **Account settings** and then select **Organization profile**.</span></span>

2. <span data-ttu-id="3b916-142">Välj **juridiskt** och sedan på fliken **partner** väljer du **företags platser** och klickar på **Lägg till en plats.**</span><span class="sxs-lookup"><span data-stu-id="3b916-142">Select **Legal** and then, on the **Partner** tab, select **Business locations,** and click on **Add a location.**</span></span>

3. <span data-ttu-id="3b916-143">Ange nödvändig information, inklusive företags namn, adress och kontakt för den plats som du vill lägga till i företaget.</span><span class="sxs-lookup"><span data-stu-id="3b916-143">Provide the required details including business name, address, and contact for the location that you want to add to your company.</span></span>
 
1. <span data-ttu-id="3b916-144">Klicka på **Lägg till plats**.</span><span class="sxs-lookup"><span data-stu-id="3b916-144">Click **Add location**.</span></span> <span data-ttu-id="3b916-145">Då skapas ett nytt MPN-ID för den nya platsen som du kan använda för CSP-transaktioner och-incitament.</span><span class="sxs-lookup"><span data-stu-id="3b916-145">This will create a new MPN ID for the new location which you can use for CSP transactions and incentives.</span></span>

:::image type="content" source="images/legal-biz.png" alt-text="Lägg till en ny juridisk verksamhet":::

> [!NOTE]
> <span data-ttu-id="3b916-147">Det går inte att ta bort en plats som har lagts till i Partner Center.</span><span class="sxs-lookup"><span data-stu-id="3b916-147">Once a location is added in Partner Center, it cannot be removed.</span></span> <span data-ttu-id="3b916-148">Du kommer att se **MPN** på den vänstra menyn i Partner Center om du har använt rätt MPN-ID för att logga in.</span><span class="sxs-lookup"><span data-stu-id="3b916-148">You will see **MPN** in the left menu of Partner Center if you have used the correct MPN ID to sign in.</span></span>

## <a name="change-country-of-partner-global-account"></a><span data-ttu-id="3b916-149">Ändra land för globalt partner konto</span><span class="sxs-lookup"><span data-stu-id="3b916-149">Change country of Partner global account</span></span> 

1. <span data-ttu-id="3b916-150">Logga in med MPN-kontot i Partner Center.</span><span class="sxs-lookup"><span data-stu-id="3b916-150">Sign in using the MPN account in Partner Center.</span></span> <span data-ttu-id="3b916-151">(Dina MPN-autentiseringsuppgifter kan skilja sig från dina autentiseringsuppgifter för din CSP).</span><span class="sxs-lookup"><span data-stu-id="3b916-151">(Your MPN credentials may be different from your CSP credentials) .</span></span> <span data-ttu-id="3b916-152">MPN-kontot ska ha global administratör eller konto administratörs behörighet.</span><span class="sxs-lookup"><span data-stu-id="3b916-152">The MPN account should have Global Admin or Account Admin privileges.</span></span> 

2. <span data-ttu-id="3b916-153">På fliken **partner** går du till **företags platser** och kontrollerar listan över platser för att se till att den plats som du vill använda som juridisk person visas.</span><span class="sxs-lookup"><span data-stu-id="3b916-153">On the **Partner** tab, go to **Business locations** and check the list of locations to ensure that the location you want as your legal entity is listed.</span></span> 
 
1. <span data-ttu-id="3b916-154">Om du vill lägga till en plats klickar du på **Lägg till en plats** och anger den information som krävs, till exempel företags namn, adress och primär kontakt för den plats som du vill lägga till i företaget.</span><span class="sxs-lookup"><span data-stu-id="3b916-154">To add a location, click **Add a location**, and, in the fly out, provide the required details including business name, address, and primary contact for the location that you want to add to your company.</span></span> 
 
1. <span data-ttu-id="3b916-155">Välj **ändra ditt land** bredvid List rutan **land/region** och följ stegen.</span><span class="sxs-lookup"><span data-stu-id="3b916-155">Select **Change your country** next to the **Country/region** drop-down and follow the steps.</span></span> 

:::image type="content" source="images/lbp.png" alt-text="Information om juridisk företags profil, flyg ut":::

5. <span data-ttu-id="3b916-157">Klicka på **Spara**.</span><span class="sxs-lookup"><span data-stu-id="3b916-157">Click **Save**.</span></span>

6. <span data-ttu-id="3b916-158">MPN globalt konto land kommer att ändras till det nya juridiska landet.</span><span class="sxs-lookup"><span data-stu-id="3b916-158">MPN global account country will be changed to the new legal country.</span></span>
  
## <a name="next-steps"></a><span data-ttu-id="3b916-159">Nästa steg</span><span class="sxs-lookup"><span data-stu-id="3b916-159">Next steps</span></span>

- <span data-ttu-id="3b916-160">Lär dig mer om [verifierings processen](verification-responses.md).</span><span class="sxs-lookup"><span data-stu-id="3b916-160">Learn about the [verification process](verification-responses.md).</span></span>
