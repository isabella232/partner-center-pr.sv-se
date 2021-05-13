---
title: Lägga till Azure Partner Shared Services
description: Använd Azure Partner Shared Services att köpa Azure-prenumerationer för eget bruk och för att ha en enhetlig metod för att köpa, spåra och hantera Azure.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: brentserbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 11/11/2020
ms.openlocfilehash: 929907c7c6f238fb84a13622227534797f0ac949
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 05/13/2021
ms.locfileid: "109855343"
---
# <a name="add-azure-partner-shared-services-so-partners-can-buy-azure-subscriptions-for-their-own-use"></a><span data-ttu-id="76c40-103">Lägg Azure Partner Shared Services så att partner kan köpa Azure-prenumerationer för eget bruk</span><span class="sxs-lookup"><span data-stu-id="76c40-103">Add Azure Partner Shared Services so partners can buy Azure subscriptions for their own use</span></span>

<span data-ttu-id="76c40-104">**Lämpliga roller:** Global | Administratörsagent | Försäljningsagent</span><span class="sxs-lookup"><span data-stu-id="76c40-104">**Appropriate roles**: Global admin | Admin agent | Sales agent</span></span>

<span data-ttu-id="76c40-105">Azure Partner Shared Services är en ny erbjudandetyp för partner i CSP-programmet som gör det möjligt för partner att köpa Azure-prenumerationer för eget bruk.</span><span class="sxs-lookup"><span data-stu-id="76c40-105">Azure Partner Shared Services is a new offer type for partners in the CSP program enabling partners to purchase Azure subscriptions for their own use.</span></span><span data-ttu-id="76c40-106">Det skapar en möjlighet för partner att använda en enhetlig metod för att köpa, spåra och hantera Azure, utöver möjligheten att konsolidera sina Azure-licensierings- och vidareförsäljningsavtal med Microsoft.</span><span class="sxs-lookup"><span data-stu-id="76c40-106">  It creates the opportunity for partners to use a uniform method for purchasing, tracking, and managing Azure in addition to the ability to consolidate their Azure licensing and reselling agreements with Microsoft.</span></span> <span data-ttu-id="76c40-107">Med Azure Partner Shared Services har partner nu samma flexibilitet att använda Azure-prenumerationer i CSP som i Microsoft Enterprise-avtal och Web Direct-program, vilket öppnar scenarier som: skapa utvecklings- och testmiljöer, distribuera interna arbetsbelastningar och vara värd för delade tjänster eller program för flera innehavare.</span><span class="sxs-lookup"><span data-stu-id="76c40-107">With Azure Partner Shared Services, partners now have the same flexibility to use Azure subscriptions in CSP as they do in the Microsoft Enterprise Agreement and Web Direct programs, opening up scenarios such as:  build development and test environments, deploy internal workloads, and host shared services or multi-tenant applications.</span></span>  

## <a name="create-the-shared-services-tenant"></a><span data-ttu-id="76c40-108">Skapa klientorganisationen för delade tjänster</span><span class="sxs-lookup"><span data-stu-id="76c40-108">Create the shared services tenant</span></span>

1. <span data-ttu-id="76c40-109">Gå till **Inställningar**  >  **Kontoinställningar**  >  **Delade tjänster.**</span><span class="sxs-lookup"><span data-stu-id="76c40-109">Go to **Settings** > **Account settings** > **Shared services**.</span></span>

   :::image type="content" source="images/sharedservices2.png" alt-text="Kontoinställningar > delade tjänster":::

2. <span data-ttu-id="76c40-111">Om du inte redan har en klientorganisation för delade tjänster klickar du på **Skapa delade tjänster.**</span><span class="sxs-lookup"><span data-stu-id="76c40-111">If you don't already have a shared services tenant, click **Create shared services**.</span></span>

   :::image type="content" source="images/sharedservices3.png" alt-text="Skapa delade tjänster":::

3. <span data-ttu-id="76c40-113">Detta skapar en klientorganisation för delade tjänster och köper Azure CSP Shared Services-prenumerationen som ska användas för delade resurser och intern arbetsbelastning.</span><span class="sxs-lookup"><span data-stu-id="76c40-113">This creates a shared services tenant and purchases the Azure CSP Shared Services subscription, to be used for shared resources and internal workload.</span></span>

   :::image type="content" source="images/sharedservices5.png" alt-text="Skapa klientorganisationen och köpa prenumerationen":::

## <a name="about-the-azure--internalshared-services-offer"></a><span data-ttu-id="76c40-115">Om Azure – interna/delade tjänster erbjudandet</span><span class="sxs-lookup"><span data-stu-id="76c40-115">About the Azure- Internal/Shared Services offer</span></span>

