---
title: Hantera platser i ditt partner konto
ms.topic: how-to
ms.date: 11/23/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Lär dig hur du lägger till en ny plats och hur plats MPN ID används i stimulans program, CSP-verksamhet, prenumerationer och andra transaktioner.
author: vinayks
ms.author: vinayks
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 03c4fb5a4adeb49602fe3736971e140ac6da6f4f
ms.sourcegitcommit: 245b4792e8221468f781f6effd1c9b23be05499a
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 11/24/2020
ms.locfileid: "95514810"
---
# <a name="manage-your-mpn-account-locations-and-add-a-new-location"></a><span data-ttu-id="a227f-103">Hantera dina MPN-konto platser och Lägg till en ny plats</span><span class="sxs-lookup"><span data-stu-id="a227f-103">Manage your MPN account locations and add a new location</span></span>

<span data-ttu-id="a227f-104">**Gäller för**</span><span class="sxs-lookup"><span data-stu-id="a227f-104">**Applies to**</span></span>

- <span data-ttu-id="a227f-105">Partnercenter</span><span class="sxs-lookup"><span data-stu-id="a227f-105">Partner Center</span></span>

<span data-ttu-id="a227f-106">**Lämpliga roller**</span><span class="sxs-lookup"><span data-stu-id="a227f-106">**Appropriate roles**</span></span>

- <span data-ttu-id="a227f-107">Global administratör</span><span class="sxs-lookup"><span data-stu-id="a227f-107">Global admin</span></span>
- <span data-ttu-id="a227f-108">Kontoadministratör</span><span class="sxs-lookup"><span data-stu-id="a227f-108">Account admin</span></span>

<span data-ttu-id="a227f-109">Platsens MPN-ID identifierar varje enskild plats för ditt företag.</span><span class="sxs-lookup"><span data-stu-id="a227f-109">The location MPN ID identifies each specific location of your company.</span></span> <span data-ttu-id="a227f-110">Du kan använda platsens MPN-ID för att registrera dig för stimulans program, till Transact Cloud Solution Provider (CSP) Business och andra affärs transaktioner.</span><span class="sxs-lookup"><span data-stu-id="a227f-110">You use the location MPN ID to enroll in incentive programs, to transact Cloud Solution Provider (CSP) business, and other business transactions.</span></span> <span data-ttu-id="a227f-111">Det globala MPN-ID: t används för icke-transaktionella aktiviteter, till exempel support förfrågningar.</span><span class="sxs-lookup"><span data-stu-id="a227f-111">The global MPN ID is used for non-transactional activities such as support requests.</span></span>

## <a name="the-following-is-a-typical-scenario"></a><span data-ttu-id="a227f-112">Följande är ett typiskt scenario:</span><span class="sxs-lookup"><span data-stu-id="a227f-112">The following is a typical scenario:</span></span>

<span data-ttu-id="a227f-113">Contoso har sitt globala partner konto (PGA) i Storbritannien.</span><span class="sxs-lookup"><span data-stu-id="a227f-113">Contoso has its Partner global account (PGA) in the UK.</span></span> <span data-ttu-id="a227f-114">Detta är deras registrerade juridiska verksamhet och det globala MPN-ID används för att hantera all icke-transaktionell verksamhet.</span><span class="sxs-lookup"><span data-stu-id="a227f-114">This is their registered legal business, and it's global MPN ID is used for managing all non-transactional business.</span></span> <span data-ttu-id="a227f-115">Contoso har även ett konto för partner lokalisering (PLA) som motsvarar dotter bolag eller divisioner på en annan plats i Storbritannien, Frankrike och USA.</span><span class="sxs-lookup"><span data-stu-id="a227f-115">Contoso also has Partner location accounts (PLA) equivalent to subsidiaries or divisions in another location in the UK, France, and the USA.</span></span> <span data-ttu-id="a227f-116">I MPN-konto strukturen visas dessa PLAs som unika plats MPN-ID: n.</span><span class="sxs-lookup"><span data-stu-id="a227f-116">In the MPN Account structure, these PLAs are represented as unique location MPN IDs.</span></span> <span data-ttu-id="a227f-117">PLAs används för transaktions företag som CSP eller incitaments program.</span><span class="sxs-lookup"><span data-stu-id="a227f-117">The PLAs are used for transactional business such as CSP or incentives programs.</span></span> <span data-ttu-id="a227f-118">Utbetalningar är knutna till vissa platser.</span><span class="sxs-lookup"><span data-stu-id="a227f-118">Payouts are tied to specific locations.</span></span> 

