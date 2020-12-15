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
ms.openlocfilehash: 1e97e2e9db798e5ef90858cf96dc06602bbfe427
ms.sourcegitcommit: 4e36d1a4ca2f074b55f9b9a08e300734eae1f06d
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 12/15/2020
ms.locfileid: "97492474"
---
# <a name="create-and-manage-incentives-payout-and-tax-profiles-in-partner-center"></a><span data-ttu-id="17e3e-104">Skapa och hantera incitaments utbetalningar och skatte profiler i Partner Center</span><span class="sxs-lookup"><span data-stu-id="17e3e-104">Create and manage incentives payout and tax profiles in Partner Center</span></span>

<span data-ttu-id="17e3e-105">**Gäller för:**</span><span class="sxs-lookup"><span data-stu-id="17e3e-105">**Applies to:**</span></span>

- <span data-ttu-id="17e3e-106">Partnercenter</span><span class="sxs-lookup"><span data-stu-id="17e3e-106">Partner Center</span></span>

<span data-ttu-id="17e3e-107">**Lämpliga roller:**</span><span class="sxs-lookup"><span data-stu-id="17e3e-107">**Appropriate roles:**</span></span>

- <span data-ttu-id="17e3e-108">Incitaments administratör</span><span class="sxs-lookup"><span data-stu-id="17e3e-108">Incentives admin</span></span>
- <span data-ttu-id="17e3e-109">Kontoadministratör</span><span class="sxs-lookup"><span data-stu-id="17e3e-109">Account admin</span></span>
- <span data-ttu-id="17e3e-110">Global administratör</span><span class="sxs-lookup"><span data-stu-id="17e3e-110">Global admin</span></span>

<span data-ttu-id="17e3e-111">Innan du kan erhålla betalningar för dina incitamentprogram för en viss MPN-plats måste du slutföra registreringen genom att associera en giltig utbetalnings- och skatteprofil med programmet och MPN-platsen.</span><span class="sxs-lookup"><span data-stu-id="17e3e-111">Before you can receive payment for your incentive programs for a particular MPN location, you must complete your enrollment by associating a valid payout and tax profile with the program and MPN location.</span></span> <span data-ttu-id="17e3e-112">Microsoft använder den här utbetalnings- och skatteprofilen för att utfärda betalningar.</span><span class="sxs-lookup"><span data-stu-id="17e3e-112">Microsoft will use this payout and tax profile to issue payments.</span></span> <span data-ttu-id="17e3e-113">Eventuellt kan du välja att använda elektronisk banköverföring eller en kreditfaktura för betalningar, beroende på reglerna för incitamentprogrammet.</span><span class="sxs-lookup"><span data-stu-id="17e3e-113">You may be allowed to use electronic bank transfer or a credit note for payment, depending on the rules of the incentive program.</span></span> 

## <a name="roles-currencies-and-other-microsoft-programs"></a><span data-ttu-id="17e3e-114">Roller, valutor och andra Microsoft-program</span><span class="sxs-lookup"><span data-stu-id="17e3e-114">Roles, currencies, and other Microsoft programs</span></span>

<span data-ttu-id="17e3e-115">Det är viktigt att förstå informationen nedan innan du börjar med din utbetalnings-och skatte profil.</span><span class="sxs-lookup"><span data-stu-id="17e3e-115">It's important to understand the information below before you get started with your payout and tax profile.</span></span>

### <a name="roles-and-permissions"></a><span data-ttu-id="17e3e-116">Roller och behörigheter</span><span class="sxs-lookup"><span data-stu-id="17e3e-116">Roles and permissions</span></span>

<span data-ttu-id="17e3e-117">Du måste vara en incitaments administratör för att ange bank-och skatte information för incitaments betalningar.</span><span class="sxs-lookup"><span data-stu-id="17e3e-117">You must be an Incentives Admin to enter bank and tax information for incentive payments.</span></span> <span data-ttu-id="17e3e-118">Om du är MPN-/konto administratör kan du tilldela dig själv och/eller en kollega som incitaments administratör.</span><span class="sxs-lookup"><span data-stu-id="17e3e-118">If you're an MPN/Account Admin, you can assign yourself and/or a colleague to be the Incentives Admin.</span></span>

