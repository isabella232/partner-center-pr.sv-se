---
title: Utbetalnings- och skatteprofiler i Partnercenter
ms.topic: how-to
ms.date: 11/12/2020
description: Skapa och hantera din utbetalnings-och skatte profil så att du kan betala för dina stimulans arbeten. Inkluderar att skapa, hantera och använda olika profiler.
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
author: Karthic83
ms.author: kashanum
ms.localizationpriority: medium
ms.openlocfilehash: 282fdacc8689ff71e885a2f0ea01ce9570611707
ms.sourcegitcommit: d37a3f353426e52dfbbac577b7576f9c3f6d2ddf
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 02/06/2021
ms.locfileid: "99624246"
---
# <a name="create-and-manage-incentives-payout-and-tax-profiles-in-partner-center"></a><span data-ttu-id="c9e9c-104">Skapa och hantera incitaments utbetalningar och skatte profiler i Partner Center</span><span class="sxs-lookup"><span data-stu-id="c9e9c-104">Create and manage incentives payout and tax profiles in Partner Center</span></span>


<span data-ttu-id="c9e9c-105">**Lämpliga roller:**</span><span class="sxs-lookup"><span data-stu-id="c9e9c-105">**Appropriate roles:**</span></span>

- <span data-ttu-id="c9e9c-106">Incitaments administratör</span><span class="sxs-lookup"><span data-stu-id="c9e9c-106">Incentives admin</span></span>
- <span data-ttu-id="c9e9c-107">Kontoadministratör</span><span class="sxs-lookup"><span data-stu-id="c9e9c-107">Account admin</span></span>
- <span data-ttu-id="c9e9c-108">Global administratör</span><span class="sxs-lookup"><span data-stu-id="c9e9c-108">Global admin</span></span>

<span data-ttu-id="c9e9c-109">Innan du kan erhålla betalningar för dina incitamentprogram för en viss MPN-plats måste du slutföra registreringen genom att associera en giltig utbetalnings- och skatteprofil med programmet och MPN-platsen.</span><span class="sxs-lookup"><span data-stu-id="c9e9c-109">Before you can receive payment for your incentive programs for a particular MPN location, you must complete your enrollment by associating a valid payout and tax profile with the program and MPN location.</span></span> <span data-ttu-id="c9e9c-110">Microsoft använder den här utbetalnings- och skatteprofilen för att utfärda betalningar.</span><span class="sxs-lookup"><span data-stu-id="c9e9c-110">Microsoft will use this payout and tax profile to issue payments.</span></span> <span data-ttu-id="c9e9c-111">Eventuellt kan du välja att använda elektronisk banköverföring eller en kreditfaktura för betalningar, beroende på reglerna för incitamentprogrammet.</span><span class="sxs-lookup"><span data-stu-id="c9e9c-111">You may be allowed to use electronic bank transfer or a credit note for payment, depending on the rules of the incentive program.</span></span> 

## <a name="roles-currencies-and-other-microsoft-programs"></a><span data-ttu-id="c9e9c-112">Roller, valutor och andra Microsoft-program</span><span class="sxs-lookup"><span data-stu-id="c9e9c-112">Roles, currencies, and other Microsoft programs</span></span>

<span data-ttu-id="c9e9c-113">Det är viktigt att förstå informationen nedan innan du börjar med din utbetalnings-och skatte profil.</span><span class="sxs-lookup"><span data-stu-id="c9e9c-113">It's important to understand the information below before you get started with your payout and tax profile.</span></span>

### <a name="roles-and-permissions"></a><span data-ttu-id="c9e9c-114">Roller och behörigheter</span><span class="sxs-lookup"><span data-stu-id="c9e9c-114">Roles and permissions</span></span>

<span data-ttu-id="c9e9c-115">Du måste vara en incitaments administratör för att ange bank-och skatte information för incitaments betalningar.</span><span class="sxs-lookup"><span data-stu-id="c9e9c-115">You must be an Incentives Admin to enter bank and tax information for incentive payments.</span></span> <span data-ttu-id="c9e9c-116">Om du är MPN-/konto administratör kan du tilldela dig själv och/eller en kollega som incitaments administratör.</span><span class="sxs-lookup"><span data-stu-id="c9e9c-116">If you're an MPN/Account Admin, you can assign yourself and/or a colleague to be the Incentives Admin.</span></span>

