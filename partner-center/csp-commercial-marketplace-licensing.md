---
title: Hantera licensiering i Marketplace-erbjudanden
ms.topic: how-to
ms.date: 04/29/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Lär dig hur du ställer in och hanterar licensiering för dina erbjudanden på den kommersiella marknadsplatsen för ISV.
author: petand123
ms.author: v-petand
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: f049ffda4c3d9476c09257fc814e5acac393cb54
ms.sourcegitcommit: 6c20c3cc4a226cada70c56df295966696affcec8
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/30/2021
ms.locfileid: "108328023"
---
# <a name="manage-licensing-in-marketplace-offers"></a><span data-ttu-id="bb109-103">Hantera licensiering i Marketplace-erbjudanden</span><span class="sxs-lookup"><span data-stu-id="bb109-103">Manage licensing in marketplace offers</span></span>

<span data-ttu-id="bb109-104">**Lämpliga roller**</span><span class="sxs-lookup"><span data-stu-id="bb109-104">**Appropriate roles**</span></span>

- <span data-ttu-id="bb109-105">Global administratör</span><span class="sxs-lookup"><span data-stu-id="bb109-105">Global admin</span></span>
- <span data-ttu-id="bb109-106">Kontoadministratör</span><span class="sxs-lookup"><span data-stu-id="bb109-106">Account admin</span></span>

<span data-ttu-id="bb109-107">Den här artikeln beskriver steg för steg hur du ställer in ett erbjudande i Partnercenter, gör det tillgängligt i Microsoft AppSource och sedan hanterar licenser för erbjudandet.</span><span class="sxs-lookup"><span data-stu-id="bb109-107">This article walks you through the process of setting up an offer in Partner Center, making it available in Microsoft AppSource, and then managing licenses for that offer.</span></span>  

>[!IMPORTANT]
><span data-ttu-id="bb109-108">Funktionerna i den här artikeln är för närvarande i allmänt tillgänglig förhandsversion.</span><span class="sxs-lookup"><span data-stu-id="bb109-108">The capabilities in this article are currently in Public Preview.</span></span>

## <a name="before-you-begin"></a><span data-ttu-id="bb109-109">Innan du börjar</span><span class="sxs-lookup"><span data-stu-id="bb109-109">Before you begin</span></span>

### <a name="commercial-marketplace-basics"></a><span data-ttu-id="bb109-110">Grundläggande om den kommersiella marknadsplatsen</span><span class="sxs-lookup"><span data-stu-id="bb109-110">Commercial marketplace basics</span></span>

<span data-ttu-id="bb109-111">Innan du påbörjar den här processen bör du bekanta dig med grunderna för den kommersiella marknadsplatsen.</span><span class="sxs-lookup"><span data-stu-id="bb109-111">Before you begin this process, you should familiarize yourself with the basics of the commercial marketplace.</span></span> <span data-ttu-id="bb109-112">Artiklarna i tabellen nedan hjälper dig att komma igång.</span><span class="sxs-lookup"><span data-stu-id="bb109-112">The articles in the table below will help get you started.</span></span> 

| <span data-ttu-id="bb109-113">Avsnitt</span><span class="sxs-lookup"><span data-stu-id="bb109-113">Topic</span></span>  | <span data-ttu-id="bb109-114">Artikel</span><span class="sxs-lookup"><span data-stu-id="bb109-114">Article</span></span>  |
|-------|--------|
|<span data-ttu-id="bb109-115">Planer för den kommersiella marknadsplatsen</span><span class="sxs-lookup"><span data-stu-id="bb109-115">Commercial marketplace plans</span></span> | [<span data-ttu-id="bb109-116">Planer och priser för erbjudanden på den kommersiella marknadsplatsen</span><span class="sxs-lookup"><span data-stu-id="bb109-116">Plans and pricing for commercial marketplace offers</span></span>](/azure/marketplace/plans-pricing)    |
|<span data-ttu-id="bb109-117">Erbjudanden på den kommersiella marknadsplatsen</span><span class="sxs-lookup"><span data-stu-id="bb109-117">Commercial marketplace offers</span></span>  | [<span data-ttu-id="bb109-118">Lista typer</span><span class="sxs-lookup"><span data-stu-id="bb109-118">Listing types</span></span>](/azure/marketplace/determine-your-listing-type)    |
|<span data-ttu-id="bb109-119">Konton på den kommersiella marknadsplatsen</span><span class="sxs-lookup"><span data-stu-id="bb109-119">Commercial marketplace accounts</span></span> |  [<span data-ttu-id="bb109-120">Skapa ett konto för den kommersiella marknadsplatsen i Partnercenter</span><span class="sxs-lookup"><span data-stu-id="bb109-120">Create a commercial marketplace account in Partner Center</span></span>](/azure/marketplace/create-account) |