<span data-ttu-id="17e3e-119">Kontakta MPN-administratören eller den globala administratören om du behöver begära att be om administratörs behörighet. Du kan ta reda på vem i företaget som har dessa roller genom att logga in på [partner Center-instrumentpanelen](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="17e3e-119">If you need to request Incentives Admin permissions, contact your MPN Admin or Global Admin. You can find out who in your company has these roles by signing into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span> <span data-ttu-id="17e3e-120">Från **inställnings** ikonen längst upp till höger väljer du **användar hantering** och filtrerar sedan på global administratör.</span><span class="sxs-lookup"><span data-stu-id="17e3e-120">From the **Settings** icon at the top right, select **User Management** and then filter on Global Admin.</span></span>

<span data-ttu-id="17e3e-121">Incitaments användare kan se incitaments vinster och betalnings information och rapporter, men kan inte redigera bank-och skatte information.</span><span class="sxs-lookup"><span data-stu-id="17e3e-121">Incentives Users can view Incentive earnings and payment details and reports, but can’t edit bank and tax details.</span></span>

### <a name="choose-your-disbursement-currency"></a><span data-ttu-id="17e3e-122">Välj din utbetalnings valuta</span><span class="sxs-lookup"><span data-stu-id="17e3e-122">Choose your disbursement currency</span></span>

<span data-ttu-id="17e3e-123">Incitaments betalningar görs i den valuta som du valde när du konfigurerade din betalnings profil.</span><span class="sxs-lookup"><span data-stu-id="17e3e-123">Incentive payments are made in the currency you selected when you set up your payment profile.</span></span> <span data-ttu-id="17e3e-124">Betalningarna beräknas med en växelkurs som ställs in månatlig av Microsoft.</span><span class="sxs-lookup"><span data-stu-id="17e3e-124">Payments will be calculated using an exchange rate as set monthly by Microsoft.</span></span> <span data-ttu-id="17e3e-125">Du ansvarar för alla ändringar i värdet på grund av vald valuta.</span><span class="sxs-lookup"><span data-stu-id="17e3e-125">You’ll be responsible for any changes in value due to the currency selected.</span></span>

### <a name="using-different-profiles-for-different-microsoft-programs"></a><span data-ttu-id="17e3e-126">Använda olika profiler för olika Microsoft-program</span><span class="sxs-lookup"><span data-stu-id="17e3e-126">Using different profiles for different Microsoft programs</span></span>

<span data-ttu-id="17e3e-127">Om ditt företag är registrerat i flera incitaments program kan du använda samma betalnings konto för alla, eller välja att använda olika betalnings konton för olika program.</span><span class="sxs-lookup"><span data-stu-id="17e3e-127">If your company is enrolled in multiple incentive programs, you can use the same payment account for all of them, or choose to use different payment accounts for different programs.</span></span>

## <a name="create-and-manage-payout-and-tax-profiles-in-partner-center"></a><span data-ttu-id="17e3e-128">Skapa och hantera utbetalnings-och skatte profiler i Partner Center</span><span class="sxs-lookup"><span data-stu-id="17e3e-128">Create and manage payout and tax profiles in Partner Center</span></span>

<span data-ttu-id="17e3e-129">I avsnitten nedan får du stegvisa anvisningar genom processen att skapa och hantera betalnings-och skatte profiler i Partner Center.</span><span class="sxs-lookup"><span data-stu-id="17e3e-129">The sections below will walk you through the process of creating and managing payment and tax profiles in Partner Center.</span></span>

>[!IMPORTANT]
><span data-ttu-id="17e3e-130">Du måste vara en incitaments administratör för att skapa eller hantera betalnings profiler i Partner Center.</span><span class="sxs-lookup"><span data-stu-id="17e3e-130">You must be an Incentive admin to create or manage payment profiles in Partner Center.</span></span> <span data-ttu-id="17e3e-131">Stimulans roller måste tilldelas till varje MPN-plats under varje incitaments program.</span><span class="sxs-lookup"><span data-stu-id="17e3e-131">Incentive roles must be assigned to each MPN location under each incentive program.</span></span> <span data-ttu-id="17e3e-132">Mer information om hur du lägger till stimulans administratörer i Partner Center finns i [skapa användar konton](create-user-accounts-and-set-permissions.md).</span><span class="sxs-lookup"><span data-stu-id="17e3e-132">For more information on how to add Incentive admins in Partner Center, see [Create user accounts](create-user-accounts-and-set-permissions.md).</span></span>

## <a name="access-the-payout-and-tax-section-in-partner-center"></a><span data-ttu-id="17e3e-133">Gå till avsnittet utbetalnings-och skatte avsnitt i Partner Center</span><span class="sxs-lookup"><span data-stu-id="17e3e-133">Access the payout and tax section in Partner Center</span></span>

1. <span data-ttu-id="17e3e-134">Logga in på [partner Center-instrumentpanelen](https://partner.microsoft.com/dashboard/) med ditt Azure Active Directory (Azure AD)-konto (företags konto) eller lämplig e-postadress om ett har tilldelats.</span><span class="sxs-lookup"><span data-stu-id="17e3e-134">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/) using your Azure Active Directory (Azure AD) account (company account), or the appropriate email address if one was assigned.</span></span>

   - <span data-ttu-id="17e3e-135">Flera domäner kan registreras i ett Azure AD-konto.</span><span class="sxs-lookup"><span data-stu-id="17e3e-135">Multiple domains can be registered within one Azure AD account.</span></span> <span data-ttu-id="17e3e-136">Kontakta din globala administratör för att avgöra vilka domäner som är associerade.</span><span class="sxs-lookup"><span data-stu-id="17e3e-136">Contact your Global admin to determine which domains are associated.</span></span>
   - <span data-ttu-id="17e3e-137">Om du bara kan logga in med @onmicrosoft.com domänen kontaktar du konto administratören för att lägga till ytterligare domäner i Azure AD-kontot.</span><span class="sxs-lookup"><span data-stu-id="17e3e-137">If you're only able to log in with the @onmicrosoft.com domain, contact your Account admin to add additional domains to the Azure AD account.</span></span>
   - <span data-ttu-id="17e3e-138">Om du uppmanas att välja **arbets-eller skol konto** eller **personligt konto** väljer du **arbets-eller skol konto**.</span><span class="sxs-lookup"><span data-stu-id="17e3e-138">If you're prompted to select **Work or school account** or **Personal Account**, select **Work or school account**.</span></span>

2. <span data-ttu-id="17e3e-139">Välj kugg hjuls ikonen för att öppna menyn **Inställningar** och välj sedan **partner inställningar**.</span><span class="sxs-lookup"><span data-stu-id="17e3e-139">Select the gear icon to open the **Settings** menu, and then select **Partner settings**.</span></span>

3. <span data-ttu-id="17e3e-140">I menyn **konto inställningar** väljer du **utbetalning och skatt**.</span><span class="sxs-lookup"><span data-stu-id="17e3e-140">In the **Account settings** menu, select **Payout and tax**.</span></span> 

## <a name="assign-payout-and-tax-profiles-to-individual-programs"></a><span data-ttu-id="17e3e-141">Tilldela utbetalnings-och skatte profiler till enskilda program</span><span class="sxs-lookup"><span data-stu-id="17e3e-141">Assign payout and tax profiles to individual programs</span></span>

1. <span data-ttu-id="17e3e-142">Logga in på [partner Center-instrumentpanelen](https://partner.microsoft.com/dashboard/)och välj sedan kugg hjuls ikonen för att öppna menyn **Inställningar** .</span><span class="sxs-lookup"><span data-stu-id="17e3e-142">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/), and then select the gear icon to open the **Settings** menu.</span></span> 

2. <span data-ttu-id="17e3e-143">Välj **partner inställningar**, expandera **avsnittet utbetalning och skatt** och välj sedan **utbetalning och skatte profil tilldelning**.</span><span class="sxs-lookup"><span data-stu-id="17e3e-143">Select **Partner settings**, expand the **Payout and tax section**, and then select **Payout and tax profile assignment**.</span></span> 
   
   <span data-ttu-id="17e3e-144">En lista över dina program kommer att visas.</span><span class="sxs-lookup"><span data-stu-id="17e3e-144">A list of your programs will be displayed.</span></span> <span data-ttu-id="17e3e-145">Välj pilen bredvid ett program om du vill se profil information.</span><span class="sxs-lookup"><span data-stu-id="17e3e-145">Select the arrow next to a program to see profile details.</span></span> 

3. <span data-ttu-id="17e3e-146">I list rutan **skatte profil** väljer du den skatte profil du vill använda, eller så väljer du alternativet för att skapa en ny profil.</span><span class="sxs-lookup"><span data-stu-id="17e3e-146">In the **Tax Profile** dropdown menu, select the tax profile you want, or select the option to create a new profile.</span></span> <span data-ttu-id="17e3e-147">När du väljer alternativet för att skapa en ny profil kommer du att omdirigeras på rätt sätt.</span><span class="sxs-lookup"><span data-stu-id="17e3e-147">When you select the option to create a new profile, you’ll be redirected appropriately.</span></span>  <span data-ttu-id="17e3e-148">Välj Fortsätt i popup-fönstret.</span><span class="sxs-lookup"><span data-stu-id="17e3e-148">Select Continue in the pop-up window.</span></span> <span data-ttu-id="17e3e-149">Processen för att skapa en ny skatte profil har angetts nedan.</span><span class="sxs-lookup"><span data-stu-id="17e3e-149">The process for creating a new tax profile has been provided below.</span></span>

4. <span data-ttu-id="17e3e-150">Välj **betalnings sätt**.</span><span class="sxs-lookup"><span data-stu-id="17e3e-150">Select **Payment method**.</span></span>

   - <span data-ttu-id="17e3e-151">Om du har valt **elektronisk bank överföring** som betalnings metod väljer du den betalnings profil som du vill använda, eller så väljer du alternativet för att skapa en ny profil.</span><span class="sxs-lookup"><span data-stu-id="17e3e-151">If you have selected **Electronic bank transfer** as your payment method, select the payment profile you want, or select the option to create a new profile.</span></span> <span data-ttu-id="17e3e-152">När du väljer alternativet för att skapa en ny profil kommer du att omdirigeras på rätt sätt.</span><span class="sxs-lookup"><span data-stu-id="17e3e-152">When you select the option to create a new profile, you’ll be redirected appropriately.</span></span> <span data-ttu-id="17e3e-153">Välj Fortsätt i popup-fönstret.</span><span class="sxs-lookup"><span data-stu-id="17e3e-153">Select Continue in the pop-up window.</span></span> <span data-ttu-id="17e3e-154">Processen för att skapa en ny betalnings profil har angetts nedan.</span><span class="sxs-lookup"><span data-stu-id="17e3e-154">The process for creating a new payment profile has been provided below.</span></span>

   - <span data-ttu-id="17e3e-155">Om du har valt **kredit anteckning** som betalnings metod slutför du verifieringen.</span><span class="sxs-lookup"><span data-stu-id="17e3e-155">If you have selected **Credit Note** as your payment method, then complete the verification.</span></span> <span data-ttu-id="17e3e-156">Detta bekräftar att det refererade SAP-numret tillhör din organisation.</span><span class="sxs-lookup"><span data-stu-id="17e3e-156">This confirms that the referenced SAP number belongs to your organization.</span></span>

    >[!NOTE]
    ><span data-ttu-id="17e3e-157">Om det finns flera Microsoft Business-entiteter i listan måste du välja en betalnings profil för varje entitet.</span><span class="sxs-lookup"><span data-stu-id="17e3e-157">If there are multiple Microsoft business entities listed, you must select a payment profile for each entity.</span></span>

    >[!NOTE]
    ><span data-ttu-id="17e3e-158">Tillgängligheten för betalnings metoden är beroende av reglerna i stimulans programmet.</span><span class="sxs-lookup"><span data-stu-id="17e3e-158">The payment method availability is dependent on the rules of the incentive program.</span></span>
    
5. <span data-ttu-id="17e3e-159">Välj **valuta**.</span><span class="sxs-lookup"><span data-stu-id="17e3e-159">Select the **Currency**.</span></span>

6. <span data-ttu-id="17e3e-160">När du har slutfört alla betalnings fält väljer du **Skicka**.</span><span class="sxs-lookup"><span data-stu-id="17e3e-160">When you’ve completed all of the payment fields, select **Submit**.</span></span>

## <a name="create-your-bank-profile"></a><span data-ttu-id="17e3e-161">Skapa din bank profil</span><span class="sxs-lookup"><span data-stu-id="17e3e-161">Create your bank profile</span></span>

<span data-ttu-id="17e3e-162">Bank profiler skapas på organisations nivå.</span><span class="sxs-lookup"><span data-stu-id="17e3e-162">Bank profiles are created at an organization level.</span></span> <span data-ttu-id="17e3e-163">Detta gör att en bank profil kan tilldelas över flera MPN-ID: n och incitaments program inom en organisation.</span><span class="sxs-lookup"><span data-stu-id="17e3e-163">This allows one bank profile to be assigned across multiple MPN ID’s and incentive programs within an organization.</span></span> <span data-ttu-id="17e3e-164">Det kan finnas undantag när du tillämpar bank profilen på olika länder, eftersom olika bank-och skatte regler kan tillämpas.</span><span class="sxs-lookup"><span data-stu-id="17e3e-164">There may be exceptions when applying the banking profile to different countries, as different banking and tax rules may apply.</span></span>

>[!NOTE]
><span data-ttu-id="17e3e-165">På följande sidor krävs fält med en asterisk.</span><span class="sxs-lookup"><span data-stu-id="17e3e-165">On the following pages, fields with an asterisk are required.</span></span> <span data-ttu-id="17e3e-166">Om du inte vet vad ett fält är väljer du informations ikonen.</span><span class="sxs-lookup"><span data-stu-id="17e3e-166">If you don’t know what a field is, select the information icon.</span></span> 

1. <span data-ttu-id="17e3e-167">På sidan **information** fyller du i följande fält: **profil namn:** ange ett unikt namn för att identifiera betalnings profilen.</span><span class="sxs-lookup"><span data-stu-id="17e3e-167">On the **Details** page, complete the following fields: **Profile name:** Enter a unique name to identify this payment profile.</span></span>
    <span data-ttu-id="17e3e-168">**Bank konto plats:** Det land där ditt företags bank befinner sig.</span><span class="sxs-lookup"><span data-stu-id="17e3e-168">**Bank account location:** The country in which your company’s bank is located.</span></span>
    <span data-ttu-id="17e3e-169">**Betalnings metod:** Den prioriterade betalnings metoden för partner Center är elektronisk bank överföring.</span><span class="sxs-lookup"><span data-stu-id="17e3e-169">**Payment method:** The preferred payment method for Partner Center is electronic bank transfer.</span></span>

2. <span data-ttu-id="17e3e-170">Välj **Nästa**.</span><span class="sxs-lookup"><span data-stu-id="17e3e-170">Select **Next**.</span></span>

3. <span data-ttu-id="17e3e-171">Ange din information på sidan **bank konto** .</span><span class="sxs-lookup"><span data-stu-id="17e3e-171">On the **Bank account** page, enter your information.</span></span> <span data-ttu-id="17e3e-172">Fälten som visas på den här sidan varierar efter land.</span><span class="sxs-lookup"><span data-stu-id="17e3e-172">Fields shown on this page will vary by country.</span></span> 

4. <span data-ttu-id="17e3e-173">Välj **Nästa**.</span><span class="sxs-lookup"><span data-stu-id="17e3e-173">Select **Next**.</span></span>

5. <span data-ttu-id="17e3e-174">Ange lämplig information på sidan **mottagare** .</span><span class="sxs-lookup"><span data-stu-id="17e3e-174">On the **Beneficiary** page, enter the appropriate information.</span></span> <span data-ttu-id="17e3e-175">Mottagaren är den person i företaget som banken kontaktar om de behöver diskutera ditt konto.</span><span class="sxs-lookup"><span data-stu-id="17e3e-175">The beneficiary is the person in your company that the bank would contact if they need to discuss your account.</span></span>

6. <span data-ttu-id="17e3e-176">När fälten har slutförts väljer du **Slutför** och väljer sedan **Bekräfta** för att skapa din bank profil.</span><span class="sxs-lookup"><span data-stu-id="17e3e-176">When the fields are completed, select **Finish**, and then select **Confirm** to create your bank profile.</span></span>

<span data-ttu-id="17e3e-177">Du omdirigeras till sidan **utbetalnings-och skatte profiler** .</span><span class="sxs-lookup"><span data-stu-id="17e3e-177">You’ll be redirected to the **Payout and tax profiles** page.</span></span> <span data-ttu-id="17e3e-178">Status för din nya profil återspeglar **väntande Microsoft-verifiering** tills verifieringen har slutförts.</span><span class="sxs-lookup"><span data-stu-id="17e3e-178">The status of your new profile will reflect **Pending Microsoft validation** until the validation has been completed.</span></span> <span data-ttu-id="17e3e-179">Den här processen kan ta upp till 48 timmar.</span><span class="sxs-lookup"><span data-stu-id="17e3e-179">This process may take up to 48 hours.</span></span> <span data-ttu-id="17e3e-180">När verifieringen har slutförts visas din profil status antingen **godkänd** eller **åtgärd krävs**.</span><span class="sxs-lookup"><span data-stu-id="17e3e-180">Once validation has been completed, your profile status will reflect either **Approved** or **Action required**.</span></span> <span data-ttu-id="17e3e-181">Om **åtgärden krävs** upprepar du stegen ovan för att ange den information som krävs.</span><span class="sxs-lookup"><span data-stu-id="17e3e-181">If **Action Required**, repeat the steps above providing the necessary information.</span></span> 

## <a name="create-your-tax-profile"></a><span data-ttu-id="17e3e-182">Skapa din skatte profil</span><span class="sxs-lookup"><span data-stu-id="17e3e-182">Create your tax profile</span></span>

<span data-ttu-id="17e3e-183">Använd följande procedur för att förse Microsoft med den skatte information som krävs för din organisation.</span><span class="sxs-lookup"><span data-stu-id="17e3e-183">Use the following procedure to provide Microsoft with the tax information required for your organization.</span></span> <span data-ttu-id="17e3e-184">Sidorna i det här avsnittet är dynamiska och varierar beroende på ditt land eller din region.</span><span class="sxs-lookup"><span data-stu-id="17e3e-184">The pages in this section are dynamic and will vary according to your country or region.</span></span> <span data-ttu-id="17e3e-185">Om du behöver hjälp med att identifiera rätt skatte information kontaktar du rätt myndighets källor i ditt land.</span><span class="sxs-lookup"><span data-stu-id="17e3e-185">If you need help with identifying the correct tax information, contact the appropriate government sources in your country.</span></span>

<span data-ttu-id="17e3e-186">För partner företag i Amerika, om du behöver information om hur du fyller i W8-eller W9-formulär, tar följande adresser till IRS-webbplatsen:</span><span class="sxs-lookup"><span data-stu-id="17e3e-186">For partner companies in the Americas, if you require information on completing the W8 or W9 forms, the following addresses take you to the IRS site:</span></span>

- [http://www.irs.gov/pub/irs-pdf/iw8.pdf](http://www.irs.gov/pub/irs-pdf/iw8.pdf)
- [http://www.irs.gov/pub/irs-pdf/iw9.pdf](http://www.irs.gov/pub/irs-pdf/iw9.pdf)

>[!IMPORTANT]
> <span data-ttu-id="17e3e-187">Ange endast information för ditt företag.</span><span class="sxs-lookup"><span data-stu-id="17e3e-187">Enter only details for your company.</span></span> <span data-ttu-id="17e3e-188">Ange aldrig personlig information.</span><span class="sxs-lookup"><span data-stu-id="17e3e-188">Never enter personal details.</span></span>

1. <span data-ttu-id="17e3e-189">Fyll i de obligatoriska fälten på sidan **företags profil** och välj sedan **Nästa**.</span><span class="sxs-lookup"><span data-stu-id="17e3e-189">On the **Business Profile** page, complete the required fields and then select **Next**.</span></span> 

2. <span data-ttu-id="17e3e-190">På sidan **installation** väljer du det alternativ som gäller för ditt företag.</span><span class="sxs-lookup"><span data-stu-id="17e3e-190">On the **Setup** page, select the option that applies to your company.</span></span>

   - <span data-ttu-id="17e3e-191">Välj alternativet till vänster om ditt företag ingår i endast USA, eller om profilen är för en person.</span><span class="sxs-lookup"><span data-stu-id="17e3e-191">Select the option on the left if your company is incorporated in the United States only, or if this profile is for an individual.</span></span>
   - <span data-ttu-id="17e3e-192">Välj alternativet till höger om ditt företag är införlivat utanför USA och välj sedan land/region i listan.</span><span class="sxs-lookup"><span data-stu-id="17e3e-192">Select the option on the right if your company is incorporated outside of the United States, and then select your country/region from the list.</span></span>

3. <span data-ttu-id="17e3e-193">Välj **Nästa**.</span><span class="sxs-lookup"><span data-stu-id="17e3e-193">Select **Next**.</span></span> 

4. <span data-ttu-id="17e3e-194">Ange den information som krävs på sidan **moms status** och välj sedan **Nästa**.</span><span class="sxs-lookup"><span data-stu-id="17e3e-194">On the **Tax status** page, enter the required information, and then select **Next**.</span></span> <span data-ttu-id="17e3e-195">Fälten på den här sidan varierar efter land.</span><span class="sxs-lookup"><span data-stu-id="17e3e-195">Fields on this page will vary by country.</span></span> <span data-ttu-id="17e3e-196">din information.</span><span class="sxs-lookup"><span data-stu-id="17e3e-196">your details.</span></span> 

5. <span data-ttu-id="17e3e-197">På sidan **Ytterligare dokumentation** , de obligatoriska fälten och välj **Nästa**.</span><span class="sxs-lookup"><span data-stu-id="17e3e-197">On the **Additional documentation** page, the required fields and select **Next**.</span></span> 

6. <span data-ttu-id="17e3e-198">Välj **Bläddra** för att ladda upp dokument som krävs av ditt land eller din region.</span><span class="sxs-lookup"><span data-stu-id="17e3e-198">Select **Browse** to upload any documents required by your country or region.</span></span> <span data-ttu-id="17e3e-199">När dokument namnet visas väljer du **överför**.</span><span class="sxs-lookup"><span data-stu-id="17e3e-199">When the document name is shown, select **Upload**.</span></span> 

7. <span data-ttu-id="17e3e-200">Om du behöver ta bort dokumentet väljer du **ta bort**.</span><span class="sxs-lookup"><span data-stu-id="17e3e-200">If you need to remove the document, select **Remove**.</span></span>

8. <span data-ttu-id="17e3e-201">Välj **Slutför** för att spara och fortsätta.</span><span class="sxs-lookup"><span data-stu-id="17e3e-201">To save and continue, select **Finish**.</span></span>

9. <span data-ttu-id="17e3e-202">Välj **Bekräfta** i popup-meddelandet.</span><span class="sxs-lookup"><span data-stu-id="17e3e-202">Select **Confirm** on the pop-up message.</span></span> <span data-ttu-id="17e3e-203">Du kommer tillbaka till sidan för **utbetalning och skatte inställningar** .</span><span class="sxs-lookup"><span data-stu-id="17e3e-203">You’ll be taken back to the **Payout and tax setup** page.</span></span>

## <a name="next-steps"></a><span data-ttu-id="17e3e-204">Nästa steg</span><span class="sxs-lookup"><span data-stu-id="17e3e-204">Next steps</span></span>

- [<span data-ttu-id="17e3e-205">Vanliga frågor om utbetalningar och skatter</span><span class="sxs-lookup"><span data-stu-id="17e3e-205">Common questions about payouts and taxes</span></span>](payout-faq.md)
