---
title: Co-Sälj koppling för Salesforce CRM-partner Center
ms.topic: how-to
ms.date: 09/29/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Synkronisera dina referenser i Partner Center med Salesforce CRM. Säljare kan sedan sälja tillsammans med Microsoft från dina CRM-system.
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: b73f0b24538daa18b93fa206fce5eda1ab9bc9b9
ms.sourcegitcommit: 7e32544cf91f932cbeb053c9de506ba9ee773fe2
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 11/20/2020
ms.locfileid: "94947859"
---
# <a name="co-sell-connector-for-salesforce-crm---overview"></a><span data-ttu-id="32413-104">Co-Sälj koppling för Salesforce CRM – översikt</span><span class="sxs-lookup"><span data-stu-id="32413-104">Co-sell connector for Salesforce CRM - overview</span></span>

### <a name="appropriate-roles"></a><span data-ttu-id="32413-105">Lämpliga roller</span><span class="sxs-lookup"><span data-stu-id="32413-105">Appropriate roles</span></span>

- <span data-ttu-id="32413-106">Referens administratör</span><span class="sxs-lookup"><span data-stu-id="32413-106">Referrals admin</span></span>
- <span data-ttu-id="32413-107">System administratör eller systemanpassare på CRM</span><span class="sxs-lookup"><span data-stu-id="32413-107">System admin or system customizer on the CRM</span></span>

<span data-ttu-id="32413-108">Partner Center Co-sälje Connector gör det möjligt för dina säljare att sälja med Microsoft från dina CRM-system.</span><span class="sxs-lookup"><span data-stu-id="32413-108">Partner Center co-sell connector enables your sellers to co-sell with Microsoft from within your CRM systems.</span></span> <span data-ttu-id="32413-109">De behöver inte tränas att använda Partner Center för att hantera samförsäljnings avtal.</span><span class="sxs-lookup"><span data-stu-id="32413-109">They won’t have to be trained to use Partner Center to manage Co-sell deals.</span></span> <span data-ttu-id="32413-110">Med hjälp av samförsäljnings kopplingarna kan du skapa en ny samförsäljnings hänvisning för att engagera en Microsoft-säljare, ta emot hänvisningar från Microsoft-säljaren, acceptera/neka referenser, ändra avtals data som avtals värde och stängnings datum.</span><span class="sxs-lookup"><span data-stu-id="32413-110">Using the Co-sell connectors, you can create a new Co-sell referral to engage a Microsoft seller, receive referrals from the Microsoft seller, accept/decline referrals, modify deal data such as deal value, and closing date.</span></span>  <span data-ttu-id="32413-111">Du kan också ta emot uppdateringar från Microsoft-säljarna om dessa samförsäljnings avtal.</span><span class="sxs-lookup"><span data-stu-id="32413-111">You can also receive any updates from the Microsoft sellers on these Co-sell deals.</span></span> <span data-ttu-id="32413-112">Du kan göra så att alla dina referenser fungerar när du arbetar i valfri CRM i stället för i Partner Center.</span><span class="sxs-lookup"><span data-stu-id="32413-112">You can do all of your referrals work while working within the CRM of your choice rather than in Partner Center.</span></span> 

<span data-ttu-id="32413-113">Lösningen baseras på Microsoft Power automatiserings lösning och använder API: er för partner Center.</span><span class="sxs-lookup"><span data-stu-id="32413-113">The solution is based on Microsoft Power Automate Solution and uses Partner Center APIs.</span></span>

## <a name="before-you-install---pre-requisites"></a><span data-ttu-id="32413-114">Innan du installerar-krav</span><span class="sxs-lookup"><span data-stu-id="32413-114">Before you install - pre-requisites</span></span>