>[!NOTE]
><span data-ttu-id="a227f-119">Det finns en 1-1-relation mellan en CSP-klient och en MPN plats-ID.</span><span class="sxs-lookup"><span data-stu-id="a227f-119">There is a 1-1 relationship between a CSP tenant and an MPN location ID.</span></span>

:::image type="content" source="images/locations/locations1.png" alt-text="Struktur för MPN-platser":::

## <a name="prerequisites-in-order-to-add-a-new-location-for-a-csp-business"></a><span data-ttu-id="a227f-121">Krav för att lägga till en ny plats för en CSP-verksamhet</span><span class="sxs-lookup"><span data-stu-id="a227f-121">Prerequisites in order to add a new location for a CSP business</span></span>

<span data-ttu-id="a227f-122">För att lägga till en ny KRYPTOGRAFIPROVIDERs affärs plats finns det flera krav:</span><span class="sxs-lookup"><span data-stu-id="a227f-122">To add a new CSP business location, there are several prerequisites:</span></span>

1. <span data-ttu-id="a227f-123">Du måste ha ett plats MPN-ID i det land där du vill göra affärer.</span><span class="sxs-lookup"><span data-stu-id="a227f-123">You must have a location MPN ID in the country where you want to do business.</span></span>

1. <span data-ttu-id="a227f-124">Du behöver en ny Azure AD-klient i [affärs området](regional-authorization-overview.md) som inte redan har registrerats i CSP.</span><span class="sxs-lookup"><span data-stu-id="a227f-124">You need a new Azure AD tenant in the [region of business](regional-authorization-overview.md) which is not already enrolled into CSP.</span></span> <span data-ttu-id="a227f-125">Skapa det när du registrerar i CSP.</span><span class="sxs-lookup"><span data-stu-id="a227f-125">Create this when you enroll in CSP.</span></span>
 
3. <span data-ttu-id="a227f-126">Använd den nya AAD-klienten för att registrera i CSP-programmet i regionen.</span><span class="sxs-lookup"><span data-stu-id="a227f-126">Use the new AAD tenant to enroll into CSP program in the region.</span></span>
<span data-ttu-id="a227f-127">Ange juridisk information om företaget, inklusive juridisk företags namn, adress, primär kontakt information.</span><span class="sxs-lookup"><span data-stu-id="a227f-127">Providing legal company details including the legal company name, address, primary contact details.</span></span> <span data-ttu-id="a227f-128">Det här kontot kommer att genomgå verifiering, så se till att lägga till giltig information.</span><span class="sxs-lookup"><span data-stu-id="a227f-128">This account will undergo verification, so make sure to add valid information.</span></span>

>[!NOTE] 
 ><span data-ttu-id="a227f-129">Kom ihåg att logga in med de **nya** autentiseringsuppgifterna för den **nya** Azure AD-klienten.</span><span class="sxs-lookup"><span data-stu-id="a227f-129">Remember to sign in with the **new** credentials for the **new** Azure AD tenant.</span></span> <span data-ttu-id="a227f-130">Använd inte dina befintliga autentiseringsuppgifter eftersom Partner Center känner igen att du redan har ett konto.</span><span class="sxs-lookup"><span data-stu-id="a227f-130">Don't use your existing credentials as Partner Center will recognize you as already having an account.</span></span>

4. <span data-ttu-id="a227f-131">Godkänn Microsoft partner Agreement och aktivera kontot.</span><span class="sxs-lookup"><span data-stu-id="a227f-131">Accept the Microsoft Partner Agreement and activate the account.</span></span>

