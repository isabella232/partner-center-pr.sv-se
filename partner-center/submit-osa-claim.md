---
title: Skapa en kund koppling
ms.topic: article
ms.date: 09/11/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
description: Skapa kund kopplingar med CPOR-modellen (anspråks partner). Hjälper till att hantera försäljning, användning, incitament för Microsoft 365 & Dynamics 365-kunder.
author: MalloryPrincipe
ms.author: mallp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: e34698b51a159445f4354e366f79f510533e6f30
ms.sourcegitcommit: 3c45a181ef86b3a4866e97fb50efeae8714ab3f7
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 10/19/2020
ms.locfileid: "92532000"
---
# <a name="customer-associations-via-the-claimed-partner-of-record-cpor-model-for-microsoft-365-and-dynamics-365"></a><span data-ttu-id="f50a4-104">Kund kopplingar via CPOR-modellen (påstått partner of Record) för Microsoft 365 och Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="f50a4-104">Customer associations via the Claimed Partner of Record (CPOR) model for Microsoft 365 and Dynamics 365</span></span>

<span data-ttu-id="f50a4-105">**Gäller för**</span><span class="sxs-lookup"><span data-stu-id="f50a4-105">**Applies to**</span></span>

- <span data-ttu-id="f50a4-106">Partnercenter</span><span class="sxs-lookup"><span data-stu-id="f50a4-106">Partner Center</span></span>

<span data-ttu-id="f50a4-107">**Lämpliga roller:**</span><span class="sxs-lookup"><span data-stu-id="f50a4-107">**Appropriate roles:**</span></span>

- <span data-ttu-id="f50a4-108">Incitaments administratör</span><span class="sxs-lookup"><span data-stu-id="f50a4-108">Incentives admin</span></span>

<span data-ttu-id="f50a4-109">Den 1 oktober 2019 började Microsoft använda CPOR-modellen (anspråks partner of Record) för att hantera de associationer som du har med din Microsoft 365-och Dynamics 365-kunder med avseende Online Services Advisory (OSA), användning av online tjänster (OSU) – Microsoft 365 och OSU-Business program.</span><span class="sxs-lookup"><span data-stu-id="f50a4-109">On October 1, 2019, Microsoft began using the Claiming Partner of Record (CPOR) model to manage the associations you have with your Microsoft 365 and Dynamics 365 customers with regards to the Online Services Advisory (OSA) Sell, Online Services Usage (OSU)-Microsoft 365 and OSU-Business Application incentives.</span></span>

>[!Important]
> <span data-ttu-id="f50a4-110">CPOR-anspråk (Customer Association) gäller endast för Online Services Advisory (OSA), (Online Services-användning), Microsoft 365 och OSU-Business program för program vara.</span><span class="sxs-lookup"><span data-stu-id="f50a4-110">Customer Association (CPOR) claims only apply to the Online Services Advisory (OSA) Sell, Online Services Usage (OSU)-Microsoft 365 and OSU-Business Application incentive programs.</span></span> <span data-ttu-id="f50a4-111">Om du skickar ett co-op-anspråk för ett annat program, t. ex. moln lösnings leverantör, hanterad åter försäljare, värd eller yta, referera till co-op anspråks process som beskrivs här.</span><span class="sxs-lookup"><span data-stu-id="f50a4-111">If you are submitting a co-op claim for another program such as Cloud Solution Provider, Managed Reseller, Hosting, or Surface, please refer to Co-op claims process outlined here.</span></span> <br><br><span data-ttu-id="f50a4-112">När du skickar in ditt anspråk, verifierar Microsoft det.</span><span class="sxs-lookup"><span data-stu-id="f50a4-112">When you submit your claim, Microsoft validates it.</span></span> <span data-ttu-id="f50a4-113">Vi kan be dig om mer information i det här skedet.</span><span class="sxs-lookup"><span data-stu-id="f50a4-113">We may ask you for more information at this point.</span></span> <span data-ttu-id="f50a4-114">Vi meddelar även kunden om din associerings förfrågan.</span><span class="sxs-lookup"><span data-stu-id="f50a4-114">We'll also notify the customer of your association request.</span></span> <span data-ttu-id="f50a4-115">Kunder har fem arbets dagar för att avanmäla sig. Om de inte avanmäler sig, kommer din Association med den här klient organisationen och arbets belastningen att bli officiell.</span><span class="sxs-lookup"><span data-stu-id="f50a4-115">Customers have five business days to opt out. If they don't opt out, your association with this specific tenant and workload will be official.</span></span> <span data-ttu-id="f50a4-116">Nu har du åtkomst till kundens användnings data.</span><span class="sxs-lookup"><span data-stu-id="f50a4-116">At this point you'll have access to the customer's usage data.</span></span> 

