---
title: Felsöka problem med att konfigurera ditt Partnercenter-konto eller MPN-förnyelse
ms.topic: how-to
ms.date: 08/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Felsöka problem när du försöker registrera i Partnercenter. Svar på problem med betalningsmetoder, att glömma lösenord och mycket annat.
author: ArpithaKanuganti
ms.author: v-arkanu
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: f34adc57e668caecb69af37afc72b5153f667335
ms.sourcegitcommit: 08a175c06ff4c6a2b12713f081adfa489e16e7a1
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 05/10/2021
ms.locfileid: "109686270"
---
# <a name="troubleshoot-account-setup-or-mpn-renewal-issues"></a><span data-ttu-id="40f70-104">Felsöka problem med kontokonfiguration eller MPN-förnyelse</span><span class="sxs-lookup"><span data-stu-id="40f70-104">Troubleshoot account setup or MPN renewal issues</span></span>


<span data-ttu-id="40f70-105">**Lämpliga roller**</span><span class="sxs-lookup"><span data-stu-id="40f70-105">**Appropriate roles**</span></span>

- <span data-ttu-id="40f70-106">Global administratör</span><span class="sxs-lookup"><span data-stu-id="40f70-106">Global admin</span></span>
- <span data-ttu-id="40f70-107">MPN-partneradministratör</span><span class="sxs-lookup"><span data-stu-id="40f70-107">MPN partner admin</span></span>
 
<span data-ttu-id="40f70-108">Här är några förslag på felsökning av vanliga problem som uppstår när du ställer in ditt Partnercenter-konto.</span><span class="sxs-lookup"><span data-stu-id="40f70-108">Here are some suggestions for troubleshooting common issues that arise when setting up your Partner Center account.</span></span>

## <a name="what-happens-if-you-are-migrating-from-partner-membership-center-and-you-cant-edit-any-company-information-fields"></a><span data-ttu-id="40f70-109">Vad händer om du migrerar från Partner Membership Center och du inte kan redigera fält för företagsinformation</span><span class="sxs-lookup"><span data-stu-id="40f70-109">What happens if you are migrating from Partner Membership Center and you can't edit any company information fields</span></span>

<span data-ttu-id="40f70-110">Om ditt företag redan finns i Partnercenter (till exempel ett CSP-konto) visas en skrivskyddad skärm.</span><span class="sxs-lookup"><span data-stu-id="40f70-110">In cases where your company already has a presence in Partner Center (for example, a CSP account) – you will be shown a read-only screen.</span></span> <span data-ttu-id="40f70-111">På den här skärmen visas all information om ditt företag när det finns i Partnercenter.</span><span class="sxs-lookup"><span data-stu-id="40f70-111">This screen will display all the information about your company as it exists in Partner Center.</span></span>

<span data-ttu-id="40f70-112">Du kan inte ändra informationen på den här skärmen.</span><span class="sxs-lookup"><span data-stu-id="40f70-112">You can't change the details on this screen.</span></span> <span data-ttu-id="40f70-113">Detta är design och inte ett fel.</span><span class="sxs-lookup"><span data-stu-id="40f70-113">This is by design and not an error.</span></span>

<span data-ttu-id="40f70-114">Välj **Acceptera** och **Fortsätt för att** fortsätta.</span><span class="sxs-lookup"><span data-stu-id="40f70-114">Select **Accept** and **Continue** to proceed.</span></span>


### <a name="if-the-it-department-has-turned-off-sign-up-for-partner-center"></a><span data-ttu-id="40f70-115">Om IT-avdelningen har inaktiverat **Registrering för Partnercenter**</span><span class="sxs-lookup"><span data-stu-id="40f70-115">If the IT department has turned off **Sign up for Partner Center**</span></span>

<span data-ttu-id="40f70-116">Du ser det här meddelandet eftersom virala användare är inaktiverade eller eftersom viral registrering är inaktiverat i Azure AD-klientorganisationen.</span><span class="sxs-lookup"><span data-stu-id="40f70-116">You see this message because viral users are disabled, or because Viral Sign-up is disabled on the Azure AD tenant.</span></span> <span data-ttu-id="40f70-117">Den globala administratören för ditt Azure AD-konto kan aktivera nödvändiga funktioner genom att köra följande PowerShell-kommando:</span><span class="sxs-lookup"><span data-stu-id="40f70-117">The Global admin for your Azure AD account can enable required features by running the following PowerShell command:</span></span>

<span data-ttu-id="40f70-118">**Set-MsolCompanySettings -AllowEmailVerifiedUsers $true -AllowAdHocSubscriptions $true**</span><span class="sxs-lookup"><span data-stu-id="40f70-118">**Set-MsolCompanySettings -AllowEmailVerifiedUsers $true -AllowAdHocSubscriptions $true**</span></span>

<span data-ttu-id="40f70-119">Mer information finns i [Registrera dig för självbetjäning.](/azure/active-directory/users-groups-roles/directory-self-service-signup)</span><span class="sxs-lookup"><span data-stu-id="40f70-119">For more information, read [Self-service sign up](/azure/active-directory/users-groups-roles/directory-self-service-signup).</span></span>

