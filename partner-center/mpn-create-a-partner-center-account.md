---
title: Skapa ett MPN-konto i Partnercenter
ms.topic: article
ms.date: 04/08/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Lär dig hur Microsoft Partner Network kan skapa ett Partnercenter-konto för att hantera sina nätverksförmåner och kompetenser.
author: ParthP
ms.author: ParthP
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 27cd00b5475914019963fad381b36b47a017dcf1
ms.sourcegitcommit: 078eac1456f68585ff1003b21e5e1fe777af314b
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/28/2021
ms.locfileid: "108120808"
---
# <a name="create-an-mpn-account-in-partner-center-to-manage-network-benefits-and-competencies"></a><span data-ttu-id="47a56-103">Skapa ett MPN-konto i Partnercenter för att hantera nätverksförmåner och kompetenser</span><span class="sxs-lookup"><span data-stu-id="47a56-103">Create an MPN account in Partner Center to manage network benefits and competencies</span></span>

<span data-ttu-id="47a56-104">**Lämpliga roller**</span><span class="sxs-lookup"><span data-stu-id="47a56-104">**Appropriate roles**</span></span>

- <span data-ttu-id="47a56-105">MPN-partneradministratör</span><span class="sxs-lookup"><span data-stu-id="47a56-105">MPN partner admin</span></span>