<span data-ttu-id="f50a4-117">Du behöver följande information för att slutföra ett anspråk:</span><span class="sxs-lookup"><span data-stu-id="f50a4-117">You'll need the following information to complete a claim:</span></span>

- <span data-ttu-id="f50a4-118">**MPN-ID** för entiteten som gör anspråk</span><span class="sxs-lookup"><span data-stu-id="f50a4-118">The **MPN ID** for your entity that makes the claim</span></span>

- <span data-ttu-id="f50a4-119">Kundens **domän namn** [hitta detta](find-domain-name.md)</span><span class="sxs-lookup"><span data-stu-id="f50a4-119">Customer's **domain name** [Find this](find-domain-name.md)</span></span>

- <span data-ttu-id="f50a4-120">Kundens **katalog-ID** eller **klient-ID** [hitta detta](find-domain-name.md)</span><span class="sxs-lookup"><span data-stu-id="f50a4-120">Customer's **Directory ID** or **Tenant ID** [Find this](find-domain-name.md)</span></span>

- <span data-ttu-id="f50a4-121">**Lösnings avsnittet** , till exempel Business Applications eller Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="f50a4-121">The **Solution area** , such as Business Applications or Microsoft 365</span></span>

- <span data-ttu-id="f50a4-122">Den **aktivitet** du har utfört och vilken typ av anspråk du vill göra, till exempel för försäljning, användning eller intäkts koppling</span><span class="sxs-lookup"><span data-stu-id="f50a4-122">The **Activity** you have performed and the type of claim you want to make, such as Pre-sales, Usage, or Revenue association</span></span>

- <span data-ttu-id="f50a4-123">Kundens **kontakt namn** , titel och e-postadress</span><span class="sxs-lookup"><span data-stu-id="f50a4-123">Your customer's **Contact name** , title, and email address</span></span>

- <span data-ttu-id="f50a4-124">För Dynamics 365 måste du också ange kundens **tekniska kontakt** namn, titel och e-postadress</span><span class="sxs-lookup"><span data-stu-id="f50a4-124">For Dynamics 365, you also need to provide your customer's **Technical contact** name, title, and email address</span></span>

- <span data-ttu-id="f50a4-125">Ditt eget företags **kontakt namn** och e-postadress</span><span class="sxs-lookup"><span data-stu-id="f50a4-125">Your own company's **Contact name** and email address</span></span>

- <span data-ttu-id="f50a4-126">Du skapar ett **namn** för det här anspråket</span><span class="sxs-lookup"><span data-stu-id="f50a4-126">You'll create a **Name** for this claim</span></span>

- <span data-ttu-id="f50a4-127">**Produkt (er)** eller arbets belastningar som du ansöker</span><span class="sxs-lookup"><span data-stu-id="f50a4-127">The **Product(s)** or workload(s) you're claiming</span></span>

- <span data-ttu-id="f50a4-128">**Poe (proof of Execution)** , till exempel en uppgift om arbete som har signerats av kunden.</span><span class="sxs-lookup"><span data-stu-id="f50a4-128">**Proof of execution (PoE)** , such as a statement of work signed by the customer.</span></span> <span data-ttu-id="f50a4-129">Du kan också hämta en PoE-mall som ska användas.</span><span class="sxs-lookup"><span data-stu-id="f50a4-129">You can also download a PoE template to use.</span></span>