## <a name="you-forgot-your-password"></a><span data-ttu-id="40f70-120">Du har glömt ditt lösenord</span><span class="sxs-lookup"><span data-stu-id="40f70-120">You forgot your password</span></span>

<span data-ttu-id="40f70-121">Om du har glömt ditt lösenord väljer du länken Kan du inte komma åt ditt **konto?** på inloggningssidan.</span><span class="sxs-lookup"><span data-stu-id="40f70-121">If you have forgotten your password, select the **Can't access your account?** link on the sign-in page.</span></span> <span data-ttu-id="40f70-122">Med det här alternativet kan du återställa lösenordet eller be din globala administratör att tilldela dig nya autentiseringsuppgifter.</span><span class="sxs-lookup"><span data-stu-id="40f70-122">This option lets you reset your password or ask your Global admin to assign you new credentials.</span></span>

## <a name="on-the-tell-us-about-your-company-screen-you-receive-a-something-went-wrong-error"></a><span data-ttu-id="40f70-123">På skärmen "Berätta om ditt företag" visas felet "Något gick fel"</span><span class="sxs-lookup"><span data-stu-id="40f70-123">On the “Tell us about your company” screen, you receive a “Something went wrong” error</span></span>

<span data-ttu-id="40f70-124">Det här felmeddelandet visas vanligtvis om du oavsiktligt använder specialtecken, blanksteg eller landskod i företagets telefonnummer.</span><span class="sxs-lookup"><span data-stu-id="40f70-124">This error message usually shows up if you inadvertently use special characters, spaces, or country code in your company phone number.</span></span> <span data-ttu-id="40f70-125">Värdet som anges i fältet Telefonnummer får bara innehålla högst 10 tecken.</span><span class="sxs-lookup"><span data-stu-id="40f70-125">The value entered in the Phone Number field can only contain a maximum of 10 characters.</span></span>


### <a name="your-credit-card-purchase-is-receiving-an-error-message-stating-that-your-order-was-declined-please-verify-your-information"></a><span data-ttu-id="40f70-126">Ditt kreditkortsköp får ett felmeddelande om att din beställning nekades.</span><span class="sxs-lookup"><span data-stu-id="40f70-126">Your credit card purchase is receiving an error message stating that “Your order was declined.</span></span> <span data-ttu-id="40f70-127">Verifiera din information"</span><span class="sxs-lookup"><span data-stu-id="40f70-127">Please verify your information”</span></span>


<span data-ttu-id="40f70-128">Använd alltid den adress som motsvarar ditt kreditkort i stället för din juridiska person.</span><span class="sxs-lookup"><span data-stu-id="40f70-128">Always use the address corresponding to your credit card rather than your legal entity.</span></span> <span data-ttu-id="40f70-129">Kontrollera också att postnumret är korrekt och motsvarar den adress som du använder.</span><span class="sxs-lookup"><span data-stu-id="40f70-129">Also, make sure the zip code is correct and corresponds to the address you use.</span></span>

## <a name="you-want-to-switch-from-offline-payment-to-online-payment-method"></a><span data-ttu-id="40f70-130">Du vill växla från offlinebetalning till onlinebetalningsmetod</span><span class="sxs-lookup"><span data-stu-id="40f70-130">You want to switch from offline payment to online payment method</span></span> 

<span data-ttu-id="40f70-131">Du måste avbryta den ursprungliga beställningen och göra ett återköp med den önskade betalningsmetoden.</span><span class="sxs-lookup"><span data-stu-id="40f70-131">You will need to cancel the original order and repurchase using the preferred payment method.</span></span>

<span data-ttu-id="40f70-132">Så här avbryter du en beställning:</span><span class="sxs-lookup"><span data-stu-id="40f70-132">To cancel an order:</span></span>

1. <span data-ttu-id="40f70-133">Välj **fliken Medlemskapserbjudanden** på instrumentpanelen.</span><span class="sxs-lookup"><span data-stu-id="40f70-133">Select **Membership Offers** tab in the Dashboard.</span></span>

2. <span data-ttu-id="40f70-134">Välj **Avbryt beställning**</span><span class="sxs-lookup"><span data-stu-id="40f70-134">Select **Cancel order**</span></span>

3. <span data-ttu-id="40f70-135">Ett bekräftelsefönster visas och du måste bekräfta för att kunna avbryta den första beställningen.</span><span class="sxs-lookup"><span data-stu-id="40f70-135">A confirmation window will appear and you must confirm in order to cancel the initial order.</span></span>

## <a name="next-steps"></a><span data-ttu-id="40f70-136">Nästa steg</span><span class="sxs-lookup"><span data-stu-id="40f70-136">Next steps</span></span>

- [<span data-ttu-id="40f70-137">Hantera ditt Partnercenter-konto</span><span class="sxs-lookup"><span data-stu-id="40f70-137">Manage your Partner Center account</span></span>](partner-center-account-setup.md)
- [<span data-ttu-id="40f70-138">Läsa fakturan och rekognoseringsfilen</span><span class="sxs-lookup"><span data-stu-id="40f70-138">How to read your bill and recon file</span></span>](read-your-bill.md)