- <span data-ttu-id="76c40-116">Prenumerationen Azure – interna/delade tjänster en ny Azure-erbjudandetyp i CSP som nås via Partnercenter och som partner får för sin egen användning av Azure.</span><span class="sxs-lookup"><span data-stu-id="76c40-116">The Azure - Internal/Shared Services subscription is a new Azure offer type in CSP accessed through Partner Center that partners get for their own use of Azure.</span></span>

- <span data-ttu-id="76c40-117">Azure Partner Shared Services prenumerationer är berättigade och kan användas för att köpa RU:er.</span><span class="sxs-lookup"><span data-stu-id="76c40-117">Azure Partner Shared Services subscriptions are eligible and can be used to purchase RIs.</span></span>

- <span data-ttu-id="76c40-118">Det Azure – interna/delade tjänster erbjudandet kan endast tillämpas på klientorganisationen för delade tjänster.</span><span class="sxs-lookup"><span data-stu-id="76c40-118">The Azure - Internal/Shared Services offer can only be applied to the shared services tenant.</span></span>

- <span data-ttu-id="76c40-119">Den primära användningen för Azure – interna/delade tjänster-prenumerationen är så att du kan använda Azure i dina egna utvecklingssyften.</span><span class="sxs-lookup"><span data-stu-id="76c40-119">The primary use for the Azure - Internal/Shared Services subscription is so that you can use Azure for your own development purposes.</span></span> <span data-ttu-id="76c40-120">Den delade klientorganisation som du använder för att etablera det här erbjudandet kan inte användas för andra tjänster, till exempel Office 365- eller Dynamics-licenser.</span><span class="sxs-lookup"><span data-stu-id="76c40-120">The shared tenant you use to provision this offer cannot be used for other services such as Office 365 or Dynamics licenses.</span></span>

- <span data-ttu-id="76c40-121">Du kan avbryta prenumerationen precis som vilken annan prenumeration som helst.</span><span class="sxs-lookup"><span data-stu-id="76c40-121">You can cancel the subscription like any other subscription.</span></span> <span data-ttu-id="76c40-122">Gå till inställningarna **Visa alla**  >    >  **Delade tjänster**.</span><span class="sxs-lookup"><span data-stu-id="76c40-122">Go to the **settings** > **View all settings** > **Shared services**.</span></span> <span data-ttu-id="76c40-123">Välj den Azure – interna/delade tjänster prenumerationen och avbryt den.</span><span class="sxs-lookup"><span data-stu-id="76c40-123">Select the Azure - Internal/Shared Services subscription and cancel it.</span></span>

## <a name="accessing-azure-partner-shared-services-consumption-details"></a><span data-ttu-id="76c40-124">Åtkomst till Azure Partner Shared Services förbrukningsinformation</span><span class="sxs-lookup"><span data-stu-id="76c40-124">Accessing Azure Partner Shared Services consumption details</span></span>

<span data-ttu-id="76c40-125">Du hittar Azure-förbrukningen på CSP-fakturan och avstämningsfilen.</span><span class="sxs-lookup"><span data-stu-id="76c40-125">You will find the Azure consumption on your CSP invoice and the reconciliation file.</span></span> <span data-ttu-id="76c40-126">Den inkluderas som en del Microsoft Azure i radobjektet på fakturan.</span><span class="sxs-lookup"><span data-stu-id="76c40-126">It will be included as part of Microsoft Azure line item in the invoice.</span></span> <span data-ttu-id="76c40-127">Den detaljerade förbrukningsinformationen blir tillgänglig i avstämningsfilen som loggas mot klientorganisationen som skapades för det här erbjudandet.</span><span class="sxs-lookup"><span data-stu-id="76c40-127">The detailed consumption information will be available in the reconciliation file logged against the tenant that was created for this offer.</span></span>

## <a name="azure-partner-shared-services-pricing"></a><span data-ttu-id="76c40-128">Azure Partner Shared Services prissättning</span><span class="sxs-lookup"><span data-stu-id="76c40-128">Azure Partner Shared Services pricing</span></span>

<span data-ttu-id="76c40-129">Om du vill se den nya prisfilen Azure Partner Shared Services du **till Säljpriser** och erbjudanden och  >   väljer den aktuella månadens prislista.</span><span class="sxs-lookup"><span data-stu-id="76c40-129">To see the new pricing file for Azure Partner Shared Services, go to **Sell** > **Pricing and offers** and select the current month's price list.</span></span> <span data-ttu-id="76c40-130">Under de kommande veckorna släpps även ett specifikt priskort-API.</span><span class="sxs-lookup"><span data-stu-id="76c40-130">In the coming weeks, a specific rate card api will also be released.</span></span>

## <a name="marketplace-offers-and-azure-partner-shared-services"></a><span data-ttu-id="76c40-131">Marketplace-erbjudanden och Azure Partner Shared Services</span><span class="sxs-lookup"><span data-stu-id="76c40-131">Marketplace offers and Azure Partner Shared Services</span></span>

