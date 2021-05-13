---
title: Byta partner för direktfakturering till indirekt återförsäljare
ms.topic: how-to
ms.date: 06/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Lär dig hur en CSP-programpartner kan använda PartnerCenter för att övergå från direktfaktureringspartner till indirekt återförsäljare.
author: aarzh-AaronZhang
ms.author: v-aarzh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: e57ae5a30e3ee4331ae509a0650d09baf4a82590
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 05/13/2021
ms.locfileid: "109854901"
---
# <a name="transition-from-cloud-solution-provider-csp-direct-bill-partner-to-csp-indirect-reseller"></a><span data-ttu-id="5e4f5-103">Övergå från en CSP-partner med direktfakturering till en indirekt CSP-återförsäljare</span><span class="sxs-lookup"><span data-stu-id="5e4f5-103">Transition from Cloud Solution Provider (CSP) direct bill partner to CSP indirect reseller</span></span>

<span data-ttu-id="5e4f5-104">**Lämpliga roller:** Global administratör</span><span class="sxs-lookup"><span data-stu-id="5e4f5-104">**Appropriate roles**: Global admin</span></span>

>[!Note]
><span data-ttu-id="5e4f5-105">Den här artikeln är avsedd för direktfaktureringspartner som har valt att övergå till indirekta återförsäljare.</span><span class="sxs-lookup"><span data-stu-id="5e4f5-105">This article is intended for direct bill partners who have decided to transition to indirect resellers.</span></span> <span data-ttu-id="5e4f5-106">Men även om du ännu inte har gjort ett uttryckligt beslut om att registrera [](direct-partner-new-requirements.md) dig som en indirekt återförsäljare, kommer direktfaktureringspartner som inte uppfyller de nya kraven för CSP:s partnerprogram för direktfakturering att informeras av Microsoft när deras direktfaktureringsfunktioner kommer att [begränsas.](restricted-direct-bill-capabilities.md)</span><span class="sxs-lookup"><span data-stu-id="5e4f5-106">However, even if you have not made an explicit decision yet to enroll as an indirect reseller, direct bill partners who do not meet the new [requirements](direct-partner-new-requirements.md) for the CSP direct bill partner program will be informed by Microsoft when their [direct bill capabilities will be restricted](restricted-direct-bill-capabilities.md).</span></span>
<br><span data-ttu-id="5e4f5-107">Från och med januari 2021 kommer ett nytt intäktskrav att läggas till.</span><span class="sxs-lookup"><span data-stu-id="5e4f5-107">As of January 2021, a new revenue requirement will be added.</span></span> <span data-ttu-id="5e4f5-108">Partner som registrerats som en partner med direktfakturering måste ha gjort en överträdelse på minst 300 000 USD i Molnlösningsleverantör-programintäkter på en global partnerkontonivå under de senaste 12 månaderna.</span><span class="sxs-lookup"><span data-stu-id="5e4f5-108">Partners enrolled as a direct bill partner will need to have transacted at least USD$300K in Cloud Solution Provider program revenue at a Partner Global Account level over the previous 12 months.</span></span>

<span data-ttu-id="5e4f5-109">Du kommer att kunna registrera dig i programmet för indirekta återförsäljare med din befintliga klientorganisation för direktfakturering.</span><span class="sxs-lookup"><span data-stu-id="5e4f5-109">You will be able to enroll in the indirect reseller program using your existing direct bill tenant.</span></span>

## <a name="get-started"></a><span data-ttu-id="5e4f5-110">Kom igång</span><span class="sxs-lookup"><span data-stu-id="5e4f5-110">Get started</span></span>

1. <span data-ttu-id="5e4f5-111">Kontrollera att din partnerprofil i Partnercenter och MPN-ID är aktuella.</span><span class="sxs-lookup"><span data-stu-id="5e4f5-111">Make sure your partner profile in Partner Center and MPN ID are current.</span></span>

2. <span data-ttu-id="5e4f5-112">Logga in på Partner Center som global administratör för den klientorganisation för direktfakturering som du övergår till en indirekt återförsäljare.</span><span class="sxs-lookup"><span data-stu-id="5e4f5-112">Sign in to Partner Center as the global admin for the direct bill tenant you are transitioning to indirect reseller.</span></span>

   :::image type="content" source="images/direct/direct1.png" alt-text="Översikt":::

3. <span data-ttu-id="5e4f5-114">Granska din partnerinformation i registreringsformuläret.</span><span class="sxs-lookup"><span data-stu-id="5e4f5-114">Review your partner details on the enrollment form.</span></span>

   :::image type="content" source="images/direct/direct2a.png" alt-text="Registrera dig nu":::

4. <span data-ttu-id="5e4f5-116">Välj Registrera nu.</span><span class="sxs-lookup"><span data-stu-id="5e4f5-116">Select Enroll now.</span></span> <span data-ttu-id="5e4f5-117">Din indirekta återförsäljare använder samma AAD-klientorganisation som du använder för din direkta verksamhet.</span><span class="sxs-lookup"><span data-stu-id="5e4f5-117">Your indirect reseller business will use the same AAD tenant you use for your direct business.</span></span>

    > [!NOTE]
    > <span data-ttu-id="5e4f5-118">Den här nya övergångskapaciteten kommer inledningsvis att vara tillgänglig för partner med årsdagen för september till december.</span><span class="sxs-lookup"><span data-stu-id="5e4f5-118">Initially, this new transition capability will be available for partners with September to December anniversary dates.</span></span> <span data-ttu-id="5e4f5-119">Om du inte har något årsdagsdatum mellan september och december ser du inte funktionen just nu.</span><span class="sxs-lookup"><span data-stu-id="5e4f5-119">If you don"t have an anniversary date between September and December, you won't see the capability at this time.</span></span> <span data-ttu-id="5e4f5-120">Partner med årsdagar efter december 2018 meddelas senare när funktionen har aktiverats för partner.</span><span class="sxs-lookup"><span data-stu-id="5e4f5-120">Partners with anniversary dates after December 2018 will be notified later once the feature is enabled for the partners.</span></span>

5. <span data-ttu-id="5e4f5-121">När registreringen har godkänts loggar du in på Partnercenter igen.</span><span class="sxs-lookup"><span data-stu-id="5e4f5-121">When your enrollment is approved, sign in to Partner Center again.</span></span>

    > [!NOTE]
    > <span data-ttu-id="5e4f5-122">Godkännande är vanligtvis omedelbart, men det kan ta upp till fem arbetsdagar.</span><span class="sxs-lookup"><span data-stu-id="5e4f5-122">While approval is usually immediate, it can take up to five business days.</span></span> <span data-ttu-id="5e4f5-123">När den har godkänts får du ett meddelande till den e-postadress som du har angett under den primära kontakten i registreringsformuläret.</span><span class="sxs-lookup"><span data-stu-id="5e4f5-123">Once approved, you will receive a notification to the email address you have specified under primary contact in the enrollment form.</span></span> <span data-ttu-id="5e4f5-124">Du kan också kontrollera din registreringsstatus under **Inställningar**  >  **Kontoinställningar**  >  **Partnerprofil och >** programinformation.</span><span class="sxs-lookup"><span data-stu-id="5e4f5-124">You can also check your enrollment status under **Settings** > **Account Settings** > **Partner Profile** > Program info.</span></span>

6. <span data-ttu-id="5e4f5-125">På **översiktssidan** visas det indirekta återförsäljaravtalet.</span><span class="sxs-lookup"><span data-stu-id="5e4f5-125">On your **Overview** page, you will see the indirect reseller agreement.</span></span> <span data-ttu-id="5e4f5-126">Välj **Acceptera och fortsätt**.</span><span class="sxs-lookup"><span data-stu-id="5e4f5-126">Select **Accept and continue**.</span></span> <span data-ttu-id="5e4f5-127">Den här åtgärden möjliggör funktioner för indirekta återförsäljare.</span><span class="sxs-lookup"><span data-stu-id="5e4f5-127">This action enables the indirect reseller capabilities.</span></span>

<span data-ttu-id="5e4f5-128">När du har accepterat det indirekta återförsäljaravtalet kan du se att din partnerprofil identifierar dig som **både** en direktfakturering och indirekt återförsäljare.</span><span class="sxs-lookup"><span data-stu-id="5e4f5-128">When you have accepted the indirect reseller agreement, notice that your Partner profile identifies you as **both** a direct bill and indirect reseller.</span></span>

:::image type="content" source="images/direct/direct3.png" alt-text="Indirekt återförsäljaravtal":::

