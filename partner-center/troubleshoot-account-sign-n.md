---
title: Felsöka konfiguration av ditt partner Center-konto eller problem med MPN-förnyelse
ms.topic: how-to
ms.date: 08/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Felsök problem när du försöker registrera dig i Partner Center. Svarar på utmaningar med betalnings metoder, Forgetting-lösenord och mycket annat.
author: ArpithaKanuganti
ms.author: v-arkanu
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 7d80651c4e5e4afb476dada388f23c118e0bdf25
ms.sourcegitcommit: 35fe0fdc41886f6f5af71ec74e4a4ebd245dfe1d
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/22/2021
ms.locfileid: "104768711"
---
# <a name="troubleshoot-account-setup-or-mpn-renewal-issues"></a><span data-ttu-id="e3928-104">Felsöka konto inställningar eller problem med MPN förnyelse</span><span class="sxs-lookup"><span data-stu-id="e3928-104">Troubleshoot account setup or MPN renewal issues</span></span>


<span data-ttu-id="e3928-105">**Lämpliga roller**</span><span class="sxs-lookup"><span data-stu-id="e3928-105">**Appropriate roles**</span></span>

- <span data-ttu-id="e3928-106">Global administratör</span><span class="sxs-lookup"><span data-stu-id="e3928-106">Global admin</span></span>
- <span data-ttu-id="e3928-107">MPN-partner administratör</span><span class="sxs-lookup"><span data-stu-id="e3928-107">MPN partner admin</span></span> 
 
<span data-ttu-id="e3928-108">Här följer några förslag på hur du felsöker vanliga problem som uppstår när du konfigurerar ditt partner Center-konto.</span><span class="sxs-lookup"><span data-stu-id="e3928-108">Here are some suggestions for troubleshooting common issues that arise when setting up your Partner Center account.</span></span>

## <a name="what-happens-if-you-are-migrating-from-partner-membership-center-and-you-cant-edit-any-company-information-fields"></a><span data-ttu-id="e3928-109">Vad händer om du migrerar från partner medlemskaps Center och du inte kan redigera företags informations fält</span><span class="sxs-lookup"><span data-stu-id="e3928-109">What happens if you are migrating from Partner Membership Center and you can't edit any company information fields</span></span>

<span data-ttu-id="e3928-110">I de fall där företaget redan har en närvaro i Partner Center (till exempel ett CSP-konto) – visas en skrivskyddad skärm.</span><span class="sxs-lookup"><span data-stu-id="e3928-110">In cases where your company already has a presence in Partner Center (for example, a CSP account) – you will be shown a read-only screen.</span></span> <span data-ttu-id="e3928-111">Den här skärmen visar all information om ditt företag som finns i Partner Center.</span><span class="sxs-lookup"><span data-stu-id="e3928-111">This screen will display all the information about your company as it exists in Partner Center.</span></span>

<span data-ttu-id="e3928-112">Du kan inte ändra informationen på den här skärmen.</span><span class="sxs-lookup"><span data-stu-id="e3928-112">You can't change the details on this screen.</span></span> <span data-ttu-id="e3928-113">Detta är avsiktligt och inte ett fel.</span><span class="sxs-lookup"><span data-stu-id="e3928-113">This is by design and not an error.</span></span>

<span data-ttu-id="e3928-114">Välj **Godkänn** och **Fortsätt** för att fortsätta.</span><span class="sxs-lookup"><span data-stu-id="e3928-114">Select **Accept** and **Continue** to proceed.</span></span>


### <a name="if-the-it-department-has-turned-off-sign-up-for-partner-center"></a><span data-ttu-id="e3928-115">Om IT-avdelningen har inaktiverat **registrering för partner Center**</span><span class="sxs-lookup"><span data-stu-id="e3928-115">If the IT department has turned off **Sign up for Partner Center**</span></span>

<span data-ttu-id="e3928-116">Du ser det här meddelandet eftersom virusbaserade användare är inaktiverade, eller om du har inaktiverat virus registrering på Azure AD-klienten.</span><span class="sxs-lookup"><span data-stu-id="e3928-116">You see this message because viral users are disabled, or because Viral Sign-up is disabled on the Azure AD tenant.</span></span> <span data-ttu-id="e3928-117">Den globala administratören för ditt Azure AD-konto kan aktivera nödvändiga funktioner genom att köra följande PowerShell-kommando:</span><span class="sxs-lookup"><span data-stu-id="e3928-117">The Global admin for your Azure AD account can enable required features by running the following PowerShell command:</span></span>

<span data-ttu-id="e3928-118">**Set-MsolCompanySettings-AllowEmailVerifiedUsers $true-AllowAdHocSubscriptions $true**</span><span class="sxs-lookup"><span data-stu-id="e3928-118">**Set-MsolCompanySettings -AllowEmailVerifiedUsers $true -AllowAdHocSubscriptions $true**</span></span>

<span data-ttu-id="e3928-119">Mer information finns i självbetjänings [registrering](/azure/active-directory/users-groups-roles/directory-self-service-signup).</span><span class="sxs-lookup"><span data-stu-id="e3928-119">For more information, read [Self-service sign up](/azure/active-directory/users-groups-roles/directory-self-service-signup).</span></span>

