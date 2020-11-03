---
title: Växla direkt fakturerings partner till indirekt åter försäljare
ms.topic: how-to
ms.date: 06/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Lär dig hur en CSP-programpartner kan använda Partner Center för att övergå från direkt fakturerings partner till indirekt åter försäljare.
author: aarzh-AaronZhang
ms.author: v-aarzh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: e3cd791f5f9f781980d73c79f0ec18627585372a
ms.sourcegitcommit: b4771fd0781d95551e65baa481a572291c729d7d
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 10/28/2020
ms.locfileid: "92795873"
---
# <a name="transition-from-cloud-solution-provider-csp-direct-bill-partner-to-csp-indirect-reseller"></a><span data-ttu-id="36cc8-103">Övergå från en CSP-partner med direktfakturering till en indirekt CSP-återförsäljare</span><span class="sxs-lookup"><span data-stu-id="36cc8-103">Transition from Cloud Solution Provider (CSP) direct bill partner to CSP indirect reseller</span></span>

<span data-ttu-id="36cc8-104">**Gäller:**</span><span class="sxs-lookup"><span data-stu-id="36cc8-104">**Applies to:**</span></span>
- <span data-ttu-id="36cc8-105">Partnercenter</span><span class="sxs-lookup"><span data-stu-id="36cc8-105">Partner Center</span></span>

<span data-ttu-id="36cc8-106">**Lämpliga roller**</span><span class="sxs-lookup"><span data-stu-id="36cc8-106">**Appropriate roles**</span></span>

- <span data-ttu-id="36cc8-107">Alla leverantörer av KRYPTOGRAFIPROVIDERs direkt fakturering</span><span class="sxs-lookup"><span data-stu-id="36cc8-107">All CSP direct bill partners</span></span>

>[!Note]
><span data-ttu-id="36cc8-108">Den här artikeln är avsedd för direkta fakturerings partner som har valt att övergå till indirekta åter försäljare.</span><span class="sxs-lookup"><span data-stu-id="36cc8-108">This article is intended for direct bill partners who have decided to transition to indirect resellers.</span></span> <span data-ttu-id="36cc8-109">Men även om du inte har gjort ett explicit beslut än att registrera sig som en indirekt åter försäljare, kommer direkta fakturerings partner som inte uppfyller de nya [kraven](direct-partner-new-requirements.md) för fakturerings programmet för CSP: n att informeras av Microsoft när deras [direkta fakturerings kapacitet är begränsad](restricted-direct-bill-capabilities.md).</span><span class="sxs-lookup"><span data-stu-id="36cc8-109">However, even if you have not made an explicit decision yet to enroll as an indirect reseller, direct bill partners who do not meet the new [requirements](direct-partner-new-requirements.md) for the CSP direct bill partner program will be informed by Microsoft when their [direct bill capabilities will be restricted](restricted-direct-bill-capabilities.md).</span></span>
<br><span data-ttu-id="36cc8-110">Från och med januari 2021 kommer ett nytt intäkts krav att läggas till.</span><span class="sxs-lookup"><span data-stu-id="36cc8-110">As of January 2021, a new revenue requirement will be added.</span></span> <span data-ttu-id="36cc8-111">Partner som har registrerats som en direkt fakturerings partner måste ha överfört minst USD $ över 300 000 i moln lösnings leverantörens program intäkt till en global partner global konto nivå under de föregående 12 månaderna.</span><span class="sxs-lookup"><span data-stu-id="36cc8-111">Partners enrolled as a direct bill partner will need to have transacted at least USD$300K in Cloud Solution Provider program revenue at a Partner Global Account level over the previous 12 months.</span></span>

<span data-ttu-id="36cc8-112">Du kommer att kunna registrera i det indirekta åter försäljar programmet med din befintliga direkt fakturerings klient.</span><span class="sxs-lookup"><span data-stu-id="36cc8-112">You will be able to enroll in the indirect reseller program using your existing direct bill tenant.</span></span>

## <a name="get-started"></a><span data-ttu-id="36cc8-113">Kom igång</span><span class="sxs-lookup"><span data-stu-id="36cc8-113">Get started</span></span>

1. <span data-ttu-id="36cc8-114">Se till att din partner profil i Partner Center och MPN-ID är aktuella.</span><span class="sxs-lookup"><span data-stu-id="36cc8-114">Make sure your partner profile in Partner Center and MPN ID are current.</span></span>

2. <span data-ttu-id="36cc8-115">Logga in på Partner Center som global administratör för den direkta fakturerings klient som du översätter till indirekt åter försäljare.</span><span class="sxs-lookup"><span data-stu-id="36cc8-115">Sign in to Partner Center as the global admin for the direct bill tenant you are transitioning to indirect reseller.</span></span>

   :::image type="content" source="images/direct/direct1.png" alt-text="Översikt":::

3. <span data-ttu-id="36cc8-117">Granska din partner information i registrerings formuläret.</span><span class="sxs-lookup"><span data-stu-id="36cc8-117">Review your partner details on the enrollment form.</span></span>

   :::image type="content" source="images/direct/direct2a.png" alt-text="Registrera dig nu":::

4. <span data-ttu-id="36cc8-119">Välj Registrera nu.</span><span class="sxs-lookup"><span data-stu-id="36cc8-119">Select Enroll now.</span></span> <span data-ttu-id="36cc8-120">Den indirekta åter försäljaren kommer att använda samma AAD-klient som du använder för din direkta verksamhet.</span><span class="sxs-lookup"><span data-stu-id="36cc8-120">Your indirect reseller business will use the same AAD tenant you use for your direct business.</span></span>

    > [!NOTE]
    > <span data-ttu-id="36cc8-121">Inlednings vis är den här nya över gångs funktionen tillgänglig för partner med datum från september till december.</span><span class="sxs-lookup"><span data-stu-id="36cc8-121">Initially, this new transition capability will be available for partners with September to December anniversary dates.</span></span> <span data-ttu-id="36cc8-122">Om du inte har ett jubileums datum mellan september och december visas inte funktionen för tillfället.</span><span class="sxs-lookup"><span data-stu-id="36cc8-122">If you don"t have an anniversary date between September and December, you won't see the capability at this time.</span></span> <span data-ttu-id="36cc8-123">Partner med jubileums datum i december 2018 kommer att meddelas senare när funktionen har Aktiver ATS för partner.</span><span class="sxs-lookup"><span data-stu-id="36cc8-123">Partners with anniversary dates after December 2018 will be notified later once the feature is enabled for the partners.</span></span>

5. <span data-ttu-id="36cc8-124">När registreringen är godkänd loggar du in på Partner Center igen.</span><span class="sxs-lookup"><span data-stu-id="36cc8-124">When your enrollment is approved, sign in to Partner Center again.</span></span>

    > [!NOTE]
    > <span data-ttu-id="36cc8-125">Även om godkännandet ofta är omedelbart kan det ta upp till fem arbets dagar.</span><span class="sxs-lookup"><span data-stu-id="36cc8-125">While approval is usually immediate, it can take up to five business days.</span></span> <span data-ttu-id="36cc8-126">När den har godkänts får du ett meddelande till den e-postadress som du har angett under primär kontakt i registrerings formuläret.</span><span class="sxs-lookup"><span data-stu-id="36cc8-126">Once approved, you will receive a notification to the email address you have specified under primary contact in the enrollment form.</span></span> <span data-ttu-id="36cc8-127">Du kan också kontrol lera registrerings statusen under **Inställningar**  >  **partner inställningar**  >  **partner profil** > program information.</span><span class="sxs-lookup"><span data-stu-id="36cc8-127">You can also check your enrollment status under **Settings** > **Partner Settings** > **Partner Profile** > Program info.</span></span>

6. <span data-ttu-id="36cc8-128">På sidan **Översikt** visas avtalet om indirekt åter försäljare.</span><span class="sxs-lookup"><span data-stu-id="36cc8-128">On your **Overview** page, you will see the indirect reseller agreement.</span></span> <span data-ttu-id="36cc8-129">Välj **Godkänn och fortsätt** .</span><span class="sxs-lookup"><span data-stu-id="36cc8-129">Select **Accept and continue** .</span></span> <span data-ttu-id="36cc8-130">Den här åtgärden aktiverar funktioner för indirekt åter försäljare.</span><span class="sxs-lookup"><span data-stu-id="36cc8-130">This action enables the indirect reseller capabilities.</span></span>

<span data-ttu-id="36cc8-131">När du har godkänt avtalet för den indirekta åter försäljaren ser du att din partner profil identifierar dig som **både** en direkt fakturerings-och indirekt åter försäljare.</span><span class="sxs-lookup"><span data-stu-id="36cc8-131">When you have accepted the indirect reseller agreement, notice that your Partner profile identifies you as **both** a direct bill and indirect reseller.</span></span>

