---
title: Skapa ett Partnercenter-konto
ms.topic: article
ms.date: 08/07/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Lär dig hur Microsoft Partner Network-medlemmar kan skapa ett partner Center-konto för att hantera sina nätverks förmåner och-kompetenser.
author: ParthP
ms.author: ParthP
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: e3f04708d3b7e2c86c88541931c120a6649674fb
ms.sourcegitcommit: 6b03ff400d1350db9696f9b457fcfe710310c5d3
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 12/03/2020
ms.locfileid: "96570798"
---
# <a name="create-a-partner-center-account-to-manage-network-benefits-and-competencies"></a><span data-ttu-id="9fa2b-103">Skapa ett partner Center-konto för att hantera nätverks förmåner och-kompetenser</span><span class="sxs-lookup"><span data-stu-id="9fa2b-103">Create a Partner Center account to manage network benefits and competencies</span></span>

<span data-ttu-id="9fa2b-104">**Lämpliga roller**</span><span class="sxs-lookup"><span data-stu-id="9fa2b-104">**Appropriate roles**</span></span>

- <span data-ttu-id="9fa2b-105">Global administratör</span><span class="sxs-lookup"><span data-stu-id="9fa2b-105">Global admin</span></span>
- <span data-ttu-id="9fa2b-106">Administratörs agent</span><span class="sxs-lookup"><span data-stu-id="9fa2b-106">Admin agent</span></span>