## <a name="you-forgot-your-password"></a><span data-ttu-id="e3928-120">Du har glömt ditt lösen ord</span><span class="sxs-lookup"><span data-stu-id="e3928-120">You forgot your password</span></span>

<span data-ttu-id="e3928-121">Om du har glömt ditt lösen ord väljer du länken **kan inte komma åt ditt konto?** på inloggnings sidan.</span><span class="sxs-lookup"><span data-stu-id="e3928-121">If you have forgotten your password, select the **Can't access your account?** link on the sign-in page.</span></span> <span data-ttu-id="e3928-122">Med det här alternativet kan du återställa ditt lösen ord eller be den globala administratören att tilldela nya autentiseringsuppgifter.</span><span class="sxs-lookup"><span data-stu-id="e3928-122">This option lets you reset your password or ask your Global admin to assign you new credentials.</span></span>

## <a name="on-the-tell-us-about-your-company-screen-you-receive-a-something-went-wrong-error"></a><span data-ttu-id="e3928-123">På skärmen "berätta för oss om ditt företag" visas fel meddelandet "något gick fel"</span><span class="sxs-lookup"><span data-stu-id="e3928-123">On the “Tell us about your company” screen, you receive a “Something went wrong” error</span></span>

<span data-ttu-id="e3928-124">Det här fel meddelandet visas vanligt vis om du oavsiktligt använder specialtecken, mellanslag eller landskod i företagets telefonnummer.</span><span class="sxs-lookup"><span data-stu-id="e3928-124">This error message usually shows up if you inadvertently use special characters, spaces, or country code in your company phone number.</span></span> <span data-ttu-id="e3928-125">Värdet som anges i fältet telefonnummer får bara innehålla högst 10 tecken.</span><span class="sxs-lookup"><span data-stu-id="e3928-125">The value entered in the Phone Number field can only contain a maximum of 10 characters.</span></span>


### <a name="your-credit-card-purchase-is-receiving-an-error-message-stating-that-your-order-was-declined-please-verify-your-information"></a><span data-ttu-id="e3928-126">Kredit korts köpet får ett fel meddelande om att "din beställning har avböjts.</span><span class="sxs-lookup"><span data-stu-id="e3928-126">Your credit card purchase is receiving an error message stating that “Your order was declined.</span></span> <span data-ttu-id="e3928-127">Verifiera din information.</span><span class="sxs-lookup"><span data-stu-id="e3928-127">Please verify your information”</span></span>


<span data-ttu-id="e3928-128">Använd alltid adressen som motsvarar ditt kredit kort i stället för din juridiska person.</span><span class="sxs-lookup"><span data-stu-id="e3928-128">Always use the address corresponding to your credit card rather than your legal entity.</span></span> <span data-ttu-id="e3928-129">Kontrol lera också att post numret är korrekt och motsvarar adressen som du använder.</span><span class="sxs-lookup"><span data-stu-id="e3928-129">Also, make sure the zip code is correct and corresponds to the address you use.</span></span>

## <a name="you-want-to-switch-from-offline-payment-to-online-payment-method"></a><span data-ttu-id="e3928-130">Du vill växla från offline-betalning till betalnings metod online</span><span class="sxs-lookup"><span data-stu-id="e3928-130">You want to switch from offline payment to online payment method</span></span> 

<span data-ttu-id="e3928-131">Du måste avbryta den ursprungliga ordern och köpa igen med hjälp av den prioriterade betalnings metoden.</span><span class="sxs-lookup"><span data-stu-id="e3928-131">You will need to cancel the original order and repurchase using the preferred payment method.</span></span>

<span data-ttu-id="e3928-132">Så här avbryter du en order:</span><span class="sxs-lookup"><span data-stu-id="e3928-132">To cancel an order:</span></span>

1. <span data-ttu-id="e3928-133">Fliken Välj **medlemskaps erbjudanden** på instrument panelen.</span><span class="sxs-lookup"><span data-stu-id="e3928-133">Select **Membership Offers** tab in the Dashboard.</span></span>

2. <span data-ttu-id="e3928-134">Välj **Avbryt order**</span><span class="sxs-lookup"><span data-stu-id="e3928-134">Select **Cancel order**</span></span>

3. <span data-ttu-id="e3928-135">Ett bekräftelse fönster visas och du måste bekräfta innan du kan avbryta den inledande ordningen.</span><span class="sxs-lookup"><span data-stu-id="e3928-135">A confirmation window will appear and you must confirm in order to cancel the initial order.</span></span>

## <a name="next-steps"></a><span data-ttu-id="e3928-136">Nästa steg</span><span class="sxs-lookup"><span data-stu-id="e3928-136">Next steps</span></span>

- [<span data-ttu-id="e3928-137">Hantera ditt Partnercenter-konto</span><span class="sxs-lookup"><span data-stu-id="e3928-137">Manage your Partner Center account</span></span>](partner-center-account-setup.md)
- [<span data-ttu-id="e3928-138">Läsa din faktura-och rekognoseringar-fil</span><span class="sxs-lookup"><span data-stu-id="e3928-138">How to read your bill and recon file</span></span>](read-your-bill.md)