:::image type="content" source="images/direct/direct3.png" alt-text="Indirekt åter försäljar avtal":::

> [!IMPORTANT]
> <span data-ttu-id="36cc8-133">När du har registrerat dig som en indirekt åter försäljare med den nya funktionen finns det inget alternativ för att återställa till en direkt fakturerings klient.</span><span class="sxs-lookup"><span data-stu-id="36cc8-133">Once you enroll as an indirect reseller using the new capability, there is no option to roll back to a direct bill- only tenant.</span></span> <span data-ttu-id="36cc8-134">Se till att du utvärderar dina affärs behov fullständigt innan du registrerar dig som en indirekt åter försäljare.</span><span class="sxs-lookup"><span data-stu-id="36cc8-134">Please make sure that you fully evaluate your business needs before enrolling as an indirect reseller.</span></span>

## <a name="while-you-transition-from-direct-to-indirect-reseller"></a><span data-ttu-id="36cc8-135">När du övergår från direkt till indirekt åter försäljare</span><span class="sxs-lookup"><span data-stu-id="36cc8-135">While you transition from direct to indirect reseller</span></span>

<span data-ttu-id="36cc8-136">Under den här fasen kommer du fortsätta att hantera dina direkta kunders prenumerations behov, inklusive fakturerings processen.</span><span class="sxs-lookup"><span data-stu-id="36cc8-136">During this phase, you will continue to manage your direct customers' subscription needs including the billing process.</span></span> <span data-ttu-id="36cc8-137">Du kan också börja acceptera kunder från den indirekta leverantören och arbeta som en indirekt åter försäljare.</span><span class="sxs-lookup"><span data-stu-id="36cc8-137">You can also begin accepting customers from your Indirect provider and operating as an indirect reseller.</span></span>

:::image type="content" source="images/direct/direct4.png" alt-text="Du är både en direkt fakturerings-och indirekt åter försäljare":::

## <a name="find-an-indirect-provider"></a><span data-ttu-id="36cc8-139">Hitta en indirekt leverantör</span><span class="sxs-lookup"><span data-stu-id="36cc8-139">Find an indirect provider</span></span>

<span data-ttu-id="36cc8-140">Efter registreringen visas en länk till indirekta leverantörer i det vänstra navigerings fältet.</span><span class="sxs-lookup"><span data-stu-id="36cc8-140">After enrolling, a link to Indirect providers will appear in your left nav.</span></span> <span data-ttu-id="36cc8-141">Som en indirekt åter försäljare upprättar du en relation med en indirekt provider som sedan kan hantera fakturerings-, inköps produkter för dina kunder och stödja infrastruktur.</span><span class="sxs-lookup"><span data-stu-id="36cc8-141">As an indirect reseller you will establish a relationship with an indirect provider who then can handle your billing, purchase products for your customers, and support infrastructure.</span></span>

<span data-ttu-id="36cc8-142">Olika indirekta leverantörer erbjuder olika support och tjänster, så du bör utvärdera leverantörerna i ditt utrymme för att avgöra vilka som bäst motsvarar dina behov.</span><span class="sxs-lookup"><span data-stu-id="36cc8-142">Different indirect providers offer different support and services, so you should evaluate the providers in your area to determine which ones best meet your needs.</span></span> <span data-ttu-id="36cc8-143">I allmänhet kommer de flesta leverantörer att:</span><span class="sxs-lookup"><span data-stu-id="36cc8-143">Generally, most providers will:</span></span>

- <span data-ttu-id="36cc8-144">Ge dig teknisk utbildning och hjälp</span><span class="sxs-lookup"><span data-stu-id="36cc8-144">Provide you with technical training and assistance</span></span>
- <span data-ttu-id="36cc8-145">Hjälp att marknadsföra dina produkter och tjänster</span><span class="sxs-lookup"><span data-stu-id="36cc8-145">Help you market your products and services</span></span>
- <span data-ttu-id="36cc8-146">Hantera dina finansierings-och kredit villkor</span><span class="sxs-lookup"><span data-stu-id="36cc8-146">Manage your financing and credit terms</span></span>

