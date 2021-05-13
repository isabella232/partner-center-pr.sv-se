---
title: Felsöka problem med att konfigurera ditt PartnerCenter-konto eller MPN-förnyelse
ms.topic: how-to
ms.date: 08/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Felsöka problem när du försöker registrera i Partnercenter. Svar på problem med betalningsmetoder, att glömma lösenord med mera.
author: ArpithaKanuganti
ms.author: v-arkanu
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: a5e8a292ad8593dc0b94179d5f0ee418344ef9af
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 05/13/2021
ms.locfileid: "109854697"
---
# <a name="troubleshoot-account-setup-or-mpn-renewal-issues"></a><span data-ttu-id="f1d33-104">Felsöka problem med kontokonfiguration eller MPN-förnyelse</span><span class="sxs-lookup"><span data-stu-id="f1d33-104">Troubleshoot account setup or MPN renewal issues</span></span>

<span data-ttu-id="f1d33-105">**Lämpliga roller:** Global | MPN-partneradministratör</span><span class="sxs-lookup"><span data-stu-id="f1d33-105">**Appropriate roles**: Global admin | MPN partner admin</span></span>
 
<span data-ttu-id="f1d33-106">Här är några förslag på felsökning av vanliga problem som uppstår när du ställer in ditt Partnercenter-konto.</span><span class="sxs-lookup"><span data-stu-id="f1d33-106">Here are some suggestions for troubleshooting common issues that arise when setting up your Partner Center account.</span></span>

## <a name="what-happens-if-you-are-migrating-from-partner-membership-center-and-you-cant-edit-any-company-information-fields"></a><span data-ttu-id="f1d33-107">Vad händer om du migrerar från Partner Membership Center och du inte kan redigera fält för företagsinformation</span><span class="sxs-lookup"><span data-stu-id="f1d33-107">What happens if you are migrating from Partner Membership Center and you can't edit any company information fields</span></span>

<span data-ttu-id="f1d33-108">Om ditt företag redan finns i Partnercenter (till exempel ett CSP-konto) visas en skrivskyddad skärm.</span><span class="sxs-lookup"><span data-stu-id="f1d33-108">In cases where your company already has a presence in Partner Center (for example, a CSP account) – you will be shown a read-only screen.</span></span> <span data-ttu-id="f1d33-109">Den här skärmen visar all information om ditt företag som det finns i Partnercenter.</span><span class="sxs-lookup"><span data-stu-id="f1d33-109">This screen will display all the information about your company as it exists in Partner Center.</span></span>

<span data-ttu-id="f1d33-110">Du kan inte ändra informationen på den här skärmen.</span><span class="sxs-lookup"><span data-stu-id="f1d33-110">You can't change the details on this screen.</span></span> <span data-ttu-id="f1d33-111">Detta är enligt design och inte ett fel.</span><span class="sxs-lookup"><span data-stu-id="f1d33-111">This is by design and not an error.</span></span>

<span data-ttu-id="f1d33-112">Välj **Acceptera** och **Fortsätt för att** fortsätta.</span><span class="sxs-lookup"><span data-stu-id="f1d33-112">Select **Accept** and **Continue** to proceed.</span></span>


### <a name="if-the-it-department-has-turned-off-sign-up-for-partner-center"></a><span data-ttu-id="f1d33-113">Om IT-avdelningen har inaktiverat **Registrera dig för Partnercenter**</span><span class="sxs-lookup"><span data-stu-id="f1d33-113">If the IT department has turned off **Sign up for Partner Center**</span></span>

<span data-ttu-id="f1d33-114">Du ser det här meddelandet eftersom virala användare är inaktiverade eller på grund av att viral registrering har inaktiverats i Azure AD-klientorganisationen.</span><span class="sxs-lookup"><span data-stu-id="f1d33-114">You see this message because viral users are disabled, or because Viral Sign-up is disabled on the Azure AD tenant.</span></span> <span data-ttu-id="f1d33-115">Den globala administratören för ditt Azure AD-konto kan aktivera nödvändiga funktioner genom att köra följande PowerShell-kommando:</span><span class="sxs-lookup"><span data-stu-id="f1d33-115">The Global admin for your Azure AD account can enable required features by running the following PowerShell command:</span></span>

<span data-ttu-id="f1d33-116">**Set-MsolCompanySettings -AllowEmailVerifiedUsers $true -AllowAdHocSubscriptions $true**</span><span class="sxs-lookup"><span data-stu-id="f1d33-116">**Set-MsolCompanySettings -AllowEmailVerifiedUsers $true -AllowAdHocSubscriptions $true**</span></span>

<span data-ttu-id="f1d33-117">Mer information finns i [Registrera dig för självbetjäning.](/azure/active-directory/users-groups-roles/directory-self-service-signup)</span><span class="sxs-lookup"><span data-stu-id="f1d33-117">For more information, read [Self-service sign up](/azure/active-directory/users-groups-roles/directory-self-service-signup).</span></span>

## <a name="you-forgot-your-password"></a><span data-ttu-id="f1d33-118">Du har glömt ditt lösenord</span><span class="sxs-lookup"><span data-stu-id="f1d33-118">You forgot your password</span></span>