> [!IMPORTANT]
> <span data-ttu-id="5e4f5-130">När du registrerar dig som en indirekt återförsäljare med den nya funktionen finns det inget alternativ för att återställa till en klientorganisation med en direkt faktura.</span><span class="sxs-lookup"><span data-stu-id="5e4f5-130">Once you enroll as an indirect reseller using the new capability, there is no option to roll back to a direct bill- only tenant.</span></span> <span data-ttu-id="5e4f5-131">Se till att du utvärderar dina affärsbehov fullständigt innan du registrerar dig som indirekt återförsäljare.</span><span class="sxs-lookup"><span data-stu-id="5e4f5-131">Please make sure that you fully evaluate your business needs before enrolling as an indirect reseller.</span></span>

## <a name="while-you-transition-from-direct-to-indirect-reseller"></a><span data-ttu-id="5e4f5-132">Medan du övergår från direkt till indirekt återförsäljare</span><span class="sxs-lookup"><span data-stu-id="5e4f5-132">While you transition from direct to indirect reseller</span></span>

<span data-ttu-id="5e4f5-133">Under den här fasen fortsätter du att hantera dina direkta kunders prenumerationsbehov, inklusive faktureringsprocessen.</span><span class="sxs-lookup"><span data-stu-id="5e4f5-133">During this phase, you will continue to manage your direct customers' subscription needs including the billing process.</span></span> <span data-ttu-id="5e4f5-134">Du kan också börja acceptera kunder från din indirekta leverantör och arbeta som en indirekt återförsäljare.</span><span class="sxs-lookup"><span data-stu-id="5e4f5-134">You can also begin accepting customers from your Indirect provider and operating as an indirect reseller.</span></span>

:::image type="content" source="images/direct/direct4.png" alt-text="Du är både en direktfakturering och en indirekt återförsäljare":::

## <a name="find-an-indirect-provider"></a><span data-ttu-id="5e4f5-136">Hitta en indirekt leverantör</span><span class="sxs-lookup"><span data-stu-id="5e4f5-136">Find an indirect provider</span></span>

<span data-ttu-id="5e4f5-137">När du har registrerat dig visas en länk till indirekta leverantörer i det vänstra navigeringsfältet.</span><span class="sxs-lookup"><span data-stu-id="5e4f5-137">After enrolling, a link to Indirect providers will appear in your left nav.</span></span> <span data-ttu-id="5e4f5-138">Som indirekt återförsäljare upprättar du en relation med en indirekt leverantör som sedan kan hantera din fakturering, köpa produkter för dina kunder och supportinfrastruktur.</span><span class="sxs-lookup"><span data-stu-id="5e4f5-138">As an indirect reseller you will establish a relationship with an indirect provider who then can handle your billing, purchase products for your customers, and support infrastructure.</span></span>

<span data-ttu-id="5e4f5-139">Olika indirekta leverantörer erbjuder olika support och tjänster, så du bör utvärdera leverantörerna i ditt område för att avgöra vilka som bäst uppfyller dina behov.</span><span class="sxs-lookup"><span data-stu-id="5e4f5-139">Different indirect providers offer different support and services, so you should evaluate the providers in your area to determine which ones best meet your needs.</span></span> <span data-ttu-id="5e4f5-140">I allmänhet kommer de flesta leverantörer att:</span><span class="sxs-lookup"><span data-stu-id="5e4f5-140">Generally, most providers will:</span></span>

- <span data-ttu-id="5e4f5-141">Ge dig teknisk utbildning och hjälp</span><span class="sxs-lookup"><span data-stu-id="5e4f5-141">Provide you with technical training and assistance</span></span>
- <span data-ttu-id="5e4f5-142">Hjälp dig att marknadsföra dina produkter och tjänster</span><span class="sxs-lookup"><span data-stu-id="5e4f5-142">Help you market your products and services</span></span>
- <span data-ttu-id="5e4f5-143">Hantera dina lån och kreditvillkor</span><span class="sxs-lookup"><span data-stu-id="5e4f5-143">Manage your financing and credit terms</span></span>

