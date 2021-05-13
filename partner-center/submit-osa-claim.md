---
title: Skapa en kundassociation
ms.topic: article
ms.date: 10/28/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
description: Skapa kundassociationer med Claiming Partner of Record -modellen (CPOR). Hjälper till att hantera försäljning, användning och incitament för Microsoft 365 & Dynamics 365-kunder.
author: MalloryPrincipe
ms.author: mallp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 9526a47d0b6d734bde48f403c11fa84d734511c1
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 05/13/2021
ms.locfileid: "109856108"
---
# <a name="customer-associations-via-the-claimed-partner-of-record-cpor-model-for-microsoft-365-and-dynamics-365"></a><span data-ttu-id="300f8-104">Kundassociationer via CPOR-modellen (Claimed Partner of Record) för Microsoft 365 och Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="300f8-104">Customer associations via the Claimed Partner of Record (CPOR) model for Microsoft 365 and Dynamics 365</span></span>


<span data-ttu-id="300f8-105">**Lämpliga roller:** Incitamentsadministratör</span><span class="sxs-lookup"><span data-stu-id="300f8-105">**Appropriate roles**: Incentives admin</span></span>

<span data-ttu-id="300f8-106">Den 1 oktober 2019 började Microsoft använda CPOR-modellen (Claiming Partner of Record) för att hantera de associationer som du har med dina Microsoft 365- och Dynamics 365-kunder med avseende på Online Services Advisory (OSA) Sell, Online Services Usage (OSU)-Microsoft 365 och OSU-Business Application incentives.</span><span class="sxs-lookup"><span data-stu-id="300f8-106">On October 1, 2019, Microsoft began using the Claiming Partner of Record (CPOR) model to manage the associations you have with your Microsoft 365 and Dynamics 365 customers with regard to the Online Services Advisory (OSA) Sell, Online Services Usage (OSU)-Microsoft 365, and OSU-Business Application incentives.</span></span>

>[!Important]
> <span data-ttu-id="300f8-107">CPOR-anspråk (Customer Association) gäller endast för OSU(Online Services Sell, Online Services Usage) – Microsoft 365 och OSU-Business program.</span><span class="sxs-lookup"><span data-stu-id="300f8-107">Customer Association (CPOR) claims only apply to the Online Services Advisory (OSA) Sell, Online Services Usage (OSU)-Microsoft 365 and OSU-Business Application incentive programs.</span></span> <span data-ttu-id="300f8-108">Om du skickar ett co-op-anspråk för ett annat program, till exempel Molnlösningsleverantör, Managed Reseller, värd eller Surface, kan du gå till co-op-anspråksprocessen som beskrivs här.</span><span class="sxs-lookup"><span data-stu-id="300f8-108">If you are submitting a co-op claim for another program such as Cloud Solution Provider, Managed Reseller, Hosting, or Surface, please refer to Co-op claims process outlined here.</span></span> <br><br><span data-ttu-id="300f8-109">När du skickar in ditt anspråk verifierar Microsoft det.</span><span class="sxs-lookup"><span data-stu-id="300f8-109">When you submit your claim, Microsoft validates it.</span></span> <span data-ttu-id="300f8-110">Vi kan be dig om mer information i det här läget.</span><span class="sxs-lookup"><span data-stu-id="300f8-110">We may ask you for more information at this point.</span></span> <span data-ttu-id="300f8-111">Vi meddelar även kunden om din associationsbegäran.</span><span class="sxs-lookup"><span data-stu-id="300f8-111">We'll also notify the customer of your association request.</span></span> <span data-ttu-id="300f8-112">Kunder har fem arbetsdagar på sig att avanmäla sig. Om de inte avanmäler sig blir din koppling till den här specifika klientorganisationen och arbetsbelastningen officiell.</span><span class="sxs-lookup"><span data-stu-id="300f8-112">Customers have five business days to opt out. If they don't opt out, your association with this specific tenant and workload will be official.</span></span> <span data-ttu-id="300f8-113">Nu har du åtkomst till kundens användningsdata.</span><span class="sxs-lookup"><span data-stu-id="300f8-113">At this point you'll have access to the customer's usage data.</span></span> 