## <a name="add-an-mpn-location"></a><span data-ttu-id="a227f-132">Lägg till en MPN-plats</span><span class="sxs-lookup"><span data-stu-id="a227f-132">Add an MPN location</span></span>

1. <span data-ttu-id="a227f-133">Logga in med MPN-kontot i Partner Center.</span><span class="sxs-lookup"><span data-stu-id="a227f-133">Sign in using the MPN account in Partner Center .</span></span> <span data-ttu-id="a227f-134">MPN-kontot ska ha global administratör eller konto administratörs behörighet.</span><span class="sxs-lookup"><span data-stu-id="a227f-134">The MPN account should have Global Admin or Account Admin privileges.</span></span> 

1. <span data-ttu-id="a227f-135">I **inställnings ikonen** väljer du **organisations inställningarna**.</span><span class="sxs-lookup"><span data-stu-id="a227f-135">From the **Setting icon**, select the **Organization settings**.</span></span>

2. <span data-ttu-id="a227f-136">Välj **juridiskt** och välj sedan **platser.**</span><span class="sxs-lookup"><span data-stu-id="a227f-136">Select **Legal** and then select **Locations.**</span></span>

3. <span data-ttu-id="a227f-137">Välj **Lägg till en plats** och Infoga adress information för den plats som du vill lägga till i företaget samt en primär kontakt för platsen.</span><span class="sxs-lookup"><span data-stu-id="a227f-137">Select **Add a location**, and insert the address details of the location that you want to add to your company as well as a primary contact for the location.</span></span>

> [!NOTE]
> <span data-ttu-id="a227f-138">Det går inte att ta bort en plats som har lagts till i Partner Center.</span><span class="sxs-lookup"><span data-stu-id="a227f-138">Once a location is added in Partner Center, it cannot be removed.</span></span> <span data-ttu-id="a227f-139">Du kommer att se **MPN** på den vänstra menyn i Partner Center om du har använt rätt MPN-ID för att logga in.</span><span class="sxs-lookup"><span data-stu-id="a227f-139">You will see **MPN** in the left menu of Partner Center if you have used the correct MPN ID to sign in.</span></span>

## <a name="change-global-partner-account-location"></a><span data-ttu-id="a227f-140">Ändra plats för global partner konto</span><span class="sxs-lookup"><span data-stu-id="a227f-140">Change Global partner account location</span></span>

1. <span data-ttu-id="a227f-141">På **[företags platser](https://partner.microsoft.com/dashboard/account/v3/organization/legalinfo#mpn)** kontrollerar du listan över platser för att se till att den plats som du vill använda som juridisk person visas.</span><span class="sxs-lookup"><span data-stu-id="a227f-141">On **[Business locations](https://partner.microsoft.com/dashboard/account/v3/organization/legalinfo#mpn)**, check the list of locations to ensure that the location you want as your legal entity is listed.</span></span> <span data-ttu-id="a227f-142">Om den inte är det lägger du till den.</span><span class="sxs-lookup"><span data-stu-id="a227f-142">If it isn't, add it.</span></span>

   :::image type="content" source="images/accountsettings/location1.png" alt-text="Skärm bild av sidan för konto platser i Partner Center med en lista över alla aktuella platser.":::

2. <span data-ttu-id="a227f-144">Välj **juridisk** information och välj sedan **Uppdatera juridisk företags profil**</span><span class="sxs-lookup"><span data-stu-id="a227f-144">Select **Legal** and then select **Update legal business profile**</span></span>
  
3. <span data-ttu-id="a227f-145">Välj region och juridisk person och **Skicka** den.</span><span class="sxs-lookup"><span data-stu-id="a227f-145">Select the region and legal entity and **Submit** it.</span></span>

  
## <a name="next-steps"></a><span data-ttu-id="a227f-146">Nästa steg</span><span class="sxs-lookup"><span data-stu-id="a227f-146">Next steps</span></span>

- <span data-ttu-id="a227f-147">Lär dig mer om [verifierings processen](verification-responses.md).</span><span class="sxs-lookup"><span data-stu-id="a227f-147">Learn about the [verification process](verification-responses.md).</span></span>