- <span data-ttu-id="f50a4-130">Endast för partner som ansöker om intäkts Association: **namnet på Dynamics-lösningens säljare** , **kundens namn** och **namnet på ISV-produkten/lösningen** .</span><span class="sxs-lookup"><span data-stu-id="f50a4-130">For partners claiming revenue association only: **Dynamics solution seller name** , **Customer name** , and **Name of ISV product/solution** .</span></span> 

<span data-ttu-id="f50a4-131">Du bör också förstå följande punkter:</span><span class="sxs-lookup"><span data-stu-id="f50a4-131">You should also understand the following points:</span></span>

- <span data-ttu-id="f50a4-132">Om du har befintliga Microsoft 365-kunder måste du associera dem igen med dem som du vill fortsätta att få OSU incitament genom att använda den här processen.</span><span class="sxs-lookup"><span data-stu-id="f50a4-132">If you have existing Microsoft 365 customers, you'll need to re-associate with those you want to continue to earn OSU incentives by using this process.</span></span>

- <span data-ttu-id="f50a4-133">Om du har befintliga associationer med Dynamics 365 eller Power BI kunder förblir dessa associationer giltiga tills förfallo tiden för deras prenumerationer går ut.</span><span class="sxs-lookup"><span data-stu-id="f50a4-133">If you have existing associations with Dynamics 365 or Power BI customers, these associations will remain valid, until the expiration of their subscriptions.</span></span>

- <span data-ttu-id="f50a4-134">En kund kan ha flera partner, men varje arbets belastning (för OSU-Microsoft 365) eller prenumeration (för OSA-Sell och OSU-Business program) kan bara kopplas till en partner.</span><span class="sxs-lookup"><span data-stu-id="f50a4-134">A customer can have multiple partners, but each workload (for OSU-Microsoft 365) or subscription (for OSA-Sell and OSU-Business Applications) can only be associated with one partner.</span></span>

## <a name="create-a-customer-association"></a><span data-ttu-id="f50a4-135">Skapa en kund koppling</span><span class="sxs-lookup"><span data-stu-id="f50a4-135">Create a customer association</span></span>