<span data-ttu-id="300f8-114">Du behöver följande information för att slutföra ett anspråk:</span><span class="sxs-lookup"><span data-stu-id="300f8-114">You'll need the following information to complete a claim:</span></span>

- <span data-ttu-id="300f8-115">**MPN-ID:t** för din entitet som gör anspråket</span><span class="sxs-lookup"><span data-stu-id="300f8-115">The **MPN ID** for your entity that makes the claim</span></span>

- <span data-ttu-id="300f8-116">Kundens domännamn **Hitta** [det här](find-ids-and-domain-names.md)</span><span class="sxs-lookup"><span data-stu-id="300f8-116">Customer's **domain name** [Find this](find-ids-and-domain-names.md)</span></span>

- <span data-ttu-id="300f8-117">Kundens **katalog-ID eller** **klientorganisations-ID Hitta** [detta](find-ids-and-domain-names.md)</span><span class="sxs-lookup"><span data-stu-id="300f8-117">Customer's **Directory ID** or **Tenant ID** [Find this](find-ids-and-domain-names.md)</span></span>

- <span data-ttu-id="300f8-118">**Lösningsområdet,** till exempel Business Applications eller Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="300f8-118">The **Solution area**, such as Business Applications or Microsoft 365</span></span>

- <span data-ttu-id="300f8-119">Den **aktivitet** som du har utfört och vilken typ av anspråk du vill göra, till exempel förförsäljning, användning eller intäktsassociating</span><span class="sxs-lookup"><span data-stu-id="300f8-119">The **Activity** you have performed and the type of claim you want to make, such as Pre-sales, Usage, or Revenue association</span></span>

- <span data-ttu-id="300f8-120">Kundens kontaktnamn, **rubrik** och e-postadress</span><span class="sxs-lookup"><span data-stu-id="300f8-120">Your customer's **Contact name**, title, and email address</span></span>

- <span data-ttu-id="300f8-121">För Dynamics 365 måste du också ange  kundens tekniska kontaktnamn, titel och e-postadress</span><span class="sxs-lookup"><span data-stu-id="300f8-121">For Dynamics 365, you also need to provide your customer's **Technical contact** name, title, and email address</span></span>

- <span data-ttu-id="300f8-122">Ditt eget företags **kontaktnamn och e-postadress**</span><span class="sxs-lookup"><span data-stu-id="300f8-122">Your own company's **Contact name** and email address</span></span>

- <span data-ttu-id="300f8-123">Du skapar ett namn **för det** här anspråket</span><span class="sxs-lookup"><span data-stu-id="300f8-123">You'll create a **Name** for this claim</span></span>

- <span data-ttu-id="300f8-124">De **produkter eller** arbetsbelastningar som du gör anspråk på</span><span class="sxs-lookup"><span data-stu-id="300f8-124">The **Product(s)** or workload(s) you're claiming</span></span>

- <span data-ttu-id="300f8-125">**PoE (Proof of Execution),** till exempel en arbetsutdrag som signerats av kunden.</span><span class="sxs-lookup"><span data-stu-id="300f8-125">**Proof of execution (PoE)**, such as a statement of work signed by the customer.</span></span> <span data-ttu-id="300f8-126">Du kan också ladda ned en PoE-mall som du kan använda.</span><span class="sxs-lookup"><span data-stu-id="300f8-126">You can also download a PoE template to use.</span></span>

- <span data-ttu-id="300f8-127">För partner som endast begär intäktsassociation: **Dynamics-lösnings** säljarnamn, Kundnamn och Namn på **ISV-produkt/lösning**.</span><span class="sxs-lookup"><span data-stu-id="300f8-127">For partners claiming revenue association only: **Dynamics solution seller name**, **Customer name**, and **Name of ISV product/solution**.</span></span> 