<span data-ttu-id="47a56-106">Om du inte har Microsoft Partner Network (MPN) och inte har något MPN-ID kan du starta registreringen genom att följa [registreringsanvisningarna](https://partner.microsoft.com/dashboard/account/v3/enrollment/introduction/partnership).</span><span class="sxs-lookup"><span data-stu-id="47a56-106">If you are new to Microsoft Partner Network (MPN) and don’t have an MPN ID, you can start your enrollment by following the [enrollment instructions](https://partner.microsoft.com/dashboard/account/v3/enrollment/introduction/partnership).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="47a56-107">Förutsättningar</span><span class="sxs-lookup"><span data-stu-id="47a56-107">Prerequisites</span></span> 

<span data-ttu-id="47a56-108">När du är redo att skapa ett konto i Partnercenter måste du ha följande till hands.</span><span class="sxs-lookup"><span data-stu-id="47a56-108">When you are ready to create an account on Partner Center, you will need to have the following items on hand.</span></span>  <span data-ttu-id="47a56-109">Det kan ta några minuter att samla in de här objekten innan du börjar:</span><span class="sxs-lookup"><span data-stu-id="47a56-109">You may want to take a few minutes to gather these items before you get started:</span></span>

- <span data-ttu-id="47a56-110">Företags e-post eller Office 365-arbetskonto.</span><span class="sxs-lookup"><span data-stu-id="47a56-110">Company work email OR Office 365 work account.</span></span> <span data-ttu-id="47a56-111">Ditt företag kan behöva köpa en e-postdomän för att du ska kunna konfigurera e-postadresser för arbete för dina anställda.</span><span class="sxs-lookup"><span data-stu-id="47a56-111">Your company may need to purchase an email domain in order for you to set up work email addresses for your employees.</span></span> <span data-ttu-id="47a56-112">Mer information finns i [Ditt företags arbetskonto och Partnercenter.](azure-active-directory-tenants-and-partner-center.md)</span><span class="sxs-lookup"><span data-stu-id="47a56-112">For more information, read [Your company work account and Partner Center](azure-active-directory-tenants-and-partner-center.md).</span></span> 
 
- <span data-ttu-id="47a56-113">Företagets juridiska namn och adress.</span><span class="sxs-lookup"><span data-stu-id="47a56-113">Your company's legal business name and address.</span></span>

- <span data-ttu-id="47a56-114">Behörighet att signera juridiska avtal.</span><span class="sxs-lookup"><span data-stu-id="47a56-114">Authority to sign legal agreements.</span></span> <span data-ttu-id="47a56-115">Se till att du har behörighet att signera juridiska avtal för ditt företags räkning eftersom du uppmanas att göra det under registreringsprocessen.</span><span class="sxs-lookup"><span data-stu-id="47a56-115">Ensure that you are authorized to sign legal agreements on your company's behalf as you'll be asked to do so during the enrollment process.</span></span>

- <span data-ttu-id="47a56-116">Namn och företagets e-postadress till den person som du vill fungera som primär kontakt.</span><span class="sxs-lookup"><span data-stu-id="47a56-116">Name and company email of the person you want to act as your primary contact.</span></span> <span data-ttu-id="47a56-117">För att säkerställa företagets säkerhet och sekretess skickar vi e-post till din primära kontakt för att verifiera e-postadressen och för att säkerställa att e-postadressen tillhör ditt företag.</span><span class="sxs-lookup"><span data-stu-id="47a56-117">To help ensure your company's security and privacy, we email your primary contact to verify the email address and to ensure that the email address belongs to your company.</span></span> <span data-ttu-id="47a56-118">När den primära kontakten har verifierat e-postadressen fortsätter vi att granska informationen som angetts.</span><span class="sxs-lookup"><span data-stu-id="47a56-118">After the primary contact verifies the email address, we'll continue our review of the information provided.</span></span> <span data-ttu-id="47a56-119">Verifieringen tar vanligtvis 3–5 arbetsdagar.</span><span class="sxs-lookup"><span data-stu-id="47a56-119">Verification usually takes 3-5 business days.</span></span> 

- <span data-ttu-id="47a56-120">Information om verifieringsprocessen finns i [Kontoverifiering.](verification-responses.md)</span><span class="sxs-lookup"><span data-stu-id="47a56-120">For information on the verification process, see [Account verification](verification-responses.md).</span></span>

>[!NOTE]
><span data-ttu-id="47a56-121">Om ditt Microsoft Partner Network är kvar i Partner Membership Center (PMC) måste du migrera ditt konto direkt till Partnercenter.</span><span class="sxs-lookup"><span data-stu-id="47a56-121">If your Microsoft Partner Network membership is still in Partner Membership Center (PMC), you need to migrate your account immediately to Partner Center.</span></span> <span data-ttu-id="47a56-122">Ladda ned [den stegvisa guiden för att migrera](https://assetsprod.microsoft.com/mpn/migrate-pmc-pc-mpa-guide.pptx).</span><span class="sxs-lookup"><span data-stu-id="47a56-122">Download the [step-by-step guide to migrate](https://assetsprod.microsoft.com/mpn/migrate-pmc-pc-mpa-guide.pptx).</span></span>

## <a name="get-started"></a><span data-ttu-id="47a56-123">Kom igång</span><span class="sxs-lookup"><span data-stu-id="47a56-123">Get started</span></span>

1. <span data-ttu-id="47a56-124">På sidan [**Kom igång**](https://partner.microsoft.com/dashboard/account/v3/enrollment/introduction/partnership) börjar du med din e-postadress till arbetet från ditt företag, till exempel you@yourcompanyname.com .</span><span class="sxs-lookup"><span data-stu-id="47a56-124">At the [**Get started**](https://partner.microsoft.com/dashboard/account/v3/enrollment/introduction/partnership) page, start with your work email given to you by your company, for example, you@yourcompanyname.com.</span></span>

 
    <span data-ttu-id="47a56-125">a.</span><span class="sxs-lookup"><span data-stu-id="47a56-125">a.</span></span>  <span data-ttu-id="47a56-126">E-postadressen måste vara giltig och tillgänglig för dig eftersom vi skickar en verifieringskod till det e-postmeddelandet för att fortsätta.</span><span class="sxs-lookup"><span data-stu-id="47a56-126">The email address must be valid and accessible to you because we will send a verification code to that email to continue.</span></span>

    <span data-ttu-id="47a56-127">b.</span><span class="sxs-lookup"><span data-stu-id="47a56-127">b.</span></span>  <span data-ttu-id="47a56-128">E-postadressen får inte innehålla ord som "info", "admin", email@ "."</span><span class="sxs-lookup"><span data-stu-id="47a56-128">The email address should not contain words like "info," "admin," "email@."</span></span> <span data-ttu-id="47a56-129">Eller " marketing@.. ."; dessa adressformat stöds inte.</span><span class="sxs-lookup"><span data-stu-id="47a56-129">Or "marketing@..."; these address formats are not supported.</span></span>

    <span data-ttu-id="47a56-130">c.</span><span class="sxs-lookup"><span data-stu-id="47a56-130">c.</span></span>  <span data-ttu-id="47a56-131">Om du vill köpa MAPS eller hantera kompetenser måste du uppgradera det här kontot [genom att verifiera din domän](become-global-admin.md) och bli administratör.</span><span class="sxs-lookup"><span data-stu-id="47a56-131">To purchase MAPS or manage competencies, you will have to upgrade this account by [verifying your domain](become-global-admin.md) and becoming an admin.</span></span> 

2. <span data-ttu-id="47a56-132">Du kan logga in med ditt Office 365-arbetskonto, till exempel you@contoso.onmicrosoft.com .</span><span class="sxs-lookup"><span data-stu-id="47a56-132">You can sign in with your Office 365 work account, for example, you@contoso.onmicrosoft.com.</span></span>

   >[!NOTE]
   > <span data-ttu-id="47a56-133">Du kan inte använda dina befintliga CSP-kontoautentiseringsuppgifter för att registrera dig för MPN.</span><span class="sxs-lookup"><span data-stu-id="47a56-133">You can’t use your existing CSP account credentials to enroll into MPN.</span></span>

3. <span data-ttu-id="47a56-134">Ange företagets juridiska information.</span><span class="sxs-lookup"><span data-stu-id="47a56-134">Provide your company's legal business details.</span></span>

<span data-ttu-id="47a56-135">Du kan antingen leta upp din företagsprofil eller ange företagsinformation manuellt.</span><span class="sxs-lookup"><span data-stu-id="47a56-135">You can either look up your company profile or enter company information manually.</span></span> <span data-ttu-id="47a56-136">Om ditt företag är registrerat med [Dun & Bradstreet](https://partner.microsoft.com/marketing/usisvshowcase/dunandbrad)använder du DUNS-ID:t för att leta upp din företagsinformation.</span><span class="sxs-lookup"><span data-stu-id="47a56-136">If your company is registered with [Dun & Bradstreet](https://partner.microsoft.com/marketing/usisvshowcase/dunandbrad), use the DUNS ID to look up your company info.</span></span> <span data-ttu-id="47a56-137">Om du vill ange företagsinformation själv väljer du **Manuell.**</span><span class="sxs-lookup"><span data-stu-id="47a56-137">If you want to provide your company details yourself, select **Manual**.</span></span>

<span data-ttu-id="47a56-138">Om ditt företag finns i  **Det** begynnande, begynnande, **kyrgyzstan,** Underegien,  **Anten** eller Ryssland, och du anger din adress manuellt, kommer vi att verifiera din adress åt dig. </span><span class="sxs-lookup"><span data-stu-id="47a56-138">If your company is located in **Armenia**, **Hungary**, **Kyrgyzstan**, **Moldova**, **Uzbekistan**, or **Russia**, and you enter your address manually, we will validate your address for you.</span></span> <span data-ttu-id="47a56-139">Om den som du anger skiljer sig från den verifierade, föreslår vi att du använder den verifierade adressen.</span><span class="sxs-lookup"><span data-stu-id="47a56-139">If the one you enter differs from the validated one, we suggest you use the validated address.</span></span> <span data-ttu-id="47a56-140">Detta säkerställer att adresselementen standardiseras enligt definitionen av landet postnummer, korrekt formaterade och kan levereras.</span><span class="sxs-lookup"><span data-stu-id="47a56-140">This ensures that the elements of the address are standardized as defined by the country's postal authority, correctly formatted, and shippable.</span></span>  

<span data-ttu-id="47a56-141">När du har angett företagsinformation anger du den primära kontaktinformationen.</span><span class="sxs-lookup"><span data-stu-id="47a56-141">Once you have provided the company info, enter the primary contact information.</span></span> <span data-ttu-id="47a56-142">Den primära kontakten ska vara den person i företaget som vi kan kontakta om ditt program (den här kontakten kan vara du eller en annan person i ditt företag).</span><span class="sxs-lookup"><span data-stu-id="47a56-142">The primary contact should be the person in your company we can contact about your application (this contact can be you or another person in your company).</span></span>

4. <span data-ttu-id="47a56-143">Välj **Registrera nu.**</span><span class="sxs-lookup"><span data-stu-id="47a56-143">Select **Enroll now**.</span></span>

>[!IMPORTANT]
><span data-ttu-id="47a56-144">För att säkerställa företagets säkerhet och sekretess skickar vi e-post till din primära kontakt för att verifiera e-postadressen och se till att e-postadressen tillhör ditt företag.</span><span class="sxs-lookup"><span data-stu-id="47a56-144">To help ensure your company's security and privacy, we email your primary contact to verify the email address and ensure that the email address belongs to your company.</span></span> <span data-ttu-id="47a56-145">När den primära kontakten har verifierat e-postadressen fortsätter vi att granska informationen som du har angett.</span><span class="sxs-lookup"><span data-stu-id="47a56-145">After the primary contact verifies the email address, we'll continue our review of the information you provided.</span></span> <span data-ttu-id="47a56-146">Verifieringen tar vanligtvis 3–5 arbetsdagar.</span><span class="sxs-lookup"><span data-stu-id="47a56-146">Verification usually takes 3-5 business days.</span></span> 

## <a name="how-to-view-account-details-or-view-and-download-the-mpn-agreement"></a><span data-ttu-id="47a56-147">Visa kontoinformation eller visa och ladda ned MPN-avtalet</span><span class="sxs-lookup"><span data-stu-id="47a56-147">How to view account details or view and download the MPN agreement</span></span>

<span data-ttu-id="47a56-148">Logga in på Partner Center med dina MPN-autentiseringsuppgifter.</span><span class="sxs-lookup"><span data-stu-id="47a56-148">Sign into Partner Center with your MPN credentials.</span></span> <span data-ttu-id="47a56-149">Välj [**Partnerprofil**](https://partner.microsoft.com/pcv/accountsettings/connectedpartnerprofile) för att visa företagets juridiska information, din verifieringsstatus, DINA MPN-ID:er och skapa även nya MPN-platser om det behövs.</span><span class="sxs-lookup"><span data-stu-id="47a56-149">Select [**Partner profile**](https://partner.microsoft.com/pcv/accountsettings/connectedpartnerprofile) to view your company’s legal details, your verification status, your MPN IDs and also create new MPN locations if needed.</span></span> 

<span data-ttu-id="47a56-150">Du kan också visa annan viktig information som MPN-ID:n, hantera MPN-platser och visa Microsoft-partneravtal med hjälp av de vänstra menylänkarna som visas i följande skärmbild.</span><span class="sxs-lookup"><span data-stu-id="47a56-150">You can also view other important information like MPN Ids, manage MPN locations, and view Microsoft Partner Agreement using the left menu links as show in the following screenshot.</span></span>

:::image type="content" source="images/mpn-new.png" alt-text="Partnerprofil":::


## <a name="next-steps"></a><span data-ttu-id="47a56-152">Nästa steg</span><span class="sxs-lookup"><span data-stu-id="47a56-152">Next steps</span></span>

-  [<span data-ttu-id="47a56-153">Lägga till kontoanvändare och tilldela behörigheter till dem</span><span class="sxs-lookup"><span data-stu-id="47a56-153">Add account users and assign permissions to them</span></span>](create-user-accounts-and-set-permissions.md)

-  [<span data-ttu-id="47a56-154">Köpa eller förnya en prenumeration på Microsoft Action Pack</span><span class="sxs-lookup"><span data-stu-id="47a56-154">Purchase or renew a subscription to Microsoft Action Pack</span></span>](mpn-get-action-pack.md)

-  [<span data-ttu-id="47a56-155">Hantera dina medlemskapsförmåner</span><span class="sxs-lookup"><span data-stu-id="47a56-155">Manage your membership benefits</span></span>](manage-your-partner-network-benefits.md)

-  [<span data-ttu-id="47a56-156">Lär dig mer om kompetenskrav för guld- och silvermedlemskap</span><span class="sxs-lookup"><span data-stu-id="47a56-156">Learn about competency requirements for Gold and Silver membership</span></span>](https://partner.microsoft.com/membership/competencies)

-  [<span data-ttu-id="47a56-157">Skapa en företagsprofil för att få kundämnen från Microsoft</span><span class="sxs-lookup"><span data-stu-id="47a56-157">Create a business profile to get sales leads from Microsoft</span></span>](create-a-marketing-profile.md)

-  [<span data-ttu-id="47a56-158">Hämta och hantera sälj leads från Microsoft</span><span class="sxs-lookup"><span data-stu-id="47a56-158">Get and manage sales leads from Microsoft</span></span>](manage-leads.md)