<span data-ttu-id="9fa2b-107">Innan du kan skapa ett konto på Partner Center måste företaget vara medlem i Microsoft Partner Network.</span><span class="sxs-lookup"><span data-stu-id="9fa2b-107">Before you can create an account on Partner Center, your company must be a member of the Microsoft Partner Network.</span></span> <span data-ttu-id="9fa2b-108">Om du inte redan är medlem i nätverket kan du [ansluta nu](https://partner.microsoft.com/commercial#).</span><span class="sxs-lookup"><span data-stu-id="9fa2b-108">If you're not already a member of the network, you can [join now](https://partner.microsoft.com/commercial#).</span></span> <span data-ttu-id="9fa2b-109">När du har skapat ett partner Center-konto kan du titta på den här korta videon [identifiera din instrument panel](https://vimeo.com/290338211).</span><span class="sxs-lookup"><span data-stu-id="9fa2b-109">After you create a Partner Center account, watch this short video [Discover your dashboard](https://vimeo.com/290338211).</span></span>

## <a name="get-a-work-email-address-before-setting-up-a-partner-center-account"></a><span data-ttu-id="9fa2b-110">Få en e-postadress till arbetet innan du konfigurerar ett partner Center-konto</span><span class="sxs-lookup"><span data-stu-id="9fa2b-110">Get a work email address before setting up a Partner Center account</span></span>

<span data-ttu-id="9fa2b-111">Företaget behöver köpa en e-postdomän för att kunna skapa e-postadresser för arbetet för dina anställda.</span><span class="sxs-lookup"><span data-stu-id="9fa2b-111">Your company needs to purchase an email domain in order for you to be able to set up work email addresses for your employees.</span></span> <span data-ttu-id="9fa2b-112">Arbeta med IT-avdelningen för att köpa en e-postdomän eftersom det är en teknisk process.</span><span class="sxs-lookup"><span data-stu-id="9fa2b-112">Work with your IT department to buy an email domain since this is a technical process.</span></span> <span data-ttu-id="9fa2b-113">Använd det nya e-postmeddelandet för att konfigurera din Azure AD-klient och ditt partner Center-konto.</span><span class="sxs-lookup"><span data-stu-id="9fa2b-113">Use the new email to set up your Azure AD tenant and your Partner Center account.</span></span>

## <a name="get-started"></a><span data-ttu-id="9fa2b-114">Kom igång</span><span class="sxs-lookup"><span data-stu-id="9fa2b-114">Get started</span></span>

<span data-ttu-id="9fa2b-115">Om du vill skapa ett konto i Partner Center måste du ha till gång till följande information.</span><span class="sxs-lookup"><span data-stu-id="9fa2b-115">To create an account on Partner Center, you'll need to have on hand the following information.</span></span> <span data-ttu-id="9fa2b-116">Det kan vara bra att ta några minuter att samla in dessa objekt innan du börjar:</span><span class="sxs-lookup"><span data-stu-id="9fa2b-116">You may want to take a few minutes to gather these items before you get started:</span></span>

- <span data-ttu-id="9fa2b-117">Global administratörs e-postadress för arbete.</span><span class="sxs-lookup"><span data-stu-id="9fa2b-117">Global administrator work email.</span></span>

- <span data-ttu-id="9fa2b-118">Om du inte är säker på vad ditt företags arbets konto är, kan du skapa ett när ditt företag inte har ett arbets konto, [men](azure-active-directory-tenants-and-partner-center.md) du kan skapa ett när du skapar kontot.</span><span class="sxs-lookup"><span data-stu-id="9fa2b-118">If you're not sure what your company's work account is, see [Your company work account and Partner Center](azure-active-directory-tenants-and-partner-center.md) If your company doesn't have a work account, you can create one during the account creation process.</span></span> 

- <span data-ttu-id="9fa2b-119">Företagets juridiska företags namn och adress.</span><span class="sxs-lookup"><span data-stu-id="9fa2b-119">Your company's legal business name and address.</span></span>  

- <span data-ttu-id="9fa2b-120">Myndighet för att signera juridiska avtal.</span><span class="sxs-lookup"><span data-stu-id="9fa2b-120">Authority to sign legal agreements.</span></span> <span data-ttu-id="9fa2b-121">Se till att du har behörighet att signera juridiska avtal på ditt företag när du blir ombedd att göra det under registrerings processen.</span><span class="sxs-lookup"><span data-stu-id="9fa2b-121">Ensure that you are authorized to sign legal agreements on your company's behalf as you'll be asked to do so during the enrollment process.</span></span>

- <span data-ttu-id="9fa2b-122">Namn och företagets e-postadress för den person som du vill ska fungera som din primära kontakt.</span><span class="sxs-lookup"><span data-stu-id="9fa2b-122">Name and company email of the person you want to act as your primary contact.</span></span> <span data-ttu-id="9fa2b-123">För att säkerställa ditt företags säkerhet och sekretess skickar vi din primära kontakt för att verifiera att (1) han eller hon registrerat sig för ett partner Center-konto och att (2) den här e-postadressen tillhör ditt företag.</span><span class="sxs-lookup"><span data-stu-id="9fa2b-123">To help ensure your company's security and privacy, we'll email your primary contact to verify that (1) he or she signed up for a Partner Center account, and that (2) this email address belongs to your company.</span></span> <span data-ttu-id="9fa2b-124">När den primära kontakten har verifierat sin e-postadress kommer vi att fortsätta med vår granskning av den information som du har angett.</span><span class="sxs-lookup"><span data-stu-id="9fa2b-124">After the primary contact verifies his or her email address, we'll continue our review of the information you provided.</span></span>

<span data-ttu-id="9fa2b-125">Vi ska kontrol lera den här informationen när kontot skapas.</span><span class="sxs-lookup"><span data-stu-id="9fa2b-125">We'll verify this information during the account creation process.</span></span> <span data-ttu-id="9fa2b-126">Information om verifierings processen finns i [konto verifiering](verification-responses.md)</span><span class="sxs-lookup"><span data-stu-id="9fa2b-126">For information on the verification process, see [Account verification](verification-responses.md)</span></span>
 
## <a name="create-a-partner-center-account"></a><span data-ttu-id="9fa2b-127">Skapa ett Partnercenter-konto</span><span class="sxs-lookup"><span data-stu-id="9fa2b-127">Create a Partner Center account</span></span>

1.  <span data-ttu-id="9fa2b-128">Granska informationen på **välkomst** sidan och välj sedan **Nästa**.</span><span class="sxs-lookup"><span data-stu-id="9fa2b-128">Review the information on the **Welcome** page and then select **Next**.</span></span>

2.  <span data-ttu-id="9fa2b-129">Logga in som global administratör till ditt företags arbets konto.</span><span class="sxs-lookup"><span data-stu-id="9fa2b-129">Sign in as a global admin to your company's work account.</span></span> <span data-ttu-id="9fa2b-130">Om du inte är säker på vad ditt företags arbets konto är, kan du gå [till ditt företags arbets konto och partner Center](azure-active-directory-tenants-and-partner-center.md).</span><span class="sxs-lookup"><span data-stu-id="9fa2b-130">If you're not sure what your company's work account   is, see [Your company work account and Partner Center](azure-active-directory-tenants-and-partner-center.md).</span></span>

    <span data-ttu-id="9fa2b-131">Välj **Logga** in om du vet att företaget har ett e-postkonto för arbetet.</span><span class="sxs-lookup"><span data-stu-id="9fa2b-131">Select **Sign in** if you know your company has a work email account.</span></span> <span data-ttu-id="9fa2b-132">På nästa sida anger du autentiseringsuppgifter för global administratör för ditt företags arbets konto.</span><span class="sxs-lookup"><span data-stu-id="9fa2b-132">On the next page, enter global admin credentials for your company's work account.</span></span> 

    <span data-ttu-id="9fa2b-133">Om ditt företag inte har ett arbets konto väljer du **skapa ett** för att ställa in det nu.</span><span class="sxs-lookup"><span data-stu-id="9fa2b-133">If your company doesn't have a work account, select **Create one** to set one up now.</span></span> <span data-ttu-id="9fa2b-134">När du har skapat ett arbets konto loggar du in med dina autentiseringsuppgifter för din globala administratör för det arbets konto som du nyss skapade.</span><span class="sxs-lookup"><span data-stu-id="9fa2b-134">After creating a work account, sign in using your global admin credentials for the work account you just created.</span></span>

3.  <span data-ttu-id="9fa2b-135">Ange eller uppdatera företagets juridiska företags profil och primär kontakt information och välj sedan **Registrera nu**.</span><span class="sxs-lookup"><span data-stu-id="9fa2b-135">Provide or update your company's legal business profile and primary contact information and then select **Enroll now**.</span></span> 

    <span data-ttu-id="9fa2b-136">Den primära kontakten bör vara den person i företaget som vi kan kontakta om ditt program (det kan vara du eller någon annan person i företaget).</span><span class="sxs-lookup"><span data-stu-id="9fa2b-136">The primary contact should be the person in your company we can contact about your application (this can be you or another person in your company).</span></span> <span data-ttu-id="9fa2b-137">Vi använder också den här informationen för att kontrol lera att personen fungerar på företaget och har registrerat sig för ett partner Center-konto.</span><span class="sxs-lookup"><span data-stu-id="9fa2b-137">We'll also use this information to verify that this person works at your company and has signed up for a Partner Center account.</span></span>

    > [!IMPORTANT]  
    > <span data-ttu-id="9fa2b-138">För att säkerställa ditt företags säkerhet och sekretess skickar vi din primära kontakt för att verifiera att (1) han eller hon registrerat sig för ett partner Center-konto och (2) att den här e-postadressen tillhör ditt företag.</span><span class="sxs-lookup"><span data-stu-id="9fa2b-138">To help ensure your company's security and privacy, we'll email your primary contact to verify that (1) he or she signed up for a Partner Center account, and (2) that this email address belongs to your company.</span></span> <span data-ttu-id="9fa2b-139">När den primära kontakten har verifierat sin e-postadress kommer vi att fortsätta med vår granskning av den information som du har angett.</span><span class="sxs-lookup"><span data-stu-id="9fa2b-139">After the primary contact verifies his or her email address, we'll continue our review of the information you provided.</span></span>

4.  <span data-ttu-id="9fa2b-140">Läs och godkänn de allmänna villkoren i Microsoft Partner Network avtalet.</span><span class="sxs-lookup"><span data-stu-id="9fa2b-140">Read and accept the terms and conditions in the Microsoft Partner Network agreement.</span></span> 

5.  <span data-ttu-id="9fa2b-141">Kontrol lera att du har lagts till i administratörs Agent gruppen.</span><span class="sxs-lookup"><span data-stu-id="9fa2b-141">Verify that you've been added to the admin agent group.</span></span> <span data-ttu-id="9fa2b-142">För att slutföra konfigurationen av ditt konto, inklusive att lägga till andra användare, måste du ha administratörs agent behörighet.</span><span class="sxs-lookup"><span data-stu-id="9fa2b-142">To finish setting up your account, including adding other users, you must have admin agent permissions.</span></span> <span data-ttu-id="9fa2b-143">Följ dessa steg om du vill visa eller uppdatera dina behörigheter:</span><span class="sxs-lookup"><span data-stu-id="9fa2b-143">Follow these steps to view or update your permissions:</span></span>

    <span data-ttu-id="9fa2b-144">a.</span><span class="sxs-lookup"><span data-stu-id="9fa2b-144">a.</span></span> <span data-ttu-id="9fa2b-145">Välj ikonen **Inställningar** på [instrument panelen](https://partner.microsoft.com/dashboard/home**)för partner Center och välj sedan **användar hantering**.</span><span class="sxs-lookup"><span data-stu-id="9fa2b-145">From the Partner Center [dashboard](https://partner.microsoft.com/dashboard/home**), select the **Settings** icon and then select **User management**.</span></span>  

    <span data-ttu-id="9fa2b-146">b.</span><span class="sxs-lookup"><span data-stu-id="9fa2b-146">b.</span></span> <span data-ttu-id="9fa2b-147">Välj ditt namn i listan användare och välj sedan **admin agent** om det inte redan är valt.</span><span class="sxs-lookup"><span data-stu-id="9fa2b-147">Select your name from the users list and then select **Admin agent** if it's not already selected.</span></span> <span data-ttu-id="9fa2b-148">Välj **Uppdatera**.</span><span class="sxs-lookup"><span data-stu-id="9fa2b-148">Select **Update**.</span></span>  

## <a name="view-mpn-account-details"></a><span data-ttu-id="9fa2b-149">Visa information om MPN-kontot</span><span class="sxs-lookup"><span data-stu-id="9fa2b-149">View MPN account details</span></span>

<span data-ttu-id="9fa2b-150">När du har skapat ett partner Center-konto kan du gå tillbaka till Partner Center och se olika konto uppgifter.</span><span class="sxs-lookup"><span data-stu-id="9fa2b-150">Once you create a Partner Center account, you can return to Partner Center to see various account details.</span></span> <span data-ttu-id="9fa2b-151">Många av dessa visas på sidan **partner profil** på [instrument panelen](https://partner.microsoft.com/dashboard)för partner Center.</span><span class="sxs-lookup"><span data-stu-id="9fa2b-151">Many of these appear on the **Partner profile** page in your Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

<span data-ttu-id="9fa2b-152">Sådan information omfattar:</span><span class="sxs-lookup"><span data-stu-id="9fa2b-152">Such details include:</span></span>

- <span data-ttu-id="9fa2b-153">Företagets juridiska företags profil</span><span class="sxs-lookup"><span data-stu-id="9fa2b-153">Your company's legal business profile</span></span>

- <span data-ttu-id="9fa2b-154">Information om ditt MPN-ID</span><span class="sxs-lookup"><span data-stu-id="9fa2b-154">Information about your MPN ID</span></span>

- <span data-ttu-id="9fa2b-155">Länkar till aktuella avtal som är kopplade till ditt registrerade Microsoft-program</span><span class="sxs-lookup"><span data-stu-id="9fa2b-155">Links to current agreements associated with your enrolled Microsoft program</span></span>

  <span data-ttu-id="9fa2b-156">Om du till exempel är registrerad i MPN-programmet visas en länk till det aktuella Microsoft Partner Network avtalet.</span><span class="sxs-lookup"><span data-stu-id="9fa2b-156">For example, if you are enrolled in the MPN program, you'll see a link to the current Microsoft Partner Network agreement.</span></span> <span data-ttu-id="9fa2b-157">Om du är registrerad i andra partner program, t. ex. Cloud Solution Provider (CSP), kan du också se länkar till andra avtal, t. ex. Microsoft partner avtal.</span><span class="sxs-lookup"><span data-stu-id="9fa2b-157">If you're enrolled in other partner programs, like the Cloud Solution Provider (CSP) program, you may also see links to other agreements, such as the Microsoft Partner Agreement.</span></span> 

  > [!NOTE]
  > <span data-ttu-id="9fa2b-158">Det kan vara praktiskt att se dessa typer av länkar om du vill gå igenom, komma åt eller ladda ned ett avtal eller kontrol lera datumet då det signerades.</span><span class="sxs-lookup"><span data-stu-id="9fa2b-158">Seeing these types of links may be useful if you ever want to review, access, or download an agreement, or, check the date it was signed.</span></span>

### <a name="how-to-view-account-details-or-view-and-download-the-mpn-agreement"></a><span data-ttu-id="9fa2b-159">Visa konto information eller Visa och ladda ned MPN-avtalet</span><span class="sxs-lookup"><span data-stu-id="9fa2b-159">How to view account details or view and download the MPN agreement</span></span>

<span data-ttu-id="9fa2b-160">Följ dessa steg om du vill visa konto information eller Visa och ladda ned MPN-avtalet:</span><span class="sxs-lookup"><span data-stu-id="9fa2b-160">Follow these steps to view account details or view and download the MPN agreement:</span></span>

1. <span data-ttu-id="9fa2b-161">Använd ditt arbets konto användar namn och lösen ord för att logga in på Partner Center- [instrumentpanelen](https://partner.microsoft.com/dashboard).</span><span class="sxs-lookup"><span data-stu-id="9fa2b-161">Using your work account username and password, sign in to the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="9fa2b-162">En översikts sida visas.</span><span class="sxs-lookup"><span data-stu-id="9fa2b-162">An Overview page appears.</span></span> <span data-ttu-id="9fa2b-163">(Om du inte ser sidan Översikt väljer du **Översikt** på menyn till vänster-navigerings.)</span><span class="sxs-lookup"><span data-stu-id="9fa2b-163">(If you do not see the Overview page, select **Overview** from the left-navigation menu.)</span></span>

3. <span data-ttu-id="9fa2b-164">Välj kugg hjuls ikonen i det övre högra hörnet på instrument panelen och välj sedan **partner inställningar**.</span><span class="sxs-lookup"><span data-stu-id="9fa2b-164">Select the Gear icon in the top-right corner of the dashboard, then select **Partner settings**.</span></span> <span data-ttu-id="9fa2b-165">Då går du till sidan partner profil.</span><span class="sxs-lookup"><span data-stu-id="9fa2b-165">This takes you to the Partner profile page.</span></span>

4. <span data-ttu-id="9fa2b-166">På sidan partner profil kan du se olika områden.</span><span class="sxs-lookup"><span data-stu-id="9fa2b-166">From the Partner profile page, you'll see different areas.</span></span> <span data-ttu-id="9fa2b-167">Dessa inkluderar ett område för **juridiska företags profiler** och ett informations område för **program** .</span><span class="sxs-lookup"><span data-stu-id="9fa2b-167">These include a **Legal business profile** area and a **Program info** area.</span></span>

5. <span data-ttu-id="9fa2b-168">Leta upp fältet **MPN program status** under **program information**.</span><span class="sxs-lookup"><span data-stu-id="9fa2b-168">Under **Program info**, locate the **MPN program status** field.</span></span> <span data-ttu-id="9fa2b-169">Då visas en länk till ditt Microsoft Partner Networks avtal.</span><span class="sxs-lookup"><span data-stu-id="9fa2b-169">This displays a link to your Microsoft Partner Network agreement.</span></span> <span data-ttu-id="9fa2b-170">Den beskriver också din aktuella status i programmet.</span><span class="sxs-lookup"><span data-stu-id="9fa2b-170">It also describes your current status in the program.</span></span>


   :::image type="content" source="images/accountsettings/mpn-program-info-download-mpn-agreement.png" alt-text="Bild som visar området program information på sidan partner profil med en röd ruta som markerar fältet MPN program status i det här området tillsammans med dess associerade länk till Microsoft Partner Network avtalet.":::

6. <span data-ttu-id="9fa2b-172">Om du vill visa eller hämta det här avtalet väljer du **Microsoft Partner Network avtal**.</span><span class="sxs-lookup"><span data-stu-id="9fa2b-172">To view or download this agreement, select **Microsoft Partner Network agreement**.</span></span>  

> [!NOTE]
> <span data-ttu-id="9fa2b-173">Du kan också använda stegen ovan för att visa eller ladda ned andra avtal för andra, registrerade program, till exempel Microsoft partner Agreement om du råkar registrera dig i CSP-programmet (Cloud Solution Provider).</span><span class="sxs-lookup"><span data-stu-id="9fa2b-173">You can also use the above steps to view or download other agreements for other, enrolled programs, such as the Microsoft Partner Agreement if you happen to be enrolled in the Cloud Solution Provider (CSP) program.</span></span>

## <a name="next-steps"></a><span data-ttu-id="9fa2b-174">Nästa steg</span><span class="sxs-lookup"><span data-stu-id="9fa2b-174">Next steps</span></span>

-   [<span data-ttu-id="9fa2b-175">Lägg till konto användare och tilldela behörigheter till dem</span><span class="sxs-lookup"><span data-stu-id="9fa2b-175">Add account users and assign permissions to them</span></span>](create-user-accounts-and-set-permissions.md)

-   [<span data-ttu-id="9fa2b-176">Köpa eller förnya en prenumeration på Microsoft Action Pack</span><span class="sxs-lookup"><span data-stu-id="9fa2b-176">Purchase or renew a subscription to Microsoft Action Pack</span></span>](mpn-get-action-pack.md)

-   [<span data-ttu-id="9fa2b-177">Hantera dina medlemskaps förmåner</span><span class="sxs-lookup"><span data-stu-id="9fa2b-177">Manage your membership benefits</span></span>](manage-your-partner-network-benefits.md)

-   [<span data-ttu-id="9fa2b-178">Lär dig mer om kompetens krav för guld-och silver-medlemskap</span><span class="sxs-lookup"><span data-stu-id="9fa2b-178">Learn about competency requirements for Gold and Silver membership</span></span>](https://partner.microsoft.com/membership/competencies)

-   [<span data-ttu-id="9fa2b-179">Skapa en företagsprofil för att få kundämnen från Microsoft</span><span class="sxs-lookup"><span data-stu-id="9fa2b-179">Create a business profile to get sales leads from Microsoft</span></span>](create-a-marketing-profile.md)

-   [<span data-ttu-id="9fa2b-180">Hämta och hantera Sälj leads från Microsoft</span><span class="sxs-lookup"><span data-stu-id="9fa2b-180">Get and manage sales leads from Microsoft</span></span>](manage-leads.md)