<span data-ttu-id="f1d33-119">Om du har glömt lösenordet väljer du **länken Kan du inte komma åt ditt konto?** på inloggningssidan.</span><span class="sxs-lookup"><span data-stu-id="f1d33-119">If you have forgotten your password, select the **Can't access your account?** link on the sign-in page.</span></span> <span data-ttu-id="f1d33-120">Med det här alternativet kan du återställa lösenordet eller be din globala administratör att tilldela dig nya autentiseringsuppgifter.</span><span class="sxs-lookup"><span data-stu-id="f1d33-120">This option lets you reset your password or ask your Global admin to assign you new credentials.</span></span>

## <a name="on-the-tell-us-about-your-company-screen-you-receive-a-something-went-wrong-error"></a><span data-ttu-id="f1d33-121">På skärmen "Berätta om ditt företag" visas felmeddelandet "Något gick fel"</span><span class="sxs-lookup"><span data-stu-id="f1d33-121">On the “Tell us about your company” screen, you receive a “Something went wrong” error</span></span>

<span data-ttu-id="f1d33-122">Det här felmeddelandet visas vanligtvis om du oavsiktligt använder specialtecken, blanksteg eller landskod i företagets telefonnummer.</span><span class="sxs-lookup"><span data-stu-id="f1d33-122">This error message usually shows up if you inadvertently use special characters, spaces, or country code in your company phone number.</span></span> <span data-ttu-id="f1d33-123">Värdet som anges i fältet Telefonnummer får bara innehålla högst 10 tecken.</span><span class="sxs-lookup"><span data-stu-id="f1d33-123">The value entered in the Phone Number field can only contain a maximum of 10 characters.</span></span>


### <a name="your-credit-card-purchase-is-receiving-an-error-message-stating-that-your-order-was-declined-please-verify-your-information"></a><span data-ttu-id="f1d33-124">Ditt kreditkortsköp får ett felmeddelande om att "Din beställning nekades.</span><span class="sxs-lookup"><span data-stu-id="f1d33-124">Your credit card purchase is receiving an error message stating that “Your order was declined.</span></span> <span data-ttu-id="f1d33-125">Verifiera din information"</span><span class="sxs-lookup"><span data-stu-id="f1d33-125">Please verify your information”</span></span>


<span data-ttu-id="f1d33-126">Använd alltid den adress som motsvarar ditt kreditkort i stället för din juridiska enhet.</span><span class="sxs-lookup"><span data-stu-id="f1d33-126">Always use the address corresponding to your credit card rather than your legal entity.</span></span> <span data-ttu-id="f1d33-127">Kontrollera också att postnumret är korrekt och motsvarar den adress som du använder.</span><span class="sxs-lookup"><span data-stu-id="f1d33-127">Also, make sure the zip code is correct and corresponds to the address you use.</span></span>

## <a name="you-want-to-switch-from-offline-payment-to-online-payment-method"></a><span data-ttu-id="f1d33-128">Du vill byta från offlinebetalning till onlinebetalningsmetod</span><span class="sxs-lookup"><span data-stu-id="f1d33-128">You want to switch from offline payment to online payment method</span></span> 

<span data-ttu-id="f1d33-129">Du måste avbryta den ursprungliga beställningen och göra ett återköp med den önskade betalningsmetoden.</span><span class="sxs-lookup"><span data-stu-id="f1d33-129">You will need to cancel the original order and repurchase using the preferred payment method.</span></span>

<span data-ttu-id="f1d33-130">Så här annullerar du en beställning:</span><span class="sxs-lookup"><span data-stu-id="f1d33-130">To cancel an order:</span></span>

1. <span data-ttu-id="f1d33-131">Välj **fliken Medlemskapserbjudanden** på instrumentpanelen.</span><span class="sxs-lookup"><span data-stu-id="f1d33-131">Select **Membership Offers** tab in the Dashboard.</span></span>

2. <span data-ttu-id="f1d33-132">Välj **Avbryt beställning**</span><span class="sxs-lookup"><span data-stu-id="f1d33-132">Select **Cancel order**</span></span>

3. <span data-ttu-id="f1d33-133">Ett bekräftelsefönster visas och du måste bekräfta för att kunna avbryta den första ordern.</span><span class="sxs-lookup"><span data-stu-id="f1d33-133">A confirmation window will appear and you must confirm in order to cancel the initial order.</span></span>

## <a name="next-steps"></a><span data-ttu-id="f1d33-134">Nästa steg</span><span class="sxs-lookup"><span data-stu-id="f1d33-134">Next steps</span></span>

- [<span data-ttu-id="f1d33-135">Hantera ditt Partnercenter-konto</span><span class="sxs-lookup"><span data-stu-id="f1d33-135">Manage your Partner Center account</span></span>](partner-center-account-setup.md)
- [<span data-ttu-id="f1d33-136">Läsa fakturan och rekognoseringsfilen</span><span class="sxs-lookup"><span data-stu-id="f1d33-136">How to read your bill and recon file</span></span>](read-your-bill.md)