1. <span data-ttu-id="f50a4-136">Logga in på [instrumentpanelen i Partnercenter](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="f50a4-136">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="f50a4-137">Välj fliken **incitament** , Välj **Översikt** och välj sedan **kund kopplingar** .</span><span class="sxs-lookup"><span data-stu-id="f50a4-137">Select the **Incentives** tab, select **Overview** , and then select **Customer associations** .</span></span>

3. <span data-ttu-id="f50a4-138">Överst på sidan kund kopplingar väljer du **+ kund koppling** .</span><span class="sxs-lookup"><span data-stu-id="f50a4-138">At the top of the Customer associations page, select **+ Customer association** .</span></span>

4. <span data-ttu-id="f50a4-139">Välj **MPN-ID** för den partnerplats som ska associeras med kunden och lägg sedan till kundens domännamn och katalog-ID.</span><span class="sxs-lookup"><span data-stu-id="f50a4-139">Select the **MPN ID** of the partner location to be associated with the customer, and then add the customer's domain name and Directory ID.</span></span> [<span data-ttu-id="f50a4-140">Hitta detta</span><span class="sxs-lookup"><span data-stu-id="f50a4-140">Find this</span></span>](find-domain-name.md)

5. <span data-ttu-id="f50a4-141">Välj **Fortsätt** .</span><span class="sxs-lookup"><span data-stu-id="f50a4-141">Select **Continue** .</span></span>

6. <span data-ttu-id="f50a4-142">Välj **lösnings Area** och- **aktivitet** .</span><span class="sxs-lookup"><span data-stu-id="f50a4-142">Select the **Solution area** and **Activity** .</span></span> 

   >[!Note]
   >
   ><span data-ttu-id="f50a4-143">Om du väljer Business Applications väljer du antingen **användning och/eller för försäljning** eller **intäkts Association** och väljer sedan **Fortsätt** .</span><span class="sxs-lookup"><span data-stu-id="f50a4-143">If you select Business Applications, select either **Usage and/or Pre-sales** , or **Revenue association** , and then select **Continue** .</span></span> 
   <br><br><span data-ttu-id="f50a4-144">Om du väljer Intäktsassociation får du ange lite annan information än vad som anges nedan.</span><span class="sxs-lookup"><span data-stu-id="f50a4-144">If you select Revenue association, you'll be prompted for slightly different information than what's listed below.</span></span>

7. <span data-ttu-id="f50a4-145">Ange lämplig information på sidan **koppla kund** och välj sedan **Skapa anspråk** .</span><span class="sxs-lookup"><span data-stu-id="f50a4-145">Enter the appropriate information on the **Associate customer** page, and then select **Create claim** .</span></span>

8. <span data-ttu-id="f50a4-146">Välj de produkter som är kopplade till den här kund kopplingen och välj sedan **Fortsätt** .</span><span class="sxs-lookup"><span data-stu-id="f50a4-146">Select the product(s) associated with this customer association, and then select **Continue** .</span></span>

9. <span data-ttu-id="f50a4-147">Fyll i kundens kontaktuppgifter och ditt företags kontaktuppgifter.</span><span class="sxs-lookup"><span data-stu-id="f50a4-147">Complete the customer contact information and your company's contact information.</span></span> <span data-ttu-id="f50a4-148">Alla fält måste fyllas i.</span><span class="sxs-lookup"><span data-stu-id="f50a4-148">All fields are required.</span></span> 

   >[!NOTE]
   ><span data-ttu-id="f50a4-149">Om produkten är Dynamics 365 och den produkt du väljer har flera prenumerationer för den här specifika kunden måste du också ange prenumerations-ID: t.</span><span class="sxs-lookup"><span data-stu-id="f50a4-149">If your product is Dynamics 365, and the product you choose has multiple subscriptions for this particular customer, you'll also need to enter the subscription ID.</span></span>

10. <span data-ttu-id="f50a4-150">Ange din bevisning för körning (PoE).</span><span class="sxs-lookup"><span data-stu-id="f50a4-150">Supply your proof of execution (PoE).</span></span> <span data-ttu-id="f50a4-151">Du kan dra den till rutan, bläddra till din egen stöddokumentation eller använda en mall genom att välja **Ladda ned mall** .</span><span class="sxs-lookup"><span data-stu-id="f50a4-151">You can drag it to the box, browse to your own supporting documentation, or use a template by selecting **Download template** .</span></span> 

11. <span data-ttu-id="f50a4-152">Lägg till och spara kommentarer om du vill och välj sedan **Skicka anspråk** .</span><span class="sxs-lookup"><span data-stu-id="f50a4-152">Add and save comments if you like, and then select **Submit claim** .</span></span> <span data-ttu-id="f50a4-153">Vi skickar ett e-postmeddelande till kunden om att godkänna din kundassociation.</span><span class="sxs-lookup"><span data-stu-id="f50a4-153">We'll send an email to the customer requesting approval of your customer association.</span></span>

   >[!NOTE]
   ><span data-ttu-id="f50a4-154">När du har skickat din kund koppling kan du inte redigera den.</span><span class="sxs-lookup"><span data-stu-id="f50a4-154">Once you submit your customer association, you can't edit it.</span></span>

<span data-ttu-id="f50a4-155">Du ser status för kundassociationen i fältet **Status** .</span><span class="sxs-lookup"><span data-stu-id="f50a4-155">The status of your customer association appears in the **Status** field.</span></span>

<span data-ttu-id="f50a4-156">Välj **Historik** om du vill visa historiken för en kundassociation.</span><span class="sxs-lookup"><span data-stu-id="f50a4-156">Select **History** to view the history of a customer association.</span></span>

## <a name="next-steps"></a><span data-ttu-id="f50a4-157">Nästa steg</span><span class="sxs-lookup"><span data-stu-id="f50a4-157">Next steps</span></span>

- [<span data-ttu-id="f50a4-158">Hantera kundassociationer</span><span class="sxs-lookup"><span data-stu-id="f50a4-158">Manage customer associations</span></span>](incentives-manage-customer-associations.md)