<span data-ttu-id="c9e9c-117">Kontakta MPN-administratören eller den globala administratören om du behöver begära att be om administratörs behörighet. Du kan ta reda på vem i företaget som har dessa roller genom att logga in på [partner Center-instrumentpanelen](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="c9e9c-117">If you need to request Incentives Admin permissions, contact your MPN Admin or Global Admin. You can find out who in your company has these roles by signing into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span> <span data-ttu-id="c9e9c-118">Från **inställnings** ikonen längst upp till höger väljer du **användar hantering** och filtrerar sedan på global administratör.</span><span class="sxs-lookup"><span data-stu-id="c9e9c-118">From the **Settings** icon at the top right, select **User Management** and then filter on Global Admin.</span></span>

<span data-ttu-id="c9e9c-119">Incitaments användare kan se incitaments vinster och betalnings information och rapporter, men kan inte redigera bank-och skatte information.</span><span class="sxs-lookup"><span data-stu-id="c9e9c-119">Incentives Users can view Incentive earnings and payment details and reports, but can’t edit bank and tax details.</span></span>

### <a name="choose-your-disbursement-currency"></a><span data-ttu-id="c9e9c-120">Välj din utbetalnings valuta</span><span class="sxs-lookup"><span data-stu-id="c9e9c-120">Choose your disbursement currency</span></span>

<span data-ttu-id="c9e9c-121">Incitaments betalningar görs i den valuta som du valde när du konfigurerade din betalnings profil.</span><span class="sxs-lookup"><span data-stu-id="c9e9c-121">Incentive payments are made in the currency you selected when you set up your payment profile.</span></span> <span data-ttu-id="c9e9c-122">Betalningarna beräknas med en växelkurs som ställs in månatlig av Microsoft.</span><span class="sxs-lookup"><span data-stu-id="c9e9c-122">Payments will be calculated using an exchange rate as set monthly by Microsoft.</span></span> <span data-ttu-id="c9e9c-123">Du ansvarar för alla ändringar i värdet på grund av vald valuta.</span><span class="sxs-lookup"><span data-stu-id="c9e9c-123">You’ll be responsible for any changes in value due to the currency selected.</span></span>

### <a name="using-different-profiles-for-different-microsoft-programs"></a><span data-ttu-id="c9e9c-124">Använda olika profiler för olika Microsoft-program</span><span class="sxs-lookup"><span data-stu-id="c9e9c-124">Using different profiles for different Microsoft programs</span></span>

<span data-ttu-id="c9e9c-125">Om ditt företag är registrerat i flera incitaments program kan du använda samma betalnings konto för alla, eller välja att använda olika betalnings konton för olika program.</span><span class="sxs-lookup"><span data-stu-id="c9e9c-125">If your company is enrolled in multiple incentive programs, you can use the same payment account for all of them, or choose to use different payment accounts for different programs.</span></span>

## <a name="create-and-manage-payout-and-tax-profiles-in-partner-center"></a><span data-ttu-id="c9e9c-126">Skapa och hantera utbetalnings-och skatte profiler i Partner Center</span><span class="sxs-lookup"><span data-stu-id="c9e9c-126">Create and manage payout and tax profiles in Partner Center</span></span>

<span data-ttu-id="c9e9c-127">I avsnitten nedan får du stegvisa anvisningar genom processen att skapa och hantera betalnings-och skatte profiler i Partner Center.</span><span class="sxs-lookup"><span data-stu-id="c9e9c-127">The sections below will walk you through the process of creating and managing payment and tax profiles in Partner Center.</span></span>

>[!IMPORTANT]
><span data-ttu-id="c9e9c-128">Du måste vara en incitaments administratör för att skapa eller hantera betalnings profiler i Partner Center.</span><span class="sxs-lookup"><span data-stu-id="c9e9c-128">You must be an Incentive admin to create or manage payment profiles in Partner Center.</span></span> <span data-ttu-id="c9e9c-129">Stimulans roller måste tilldelas till varje MPN-plats under varje incitaments program.</span><span class="sxs-lookup"><span data-stu-id="c9e9c-129">Incentive roles must be assigned to each MPN location under each incentive program.</span></span> <span data-ttu-id="c9e9c-130">Mer information om hur du lägger till stimulans administratörer i Partner Center finns i [skapa användar konton](create-user-accounts-and-set-permissions.md).</span><span class="sxs-lookup"><span data-stu-id="c9e9c-130">For more information on how to add Incentive admins in Partner Center, see [Create user accounts](create-user-accounts-and-set-permissions.md).</span></span>

## <a name="access-the-payout-and-tax-section-in-partner-center"></a><span data-ttu-id="c9e9c-131">Gå till avsnittet utbetalnings-och skatte avsnitt i Partner Center</span><span class="sxs-lookup"><span data-stu-id="c9e9c-131">Access the payout and tax section in Partner Center</span></span>

1. <span data-ttu-id="c9e9c-132">Logga in på [partner Center-instrumentpanelen](https://partner.microsoft.com/dashboard/) med ditt Azure Active Directory (Azure AD)-konto (företags konto) eller lämplig e-postadress om ett har tilldelats.</span><span class="sxs-lookup"><span data-stu-id="c9e9c-132">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/) using your Azure Active Directory (Azure AD) account (company account), or the appropriate email address if one was assigned.</span></span>

   - <span data-ttu-id="c9e9c-133">Flera domäner kan registreras i ett Azure AD-konto.</span><span class="sxs-lookup"><span data-stu-id="c9e9c-133">Multiple domains can be registered within one Azure AD account.</span></span> <span data-ttu-id="c9e9c-134">Kontakta din globala administratör för att avgöra vilka domäner som är associerade.</span><span class="sxs-lookup"><span data-stu-id="c9e9c-134">Contact your Global admin to determine which domains are associated.</span></span>
   - <span data-ttu-id="c9e9c-135">Om du bara kan logga in med @onmicrosoft.com domänen kontaktar du konto administratören för att lägga till ytterligare domäner i Azure AD-kontot.</span><span class="sxs-lookup"><span data-stu-id="c9e9c-135">If you're only able to log in with the @onmicrosoft.com domain, contact your Account admin to add additional domains to the Azure AD account.</span></span>
   - <span data-ttu-id="c9e9c-136">Om du uppmanas att välja **arbets-eller skol konto** eller **personligt konto** väljer du **arbets-eller skol konto**.</span><span class="sxs-lookup"><span data-stu-id="c9e9c-136">If you're prompted to select **Work or school account** or **Personal Account**, select **Work or school account**.</span></span>

2. <span data-ttu-id="c9e9c-137">Välj kugg hjuls ikonen för att öppna menyn **Inställningar** och välj sedan **konto inställningar**.</span><span class="sxs-lookup"><span data-stu-id="c9e9c-137">Select the gear icon to open the **Settings** menu, and then select **Account settings**.</span></span>

3. <span data-ttu-id="c9e9c-138">I menyn **konto inställningar** väljer du **utbetalning och skatt**.</span><span class="sxs-lookup"><span data-stu-id="c9e9c-138">In the **Account settings** menu, select **Payout and tax**.</span></span> 

## <a name="assign-payout-and-tax-profiles-to-individual-programs"></a><span data-ttu-id="c9e9c-139">Tilldela utbetalnings-och skatte profiler till enskilda program</span><span class="sxs-lookup"><span data-stu-id="c9e9c-139">Assign payout and tax profiles to individual programs</span></span>

1. <span data-ttu-id="c9e9c-140">Logga in på [partner Center-instrumentpanelen](https://partner.microsoft.com/dashboard/)och välj sedan kugg hjuls ikonen för att öppna menyn **Inställningar** .</span><span class="sxs-lookup"><span data-stu-id="c9e9c-140">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/), and then select the gear icon to open the **Settings** menu.</span></span> 

2. <span data-ttu-id="c9e9c-141">Välj **konto inställningar**, expandera **avsnittet utbetalning och skatt** och välj sedan **utbetalning och skatte profil tilldelning**.</span><span class="sxs-lookup"><span data-stu-id="c9e9c-141">Select **Account settings**, expand the **Payout and tax section**, and then select **Payout and tax profile assignment**.</span></span> 
   
   <span data-ttu-id="c9e9c-142">En lista över dina program kommer att visas.</span><span class="sxs-lookup"><span data-stu-id="c9e9c-142">A list of your programs will be displayed.</span></span> <span data-ttu-id="c9e9c-143">Välj pilen bredvid ett program om du vill se profil information.</span><span class="sxs-lookup"><span data-stu-id="c9e9c-143">Select the arrow next to a program to see profile details.</span></span> 

3. <span data-ttu-id="c9e9c-144">I list rutan **skatte profil** väljer du den skatte profil du vill använda, eller så väljer du alternativet för att skapa en ny profil.</span><span class="sxs-lookup"><span data-stu-id="c9e9c-144">In the **Tax Profile** dropdown menu, select the tax profile you want, or select the option to create a new profile.</span></span> <span data-ttu-id="c9e9c-145">När du väljer alternativet för att skapa en ny profil kommer du att omdirigeras på rätt sätt.</span><span class="sxs-lookup"><span data-stu-id="c9e9c-145">When you select the option to create a new profile, you’ll be redirected appropriately.</span></span>  <span data-ttu-id="c9e9c-146">Välj Fortsätt i popup-fönstret.</span><span class="sxs-lookup"><span data-stu-id="c9e9c-146">Select Continue in the pop-up window.</span></span> <span data-ttu-id="c9e9c-147">Processen för att skapa en ny skatte profil har angetts nedan.</span><span class="sxs-lookup"><span data-stu-id="c9e9c-147">The process for creating a new tax profile has been provided below.</span></span>

4. <span data-ttu-id="c9e9c-148">Välj **betalnings sätt**.</span><span class="sxs-lookup"><span data-stu-id="c9e9c-148">Select **Payment method**.</span></span>

   - <span data-ttu-id="c9e9c-149">Om du har valt **elektronisk bank överföring** som betalnings metod väljer du den betalnings profil som du vill använda, eller så väljer du alternativet för att skapa en ny profil.</span><span class="sxs-lookup"><span data-stu-id="c9e9c-149">If you have selected **Electronic bank transfer** as your payment method, select the payment profile you want, or select the option to create a new profile.</span></span> <span data-ttu-id="c9e9c-150">När du väljer alternativet för att skapa en ny profil kommer du att omdirigeras på rätt sätt.</span><span class="sxs-lookup"><span data-stu-id="c9e9c-150">When you select the option to create a new profile, you’ll be redirected appropriately.</span></span> <span data-ttu-id="c9e9c-151">Välj Fortsätt i popup-fönstret.</span><span class="sxs-lookup"><span data-stu-id="c9e9c-151">Select Continue in the pop-up window.</span></span> <span data-ttu-id="c9e9c-152">Processen för att skapa en ny betalnings profil har angetts nedan.</span><span class="sxs-lookup"><span data-stu-id="c9e9c-152">The process for creating a new payment profile has been provided below.</span></span>

   - <span data-ttu-id="c9e9c-153">Om du har valt **kredit anteckning** som betalnings metod slutför du verifieringen.</span><span class="sxs-lookup"><span data-stu-id="c9e9c-153">If you have selected **Credit Note** as your payment method, then complete the verification.</span></span> <span data-ttu-id="c9e9c-154">Detta bekräftar att det refererade SAP-numret tillhör din organisation.</span><span class="sxs-lookup"><span data-stu-id="c9e9c-154">This confirms that the referenced SAP number belongs to your organization.</span></span>

    >[!NOTE]
    ><span data-ttu-id="c9e9c-155">Om det finns flera Microsoft Business-entiteter i listan måste du välja en betalnings profil för varje entitet.</span><span class="sxs-lookup"><span data-stu-id="c9e9c-155">If there are multiple Microsoft business entities listed, you must select a payment profile for each entity.</span></span>

    >[!NOTE]
    ><span data-ttu-id="c9e9c-156">Tillgängligheten för betalnings metoden är beroende av reglerna i stimulans programmet.</span><span class="sxs-lookup"><span data-stu-id="c9e9c-156">The payment method availability is dependent on the rules of the incentive program.</span></span>
    
5. <span data-ttu-id="c9e9c-157">Välj **valuta**.</span><span class="sxs-lookup"><span data-stu-id="c9e9c-157">Select the **Currency**.</span></span>

6. <span data-ttu-id="c9e9c-158">När du har slutfört alla betalnings fält väljer du **Skicka**.</span><span class="sxs-lookup"><span data-stu-id="c9e9c-158">When you’ve completed all of the payment fields, select **Submit**.</span></span>

## <a name="create-your-bank-profile"></a><span data-ttu-id="c9e9c-159">Skapa din bank profil</span><span class="sxs-lookup"><span data-stu-id="c9e9c-159">Create your bank profile</span></span>

<span data-ttu-id="c9e9c-160">Bank profiler skapas på organisations nivå.</span><span class="sxs-lookup"><span data-stu-id="c9e9c-160">Bank profiles are created at an organization level.</span></span> <span data-ttu-id="c9e9c-161">Detta gör att en bank profil kan tilldelas över flera MPN-ID: n och incitaments program inom en organisation.</span><span class="sxs-lookup"><span data-stu-id="c9e9c-161">This allows one bank profile to be assigned across multiple MPN ID’s and incentive programs within an organization.</span></span> <span data-ttu-id="c9e9c-162">Det kan finnas undantag när du tillämpar bank profilen på olika länder, eftersom olika bank-och skatte regler kan tillämpas.</span><span class="sxs-lookup"><span data-stu-id="c9e9c-162">There may be exceptions when applying the banking profile to different countries, as different banking and tax rules may apply.</span></span>

>[!NOTE]
><span data-ttu-id="c9e9c-163">På följande sidor krävs fält med en asterisk.</span><span class="sxs-lookup"><span data-stu-id="c9e9c-163">On the following pages, fields with an asterisk are required.</span></span> <span data-ttu-id="c9e9c-164">Om du inte vet vad ett fält är väljer du informations ikonen.</span><span class="sxs-lookup"><span data-stu-id="c9e9c-164">If you don’t know what a field is, select the information icon.</span></span> 

1. <span data-ttu-id="c9e9c-165">På sidan **information** fyller du i följande fält: **profil namn:** ange ett unikt namn för att identifiera betalnings profilen.</span><span class="sxs-lookup"><span data-stu-id="c9e9c-165">On the **Details** page, complete the following fields: **Profile name:** Enter a unique name to identify this payment profile.</span></span>
    <span data-ttu-id="c9e9c-166">**Bank konto plats:** Det land där ditt företags bank befinner sig.</span><span class="sxs-lookup"><span data-stu-id="c9e9c-166">**Bank account location:** The country in which your company’s bank is located.</span></span>
    <span data-ttu-id="c9e9c-167">**Betalnings metod:** Den prioriterade betalnings metoden för partner Center är elektronisk bank överföring.</span><span class="sxs-lookup"><span data-stu-id="c9e9c-167">**Payment method:** The preferred payment method for Partner Center is electronic bank transfer.</span></span>

2. <span data-ttu-id="c9e9c-168">Välj **Nästa**.</span><span class="sxs-lookup"><span data-stu-id="c9e9c-168">Select **Next**.</span></span>

3. <span data-ttu-id="c9e9c-169">Ange din information på sidan **bank konto** .</span><span class="sxs-lookup"><span data-stu-id="c9e9c-169">On the **Bank account** page, enter your information.</span></span> <span data-ttu-id="c9e9c-170">Fälten som visas på den här sidan varierar efter land.</span><span class="sxs-lookup"><span data-stu-id="c9e9c-170">Fields shown on this page will vary by country.</span></span> 

4. <span data-ttu-id="c9e9c-171">Välj **Nästa**.</span><span class="sxs-lookup"><span data-stu-id="c9e9c-171">Select **Next**.</span></span>

5. <span data-ttu-id="c9e9c-172">Ange lämplig information på sidan **mottagare** .</span><span class="sxs-lookup"><span data-stu-id="c9e9c-172">On the **Beneficiary** page, enter the appropriate information.</span></span> <span data-ttu-id="c9e9c-173">Mottagaren är den person i företaget som banken kontaktar om de behöver diskutera ditt konto.</span><span class="sxs-lookup"><span data-stu-id="c9e9c-173">The beneficiary is the person in your company that the bank would contact if they need to discuss your account.</span></span>

6. <span data-ttu-id="c9e9c-174">När fälten har slutförts väljer du **Slutför** och väljer sedan **Bekräfta** för att skapa din bank profil.</span><span class="sxs-lookup"><span data-stu-id="c9e9c-174">When the fields are completed, select **Finish**, and then select **Confirm** to create your bank profile.</span></span>

<span data-ttu-id="c9e9c-175">Du omdirigeras till sidan **utbetalnings-och skatte profiler** .</span><span class="sxs-lookup"><span data-stu-id="c9e9c-175">You’ll be redirected to the **Payout and tax profiles** page.</span></span> <span data-ttu-id="c9e9c-176">Status för din nya profil återspeglar **väntande Microsoft-verifiering** tills verifieringen har slutförts.</span><span class="sxs-lookup"><span data-stu-id="c9e9c-176">The status of your new profile will reflect **Pending Microsoft validation** until the validation has been completed.</span></span> <span data-ttu-id="c9e9c-177">Den här processen kan ta upp till 48 timmar.</span><span class="sxs-lookup"><span data-stu-id="c9e9c-177">This process may take up to 48 hours.</span></span> <span data-ttu-id="c9e9c-178">När verifieringen har slutförts visas din profil status antingen **godkänd** eller **åtgärd krävs**.</span><span class="sxs-lookup"><span data-stu-id="c9e9c-178">Once validation has been completed, your profile status will reflect either **Approved** or **Action required**.</span></span> <span data-ttu-id="c9e9c-179">Om **åtgärden krävs** upprepar du stegen ovan för att ange den information som krävs.</span><span class="sxs-lookup"><span data-stu-id="c9e9c-179">If **Action Required**, repeat the steps above providing the necessary information.</span></span> 

## <a name="create-your-tax-profile"></a><span data-ttu-id="c9e9c-180">Skapa din skatte profil</span><span class="sxs-lookup"><span data-stu-id="c9e9c-180">Create your tax profile</span></span>

<span data-ttu-id="c9e9c-181">Använd följande procedur för att förse Microsoft med den skatte information som krävs för din organisation.</span><span class="sxs-lookup"><span data-stu-id="c9e9c-181">Use the following procedure to provide Microsoft with the tax information required for your organization.</span></span> <span data-ttu-id="c9e9c-182">Sidorna i det här avsnittet är dynamiska och varierar beroende på ditt land eller din region.</span><span class="sxs-lookup"><span data-stu-id="c9e9c-182">The pages in this section are dynamic and will vary according to your country or region.</span></span> <span data-ttu-id="c9e9c-183">Om du behöver hjälp med att identifiera rätt skatte information kontaktar du rätt myndighets källor i ditt land.</span><span class="sxs-lookup"><span data-stu-id="c9e9c-183">If you need help with identifying the correct tax information, contact the appropriate government sources in your country.</span></span>

<span data-ttu-id="c9e9c-184">För partner företag i Amerika, om du behöver information om hur du fyller i W8-eller W9-formulär, tar följande adresser till IRS-webbplatsen:</span><span class="sxs-lookup"><span data-stu-id="c9e9c-184">For partner companies in the Americas, if you require information on completing the W8 or W9 forms, the following addresses take you to the IRS site:</span></span>

- [http://www.irs.gov/pub/irs-pdf/iw8.pdf](http://www.irs.gov/pub/irs-pdf/iw8.pdf)
- [http://www.irs.gov/pub/irs-pdf/iw9.pdf](http://www.irs.gov/pub/irs-pdf/iw9.pdf)

>[!IMPORTANT]
> <span data-ttu-id="c9e9c-185">Ange endast information för ditt företag.</span><span class="sxs-lookup"><span data-stu-id="c9e9c-185">Enter only details for your company.</span></span> <span data-ttu-id="c9e9c-186">Ange aldrig personlig information.</span><span class="sxs-lookup"><span data-stu-id="c9e9c-186">Never enter personal details.</span></span>

1. <span data-ttu-id="c9e9c-187">Fyll i de obligatoriska fälten på sidan **företags profil** och välj sedan **Nästa**.</span><span class="sxs-lookup"><span data-stu-id="c9e9c-187">On the **Business Profile** page, complete the required fields and then select **Next**.</span></span> 

2. <span data-ttu-id="c9e9c-188">På sidan **installation** väljer du det alternativ som gäller för ditt företag.</span><span class="sxs-lookup"><span data-stu-id="c9e9c-188">On the **Setup** page, select the option that applies to your company.</span></span>

   - <span data-ttu-id="c9e9c-189">Välj alternativet till vänster om ditt företag ingår i endast USA, eller om profilen är för en person.</span><span class="sxs-lookup"><span data-stu-id="c9e9c-189">Select the option on the left if your company is incorporated in the United States only, or if this profile is for an individual.</span></span>
   - <span data-ttu-id="c9e9c-190">Välj alternativet till höger om ditt företag är införlivat utanför USA och välj sedan land/region i listan.</span><span class="sxs-lookup"><span data-stu-id="c9e9c-190">Select the option on the right if your company is incorporated outside of the United States, and then select your country/region from the list.</span></span>

3. <span data-ttu-id="c9e9c-191">Välj **Nästa**.</span><span class="sxs-lookup"><span data-stu-id="c9e9c-191">Select **Next**.</span></span> 

4. <span data-ttu-id="c9e9c-192">Ange den information som krävs på sidan **moms status** och välj sedan **Nästa**.</span><span class="sxs-lookup"><span data-stu-id="c9e9c-192">On the **Tax status** page, enter the required information, and then select **Next**.</span></span> <span data-ttu-id="c9e9c-193">Fälten på den här sidan varierar efter land.</span><span class="sxs-lookup"><span data-stu-id="c9e9c-193">Fields on this page will vary by country.</span></span> <span data-ttu-id="c9e9c-194">din information.</span><span class="sxs-lookup"><span data-stu-id="c9e9c-194">your details.</span></span> 

5. <span data-ttu-id="c9e9c-195">På sidan **Ytterligare dokumentation** , de obligatoriska fälten och välj **Nästa**.</span><span class="sxs-lookup"><span data-stu-id="c9e9c-195">On the **Additional documentation** page, the required fields and select **Next**.</span></span> 

6. <span data-ttu-id="c9e9c-196">Välj **Bläddra** för att ladda upp dokument som krävs av ditt land eller din region.</span><span class="sxs-lookup"><span data-stu-id="c9e9c-196">Select **Browse** to upload any documents required by your country or region.</span></span> <span data-ttu-id="c9e9c-197">När dokument namnet visas väljer du **överför**.</span><span class="sxs-lookup"><span data-stu-id="c9e9c-197">When the document name is shown, select **Upload**.</span></span> 

7. <span data-ttu-id="c9e9c-198">Om du behöver ta bort dokumentet väljer du **ta bort**.</span><span class="sxs-lookup"><span data-stu-id="c9e9c-198">If you need to remove the document, select **Remove**.</span></span>

8. <span data-ttu-id="c9e9c-199">Välj **Slutför** för att spara och fortsätta.</span><span class="sxs-lookup"><span data-stu-id="c9e9c-199">To save and continue, select **Finish**.</span></span>

9. <span data-ttu-id="c9e9c-200">Välj **Bekräfta** i popup-meddelandet.</span><span class="sxs-lookup"><span data-stu-id="c9e9c-200">Select **Confirm** on the pop-up message.</span></span> <span data-ttu-id="c9e9c-201">Du kommer tillbaka till sidan för **utbetalning och skatte inställningar** .</span><span class="sxs-lookup"><span data-stu-id="c9e9c-201">You’ll be taken back to the **Payout and tax setup** page.</span></span>

## <a name="next-steps"></a><span data-ttu-id="c9e9c-202">Nästa steg</span><span class="sxs-lookup"><span data-stu-id="c9e9c-202">Next steps</span></span>

- [<span data-ttu-id="c9e9c-203">Vanliga frågor om utbetalningar och skatter</span><span class="sxs-lookup"><span data-stu-id="c9e9c-203">Common questions about payouts and taxes</span></span>](payout-faq.md)
