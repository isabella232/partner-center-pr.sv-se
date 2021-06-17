---
title: Anslutningsappen för säljförsäljning för Salesforce CRM Partner Center
ms.topic: how-to
ms.date: 01/06/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Synkronisera dina hänvisningar i PartnerCenter med salesforce CRM. Säljare kan sedan samförsäljninga med Microsoft inifrån dina CRM-system.
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: 74894671966ac0409f6366f33c91ddadfae1ba4c
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/17/2021
ms.locfileid: "112276985"
---
# <a name="co-sell-connector-for-salesforce-crm---overview"></a><span data-ttu-id="40649-104">Anslutningsapp för säljförsäljning för Salesforce CRM – översikt</span><span class="sxs-lookup"><span data-stu-id="40649-104">Co-sell connector for Salesforce CRM - overview</span></span>

<span data-ttu-id="40649-105">**Lämpliga roller:** Referensadministratörsroller | Systemadministratör eller systemanpassare för CRM</span><span class="sxs-lookup"><span data-stu-id="40649-105">**Appropriate roles**: Referrals admin | System admin or system customizer on the CRM</span></span>

<span data-ttu-id="40649-106">PartnerCenter-anslutning för säljpartner gör det möjligt för dina säljare att samförsäljninga med Microsoft inifrån dina CRM-system.</span><span class="sxs-lookup"><span data-stu-id="40649-106">Partner Center co-sell connector enables your sellers to co-sell with Microsoft from within your CRM systems.</span></span> <span data-ttu-id="40649-107">De behöver inte tränas för att använda Partner Center för att hantera säljavtal.</span><span class="sxs-lookup"><span data-stu-id="40649-107">They won’t have to be trained to use Partner Center to manage Co-sell deals.</span></span> <span data-ttu-id="40649-108">Med hjälp av anslutningsapparna för säljförsäljning kan du skapa en ny hänvisning för säljförsäljning för att engagera en Microsoft-säljare, få hänvisningar från Microsoft-säljaren, acceptera/avvisa hänvisningar, ändra avtalsdata som avtalsvärde och slutdatum.</span><span class="sxs-lookup"><span data-stu-id="40649-108">Using the Co-sell connectors, you can create a new Co-sell referral to engage a Microsoft seller, receive referrals from the Microsoft seller, accept/decline referrals, modify deal data such as deal value, and closing date.</span></span>  <span data-ttu-id="40649-109">Du kan också få uppdateringar från Microsofts säljare om dessa samförsäljningserbjudanden.</span><span class="sxs-lookup"><span data-stu-id="40649-109">You can also receive any updates from the Microsoft sellers on these Co-sell deals.</span></span> <span data-ttu-id="40649-110">Du kan göra så att alla dina hänvisningar fungerar när du arbetar med den CRM du väljer i stället för i Partnercenter.</span><span class="sxs-lookup"><span data-stu-id="40649-110">You can do all of your referrals work while working within the CRM of your choice rather than in Partner Center.</span></span> 

<span data-ttu-id="40649-111">Lösningen är baserad på Microsoft Power Automate Solution och använder Partner Center-API:er.</span><span class="sxs-lookup"><span data-stu-id="40649-111">The solution is based on Microsoft Power Automate Solution and uses Partner Center APIs.</span></span>

## <a name="before-you-install---pre-requisites"></a><span data-ttu-id="40649-112">Innan du installerar – förutsättningar</span><span class="sxs-lookup"><span data-stu-id="40649-112">Before you install - pre-requisites</span></span>