|<span data-ttu-id="32413-115">**Ämnen**</span><span class="sxs-lookup"><span data-stu-id="32413-115">**Topics**</span></span>   |<span data-ttu-id="32413-116">**Detaljer**</span><span class="sxs-lookup"><span data-stu-id="32413-116">**Details**</span></span>   |<span data-ttu-id="32413-117">**Länkar**</span><span class="sxs-lookup"><span data-stu-id="32413-117">**Links**</span></span>   |
|--------------|--------------------|------|
|<span data-ttu-id="32413-118">Microsoft Partner Network-ID</span><span class="sxs-lookup"><span data-stu-id="32413-118">Microsoft Partner Network ID</span></span> |<span data-ttu-id="32413-119">Du behöver ett giltigt MPN-ID</span><span class="sxs-lookup"><span data-stu-id="32413-119">You need a valid MPN ID</span></span>|<span data-ttu-id="32413-120">För att ansluta till [MPN](https://partner.microsoft.com/)</span><span class="sxs-lookup"><span data-stu-id="32413-120">To join [MPN](https://partner.microsoft.com/)</span></span>|
|<span data-ttu-id="32413-121">Färdiga försäljnings produkter</span><span class="sxs-lookup"><span data-stu-id="32413-121">Co-sell ready</span></span>|<span data-ttu-id="32413-122">Din lösning för IP/tjänster måste vara samförsäljnings klar.</span><span class="sxs-lookup"><span data-stu-id="32413-122">Your IP/Services solution must be co-sell ready.</span></span>|[<span data-ttu-id="32413-123">Sälj med Microsoft</span><span class="sxs-lookup"><span data-stu-id="32413-123">Sell with Microsoft</span></span>](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|<span data-ttu-id="32413-124">Partnercenter-konto</span><span class="sxs-lookup"><span data-stu-id="32413-124">Partner Center account</span></span>|<span data-ttu-id="32413-125">Det MPN-ID som är kopplat till Partner Center-klienten måste vara samma som det MPN-ID som är kopplat till din co-Sälj-lösning.</span><span class="sxs-lookup"><span data-stu-id="32413-125">The MPN ID associated with the Partner Center tenant must be same as the MPN ID associated with your Co-sell solution.</span></span> <span data-ttu-id="32413-126">Kontrol lera att du kan se dina samförsäljnings referenser på Partner Center-portalen innan du distribuerar anslutningarna.</span><span class="sxs-lookup"><span data-stu-id="32413-126">Verify that you can see your co-sell referrals in Partner Center portal before deploying the connectors.</span></span>|[<span data-ttu-id="32413-127">Hantera ditt konto</span><span class="sxs-lookup"><span data-stu-id="32413-127">Manage your account</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="32413-128">Användar roller för partner Center</span><span class="sxs-lookup"><span data-stu-id="32413-128">Partner Center user roles</span></span>|<span data-ttu-id="32413-129">Den medarbetare som ska installera och använda anslutningarna måste vara en referens administratör</span><span class="sxs-lookup"><span data-stu-id="32413-129">The employee who will install and use the connectors must be a Referrals admin</span></span>|[<span data-ttu-id="32413-130">Tilldela användarroller och -behörigheter</span><span class="sxs-lookup"><span data-stu-id="32413-130">Assign users roles and permissions</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="32413-131">Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="32413-131">Salesforce CRM</span></span>|<span data-ttu-id="32413-132">Användar rollen CRM är system administratör eller systemanpassare</span><span class="sxs-lookup"><span data-stu-id="32413-132">The CRM user role is System admin or System customizer</span></span>|[<span data-ttu-id="32413-133">Tilldela roller i Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="32413-133">Assign roles in Salesforce CRM</span></span>](https://help.salesforce.com/articleView?id=assigning_users_to_roles.htm&type=5)|
|<span data-ttu-id="32413-134">Flödes konto för automatiserad energi</span><span class="sxs-lookup"><span data-stu-id="32413-134">Power Automate Flow Account</span></span>|<span data-ttu-id="32413-135">Ett aktivt [energi automatiserat](https://flow.microsoft.com) konto för CRM-systemadministratören eller systemanpassaren.</span><span class="sxs-lookup"><span data-stu-id="32413-135">An active [Power Automate](https://flow.microsoft.com) account for the CRM System admin or System customizer.</span></span> <span data-ttu-id="32413-136">Användaren ska logga in i [energi spar läge](https://flow.microsoft.com) minst en gång före installationen.</span><span class="sxs-lookup"><span data-stu-id="32413-136">That user should sign into [Power Automate](https://flow.microsoft.com) at least once before installation.</span></span>|

## <a name="installation-of-salesforce-package-for-microsoft-custom-fields"></a><span data-ttu-id="32413-137">Installation av Salesforce-paket för anpassade Microsoft-fält</span><span class="sxs-lookup"><span data-stu-id="32413-137">Installation of Salesforce Package for Microsoft Custom Fields</span></span> 

<span data-ttu-id="32413-138">Om du vill synkronisera hänvisningarna över partner Center och Salesforce CRM måste den automatiserade lösningen för att tydligt identifiera Microsoft-speciella hänvisnings fält.</span><span class="sxs-lookup"><span data-stu-id="32413-138">To synchronize the referrals across Partner Center and Salesforce CRM, the Power Automate solution needs to clearly identify Microsoft specific referral fields.</span></span> <span data-ttu-id="32413-139">Denna avgränsning ger partner säljares team möjlighet att bestämma vilka hänvisningar de vill dela med Microsoft för samförsäljning.</span><span class="sxs-lookup"><span data-stu-id="32413-139">This demarcation provides partner seller teams with the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

1. <span data-ttu-id="32413-140">I Salesforce aktiverar du **anteckningar** och lägger till det i listan relaterade affärs möjligheter.</span><span class="sxs-lookup"><span data-stu-id="32413-140">In Salesforce, activate **Notes** and add it to the opportunities related list.</span></span> 
[<span data-ttu-id="32413-141">Referens</span><span class="sxs-lookup"><span data-stu-id="32413-141">Reference</span></span>](https://help.salesforce.com/articleView?err=1&id=notes_admin_setup.htm&type=5)

2. <span data-ttu-id="32413-142">Aktivera **affärs möjlighets team** genom att följa stegen:</span><span class="sxs-lookup"><span data-stu-id="32413-142">Activate **Opportunity teams** by following the steps:</span></span> 
    - <span data-ttu-id="32413-143">I installations programmet använder du rutan **snabb sökning** för att hitta team inställningar för affärs möjligheter.</span><span class="sxs-lookup"><span data-stu-id="32413-143">In Setup, use the **Quick Find** box to locate Opportunity Team Settings.</span></span>
    - <span data-ttu-id="32413-144">Definiera inställningarna efter behov.</span><span class="sxs-lookup"><span data-stu-id="32413-144">Define the settings as needed.</span></span>
[<span data-ttu-id="32413-145">Referens</span><span class="sxs-lookup"><span data-stu-id="32413-145">Reference</span></span>](https://help.salesforce.com/articleView?id=teamselling_enabling.htm&type=5]) 

3. <span data-ttu-id="32413-146">I Salesforce installerar du anpassade fält och objekt med hjälp av Package Installer nedan.</span><span class="sxs-lookup"><span data-stu-id="32413-146">In Salesforce, install custom fields and objects using package installer below.</span></span>
  
<span data-ttu-id="32413-147">Gå [hit](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t2w000006Vs9a) om du vill installera paketet i valfritt företag:</span><span class="sxs-lookup"><span data-stu-id="32413-147">Go [here](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t2w000006Vs9a) to install the package into any company:</span></span>


<span data-ttu-id="32413-148">Obs! Om du installerar i ett begränsat läge måste du ersätta den inledande delen av URL: en med http://test.salesforce.com</span><span class="sxs-lookup"><span data-stu-id="32413-148">Note: If you are installing into a sandbox you must replace the initial portion of the URL with http://test.salesforce.com</span></span>

4. <span data-ttu-id="32413-149">I Salesforce lägger du till Microsoft-lösningar i listan relaterad **affärs möjlighet** .</span><span class="sxs-lookup"><span data-stu-id="32413-149">In Salesforce, add Microsoft Solutions to the **Opportunity** related list.</span></span> <span data-ttu-id="32413-150">När du har lagt till klickar du på **SKIFT nyckel** ikonen och uppdaterar egenskaperna</span><span class="sxs-lookup"><span data-stu-id="32413-150">Once added, click on the **wrench** icon and update properties</span></span>

## <a name="best-practice-test-before-you-go-live"></a><span data-ttu-id="32413-151">Bästa praxis: testa innan du går live</span><span class="sxs-lookup"><span data-stu-id="32413-151">Best Practice: Test before you go live</span></span>

<span data-ttu-id="32413-152">Innan du installerar, konfigurerar och anpassar den automatiserade energi lösningen i produktions miljön måste du testa lösningen på en mellanlagringsplatsen CRM-instans.</span><span class="sxs-lookup"><span data-stu-id="32413-152">Before you install, configure, and customize the Power Automate solution on the production environment, be sure to test the solution on a staging CRM instance.</span></span>

- <span data-ttu-id="32413-153">Installera Microsoft Power automatiserings lösning på en mellanlagringsplatss miljö/CRM-instans.</span><span class="sxs-lookup"><span data-stu-id="32413-153">Install Microsoft Power Automate solution on a staging environment/CRM instance.</span></span>

- <span data-ttu-id="32413-154">Gör en kopia av lösningen och kör din konfiguration och automatisera automatiserade flödes anpassningar i mellanlagrings miljön.</span><span class="sxs-lookup"><span data-stu-id="32413-154">Make a copy of the solution and run your configuration and Power Automate flow customizations on the staging environment.</span></span>

- <span data-ttu-id="32413-155">Testa lösningen på en mellanlagrings-/CRM-instans.</span><span class="sxs-lookup"><span data-stu-id="32413-155">Test the solution on a staging/CRM instance.</span></span>

- <span data-ttu-id="32413-156">Vid lyckad import importerar du som en hanterad lösning till produktions instansen.</span><span class="sxs-lookup"><span data-stu-id="32413-156">On success, import as a managed solution to the production instance.</span></span>

## <a name="install-partner-center-referrals-synchronization-for-salesforce-crm"></a><span data-ttu-id="32413-157">Installera synkronisering av Partner Center-referenser för Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="32413-157">Install Partner Center Referrals Synchronization for Salesforce CRM</span></span>

1. <span data-ttu-id="32413-158">Gå till [Power automatisera](https://flow.microsoft.com) och välj **miljöer** i det högra övre hörnet.</span><span class="sxs-lookup"><span data-stu-id="32413-158">Go to [Power Automate](https://flow.microsoft.com) and select **Environments** on the right top corner.</span></span> <span data-ttu-id="32413-159">Då visas tillgängliga CRM-instanser.</span><span class="sxs-lookup"><span data-stu-id="32413-159">This will show you the available CRM instances.</span></span>

2. <span data-ttu-id="32413-160">Välj lämplig CRM-instans i list rutan i det högra övre hörnet.</span><span class="sxs-lookup"><span data-stu-id="32413-160">Select the appropriate CRM instance from the drop-down on the right top corner.</span></span>

3. <span data-ttu-id="32413-161">Välj **lösningar** i det vänstra navigerings fältet.</span><span class="sxs-lookup"><span data-stu-id="32413-161">Select **Solutions** on the left navigation bar.</span></span>

4. <span data-ttu-id="32413-162">Klicka på länken **Öppna AppSource** på den översta menyn.</span><span class="sxs-lookup"><span data-stu-id="32413-162">Click on the **Open AppSource** link on the top menu.</span></span>

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="Öppna AppSource":::

5. <span data-ttu-id="32413-164">Sök efter **partner Center-referenser för Salesforce** i popup-fönstret.</span><span class="sxs-lookup"><span data-stu-id="32413-164">Search for **Partner Center Referrals Connectors for Salesforce** in the pop-up screen.</span></span>  

   :::image type="content" source="images/salesforce/salesforce1.png" alt-text="Salesforce":::

6. <span data-ttu-id="32413-166">Klicka på knappen **Hämta nu** och **Fortsätt** sedan.</span><span class="sxs-lookup"><span data-stu-id="32413-166">Click the **Get it now** button and then **Continue**.</span></span>

7. <span data-ttu-id="32413-167">Då öppnas sidan där du kan välja Salesforce CRM-miljön för att installera programmet.</span><span class="sxs-lookup"><span data-stu-id="32413-167">This opens the page where you can select the Salesforce CRM  environment to install application.</span></span>  <span data-ttu-id="32413-168">Godkänn de allmänna villkoren.</span><span class="sxs-lookup"><span data-stu-id="32413-168">Agree to terms and conditions.</span></span>

   :::image type="content" source="images/salesforce/available-crm.png" alt-text="Tillgängliga CRMS":::

8. <span data-ttu-id="32413-170">Sedan dirigeras du till sidan **Hantera dina lösningar** .</span><span class="sxs-lookup"><span data-stu-id="32413-170">You're then directed to the **Manage your solutions** page.</span></span>  <span data-ttu-id="32413-171">Gå till "Partner Center-referenser" genom att använda pilknapparna längst ned på sidan.</span><span class="sxs-lookup"><span data-stu-id="32413-171">Navigate to "Partner Center Referrals" by using the arrow buttons on the bottom of the page.</span></span> <span data-ttu-id="32413-172">**Installationen är schemalagd** bör visas bredvid lösningen för partner Center-hänvisningar.</span><span class="sxs-lookup"><span data-stu-id="32413-172">**Installation scheduled** should appear next to Partner Center Referrals solution.</span></span> <span data-ttu-id="32413-173">Installationen tar 10-15 minuter.</span><span class="sxs-lookup"><span data-stu-id="32413-173">Installation will take 10-15 minutes.</span></span>

9. <span data-ttu-id="32413-174">När installationen är klar navigerar du tillbaka till [Automatisera](https://flow.microsoft.com) och väljer **lösningar** från det vänstra navigerings fältet.</span><span class="sxs-lookup"><span data-stu-id="32413-174">Once the installation is complete, navigate back to [Power Automate](https://flow.microsoft.com) and select **Solutions** from left navigation area.</span></span> <span data-ttu-id="32413-175">Observera att **synkronisering av Partner Center för Salesforce** är tillgängligt i lösnings listan.</span><span class="sxs-lookup"><span data-stu-id="32413-175">Notice that **Partner Center Referrals Synchronization for Salesforce** is available in the Solutions list.</span></span>

10. <span data-ttu-id="32413-176">Välj **synkronisering av Partner Center-referenser för Salesforce**.</span><span class="sxs-lookup"><span data-stu-id="32413-176">Select **Partner Center Referrals Synchronization for Salesforce**.</span></span> <span data-ttu-id="32413-177">Följande energi flöden och entiteter är tillgängliga:</span><span class="sxs-lookup"><span data-stu-id="32413-177">The following Power Automate flows and entities are available:</span></span>

    :::image type="content" source="images/cosellconnectors/salesforce10.png" alt-text="Salesforce-flöden":::



## <a name="configure-the-solution"></a><span data-ttu-id="32413-179">Konfigurera lösningen</span><span class="sxs-lookup"><span data-stu-id="32413-179">Configure the solution</span></span>

1. <span data-ttu-id="32413-180">När du har installerat lösningen i din CRM-instans går du tillbaka till [Energis par](https://flow.microsoft.com/).</span><span class="sxs-lookup"><span data-stu-id="32413-180">Once you have installed the solution in your CRM instance, navigate back to [Power Automate](https://flow.microsoft.com/).</span></span>

2. <span data-ttu-id="32413-181">I list rutan **miljöer** i det högra hörnet väljer du den CRM-instans där du installerade den automatiserade energi lösningen.</span><span class="sxs-lookup"><span data-stu-id="32413-181">From the **Environments** drop-down on the right top corner, select the CRM instance where you installed the Power Automate solution.</span></span>
3. <span data-ttu-id="32413-182">Du måste skapa anslutningar som associerar de tre användar kontona:</span><span class="sxs-lookup"><span data-stu-id="32413-182">You will need to create connections that associate the three user accounts:</span></span>
    - <span data-ttu-id="32413-183">Partner Center-användare med referenser för administratörs behörighet</span><span class="sxs-lookup"><span data-stu-id="32413-183">Partner Center user with referrals admin credentials</span></span>
    - <span data-ttu-id="32413-184">Partnercenter-händelser</span><span class="sxs-lookup"><span data-stu-id="32413-184">Partner Center Events</span></span>
    - <span data-ttu-id="32413-185">CRM-administratören med de energi automatiserade flödena i lösningen.</span><span class="sxs-lookup"><span data-stu-id="32413-185">CRM admin with the Power Automate flows in the solution.</span></span>
4. <span data-ttu-id="32413-186">Välj **anslutningar** i det vänstra navigerings fältet och välj lösningen "Partner Center-hänvisningar" i listan.</span><span class="sxs-lookup"><span data-stu-id="32413-186">Select **Connections** from the left navigation bar and select the "Partner Center Referrals" solution from the list.</span></span>

5. <span data-ttu-id="32413-187">Skapa en anslutning genom att klicka på **skapa en anslutning**.</span><span class="sxs-lookup"><span data-stu-id="32413-187">Create a connection by clicking **Create a connection**.</span></span>

:::image type="content" source="images/cosellconnectors/salesforce12.png" alt-text="Skapa anslutning":::

- <span data-ttu-id="32413-189">Sök efter partner Center-referenser (för hands version) i Sök fältet i det övre högra hörnet.</span><span class="sxs-lookup"><span data-stu-id="32413-189">Search for Partner Center Referrals (preview) in the search bar on the top right corner.</span></span>

- <span data-ttu-id="32413-190">Skapa en anslutning för din partner Center-användare med rollen autentiseringsuppgifter för referral admin.</span><span class="sxs-lookup"><span data-stu-id="32413-190">Create a connection for your Partner Center user with the credentials role of Referrals admin.</span></span>

-  <span data-ttu-id="32413-191">Skapa sedan en anslutning för partner Center-händelser för din partner Center-användare med autentiseringsuppgifterna för referral admin.</span><span class="sxs-lookup"><span data-stu-id="32413-191">Next, create a Partner Center Events connection for your Partner Center user with the credentials of Referrals admin.</span></span>

- <span data-ttu-id="32413-192">Skapa en anslutning för Salesforce för administratörs användaren för CRM.</span><span class="sxs-lookup"><span data-stu-id="32413-192">Create a connection for Salesforce for the CRM administrator user.</span></span>

-  <span data-ttu-id="32413-193">När du har lagt till alla anslutningar bör du se följande anslutningar i din miljö:</span><span class="sxs-lookup"><span data-stu-id="32413-193">Once you have all the Connections added, you should see the following Connections in your environment:</span></span>

 :::image type="content" source="images/cosellconnectors/salesforce13.png" alt-text="Observera anslutningar":::

### <a name="edit-the-connections"></a><span data-ttu-id="32413-195">Redigera anslutningarna</span><span class="sxs-lookup"><span data-stu-id="32413-195">Edit the connections</span></span>

1. <span data-ttu-id="32413-196">Gå tillbaka till sidan lösningar och välj **standard lösning**.</span><span class="sxs-lookup"><span data-stu-id="32413-196">Return to the Solutions page and select **Default Solution**.</span></span>  <span data-ttu-id="32413-197">Välj **anslutnings referens (för hands version)** genom att klicka på **alla**.</span><span class="sxs-lookup"><span data-stu-id="32413-197">Select **Connection Reference (preview)** by clicking **All**.</span></span>
 
:::image type="content" source="images/cosellconnectors/salesforce14.png" alt-text="Börja redigera koppling":::

2. <span data-ttu-id="32413-199">Redigera varje anslutning en i taget genom att välja ikonen tre punkter.</span><span class="sxs-lookup"><span data-stu-id="32413-199">Edit each of the Connections one by one by selecting the three dots icon.</span></span> <span data-ttu-id="32413-200">Lägg till relevanta anslutningar.</span><span class="sxs-lookup"><span data-stu-id="32413-200">Add the relevant connections.</span></span>

:::image type="content" source="images/cosellconnectors/salesforce15.png" alt-text="Redigera anslutningar":::

3. <span data-ttu-id="32413-202">Aktivera flödena i följande ordning:</span><span class="sxs-lookup"><span data-stu-id="32413-202">Turn on the flows in the following sequence:</span></span>

- <span data-ttu-id="32413-203">Partner Center – registrering av webhook (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="32413-203">Partner Center Webhook Registration (Insider Preview)</span></span>
- <span data-ttu-id="32413-204">Skapa Co-sälje referral-Salesforce till Partner Center (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="32413-204">Create Co-sell Referral - Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="32413-205">Partner Center Microsoft Co-Sälj hänvisnings uppdateringar till Salesforce (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="32413-205">Partner Center Microsoft Co-sell Referral Updates to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="32413-206">Partner Center till Salesforce (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="32413-206">Partner Center to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="32413-207">Salesforce till Partner Center (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="32413-207">Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="32413-208">Salesforce-möjlighet till Partner Center (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="32413-208">Salesforce Opportunity to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="32413-209">Salesforce Microsoft-lösningar till Partner Center (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="32413-209">Salesforce Microsoft Solutions to Partner Center (Insider Preview)</span></span>

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a><span data-ttu-id="32413-210">Använda webhook-API: er för att registrera för resurs ändrings händelser</span><span class="sxs-lookup"><span data-stu-id="32413-210">Use Webhook APIs to register for resource change events</span></span>

<span data-ttu-id="32413-211">Med API: er för webhook i Partner Center kan du registrera för resurs ändrings händelser.</span><span class="sxs-lookup"><span data-stu-id="32413-211">The Partner Center Webhook APIs allow you to register for resource change events.</span></span> <span data-ttu-id="32413-212">De här ändrings händelserna skickas till din URL som HTTP-inlägg.</span><span class="sxs-lookup"><span data-stu-id="32413-212">These change events are sent to your url as HTTP posts.</span></span>

1. <span data-ttu-id="32413-213">Registrera din URL genom att välja **partner Center webhook Registration (Insider Preview)** energi automatisera flöde.</span><span class="sxs-lookup"><span data-stu-id="32413-213">To register your url, select **Partner Center Webhook Registration (Insider Preview)** Power Automate flow.</span></span>

2. <span data-ttu-id="32413-214">Lägg till anslutningar för (a.) partner Center användare med referenser admin-autentiseringsuppgifter (b.) partner Center-händelser som marker ATS nedan</span><span class="sxs-lookup"><span data-stu-id="32413-214">Add connections for (a.) Partner Center user with referrals admin credentials (b.) Partner Center Events as highlighted below</span></span>

   :::image type="content" source="images/cosellconnectors/triggerflow.png" alt-text="Utlösare":::

3. <span data-ttu-id="32413-216">När du gör dessa uppdateringar visas</span><span class="sxs-lookup"><span data-stu-id="32413-216">When you make these updates, you'll see</span></span>

   :::image type="content" source="images/cosellconnectors/webhook1.png" alt-text="Webhooks":::

4. <span data-ttu-id="32413-218">Spara ändringarna och välj **Aktivera**.</span><span class="sxs-lookup"><span data-stu-id="32413-218">Save your changes and select **Turn on**.</span></span>

   <span data-ttu-id="32413-219">Gör så här om du vill att Webhooks i Partner Center ska lyssna på händelse ändringar:</span><span class="sxs-lookup"><span data-stu-id="32413-219">To enable Partner Center webhooks to listen to event changes, perform the following steps:</span></span>

5. <span data-ttu-id="32413-220">Välj **partner Center till Salesforce CRM (Insider Preview)**.</span><span class="sxs-lookup"><span data-stu-id="32413-220">Select **Partner Center to Salesforce CRM (Insider Preview)**.</span></span>

6. <span data-ttu-id="32413-221">Välj **redigerings** ikonen och välj **när en http-begäran tas emot**.</span><span class="sxs-lookup"><span data-stu-id="32413-221">Select the **Edit** icon and select **When a HTTP request is received**.</span></span>

7. <span data-ttu-id="32413-222">Välj **kopierings** ikonen för att kopiera den tillhandahållna HTTP post-URL: en.</span><span class="sxs-lookup"><span data-stu-id="32413-222">Select the **Copy** icon to copy the provided HTTP POST URL.</span></span>

   :::image type="content" source="images/salesforce/copy-url.png" alt-text="Kopiera URL":::

8. <span data-ttu-id="32413-224">Välj nu "partner för webhook-registrering (Insider Preview)" i Power Center och välj **Kör**.</span><span class="sxs-lookup"><span data-stu-id="32413-224">Now select the "Partner Center Webhook Registration (Insider Preview)" Power Automate flow and select **Run**.</span></span>

9. <span data-ttu-id="32413-225">Se till att fönstret kör flöde visas i den högra rutan och klicka på **Fortsätt**.</span><span class="sxs-lookup"><span data-stu-id="32413-225">Ensure that the "Run Flow" window opens on the right-hand pane and click **Continue**.</span></span>

10. <span data-ttu-id="32413-226">Ange följande uppgifter:</span><span class="sxs-lookup"><span data-stu-id="32413-226">Enter the following details:</span></span>

    1. <span data-ttu-id="32413-227">**Http-utlösare slut punkt**: URL kopierad från föregående steg</span><span class="sxs-lookup"><span data-stu-id="32413-227">**Http Trigger Endpoint**: URL copied from earlier step</span></span>

    2. <span data-ttu-id="32413-228">**Händelser att registrera**: "referral-created" och "referral-updated"</span><span class="sxs-lookup"><span data-stu-id="32413-228">**Events to Register**: "referral-created" and "referral-updated"</span></span>

    3. <span data-ttu-id="32413-229">**Skriv över befintliga utlösare slut punkter om det finns**: Ja (detta skriver över alla befintliga slut punkter.)</span><span class="sxs-lookup"><span data-stu-id="32413-229">**Overwrite existing trigger endpoints if present**: Yes (This overwrites any existing endpoints.)</span></span>

11. <span data-ttu-id="32413-230">Välj **Kör** och välj sedan **Slutför.**</span><span class="sxs-lookup"><span data-stu-id="32413-230">Select **Run** and then select **Done.**</span></span>

<span data-ttu-id="32413-231">Webhooken kan nu lyssna på att skapa och uppdatera händelser.</span><span class="sxs-lookup"><span data-stu-id="32413-231">The webhook can now listen to create and update events.</span></span>

## <a name="customize-synchronization-steps"></a><span data-ttu-id="32413-232">Anpassa synkroniserings steg</span><span class="sxs-lookup"><span data-stu-id="32413-232">Customize synchronization steps</span></span>

<span data-ttu-id="32413-233">När samförsäljnings hänvisningar synkroniseras mellan partner Center och ditt CRM-system, visas fälten som synkroniseras på Partner Center-datorn här.</span><span class="sxs-lookup"><span data-stu-id="32413-233">When Co-sell referrals are synced between Partner Center and your CRM system, the fields that are synced on Partner Center PC are listed here.</span></span>

<span data-ttu-id="32413-234">CRM-system är ofta anpassade.</span><span class="sxs-lookup"><span data-stu-id="32413-234">Often CRM systems are highly customized.</span></span> <span data-ttu-id="32413-235">Du kan anpassa automatiserade energi flöden.</span><span class="sxs-lookup"><span data-stu-id="32413-235">You can customize the Power Automate flows.</span></span> <span data-ttu-id="32413-236">Följ guiden för fält mappning och om det behövs kan du göra lämpliga ändringar i stegen i de automatiserade energi flödena.</span><span class="sxs-lookup"><span data-stu-id="32413-236">Follow the field mapping guide, and if necessary, make appropriate changes in the steps of the Power Automate flows.</span></span>  <span data-ttu-id="32413-237">Microsoft Partner Center till CRM-mappningar tillhandahålls, men baserat på din CRM-miljö kan du välja att ytterligare anpassa fälten.</span><span class="sxs-lookup"><span data-stu-id="32413-237">Microsoft Partner Centers to CRM mappings are provided, but based on your CRM environment, you can choose to further customize the fields.</span></span>

<span data-ttu-id="32413-238">Flera steg i vart och ett av de automatiserade energi flödena kan anpassas efter dina behov.</span><span class="sxs-lookup"><span data-stu-id="32413-238">Multiple steps of each of the Power Automate flows can be customized based on your needs.</span></span> <span data-ttu-id="32413-239">Följande är exempel på tillgängliga anpassningar:</span><span class="sxs-lookup"><span data-stu-id="32413-239">The following are examples of available customizations:</span></span>

1. <span data-ttu-id="32413-240">Så här anpassar du fälten för Create-eller Update-händelserna i Partner Center till CRM referral Synchronization:</span><span class="sxs-lookup"><span data-stu-id="32413-240">To customize the fields for the create or update events in the Partner Center to CRM referral synchronization:</span></span>

   1. <span data-ttu-id="32413-241">Välj Partner Center till Salesforce CRM (Insider Preview).</span><span class="sxs-lookup"><span data-stu-id="32413-241">Select Partner Center to Salesforce CRM (Insider Preview).</span></span>

   2. <span data-ttu-id="32413-242">Välj **Redigera** för att redigera/anpassa det energi automatiserade flödet.</span><span class="sxs-lookup"><span data-stu-id="32413-242">Select **Edit** to edit/customize the Power Automate flow.</span></span>

   3. <span data-ttu-id="32413-243">Välj **(omfång) synkronisera lead eller affärs möjlighet**.</span><span class="sxs-lookup"><span data-stu-id="32413-243">Select **(Scope) Synchronize the lead or opportunity**.</span></span>

2. <span data-ttu-id="32413-244">Om du vill anpassa fält mappningar för CRM för skapa händelser väljer du **om den är ny delad affärs möjlighet och sedan**.</span><span class="sxs-lookup"><span data-stu-id="32413-244">To customize CRM field mappings for create events, select **If it’s new Shared opportunity, then**.</span></span> <span data-ttu-id="32413-245">Välj under steget **om ja** och expandera sedan **skapa en ny affärs möjlighet i CRM**.</span><span class="sxs-lookup"><span data-stu-id="32413-245">Select the sub-step **if yes** and then expand **Creating a new opportunity in the CRM**.</span></span> <span data-ttu-id="32413-246">Du kan redigera mappningarna i det här avsnittet med hjälp av fält mappnings guiden.</span><span class="sxs-lookup"><span data-stu-id="32413-246">You can edit the mappings in this section using the Field Mapping Guide.</span></span>

   1. <span data-ttu-id="32413-247">Om du vill anpassa fält mappningar för CRM för uppdaterings händelser klickar du på steget "(omfattning) synkronisera lead eller affärs möjlighet".</span><span class="sxs-lookup"><span data-stu-id="32413-247">To customize CRM field mappings for update events, click on the step "(Scope) Synchronize the lead or opportunity".</span></span>

   2. <span data-ttu-id="32413-248">Välj **om det är en uppdatering av en affärs möjlighet och sedan**.</span><span class="sxs-lookup"><span data-stu-id="32413-248">Select **If it’s an update to an opportunity, then**.</span></span> <span data-ttu-id="32413-249">Välj under steget **om ja** och expandera sedan **differensen mellan affärs möjlighets objekt i Partner Center och CRM**.</span><span class="sxs-lookup"><span data-stu-id="32413-249">Select the substep **if yes** and then expand **If difference between the opportunity objects in Partner Center and CRM, then**.</span></span>  

   3. <span data-ttu-id="32413-250">Välj **om ja** följt av **Uppdatera befintlig affärs möjlighet**</span><span class="sxs-lookup"><span data-stu-id="32413-250">Select **If yes** followed with **Update existing opportunity**</span></span>

3. <span data-ttu-id="32413-251">Så här anpassar du fälten för CRM till PC referral-synkronisering för uppdaterings händelser:</span><span class="sxs-lookup"><span data-stu-id="32413-251">To customize the fields for CRM to PC referral synchronization for update events:</span></span>

   1. <span data-ttu-id="32413-252">Välj **Redigera**  för att redigera/anpassa det energi automatiserade flödet.</span><span class="sxs-lookup"><span data-stu-id="32413-252">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   2. <span data-ttu-id="32413-253">Välj **(omfång) synkronisera affärs möjligheten**.</span><span class="sxs-lookup"><span data-stu-id="32413-253">Select **(Scope) Synchronize the opportunity**.</span></span>

   3. <span data-ttu-id="32413-254">För att anpassa fält mappningar för CRM (baserat på fält mappnings guide) för uppdaterings händelser väljer du **om det finns skillnader mellan lead-objekten i Partner Center och CRM**.</span><span class="sxs-lookup"><span data-stu-id="32413-254">For customizing CRM field mappings (based on field mappings guide) for update events, select **If there is difference between the lead objects in Partner Center and CRM, then**.</span></span>

   4. <span data-ttu-id="32413-255">Välj under steget **om ja** och expandera sedan steget **Uppdatera en referens med affärs möjlighets data**.</span><span class="sxs-lookup"><span data-stu-id="32413-255">Select the sub-step **if yes** and then expand the step **Update a referral with opportunity data**.</span></span>

   <span data-ttu-id="32413-256">Du kan redigera mappningarna i det här avsnittet baserat på fält mappnings guiden.</span><span class="sxs-lookup"><span data-stu-id="32413-256">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

4. <span data-ttu-id="32413-257">Vill du anpassa fälten för synkronisering av CRM till PC-hänvisning för Create Events?</span><span class="sxs-lookup"><span data-stu-id="32413-257">To customize the fields for CRM to PC referral synchronization for create events?</span></span>

   1. <span data-ttu-id="32413-258">Välj **Redigera**  för att redigera/anpassa det energi automatiserade flödet.</span><span class="sxs-lookup"><span data-stu-id="32413-258">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   2. <span data-ttu-id="32413-259">Välj **(omfång)-synkronisering av referenser.**</span><span class="sxs-lookup"><span data-stu-id="32413-259">Select **(Scope) Synchronizing Referrals.**</span></span>

   3. <span data-ttu-id="32413-260">För att anpassa fält mappningar för CRM (baserat på fält mappnings guide) för skapa händelser väljer du **skapa Microsoft referral**.</span><span class="sxs-lookup"><span data-stu-id="32413-260">For customizing CRM field mappings (based on field mappings guide) for create events, select **Create Microsoft Referral**.</span></span>

<span data-ttu-id="32413-261">Du kan redigera mappningarna i det här avsnittet baserat på fält mappnings guiden.</span><span class="sxs-lookup"><span data-stu-id="32413-261">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>


## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a><span data-ttu-id="32413-262">Slutförd dubbelriktad referens synkronisering från slut punkt till slut punkt</span><span class="sxs-lookup"><span data-stu-id="32413-262">End-to-end bi-directional co-sell referral synchronization</span></span>

<span data-ttu-id="32413-263">När du har installerat, konfigurerat och anpassat den automatiserade lösningen för Energis par kan du testa synkroniseringen av referenser för samförsäljning mellan Salesforce CRM och partner Center.</span><span class="sxs-lookup"><span data-stu-id="32413-263">Once you have installed, configured, and customized the Power Automate solution, you can test for Co-sell referrals synchronization between Salesforce CRM and Partner Center.</span></span>

### <a name="pre-requisites"></a><span data-ttu-id="32413-264">Förutsättningar</span><span class="sxs-lookup"><span data-stu-id="32413-264">Pre-requisites</span></span>

<span data-ttu-id="32413-265">Om du vill synkronisera hänvisningarna över partner Center och Salesforce CRM måste den automatiserade lösningen för automatisk avgränsning av de Microsoft-speciella hänvisnings fälten.</span><span class="sxs-lookup"><span data-stu-id="32413-265">To synchronize the referrals across Partner Center and Salesforce CRM, the Power Automate solution needs to clearly demarcate Microsoft-specific referral fields.</span></span> <span data-ttu-id="32413-266">Den här identifieringen ger dina säljar grupper möjlighet att bestämma vilka hänvisningar de vill dela med Microsoft för samförsäljning.</span><span class="sxs-lookup"><span data-stu-id="32413-266">This identification provides your seller teams with the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

<span data-ttu-id="32413-267">En uppsättning anpassade fält är tillgänglig som en del av-synkroniseringen av Partner Center-referenser för Salesforce CRM-lösning för **affärs möjlighet** .</span><span class="sxs-lookup"><span data-stu-id="32413-267">A set of custom fields is available as part of Partner Center Referrals Synchronization for Salesforce CRM solution **Opportunity** entity.</span></span> <span data-ttu-id="32413-268">En administratörs användare i CRM måste skapa ett separat CRM-avsnitt med anpassade **affärs möjlighets** fält.</span><span class="sxs-lookup"><span data-stu-id="32413-268">A CRM admin user will need to create a separate CRM section with the **Opportunity** custom fields.</span></span>

<span data-ttu-id="32413-269">Följande anpassade fält ska ingå i CRM-avsnittet:</span><span class="sxs-lookup"><span data-stu-id="32413-269">The following custom fields should be part of the CRM section:</span></span>

- <span data-ttu-id="32413-270">**Synkronisera med partner Center**: om du vill synkronisera affärs möjligheten med Microsoft Partner Center</span><span class="sxs-lookup"><span data-stu-id="32413-270">**Sync with Partner Center**: Whether to sync the opportunity with Microsoft Partner Center</span></span>

- <span data-ttu-id="32413-271">**Hänvisnings-ID**: ett skrivskyddat ID-fält för Microsoft Partner Center-hänvisning</span><span class="sxs-lookup"><span data-stu-id="32413-271">**Referral Identifier**: A read-only identifier field for Microsoft Partner Center referral</span></span>

- <span data-ttu-id="32413-272">**Hänvisnings länk**: en skrivskyddad länk till hänvisningen i Microsoft Partner Center</span><span class="sxs-lookup"><span data-stu-id="32413-272">**Referral Link**: A read-only link to the referral in Microsoft Partner Center</span></span>

- <span data-ttu-id="32413-273">**Hur kan Microsoft hjälpa**: hjälp som krävs från Microsoft för hänvisning</span><span class="sxs-lookup"><span data-stu-id="32413-273">**How can Microsoft help**: Help required from Microsoft for the referral</span></span>

- <span data-ttu-id="32413-274">**Produkter**: lista över produkter som är kopplade till den här affärs möjligheten</span><span class="sxs-lookup"><span data-stu-id="32413-274">**Products**: List of products associated with this opportunity</span></span>

- <span data-ttu-id="32413-275">**Granskning**: en skrivskyddad Gransknings logg för synkronisering med partner Center-hänvisningar</span><span class="sxs-lookup"><span data-stu-id="32413-275">**Audit**: A read-only audit trail for syncing with Partner Center referrals</span></span>

### <a name="scenarios"></a><span data-ttu-id="32413-276">OLIKA</span><span class="sxs-lookup"><span data-stu-id="32413-276">SCENARIOS:</span></span>

1. <span data-ttu-id="32413-277">Hänvisnings-synkronisering när hänvisning skapas eller uppdateras i CRM och synkroniseras i Partner Center:</span><span class="sxs-lookup"><span data-stu-id="32413-277">Referral synchronization when referral is created or updated in CRM and synced in Partner Center:</span></span>

   1. <span data-ttu-id="32413-278">Logga in på din Salesforce CRM-miljö med användare som har synlighet i avsnittet **affärs möjlighet** i CRM.</span><span class="sxs-lookup"><span data-stu-id="32413-278">Sign into your Salesforce CRM environment with user who has visibility in the **Opportunity** section of the CRM.</span></span>

   2. <span data-ttu-id="32413-279">Se till att följande avsnitt finns när du skapar en "ny affärs möjlighet" i Salesforce CRM-miljön</span><span class="sxs-lookup"><span data-stu-id="32413-279">Ensure that the following section is present when you create a "New Opportunity" in Salesforce CRM environment</span></span>

      :::image type="content" source="images/salesforce/salesforce-scenario-1.png" alt-text="Salesforce-miljö":::

   3. <span data-ttu-id="32413-281">För att synkronisera den här affärs möjligheten med Microsoft Partner Center, se till att du anger följande fält i kort vyn:</span><span class="sxs-lookup"><span data-stu-id="32413-281">To synchronize this opportunity with Microsoft Partner Center, ensure that you set the following fields in the card view:</span></span>

       - <span data-ttu-id="32413-282">"Synkronisera med partner Center": Ja</span><span class="sxs-lookup"><span data-stu-id="32413-282">"Sync with Partner Center": Yes</span></span>
       - <span data-ttu-id="32413-283">"Hur kan Microsoft Hjälp?": Välj bland följande alternativ:</span><span class="sxs-lookup"><span data-stu-id="32413-283">"How can Microsoft help?": Select from the following options:</span></span>
       - <span data-ttu-id="32413-284">Produkter: lösnings-ID för produkten</span><span class="sxs-lookup"><span data-stu-id="32413-284">Products: Solution IDs of the product</span></span>

   4. <span data-ttu-id="32413-285">När du har ställt in alternativet för synkronisering av affärs möjligheter med **alternativet för att** **Synkronisera med partner Center** väntar du 10 minuter och loggar in på ditt partner Center-konto.</span><span class="sxs-lookup"><span data-stu-id="32413-285">Once you have set the opportunity  **Sync with Partner Center** option to **Yes**, wait 10 minutes, sign into your Partner Center account.</span></span> <span data-ttu-id="32413-286">Dina referenser kommer att synkroniseras med Salesforce CRM.</span><span class="sxs-lookup"><span data-stu-id="32413-286">Your referrals will be synchronized with Salesforce CRM.</span></span>

   5. <span data-ttu-id="32413-287">När alternativet "synkronisera med partner Center" är inställt på "Ja", kommer ändringarna att synkroniseras med ditt partner Center-konto om du uppdaterar affärs möjligheten i Salesforce CRM.</span><span class="sxs-lookup"><span data-stu-id="32413-287">When the "Sync with Partner Center" option is set to "Yes", if you update the opportunity in Salesforce CRM, the changes will synchronize with your Partner Center account.</span></span>

   6. <span data-ttu-id="32413-288">Affärs möjligheter som har synkroniserats med partner Center identifieras med ✔-ikonen i Salesforce CRM.</span><span class="sxs-lookup"><span data-stu-id="32413-288">Opportunities that are synchronized successfully with Partner Center will be identified with ✔icon in Salesforce CRM.</span></span>

2. <span data-ttu-id="32413-289">Hänvisnings-synkronisering när hänvisning skapas eller uppdateras i Microsoft Partner Center och synkroniseras i Salesforce CRM-miljö:</span><span class="sxs-lookup"><span data-stu-id="32413-289">Referral Synchronization when referral is created or updated in Microsoft Partner Center and synchronized in Salesforce CRM environment:</span></span>

    1. <span data-ttu-id="32413-290">Logga in på [instrument panelen](https://partner.microsoft.com/dashboard/home)för partner Center.</span><span class="sxs-lookup"><span data-stu-id="32413-290">Sign into your Partner Center [dashboard](https://partner.microsoft.com/dashboard/home).</span></span>

    2. <span data-ttu-id="32413-291">Välj **referenser** på menyn till vänster.</span><span class="sxs-lookup"><span data-stu-id="32413-291">Select **Referrals** from the left-hand menu.</span></span>

    3. <span data-ttu-id="32413-292">Skapa en ny samförsäljnings hänvisning från Partner Center genom att klicka på alternativet "nytt erbjudande".</span><span class="sxs-lookup"><span data-stu-id="32413-292">Create a new Co-sell referral from Partner Center by clicking "New deal" option.</span></span>

    4. <span data-ttu-id="32413-293">Logga in på din Salesforce CRM-miljö.</span><span class="sxs-lookup"><span data-stu-id="32413-293">Sign into your Salesforce CRM environment.</span></span>

    5. <span data-ttu-id="32413-294">Navigera till **Öppna affärs möjligheter**.</span><span class="sxs-lookup"><span data-stu-id="32413-294">Navigate to **Open Opportunities**.</span></span> <span data-ttu-id="32413-295">Den hänvisning som skapats i Microsoft Partner Center synkroniseras nu i Salesforce CRM.</span><span class="sxs-lookup"><span data-stu-id="32413-295">The referral created in Microsoft Partner Center is now synchronized in Salesforce CRM.</span></span>

       :::image type="content" source="images/salesforce/salesforce-casino-e.png" alt-text="Skärmen för Salesforce-möjligheter":::

    6. <span data-ttu-id="32413-297">När du väljer en synkroniserad referens fylls kort visnings informationen i.</span><span class="sxs-lookup"><span data-stu-id="32413-297">When you select a synchronized referral, the card view details are populated.</span></span>

## <a name="next-steps"></a><span data-ttu-id="32413-298">Nästa steg</span><span class="sxs-lookup"><span data-stu-id="32413-298">Next steps</span></span>

- [<span data-ttu-id="32413-299">Hantera leads</span><span class="sxs-lookup"><span data-stu-id="32413-299">Manage leads</span></span>](manage-leads.md)

- [<span data-ttu-id="32413-300">Hantera möjligheter till samförsäljning</span><span class="sxs-lookup"><span data-stu-id="32413-300">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)

- [<span data-ttu-id="32413-301">Webhooks för partner Center</span><span class="sxs-lookup"><span data-stu-id="32413-301">Partner Center webhooks</span></span>](/partner-center/develop/partner-center-webhooks)