### <a name="determine-your-offer-id"></a><span data-ttu-id="bb109-121">Fastställa ditt erbjudande-ID</span><span class="sxs-lookup"><span data-stu-id="bb109-121">Determine your Offer ID</span></span>

<span data-ttu-id="bb109-122">I procedurerna nedan uppmanas du att ange ett erbjudande-ID.</span><span class="sxs-lookup"><span data-stu-id="bb109-122">In the procedures below, you’ll be prompted to enter an Offer ID.</span></span> <span data-ttu-id="bb109-123">Ta dig tid att ta fram ett lämpligt erbjudande-ID, med följande i åtanke:</span><span class="sxs-lookup"><span data-stu-id="bb109-123">Take some time now to come up with a suitable Offer ID, keeping in mind the following points:</span></span>

- <span data-ttu-id="bb109-124">Det här ID:t är synligt för kunder i webbadressen för Marketplace-erbjudandet och Azure Resource Manager mallar, om tillämpligt.</span><span class="sxs-lookup"><span data-stu-id="bb109-124">This ID is visible to customers in the web address for the marketplace offer and Azure Resource Manager templates, if applicable.</span></span>
- <span data-ttu-id="bb109-125">Erbjudande-ID i kombination med utgivar-ID måste vara under 40 tecken långt.</span><span class="sxs-lookup"><span data-stu-id="bb109-125">The Offer ID combined with the Publisher ID must be under 40 characters in length.</span></span>
- <span data-ttu-id="bb109-126">Använd bara gemena bokstäver och siffror.</span><span class="sxs-lookup"><span data-stu-id="bb109-126">Use only lowercase letters and numbers.</span></span> <span data-ttu-id="bb109-127">Erbjudande-ID:t kan innehålla bindestreck och understreck, men inga blanksteg.</span><span class="sxs-lookup"><span data-stu-id="bb109-127">The Offer ID can include hyphens and underscores, but no spaces.</span></span> <span data-ttu-id="bb109-128">Om ditt utgivar-ID till exempel `testpublisherid` är och du anger blir `test-offer-1` erbjudandets webbadress `https://appsource.microsoft.com/product/dynamics-365/testpublisherid.test-offer-1` .</span><span class="sxs-lookup"><span data-stu-id="bb109-128">For example, if your Publisher ID is `testpublisherid` and you enter `test-offer-1`, the offer web address will be `https://appsource.microsoft.com/product/dynamics-365/testpublisherid.test-offer-1`.</span></span>
- <span data-ttu-id="bb109-129">Det här ID:t kan inte ändras när du har valt **Skapa**.</span><span class="sxs-lookup"><span data-stu-id="bb109-129">This ID can't be changed after you select **Create**.</span></span>

### <a name="determine-your-offer-alias"></a><span data-ttu-id="bb109-130">Fastställa ditt erbjudandealias</span><span class="sxs-lookup"><span data-stu-id="bb109-130">Determine your Offer alias</span></span>

<span data-ttu-id="bb109-131">Erbjudandets alias är det namn som används för erbjudandet i Partnercenter.</span><span class="sxs-lookup"><span data-stu-id="bb109-131">The Offer alias is the name used for the offer in Partner Center.</span></span> <span data-ttu-id="bb109-132">Du behöver också ett lämpligt erbjudandealias som följer riktlinjerna nedan:</span><span class="sxs-lookup"><span data-stu-id="bb109-132">You’ll also need an appropriate Offer alias that follows the guidelines below:</span></span>

- <span data-ttu-id="bb109-133">Det här namnet används inte på Marketplace och skiljer sig från erbjudandets namn och andra värden som visas för kunder.</span><span class="sxs-lookup"><span data-stu-id="bb109-133">This name isn't used in the marketplace and is different from the offer name and other values shown to customers.</span></span>
- <span data-ttu-id="bb109-134">Det går inte att ändra det här namnet när du har valt Skapa.</span><span class="sxs-lookup"><span data-stu-id="bb109-134">This name can't be changed after you select Create.</span></span>