|<span data-ttu-id="40649-113">**Ämnen**</span><span class="sxs-lookup"><span data-stu-id="40649-113">**Topics**</span></span>   |<span data-ttu-id="40649-114">**Information**</span><span class="sxs-lookup"><span data-stu-id="40649-114">**Details**</span></span>   |<span data-ttu-id="40649-115">**Länkar**</span><span class="sxs-lookup"><span data-stu-id="40649-115">**Links**</span></span>   |
|--------------|--------------------|------|
|<span data-ttu-id="40649-116">Microsoft Partner Network-ID</span><span class="sxs-lookup"><span data-stu-id="40649-116">Microsoft Partner Network ID</span></span> |<span data-ttu-id="40649-117">Du behöver ett giltigt MPN-ID</span><span class="sxs-lookup"><span data-stu-id="40649-117">You need a valid MPN ID</span></span>|<span data-ttu-id="40649-118">Så här ansluter du [till MPN](https://partner.microsoft.com/)</span><span class="sxs-lookup"><span data-stu-id="40649-118">To join [MPN](https://partner.microsoft.com/)</span></span>|
|<span data-ttu-id="40649-119">Redo för säljförsäljning</span><span class="sxs-lookup"><span data-stu-id="40649-119">Co-sell ready</span></span>|<span data-ttu-id="40649-120">Din IP-/tjänstlösning måste vara redo för säljförsäljning.</span><span class="sxs-lookup"><span data-stu-id="40649-120">Your IP/Services solution must be co-sell ready.</span></span>|[<span data-ttu-id="40649-121">Sälja med Microsoft</span><span class="sxs-lookup"><span data-stu-id="40649-121">Sell with Microsoft</span></span>](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|<span data-ttu-id="40649-122">Partnercenter-konto</span><span class="sxs-lookup"><span data-stu-id="40649-122">Partner Center account</span></span>|<span data-ttu-id="40649-123">MPN-ID:t som är associerat med Partnercenter-klienten måste vara samma som det MPN-ID som är associerat med din säljpartnerlösning.</span><span class="sxs-lookup"><span data-stu-id="40649-123">The MPN ID associated with the Partner Center tenant must be same as the MPN ID associated with your Co-sell solution.</span></span> <span data-ttu-id="40649-124">Kontrollera att du kan se dina hänvisningar till säljförsäljning i Partner Center-portalen innan du distribuerar anslutningsapparna.</span><span class="sxs-lookup"><span data-stu-id="40649-124">Verify that you can see your co-sell referrals in Partner Center portal before deploying the connectors.</span></span>|[<span data-ttu-id="40649-125">Hantera ditt konto</span><span class="sxs-lookup"><span data-stu-id="40649-125">Manage your account</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="40649-126">Användarroller i Partnercenter</span><span class="sxs-lookup"><span data-stu-id="40649-126">Partner Center user roles</span></span>|<span data-ttu-id="40649-127">Medarbetaren som ska installera och använda anslutningsapparna måste vara referensadministratör</span><span class="sxs-lookup"><span data-stu-id="40649-127">The employee who will install and use the connectors must be a Referrals admin</span></span>|[<span data-ttu-id="40649-128">Tilldela användarroller och -behörigheter</span><span class="sxs-lookup"><span data-stu-id="40649-128">Assign users roles and permissions</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="40649-129">Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="40649-129">Salesforce CRM</span></span>|<span data-ttu-id="40649-130">CRM-användarrollen är Systemadministratör eller Systemanpassare</span><span class="sxs-lookup"><span data-stu-id="40649-130">The CRM user role is System admin or System customizer</span></span>|[<span data-ttu-id="40649-131">Tilldela roller i Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="40649-131">Assign roles in Salesforce CRM</span></span>](https://help.salesforce.com/articleView?id=assigning_users_to_roles.htm&type=5)|
|<span data-ttu-id="40649-132">Power Automate Flow-konto</span><span class="sxs-lookup"><span data-stu-id="40649-132">Power Automate Flow Account</span></span>|<span data-ttu-id="40649-133">Ett aktivt [Power Automate](https://flow.microsoft.com) konto för CRM-systemadministratören eller systemanpassaren.</span><span class="sxs-lookup"><span data-stu-id="40649-133">An active [Power Automate](https://flow.microsoft.com) account for the CRM System admin or System customizer.</span></span> <span data-ttu-id="40649-134">Användaren bör logga in på [Power Automate](https://flow.microsoft.com) minst en gång före installationen.</span><span class="sxs-lookup"><span data-stu-id="40649-134">That user should sign into [Power Automate](https://flow.microsoft.com) at least once before installation.</span></span>|

## <a name="installation-of-salesforce-package-for-microsoft-custom-fields"></a><span data-ttu-id="40649-135">Installation av Salesforce-paket för Microsoft Custom Fields</span><span class="sxs-lookup"><span data-stu-id="40649-135">Installation of Salesforce Package for Microsoft Custom Fields</span></span> 

<span data-ttu-id="40649-136">Om du vill synkronisera hänvisningarna i Partner Center och Salesforce CRM Power Automate lösningen tydligt identifiera Microsoft-specifika hänvisningsfält.</span><span class="sxs-lookup"><span data-stu-id="40649-136">To synchronize the referrals across Partner Center and Salesforce CRM, the Power Automate solution needs to clearly identify Microsoft-specific referral fields.</span></span> <span data-ttu-id="40649-137">Den här avgränsningen ger partnerförsäljningsteam möjlighet att bestämma vilka hänvisningar de vill dela med Microsoft för säljpartner.</span><span class="sxs-lookup"><span data-stu-id="40649-137">This demarcation provides partner seller teams with the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

1. <span data-ttu-id="40649-138">I Salesforce aktiverar du **Anteckningar och** lägger till den i listan med affärsmöjligheter.</span><span class="sxs-lookup"><span data-stu-id="40649-138">In Salesforce, activate **Notes** and add it to the opportunities related list.</span></span> 
[<span data-ttu-id="40649-139">Referens</span><span class="sxs-lookup"><span data-stu-id="40649-139">Reference</span></span>](https://help.salesforce.com/articleView?err=1&id=notes_admin_setup.htm&type=5)

2. <span data-ttu-id="40649-140">Aktivera **affärsmöjlighetsteam** genom att följa stegen:</span><span class="sxs-lookup"><span data-stu-id="40649-140">Activate **Opportunity teams** by following the steps:</span></span> 
    - <span data-ttu-id="40649-141">I installationsprogrammet använder du rutan **Snabb hitta** för att hitta gruppinställningar för a tillfället.</span><span class="sxs-lookup"><span data-stu-id="40649-141">In Setup, use the **Quick Find** box to locate Opportunity Team Settings.</span></span>
    - <span data-ttu-id="40649-142">Definiera inställningarna efter behov.</span><span class="sxs-lookup"><span data-stu-id="40649-142">Define the settings as needed.</span></span>
[<span data-ttu-id="40649-143">Referens</span><span class="sxs-lookup"><span data-stu-id="40649-143">Reference</span></span>](https://help.salesforce.com/articleView?id=teamselling_enabling.htm&type=5]) 

3. <span data-ttu-id="40649-144">Installera anpassade fält och objekt i Salesforce med hjälp av [installationsprogrammet för paketet](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t2w000006WIwV).</span><span class="sxs-lookup"><span data-stu-id="40649-144">In Salesforce, install custom fields and objects using the [package installer](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t2w000006WIwV).</span></span> <span data-ttu-id="40649-145">Använd det här om du vill installera paketet på ett företag.</span><span class="sxs-lookup"><span data-stu-id="40649-145">Use this to install the package into any company.</span></span>

>[!NOTE]
><span data-ttu-id="40649-146">Om du installerar i en sandbox-miljö måste du ersätta den första delen av URL:en med http://test.salesforce.com</span><span class="sxs-lookup"><span data-stu-id="40649-146">If you are installing into a sandbox, you must replace the initial portion of the URL with http://test.salesforce.com</span></span>

4. <span data-ttu-id="40649-147">I Salesforce lägger du till Microsoft-lösningar i **listan Affärsmöjlighetsrelaterade.**</span><span class="sxs-lookup"><span data-stu-id="40649-147">In Salesforce, add Microsoft Solutions to the **Opportunity** related list.</span></span> <span data-ttu-id="40649-148">När du har lagt till väljer **du ikonen** för färgning och uppdaterar egenskaper</span><span class="sxs-lookup"><span data-stu-id="40649-148">Once added, select the **wrench** icon and update properties</span></span>

## <a name="best-practice-test-before-you-go-live"></a><span data-ttu-id="40649-149">Bästa praxis: Testa innan du går live</span><span class="sxs-lookup"><span data-stu-id="40649-149">Best Practice: Test before you go live</span></span>

<span data-ttu-id="40649-150">Innan du installerar, konfigurerar och anpassar Power Automate-lösningen i produktionsmiljön måste du testa lösningen på en CRM-mellanlagringsinstans.</span><span class="sxs-lookup"><span data-stu-id="40649-150">Before you install, configure, and customize the Power Automate solution on the production environment, be sure to test the solution on a staging CRM instance.</span></span>

- <span data-ttu-id="40649-151">Installera Microsoft Power Automate lösning på en mellanlagringsmiljö/CRM-instans.</span><span class="sxs-lookup"><span data-stu-id="40649-151">Install Microsoft Power Automate solution on a staging environment/CRM instance.</span></span>

- <span data-ttu-id="40649-152">Skapa en kopia av lösningen och kör konfigurationen och Power Automate av flödesanpassningar i mellanlagringsmiljön.</span><span class="sxs-lookup"><span data-stu-id="40649-152">Make a copy of the solution and run your configuration and Power Automate flow customizations on the staging environment.</span></span>

- <span data-ttu-id="40649-153">Testa lösningen på en mellanlagrings-/CRM-instans.</span><span class="sxs-lookup"><span data-stu-id="40649-153">Test the solution on a staging/CRM instance.</span></span>

- <span data-ttu-id="40649-154">Vid lyckad import som en hanterad lösning till produktionsinstansen.</span><span class="sxs-lookup"><span data-stu-id="40649-154">On success, import as a managed solution to the production instance.</span></span>

## <a name="install-partner-center-referrals-synchronization-for-salesforce-crm"></a><span data-ttu-id="40649-155">Installera synkronisering av partnercenterreferenser för Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="40649-155">Install Partner Center Referrals Synchronization for Salesforce CRM</span></span>

1. <span data-ttu-id="40649-156">Gå till [Power Automate](https://flow.microsoft.com) och **välj Miljöer** i det övre högra hörnet.</span><span class="sxs-lookup"><span data-stu-id="40649-156">Go to [Power Automate](https://flow.microsoft.com) and select **Environments** on the right top corner.</span></span> <span data-ttu-id="40649-157">Då visas de tillgängliga CRM-instanserna.</span><span class="sxs-lookup"><span data-stu-id="40649-157">This will show you the available CRM instances.</span></span>

2. <span data-ttu-id="40649-158">Välj lämplig CRM-instans i listrutan i det högra övre hörnet.</span><span class="sxs-lookup"><span data-stu-id="40649-158">Select the appropriate CRM instance from the drop-down on the right top corner.</span></span>

3. <span data-ttu-id="40649-159">Välj **Lösningar** i det vänstra navigeringsfältet.</span><span class="sxs-lookup"><span data-stu-id="40649-159">Select **Solutions** on the left navigation bar.</span></span>

4. <span data-ttu-id="40649-160">Välj länken **Öppna AppSource** på den översta menyn.</span><span class="sxs-lookup"><span data-stu-id="40649-160">Select the **Open AppSource** link on the top menu.</span></span>

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="Öppna AppSource.":::

5. <span data-ttu-id="40649-162">Sök efter **partnercenterreferenser för Salesforce** på popup-skärmen.</span><span class="sxs-lookup"><span data-stu-id="40649-162">Search for **Partner Center Referrals Connectors for Salesforce** in the pop-up screen.</span></span>  

   :::image type="content" source="images/salesforce/salesforce1.png" alt-text="Salesforce.":::

6. <span data-ttu-id="40649-164">Välj knappen **Hämta nu** och sedan **Fortsätt.**</span><span class="sxs-lookup"><span data-stu-id="40649-164">Select the **Get it now** button and then **Continue**.</span></span>

7. <span data-ttu-id="40649-165">Då öppnas sidan där du kan välja Salesforce CRM-miljön för att installera programmet.</span><span class="sxs-lookup"><span data-stu-id="40649-165">This opens the page where you can select the Salesforce CRM  environment to install application.</span></span>  <span data-ttu-id="40649-166">Godkänn villkoren.</span><span class="sxs-lookup"><span data-stu-id="40649-166">Agree to terms and conditions.</span></span>

   :::image type="content" source="images/salesforce/available-crm.png" alt-text="Tillgängliga CRMS.":::

8. <span data-ttu-id="40649-168">Du dirigeras sedan till sidan **Hantera dina** lösningar.</span><span class="sxs-lookup"><span data-stu-id="40649-168">You're then directed to the **Manage your solutions** page.</span></span>  <span data-ttu-id="40649-169">Gå till "Partner Center-referenser" med hjälp av pilknapparna längst ned på sidan.</span><span class="sxs-lookup"><span data-stu-id="40649-169">Navigate to "Partner Center Referrals" by using the arrow buttons on the bottom of the page.</span></span> <span data-ttu-id="40649-170">**Schemalagd installation** bör visas bredvid referenslösningen i Partnercenter.</span><span class="sxs-lookup"><span data-stu-id="40649-170">**Installation scheduled** should appear next to Partner Center Referrals solution.</span></span> <span data-ttu-id="40649-171">Installationen tar 10–15 minuter.</span><span class="sxs-lookup"><span data-stu-id="40649-171">Installation will take 10-15 minutes.</span></span>

9. <span data-ttu-id="40649-172">När installationen är klar går du tillbaka till [Power Automate](https://flow.microsoft.com) väljer **Lösningar i** det vänstra navigeringsområdet.</span><span class="sxs-lookup"><span data-stu-id="40649-172">Once the installation is complete, navigate back to [Power Automate](https://flow.microsoft.com) and select **Solutions** from left navigation area.</span></span> <span data-ttu-id="40649-173">Observera att **synkronisering av Referenser för Partnercenter för Salesforce** finns i listan Lösningar.</span><span class="sxs-lookup"><span data-stu-id="40649-173">Notice that **Partner Center Referrals Synchronization for Salesforce** is available in the Solutions list.</span></span>

10. <span data-ttu-id="40649-174">Välj **Synkronisering av partnercenterreferenser för Salesforce.**</span><span class="sxs-lookup"><span data-stu-id="40649-174">Select **Partner Center Referrals Synchronization for Salesforce**.</span></span> <span data-ttu-id="40649-175">Följande flöden Power Automate och entiteter är tillgängliga:</span><span class="sxs-lookup"><span data-stu-id="40649-175">The following Power Automate flows and entities are available:</span></span>

    :::image type="content" source="images/cosellconnectors/salesforce10.png" alt-text="Salesforce-flöden.":::



## <a name="configure-the-solution"></a><span data-ttu-id="40649-177">Konfigurera lösningen</span><span class="sxs-lookup"><span data-stu-id="40649-177">Configure the solution</span></span>

1. <span data-ttu-id="40649-178">När du har installerat lösningen i din CRM-instans går du tillbaka till [Power Automate](https://flow.microsoft.com/).</span><span class="sxs-lookup"><span data-stu-id="40649-178">Once you have installed the solution in your CRM instance, navigate back to [Power Automate](https://flow.microsoft.com/).</span></span>

2. <span data-ttu-id="40649-179">I **listrutan Miljöer** i det övre högra hörnet väljer du den CRM-instans där du installerade Power Automate lösningen.</span><span class="sxs-lookup"><span data-stu-id="40649-179">From the **Environments** drop-down on the right top corner, select the CRM instance where you installed the Power Automate solution.</span></span>
3. <span data-ttu-id="40649-180">Du måste skapa anslutningar som associerar de tre användarkontona:</span><span class="sxs-lookup"><span data-stu-id="40649-180">You will need to create connections that associate the three user accounts:</span></span>
    - <span data-ttu-id="40649-181">PartnerCenter-användare med referenser för administratörsautentiseringsuppgifter</span><span class="sxs-lookup"><span data-stu-id="40649-181">Partner Center user with referrals admin credentials</span></span>
    - <span data-ttu-id="40649-182">Partnercenter-händelser</span><span class="sxs-lookup"><span data-stu-id="40649-182">Partner Center Events</span></span>
    - <span data-ttu-id="40649-183">CRM-administratör med Power Automate flöden i lösningen.</span><span class="sxs-lookup"><span data-stu-id="40649-183">CRM admin with the Power Automate flows in the solution.</span></span>
4. <span data-ttu-id="40649-184">Välj **Anslutningar** i det vänstra navigeringsfältet och välj lösningen "PartnerCenter-referenser" i listan.</span><span class="sxs-lookup"><span data-stu-id="40649-184">Select **Connections** from the left navigation bar and select the "Partner Center Referrals" solution from the list.</span></span>

5. <span data-ttu-id="40649-185">Skapa en anslutning genom att klicka **på Skapa en anslutning.**</span><span class="sxs-lookup"><span data-stu-id="40649-185">Create a connection by clicking **Create a connection**.</span></span>

:::image type="content" source="images/cosellconnectors/salesforce12.png" alt-text="Skapa anslutning.":::

- <span data-ttu-id="40649-187">Sök efter Referenser till Partnercenter (förhandsversion) i sökfältet i det övre högra hörnet.</span><span class="sxs-lookup"><span data-stu-id="40649-187">Search for Partner Center Referrals (preview) in the search bar on the top-right corner.</span></span>

- <span data-ttu-id="40649-188">Skapa en anslutning för din Partnercenter-användare med rollen Referensadministratör.</span><span class="sxs-lookup"><span data-stu-id="40649-188">Create a connection for your Partner Center user with the credentials role of Referrals admin.</span></span>

-  <span data-ttu-id="40649-189">Skapa sedan en partnercenterhändelser-anslutning för din Partnercenter-användare med autentiseringsuppgifterna för referensadministratören.</span><span class="sxs-lookup"><span data-stu-id="40649-189">Next, create a Partner Center Events connection for your Partner Center user with the credentials of Referrals admin.</span></span>

- <span data-ttu-id="40649-190">Skapa en anslutning för Salesforce för CRM-administratörsanvändaren.</span><span class="sxs-lookup"><span data-stu-id="40649-190">Create a connection for Salesforce for the CRM administrator user.</span></span>

-  <span data-ttu-id="40649-191">När du har lagt till alla anslutningar bör du se följande anslutningar i din miljö:</span><span class="sxs-lookup"><span data-stu-id="40649-191">Once you have all the Connections added, you should see the following Connections in your environment:</span></span>

 :::image type="content" source="images/cosellconnectors/salesforce13.png" alt-text="Observera anslutningar.":::

### <a name="edit-the-connections"></a><span data-ttu-id="40649-193">Redigera anslutningarna</span><span class="sxs-lookup"><span data-stu-id="40649-193">Edit the connections</span></span>

1. <span data-ttu-id="40649-194">Gå tillbaka till sidan Lösningar och välj **Standardlösning.**</span><span class="sxs-lookup"><span data-stu-id="40649-194">Return to the Solutions page and select **Default Solution**.</span></span>  <span data-ttu-id="40649-195">Välj **Anslutningsreferens (förhandsversion) genom att** klicka på **Alla.**</span><span class="sxs-lookup"><span data-stu-id="40649-195">Select **Connection Reference (preview)** by clicking **All**.</span></span>
 
:::image type="content" source="images/cosellconnectors/salesforce14.png" alt-text="Börja redigera anslutningsappen.":::

2. <span data-ttu-id="40649-197">Redigera var och en av anslutningarna individuellt genom att välja ikonen med tre punkter.</span><span class="sxs-lookup"><span data-stu-id="40649-197">Edit each of the Connections individually by selecting the three dots icon.</span></span> <span data-ttu-id="40649-198">Lägg till relevanta anslutningar.</span><span class="sxs-lookup"><span data-stu-id="40649-198">Add the relevant connections.</span></span>

:::image type="content" source="images/cosellconnectors/salesforce15.png" alt-text="Redigera anslutningsappar.":::

3. <span data-ttu-id="40649-200">Aktivera flöden i följande ordning:</span><span class="sxs-lookup"><span data-stu-id="40649-200">Turn on the flows in the following sequence:</span></span>

- <span data-ttu-id="40649-201">Partner Center Webhook Registration (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="40649-201">Partner Center Webhook Registration (Insider Preview)</span></span>
- <span data-ttu-id="40649-202">Skapa hänvisning till säljpartner – Salesforce till Partner Center (insiderförhandsvisning)</span><span class="sxs-lookup"><span data-stu-id="40649-202">Create Co-sell Referral - Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="40649-203">Partner center Microsoft co-sell hänvisningsuppdateringar till Salesforce (insiderförhandsvisning)</span><span class="sxs-lookup"><span data-stu-id="40649-203">Partner Center Microsoft Co-sell Referral Updates to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="40649-204">Partner center till Salesforce (insiderförhandsvisning)</span><span class="sxs-lookup"><span data-stu-id="40649-204">Partner Center to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="40649-205">Salesforce till Partner Center (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="40649-205">Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="40649-206">Salesforce Opportunity to Partner Center (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="40649-206">Salesforce Opportunity to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="40649-207">Salesforce Microsoft Solutions to Partner Center (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="40649-207">Salesforce Microsoft Solutions to Partner Center (Insider Preview)</span></span>

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a><span data-ttu-id="40649-208">Använda Webhook-API:er för att registrera för resursändringshändelser</span><span class="sxs-lookup"><span data-stu-id="40649-208">Use Webhook APIs to register for resource change events</span></span>

<span data-ttu-id="40649-209">Med Partnercenter Webhook-API:er kan du registrera dig för resursändringshändelser.</span><span class="sxs-lookup"><span data-stu-id="40649-209">The Partner Center Webhook APIs allow you to register for resource change events.</span></span> <span data-ttu-id="40649-210">Dessa ändringshändelser skickas till din URL som HTTP-inlägg.</span><span class="sxs-lookup"><span data-stu-id="40649-210">These change events are sent to your url as HTTP posts.</span></span>

1. <span data-ttu-id="40649-211">Om du vill registrera din URL väljer **du Partner Center Webhook Registration (Insider Preview)** Power Automate flöde.</span><span class="sxs-lookup"><span data-stu-id="40649-211">To register your url, select **Partner Center Webhook Registration (Insider Preview)** Power Automate flow.</span></span>

2. <span data-ttu-id="40649-212">Lägg till anslutningar för (a.) Partner Center-användare med referenser administratörsautentiseringsuppgifter (b.) Partner Center-händelser enligt nedan</span><span class="sxs-lookup"><span data-stu-id="40649-212">Add connections for (a.) Partner Center user with referrals admin credentials (b.) Partner Center Events as highlighted below</span></span>

   :::image type="content" source="images/cosellconnectors/triggerflow.png" alt-text="Utlösa.":::

3. <span data-ttu-id="40649-214">När du gör dessa uppdateringar visas</span><span class="sxs-lookup"><span data-stu-id="40649-214">When you make these updates, you'll see</span></span>

   :::image type="content" source="images/cosellconnectors/webhook1.png" alt-text="Webhooks.":::

4. <span data-ttu-id="40649-216">Spara ändringarna och välj **Aktivera**.</span><span class="sxs-lookup"><span data-stu-id="40649-216">Save your changes and select **Turn on**.</span></span>

   <span data-ttu-id="40649-217">Utför följande steg för att aktivera Partnercenter-webhooks för att lyssna på händelseändringar:</span><span class="sxs-lookup"><span data-stu-id="40649-217">To enable Partner Center webhooks to listen to event changes, perform the following steps:</span></span>

5. <span data-ttu-id="40649-218">Välj **Partner Center till Salesforce CRM (Insider Preview).**</span><span class="sxs-lookup"><span data-stu-id="40649-218">Select **Partner Center to Salesforce CRM (Insider Preview)**.</span></span>

6. <span data-ttu-id="40649-219">Välj ikonen **Redigera** och välj När **en HTTP-begäran tas emot.**</span><span class="sxs-lookup"><span data-stu-id="40649-219">Select the **Edit** icon and select **When a HTTP request is received**.</span></span>

7. <span data-ttu-id="40649-220">Välj ikonen **Kopiera för** att kopiera den angivna HTTP POST-URL:en.</span><span class="sxs-lookup"><span data-stu-id="40649-220">Select the **Copy** icon to copy the provided HTTP POST URL.</span></span>

   :::image type="content" source="images/salesforce/copy-url.png" alt-text="Kopiera URL:en.":::

8. <span data-ttu-id="40649-222">Välj nu flödet "Partner Center Webhook Registration (Insider Preview)" och Power Automate **kör**.</span><span class="sxs-lookup"><span data-stu-id="40649-222">Now select the "Partner Center Webhook Registration (Insider Preview)" Power Automate flow and select **Run**.</span></span>

9. <span data-ttu-id="40649-223">Kontrollera att fönstret "Kör flöde" öppnas i den högra rutan och välj **Fortsätt.**</span><span class="sxs-lookup"><span data-stu-id="40649-223">Ensure that the "Run Flow" window opens on the right-hand pane and select **Continue**.</span></span>

10. <span data-ttu-id="40649-224">Ange följande information:</span><span class="sxs-lookup"><span data-stu-id="40649-224">Enter the following details:</span></span>

    1. <span data-ttu-id="40649-225">**Http-utlösarslutpunkt:** URL som kopierades från ett tidigare steg</span><span class="sxs-lookup"><span data-stu-id="40649-225">**Http Trigger Endpoint**: URL copied from earlier step</span></span>

    2. <span data-ttu-id="40649-226">**Händelser att registrera:**"referral-created" och "referral-updated"</span><span class="sxs-lookup"><span data-stu-id="40649-226">**Events to Register**: "referral-created" and "referral-updated"</span></span>

    3. <span data-ttu-id="40649-227">**Skriva över befintliga utlösarslutpunkter om de finns**: Ja (detta skriver över befintliga slutpunkter.)</span><span class="sxs-lookup"><span data-stu-id="40649-227">**Overwrite existing trigger endpoints if present**: Yes (This overwrites any existing endpoints.)</span></span>

11. <span data-ttu-id="40649-228">Välj **Kör** och sedan **Klar.**</span><span class="sxs-lookup"><span data-stu-id="40649-228">Select **Run** and then select **Done.**</span></span>

<span data-ttu-id="40649-229">Webhooken kan nu lyssna efter händelser som skapas och uppdateras.</span><span class="sxs-lookup"><span data-stu-id="40649-229">The webhook can now listen to create and update events.</span></span>

## <a name="customize-synchronization-steps"></a><span data-ttu-id="40649-230">Anpassa synkroniseringssteg</span><span class="sxs-lookup"><span data-stu-id="40649-230">Customize synchronization steps</span></span>

<span data-ttu-id="40649-231">När hänvisningar till säljförsäljning synkroniseras mellan Partner Center och ditt CRM-system visas fälten som synkroniseras på Partner Center-datorn här.</span><span class="sxs-lookup"><span data-stu-id="40649-231">When Co-sell referrals are synced between Partner Center and your CRM system, the fields that are synced on Partner Center PC are listed here.</span></span>

<span data-ttu-id="40649-232">CRM-system är ofta mycket anpassade.</span><span class="sxs-lookup"><span data-stu-id="40649-232">Often CRM systems are highly customized.</span></span> <span data-ttu-id="40649-233">Du kan anpassa Power Automate flöden.</span><span class="sxs-lookup"><span data-stu-id="40649-233">You can customize the Power Automate flows.</span></span> <span data-ttu-id="40649-234">Följ guiden för fältmappning och gör vid behov lämpliga ändringar i stegen i Power Automate flöden.</span><span class="sxs-lookup"><span data-stu-id="40649-234">Follow the field mapping guide, and if necessary, make appropriate changes in the steps of the Power Automate flows.</span></span>  <span data-ttu-id="40649-235">Microsoft Partner Centers till CRM-mappningar tillhandahålls, men baserat på din CRM-miljö kan du välja att anpassa fälten ytterligare.</span><span class="sxs-lookup"><span data-stu-id="40649-235">Microsoft Partner Centers to CRM mappings are provided, but based on your CRM environment, you can choose to further customize the fields.</span></span>

<span data-ttu-id="40649-236">Flera steg i varje Power Automate kan anpassas efter dina behov.</span><span class="sxs-lookup"><span data-stu-id="40649-236">Multiple steps of each of the Power Automate flows can be customized based on your needs.</span></span> <span data-ttu-id="40649-237">Följande är exempel på tillgängliga anpassningar:</span><span class="sxs-lookup"><span data-stu-id="40649-237">The following are examples of available customizations:</span></span>

1. <span data-ttu-id="40649-238">Anpassa fälten för skapa eller uppdatera händelser i Partnercenter till CRM-referenssynkronisering:</span><span class="sxs-lookup"><span data-stu-id="40649-238">To customize the fields for the create or update events in the Partner Center to CRM referral synchronization:</span></span>

   1. <span data-ttu-id="40649-239">Välj PartnerCenter till Salesforce CRM (Insider Preview).</span><span class="sxs-lookup"><span data-stu-id="40649-239">Select Partner Center to Salesforce CRM (Insider Preview).</span></span>

   2. <span data-ttu-id="40649-240">Välj **Redigera** för att redigera/anpassa Power Automate flöde.</span><span class="sxs-lookup"><span data-stu-id="40649-240">Select **Edit** to edit/customize the Power Automate flow.</span></span>

   3. <span data-ttu-id="40649-241">Välj **(Omfång) Synkronisera leadet eller affärsmöjligheten**.</span><span class="sxs-lookup"><span data-stu-id="40649-241">Select **(Scope) Synchronize the lead or opportunity**.</span></span>

2. <span data-ttu-id="40649-242">Om du vill anpassa CRM-fältmappningar för att skapa **händelser väljer du Om det är en ny delad affärsmöjlighet och sedan**.</span><span class="sxs-lookup"><span data-stu-id="40649-242">To customize CRM field mappings for create events, select **If it’s new Shared opportunity, then**.</span></span> <span data-ttu-id="40649-243">Välj understeget om **ja och** expandera sedan Skapa en ny affärsmöjlighet **i CRM.**</span><span class="sxs-lookup"><span data-stu-id="40649-243">Select the sub-step **if yes** and then expand **Creating a new opportunity in the CRM**.</span></span> <span data-ttu-id="40649-244">Du kan redigera mappningarna i det här avsnittet med hjälp av guiden Fältmappning.</span><span class="sxs-lookup"><span data-stu-id="40649-244">You can edit the mappings in this section using the Field Mapping Guide.</span></span>

   1. <span data-ttu-id="40649-245">Om du vill anpassa CRM-fältmappningar för uppdateringshändelser väljer du steget "(Omfång) Synkronisera lead eller affärsmöjlighet".</span><span class="sxs-lookup"><span data-stu-id="40649-245">To customize CRM field mappings for update events, select the step "(Scope) Synchronize the lead or opportunity".</span></span>

   2. <span data-ttu-id="40649-246">Välj **Om det är en uppdatering av en affärsmöjlighet, sedan**.</span><span class="sxs-lookup"><span data-stu-id="40649-246">Select **If it’s an update to an opportunity, then**.</span></span> <span data-ttu-id="40649-247">Välj understeget **om ja** och expandera sedan If difference between the opportunity objects in Partner Center and CRM (Om skillnaden mellan **affärsmöjlighetsobjekten i Partnercenter och CRM) och sedan**.</span><span class="sxs-lookup"><span data-stu-id="40649-247">Select the sub-step **if yes** and then expand **If difference between the opportunity objects in Partner Center and CRM, then**.</span></span>  

   3. <span data-ttu-id="40649-248">Välj **Om ja följt** av Uppdatera befintlig **affärsmöjlighet**</span><span class="sxs-lookup"><span data-stu-id="40649-248">Select **If yes** followed with **Update existing opportunity**</span></span>

3. <span data-ttu-id="40649-249">Så här anpassar du fälten för referenssynkronisering från CRM till dator för uppdateringshändelser:</span><span class="sxs-lookup"><span data-stu-id="40649-249">To customize the fields for CRM to PC referral synchronization for update events:</span></span>

   1. <span data-ttu-id="40649-250">Välj **Redigera**  för att redigera/anpassa Power Automate flöde.</span><span class="sxs-lookup"><span data-stu-id="40649-250">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   2. <span data-ttu-id="40649-251">Välj **(Omfång) Synkronisera affärsmöjligheten**.</span><span class="sxs-lookup"><span data-stu-id="40649-251">Select **(Scope) Synchronize the opportunity**.</span></span>

   3. <span data-ttu-id="40649-252">Om du vill anpassa CRM-fältmappningar (baserat på guiden för fältmappningar) för uppdateringshändelser väljer du Om det är skillnad mellan leadobjekten i **Partnercenter och CRM och sedan**.</span><span class="sxs-lookup"><span data-stu-id="40649-252">For customizing CRM field mappings (based on field mappings guide) for update events, select **If there is difference between the lead objects in Partner Center and CRM, then**.</span></span>

   4. <span data-ttu-id="40649-253">Välj understeget om **ja och** expandera sedan steget Uppdatera en referens **med affärsmöjlighetsdata**.</span><span class="sxs-lookup"><span data-stu-id="40649-253">Select the sub-step **if yes** and then expand the step **Update a referral with opportunity data**.</span></span>

   <span data-ttu-id="40649-254">Du kan redigera mappningarna i det här avsnittet baserat på guiden Fältmappning.</span><span class="sxs-lookup"><span data-stu-id="40649-254">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

4. <span data-ttu-id="40649-255">Vill du anpassa fälten för referenssynkronisering mellan CRM och dator för att skapa händelser?</span><span class="sxs-lookup"><span data-stu-id="40649-255">To customize the fields for CRM to PC referral synchronization for create events?</span></span>

   1. <span data-ttu-id="40649-256">Välj **Redigera**  för att redigera/anpassa Power Automate flöde.</span><span class="sxs-lookup"><span data-stu-id="40649-256">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   2. <span data-ttu-id="40649-257">Välj **(Omfång) Synkronisera hänvisningar.**</span><span class="sxs-lookup"><span data-stu-id="40649-257">Select **(Scope) Synchronizing Referrals.**</span></span>

   3. <span data-ttu-id="40649-258">Om du vill anpassa CRM-fältmappningar (baserat på fältmappningsguiden) för att skapa händelser väljer **du Skapa Microsoft-referens.**</span><span class="sxs-lookup"><span data-stu-id="40649-258">For customizing CRM field mappings (based on field mappings guide) for create events, select **Create Microsoft Referral**.</span></span>

<span data-ttu-id="40649-259">Du kan redigera mappningarna i det här avsnittet baserat på guiden Fältmappning.</span><span class="sxs-lookup"><span data-stu-id="40649-259">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>


## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a><span data-ttu-id="40649-260">Synkronisering av dubbelriktad hänvisning från end-to-end</span><span class="sxs-lookup"><span data-stu-id="40649-260">End-to-end bi-directional co-sell referral synchronization</span></span>

<span data-ttu-id="40649-261">När du har installerat, konfigurerat och anpassat Power Automate lösningen kan du testa synkroniseringen av hänvisningar till säljförsäljning mellan Salesforce CRM och Partnercenter.</span><span class="sxs-lookup"><span data-stu-id="40649-261">Once you have installed, configured, and customized the Power Automate solution, you can test for Co-sell referrals synchronization between Salesforce CRM and Partner Center.</span></span>

### <a name="pre-requisites"></a><span data-ttu-id="40649-262">Förutsättningar</span><span class="sxs-lookup"><span data-stu-id="40649-262">Pre-requisites</span></span>

<span data-ttu-id="40649-263">För att synkronisera hänvisningarna mellan Partner Center och Salesforce CRM måste Power Automate-lösningen tydligt avgränsa Microsoft-specifika referensfält.</span><span class="sxs-lookup"><span data-stu-id="40649-263">To synchronize the referrals across Partner Center and Salesforce CRM, the Power Automate solution needs to clearly demarcate Microsoft-specific referral fields.</span></span> <span data-ttu-id="40649-264">Den här identifieringen ger säljteamen möjlighet att bestämma vilka hänvisningar de vill dela med Microsoft för säljförsäljning.</span><span class="sxs-lookup"><span data-stu-id="40649-264">This identification provides your seller teams with the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

<span data-ttu-id="40649-265">En uppsättning anpassade fält är tillgängliga som en del av Partner Center-referenssynkronisering för Salesforce CRM-lösningens **affärsmöjlighetsentitet.**</span><span class="sxs-lookup"><span data-stu-id="40649-265">A set of custom fields is available as part of Partner Center Referrals Synchronization for Salesforce CRM solution **Opportunity** entity.</span></span> <span data-ttu-id="40649-266">En CRM-administratörsanvändare måste skapa ett separat CRM-avsnitt med de **anpassade affärsmöjlighetsfälten.**</span><span class="sxs-lookup"><span data-stu-id="40649-266">A CRM admin user will need to create a separate CRM section with the **Opportunity** custom fields.</span></span>

<span data-ttu-id="40649-267">Följande anpassade fält bör ingå i CRM-avsnittet:</span><span class="sxs-lookup"><span data-stu-id="40649-267">The following custom fields should be part of the CRM section:</span></span>

- <span data-ttu-id="40649-268">**Synkronisera med Partnercenter:** Om du vill synkronisera affärsmöjligheten med Microsoft Partner Center</span><span class="sxs-lookup"><span data-stu-id="40649-268">**Sync with Partner Center**: Whether to sync the opportunity with Microsoft Partner Center</span></span>

- <span data-ttu-id="40649-269">**Hänvisningsidentifierare:** Ett skrivskyddade identifierarfält för Microsoft Partner Center-hänvisning</span><span class="sxs-lookup"><span data-stu-id="40649-269">**Referral Identifier**: A read-only identifier field for Microsoft Partner Center referral</span></span>

- <span data-ttu-id="40649-270">**Hänvisningslänk:** En skrivskyddade länk till hänvisningen i Microsoft Partner Center</span><span class="sxs-lookup"><span data-stu-id="40649-270">**Referral Link**: A read-only link to the referral in Microsoft Partner Center</span></span>

- <span data-ttu-id="40649-271">**Hur kan Microsoft hjälpa:** Hjälp krävs från Microsoft för hänvisningen</span><span class="sxs-lookup"><span data-stu-id="40649-271">**How can Microsoft help**: Help required from Microsoft for the referral</span></span>

- <span data-ttu-id="40649-272">**Produkter:** Lista över produkter som är associerade med den här affärsmöjligheten</span><span class="sxs-lookup"><span data-stu-id="40649-272">**Products**: List of products associated with this opportunity</span></span>

- <span data-ttu-id="40649-273">**Granskning:** En skrivskyddade granskningslogg för synkronisering med PartnerCenter-referenser</span><span class="sxs-lookup"><span data-stu-id="40649-273">**Audit**: A read-only audit trail for syncing with Partner Center referrals</span></span>

### <a name="scenarios"></a><span data-ttu-id="40649-274">Scenarier:</span><span class="sxs-lookup"><span data-stu-id="40649-274">SCENARIOS:</span></span>

1. <span data-ttu-id="40649-275">Referenssynkronisering när en hänvisning skapas eller uppdateras i CRM och synkroniseras i Partnercenter:</span><span class="sxs-lookup"><span data-stu-id="40649-275">Referral synchronization when referral is created or updated in CRM and synced in Partner Center:</span></span>

   1. <span data-ttu-id="40649-276">Logga in på Salesforce CRM-miljön med användare som har insyn i **avsnittet Affärsmöjlighet** i CRM.</span><span class="sxs-lookup"><span data-stu-id="40649-276">Sign into your Salesforce CRM environment with user who has visibility in the **Opportunity** section of the CRM.</span></span>

   2. <span data-ttu-id="40649-277">Se till att följande avsnitt visas när du skapar en "Ny affärsmöjlighet" i Salesforce CRM-miljön</span><span class="sxs-lookup"><span data-stu-id="40649-277">Ensure that the following section is present when you create a "New Opportunity" in Salesforce CRM environment</span></span>

      :::image type="content" source="images/salesforce/salesforce-scenario-1.png" alt-text="Salesforce-miljö.":::

   3. <span data-ttu-id="40649-279">Om du vill synkronisera den här affärsmöjligheten med Microsoft Partner Center måste du ange följande fält i kortvyn:</span><span class="sxs-lookup"><span data-stu-id="40649-279">To synchronize this opportunity with Microsoft Partner Center, ensure that you set the following fields in the card view:</span></span>

       - <span data-ttu-id="40649-280">"Synkronisera med Partnercenter": Ja</span><span class="sxs-lookup"><span data-stu-id="40649-280">"Sync with Partner Center": Yes</span></span>
       - <span data-ttu-id="40649-281">"Hur kan Microsoft hjälpa?": Välj bland följande alternativ:</span><span class="sxs-lookup"><span data-stu-id="40649-281">"How can Microsoft help?": Select from the following options:</span></span>
       - <span data-ttu-id="40649-282">Produkter: Produktens lösnings-ID:er</span><span class="sxs-lookup"><span data-stu-id="40649-282">Products: Solution IDs of the product</span></span>

   4. <span data-ttu-id="40649-283">När du har angett alternativet Synkronisera  **med Partnercenter för affärsmöjlighet** till **Ja,** vänta i 10 minuter och logga in på ditt Partnercenter-konto.</span><span class="sxs-lookup"><span data-stu-id="40649-283">Once you have set the opportunity  **Sync with Partner Center** option to **Yes**, wait 10 minutes, sign into your Partner Center account.</span></span> <span data-ttu-id="40649-284">Dina hänvisningar synkroniseras med Salesforce CRM.</span><span class="sxs-lookup"><span data-stu-id="40649-284">Your referrals will be synchronized with Salesforce CRM.</span></span>

   5. <span data-ttu-id="40649-285">När alternativet "Synkronisera med Partnercenter" är inställt på "Ja", kommer ändringarna att synkroniseras med ditt Partnercenter-konto om du uppdaterar affärsmöjligheten i Salesforce CRM.</span><span class="sxs-lookup"><span data-stu-id="40649-285">When the "Sync with Partner Center" option is set to "Yes", if you update the opportunity in Salesforce CRM, the changes will synchronize with your Partner Center account.</span></span>

   6. <span data-ttu-id="40649-286">Affärsmöjligheter som har synkroniserats med Partnercenter identifieras med ✔icon i Salesforce CRM.</span><span class="sxs-lookup"><span data-stu-id="40649-286">Opportunities that are synchronized successfully with Partner Center will be identified with ✔icon in Salesforce CRM.</span></span>

2. <span data-ttu-id="40649-287">Referenssynkronisering när hänvisningar skapas eller uppdateras i Microsoft Partner Center och synkroniseras i Salesforce CRM-miljön:</span><span class="sxs-lookup"><span data-stu-id="40649-287">Referral Synchronization when referral is created or updated in Microsoft Partner Center and synchronized in Salesforce CRM environment:</span></span>

    1. <span data-ttu-id="40649-288">Logga in på instrumentpanelen i [Partnercenter.](https://partner.microsoft.com/dashboard/home)</span><span class="sxs-lookup"><span data-stu-id="40649-288">Sign into your Partner Center [dashboard](https://partner.microsoft.com/dashboard/home).</span></span>

    2. <span data-ttu-id="40649-289">Välj **Referenser** på den vänstra menyn.</span><span class="sxs-lookup"><span data-stu-id="40649-289">Select **Referrals** from the left-hand menu.</span></span>

    3. <span data-ttu-id="40649-290">Skapa en ny hänvisning om säljförsäljning från Partnercenter genom att klicka på alternativet "Nytt avtal".</span><span class="sxs-lookup"><span data-stu-id="40649-290">Create a new Co-sell referral from Partner Center by clicking "New deal" option.</span></span>

    4. <span data-ttu-id="40649-291">Logga in på Salesforce CRM-miljön.</span><span class="sxs-lookup"><span data-stu-id="40649-291">Sign into your Salesforce CRM environment.</span></span>

    5. <span data-ttu-id="40649-292">Gå till **Öppna affärsmöjligheter.**</span><span class="sxs-lookup"><span data-stu-id="40649-292">Navigate to **Open Opportunities**.</span></span> <span data-ttu-id="40649-293">Hänvisningen som skapades i Microsoft Partner Center synkroniseras nu i Salesforce CRM.</span><span class="sxs-lookup"><span data-stu-id="40649-293">The referral created in Microsoft Partner Center is now synchronized in Salesforce CRM.</span></span>

       :::image type="content" source="images/salesforce/salesforce-casino-e.png" alt-text="Skärmen Salesforce-affärsmöjlighet.":::

    6. <span data-ttu-id="40649-295">När du väljer en synkroniserad hänvisning fylls kortvisningsinformationen i.</span><span class="sxs-lookup"><span data-stu-id="40649-295">When you select a synchronized referral, the card view details are populated.</span></span>

## <a name="next-steps"></a><span data-ttu-id="40649-296">Nästa steg</span><span class="sxs-lookup"><span data-stu-id="40649-296">Next steps</span></span>

- [<span data-ttu-id="40649-297">Hantera leads</span><span class="sxs-lookup"><span data-stu-id="40649-297">Manage leads</span></span>](manage-leads.md)

- [<span data-ttu-id="40649-298">Hantera möjligheter till samförsäljning</span><span class="sxs-lookup"><span data-stu-id="40649-298">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)

- [<span data-ttu-id="40649-299">Partnercenter – webhooks</span><span class="sxs-lookup"><span data-stu-id="40649-299">Partner Center webhooks</span></span>](/partner-center/develop/partner-center-webhooks)