<span data-ttu-id="5e4f5-144">Sök i listan över officiella [indirekta Microsoft-leverantörer.](https://partnercenter.microsoft.com/partner/find-a-provider)</span><span class="sxs-lookup"><span data-stu-id="5e4f5-144">Search the list of official [Microsoft indirect providers](https://partnercenter.microsoft.com/partner/find-a-provider).</span></span>

<span data-ttu-id="5e4f5-145">Läs mer i Partner  [with indirect providers (Partner med indirekta leverantörer)](indirect-reseller-tasks-in-partner-center.md)</span><span class="sxs-lookup"><span data-stu-id="5e4f5-145">Learn more, read  [Partner with indirect providers](indirect-reseller-tasks-in-partner-center.md)</span></span>

## <a name="accept-a-partnership-invitation-from-your-indirect-provider"></a><span data-ttu-id="5e4f5-146">Acceptera en partnerinbjudan från din indirekta leverantör</span><span class="sxs-lookup"><span data-stu-id="5e4f5-146">Accept a partnership invitation from your indirect provider</span></span>

<span data-ttu-id="5e4f5-147">När du hittar en indirekt leverantör att samarbeta med kan du upprätta ett partnerskap med den indirekta leverantören i Partnercenter.</span><span class="sxs-lookup"><span data-stu-id="5e4f5-147">When you find an indirect provider to partner with, establish a partnership with the indirect provider in Partner Center.</span></span>

<span data-ttu-id="5e4f5-148">Den indirekta provider som du väljer skickar dig via e-post en länk för partnerskapsinbjudan som tar dig till deras inbjudan i Partnercenter.</span><span class="sxs-lookup"><span data-stu-id="5e4f5-148">The indirect provider you select will send you in email a partnership invitation link that will take you to their invitation in Partner Center.</span></span> <span data-ttu-id="5e4f5-149">Se till att din globala administratör loggar in på Partnercenter och följer inbjudningslänken.</span><span class="sxs-lookup"><span data-stu-id="5e4f5-149">Be sure your global admin signs in to Partner Center and follows the invitation link.</span></span> <span data-ttu-id="5e4f5-150">När du godkänner inbjudan visas leverantörens namn i listan över indirekta leverantörer.</span><span class="sxs-lookup"><span data-stu-id="5e4f5-150">When you accept the invitation, the provider's name will appear in your indirect provider list.</span></span>

## <a name="acquire-new-customers-as-indirect-reseller"></a><span data-ttu-id="5e4f5-151">Skaffa nya kunder som indirekt återförsäljare</span><span class="sxs-lookup"><span data-stu-id="5e4f5-151">Acquire new customers as indirect reseller</span></span>

<span data-ttu-id="5e4f5-152">Både du och din indirekta leverantör måste ha återförsäljarrelationer med kunder.</span><span class="sxs-lookup"><span data-stu-id="5e4f5-152">Both you and your indirect provider need to have reseller relationships with customers.</span></span> <span data-ttu-id="5e4f5-153">Med dessa återförsäljarrelationer kan du hantera en kunds prenumerationer och tjänster för deras räkning.</span><span class="sxs-lookup"><span data-stu-id="5e4f5-153">These reseller relationships enable you to manage a customer's subscriptions and services on their behalf.</span></span> <span data-ttu-id="5e4f5-154">Om du vill skaffa en ny kund som har en befintlig Azure AD-klientorganisation kan du bjuda in kunden att upprätta en återförsäljarrelation med både dig och leverantören på samma gång.</span><span class="sxs-lookup"><span data-stu-id="5e4f5-154">To acquire a new customer who has an existing Azure AD tenant, you can invite the customer to establish a reseller relationship with both you and your provider at the same time.</span></span>

<span data-ttu-id="5e4f5-155">Så här skapar du en indirekt återförsäljarinbjudan:</span><span class="sxs-lookup"><span data-stu-id="5e4f5-155">To create an indirect reseller invitation:</span></span>

1. <span data-ttu-id="5e4f5-156">Välj **Indirekta leverantörer i** det vänstra navigeringsfältet i Partnercenter.</span><span class="sxs-lookup"><span data-stu-id="5e4f5-156">Select **Indirect providers** from your Partner Center left nav.</span></span>

2. <span data-ttu-id="5e4f5-157">Välj **Bjud in nya** kunder att bjuda in en kund att upprätta en återförsäljarrelation med både dig och den indirekta leverantören på samma gång.</span><span class="sxs-lookup"><span data-stu-id="5e4f5-157">Select **Invite new customers** to invite a customer to establish a reseller relationship with both you and the indirect provider at the same time.</span></span> <span data-ttu-id="5e4f5-158">Leverantören måste ha en återförsäljarrelation med kunden så att de kan skicka beställningar åt kunden när kunden vill köpa nya prenumerationer eller lägga till nya licenser i befintliga prenumerationer.</span><span class="sxs-lookup"><span data-stu-id="5e4f5-158">The provider needs to have a reseller relationship with your customer, so they can submit orders on your customer's behalf when the customer wants to buy new subscriptions or add new licenses to existing subscriptions.</span></span>

3. <span data-ttu-id="5e4f5-159">På nästa sida granskar du utkastet till e-postmeddelandet.</span><span class="sxs-lookup"><span data-stu-id="5e4f5-159">On the next page, review the draft email message.</span></span> <span data-ttu-id="5e4f5-160">Du kan öppna utkastmeddelandet i ett e-postmeddelande eller kopiera meddelandet till Urklipp och klistra in det i ett e-postmeddelande.</span><span class="sxs-lookup"><span data-stu-id="5e4f5-160">You can open the draft message in email, or you can copy the message to your clipboard and paste it into an email.</span></span>

4. <span data-ttu-id="5e4f5-161">Redigera texten i e-postmeddelandet för att säga vad du behöver, men se till att inkludera länken eftersom den är anpassad för att ansluta kunden direkt till både ditt konto och leverantörens konto.</span><span class="sxs-lookup"><span data-stu-id="5e4f5-161">Edit the text in the email to say what you need but be sure to include the link as it is personalized to connect the customer directly to both your account and your provider's account.</span></span> <span data-ttu-id="5e4f5-162">Välj sedan **Done** (Klar).</span><span class="sxs-lookup"><span data-stu-id="5e4f5-162">Then select **Done**.</span></span>

5. <span data-ttu-id="5e4f5-163">När kunden ger dig och din leverantör tillstånd att bli återförsäljare av posten, har du administratörsbehörighet att hantera deras prenumerationer, licenser och användare för deras räkning, och din indirekta leverantör kommer att kunna skicka beställningar för deras räkning.</span><span class="sxs-lookup"><span data-stu-id="5e4f5-163">After the customer authorizes you and your provider to be their resellers of record, you'll have administrator permissions to manage their subscriptions, licenses, and users on their behalf, and your indirect provider will be able to submit orders on their behalf.</span></span>
6. <span data-ttu-id="5e4f5-164">Om du vill hantera kundens konto, tjänster, användare och licenser expanderar du kundens post genom att välja nedåtpilen nära kundens namn.</span><span class="sxs-lookup"><span data-stu-id="5e4f5-164">To manage the customer's account, services, users, and licenses, expand the customer's record by selecting the down arrow near their name.</span></span>

<span data-ttu-id="5e4f5-165">Till skillnad från partner med direktfakturering kan indirekta återförsäljare inte skapa Azure AD-klienter för sina nya kunder i Partnercenter.</span><span class="sxs-lookup"><span data-stu-id="5e4f5-165">Unlike direct bill partners, indirect resellers can't create Azure AD tenants for their new customers in Partner Center.</span></span> <span data-ttu-id="5e4f5-166">Leverantören skapar klienten och anger dig som indirekt återförsäljare för den här kunden.</span><span class="sxs-lookup"><span data-stu-id="5e4f5-166">Your provider will create the tenant and will specify you as the indirect reseller for this customer.</span></span> <span data-ttu-id="5e4f5-167">Detta säkerställer att kunden visas i kundlistan i Partnercenter.</span><span class="sxs-lookup"><span data-stu-id="5e4f5-167">This ensures that the customer will appear in your customer list in Partner Center.</span></span>

>[!Note]
><span data-ttu-id="5e4f5-168">Du kommer inte att kunna använda din direktfaktureringsfunktion för att skapa inköp för kunder som du skaffar som en indirekt återförsäljare.</span><span class="sxs-lookup"><span data-stu-id="5e4f5-168">You will not be able to use your direct bill capability to create purchases for customers you acquire as an indirect reseller.</span></span>

## <a name="managing-your-direct-bill-customers-and-your-indirect-reseller-customers"></a><span data-ttu-id="5e4f5-169">Hantera dina direktfaktureringskunder och dina indirekta återförsäljares kunder</span><span class="sxs-lookup"><span data-stu-id="5e4f5-169">Managing your direct bill customers and your indirect reseller customers</span></span>

<span data-ttu-id="5e4f5-170">Du hanterar dina direktfaktureringskunder och dina indirekta återförsäljares kunder på olika sätt.</span><span class="sxs-lookup"><span data-stu-id="5e4f5-170">You manage your direct bill customers and your indirect reseller customers differently.</span></span>

### <a name="direct-bill-customers-things-you-wont-do-as-an-indirect-reseller"></a><span data-ttu-id="5e4f5-171">Fakturera kunder direkt (saker som du inte kommer att göra som indirekt återförsäljare)</span><span class="sxs-lookup"><span data-stu-id="5e4f5-171">Direct bill customers (things you won't do as an indirect reseller)</span></span>

- <span data-ttu-id="5e4f5-172">Skapa beställningar av produkter</span><span class="sxs-lookup"><span data-stu-id="5e4f5-172">Create orders for products</span></span>
- <span data-ttu-id="5e4f5-173">Hantera Azure-reservationer</span><span class="sxs-lookup"><span data-stu-id="5e4f5-173">Manage Azure reservations</span></span>
- <span data-ttu-id="5e4f5-174">Hantera sin orderhistorik</span><span class="sxs-lookup"><span data-stu-id="5e4f5-174">Manage their order history</span></span>
- <span data-ttu-id="5e4f5-175">Köpa programvara</span><span class="sxs-lookup"><span data-stu-id="5e4f5-175">Purchase software</span></span>
- <span data-ttu-id="5e4f5-176">Fakturera kunder direkt</span><span class="sxs-lookup"><span data-stu-id="5e4f5-176">Bill customers directly</span></span>

### <a name="indirect-reseller-customers"></a><span data-ttu-id="5e4f5-177">Indirekta återförsäljares kunder</span><span class="sxs-lookup"><span data-stu-id="5e4f5-177">Indirect reseller customers</span></span>

- <span data-ttu-id="5e4f5-178">Din indirekta leverantör beställer produkter åt dina kunder</span><span class="sxs-lookup"><span data-stu-id="5e4f5-178">Your indirect provider orders products for your customers</span></span>
- <span data-ttu-id="5e4f5-179">Hantera kunders licenser och användare</span><span class="sxs-lookup"><span data-stu-id="5e4f5-179">Manage customers' licenses and users</span></span>
- <span data-ttu-id="5e4f5-180">Hantera prenumerationsförnyelse</span><span class="sxs-lookup"><span data-stu-id="5e4f5-180">Handle subscription renewals</span></span>

### <a name="to-identify-customers-that-you-acquired-as-a-direct-bill-partner"></a><span data-ttu-id="5e4f5-181">Identifiera kunder som du har köpt som partner för direktfakturering</span><span class="sxs-lookup"><span data-stu-id="5e4f5-181">To identify customers that you acquired as a direct bill partner</span></span>

1. <span data-ttu-id="5e4f5-182">Välj **Kunder**.</span><span class="sxs-lookup"><span data-stu-id="5e4f5-182">Select **Customers**.</span></span>

2. <span data-ttu-id="5e4f5-183">Välj en kund för att visa information.</span><span class="sxs-lookup"><span data-stu-id="5e4f5-183">Select a customer to view their details.</span></span>

3. <span data-ttu-id="5e4f5-184">Om kunden är en kund som du har köpt  som direktfaktureringspartner visas alternativ för att lägga till **eller** visa produkter, och du ser deras prenumerationer.</span><span class="sxs-lookup"><span data-stu-id="5e4f5-184">If this customer is one you acquired as a direct bill partner, you will see options to **add** or **view products** and you will see their subscriptions.</span></span>

4. <span data-ttu-id="5e4f5-185">Om kunden har en indirekt återförsäljarrelation med dig är dessa alternativ inte tillgängliga.</span><span class="sxs-lookup"><span data-stu-id="5e4f5-185">If the customer has an indirect reseller relationship with you, those options will not be available.</span></span>

## <a name="move-your-direct-bill-customers-to-your-indirect-provider"></a><span data-ttu-id="5e4f5-186">Flytta dina direktfaktureringskunder till din indirekta leverantör</span><span class="sxs-lookup"><span data-stu-id="5e4f5-186">Move your direct bill customers to your indirect provider</span></span>

<span data-ttu-id="5e4f5-187">Din indirekta leverantör kan inte skicka beställningar eller befintliga prenumerationsöverföringar för dina befintliga direktfaktureringskunder förrän de har en återförsäljarrelation med dem.</span><span class="sxs-lookup"><span data-stu-id="5e4f5-187">Your indirect provider cannot submit orders or existing subscription transfers for your existing direct bill customers until they have a reseller relationship with them.</span></span> <span data-ttu-id="5e4f5-188">Om du vill upprätta återförsäljarrelationen mellan din indirekta leverantör och din befintliga direktfaktureringskund kan du använda någon av följande metoder:</span><span class="sxs-lookup"><span data-stu-id="5e4f5-188">To establish the reseller relationship between your indirect provider and your existing direct bill customer, you can use one of the following methods:</span></span>

- [<span data-ttu-id="5e4f5-189">Tillägg för återförsäljarrelation</span><span class="sxs-lookup"><span data-stu-id="5e4f5-189">Reseller relationship extension</span></span>](#reseller-relationship-extension)

- [<span data-ttu-id="5e4f5-190">Skicka en indirekt återförsäljarinbjudan till kunden</span><span class="sxs-lookup"><span data-stu-id="5e4f5-190">Send an indirect reseller invitation to the customer</span></span>](#send-an-indirect-reseller-invitation-to-the-customer)

<span data-ttu-id="5e4f5-191">Du hittar en detaljerad översikt över den stegvisa processen i dokumentet [Direkt till indirekt övergång](https://partner.microsoft.com/resources/collection/Direct-Bill-transition-to-Indirect-reseller#/)</span><span class="sxs-lookup"><span data-stu-id="5e4f5-191">You can find a detailed overview of the step-by-step process in the [Direct to indirect transition document](https://partner.microsoft.com/resources/collection/Direct-Bill-transition-to-Indirect-reseller#/)</span></span>

### <a name="reseller-relationship-extension"></a><span data-ttu-id="5e4f5-192">Tillägg för återförsäljarrelation</span><span class="sxs-lookup"><span data-stu-id="5e4f5-192">Reseller relationship extension</span></span>

<span data-ttu-id="5e4f5-193">Du kan använda funktionen för tillägget för återförsäljarrelationer för att upprätta återförsäljarrelationer mellan dina befintliga direktfaktureringskunder och din indirekta leverantör med hjälp av instrumentpanelen i Partnercenter.</span><span class="sxs-lookup"><span data-stu-id="5e4f5-193">You can use the reseller relationship extension feature to establish reseller relationship between your existing direct bill customers and your indirect provider using Partner Center Dashboard.</span></span> <span data-ttu-id="5e4f5-194">Observera följande innan du använder funktionen:</span><span class="sxs-lookup"><span data-stu-id="5e4f5-194">Before using the feature, note the following:</span></span>

- <span data-ttu-id="5e4f5-195">Den här funktionen är endast tillgänglig för direktfaktureringspartner som övergår till att bli en indirekt återförsäljare har slutfört registreringen [av den indirekta återförsäljaren.](#get-started)</span><span class="sxs-lookup"><span data-stu-id="5e4f5-195">This feature is only available to direct bill partners who are transitioning to become an indirect reseller have completed the [indirect reseller enrollment](#get-started).</span></span>

- <span data-ttu-id="5e4f5-196">Du kan bara använda den här funktionen på befintliga direktfaktureringskunder.</span><span class="sxs-lookup"><span data-stu-id="5e4f5-196">You can only apply this feature to existing direct bill customers.</span></span> <span data-ttu-id="5e4f5-197">Det gäller inte för indirekta [återförsäljares kunder.](#acquire-new-customers-as-indirect-reseller)</span><span class="sxs-lookup"><span data-stu-id="5e4f5-197">It is not applicable to [indirect reseller customers](#acquire-new-customers-as-indirect-reseller).</span></span>

- <span data-ttu-id="5e4f5-198">Du kan bara välja en indirekt leverantör som du har accepterat [en partnerinbjudan från din indirekta leverantör för.](#accept-a-partnership-invitation-from-your-indirect-provider)</span><span class="sxs-lookup"><span data-stu-id="5e4f5-198">You can only select an indirect provider for which you have [accepted a partner invitation from your indirect provider](#accept-a-partnership-invitation-from-your-indirect-provider).</span></span>

- <span data-ttu-id="5e4f5-199">En kopia av faktureringsinformationen för den här kunden görs tillgänglig för den indirekta leverantören.</span><span class="sxs-lookup"><span data-stu-id="5e4f5-199">A copy of the bill-to info you have for this customer will be made available to the indirect provider.</span></span> <span data-ttu-id="5e4f5-200">Du kan komma åt faktureringsinformationen genom att gå till kontosidan för den här kunden i Partnercenter-instrumentpanelen.</span><span class="sxs-lookup"><span data-stu-id="5e4f5-200">You can access the bill-to info by accessing the Account page for this customer in Partner Center Dashboard.</span></span>

    > [!NOTE]
    > <span data-ttu-id="5e4f5-201">Genom att använda tilläggsfunktionen för återförsäljarrelationer samtycker du till att dela den fakturainformation som du har för den här kunden med den indirekta leverantören.</span><span class="sxs-lookup"><span data-stu-id="5e4f5-201">By using the reseller relationship extension feature, you consent to sharing the bill-to info you have for this customer with the indirect provider.</span></span>

- <span data-ttu-id="5e4f5-202">Din indirekta provider får inte delegerade [administrationsbehörigheter till](customers-revoke-admin-privileges.md) kundens klientorganisation.</span><span class="sxs-lookup"><span data-stu-id="5e4f5-202">Your indirect provider will not be provided with [delegated administration privileges](customers-revoke-admin-privileges.md) to the customer tenant.</span></span> <span data-ttu-id="5e4f5-203">Om din indirekta leverantör kräver delegerade administrationsbehörigheter måste du skicka en indirekt återförsäljarinbjudan till kunden i stället.</span><span class="sxs-lookup"><span data-stu-id="5e4f5-203">If your indirect provider requires delegated administration privileges, you must send an indirect reseller invitation to the customer instead.</span></span>

- <span data-ttu-id="5e4f5-204">När återförsäljarrelationen har upprättats visas den indirekta leverantören som CSP-partner för kunden under sidan Partnerrelationer i [Microsoft 365 administrationscenter](https://admin.microsoft.com/AdminPortal/Home#/partners) [och Microsoft Store för företag](/microsoft-store/work-with-partner-microsoft-store-business).</span><span class="sxs-lookup"><span data-stu-id="5e4f5-204">Once the reseller relationship is established, the indirect provider will appear as a CSP partner to the customer under the Partner Relationships page in [Microsoft 365 Admin Center](https://admin.microsoft.com/AdminPortal/Home#/partners) and [Microsoft Store for Business](/microsoft-store/work-with-partner-microsoft-store-business).</span></span>

    > [!IMPORTANT]
    > <span data-ttu-id="5e4f5-205">För att undvika förvirring och förvirring godkänns du enligt ditt partneravtal för att informera och få medgivande från direktfaktureringskunden innan du använder relationstilläggsfunktionen för att upprätta en återförsäljarrelation mellan en befintlig direktfaktureringskund och en indirekt leverantör.</span><span class="sxs-lookup"><span data-stu-id="5e4f5-205">To avoid confusion and misunderstanding, you are contractually obliged by your partner agreement to inform and obtain consent from the direct bill customer before you use the relationship extension feature to establish reseller relationship between an existing direct bill customer and an indirect provider.</span></span>

<span data-ttu-id="5e4f5-206">Så här använder du den här funktionen på en befintlig kundklientorganisation:</span><span class="sxs-lookup"><span data-stu-id="5e4f5-206">To use this feature on an existing customer tenant:</span></span>

1. <span data-ttu-id="5e4f5-207">Logga in på Partner Center som **administratörsagent.**</span><span class="sxs-lookup"><span data-stu-id="5e4f5-207">Log in to Partner Center as an **Admin Agent**.</span></span>

2. <span data-ttu-id="5e4f5-208">På sidan **Kunder väljer** du en befintlig kund och klickar på ikonen **Snabblänkar** för att expandera sammanfattningsvyn för kunden.</span><span class="sxs-lookup"><span data-stu-id="5e4f5-208">In the **Customers page**, select an existing customer and click on its **Quick links** icon to expand the summary view of the customer.</span></span>

3. <span data-ttu-id="5e4f5-209">Under **Indirekta leverantörer klickar du på** Överför kund på en indirekt **leverantör.**</span><span class="sxs-lookup"><span data-stu-id="5e4f5-209">Under **Indirect provider(s)**, click **Transfer customer on an indirect provider**.</span></span>

    :::image type="content" source="images/direct/direct5-1.png" alt-text="Överföra kunden till en indirekt leverantör":::

4. <span data-ttu-id="5e4f5-211">I popup-dialogrutan väljer du den **indirekta leverantör** som du vill ha återförsäljarrelation med kunden.</span><span class="sxs-lookup"><span data-stu-id="5e4f5-211">In the pop-up dialog, select the **Indirect Provider** you would like to have reseller relationship with the customer.</span></span>

5. <span data-ttu-id="5e4f5-212">Klicka **på Spara och fortsätt**.</span><span class="sxs-lookup"><span data-stu-id="5e4f5-212">Click **Save and continue**.</span></span>

6. <span data-ttu-id="5e4f5-213">Kontrollera att den valda indirekta providern visas under **Indirekta leverantörer.**</span><span class="sxs-lookup"><span data-stu-id="5e4f5-213">Verify the selected indirect provider shows up under **Indirect provider(s)**.</span></span>

    :::image type="content" source="images/direct/direct5-2.png" alt-text="Indirekt leverantör listad":::

### <a name="send-an-indirect-reseller-invitation-to-the-customer"></a><span data-ttu-id="5e4f5-215">Skicka en indirekt återförsäljarinbjudan till kunden</span><span class="sxs-lookup"><span data-stu-id="5e4f5-215">Send an indirect reseller invitation to the customer</span></span>

<span data-ttu-id="5e4f5-216">Din indirekta leverantör kan inte skicka beställningar för dina befintliga direktfaktureringskunder förrän de har en återförsäljarrelation med dem.</span><span class="sxs-lookup"><span data-stu-id="5e4f5-216">Your indirect provider cannot submit orders for your existing direct bill customers until they have a reseller relationship with them.</span></span> <span data-ttu-id="5e4f5-217">Om du vill upprätta återförsäljarrelationen mellan dina befintliga kunder och din indirekta leverantör bjuder du in kunden med hjälp av en indirekt återförsäljarinbjudan.</span><span class="sxs-lookup"><span data-stu-id="5e4f5-217">To establish the reseller relationship between your existing customers and your indirect provider, invite the customer using an indirect reseller invitation.</span></span>

1. <span data-ttu-id="5e4f5-218">Välj **Indirekta leverantörer** i det vänstra navigeringsfältet i Partnercenter.</span><span class="sxs-lookup"><span data-stu-id="5e4f5-218">Select **Indirect providers** from your Partner Center left nav.</span></span>

2. <span data-ttu-id="5e4f5-219">Välj **Bjud in nya** kunder att bjuda in en kund att upprätta en återförsäljarrelation med både dig och den indirekta leverantören på samma gång.</span><span class="sxs-lookup"><span data-stu-id="5e4f5-219">Select **Invite new customers** to invite a customer to establish a reseller relationship with both you and the indirect provider at the same time.</span></span> <span data-ttu-id="5e4f5-220">Leverantören måste ha en återförsäljarrelation med kunden så att de kan skicka beställningar för kundens räkning när kunden vill köpa nya prenumerationer eller lägga till nya licenser i befintliga prenumerationer.</span><span class="sxs-lookup"><span data-stu-id="5e4f5-220">The provider needs to have a reseller relationship with your customer, so they can submit orders on your customer's behalf when the customer wants to buy new subscriptions or add new licenses to existing subscriptions.</span></span>

    :::image type="content" source="images/direct/direct6.png" alt-text="Bjud in nya kunder":::

3. <span data-ttu-id="5e4f5-222">På nästa sida granskar du utkastet till e-postmeddelandet.</span><span class="sxs-lookup"><span data-stu-id="5e4f5-222">On the next page, review the draft email message.</span></span> <span data-ttu-id="5e4f5-223">Du kan öppna utkastmeddelandet i ett e-postmeddelande eller kopiera meddelandet till Urklipp och klistra in det i ett e-postmeddelande.</span><span class="sxs-lookup"><span data-stu-id="5e4f5-223">You can open the draft message in email, or you can copy the message to your clipboard and paste it into an email.</span></span>

4. <span data-ttu-id="5e4f5-224">Redigera texten i e-postmeddelandet för att säga vad du behöver, men se till att inkludera länken eftersom den är anpassad för att ansluta kunden direkt till både ditt konto och leverantörens konto.</span><span class="sxs-lookup"><span data-stu-id="5e4f5-224">Edit the text in the email to say what you need but be sure to include the link as it is personalized to connect the customer directly to both your account and your provider's account.</span></span> <span data-ttu-id="5e4f5-225">Välj sedan **Done** (Klar).</span><span class="sxs-lookup"><span data-stu-id="5e4f5-225">Then select **Done**.</span></span>

5. <span data-ttu-id="5e4f5-226">När kunden har godkänt dig och din leverantör att bli återförsäljare av posten, har du administratörsbehörighet att hantera deras prenumerationer, licenser och användare för deras räkning, och din indirekta leverantör kommer att kunna skicka beställningar för deras räkning.</span><span class="sxs-lookup"><span data-stu-id="5e4f5-226">After the customer authorizes you and your provider to be their resellers of record, you'll have administrator permissions to manage their subscriptions, licenses, and users on their behalf, and your indirect provider will be able to submit orders on their behalf.</span></span>

6. <span data-ttu-id="5e4f5-227">Om du vill hantera kundens konto, tjänster, användare och licenser expanderar du kundens post genom att välja nedåtpilen nära kundens namn.</span><span class="sxs-lookup"><span data-stu-id="5e4f5-227">To manage the customer's account, services, users, and licenses, expand the customer's record by selecting the down arrow near their name.</span></span>

### <a name="microsoft-customer-agreement-acceptance"></a><span data-ttu-id="5e4f5-228">Microsoft-kundavtal godkännande</span><span class="sxs-lookup"><span data-stu-id="5e4f5-228">Microsoft Customer Agreement acceptance</span></span>

<span data-ttu-id="5e4f5-229">Microsoft Cloud-avtal är giltig fram till den 31 januari 2020.</span><span class="sxs-lookup"><span data-stu-id="5e4f5-229">Microsoft Cloud Agreement is valid until January 31, 2020.</span></span> <span data-ttu-id="5e4f5-230">Efter det datumet måste alla kunder, befintliga och nya, signera den nya [Microsoft-kundavtal](confirm-customer-agreement.md).</span><span class="sxs-lookup"><span data-stu-id="5e4f5-230">After that date, all customers, existing and new, must sign the new [Microsoft Customer Agreement](confirm-customer-agreement.md).</span></span> <span data-ttu-id="5e4f5-231">För kunder som övergår, om:</span><span class="sxs-lookup"><span data-stu-id="5e4f5-231">For transitioning customers, if:</span></span>

- <span data-ttu-id="5e4f5-232">**Kunden har inte godkänt Microsoft-kundavtal ännu**</span><span class="sxs-lookup"><span data-stu-id="5e4f5-232">**Customer has not accepted Microsoft Customer Agreement yet**</span></span>

   <span data-ttu-id="5e4f5-233">Kontakta den indirekta leverantören så att kunden [accepterar Microsoft-kundavtal](confirm-customer-agreement.md).</span><span class="sxs-lookup"><span data-stu-id="5e4f5-233">Please work with Indirect Provider to have customer [accept the Microsoft Customer Agreement](confirm-customer-agreement.md).</span></span>

- <span data-ttu-id="5e4f5-234">**Kunden har accepterat Microsoft-kundavtal med dig via Microsoft 365 Administrationscenter**</span><span class="sxs-lookup"><span data-stu-id="5e4f5-234">**Customer has accepted Microsoft Customer Agreement with you through the Microsoft 365 Admin Center**</span></span>

   <span data-ttu-id="5e4f5-235">Godkännandet behålls när återförsäljarrelationen har upprättats med den indirekta leverantören.</span><span class="sxs-lookup"><span data-stu-id="5e4f5-235">The acceptance will be retained once the reseller relationship is established with the Indirect Provider.</span></span> <span data-ttu-id="5e4f5-236">Du behöver inte göra något.</span><span class="sxs-lookup"><span data-stu-id="5e4f5-236">There is nothing you need to do.</span></span>

- <span data-ttu-id="5e4f5-237">**Kunden har accepterat Microsoft-kundavtal med dig via attestationering av partner**</span><span class="sxs-lookup"><span data-stu-id="5e4f5-237">**Customer has accepted Microsoft Customer Agreement with you through partner attestation**</span></span>

   <span data-ttu-id="5e4f5-238">Godkännandet behålls inte.</span><span class="sxs-lookup"><span data-stu-id="5e4f5-238">The acceptance will not be retained.</span></span> <span data-ttu-id="5e4f5-239">Kontakta den indirekta leverantören för [att uppdatera kundens godkännande i Partnercenter.](confirm-customer-agreement.md#confirm-customer-acceptance-for-existing-customers)</span><span class="sxs-lookup"><span data-stu-id="5e4f5-239">Please work with Indirect Provider to [update the customer's acceptance in Partner Center](confirm-customer-agreement.md#confirm-customer-acceptance-for-existing-customers).</span></span>

## <a name="transfer-existing-direct-bill-subscriptions-to-indirect-provider"></a><span data-ttu-id="5e4f5-240">Överföra befintliga prenumerationer på direktfakturering till indirekt leverantör</span><span class="sxs-lookup"><span data-stu-id="5e4f5-240">Transfer existing direct bill subscriptions to indirect provider</span></span>

<span data-ttu-id="5e4f5-241">Under en indirekt CSP-modell har indirekta återförsäljare inte faktureringsrelationer med Microsoft.</span><span class="sxs-lookup"><span data-stu-id="5e4f5-241">Under CSP indirect model, indirect resellers do not have billing relationships with Microsoft.</span></span> <span data-ttu-id="5e4f5-242">I stället får indirekta återförsäljare prenumerationer åt sina kunder via sina indirekta leverantörer.</span><span class="sxs-lookup"><span data-stu-id="5e4f5-242">Instead, indirect resellers obtain subscriptions for their customers through their indirect providers.</span></span> <span data-ttu-id="5e4f5-243">När du övergår från partner för direktfakturering till indirekt återförsäljare måste du överföra de befintliga prenumerationer som du har som partner för direktfakturering till din indirekta leverantör.</span><span class="sxs-lookup"><span data-stu-id="5e4f5-243">While transitioning from direct bill partner to indirect reseller, you need to transfer the existing subscriptions you have as the direct bill partner to your indirect provider.</span></span> <span data-ttu-id="5e4f5-244">Du kan använda funktionen för överföring av självbetjänad prenumeration på instrumentpanelen i Partnercenter för att göra det.</span><span class="sxs-lookup"><span data-stu-id="5e4f5-244">You can use the self-served subscription transfer feature in Partner Center Dashboard to do so.</span></span>

### <a name="prerequisites"></a><span data-ttu-id="5e4f5-245">Förutsättningar</span><span class="sxs-lookup"><span data-stu-id="5e4f5-245">Prerequisites</span></span>

- <span data-ttu-id="5e4f5-246">Den här funktionen är endast tillgänglig för övergångspartner som har slutfört registreringen av den indirekta återförsäljaren med sina befintliga partnerklienter för direktfakturering.</span><span class="sxs-lookup"><span data-stu-id="5e4f5-246">This feature is only available to transitioning partners who have completed the indirect reseller enrollment using their existing direct bill partner tenants.</span></span>

- <span data-ttu-id="5e4f5-247">Innan prenumerationer som är kopplade till en viss kund överförs måste den överförande partnern flytta kunden till en indirekt leverantör.</span><span class="sxs-lookup"><span data-stu-id="5e4f5-247">Before transferring subscriptions associated with a given customer, the transitioning partner must move the customer to an indirect provider.</span></span>

- <span data-ttu-id="5e4f5-248">Kunden måste ha [accepterat Microsoft-kundavtal via den indirekta providern](#microsoft-customer-agreement-acceptance).</span><span class="sxs-lookup"><span data-stu-id="5e4f5-248">Customer must have [accepted Microsoft Customer Agreement through the Indirect Provider](#microsoft-customer-agreement-acceptance).</span></span>

### <a name="how-to-transition-to-indirect-reseller-status"></a><span data-ttu-id="5e4f5-249">Så här övergår du till status för indirekt återförsäljare</span><span class="sxs-lookup"><span data-stu-id="5e4f5-249">How to transition to indirect reseller status</span></span>

<span data-ttu-id="5e4f5-250">Funktionen är en 4-stegsprocess där:</span><span class="sxs-lookup"><span data-stu-id="5e4f5-250">The feature is a 4-step process, where:</span></span>

- <span data-ttu-id="5e4f5-251">Övergångspartnern skapar en begäran om prenumerationsöverföring.</span><span class="sxs-lookup"><span data-stu-id="5e4f5-251">The transitioning partner creates a subscription transfer request.</span></span> <span data-ttu-id="5e4f5-252">Begäran innehåller en eller flera befintliga prenumerationer som är associerade med samma kund och adresseras till en indirekt leverantör.</span><span class="sxs-lookup"><span data-stu-id="5e4f5-252">The request contains one or more existing subscriptions associated with the same customer and is addressed to an indirect provider.</span></span>

- <span data-ttu-id="5e4f5-253">Den indirekta leverantören granskar och godkänner (eller avvisar) överföringsbegäran.</span><span class="sxs-lookup"><span data-stu-id="5e4f5-253">The indirect provider reviews and accepts (or reject) the transfer request.</span></span>

- <span data-ttu-id="5e4f5-254">Den indirekta providern verifierar att överföringsbegäran har slutförts.</span><span class="sxs-lookup"><span data-stu-id="5e4f5-254">The indirect provider verifies that the transfer request is complete.</span></span>

- <span data-ttu-id="5e4f5-255">Övergångspartnern verifierar att överföringsbegäran har slutförts.</span><span class="sxs-lookup"><span data-stu-id="5e4f5-255">The transitioning partner verifies that the transfer request is complete.</span></span>

### <a name="transitioning-partner"></a><span data-ttu-id="5e4f5-256">Övergångspartner</span><span class="sxs-lookup"><span data-stu-id="5e4f5-256">Transitioning partner</span></span>

> [!NOTE]
> <span data-ttu-id="5e4f5-257">Du kan också använda [Partner Center API/SDK för](/partner-center/develop/manage-customers) att överföra befintliga prenumerationer till din indirekta leverantör.</span><span class="sxs-lookup"><span data-stu-id="5e4f5-257">You can also use [Partner Center API/SDK](/partner-center/develop/manage-customers) to transfer the existing subscriptions to your indirect provider.</span></span>
>
> - [<span data-ttu-id="5e4f5-258">Hämta en kunds prenumerationers överföringsberättigande</span><span class="sxs-lookup"><span data-stu-id="5e4f5-258">Get a customer's subscriptions transfer eligibility</span></span>](/partner-center/develop/get-customer-s-subscriptions-transfer-eligibility)
> - [<span data-ttu-id="5e4f5-259">Skapa en kunds överföring</span><span class="sxs-lookup"><span data-stu-id="5e4f5-259">Create a customer's transfer</span></span>](/partner-center/develop/create-a-transfer)
> - [<span data-ttu-id="5e4f5-260">Återkalla en kunds överföring</span><span class="sxs-lookup"><span data-stu-id="5e4f5-260">Withdraw a customer's transfer</span></span>](/partner-center/develop/withdraw-a-transfer)
> - [<span data-ttu-id="5e4f5-261">Acceptera en kunds överföring</span><span class="sxs-lookup"><span data-stu-id="5e4f5-261">Accept a customer's transfer</span></span>](/partner-center/develop/accept-a-transfer)
> - [<span data-ttu-id="5e4f5-262">Avvisa en kunds överföring</span><span class="sxs-lookup"><span data-stu-id="5e4f5-262">Reject a Customer's transfer</span></span>](/partner-center/develop/reject-a-transfer)
> - [<span data-ttu-id="5e4f5-263">Hämta en kunds överföringar</span><span class="sxs-lookup"><span data-stu-id="5e4f5-263">Get a customer's transfers</span></span>](/partner-center/develop/get-all-of-a-customer-s-transfers)
> - [<span data-ttu-id="5e4f5-264">Hämta överföringsinformation per ID</span><span class="sxs-lookup"><span data-stu-id="5e4f5-264">Get transfer details by id</span></span>](/partner-center/develop/get-transfer-by-id)

### <a name="transitioning-partner---create-transfer-request"></a><span data-ttu-id="5e4f5-265">Övergångspartner – skapa överföringsbegäran</span><span class="sxs-lookup"><span data-stu-id="5e4f5-265">Transitioning partner - create transfer request</span></span>

<span data-ttu-id="5e4f5-266">Så här skapar du en överföringsbegäran som övergångspartner:</span><span class="sxs-lookup"><span data-stu-id="5e4f5-266">To create a transfer request as the transitioning partner:</span></span>

1. <span data-ttu-id="5e4f5-267">Logga in på Partner Center som **administratörsagent.**</span><span class="sxs-lookup"><span data-stu-id="5e4f5-267">Log in to Partner Center as an **Admin Agent**.</span></span>

2. <span data-ttu-id="5e4f5-268">På sidan **Kunder** väljer du den avsedda kunden och klickar på ikonen Snabblänkar för att expandera sammanfattningsvyn för kunden.</span><span class="sxs-lookup"><span data-stu-id="5e4f5-268">In the **Customers** page, select the intended customer and click on the Quick links icon to expand the summary view of the customer.</span></span>

3. <span data-ttu-id="5e4f5-269">Under **Indirekta leverantörer bekräftar du** att den avsedda indirekta providern visas.</span><span class="sxs-lookup"><span data-stu-id="5e4f5-269">Under **Indirect provider(s)**, confirm that the intended indirect provider is listed.</span></span>

4. <span data-ttu-id="5e4f5-270">Klicka **på Visa prenumerationer.**</span><span class="sxs-lookup"><span data-stu-id="5e4f5-270">Click **View Subscriptions**.</span></span>

5. <span data-ttu-id="5e4f5-271">På sidan **Prenumerationer** letar du upp **Prenumerationsöverföring.**</span><span class="sxs-lookup"><span data-stu-id="5e4f5-271">In the **Subscriptions** page, look for **Subscription Transfer**.</span></span>

6. <span data-ttu-id="5e4f5-272">Under **Prenumerationsöverföring** klickar du på **Begär prenumerationsöverföring.**</span><span class="sxs-lookup"><span data-stu-id="5e4f5-272">Under **Subscription Transfer**, click **Request subscription transfer**.</span></span>

    :::image type="content" source="images/direct/direct8.png" alt-text="Begära prenumerationsöverföring":::

7. <span data-ttu-id="5e4f5-274">I dialogrutan överföringsbegäran väljer du en eller flera prenumerationer som ska överföras.</span><span class="sxs-lookup"><span data-stu-id="5e4f5-274">In the transfer request dialog, select one or more subscriptions to be transferred.</span></span>

    :::image type="content" source="images/direct/direct9.png" alt-text="Skapa överföringsbegäran":::

8. <span data-ttu-id="5e4f5-276">Klicka på **Skapa**.</span><span class="sxs-lookup"><span data-stu-id="5e4f5-276">Click **Create**.</span></span>

9. <span data-ttu-id="5e4f5-277">En begäran om aktiv prenumerationsöverföring visas under **Prenumerationsöverföring.**</span><span class="sxs-lookup"><span data-stu-id="5e4f5-277">An active subscription transfer request will appear under **Subscription Transfer**.</span></span>

    :::image type="content" source="images/direct/direct10.png" alt-text="Lista över överföringsbegäran":::

10. <span data-ttu-id="5e4f5-279">Informera den indirekta leverantören om att du har skapat en begäran om prenumerationsöverföring till dem.</span><span class="sxs-lookup"><span data-stu-id="5e4f5-279">Inform your indirect provider that you have created a subscription transfer request to them.</span></span>

### <a name="indirect-provider---accept-transfer-request"></a><span data-ttu-id="5e4f5-280">Indirekt provider – acceptera överföringsbegäran</span><span class="sxs-lookup"><span data-stu-id="5e4f5-280">Indirect provider - accept transfer request</span></span>

<span data-ttu-id="5e4f5-281">Så här granskar och godkänner du en överföringsbegäran som indirekt leverantör:</span><span class="sxs-lookup"><span data-stu-id="5e4f5-281">To review and accept a transfer request as the indirect provider:</span></span>

1. <span data-ttu-id="5e4f5-282">Logga in på Partnercenter som **administratörsagent** eller **försäljningsagent.**</span><span class="sxs-lookup"><span data-stu-id="5e4f5-282">Log in to Partner Center as an **Admin** Agent or **Sales Agent**.</span></span>

2. <span data-ttu-id="5e4f5-283">På sidan **Kunder** väljer du den avsedda kunden och klickar på ikonen Snabblänkar för att expandera sammanfattningsvyn för kunden.</span><span class="sxs-lookup"><span data-stu-id="5e4f5-283">In the **Customers** page, select the intended customer and click on its Quick links icon to expand the summary view of the customer.</span></span>

3. <span data-ttu-id="5e4f5-284">Under **Indirekta återförsäljare bekräftar du** att den övergångande partnern visas.</span><span class="sxs-lookup"><span data-stu-id="5e4f5-284">Under **Indirect reseller(s)**, confirm the transitioning partner is listed.</span></span>

4. <span data-ttu-id="5e4f5-285">Klicka **på Visa prenumerationer.**</span><span class="sxs-lookup"><span data-stu-id="5e4f5-285">Click **View Subscriptions**.</span></span>

5. <span data-ttu-id="5e4f5-286">På sidan **Prenumerationer** letar du upp **Prenumerationsöverföring.**</span><span class="sxs-lookup"><span data-stu-id="5e4f5-286">In the **Subscriptions** page, look for **Subscription Transfer**.</span></span>

    :::image type="content" source="images/direct/direct11.png" alt-text="Visa överföringsbegäran":::

6. <span data-ttu-id="5e4f5-288">Under **Prenumerationsöverföring** klickar du på den överföringsbegäran som ska granskas.</span><span class="sxs-lookup"><span data-stu-id="5e4f5-288">Under **Subscription Transfer**, click on the transfer request to review.</span></span>

7. <span data-ttu-id="5e4f5-289">Klicka **på Acceptera** **(eller Avvisa)** efter behov.</span><span class="sxs-lookup"><span data-stu-id="5e4f5-289">Click **Accept** (or **Reject**) as appropriate.</span></span>

    :::image type="content" source="images/direct/direct12.png" alt-text="Acceptera överföringsbegäran":::

8. <span data-ttu-id="5e4f5-291">Vänta tills överföringsbegäran har slutförts.</span><span class="sxs-lookup"><span data-stu-id="5e4f5-291">Wait for the transfer request to complete.</span></span>

### <a name="indirect-provider---verify-transfer-request-is-complete"></a><span data-ttu-id="5e4f5-292">Indirekt leverantör – verifiera att överföringsbegäran har slutförts</span><span class="sxs-lookup"><span data-stu-id="5e4f5-292">Indirect provider - verify transfer request is complete</span></span>

1. <span data-ttu-id="5e4f5-293">När överföringsbegäran har slutförts kontrollerar du att prenumerationerna visas under **Prenumerationer.**</span><span class="sxs-lookup"><span data-stu-id="5e4f5-293">After the transfer request is completed successfully, verify that you can see the subscriptions appear under **Subscriptions**.</span></span>

2. <span data-ttu-id="5e4f5-294">Informera övergångspartnern.</span><span class="sxs-lookup"><span data-stu-id="5e4f5-294">Inform the transitioning partner.</span></span>

### <a name="transitioning-partner---verify-transfer-request-is-complete"></a><span data-ttu-id="5e4f5-295">Övergångspartner – kontrollera att överföringsbegäran har slutförts</span><span class="sxs-lookup"><span data-stu-id="5e4f5-295">Transitioning partner - verify transfer request is complete</span></span>

<span data-ttu-id="5e4f5-296">Övergångspartnern bör göra följande:</span><span class="sxs-lookup"><span data-stu-id="5e4f5-296">The transitioning partner should do the following:</span></span>

1. <span data-ttu-id="5e4f5-297">Logga in på Partner Center som **administratörsagent** eller **försäljningsagent.**</span><span class="sxs-lookup"><span data-stu-id="5e4f5-297">Sign into Partner Center as an **Admin Agent** or **Sales Agent**.</span></span>

2. <span data-ttu-id="5e4f5-298">På sidan **Kunder** väljer du den avsedda kunden och klickar på ikonen **Snabblänkar** för att expandera sammanfattningsvyn för kunden.</span><span class="sxs-lookup"><span data-stu-id="5e4f5-298">In the **Customers** page, select the intended customer and click on the **Quick links** icon to expand the summary view of the customer.</span></span>

3. <span data-ttu-id="5e4f5-299">Klicka **på Visa prenumerationer.**</span><span class="sxs-lookup"><span data-stu-id="5e4f5-299">Click **View Subscriptions**.</span></span>

4. <span data-ttu-id="5e4f5-300">På sidan **Prenumerationer** letar du upp **Prenumerationsöverföring.**</span><span class="sxs-lookup"><span data-stu-id="5e4f5-300">In the **Subscriptions** page, look for **Subscription Transfer**.</span></span>

5. <span data-ttu-id="5e4f5-301">Kontrollera att överföringsbegäran har markerats som **Fullständig.**</span><span class="sxs-lookup"><span data-stu-id="5e4f5-301">Verify that the transfer request is marked as **Complete**.</span></span>

6. <span data-ttu-id="5e4f5-302">Kontrollera att prenumerationerna inte längre visas som aktiva på **sidan** Prenumerationer:</span><span class="sxs-lookup"><span data-stu-id="5e4f5-302">Verify that the subscription(s) no longer appear as active in the **Subscriptions** page:</span></span>

   1. <span data-ttu-id="5e4f5-303">Om det här är en Azure-prenumeration (MS-AZR-0145P) visas den inte längre.</span><span class="sxs-lookup"><span data-stu-id="5e4f5-303">If this is an Azure subscription (MS-AZR-0145P), it will no longer be listed.</span></span>

   2. <span data-ttu-id="5e4f5-304">Om det här är en licensbaserad prenumeration (Office 365, Dynamics, Intune) visas den med tillståndet **Pausad.**</span><span class="sxs-lookup"><span data-stu-id="5e4f5-304">If this is a license-based subscription (Office 365, Dynamics, Intune), it will be listed with state as **Suspended**.</span></span>

   :::image type="content" source="images/direct/direct13.png" alt-text="Prenumerationen har pausats":::

### <a name="considerations"></a><span data-ttu-id="5e4f5-306">Överväganden</span><span class="sxs-lookup"><span data-stu-id="5e4f5-306">Considerations</span></span>

- <span data-ttu-id="5e4f5-307">**Prenumerations-ID skiljer sig efter överföringen.**</span><span class="sxs-lookup"><span data-stu-id="5e4f5-307">**Subscription ID will be different after transfer.**</span></span> <span data-ttu-id="5e4f5-308">Om det är en Azure-prenumeration (MS-AZR-0145P) har den dessutom ett Azure-prenumerations-ID som behålls från den tidigare ägaren och visas i Azure-hanteringsportalen.</span><span class="sxs-lookup"><span data-stu-id="5e4f5-308">If it is an Azure subscription (MS-AZR-0145P), additionally, it will have an Azure Subscription ID, which is retained from the previous owner, and will appear in the Azure management portal.</span></span>

- <span data-ttu-id="5e4f5-309">**Samma prenumeration kan inte refereras till av flera överföringsbegäranden.**</span><span class="sxs-lookup"><span data-stu-id="5e4f5-309">**The same subscription cannot be referenced by multiple transfer requests.**</span></span> <span data-ttu-id="5e4f5-310">När du har skapat en överföringsbegäran, som innehåller en befintlig prenumeration, kan du inte skapa ytterligare överföringsbegäranden, inklusive samma prenumeration, förrän den första överföringsbegäran avbryts.</span><span class="sxs-lookup"><span data-stu-id="5e4f5-310">After you have created a transfer request, which includes an existing subscription, you cannot create additional transfer requests including the same subscription, until the first transfer request is canceled.</span></span>

- <span data-ttu-id="5e4f5-311">**Tillägg för licensbaserade prenumerationer måste överföras tillsammans med basprenumerationen.**</span><span class="sxs-lookup"><span data-stu-id="5e4f5-311">**Add-ons for license-based subscriptions must be transferred along with their base subscription.**</span></span> <span data-ttu-id="5e4f5-312">När du skapar en överföringsbegäran tas tilläggen automatiskt med i överföringsbegäran om du väljer en befintlig prenumeration med ett eller flera tillägg.</span><span class="sxs-lookup"><span data-stu-id="5e4f5-312">When creating a transfer request, if you pick an existing subscription with one or more add-ons, the add-ons will automatically be included in the transfer request.</span></span>

- <span data-ttu-id="5e4f5-313">**Licensantalsändringar i en prenumeration återspeglas inte i en befintlig överföringsbegäran.**</span><span class="sxs-lookup"><span data-stu-id="5e4f5-313">**License count changes to a subscription will not be reflected in existing transfer request.**</span></span> <span data-ttu-id="5e4f5-314">När du har skapat en överföringsbegäran som innehåller en befintlig prenumeration bör du undvika att uppdatera prenumerationens licenskvantitet (eller associerade addons).</span><span class="sxs-lookup"><span data-stu-id="5e4f5-314">After you have created a transfer request which includes an existing subscription, you should avoid updating the license quantity of the subscription (or associated addons).</span></span> <span data-ttu-id="5e4f5-315">Om du gör det återspeglas inte den nya kvantiteten i överföringsbegäran.</span><span class="sxs-lookup"><span data-stu-id="5e4f5-315">If you do so, the new quantity will not be reflected in the transfer request.</span></span> <span data-ttu-id="5e4f5-316">När den indirekta providern har accepterat överföringsbegäran får den resulterande prenumerationen den gamla kvantiteten.</span><span class="sxs-lookup"><span data-stu-id="5e4f5-316">After the indirect provider accepts the transfer request, the resultant subscription will have the old quantity.</span></span> <span data-ttu-id="5e4f5-317">Om du vill att den nya kvantiteten ska överföras till den indirekta providern måste du avbryta den befintliga överföringsbegäran och återskapa en ny.</span><span class="sxs-lookup"><span data-stu-id="5e4f5-317">If you wish for the new quantity to be transferred to the indirect provider, you must cancel the existing transfer request and recreate a new one.</span></span>

- <span data-ttu-id="5e4f5-318">**Alla köp kan inte överföras med hjälp av självbetjänad prenumerationsöverföring.**</span><span class="sxs-lookup"><span data-stu-id="5e4f5-318">**Not all purchases can be transferred using self-served subscription transfer.**</span></span> <span data-ttu-id="5e4f5-319">För närvarande kan du bara överföra O365-prenumerationer och Azure PAYG-prenumerationer (MS-AZR-0145P) med den här funktionen.</span><span class="sxs-lookup"><span data-stu-id="5e4f5-319">Currently, you can only transfer O365 subscriptions and Azure PAYG subscriptions (MS-AZR-0145P) using this feature.</span></span> <span data-ttu-id="5e4f5-320">Andra inköp, inklusive Azure-planer, reserverade Azure-instanser, termbaserade prenumerationer och SaaS-prenumerationer för Azure Marketplace stöds inte.</span><span class="sxs-lookup"><span data-stu-id="5e4f5-320">Other purchases including Azure Plans, Azure Reserved Instances, Term-based Subscriptions and SaaS subscriptions for Azure Marketplace are not supported.</span></span> <span data-ttu-id="5e4f5-321">Du ser en orsak till varför en prenumeration inte kan överföras på sidan skicka överföringsbegäran.</span><span class="sxs-lookup"><span data-stu-id="5e4f5-321">You will see a reason why a subscription cannot be transferred in the submit transfer request page.</span></span> <span data-ttu-id="5e4f5-322">Om du vill överföra dessa prenumerationer måste du avbryta [den befintliga prenumerationen och](create-a-new-subscription.md#suspend-or-cancel-a-subscription) köpa ett nytt erbjudande för kunden via indirekt leverantör.</span><span class="sxs-lookup"><span data-stu-id="5e4f5-322">To transfer these subscriptions, you will need to [cancel the existing subscription](create-a-new-subscription.md#suspend-or-cancel-a-subscription) and purchase new offer for customer through Indirect Provider.</span></span>

- <span data-ttu-id="5e4f5-323">**Det går inte att testa med sandbox-miljön.**</span><span class="sxs-lookup"><span data-stu-id="5e4f5-323">**Cannot be tested using sandbox environment.**</span></span>

## <a name="enroll-for-indirect-reseller-incentives"></a><span data-ttu-id="5e4f5-324">Registrera dig för indirekta återförsäljarincitament</span><span class="sxs-lookup"><span data-stu-id="5e4f5-324">Enroll for indirect reseller incentives</span></span>

<span data-ttu-id="5e4f5-325">När du har registrerat dig som indirekt återförsäljare på din befintliga partnerklient för direktfakturering får du en inbjudan att registrera dig för indirekt återförsäljares incitament inom 30 dagar.</span><span class="sxs-lookup"><span data-stu-id="5e4f5-325">After you have successfully enrolled as an indirect reseller on your existing direct bill partner tenant, you will receive an invitation to enroll for indirect reseller incentive within 30 days.</span></span> <span data-ttu-id="5e4f5-326">Inbjudan baseras på partnerns MPN-konto som för närvarande är associerat med din CSP-partnerklientorganisation.</span><span class="sxs-lookup"><span data-stu-id="5e4f5-326">The invitation is based on the partner MPN account that is currently associated with your CSP partner tenant.</span></span> <span data-ttu-id="5e4f5-327">Inbjudan skickas till den e-postadress som är associerad med partnerns MPN-konto.</span><span class="sxs-lookup"><span data-stu-id="5e4f5-327">The invitation will be sent to the email address associated with the partner MPN account.</span></span>

<span data-ttu-id="5e4f5-328">Du är också berättigad att registrera dig för incitamentprogram med direktfakturering med samma partnerklientorganisation.</span><span class="sxs-lookup"><span data-stu-id="5e4f5-328">You are also eligible to enroll for direct bill incentive programs with that same partner tenant.</span></span> <span data-ttu-id="5e4f5-329">Du måste hantera programmen separat.</span><span class="sxs-lookup"><span data-stu-id="5e4f5-329">You must manage the programs separately.</span></span>

## <a name="next-steps"></a><span data-ttu-id="5e4f5-330">Nästa steg</span><span class="sxs-lookup"><span data-stu-id="5e4f5-330">Next steps</span></span>

- [<span data-ttu-id="5e4f5-331">Ytterligare information om hur du blir en indirekt återförsäljare</span><span class="sxs-lookup"><span data-stu-id="5e4f5-331">Additional information on becoming an indirect reseller</span></span>](https://assetsprod.microsoft.com/csp-directbill-to-indirect-transition.pdf)
- [<span data-ttu-id="5e4f5-332">Nya krav för CSP-direktpartner</span><span class="sxs-lookup"><span data-stu-id="5e4f5-332">CSP direct partner new requirements</span></span>](direct-partner-new-requirements.md)
- [<span data-ttu-id="5e4f5-333">Begränsade funktioner för direktfakturering</span><span class="sxs-lookup"><span data-stu-id="5e4f5-333">Restricted direct bill capabilities</span></span>](restricted-direct-bill-capabilities.md)