## <a name="create-your-offer"></a><span data-ttu-id="bb109-135">Skapa ditt erbjudande</span><span class="sxs-lookup"><span data-stu-id="bb109-135">Create your offer</span></span>

<span data-ttu-id="bb109-136">Det första steget i licensieringsprocessen är att skapa ditt erbjudande på den kommersiella marknadsplatsen.</span><span class="sxs-lookup"><span data-stu-id="bb109-136">The first step in the licensing process is to create your commercial marketplace offer.</span></span> 

1. <span data-ttu-id="bb109-137">Logga in på [instrumentpanelen i Partnercenter](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="bb109-137">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="bb109-138">I den vänstra navigeringsmenyn väljer du **Kommersiell marknadsplats/Översikt.**</span><span class="sxs-lookup"><span data-stu-id="bb109-138">On the left navigation menu, select **Commercial Marketplace/Overview**.</span></span>
3. <span data-ttu-id="bb109-139">Längst upp på sidan Översikt väljer du **Nytt erbjudande** och sedan **Dynamics 365 for Customer Engagement & PowerApps**.</span><span class="sxs-lookup"><span data-stu-id="bb109-139">At the top of the Overview page, select **New offer**, and then select **Dynamics 365 for Customer Engagement & PowerApps**.</span></span>
4. <span data-ttu-id="bb109-140">Ange det **erbjudande-ID och** **erbjudandealias** som du skapade tidigare.</span><span class="sxs-lookup"><span data-stu-id="bb109-140">Enter the **Offer ID** and **Offer alias** you created earlier.</span></span>
5. <span data-ttu-id="bb109-141">Välj **Skapa** för att generera erbjudandet och fortsätta.</span><span class="sxs-lookup"><span data-stu-id="bb109-141">Select **Create** to generate the offer and continue.</span></span>
6. <span data-ttu-id="bb109-142">Välj dina licensieringsalternativ.</span><span class="sxs-lookup"><span data-stu-id="bb109-142">Choose your licensing options.</span></span>

    - <span data-ttu-id="bb109-143">Om du vill aktivera licenshantering för ditt erbjudande väljer **du Aktivera applicenshantering via Microsoft**.</span><span class="sxs-lookup"><span data-stu-id="bb109-143">To enable license management for your offer, select **Enable app license management through Microsoft**.</span></span> <span data-ttu-id="bb109-144">Det här är en enda inställning och du kan inte ändra den när ditt erbjudande har publicerats.</span><span class="sxs-lookup"><span data-stu-id="bb109-144">This is a one-time setting, and you can’t change it once your offer is published.</span></span>

    - <span data-ttu-id="bb109-145">Du kan också låta kunder köra appens grundläggande funktioner utan licens och köra Premium-funktioner när de har köpt en licens.</span><span class="sxs-lookup"><span data-stu-id="bb109-145">You can also enable customers to run your app’s base functionality without a license, and run premium features once they’ve purchased a license.</span></span> <span data-ttu-id="bb109-146">Det gör du genom att **välja Tillåt att kunder installerar min app även om licenserna inte har tilldelats**.</span><span class="sxs-lookup"><span data-stu-id="bb109-146">To do this, select **Allow customers to install my app even if licenses are not assigned**.</span></span>

    - <span data-ttu-id="bb109-147">Om du inte vill att ditt erbjudande ska ha licenshantering aktiverat väljer du Hämta nu **(kostnadsfri),** **Kostnadsfri utvärderingsversion** eller **Kontakta mig.**</span><span class="sxs-lookup"><span data-stu-id="bb109-147">If you don’t want your offer to have license management enabled, select **Get it now (Free)**, **Free trial**, or **Contact me**.</span></span>

## <a name="create-your-plan"></a><span data-ttu-id="bb109-148">Skapa din plan</span><span class="sxs-lookup"><span data-stu-id="bb109-148">Create your plan</span></span>

<span data-ttu-id="bb109-149">I de här stegen definierar du den plan eller de planer som du vill aktivera för ditt erbjudande.</span><span class="sxs-lookup"><span data-stu-id="bb109-149">In these steps you’ll define the plan or plans you want to enable for your offer.</span></span>

1. <span data-ttu-id="bb109-150">I den vänstra navigeringsmenyn väljer **du Planera översikt** och sedan Skapa ny **plan.**</span><span class="sxs-lookup"><span data-stu-id="bb109-150">On the left navigation menu, select **Plan overview**, and then select **Create new plan**.</span></span>
2. <span data-ttu-id="bb109-151">Ange ett **plan-ID** **och ett plannamn** och välj sedan **Skapa.**</span><span class="sxs-lookup"><span data-stu-id="bb109-151">Enter a **Plan ID** and **Plan name**, and then select **Create**.</span></span>
3. <span data-ttu-id="bb109-152">Ange din **planbeskrivning** på sidan **Planlista.**</span><span class="sxs-lookup"><span data-stu-id="bb109-152">On the **Plan listing** page, enter your **Plan description**.</span></span>
4. <span data-ttu-id="bb109-153">Spara beskrivningen och slutför senare genom att välja **Spara utkast.**</span><span class="sxs-lookup"><span data-stu-id="bb109-153">To save the description and finish later, select **Save draft**.</span></span>

5. <span data-ttu-id="bb109-154">När du är klar väljer du **Granska och publicera**.</span><span class="sxs-lookup"><span data-stu-id="bb109-154">When you’re finished, select **Review and publish**.</span></span> <span data-ttu-id="bb109-155">Informationen om planen visas nu på sidan appsource.microsoft.com under erbjudandelistan (avsnittet med planer).</span><span class="sxs-lookup"><span data-stu-id="bb109-155">The plan information will now be displayed on appsource.microsoft.com under offer listing (plans section).</span></span>

6. <span data-ttu-id="bb109-156">När du har skapat alla planer för det här erbjudandet måste du kopiera tjänst-ID:t för varje plan.</span><span class="sxs-lookup"><span data-stu-id="bb109-156">After you’ve created all of the plans for this offer, you’ll need to copy each plan’s Service ID.</span></span> <span data-ttu-id="bb109-157">Välj **Översikt över** plan överst på sidan Planlista.</span><span class="sxs-lookup"><span data-stu-id="bb109-157">Select **Plan overview** at the top of the Plan listing page.</span></span> <span data-ttu-id="bb109-158">Kopiera tjänst-ID:t för varje plan till en säker plats.</span><span class="sxs-lookup"><span data-stu-id="bb109-158">Copy the Service ID for each plan to a safe location.</span></span>

## <a name="add-service-ids-to-your-solution"></a><span data-ttu-id="bb109-159">Lägga till tjänst-ID:er i din lösning</span><span class="sxs-lookup"><span data-stu-id="bb109-159">Add Service IDs to your solution</span></span>

<span data-ttu-id="bb109-160">Nästa steg är att uppdatera din lösning genom att lägga till tjänst-ID:erna för varje plan som du nyss kopierade.</span><span class="sxs-lookup"><span data-stu-id="bb109-160">The next step is to update your solution by adding the Service IDs for each plan that you just copied.</span></span> <span data-ttu-id="bb109-161">Vägledning om detta finns i [Skapa ett AppSource-paket för din lösning.](https://docs.microsoft.com/powerapps/developer/data-platform/create-package-app-appsource)</span><span class="sxs-lookup"><span data-stu-id="bb109-161">For guidance on this, see [Create an AppSource Package for your solution](https://docs.microsoft.com/powerapps/developer/data-platform/create-package-app-appsource).</span></span>

## <a name="upload-your-package-and-publish-your-offer"></a><span data-ttu-id="bb109-162">Ladda upp ditt paket och publicera ditt erbjudande</span><span class="sxs-lookup"><span data-stu-id="bb109-162">Upload your package and publish your offer</span></span>

1. <span data-ttu-id="bb109-163">I det vänstra navigeringsfönstret väljer **du Kommersiell marknadsplats** och sedan Teknisk **konfiguration.**</span><span class="sxs-lookup"><span data-stu-id="bb109-163">On the left navigation pane, select **Commercial Marketplace**, and then select **Technical configuration**.</span></span>
2. <span data-ttu-id="bb109-164">Under **Baslicensmodell** väljer du **Användare**.</span><span class="sxs-lookup"><span data-stu-id="bb109-164">Under **Base License Model**, select **User**.</span></span>
3. <span data-ttu-id="bb109-165">Under **CRM-paket** anger du URL:en för din paketplats.</span><span class="sxs-lookup"><span data-stu-id="bb109-165">Under **CRM Package**, enter the URL of your package location.</span></span>
4. <span data-ttu-id="bb109-166">Använd de andra flikarna i det vänstra navigeringsfönstret för att ange annan nödvändig information.</span><span class="sxs-lookup"><span data-stu-id="bb109-166">Use the other tabs on the left navigation pane to enter any other required information.</span></span> <span data-ttu-id="bb109-167">När du är klar väljer du **Granska och publicera**.</span><span class="sxs-lookup"><span data-stu-id="bb109-167">When you’re done, select **Review and publish**.</span></span>

<span data-ttu-id="bb109-168">När du har publicerat erbjudandet granskar och verifierar vi din information.</span><span class="sxs-lookup"><span data-stu-id="bb109-168">After you publish the offer, we’ll review and verify your information.</span></span> <span data-ttu-id="bb109-169">Om det finns några problem med den här processen meddelar vi dig.</span><span class="sxs-lookup"><span data-stu-id="bb109-169">If there are any issues with this process, we’ll notify you.</span></span> <span data-ttu-id="bb109-170">När alla problem har lösts får du ett meddelande om att ditt erbjudande är tillgängligt i AppSource.</span><span class="sxs-lookup"><span data-stu-id="bb109-170">When all issues have been resolved, you’ll get a notification that your offer is available in AppSource.</span></span> <span data-ttu-id="bb109-171">Då kan du göra det live.</span><span class="sxs-lookup"><span data-stu-id="bb109-171">At that point you can make it live.</span></span>

## <a name="make-your-offer-live-in-partner-center"></a><span data-ttu-id="bb109-172">Gör ditt erbjudande live i Partnercenter</span><span class="sxs-lookup"><span data-stu-id="bb109-172">Make your offer live in Partner Center</span></span>

<span data-ttu-id="bb109-173">Proceduren nedan går igenom processen för att göra ditt erbjudande live i AppSource.</span><span class="sxs-lookup"><span data-stu-id="bb109-173">The procedure below walks you through the process of making your offer live in AppSource.</span></span> <span data-ttu-id="bb109-174">Mer information om den här processen finns i [Introduktion till listalternativ.](https://docs.microsoft.com/azure/marketplace/determine-your-listing-type)</span><span class="sxs-lookup"><span data-stu-id="bb109-174">To learn more about this process, see [Introduction to listing options](https://docs.microsoft.com/azure/marketplace/determine-your-listing-type).</span></span>

>[!NOTE]
><span data-ttu-id="bb109-175">När du har publicerat ditt erbjudande tar det 4–6 timmar att publicera det.</span><span class="sxs-lookup"><span data-stu-id="bb109-175">Once you publish your offer, it will take 4-6 hours to go live.</span></span>

1. <span data-ttu-id="bb109-176">Logga in på [instrumentpanelen i Partnercenter](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="bb109-176">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="bb109-177">I den vänstra navigeringsmenyn väljer du **Kommersiell marknadsplats/Översikt.**</span><span class="sxs-lookup"><span data-stu-id="bb109-177">On the left navigation menu, select **Commercial Marketplace/Overview**.</span></span>
3. <span data-ttu-id="bb109-178">På **sidan** Översikt letar du reda på det erbjudande som du letar efter.</span><span class="sxs-lookup"><span data-stu-id="bb109-178">On the **Overview** page, find the offer you’re looking for.</span></span> <span data-ttu-id="bb109-179">Erbjudanden som är klara att publiceras har statusen **Förhandsversion.**</span><span class="sxs-lookup"><span data-stu-id="bb109-179">Offers ready to be published will have a status of **Preview**.</span></span> <span data-ttu-id="bb109-180">Välj erbjudandet.</span><span class="sxs-lookup"><span data-stu-id="bb109-180">Select the offer.</span></span>
4. <span data-ttu-id="bb109-181">På sidan **Översikt över** erbjudande väljer du **Go live**.</span><span class="sxs-lookup"><span data-stu-id="bb109-181">On the **Offer overview** page, select **Go live**.</span></span>
<span data-ttu-id="bb109-182">Erbjudandet är live om 4–6 timmar.</span><span class="sxs-lookup"><span data-stu-id="bb109-182">The offer will be live in 4-6 hours.</span></span>
5. <span data-ttu-id="bb109-183">Om du vill se din erbjudandelista på AppSource väljer du **länken AppSource** längst ned på **översiktssidan för** erbjudandet.</span><span class="sxs-lookup"><span data-stu-id="bb109-183">To see your offer listing on AppSource, select the **AppSource** link at the bottom of the **Offer overview** page.</span></span>

    - <span data-ttu-id="bb109-184">**För licensaktiverade erbjudanden:** Om ditt erbjudande kräver en licenskontroll kan användarna bara ange ett lead genom att klicka på **Kontakta** mig så att du kan kommunicera med dem.</span><span class="sxs-lookup"><span data-stu-id="bb109-184">**For license-enabled offers**: If your offer requires a license check, users will only be able to enter a lead by clicking **Contact Me**, so that you can communicate with them.</span></span>

    - <span data-ttu-id="bb109-185">**För licensaktiverade** erbjudanden med alternativet för kostnadsfri installation: Om ditt erbjudande  inte kräver en licenskontroll ser administratörsanvändarna knappen Hämta nu utöver **Kontakta mig.**</span><span class="sxs-lookup"><span data-stu-id="bb109-185">**For license-enabled offers with free installation option**: If your offer does not require a license check, admin users will see a **Get It Now** button in addition to **Contact Me**.</span></span> <span data-ttu-id="bb109-186">Användare som vill testa ditt kostnadsfria installationsalternativ bör klicka på **Hämta** nu, vilket gör att de kan installera erbjudandet i Power Platform Administrationscenter.</span><span class="sxs-lookup"><span data-stu-id="bb109-186">Users who want to try your free installation option should click **Get It Now**, which will bring them to install the offer on Power Platform Admin Center.</span></span> <span data-ttu-id="bb109-187">Användarna kan fortfarande använda **Kontakta mig** om de har frågor eller om de vill uppgradera till en betald plan.</span><span class="sxs-lookup"><span data-stu-id="bb109-187">Users can still use **Contact Me** if they have any questions, or if they want to upgrade to a paid plan.</span></span>

## <a name="register-isv-connect-deal-in-deal-registration"></a><span data-ttu-id="bb109-188">Registrera ISV Connect-avtalet i Avtalsregistrering</span><span class="sxs-lookup"><span data-stu-id="bb109-188">Register ISV Connect deal in Deal Registration</span></span>

<span data-ttu-id="bb109-189">Innan du kan tilldela licenser till en kund måste varje försäljning registreras i Partnercenter.</span><span class="sxs-lookup"><span data-stu-id="bb109-189">Before you can assign licenses to a customer, each sale needs to be registered in Partner Center.</span></span> <span data-ttu-id="bb109-190">Det gör du genom att [registrera dina avtal.](register-deals.md)</span><span class="sxs-lookup"><span data-stu-id="bb109-190">To do this, see [Register your deals](register-deals.md).</span></span>

## <a name="invite-the-customer"></a><span data-ttu-id="bb109-191">Bjud in kunden</span><span class="sxs-lookup"><span data-stu-id="bb109-191">Invite the customer</span></span>

<span data-ttu-id="bb109-192">Använd följande procedur för att bjuda in kunden att delta i det här avtalet.</span><span class="sxs-lookup"><span data-stu-id="bb109-192">Use the following procedure to invite the customer to participate in this deal.</span></span>  

1. <span data-ttu-id="bb109-193">Logga in på [instrumentpanelen i Partnercenter](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="bb109-193">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="bb109-194">I den vänstra navigeringsmenyn väljer du **Kommersiell marknadsplats/Översikt.**</span><span class="sxs-lookup"><span data-stu-id="bb109-194">On the left navigation menu, select **Commercial Marketplace/Overview**.</span></span>
3. <span data-ttu-id="bb109-195">I den vänstra navigeringsmenyn **väljer du Referenser** och sedan **Avtalsregistrering.**</span><span class="sxs-lookup"><span data-stu-id="bb109-195">On the left navigation menu, select **Referrals**, and then select **Deal Registration**.</span></span>
4. <span data-ttu-id="bb109-196">Filtrera efter **Skickade** avtal, välj **fliken Pågår** och välj sedan det avtal du vill ha.</span><span class="sxs-lookup"><span data-stu-id="bb109-196">Filter for **Submitted** deals, select the **In Progress** tab, and then select the deal you want.</span></span>
5. <span data-ttu-id="bb109-197">På översiktssidan för det här avtalet väljer du **Hantera licenser.**</span><span class="sxs-lookup"><span data-stu-id="bb109-197">On the overview page for this deal, select **Manage licenses**.</span></span>
6. <span data-ttu-id="bb109-198">I fönstret **Hantera** licenser väljer du kunden i **listrutan Kundinformation.**</span><span class="sxs-lookup"><span data-stu-id="bb109-198">In the **Manage licenses** window, select the customer from the **Customer details** dropdown list.</span></span> <span data-ttu-id="bb109-199">Om kundrelationen inte finns ännu väljer du **+Bjud in en ny kund att godkänna**.</span><span class="sxs-lookup"><span data-stu-id="bb109-199">If the customer relationship does not exist yet, select **+Invite a new customer to consent**.</span></span>
7. <span data-ttu-id="bb109-200">Kopiera länken som visas.</span><span class="sxs-lookup"><span data-stu-id="bb109-200">Copy the link that is displayed.</span></span>
8. <span data-ttu-id="bb109-201">Skicka den här länken via e-post till din kunds faktureringsadministratör eller globala administratör och be dem använda den här länken för att komma åt admin.microsoft.com och godkänna och auktorisera relationen som du upprättar.</span><span class="sxs-lookup"><span data-stu-id="bb109-201">Email this link to your customer’s billing admin or global admin, and have them use this link to access admin.microsoft.com and accept and authorize the relationship you’re establishing.</span></span>

    >[!NOTE]
    ><span data-ttu-id="bb109-202">Relationen upprättas inte förrän kunden utför det här steget.</span><span class="sxs-lookup"><span data-stu-id="bb109-202">The relationship will not be established until the customer performs this step.</span></span>

## <a name="activate-manage-and-remove-your-licenses"></a><span data-ttu-id="bb109-203">Aktivera, hantera och ta bort dina licenser</span><span class="sxs-lookup"><span data-stu-id="bb109-203">Activate, manage, and remove your licenses</span></span>

<span data-ttu-id="bb109-204">När kunden har godkänt relationen med dig kan du börja lägga till planer från ditt erbjudande och tilldela licenser till varje plan.</span><span class="sxs-lookup"><span data-stu-id="bb109-204">Once your customer has authorized the relationship with you, you can start adding plans from your offer and assigning licenses to each plan.</span></span>

1. <span data-ttu-id="bb109-205">I fönstret Hantera licenser för det här avtalet väljer du **+Lägg till en plan**.</span><span class="sxs-lookup"><span data-stu-id="bb109-205">In the Manage licenses window for this deal, select **+Add a plan**.</span></span>
2. <span data-ttu-id="bb109-206">Slutför fälten **Planer för den här** lösningen och **Antal** licenser och välj sedan **Uppdatera licenser.**</span><span class="sxs-lookup"><span data-stu-id="bb109-206">Complete the **Plans for this solution** and **Number of licenses** fields, and then select **Update licenses**.</span></span> <span data-ttu-id="bb109-207">Licenserna blir tillgängliga på admin.microsoft.com kunder kan hantera och tilldela till anställda.</span><span class="sxs-lookup"><span data-stu-id="bb109-207">The licenses will be available at admin.microsoft.com for customers to manage and assign to employees.</span></span>

    - <span data-ttu-id="bb109-208">Om du vill ändra antalet licenser för en befintlig plan anger du det nya numret i fältet Antal **licenser** och väljer sedan **Uppdatera licenser.**</span><span class="sxs-lookup"><span data-stu-id="bb109-208">To change the number of licenses for an existing plan, enter the new number in the **Number of licenses** field and then select **Update licenses**.</span></span>

    - <span data-ttu-id="bb109-209">Om du vill inaktivera eller ta bort licenser för ett avtal väljer du papperskorgsikonen **i fältet Åtgärder** och väljer sedan Uppdatera **licenser.**</span><span class="sxs-lookup"><span data-stu-id="bb109-209">To deactivate or remove licenses for a deal, select the trash can icon in the **Actions** field and then select **Update licenses**.</span></span>

## <a name="next-steps"></a><span data-ttu-id="bb109-210">Nästa steg</span><span class="sxs-lookup"><span data-stu-id="bb109-210">Next steps</span></span>

[<span data-ttu-id="bb109-211">Licensieringsresurser</span><span class="sxs-lookup"><span data-stu-id="bb109-211">Licensing resources</span></span>](support-resources-licensing.md)