<span data-ttu-id="300f8-128">Du bör också förstå följande:</span><span class="sxs-lookup"><span data-stu-id="300f8-128">You should also understand the following points:</span></span>

- <span data-ttu-id="300f8-129">Om du har Microsoft 365 kunder måste du associera med dem som du vill fortsätta att skaffa OSU-incitament genom att använda den här processen.</span><span class="sxs-lookup"><span data-stu-id="300f8-129">If you have existing Microsoft 365 customers, you'll need to re-associate with those you want to continue to earn OSU incentives by using this process.</span></span>

- <span data-ttu-id="300f8-130">Om du har befintliga associationer med Dynamics 365 eller Power BI kunder förblir dessa associationer giltiga fram till dess att prenumerationerna upphör att gälla.</span><span class="sxs-lookup"><span data-stu-id="300f8-130">If you have existing associations with Dynamics 365 or Power BI customers, these associations will remain valid, until the expiration of their subscriptions.</span></span>

- <span data-ttu-id="300f8-131">En kund kan ha flera partner, men varje arbetsbelastning (för OSU-Microsoft 365) eller prenumeration (för OSA-Sell- och OSU-Business-program) kan bara associeras med en partner.</span><span class="sxs-lookup"><span data-stu-id="300f8-131">A customer can have multiple partners, but each workload (for OSU-Microsoft 365) or subscription (for OSA-Sell and OSU-Business Applications) can only be associated with one partner.</span></span>

## <a name="create-a-customer-association"></a><span data-ttu-id="300f8-132">Skapa en kundassociation</span><span class="sxs-lookup"><span data-stu-id="300f8-132">Create a customer association</span></span>