<span data-ttu-id="36cc8-147">Sök i listan över officiella [Microsoft-indirekta leverantörer](https://partnercenter.microsoft.com/partner/find-a-provider).</span><span class="sxs-lookup"><span data-stu-id="36cc8-147">Search the list of official [Microsoft indirect providers](https://partnercenter.microsoft.com/partner/find-a-provider).</span></span>

<span data-ttu-id="36cc8-148">Läs mer, Läs  [partner med indirekta leverantörer](indirect-reseller-tasks-in-partner-center.md)</span><span class="sxs-lookup"><span data-stu-id="36cc8-148">Learn more, read  [Partner with indirect providers](indirect-reseller-tasks-in-partner-center.md)</span></span>

## <a name="accept-a-partnership-invitation-from-your-indirect-provider"></a><span data-ttu-id="36cc8-149">Acceptera en inbjudan från din indirekta leverantör</span><span class="sxs-lookup"><span data-stu-id="36cc8-149">Accept a partnership invitation from your indirect provider</span></span>

<span data-ttu-id="36cc8-150">När du hittar en indirekt Provider för partner med, upprätta ett partnerskap med den indirekta providern i Partner Center.</span><span class="sxs-lookup"><span data-stu-id="36cc8-150">When you find an indirect provider to partner with, establish a partnership with the indirect provider in Partner Center.</span></span>

<span data-ttu-id="36cc8-151">Den indirekta providern du väljer skickar dig via e-post till en länk för inbjudan till inbjudan som tar dig till deras inbjudan i Partner Center.</span><span class="sxs-lookup"><span data-stu-id="36cc8-151">The indirect provider you select will send you in email a partnership invitation link that will take you to their invitation in Partner Center.</span></span> <span data-ttu-id="36cc8-152">Se till att din globala administratör loggar in på Partner Center och följer Inbjudnings länken.</span><span class="sxs-lookup"><span data-stu-id="36cc8-152">Be sure your global admin signs in to Partner Center and follows the invitation link.</span></span> <span data-ttu-id="36cc8-153">När du godkänner inbjudan visas leverantörens namn i listan över den indirekta providern.</span><span class="sxs-lookup"><span data-stu-id="36cc8-153">When you accept the invitation, the provider's name will appear in your indirect provider list.</span></span>

## <a name="acquire-new-customers-as-indirect-reseller"></a><span data-ttu-id="36cc8-154">Skaffa nya kunder som indirekt åter försäljare</span><span class="sxs-lookup"><span data-stu-id="36cc8-154">Acquire new customers as indirect reseller</span></span>

<span data-ttu-id="36cc8-155">Både du och din indirekta leverantör måste ha åter försäljarnas relationer med kunderna.</span><span class="sxs-lookup"><span data-stu-id="36cc8-155">Both you and your indirect provider need to have reseller relationships with customers.</span></span> <span data-ttu-id="36cc8-156">Med dessa relationer för åter försäljare kan du hantera en kunds prenumerationer och tjänster för deras räkning.</span><span class="sxs-lookup"><span data-stu-id="36cc8-156">These reseller relationships enable you to manage a customer's subscriptions and services on their behalf.</span></span> <span data-ttu-id="36cc8-157">Om du vill skaffa en ny kund som har en befintlig Azure AD-klient kan du bjuda in kunden att upprätta en åter försäljares relation med både du och din leverantör på samma tid.</span><span class="sxs-lookup"><span data-stu-id="36cc8-157">To acquire a new customer who has an existing Azure AD tenant, you can invite the customer to establish a reseller relationship with both you and your provider at the same time.</span></span>

<span data-ttu-id="36cc8-158">Så här skapar du en indirekt åter försäljare-inbjudan:</span><span class="sxs-lookup"><span data-stu-id="36cc8-158">To create an indirect reseller invitation:</span></span>

1. <span data-ttu-id="36cc8-159">Välj **indirekta leverantörer** från din partner Center vänstra navigerings fältet.</span><span class="sxs-lookup"><span data-stu-id="36cc8-159">Select **Indirect providers** from your Partner Center left nav.</span></span>

2. <span data-ttu-id="36cc8-160">Välj **Bjud in nya kunder** för att bjuda in en kund att upprätta en åter försäljares relation med både du och den indirekta providern på samma tid.</span><span class="sxs-lookup"><span data-stu-id="36cc8-160">Select **Invite new customers** to invite a customer to establish a reseller relationship with both you and the indirect provider at the same time.</span></span> <span data-ttu-id="36cc8-161">Leverantören måste ha en åter försäljar relation med din kund, så att de kan skicka beställningar på din kunds räkning när kunden vill köpa nya prenumerationer eller lägga till nya licenser i befintliga prenumerationer.</span><span class="sxs-lookup"><span data-stu-id="36cc8-161">The provider needs to have a reseller relationship with your customer, so they can submit orders on your customer's behalf when the customer wants to buy new subscriptions or add new licenses to existing subscriptions.</span></span>

3. <span data-ttu-id="36cc8-162">På nästa sida granskar du utkastet till e-postmeddelandet.</span><span class="sxs-lookup"><span data-stu-id="36cc8-162">On the next page, review the draft email message.</span></span> <span data-ttu-id="36cc8-163">Du kan öppna utkast meddelandet i ett e-postmeddelande, eller så kan du kopiera meddelandet till Urklipp och klistra in det i ett e-postmeddelande.</span><span class="sxs-lookup"><span data-stu-id="36cc8-163">You can open the draft message in email, or you can copy the message to your clipboard and paste it into an email.</span></span>

4. <span data-ttu-id="36cc8-164">Redigera texten i e-postmeddelandet för att säga vad du behöver, men se till att inkludera länken som den är anpassad för att ansluta kunden direkt till både ditt konto och ditt leverantörs konto.</span><span class="sxs-lookup"><span data-stu-id="36cc8-164">Edit the text in the email to say what you need but be sure to include the link as it is personalized to connect the customer directly to both your account and your provider's account.</span></span> <span data-ttu-id="36cc8-165">Välj sedan **Done** (Klar).</span><span class="sxs-lookup"><span data-stu-id="36cc8-165">Then select **Done** .</span></span>

5. <span data-ttu-id="36cc8-166">När kunden har auktoriserat att du och din leverantör ska bli åter försäljare av poster, har du administratörs behörighet för att hantera prenumerationer, licenser och användare för deras räkning, och den indirekta leverantören kommer att kunna skicka beställningar för deras räkning.</span><span class="sxs-lookup"><span data-stu-id="36cc8-166">After the customer authorizes you and your provider to be their resellers of record, you'll have administrator permissions to manage their subscriptions, licenses, and users on their behalf, and your indirect provider will be able to submit orders on their behalf.</span></span>
6. <span data-ttu-id="36cc8-167">Om du vill hantera kundens konto, tjänster, användare och licenser expanderar du kundens post genom att välja nedåtpilen nära sitt namn.</span><span class="sxs-lookup"><span data-stu-id="36cc8-167">To manage the customer's account, services, users, and licenses, expand the customer's record by selecting the down arrow near their name.</span></span>

<span data-ttu-id="36cc8-168">Till skillnad från direkta fakturerings partner kan indirekta åter försäljare inte skapa Azure AD-klienter för sina nya kunder i Partner Center.</span><span class="sxs-lookup"><span data-stu-id="36cc8-168">Unlike direct bill partners, indirect resellers can't create Azure AD tenants for their new customers in Partner Center.</span></span> <span data-ttu-id="36cc8-169">Leverantören skapar klienten och anger dig som den indirekta åter försäljaren för den här kunden.</span><span class="sxs-lookup"><span data-stu-id="36cc8-169">Your provider will create the tenant and will specify you as the indirect reseller for this customer.</span></span> <span data-ttu-id="36cc8-170">Detta säkerställer att kunden kommer att visas i kund listan i Partner Center.</span><span class="sxs-lookup"><span data-stu-id="36cc8-170">This ensures that the customer will appear in your customer list in Partner Center.</span></span>

>[!Note]
><span data-ttu-id="36cc8-171">Du kan inte använda din direkta fakturerings funktion för att skapa inköp för kunder som du får som en indirekt åter försäljare.</span><span class="sxs-lookup"><span data-stu-id="36cc8-171">You will not be able to use your direct bill capability to create purchases for customers you acquire as an indirect reseller.</span></span>

## <a name="managing-your-direct-bill-customers-and-your-indirect-reseller-customers"></a><span data-ttu-id="36cc8-172">Hantera dina kunder med direkt fakturering och dina indirekta åter försäljare</span><span class="sxs-lookup"><span data-stu-id="36cc8-172">Managing your direct bill customers and your indirect reseller customers</span></span>

<span data-ttu-id="36cc8-173">Du hanterar dina kunder med direkt fakturering och dina indirekta åter försäljar kunder på olika sätt.</span><span class="sxs-lookup"><span data-stu-id="36cc8-173">You manage your direct bill customers and your indirect reseller customers differently.</span></span>

### <a name="direct-bill-customers-things-you-wont-do-as-an-indirect-reseller"></a><span data-ttu-id="36cc8-174">Direkt fakturerings kunder (saker som du inte gör som en indirekt åter försäljare)</span><span class="sxs-lookup"><span data-stu-id="36cc8-174">Direct bill customers (things you won't do as an indirect reseller)</span></span>

- <span data-ttu-id="36cc8-175">Skapa beställningar för produkter</span><span class="sxs-lookup"><span data-stu-id="36cc8-175">Create orders for products</span></span>
- <span data-ttu-id="36cc8-176">Hantera Azure-reservationer</span><span class="sxs-lookup"><span data-stu-id="36cc8-176">Manage Azure reservations</span></span>
- <span data-ttu-id="36cc8-177">Hantera deras order historik</span><span class="sxs-lookup"><span data-stu-id="36cc8-177">Manage their order history</span></span>
- <span data-ttu-id="36cc8-178">Köp program vara</span><span class="sxs-lookup"><span data-stu-id="36cc8-178">Purchase software</span></span>
- <span data-ttu-id="36cc8-179">Fakturera kunder direkt</span><span class="sxs-lookup"><span data-stu-id="36cc8-179">Bill customers directly</span></span>

### <a name="indirect-reseller-customers"></a><span data-ttu-id="36cc8-180">Kunder med indirekt åter försäljare</span><span class="sxs-lookup"><span data-stu-id="36cc8-180">Indirect reseller customers</span></span>

- <span data-ttu-id="36cc8-181">Din indirekta leverantör beställer produkter för dina kunder</span><span class="sxs-lookup"><span data-stu-id="36cc8-181">Your indirect provider orders products for your customers</span></span>
- <span data-ttu-id="36cc8-182">Hantera kunders licenser och användare</span><span class="sxs-lookup"><span data-stu-id="36cc8-182">Manage customers' licenses and users</span></span>
- <span data-ttu-id="36cc8-183">Hantera prenumerations förnyelser</span><span class="sxs-lookup"><span data-stu-id="36cc8-183">Handle subscription renewals</span></span>

### <a name="to-identify-customers-that-you-acquired-as-a-direct-bill-partner"></a><span data-ttu-id="36cc8-184">Identifiera kunder som du har köpt som en direkt fakturerings partner</span><span class="sxs-lookup"><span data-stu-id="36cc8-184">To identify customers that you acquired as a direct bill partner</span></span>

1. <span data-ttu-id="36cc8-185">Välj **kunder**</span><span class="sxs-lookup"><span data-stu-id="36cc8-185">Select **Customers**</span></span>

2. <span data-ttu-id="36cc8-186">Välj en kund för att visa information om den</span><span class="sxs-lookup"><span data-stu-id="36cc8-186">Select a customer to view their details</span></span>

3. <span data-ttu-id="36cc8-187">Om den här kunden är en direkt fakturerings partner kan du se alternativ för att **lägga till** eller **Visa produkter** och du kommer att se deras prenumerationer.</span><span class="sxs-lookup"><span data-stu-id="36cc8-187">If this customer is one you acquired as a direct bill partner, you will see options to **add** or **view products** and you will see their subscriptions.</span></span>

4. <span data-ttu-id="36cc8-188">Om kunden har en indirekt åter försäljare relation med dig är dessa alternativ inte tillgängliga.</span><span class="sxs-lookup"><span data-stu-id="36cc8-188">If the customer has an indirect reseller relationship with you, those options will not be available.</span></span>

## <a name="move-your-direct-bill-customers-to-your-indirect-provider"></a><span data-ttu-id="36cc8-189">Flytta dina direkt fakturerings kunder till din indirekta leverantör</span><span class="sxs-lookup"><span data-stu-id="36cc8-189">Move your direct bill customers to your indirect provider</span></span>

<span data-ttu-id="36cc8-190">Din indirekta Provider kan inte skicka beställningar eller befintliga prenumerations överföringar för dina befintliga kunder förrän de har en åter försäljares relation med dem.</span><span class="sxs-lookup"><span data-stu-id="36cc8-190">Your indirect provider cannot submit orders or existing subscription transfers for your existing direct bill customers until they have a reseller relationship with them.</span></span> <span data-ttu-id="36cc8-191">Du kan använda någon av följande metoder för att upprätta åter försäljarens relation mellan din indirekta leverantör och din befintliga direkta faktura.</span><span class="sxs-lookup"><span data-stu-id="36cc8-191">To establish the reseller relationship between your indirect provider and your existing direct bill customer, you can use one of the following methods:</span></span>

- [<span data-ttu-id="36cc8-192">Relations tillägg för åter försäljare</span><span class="sxs-lookup"><span data-stu-id="36cc8-192">Reseller relationship extension</span></span>](#reseller-relationship-extension)

- [<span data-ttu-id="36cc8-193">Skicka en indirekt åter försäljares inbjudan till kunden</span><span class="sxs-lookup"><span data-stu-id="36cc8-193">Send an indirect reseller invitation to the customer</span></span>](#send-an-indirect-reseller-invitation-to-the-customer)

<span data-ttu-id="36cc8-194">En detaljerad översikt över steg för steg-processen finns i [dokumentet direkt till indirekt över gång](https://partner.microsoft.com/resources/collection/Direct-Bill-transition-to-Indirect-reseller#/)</span><span class="sxs-lookup"><span data-stu-id="36cc8-194">You can find a detailed overview of the step-by-step process in the [Direct to indirect transition document](https://partner.microsoft.com/resources/collection/Direct-Bill-transition-to-Indirect-reseller#/)</span></span>

### <a name="reseller-relationship-extension"></a><span data-ttu-id="36cc8-195">Relations tillägg för åter försäljare</span><span class="sxs-lookup"><span data-stu-id="36cc8-195">Reseller relationship extension</span></span>

<span data-ttu-id="36cc8-196">Du kan använda funktionen för Relations tillägg för åter försäljare för att upprätta åter försäljarens relation mellan dina befintliga kunder med direkt fakturering och den indirekta providern med hjälp av instrument panelen för partner Center.</span><span class="sxs-lookup"><span data-stu-id="36cc8-196">You can use the reseller relationship extension feature to establish reseller relationship between your existing direct bill customers and your indirect provider using Partner Center Dashboard.</span></span> <span data-ttu-id="36cc8-197">Observera följande innan du använder funktionen:</span><span class="sxs-lookup"><span data-stu-id="36cc8-197">Before using the feature, note the following:</span></span>

- <span data-ttu-id="36cc8-198">Den här funktionen är bara tillgänglig för direkta fakturerings partner som över gången till bli en indirekt åter försäljare har slutfört [registreringen av den indirekta åter försäljaren](#get-started).</span><span class="sxs-lookup"><span data-stu-id="36cc8-198">This feature is only available to direct bill partners who are transitioning to become an indirect reseller have completed the [indirect reseller enrollment](#get-started).</span></span>

- <span data-ttu-id="36cc8-199">Du kan bara använda den här funktionen för befintliga kunder med direkt fakturering.</span><span class="sxs-lookup"><span data-stu-id="36cc8-199">You can only apply this feature to existing direct bill customers.</span></span> <span data-ttu-id="36cc8-200">Det gäller inte för [indirekta åter försäljar kunder](#acquire-new-customers-as-indirect-reseller).</span><span class="sxs-lookup"><span data-stu-id="36cc8-200">It is not applicable to [indirect reseller customers](#acquire-new-customers-as-indirect-reseller).</span></span>

- <span data-ttu-id="36cc8-201">Du kan bara välja en indirekt Provider för vilken du har [accepterat en partner-inbjudan från den indirekta providern](#accept-a-partnership-invitation-from-your-indirect-provider).</span><span class="sxs-lookup"><span data-stu-id="36cc8-201">You can only select an indirect provider for which you have [accepted a partner invitation from your indirect provider](#accept-a-partnership-invitation-from-your-indirect-provider).</span></span>

- <span data-ttu-id="36cc8-202">En kopia av den fakturerings information som du har för den här kunden kommer att göras tillgänglig för den indirekta leverantören.</span><span class="sxs-lookup"><span data-stu-id="36cc8-202">A copy of the bill-to info you have for this customer will be made available to the indirect provider.</span></span> <span data-ttu-id="36cc8-203">Du kan komma åt fakturerings informationen genom att gå till konto sidan för den här kunden i Partner Center-instrumentpanelen.</span><span class="sxs-lookup"><span data-stu-id="36cc8-203">You can access the bill-to info by accessing the Account page for this customer in Partner Center Dashboard.</span></span>

    > [!NOTE]
    > <span data-ttu-id="36cc8-204">Genom att använda funktionen för Relations tillägg för åter försäljare godkänner du att du delar den fakturerings information som du har för den här kunden med den indirekta providern.</span><span class="sxs-lookup"><span data-stu-id="36cc8-204">By using the reseller relationship extension feature, you consent to sharing the bill-to info you have for this customer with the indirect provider.</span></span>

- <span data-ttu-id="36cc8-205">Den indirekta providern kommer inte att tillhandahållas med [delegerad administrations behörighet](customers-revoke-admin-privileges.md) till kund klienten.</span><span class="sxs-lookup"><span data-stu-id="36cc8-205">Your indirect provider will not be provided with [delegated administration privileges](customers-revoke-admin-privileges.md) to the customer tenant.</span></span> <span data-ttu-id="36cc8-206">Om den indirekta leverantören kräver delegerad administrations behörighet måste du skicka en indirekt åter försäljare-inbjudan till kunden i stället.</span><span class="sxs-lookup"><span data-stu-id="36cc8-206">If your indirect provider requires delegated administration privileges, you must send an indirect reseller invitation to the customer instead.</span></span>

- <span data-ttu-id="36cc8-207">När åter försäljarens relation har upprättats visas den indirekta providern som en CSP-partner till kunden på sidan partner relationer i [M365 administrations Center](https://admin.microsoft.com/AdminPortal/Home#/partners) och [Microsoft Store för företag](/microsoft-store/work-with-partner-microsoft-store-business).</span><span class="sxs-lookup"><span data-stu-id="36cc8-207">Once the reseller relationship is established, the indirect provider will appear as a CSP partner to the customer under the Partner Relationships page in [M365 Admin Center](https://admin.microsoft.com/AdminPortal/Home#/partners) and [Microsoft Store for Business](/microsoft-store/work-with-partner-microsoft-store-business).</span></span>

    > [!IMPORTANT]
    > <span data-ttu-id="36cc8-208">För att undvika förvirring och missförstånd är du avtals enlig avtal av ditt partner avtal för att informera och erhålla medgivande från direkt fakturerings kunden innan du använder funktionen för Relations tillägg för att upprätta åter försäljarens relation mellan en befintlig direkt fakturerings kund och en indirekt leverantör.</span><span class="sxs-lookup"><span data-stu-id="36cc8-208">To avoid confusion and misunderstanding, you are contractually obliged by your partner agreement to inform and obtain consent from the direct bill customer before you use the relationship extension feature to establish reseller relationship between an existing direct bill customer and an indirect provider.</span></span>

<span data-ttu-id="36cc8-209">Så här använder du den här funktionen på en befintlig kund klient organisation:</span><span class="sxs-lookup"><span data-stu-id="36cc8-209">To use this feature on an existing customer tenant:</span></span>

1. <span data-ttu-id="36cc8-210">Logga in på Partner Center som **Administratörs agent** .</span><span class="sxs-lookup"><span data-stu-id="36cc8-210">Log in to Partner Center as an **Admin Agent** .</span></span>

2. <span data-ttu-id="36cc8-211">På **sidan kunder** väljer du en befintlig kund och klickar på dess **snabb länkars** ikon för att expandera kundens sammanfattningsvy.</span><span class="sxs-lookup"><span data-stu-id="36cc8-211">In the **Customers page** , select an existing customer and click on its **Quick links** icon to expand the summary view of the customer.</span></span>

3. <span data-ttu-id="36cc8-212">Under **indirekta providers** klickar du på **överför kund på en indirekt Provider** .</span><span class="sxs-lookup"><span data-stu-id="36cc8-212">Under **Indirect provider(s)** , click **Transfer customer on an indirect provider** .</span></span>

    :::image type="content" source="images/direct/direct5-1.png" alt-text="Överför kunden till en indirekt Provider":::

4. <span data-ttu-id="36cc8-214">I popup-dialogrutan väljer du den **indirekta providern** som du vill ha åter försäljarens relation med kunden.</span><span class="sxs-lookup"><span data-stu-id="36cc8-214">In the pop-up dialog, select the **Indirect Provider** you would like to have reseller relationship with the customer.</span></span>

5. <span data-ttu-id="36cc8-215">Klicka på **Spara och fortsätt** .</span><span class="sxs-lookup"><span data-stu-id="36cc8-215">Click **Save and continue** .</span></span>

6. <span data-ttu-id="36cc8-216">Kontrol lera att den valda indirekta providern visas under **indirekta providers** .</span><span class="sxs-lookup"><span data-stu-id="36cc8-216">Verify the selected indirect provider shows up under **Indirect provider(s)** .</span></span>

    :::image type="content" source="images/direct/direct5-2.png" alt-text="Indirekt Provider listad":::

### <a name="send-an-indirect-reseller-invitation-to-the-customer"></a><span data-ttu-id="36cc8-218">Skicka en indirekt åter försäljares inbjudan till kunden</span><span class="sxs-lookup"><span data-stu-id="36cc8-218">Send an indirect reseller invitation to the customer</span></span>

<span data-ttu-id="36cc8-219">Din indirekta leverantör kan inte skicka in beställningar för dina befintliga kunder för direkt fakturering förrän de har en åter försäljares relation med dem.</span><span class="sxs-lookup"><span data-stu-id="36cc8-219">Your indirect provider cannot submit orders for your existing direct bill customers until they have a reseller relationship with them.</span></span> <span data-ttu-id="36cc8-220">För att upprätta åter försäljarens relation mellan dina befintliga kunder och den indirekta leverantören, bjuder du in kunden med en indirekt åter försäljares inbjudan.</span><span class="sxs-lookup"><span data-stu-id="36cc8-220">To establish the reseller relationship between your existing customers and your indirect provider, invite the customer using an indirect reseller invitation.</span></span>

1. <span data-ttu-id="36cc8-221">Välj **indirekta leverantörer** från din partner Center vänstra navigerings fältet.</span><span class="sxs-lookup"><span data-stu-id="36cc8-221">Select **Indirect providers** from your Partner Center left nav.</span></span>

2. <span data-ttu-id="36cc8-222">Välj **Bjud in nya kunder** för att bjuda in en kund att upprätta en åter försäljares relation med både du och den indirekta providern på samma tid.</span><span class="sxs-lookup"><span data-stu-id="36cc8-222">Select **Invite new customers** to invite a customer to establish a reseller relationship with both you and the indirect provider at the same time.</span></span> <span data-ttu-id="36cc8-223">Leverantören måste ha en åter försäljar relation med din kund, så att de kan skicka beställningar på din kunds räkning när kunden vill köpa nya prenumerationer eller lägga till nya licenser i befintliga prenumerationer.</span><span class="sxs-lookup"><span data-stu-id="36cc8-223">The provider needs to have a reseller relationship with your customer, so they can submit orders on your customer's behalf when the customer wants to buy new subscriptions or add new licenses to existing subscriptions.</span></span>

    :::image type="content" source="images/direct/direct6.png" alt-text="Bjud in nya kunder":::

3. <span data-ttu-id="36cc8-225">På nästa sida granskar du utkastet till e-postmeddelandet.</span><span class="sxs-lookup"><span data-stu-id="36cc8-225">On the next page, review the draft email message.</span></span> <span data-ttu-id="36cc8-226">Du kan öppna utkast meddelandet i ett e-postmeddelande, eller så kan du kopiera meddelandet till Urklipp och klistra in det i ett e-postmeddelande.</span><span class="sxs-lookup"><span data-stu-id="36cc8-226">You can open the draft message in email, or you can copy the message to your clipboard and paste it into an email.</span></span>

4. <span data-ttu-id="36cc8-227">Redigera texten i e-postmeddelandet för att säga vad du behöver, men se till att inkludera länken som den är anpassad för att ansluta kunden direkt till både ditt konto och ditt leverantörs konto.</span><span class="sxs-lookup"><span data-stu-id="36cc8-227">Edit the text in the email to say what you need but be sure to include the link as it is personalized to connect the customer directly to both your account and your provider's account.</span></span> <span data-ttu-id="36cc8-228">Välj sedan **Done** (Klar).</span><span class="sxs-lookup"><span data-stu-id="36cc8-228">Then select **Done** .</span></span>

5. <span data-ttu-id="36cc8-229">När kunden har auktoriserat att du och din leverantör ska bli åter försäljare av poster, har du administratörs behörighet för att hantera prenumerationer, licenser och användare för deras räkning, och den indirekta leverantören kommer att kunna skicka beställningar för deras räkning.</span><span class="sxs-lookup"><span data-stu-id="36cc8-229">After the customer authorizes you and your provider to be their resellers of record, you'll have administrator permissions to manage their subscriptions, licenses, and users on their behalf, and your indirect provider will be able to submit orders on their behalf.</span></span>

6. <span data-ttu-id="36cc8-230">Om du vill hantera kundens konto, tjänster, användare och licenser expanderar du kundens post genom att välja nedåtpilen nära sitt namn.</span><span class="sxs-lookup"><span data-stu-id="36cc8-230">To manage the customer's account, services, users, and licenses, expand the customer's record by selecting the down arrow near their name.</span></span>

### <a name="microsoft-customer-agreement-acceptance"></a><span data-ttu-id="36cc8-231">Godkännande av Microsofts kund avtal</span><span class="sxs-lookup"><span data-stu-id="36cc8-231">Microsoft Customer Agreement acceptance</span></span>

<span data-ttu-id="36cc8-232">Microsoft Cloud avtalet gäller till och med 31 januari 2020.</span><span class="sxs-lookup"><span data-stu-id="36cc8-232">Microsoft Cloud Agreement is valid until January 31, 2020.</span></span> <span data-ttu-id="36cc8-233">Efter det datumet måste alla kunder, befintliga och nya, signera det nya [Microsofts kund avtal](confirm-customer-agreement.md).</span><span class="sxs-lookup"><span data-stu-id="36cc8-233">After that date, all customers, existing and new, must sign the new [Microsoft Customer Agreement](confirm-customer-agreement.md).</span></span> <span data-ttu-id="36cc8-234">Vid över gång av kunder, om:</span><span class="sxs-lookup"><span data-stu-id="36cc8-234">For transitioning customers, if:</span></span>

- <span data-ttu-id="36cc8-235">**Kunden har inte accepterat Microsofts kund avtal ännu**</span><span class="sxs-lookup"><span data-stu-id="36cc8-235">**Customer has not accepted Microsoft Customer Agreement yet**</span></span>

   <span data-ttu-id="36cc8-236">Arbeta med den indirekta leverantören för att låta kunden [godkänna Microsofts kund avtal](confirm-customer-agreement.md).</span><span class="sxs-lookup"><span data-stu-id="36cc8-236">Please work with Indirect Provider to have customer [accept the Microsoft Customer Agreement](confirm-customer-agreement.md).</span></span>

- <span data-ttu-id="36cc8-237">**Kunden har accepterat Microsofts kund avtal med dig via Microsoft 365 administrations centret**</span><span class="sxs-lookup"><span data-stu-id="36cc8-237">**Customer has accepted Microsoft Customer Agreement with you through the Microsoft 365 Admin Center**</span></span>

   <span data-ttu-id="36cc8-238">Godkännandet kommer att behållas när åter försäljarens relation upprättas med den indirekta providern.</span><span class="sxs-lookup"><span data-stu-id="36cc8-238">The acceptance will be retained once the reseller relationship is established with the Indirect Provider.</span></span> <span data-ttu-id="36cc8-239">Du behöver inte göra något.</span><span class="sxs-lookup"><span data-stu-id="36cc8-239">There is nothing you need to do.</span></span>

- <span data-ttu-id="36cc8-240">**Kunden har accepterat Microsofts kund avtal med dig genom partner attestering**</span><span class="sxs-lookup"><span data-stu-id="36cc8-240">**Customer has accepted Microsoft Customer Agreement with you through partner attestation**</span></span>

   <span data-ttu-id="36cc8-241">Godkännandet kommer inte att behållas.</span><span class="sxs-lookup"><span data-stu-id="36cc8-241">The acceptance will not be retained.</span></span> <span data-ttu-id="36cc8-242">Arbeta med den indirekta providern för att [Uppdatera kundens godkännande i Partner Center](confirm-customer-agreement.md#confirm-customer-acceptance-for-existing-customers).</span><span class="sxs-lookup"><span data-stu-id="36cc8-242">Please work with Indirect Provider to [update the customer's acceptance in Partner Center](confirm-customer-agreement.md#confirm-customer-acceptance-for-existing-customers).</span></span>

## <a name="transfer-existing-direct-bill-subscriptions-to-indirect-provider"></a><span data-ttu-id="36cc8-243">Överför befintliga direkt fakturerings prenumerationer till en indirekt Provider</span><span class="sxs-lookup"><span data-stu-id="36cc8-243">Transfer existing direct bill subscriptions to indirect provider</span></span>

<span data-ttu-id="36cc8-244">Under KRYPTOGRAFIPROVIDERns indirekta modell har indirekta åter försäljare inga fakturerings relationer med Microsoft.</span><span class="sxs-lookup"><span data-stu-id="36cc8-244">Under CSP indirect model, indirect resellers do not have billing relationships with Microsoft.</span></span> <span data-ttu-id="36cc8-245">I stället får indirekta åter försäljare prenumerationer för sina kunder via sina indirekta leverantörer.</span><span class="sxs-lookup"><span data-stu-id="36cc8-245">Instead, indirect resellers obtain subscriptions for their customers through their indirect providers.</span></span> <span data-ttu-id="36cc8-246">Vid över gång från direkt fakturerings partner till indirekt åter försäljare måste du överföra de befintliga prenumerationerna som du har som direkt fakturerings partner till din indirekta leverantör.</span><span class="sxs-lookup"><span data-stu-id="36cc8-246">While transitioning from direct bill partner to indirect reseller, you need to transfer the existing subscriptions you have as the direct bill partner to your indirect provider.</span></span> <span data-ttu-id="36cc8-247">Du kan använda funktionen för att överföra prenumerationer på Partner Center-instrumentpanelen.</span><span class="sxs-lookup"><span data-stu-id="36cc8-247">You can use the self-served subscription transfer feature in Partner Center Dashboard to do so.</span></span>

### <a name="pre-requisites"></a><span data-ttu-id="36cc8-248">Förutsättningar</span><span class="sxs-lookup"><span data-stu-id="36cc8-248">Pre-requisites</span></span>

- <span data-ttu-id="36cc8-249">Den här funktionen är bara tillgänglig för att överföra partner som har slutfört registreringen av den indirekta åter försäljaren med sina befintliga leverantörer av direkt fakturerings partner</span><span class="sxs-lookup"><span data-stu-id="36cc8-249">This feature is only available to transitioning partners who have completed the indirect reseller enrollment using their existing direct bill partner tenants</span></span>

- <span data-ttu-id="36cc8-250">Innan prenumerationer som är kopplade till en specifik kund överförs måste övergående partner flytta kunden till en indirekt Provider.</span><span class="sxs-lookup"><span data-stu-id="36cc8-250">Before transferring subscriptions associated with a given customer, the transitioning partner must move the customer to an indirect provider.</span></span>

- <span data-ttu-id="36cc8-251">Kunden måste ha [godkänt Microsofts kund avtal via den indirekta providern](#microsoft-customer-agreement-acceptance).</span><span class="sxs-lookup"><span data-stu-id="36cc8-251">Customer must have [accepted Microsoft Customer Agreement through the Indirect Provider](#microsoft-customer-agreement-acceptance).</span></span>

### <a name="how-to-transition-to-indirect-reseller-status"></a><span data-ttu-id="36cc8-252">Hur du övergår till en indirekt åter försäljares status</span><span class="sxs-lookup"><span data-stu-id="36cc8-252">How to transition to indirect reseller status</span></span>

<span data-ttu-id="36cc8-253">Funktionen är en fyra stegs process där:</span><span class="sxs-lookup"><span data-stu-id="36cc8-253">The feature is a 4-step process, where:</span></span>

- <span data-ttu-id="36cc8-254">Över gångs partnern skapar en begäran om prenumerations överföring.</span><span class="sxs-lookup"><span data-stu-id="36cc8-254">The transitioning partner creates a subscription transfer request.</span></span> <span data-ttu-id="36cc8-255">Begäran innehåller en eller flera befintliga prenumerationer som är kopplade till samma kund och som är adresserad till en indirekt Provider.</span><span class="sxs-lookup"><span data-stu-id="36cc8-255">The request contains one or more existing subscriptions associated with the same customer and is addressed to an indirect provider.</span></span>

- <span data-ttu-id="36cc8-256">Den indirekta providern granskar och godkänner (eller avvisar) överföringsbegäran.</span><span class="sxs-lookup"><span data-stu-id="36cc8-256">The indirect provider reviews and accepts (or reject) the transfer request.</span></span>

- <span data-ttu-id="36cc8-257">Den indirekta providern verifierar att överföringsbegäran är slutförd.</span><span class="sxs-lookup"><span data-stu-id="36cc8-257">The indirect provider verifies that the transfer request is complete.</span></span>

- <span data-ttu-id="36cc8-258">Över gångs partner verifierar att överföringsbegäran är slutförd.</span><span class="sxs-lookup"><span data-stu-id="36cc8-258">The transitioning partner verifies that the transfer request is complete.</span></span>

### <a name="transitioning-partner"></a><span data-ttu-id="36cc8-259">Över gångs partner</span><span class="sxs-lookup"><span data-stu-id="36cc8-259">Transitioning partner</span></span>

> [!NOTE]
> <span data-ttu-id="36cc8-260">Du kan också använda [partner Center API/SDK](/partner-center/develop/manage-customers) för att överföra befintliga prenumerationer till den indirekta providern.</span><span class="sxs-lookup"><span data-stu-id="36cc8-260">You can also use [Partner Center API/SDK](/partner-center/develop/manage-customers) to transfer the existing subscriptions to your indirect provider.</span></span>
>
> - [<span data-ttu-id="36cc8-261">Få en kunds tillstånd för överföring av prenumerationer</span><span class="sxs-lookup"><span data-stu-id="36cc8-261">Get a customer's subscriptions transfer eligibility</span></span>](/partner-center/develop/get-customer-s-subscriptions-transfer-eligibility)
> - [<span data-ttu-id="36cc8-262">Skapa en kunds överföring</span><span class="sxs-lookup"><span data-stu-id="36cc8-262">Create a customer's transfer</span></span>](/partner-center/develop/create-a-transfer)
> - [<span data-ttu-id="36cc8-263">Återkalla en kunds överföring</span><span class="sxs-lookup"><span data-stu-id="36cc8-263">Withdraw a customer's transfer</span></span>](/partner-center/develop/withdraw-a-transfer)
> - [<span data-ttu-id="36cc8-264">Acceptera en kunds överföring</span><span class="sxs-lookup"><span data-stu-id="36cc8-264">Accept a customer's transfer</span></span>](/partner-center/develop/accept-a-transfer)
> - [<span data-ttu-id="36cc8-265">Avvisa en kunds överföring</span><span class="sxs-lookup"><span data-stu-id="36cc8-265">Reject a Customer's transfer</span></span>](/partner-center/develop/reject-a-transfer)
> - [<span data-ttu-id="36cc8-266">Hämta en kunds överföringar</span><span class="sxs-lookup"><span data-stu-id="36cc8-266">Get a customer's transfers</span></span>](/partner-center/develop/get-all-of-a-customer-s-transfers)
> - [<span data-ttu-id="36cc8-267">Hämta överförings information per ID</span><span class="sxs-lookup"><span data-stu-id="36cc8-267">Get transfer details by id</span></span>](/partner-center/develop/get-transfer-by-id)

### <a name="transitioning-partner---create-transfer-request"></a><span data-ttu-id="36cc8-268">Över gångs partner – skapa överföringsbegäran</span><span class="sxs-lookup"><span data-stu-id="36cc8-268">Transitioning partner - create transfer request</span></span>

<span data-ttu-id="36cc8-269">Så här skapar du en överföringsbegäran som över gångs partner:</span><span class="sxs-lookup"><span data-stu-id="36cc8-269">To create a transfer request as the transitioning partner:</span></span>

1. <span data-ttu-id="36cc8-270">Logga in på Partner Center som **Administratörs agent** .</span><span class="sxs-lookup"><span data-stu-id="36cc8-270">Log in to Partner Center as an **Admin Agent** .</span></span>

2. <span data-ttu-id="36cc8-271">På sidan **kunder** väljer du den avsedda kunden och klickar på ikonen snabb Länkar för att expandera kundens sammanfattningsvy.</span><span class="sxs-lookup"><span data-stu-id="36cc8-271">In the **Customers** page, select the intended customer and click on the Quick links icon to expand the summary view of the customer.</span></span>

3. <span data-ttu-id="36cc8-272">Under **indirekta providers** kontrollerar du att den avsedda indirekta providern visas.</span><span class="sxs-lookup"><span data-stu-id="36cc8-272">Under **Indirect provider(s)** , confirm that the intended indirect provider is listed.</span></span>

4. <span data-ttu-id="36cc8-273">Klicka på **Visa prenumerationer** .</span><span class="sxs-lookup"><span data-stu-id="36cc8-273">Click **View Subscriptions** .</span></span>

5. <span data-ttu-id="36cc8-274">På sidan **prenumerationer** söker du efter **prenumerations överföring** .</span><span class="sxs-lookup"><span data-stu-id="36cc8-274">In the **Subscriptions** page, look for **Subscription Transfer** .</span></span>

6. <span data-ttu-id="36cc8-275">Under **prenumerations överföring** klickar du på **begär prenumerations överföring** .</span><span class="sxs-lookup"><span data-stu-id="36cc8-275">Under **Subscription Transfer** , click **Request subscription transfer** .</span></span>

    :::image type="content" source="images/direct/direct8.png" alt-text="Begär prenumerations överföring":::

7. <span data-ttu-id="36cc8-277">I dialog rutan överför begäran väljer du en eller flera prenumerationer som ska överföras.</span><span class="sxs-lookup"><span data-stu-id="36cc8-277">In the transfer request dialog, select one or more subscriptions to be transferred.</span></span>

    :::image type="content" source="images/direct/direct9.png" alt-text="Skapa överföringsbegäran":::

8. <span data-ttu-id="36cc8-279">Klicka på **Skapa** .</span><span class="sxs-lookup"><span data-stu-id="36cc8-279">Click **Create** .</span></span>

9. <span data-ttu-id="36cc8-280">En aktiv begäran om prenumerations överföring visas under **prenumerations överföring** .</span><span class="sxs-lookup"><span data-stu-id="36cc8-280">An active subscription transfer request will appear under **Subscription Transfer** .</span></span>

    :::image type="content" source="images/direct/direct10.png" alt-text="Lista över överförings begär Anden":::

10. <span data-ttu-id="36cc8-282">Informera den indirekta leverantören att du har skapat en begäran om prenumerations överföring.</span><span class="sxs-lookup"><span data-stu-id="36cc8-282">Inform your indirect provider that you have created a subscription transfer request to them.</span></span>

### <a name="indirect-provider---accept-transfer-request"></a><span data-ttu-id="36cc8-283">Indirekt Provider-Godkänn överföringsbegäran</span><span class="sxs-lookup"><span data-stu-id="36cc8-283">Indirect provider - accept transfer request</span></span>

<span data-ttu-id="36cc8-284">Så här granskar och godkänner du en överföringsbegäran som den indirekta providern:</span><span class="sxs-lookup"><span data-stu-id="36cc8-284">To review and accept a transfer request as the indirect provider:</span></span>

1. <span data-ttu-id="36cc8-285">Logga in på Partner Center som **Administratörs** agent eller **försäljnings agent** .</span><span class="sxs-lookup"><span data-stu-id="36cc8-285">Log in to Partner Center as an **Admin** Agent or **Sales Agent** .</span></span>

2. <span data-ttu-id="36cc8-286">På sidan **kunder** väljer du den avsedda kunden och klickar på dess snabb länkars ikon för att expandera kundens sammanfattningsvy.</span><span class="sxs-lookup"><span data-stu-id="36cc8-286">In the **Customers** page, select the intended customer and click on its Quick links icon to expand the summary view of the customer.</span></span>

3. <span data-ttu-id="36cc8-287">Under **indirekta åter försäljare** bekräftar du att över gångs partnern visas.</span><span class="sxs-lookup"><span data-stu-id="36cc8-287">Under **Indirect reseller(s)** , confirm the transitioning partner is listed.</span></span>

4. <span data-ttu-id="36cc8-288">Klicka på **Visa prenumerationer** .</span><span class="sxs-lookup"><span data-stu-id="36cc8-288">Click **View Subscriptions** .</span></span>

5. <span data-ttu-id="36cc8-289">På sidan **prenumerationer** söker du efter **prenumerations överföring** .</span><span class="sxs-lookup"><span data-stu-id="36cc8-289">In the **Subscriptions** page, look for **Subscription Transfer** .</span></span>

    :::image type="content" source="images/direct/direct11.png" alt-text="Visa överförings förfrågan":::

6. <span data-ttu-id="36cc8-291">Under **prenumerations överföring** klickar du på den överföringsbegäran som ska granskas.</span><span class="sxs-lookup"><span data-stu-id="36cc8-291">Under **Subscription Transfer** , click on the transfer request to review.</span></span>

7. <span data-ttu-id="36cc8-292">Klicka på **acceptera** (eller **avvisa** ) efter behov.</span><span class="sxs-lookup"><span data-stu-id="36cc8-292">Click **Accept** (or **Reject** ) as appropriate.</span></span>

    :::image type="content" source="images/direct/direct12.png" alt-text="Godkänn överföringsbegäran":::

8. <span data-ttu-id="36cc8-294">Vänta tills överförings förfrågan har slutförts.</span><span class="sxs-lookup"><span data-stu-id="36cc8-294">Wait for the transfer request to complete.</span></span>

### <a name="indirect-provider---verify-transfer-request-is-complete"></a><span data-ttu-id="36cc8-295">Indirekt provider-Kontrol lera att överföringsbegäran har slutförts</span><span class="sxs-lookup"><span data-stu-id="36cc8-295">Indirect provider - verify transfer request is complete</span></span>

1. <span data-ttu-id="36cc8-296">När överföringsbegäran har slutförts kontrollerar du att du kan se att prenumerationerna visas under **prenumerationer** .</span><span class="sxs-lookup"><span data-stu-id="36cc8-296">After the transfer request is completed successfully, verify that you can see the subscriptions appear under **Subscriptions** .</span></span>

2. <span data-ttu-id="36cc8-297">Informera över gångs partnern.</span><span class="sxs-lookup"><span data-stu-id="36cc8-297">Inform the transitioning partner.</span></span>

### <a name="transitioning-partner---verify-transfer-request-is-complete"></a><span data-ttu-id="36cc8-298">Övergående partner – kontrol lera att överföringsbegäran har slutförts</span><span class="sxs-lookup"><span data-stu-id="36cc8-298">Transitioning partner - verify transfer request is complete</span></span>

<span data-ttu-id="36cc8-299">Över gångs partner bör göra följande:</span><span class="sxs-lookup"><span data-stu-id="36cc8-299">The transitioning partner should do the following:</span></span>

1. <span data-ttu-id="36cc8-300">Logga in på Partner Center som **Administratörs agent** eller **försäljnings agent** .</span><span class="sxs-lookup"><span data-stu-id="36cc8-300">Sign into Partner Center as an **Admin Agent** or **Sales Agent** .</span></span>

2. <span data-ttu-id="36cc8-301">På sidan **kunder** väljer du den avsedda kunden och klickar på ikonen **snabb länkar** för att expandera kundens sammanfattningsvy.</span><span class="sxs-lookup"><span data-stu-id="36cc8-301">In the **Customers** page, select the intended customer and click on the **Quick links** icon to expand the summary view of the customer.</span></span>

3. <span data-ttu-id="36cc8-302">Klicka på **Visa prenumerationer** .</span><span class="sxs-lookup"><span data-stu-id="36cc8-302">Click **View Subscriptions** .</span></span>

4. <span data-ttu-id="36cc8-303">På sidan **prenumerationer** söker du efter **prenumerations överföring** .</span><span class="sxs-lookup"><span data-stu-id="36cc8-303">In the **Subscriptions** page, look for **Subscription Transfer** .</span></span>

5. <span data-ttu-id="36cc8-304">Kontrol lera att överföringsbegäran har marker ATS som **slutförd** .</span><span class="sxs-lookup"><span data-stu-id="36cc8-304">Verify that the transfer request is marked as **Complete** .</span></span>

6. <span data-ttu-id="36cc8-305">Kontrol lera att prenumerationerna inte längre visas som aktiva på sidan **prenumerationer** :</span><span class="sxs-lookup"><span data-stu-id="36cc8-305">Verify that the subscription(s) no longer appear as active in the **Subscriptions** page:</span></span>

   1. <span data-ttu-id="36cc8-306">Om det här är en Azure-prenumeration (MS-AZR-0145P) visas den inte längre.</span><span class="sxs-lookup"><span data-stu-id="36cc8-306">If this is an Azure subscription (MS-AZR-0145P), it will no longer be listed.</span></span>

   2. <span data-ttu-id="36cc8-307">Om det här är en licens baserad prenumeration (Office 365, Dynamics, Intune) visas den med tillståndet **pausad** .</span><span class="sxs-lookup"><span data-stu-id="36cc8-307">If this is a license-based subscription (Office 365, Dynamics, Intune), it will be listed with state as **Suspended** .</span></span>

   :::image type="content" source="images/direct/direct13.png" alt-text="Prenumerationen har pausats":::

### <a name="considerations"></a><span data-ttu-id="36cc8-309">Överväganden</span><span class="sxs-lookup"><span data-stu-id="36cc8-309">Considerations</span></span>

- <span data-ttu-id="36cc8-310">**Prenumerations-ID skiljer sig efter överföringen.**</span><span class="sxs-lookup"><span data-stu-id="36cc8-310">**Subscription ID will be different after transfer.**</span></span> <span data-ttu-id="36cc8-311">Om det är en Azure-prenumeration (MS-AZR-0145P) har dessutom ett ID för Azure-prenumeration, som är kvar från den tidigare ägaren, och kommer att visas i Azures hanterings Portal.</span><span class="sxs-lookup"><span data-stu-id="36cc8-311">If it is an Azure subscription (MS-AZR-0145P), additionally, it will have an Azure Subscription ID, which is retained from the previous owner, and will appear in the Azure management portal.</span></span>

- <span data-ttu-id="36cc8-312">**Det går inte att referera till samma prenumeration av flera överförings begär Anden.**</span><span class="sxs-lookup"><span data-stu-id="36cc8-312">**The same subscription cannot be referenced by multiple transfer requests.**</span></span> <span data-ttu-id="36cc8-313">När du har skapat en överföringsbegäran som innehåller en befintlig prenumeration kan du inte skapa ytterligare överförings begär Anden, inklusive samma prenumeration, tills den första överförings förfrågan har avbrutits.</span><span class="sxs-lookup"><span data-stu-id="36cc8-313">After you have created a transfer request, which includes an existing subscription, you cannot create additional transfer requests including the same subscription, until the first transfer request is canceled.</span></span>

- <span data-ttu-id="36cc8-314">**Tilläggs komponenter för licensbaserade prenumerationer måste överföras tillsammans med deras bas prenumeration.**</span><span class="sxs-lookup"><span data-stu-id="36cc8-314">**Add-ons for license-based subscriptions must be transferred along with their base subscription.**</span></span> <span data-ttu-id="36cc8-315">Om du väljer en befintlig prenumeration med ett eller flera tillägg tas tilläggen automatiskt med i överföringsbegäran när du skapar en överföringsbegäran.</span><span class="sxs-lookup"><span data-stu-id="36cc8-315">When creating a transfer request, if you pick an existing subscription with one or more add-ons, the add-ons will automatically be included in the transfer request.</span></span>

- <span data-ttu-id="36cc8-316">**Ändringar av licens antalet för en prenumeration visas inte i den befintliga överförings förfrågan.**</span><span class="sxs-lookup"><span data-stu-id="36cc8-316">**License count changes to a subscription will not be reflected in existing transfer request.**</span></span> <span data-ttu-id="36cc8-317">När du har skapat en överföringsbegäran som innehåller en befintlig prenumeration bör du undvika att uppdatera licens antalet för prenumerationen (eller tillhör ande tillägg).</span><span class="sxs-lookup"><span data-stu-id="36cc8-317">After you have created a transfer request which includes an existing subscription, you should avoid updating the license quantity of the subscription (or associated addons).</span></span> <span data-ttu-id="36cc8-318">Om du gör det visas inte den nya kvantiteten i överförings förfrågan.</span><span class="sxs-lookup"><span data-stu-id="36cc8-318">If you do so, the new quantity will not be reflected in the transfer request.</span></span> <span data-ttu-id="36cc8-319">När den indirekta providern har accepterat överförings förfrågan kommer den resulterande prenumerationen att ha den gamla kvantiteten.</span><span class="sxs-lookup"><span data-stu-id="36cc8-319">After the indirect provider accepts the transfer request, the resultant subscription will have the old quantity.</span></span> <span data-ttu-id="36cc8-320">Om du vill att den nya kvantiteten ska överföras till den indirekta providern måste du avbryta den befintliga överföringsbegäran och återskapa en ny.</span><span class="sxs-lookup"><span data-stu-id="36cc8-320">If you wish for the new quantity to be transferred to the indirect provider, you must cancel the existing transfer request and recreate a new one.</span></span>

- <span data-ttu-id="36cc8-321">**Alla inköp kan inte överföras med hjälp av prenumerations överföring med egen prenumeration.**</span><span class="sxs-lookup"><span data-stu-id="36cc8-321">**Not all purchases can be transferred using self-served subscription transfer.**</span></span> <span data-ttu-id="36cc8-322">För närvarande kan du bara överföra O365-prenumerationer och Azure PAYG-prenumerationer (MS-AZR-0145P) med hjälp av den här funktionen.</span><span class="sxs-lookup"><span data-stu-id="36cc8-322">Currently, you can only transfer O365 subscriptions and Azure PAYG subscriptions (MS-AZR-0145P) using this feature.</span></span> <span data-ttu-id="36cc8-323">Andra köp, inklusive Azure-planer, reserverade Azure-instanser, Termbaserade prenumerationer och SaaS-prenumerationer för Azure Marketplace stöds inte.</span><span class="sxs-lookup"><span data-stu-id="36cc8-323">Other purchases including Azure Plans, Azure Reserved Instances, Term-based Subscriptions and SaaS subscriptions for Azure Marketplace are not supported.</span></span> <span data-ttu-id="36cc8-324">Du kommer att se en orsak till varför en prenumeration inte kan överföras på sidan skicka överförings förfrågan.</span><span class="sxs-lookup"><span data-stu-id="36cc8-324">You will see a reason why a subscription cannot be transferred in the submit transfer request page.</span></span> <span data-ttu-id="36cc8-325">Om du vill överföra dessa prenumerationer måste du [avbryta den befintliga prenumerationen](create-a-new-subscription.md#suspend-or-cancel-a-subscription) och köpa ett nytt erbjudande för kunden via den indirekta providern.</span><span class="sxs-lookup"><span data-stu-id="36cc8-325">To transfer these subscriptions, you will need to [cancel the existing subscription](create-a-new-subscription.md#suspend-or-cancel-a-subscription) and purchase new offer for customer through Indirect Provider.</span></span>

- <span data-ttu-id="36cc8-326">**Kan inte testas med sandbox-miljö.**</span><span class="sxs-lookup"><span data-stu-id="36cc8-326">**Cannot be tested using sandbox environment.**</span></span>

## <a name="enroll-for-indirect-reseller-incentives"></a><span data-ttu-id="36cc8-327">Registrera dig för indirekta åter försäljares incitament</span><span class="sxs-lookup"><span data-stu-id="36cc8-327">Enroll for indirect reseller incentives</span></span>

<span data-ttu-id="36cc8-328">När du har registrerat dig som en indirekt åter försäljare på din befintliga leverantör av direkt fakturerings partner får du en inbjudan om att registrera sig för en indirekt åter försäljares stimulans inom 30 dagar.</span><span class="sxs-lookup"><span data-stu-id="36cc8-328">After you have successfully enrolled as an indirect reseller on your existing direct bill partner tenant, you will receive an invitation to enroll for indirect reseller incentive within 30 days.</span></span> <span data-ttu-id="36cc8-329">Inbjudan baseras på partner MPN-kontot som för närvarande är associerat med din CSP-partners klient.</span><span class="sxs-lookup"><span data-stu-id="36cc8-329">The invitation is based on the partner MPN account that is currently associated with your CSP partner tenant.</span></span> <span data-ttu-id="36cc8-330">Inbjudan skickas till den e-postadress som är kopplad till partner MPN-kontot.</span><span class="sxs-lookup"><span data-stu-id="36cc8-330">The invitation will be sent to the email address associated with the partner MPN account.</span></span>

<span data-ttu-id="36cc8-331">Du är också berättigad till att registrera sig för direkt fakturerings program med samma partner klient organisation.</span><span class="sxs-lookup"><span data-stu-id="36cc8-331">You are also eligible to enroll for direct bill incentive programs with that same partner tenant.</span></span> <span data-ttu-id="36cc8-332">Du måste hantera programmen separat.</span><span class="sxs-lookup"><span data-stu-id="36cc8-332">You must manage the programs separately.</span></span>

## <a name="next-steps"></a><span data-ttu-id="36cc8-333">Nästa steg</span><span class="sxs-lookup"><span data-stu-id="36cc8-333">Next steps</span></span>

- [<span data-ttu-id="36cc8-334">Ytterligare information om att bli en indirekt åter försäljare</span><span class="sxs-lookup"><span data-stu-id="36cc8-334">Additional information on becoming an indirect reseller</span></span>](https://assetsprod.microsoft.com/csp-directbill-to-indirect-transition.pdf)
- [<span data-ttu-id="36cc8-335">CSP Direct-partner nya krav</span><span class="sxs-lookup"><span data-stu-id="36cc8-335">CSP direct partner new requirements</span></span>](direct-partner-new-requirements.md)
- [<span data-ttu-id="36cc8-336">Begränsade direkta fakturerings funktioner</span><span class="sxs-lookup"><span data-stu-id="36cc8-336">Restricted direct bill capabilities</span></span>](restricted-direct-bill-capabilities.md)