<span data-ttu-id="76c40-132">Från och med 1 mars 2019 stöder Azure Partner Shared Services (APSS) inte längre Marketplace-erbjudanden.</span><span class="sxs-lookup"><span data-stu-id="76c40-132">As of March 1, 2019, Azure Partner Shared Services (APSS) no longer supports Marketplace offers.</span></span>

|<span data-ttu-id="76c40-133">**Marketplace-support**</span><span class="sxs-lookup"><span data-stu-id="76c40-133">**Marketplace support**</span></span>   |<span data-ttu-id="76c40-134">**APSS stöds före 1 mars 2019**</span><span class="sxs-lookup"><span data-stu-id="76c40-134">**APSS supported before March 1, 2019**</span></span>|<span data-ttu-id="76c40-135">**Efter den 1 mars 2019**</span><span class="sxs-lookup"><span data-stu-id="76c40-135">**After March 1, 2019**</span></span>|
|---------------------------|:----------------------------|:-------------------|
|<span data-ttu-id="76c40-136">Bring your own license (BYOL) och kostnadsfria tjänster</span><span class="sxs-lookup"><span data-stu-id="76c40-136">Bring your own license (BYOL) and free services</span></span>   | <span data-ttu-id="76c40-137">Ja</span><span class="sxs-lookup"><span data-stu-id="76c40-137">Yes</span></span>   | <span data-ttu-id="76c40-138">Inga</span><span class="sxs-lookup"><span data-stu-id="76c40-138">No</span></span>|
|<span data-ttu-id="76c40-139">Andra Marketplace-erbjudanden från tredje part</span><span class="sxs-lookup"><span data-stu-id="76c40-139">Other third-party marketplace offers</span></span>   | <span data-ttu-id="76c40-140">Inga</span><span class="sxs-lookup"><span data-stu-id="76c40-140">No</span></span>   |<span data-ttu-id="76c40-141">Inga</span><span class="sxs-lookup"><span data-stu-id="76c40-141">No</span></span>|

<span data-ttu-id="76c40-142">Partner som har BYOL eller kostnadsfria tjänster som distribueras med APSS påverkas inte. Efter den 1 mars 2019 kommer de dock inte att kunna köpa nya BYOL eller kostnadsfria tjänster.</span><span class="sxs-lookup"><span data-stu-id="76c40-142">Partners who have BYOL or free services deployed using APSS will not be impacted; however after March 1, 2019 they will not be able to purchase new BYOL or free services.</span></span>

<span data-ttu-id="76c40-143">Om du vill dra nytta av den fullständiga katalogen med Marketplace-erbjudanden (inte bara BYOL och kostnadsfria tjänster) rekommenderar vi att CSP-partner distribuerar delade tjänster med Azure-prenumerationer för web direct.</span><span class="sxs-lookup"><span data-stu-id="76c40-143">To take advantage of the full catalog of Marketplace offers available (not just BYOL and free services), we recommend CSP partners deploy shared services using web direct Azure subscriptions.</span></span>  <span data-ttu-id="76c40-144">CSP-partner som tidigare har distribuerat BYOL från tredje part och kostnadsfria tjänstresurser från Marketplace och vill fortsätta att använda dem och distribuera fler tredjepartserbjudanden uppmanas att migrera APSS-prenumerationen till webb direktMigrering av befintliga [Azure-prenumerationer.](/azure/cloud-solution-provider/migration/migration#migrating-existing-azure-subscriptions)</span><span class="sxs-lookup"><span data-stu-id="76c40-144">CSP partners who have deployed third-party BYOL and free service resources from the Marketplace previously and wish to continue using them and deploy more third-party offerings are encouraged to migrate the APSS subscription to web direct [Migrating Existing Azure Subscriptions](/azure/cloud-solution-provider/migration/migration#migrating-existing-azure-subscriptions).</span></span>

<span data-ttu-id="76c40-145">Partner som planerar att fortsätta använda APSS-prenumerationen efter den 1 mars 2019 och vill distribuera nya [BYOL-tjänster](https://azuremarketplace.microsoft.com/marketplace/apps?filters=byol) från tredje part eller kostnadsfria tjänster kan följa instruktionerna från ISV:er för att distribuera dem till sina APSS-prenumerationer.</span><span class="sxs-lookup"><span data-stu-id="76c40-145">Partners, who plan to continue using APSS subscription after the March 1, 2019 and wish to deploy new third-party [BYOL services](https://azuremarketplace.microsoft.com/marketplace/apps?filters=byol) or free services, can follow the instructions from ISVs to deploy these to their APSS subscriptions.</span></span>

## <a name="next-steps"></a><span data-ttu-id="76c40-146">Nästa steg</span><span class="sxs-lookup"><span data-stu-id="76c40-146">Next steps</span></span>

- [<span data-ttu-id="76c40-147">Sälja programvaruprenumerationer via CSP</span><span class="sxs-lookup"><span data-stu-id="76c40-147">Sell software subscriptions through CSP</span></span>](csp-software-subscriptions.md)