1. <span data-ttu-id="300f8-133">Logga in på [instrumentpanelen i Partnercenter](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="300f8-133">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="300f8-134">Välj fliken **Incitament,** välj **Översikt** och välj sedan **Kundassociationer.**</span><span class="sxs-lookup"><span data-stu-id="300f8-134">Select the **Incentives** tab, select **Overview**, and then select **Customer associations**.</span></span>

3. <span data-ttu-id="300f8-135">Längst upp på sidan Kundassociationer väljer du **+ Kundassociationer**.</span><span class="sxs-lookup"><span data-stu-id="300f8-135">At the top of the Customer associations page, select **+ Customer association**.</span></span>

4. <span data-ttu-id="300f8-136">Välj **MPN-ID** för den partnerplats som ska associeras med kunden och lägg sedan till kundens domännamn och katalog-ID.</span><span class="sxs-lookup"><span data-stu-id="300f8-136">Select the **MPN ID** of the partner location to be associated with the customer, and then add the customer's domain name and Directory ID.</span></span> [<span data-ttu-id="300f8-137">Hitta det här</span><span class="sxs-lookup"><span data-stu-id="300f8-137">Find this</span></span>](find-ids-and-domain-names.md)

5. <span data-ttu-id="300f8-138">Välj **Fortsätt**.</span><span class="sxs-lookup"><span data-stu-id="300f8-138">Select **Continue**.</span></span>

6. <span data-ttu-id="300f8-139">Välj **lösningsområdet och** **aktivitet**.</span><span class="sxs-lookup"><span data-stu-id="300f8-139">Select the **Solution area** and **Activity**.</span></span> 

   >[!Note]
   >
   ><span data-ttu-id="300f8-140">Om du Business Applications väljer du **antingen Användning och/eller Förförsäljning** eller **Intäktsassociaty** och väljer sedan **Fortsätt.**</span><span class="sxs-lookup"><span data-stu-id="300f8-140">If you select Business Applications, select either **Usage and/or Pre-sales**, or **Revenue association**, and then select **Continue**.</span></span> 
   <br><br><span data-ttu-id="300f8-141">Om du väljer Intäktsassociation får du ange lite annan information än vad som anges nedan.</span><span class="sxs-lookup"><span data-stu-id="300f8-141">If you select Revenue association, you'll be prompted for slightly different information than what's listed below.</span></span>

7. <span data-ttu-id="300f8-142">Ange lämplig information på sidan **Associera** kund och välj sedan **Skapa anspråk.**</span><span class="sxs-lookup"><span data-stu-id="300f8-142">Enter the appropriate information on the **Associate customer** page, and then select **Create claim**.</span></span>

8. <span data-ttu-id="300f8-143">Välj de produkter som är associerade med den här kundassociaten och välj sedan **Fortsätt.**</span><span class="sxs-lookup"><span data-stu-id="300f8-143">Select the product(s) associated with this customer association, and then select **Continue**.</span></span>

9. <span data-ttu-id="300f8-144">Fyll i kundens kontaktuppgifter och ditt företags kontaktuppgifter.</span><span class="sxs-lookup"><span data-stu-id="300f8-144">Complete the customer contact information and your company's contact information.</span></span> <span data-ttu-id="300f8-145">Alla fält måste fyllas i.</span><span class="sxs-lookup"><span data-stu-id="300f8-145">All fields are required.</span></span> 

   >[!NOTE]
   ><span data-ttu-id="300f8-146">Om din produkt är Dynamics 365 och den produkt du väljer har flera prenumerationer för den här specifika kunden måste du också ange prenumerations-ID:t.</span><span class="sxs-lookup"><span data-stu-id="300f8-146">If your product is Dynamics 365, and the product you choose has multiple subscriptions for this particular customer, you'll also need to enter the subscription ID.</span></span>

10. <span data-ttu-id="300f8-147">Ange ditt poE (Proof of Execution).</span><span class="sxs-lookup"><span data-stu-id="300f8-147">Supply your proof of execution (PoE).</span></span> <span data-ttu-id="300f8-148">Du kan dra den till rutan, bläddra till din egen stöddokumentation eller använda en mall genom att välja **Ladda ned mall**.</span><span class="sxs-lookup"><span data-stu-id="300f8-148">You can drag it to the box, browse to your own supporting documentation, or use a template by selecting **Download template**.</span></span> 

11. <span data-ttu-id="300f8-149">Lägg till och spara kommentarer om du vill och välj sedan **Skicka anspråk**.</span><span class="sxs-lookup"><span data-stu-id="300f8-149">Add and save comments if you like, and then select **Submit claim**.</span></span> <span data-ttu-id="300f8-150">Vi skickar ett e-postmeddelande till kunden om att godkänna din kundassociation.</span><span class="sxs-lookup"><span data-stu-id="300f8-150">We'll send an email to the customer requesting approval of your customer association.</span></span>

   >[!NOTE]
   ><span data-ttu-id="300f8-151">När du har skickat in din kundassociaty kan du inte redigera den.</span><span class="sxs-lookup"><span data-stu-id="300f8-151">Once you submit your customer association, you can't edit it.</span></span>

<span data-ttu-id="300f8-152">Du ser status för kundassociationen i fältet **Status**.</span><span class="sxs-lookup"><span data-stu-id="300f8-152">The status of your customer association appears in the **Status** field.</span></span>

<span data-ttu-id="300f8-153">Välj **Historik** om du vill visa historiken för en kundassociation.</span><span class="sxs-lookup"><span data-stu-id="300f8-153">Select **History** to view the history of a customer association.</span></span>

## <a name="next-steps"></a><span data-ttu-id="300f8-154">Nästa steg</span><span class="sxs-lookup"><span data-stu-id="300f8-154">Next steps</span></span>

- [<span data-ttu-id="300f8-155">Hantera kundassociationer</span><span class="sxs-lookup"><span data-stu-id="300f8-155">Manage customer associations</span></span>](incentives-manage-customer-associations.md)