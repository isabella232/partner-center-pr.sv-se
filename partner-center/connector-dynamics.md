---
title: Co-Sälj koppling för Dynamics 365 CRM-partner Center
ms.topic: how-to
ms.date: 05/27/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Synkronisera dina referenser i Partner Center med din co-sälje Connector för Dynamics 365 CRM. Säljare kan sedan sälja tillsammans med Microsoft från dina CRM-system.
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: c92938bbb4ffa6875419d06a9bbf23010ee60724
ms.sourcegitcommit: 7e32544cf91f932cbeb053c9de506ba9ee773fe2
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 11/20/2020
ms.locfileid: "94947826"
---
# <a name="co-sell-connector-for-dynamics-365-crm--overview"></a><span data-ttu-id="68d90-104">Co-Sälj koppling för Dynamics 365 CRM – översikt</span><span class="sxs-lookup"><span data-stu-id="68d90-104">Co-sell connector for Dynamics 365 CRM – Overview</span></span>

### <a name="appropriate-roles"></a><span data-ttu-id="68d90-105">Lämpliga roller</span><span class="sxs-lookup"><span data-stu-id="68d90-105">Appropriate roles</span></span>

- <span data-ttu-id="68d90-106">Referens administratör</span><span class="sxs-lookup"><span data-stu-id="68d90-106">Referrals admin</span></span>
- <span data-ttu-id="68d90-107">System administratör eller systemanpassare på CRM</span><span class="sxs-lookup"><span data-stu-id="68d90-107">System admin or system customizer on the CRM</span></span>

<span data-ttu-id="68d90-108">Partner Center Co-sälje Connector gör det möjligt för dina säljare att sälja med Microsoft från dina CRM-system.</span><span class="sxs-lookup"><span data-stu-id="68d90-108">Partner Center co-sell connector enables your sellers to co-sell with Microsoft from within your CRM systems.</span></span> <span data-ttu-id="68d90-109">De behöver inte tränas att använda Partner Center för att hantera samförsäljnings avtal.</span><span class="sxs-lookup"><span data-stu-id="68d90-109">They won’t have to be trained to use Partner Center to manage Co-sell deals.</span></span> <span data-ttu-id="68d90-110">Använd Co-Sälj-anslutningarna för att skapa en ny samförsäljnings hänvisning för att engagera en Microsoft-säljare, ta emot hänvisningar från Microsoft-säljaren, acceptera/neka referenser, ändra avtals data som avtals värde och stängnings datum.</span><span class="sxs-lookup"><span data-stu-id="68d90-110">Use the Co-sell connectors, to create a new Co-sell referral to engage a Microsoft seller, receive referrals from the Microsoft seller, accept/decline referrals, modify deal data such as deal value, and closing date.</span></span> <span data-ttu-id="68d90-111">Du kan också ta emot uppdateringar från Microsoft-säljarna om dessa samförsäljnings avtal.</span><span class="sxs-lookup"><span data-stu-id="68d90-111">You can also receive any updates from the Microsoft sellers on these Co-sell deals.</span></span> <span data-ttu-id="68d90-112">Du kan göra så att alla dina referenser fungerar i det valda CRM-nätverket i stället för i Partner Center.</span><span class="sxs-lookup"><span data-stu-id="68d90-112">You can do all of your referrals work within the CRM of your choice rather than in Partner Center.</span></span> 

<span data-ttu-id="68d90-113">Lösningen baseras på Microsoft Power automatiserings lösning och använder API: er för partner Center.</span><span class="sxs-lookup"><span data-stu-id="68d90-113">The solution is based on Microsoft Power Automate Solution and uses Partner Center APIs.</span></span>

## <a name="before-you-install---pre-requisites"></a><span data-ttu-id="68d90-114">Innan du installerar-krav</span><span class="sxs-lookup"><span data-stu-id="68d90-114">Before you install - pre-requisites</span></span>

|<span data-ttu-id="68d90-115">**Ämnen**</span><span class="sxs-lookup"><span data-stu-id="68d90-115">**Topics**</span></span>   |<span data-ttu-id="68d90-116">**Detaljer**</span><span class="sxs-lookup"><span data-stu-id="68d90-116">**Details**</span></span>   |<span data-ttu-id="68d90-117">**Länkar**</span><span class="sxs-lookup"><span data-stu-id="68d90-117">**Links**</span></span>   |
|--------------|--------------------|------|
|<span data-ttu-id="68d90-118">Microsoft Partner Network-ID</span><span class="sxs-lookup"><span data-stu-id="68d90-118">Microsoft Partner Network ID</span></span> |<span data-ttu-id="68d90-119">Du behöver ett giltigt MPN-ID</span><span class="sxs-lookup"><span data-stu-id="68d90-119">You need a valid MPN ID</span></span>|<span data-ttu-id="68d90-120">För att ansluta till [MPN](https://partner.microsoft.com/)</span><span class="sxs-lookup"><span data-stu-id="68d90-120">To join [MPN](https://partner.microsoft.com/)</span></span>|
|<span data-ttu-id="68d90-121">Samförsäljnings klar</span><span class="sxs-lookup"><span data-stu-id="68d90-121">Cosell ready</span></span>|<span data-ttu-id="68d90-122">Din lösning för IP/tjänster måste vara samförsäljnings klar.</span><span class="sxs-lookup"><span data-stu-id="68d90-122">Your IP/Services solution must be co-sell ready.</span></span>|[<span data-ttu-id="68d90-123">Sälj med Microsoft</span><span class="sxs-lookup"><span data-stu-id="68d90-123">Sell with Microsoft</span></span>](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|<span data-ttu-id="68d90-124">Partnercenter-konto</span><span class="sxs-lookup"><span data-stu-id="68d90-124">Partner Center account</span></span>|<span data-ttu-id="68d90-125">Det MPN-ID som är kopplat till Partner Center-klienten måste vara samma som det MPN-ID som är kopplat till din co-Sälj-lösning.</span><span class="sxs-lookup"><span data-stu-id="68d90-125">The MPN ID associated with the Partner Center tenant must be same as the MPN ID associated with your Co-sell solution.</span></span> <span data-ttu-id="68d90-126">Kontrol lera att du kan se dina samförsäljnings referenser på Partner Center-portalen innan du distribuerar anslutningarna.</span><span class="sxs-lookup"><span data-stu-id="68d90-126">Verify that you can see your co-sell referrals in Partner Center portal before deploying the connectors.</span></span>|[<span data-ttu-id="68d90-127">Hantera ditt konto</span><span class="sxs-lookup"><span data-stu-id="68d90-127">Manage your account</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="68d90-128">Användar roller för partner Center</span><span class="sxs-lookup"><span data-stu-id="68d90-128">Partner Center user roles</span></span>|<span data-ttu-id="68d90-129">Den medarbetare som ska installera och använda anslutningarna måste vara en referens administratör</span><span class="sxs-lookup"><span data-stu-id="68d90-129">The employee who will install and use the connectors must be a Referrals admin</span></span>|[<span data-ttu-id="68d90-130">Tilldela användarroller och -behörigheter</span><span class="sxs-lookup"><span data-stu-id="68d90-130">Assign users roles and permissions</span></span>](create-user-accounts-and-set-permissions.md)| |<span data-ttu-id="68d90-131">Dynamics 365 CRM</span><span class="sxs-lookup"><span data-stu-id="68d90-131">Dynamics 365 CRM</span></span>|<span data-ttu-id="68d90-132">Användar rollen CRM är system administratör eller systemanpassare</span><span class="sxs-lookup"><span data-stu-id="68d90-132">The CRM user role is System admin or System customizer</span></span>|[<span data-ttu-id="68d90-133">Tilldela roller i Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="68d90-133">Assign roles in Dynamics 365</span></span>](/dynamics365/customerengagement/on-premises/customize/privileges-required-customization)|
|<span data-ttu-id="68d90-134">Flödes konto för automatiserad energi</span><span class="sxs-lookup"><span data-stu-id="68d90-134">Power Automate Flow Account</span></span>|<span data-ttu-id="68d90-135">Ett aktivt [energi automatiserat](https://flow.microsoft.com) konto för CRM-systemadministratören eller systemanpassaren.</span><span class="sxs-lookup"><span data-stu-id="68d90-135">An active [Power Automate](https://flow.microsoft.com) account for the CRM System admin or System customizer.</span></span> <span data-ttu-id="68d90-136">Användaren ska logga in i [energi spar läge](https://flow.microsoft.com) minst en gång före installationen.</span><span class="sxs-lookup"><span data-stu-id="68d90-136">That user should sign into [Power Automate](https://flow.microsoft.com) at least once before installation.</span></span>|

## <a name="install-partner-center-referrals-synchronization-for-dynamics-365-power-automate-solution"></a><span data-ttu-id="68d90-137">Installera synkronisering av Partner Center-referenser för Dynamics 365 (energi automatiserings lösning)</span><span class="sxs-lookup"><span data-stu-id="68d90-137">Install Partner Center Referrals Synchronization for Dynamics 365 (Power Automate Solution)</span></span>

1. <span data-ttu-id="68d90-138">Gå till [Power automatisera](https://flow.microsoft.com) och välj **miljöer** i det högra övre hörnet.</span><span class="sxs-lookup"><span data-stu-id="68d90-138">Go to [Power Automate](https://flow.microsoft.com) and select **Environments** on the right top corner.</span></span> <span data-ttu-id="68d90-139">I det här steget visas tillgängliga CRM-instanser.</span><span class="sxs-lookup"><span data-stu-id="68d90-139">This step will show you the available CRM instances.</span></span>

2. <span data-ttu-id="68d90-140">Välj lämplig CRM-instans i list rutan i det högra övre hörnet.</span><span class="sxs-lookup"><span data-stu-id="68d90-140">Select the appropriate CRM instance from the drop-down on the right top corner.</span></span>

3. <span data-ttu-id="68d90-141">Välj **lösningar** i det vänstra navigerings fältet.</span><span class="sxs-lookup"><span data-stu-id="68d90-141">Select **Solutions** on the left navigation bar.</span></span>

4. <span data-ttu-id="68d90-142">Klicka på länken **Öppna AppSource** på den översta menyn.</span><span class="sxs-lookup"><span data-stu-id="68d90-142">Click on the **Open AppSource** link on the top menu.</span></span>

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="Öppna AppSource":::

5. <span data-ttu-id="68d90-144">Sök efter **partner Center-referenser till kopplingar för Dynamics365** på popup-skärmen.</span><span class="sxs-lookup"><span data-stu-id="68d90-144">Search for **Partner Center Referrals Connectors for Dynamics365** in the pop-up screen.</span></span>  

6. <span data-ttu-id="68d90-145">Klicka på knappen **Hämta nu** och **Fortsätt** sedan.</span><span class="sxs-lookup"><span data-stu-id="68d90-145">Click the **Get it now** button and then **Continue**.</span></span>

7. <span data-ttu-id="68d90-146">Då öppnas sidan där du kan välja CRM-miljön (Dynamics 365) för att installera programmet.</span><span class="sxs-lookup"><span data-stu-id="68d90-146">This opens the page where you can select the CRM (Dynamics 365) environment to install application.</span></span>  <span data-ttu-id="68d90-147">Godkänn de allmänna villkoren.</span><span class="sxs-lookup"><span data-stu-id="68d90-147">Agree to terms and conditions.</span></span>

8. <span data-ttu-id="68d90-148">Sedan dirigeras du till sidan **Hantera dina lösningar** .</span><span class="sxs-lookup"><span data-stu-id="68d90-148">You're then directed to the **Manage your solutions** page.</span></span>  <span data-ttu-id="68d90-149">Gå till "Partner Center-referenser" genom att använda pilknapparna längst ned på sidan.</span><span class="sxs-lookup"><span data-stu-id="68d90-149">Navigate to "Partner Center Referrals" by using the arrow buttons on the bottom of the page.</span></span> <span data-ttu-id="68d90-150">**Installationen är schemalagd** bör visas bredvid lösningen för partner Center-hänvisningar.</span><span class="sxs-lookup"><span data-stu-id="68d90-150">**Installation scheduled** should appear next to Partner Center Referrals solution.</span></span> <span data-ttu-id="68d90-151">Installationen tar 10-15 minuter.</span><span class="sxs-lookup"><span data-stu-id="68d90-151">Installation will take 10-15 minutes.</span></span> 

9. <span data-ttu-id="68d90-152">När installationen är klar navigerar du tillbaka till [Automatisera](https://flow.microsoft.com) och väljer **lösningar** från det vänstra navigerings fältet.</span><span class="sxs-lookup"><span data-stu-id="68d90-152">Once the installation is complete, navigate back to [Power Automate](https://flow.microsoft.com) and select **Solutions** from left navigation area.</span></span> <span data-ttu-id="68d90-153">Observera att **synkroniseringen av Partner Center för Dynamics 365** är tillgänglig i lösnings listan.</span><span class="sxs-lookup"><span data-stu-id="68d90-153">Notice that **Partner Center Referrals Synchronization for Dynamics 365** is available in the Solutions list.</span></span>

10. <span data-ttu-id="68d90-154">Välj **synkronisering av Partner Center-referenser för Dynamics 365**.</span><span class="sxs-lookup"><span data-stu-id="68d90-154">Select **Partner Center Referrals Synchronization for Dynamics 365**.</span></span> <span data-ttu-id="68d90-155">Följande energi flöden och entiteter är tillgängliga:</span><span class="sxs-lookup"><span data-stu-id="68d90-155">The following Power Automate flows and entities are available:</span></span>

    :::image type="content" source="images/cosellconnectors/dynamics-available-crms.png" alt-text="Tillgängliga CRMS":::

## <a name="best-practice-test-before-you-go-live"></a><span data-ttu-id="68d90-157">Bästa praxis: testa innan du går live</span><span class="sxs-lookup"><span data-stu-id="68d90-157">Best practice: test before you go live</span></span>

<span data-ttu-id="68d90-158">Innan du installerar, konfigurerar och anpassar den automatiserade energi lösningen i produktions miljön måste du testa lösningen på en mellanlagringsplatsen CRM-instans.</span><span class="sxs-lookup"><span data-stu-id="68d90-158">Before you install, configure, and customize the Power Automate solution on the production environment, be sure to test the solution on a staging CRM instance.</span></span>

- <span data-ttu-id="68d90-159">Installera Microsoft Power automatiserings lösning på en mellanlagringsplatss miljö/CRM-instans.</span><span class="sxs-lookup"><span data-stu-id="68d90-159">Install Microsoft Power Automate solution on a staging environment/CRM instance.</span></span>
- <span data-ttu-id="68d90-160">Gör en kopia av lösningen och kör din konfiguration och automatisera automatiserade flödes anpassningar i mellanlagrings miljön.</span><span class="sxs-lookup"><span data-stu-id="68d90-160">Make a copy of the solution and run your configuration and Power Automate flow customizations on the staging environment.</span></span>
- <span data-ttu-id="68d90-161">Testa lösningen på en mellanlagrings-/CRM-instans.</span><span class="sxs-lookup"><span data-stu-id="68d90-161">Test the solution on a staging/CRM instance.</span></span> 
- <span data-ttu-id="68d90-162">Vid lyckad, importera som hanterad lösning till produktions instansen.</span><span class="sxs-lookup"><span data-stu-id="68d90-162">On success, import as managed solution to the production instance.</span></span> 

## <a name="configure-the-solution"></a><span data-ttu-id="68d90-163">Konfigurera lösningen</span><span class="sxs-lookup"><span data-stu-id="68d90-163">Configure the solution</span></span>

1. <span data-ttu-id="68d90-164">När du har installerat lösningen i din CRM-instans går du tillbaka till [Energis par](https://flow.microsoft.com/).</span><span class="sxs-lookup"><span data-stu-id="68d90-164">Once you have installed the solution in your CRM instance, navigate back to [Power Automate](https://flow.microsoft.com/).</span></span>


2. <span data-ttu-id="68d90-165">I list rutan **miljöer** i det högra hörnet väljer du den CRM-instans där du installerade den automatiserade energi lösningen.</span><span class="sxs-lookup"><span data-stu-id="68d90-165">From the **Environments** drop-down on the right top corner, select the CRM instance where you installed the Power Automate solution.</span></span>

3. <span data-ttu-id="68d90-166">Du måste skapa anslutningar som associerar de tre användar kontona:</span><span class="sxs-lookup"><span data-stu-id="68d90-166">You'll need to create connections that associate the three user accounts:</span></span>

   - <span data-ttu-id="68d90-167">Partner Center-användare med referenser för administratörs behörighet</span><span class="sxs-lookup"><span data-stu-id="68d90-167">Partner Center user with referrals admin credentials</span></span>

   - <span data-ttu-id="68d90-168">Partnercenter-händelser</span><span class="sxs-lookup"><span data-stu-id="68d90-168">Partner Center Events</span></span>

   - <span data-ttu-id="68d90-169">CRM-administratören med de energi automatiserade flödena i lösningen.</span><span class="sxs-lookup"><span data-stu-id="68d90-169">CRM admin with the Power Automate flows in the solution.</span></span>

      1. <span data-ttu-id="68d90-170">Välj **anslutningar** i det vänstra navigerings fältet och välj lösningen "Partner Center-hänvisningar" i listan.</span><span class="sxs-lookup"><span data-stu-id="68d90-170">Select **Connections** from the left navigation bar and select the “Partner Center Referrals” solution from the list.</span></span>

      2. <span data-ttu-id="68d90-171">Skapa en anslutning genom att klicka på **skapa en anslutning**.</span><span class="sxs-lookup"><span data-stu-id="68d90-171">Create a connection by clicking **Create a connection**.</span></span>

         :::image type="content" source="images/cosellconnectors/dynamics1.png" alt-text="Skapa anslutning":::

      3. <span data-ttu-id="68d90-173">Sök efter **partner Center-referenser (för hands version)** i Sök fältet i det övre högra hörnet.</span><span class="sxs-lookup"><span data-stu-id="68d90-173">Search for **Partner Center Referrals (preview)** in the search bar on the top-right corner.</span></span>

      4. <span data-ttu-id="68d90-174">Skapa en anslutning för din partner Center-användare med rollen autentiseringsuppgifter för referral admin.</span><span class="sxs-lookup"><span data-stu-id="68d90-174">Create a connection for your Partner Center user with the credentials role of Referrals admin.</span></span>

      5. <span data-ttu-id="68d90-175">Skapa sedan en anslutning för partner Center-händelser för din partner Center-användare med autentiseringsuppgifterna för referral admin.</span><span class="sxs-lookup"><span data-stu-id="68d90-175">Next, create a Partner Center Events connection for your Partner Center user with the credentials of Referrals admin.</span></span>

      6. <span data-ttu-id="68d90-176">Skapa en anslutning för Common Data Service (aktuell miljö) för CRM-administratörens användare.</span><span class="sxs-lookup"><span data-stu-id="68d90-176">Create a connection for Common Data Service (current environment) for the CRM administrator user.</span></span>
       
     
      7. <span data-ttu-id="68d90-177">När du har lagt till alla anslutningar bör du se följande anslutningar i din miljö:</span><span class="sxs-lookup"><span data-stu-id="68d90-177">Once you have all the Connections added, you should see the following Connections in your environment:</span></span>

:::image type="content" source="images/cosellconnectors/dynamics2.png" alt-text="Anslutningar":::
   
## <a name="edit-the-connections"></a><span data-ttu-id="68d90-179">Redigera anslutningarna</span><span class="sxs-lookup"><span data-stu-id="68d90-179">Edit the connections</span></span>

1. <span data-ttu-id="68d90-180">Gå tillbaka till sidan **lösningar** och välj **standard lösning**.</span><span class="sxs-lookup"><span data-stu-id="68d90-180">Return to the **Solutions** page and select **Default Solution**.</span></span> <span data-ttu-id="68d90-181">Välj **anslutnings referens (för hands version)** genom att klicka på **alla**.</span><span class="sxs-lookup"><span data-stu-id="68d90-181">Select **Connection Reference (preview)** by clicking **All**.</span></span>

:::image type="content" source="images/cosellconnectors/dynamics3.png" alt-text="Anslut":::

2. <span data-ttu-id="68d90-183">Redigera varje anslutning en i taget genom att välja ikonen tre punkter.</span><span class="sxs-lookup"><span data-stu-id="68d90-183">Edit each of the Connections one by one by selecting the three dots icon.</span></span> <span data-ttu-id="68d90-184">Lägg till relevanta anslutningar.</span><span class="sxs-lookup"><span data-stu-id="68d90-184">Add the relevant connections.</span></span>

:::image type="content" source="images/cosellconnectors/dynamics4.png" alt-text="Anslutningar i listan"::: 

3.  <span data-ttu-id="68d90-186">Aktivera flödena i följande ordning:</span><span class="sxs-lookup"><span data-stu-id="68d90-186">Turn on the flows in the following sequence:</span></span>
- <span data-ttu-id="68d90-187">Partner Center – registrering av webhook (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="68d90-187">Partner Center Webhook Registration (Insider Preview)</span></span>
- <span data-ttu-id="68d90-188">Skapa samförsäljnings hänvisning – Dynamics 365 till Partner Center (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="68d90-188">Create Co-sell Referral – Dynamics 365 to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="68d90-189">Partner Center Microsoft Co-Sälj hänvisnings uppdateringar till Dynamics 365 (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="68d90-189">Partner Center Microsoft Co-sell Referral Updates to Dynamics 365 (Insider Preview)</span></span>
- <span data-ttu-id="68d90-190">Partner Center till Dynamics 365 (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="68d90-190">Partner Center to Dynamics 365 (Insider Preview)</span></span>
- <span data-ttu-id="68d90-191">Dynamics 365 till Partner Center (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="68d90-191">Dynamics 365 to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="68d90-192">Dynamics 365-möjlighet till Partner Center (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="68d90-192">Dynamics 365 Opportunity to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="68d90-193">Dynamics 365 Microsoft-lösningar till Partner Center (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="68d90-193">Dynamics 365 Microsoft Solutions to Partner Center (Insider Preview)</span></span>
 

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a><span data-ttu-id="68d90-194">Använda webhook-API: er för att registrera för resurs ändrings händelser</span><span class="sxs-lookup"><span data-stu-id="68d90-194">Use Webhook APIs to register for resource change events</span></span>

<span data-ttu-id="68d90-195">Med API: er för webhook i Partner Center kan du registrera för resurs ändrings händelser.</span><span class="sxs-lookup"><span data-stu-id="68d90-195">The Partner Center Webhook APIs allow you to register for resource change events.</span></span> <span data-ttu-id="68d90-196">De här ändrings händelserna skickas till din URL som HTTP-inlägg.</span><span class="sxs-lookup"><span data-stu-id="68d90-196">These change events are sent to your url as HTTP posts.</span></span>

1. <span data-ttu-id="68d90-197">Registrera din URL genom att välja **partner Center webhook Registration (Insider Preview)** energi automatisera flöde.</span><span class="sxs-lookup"><span data-stu-id="68d90-197">To register your url, select **Partner Center Webhook Registration (Insider Preview)** Power Automate flow.</span></span>

2. <span data-ttu-id="68d90-198">Lägg till anslutningar för (a.) partner Center användare med referenser admin-autentiseringsuppgifter (b.) partner Center-händelser som marker ATS nedan</span><span class="sxs-lookup"><span data-stu-id="68d90-198">Add connections for (a.) Partner Center user with referrals admin credentials (b.) Partner Center Events as highlighted below</span></span>

   :::image type="content" source="images/cosellconnectors/triggerflow.png" alt-text="Utlösare":::

3. <span data-ttu-id="68d90-200">När du gör dessa uppdateringar visas</span><span class="sxs-lookup"><span data-stu-id="68d90-200">When you make these updates, you'll see</span></span>

   :::image type="content" source="images/cosellconnectors/webhook1.png" alt-text="Webhooks":::

4. <span data-ttu-id="68d90-202">Spara ändringarna och välj **Aktivera**.</span><span class="sxs-lookup"><span data-stu-id="68d90-202">Save your changes and select **Turn on**.</span></span>

   <span data-ttu-id="68d90-203">Gör så här om du vill aktivera att Webhooks i Partner Center ska lyssna på händelse ändringar:</span><span class="sxs-lookup"><span data-stu-id="68d90-203">To enable Partner Center webhooks to listen to event changes, do the following steps:</span></span>

5. <span data-ttu-id="68d90-204">Välj **partner Center till Dynamics 365 (Insider Preview)**.</span><span class="sxs-lookup"><span data-stu-id="68d90-204">Select **Partner Center to Dynamics 365 (Insider Preview)**.</span></span>

6. <span data-ttu-id="68d90-205">Välj **redigerings** ikonen och välj **när en http-begäran tas emot**.</span><span class="sxs-lookup"><span data-stu-id="68d90-205">Select the **Edit** icon and select **When a HTTP request is received**.</span></span>

7. <span data-ttu-id="68d90-206">Välj **kopierings** ikonen för att kopiera den tillhandahållna HTTP post-URL: en.</span><span class="sxs-lookup"><span data-stu-id="68d90-206">Select the **Copy** icon to copy the provided HTTP POST URL.</span></span>

   :::image type="content" source="images/cosellconnectors/copyurl.png" alt-text="Kopiera URL":::

8. <span data-ttu-id="68d90-208">Välj nu "partner för webhook-registrering (Insider Preview)" i Power Center och välj **Kör**.</span><span class="sxs-lookup"><span data-stu-id="68d90-208">Now select the “Partner Center Webhook Registration (Insider Preview)” Power Automate flow and select **Run**.</span></span>

9. <span data-ttu-id="68d90-209">Se till att fönstret kör flöde visas i den högra rutan och klicka på **Fortsätt**.</span><span class="sxs-lookup"><span data-stu-id="68d90-209">Ensure that the “Run Flow” window opens on the right-hand pane and click **Continue**.</span></span>

10. <span data-ttu-id="68d90-210">Ange följande uppgifter:</span><span class="sxs-lookup"><span data-stu-id="68d90-210">Enter the following details:</span></span>

    1. <span data-ttu-id="68d90-211">**Http-utlösare slut punkt**: URL kopierad från föregående steg</span><span class="sxs-lookup"><span data-stu-id="68d90-211">**Http Trigger Endpoint**: URL copied from earlier step</span></span>

    2. <span data-ttu-id="68d90-212">**Händelser att registrera**: "referral-created" och "referral-updated"</span><span class="sxs-lookup"><span data-stu-id="68d90-212">**Events to Register**: “referral-created” and “referral-updated”</span></span>

    3. <span data-ttu-id="68d90-213">**Skriv över befintliga utlösare slut punkter om det finns**: Ja (detta skriver över alla befintliga slut punkter.)</span><span class="sxs-lookup"><span data-stu-id="68d90-213">**Overwrite existing trigger endpoints if present**: Yes (This overwrites any existing endpoints.)</span></span>

11. <span data-ttu-id="68d90-214">Välj **Kör** och välj sedan **Slutför.**</span><span class="sxs-lookup"><span data-stu-id="68d90-214">Select **Run** and then select **Done.**</span></span>

<span data-ttu-id="68d90-215">Webhooken kan nu lyssna på att skapa och uppdatera händelser.</span><span class="sxs-lookup"><span data-stu-id="68d90-215">The webhook can now listen to create and update events.</span></span>

## <a name="customize-synchronization-steps"></a><span data-ttu-id="68d90-216">Anpassa synkroniserings steg</span><span class="sxs-lookup"><span data-stu-id="68d90-216">Customize synchronization steps</span></span>

<span data-ttu-id="68d90-217">När samförsäljnings hänvisningar synkroniseras mellan partner Center och ditt CRM-system, visas fälten som synkroniseras på Partner Center-datorn här.</span><span class="sxs-lookup"><span data-stu-id="68d90-217">When Co-sell referrals are synced between Partner Center and your CRM system, the fields that are synced on Partner Center PC are listed here.</span></span>

<span data-ttu-id="68d90-218">CRM-system är ofta anpassade.</span><span class="sxs-lookup"><span data-stu-id="68d90-218">Often CRM systems are highly customized.</span></span> <span data-ttu-id="68d90-219">Du kan anpassa automatiserade energi flöden.</span><span class="sxs-lookup"><span data-stu-id="68d90-219">You can customize the Power Automate flows.</span></span> <span data-ttu-id="68d90-220">Följ guiden för fält mappning och om det behövs kan du göra lämpliga ändringar i stegen i de automatiserade energi flödena.</span><span class="sxs-lookup"><span data-stu-id="68d90-220">Follow the field mapping guide, and if necessary, make appropriate changes in the steps of the Power Automate flows.</span></span>  <span data-ttu-id="68d90-221">Microsoft Partner Center till CRM-mappningar tillhandahålls, men baserat på din CRM-miljö kan du välja att ytterligare anpassa fälten.</span><span class="sxs-lookup"><span data-stu-id="68d90-221">Microsoft Partner Centers to CRM mappings are provided, but based on your CRM environment, you can choose to further customize the fields.</span></span>

<span data-ttu-id="68d90-222">Flera steg i vart och ett av de automatiserade energi flödena kan anpassas efter dina behov.</span><span class="sxs-lookup"><span data-stu-id="68d90-222">Multiple steps of each of the Power Automate flows can be customized based on your needs.</span></span> <span data-ttu-id="68d90-223">Följande är exempel på tillgängliga anpassningar:</span><span class="sxs-lookup"><span data-stu-id="68d90-223">The following are examples of available customizations:</span></span>

1. <span data-ttu-id="68d90-224">Så här anpassar du fälten för Create-eller Update-händelserna i Partner Center till CRM referral Synchronization:</span><span class="sxs-lookup"><span data-stu-id="68d90-224">To customize the fields for the create or update events in the Partner Center to CRM referral synchronization:</span></span> 

    <span data-ttu-id="68d90-225">a.</span><span class="sxs-lookup"><span data-stu-id="68d90-225">a.</span></span> <span data-ttu-id="68d90-226">Välj Partner Center till Dynamics 365 (Insider Preview) eller partner Center till Salesforce (Insider Preview).</span><span class="sxs-lookup"><span data-stu-id="68d90-226">Select Partner Center to Dynamics 365 (Insider Preview) or Partner Center to Salesforce (Insider Preview).</span></span>

    <span data-ttu-id="68d90-227">b.</span><span class="sxs-lookup"><span data-stu-id="68d90-227">b.</span></span> <span data-ttu-id="68d90-228">Välj **Redigera** för att redigera/anpassa det energi automatiserade flödet.</span><span class="sxs-lookup"><span data-stu-id="68d90-228">Select **Edit** to edit/customize the Power Automate flow.</span></span>

    <span data-ttu-id="68d90-229">c.</span><span class="sxs-lookup"><span data-stu-id="68d90-229">c.</span></span> <span data-ttu-id="68d90-230">Välj **(omfång) synkronisera lead eller affärs möjlighet**.</span><span class="sxs-lookup"><span data-stu-id="68d90-230">Select **(Scope) Synchronize the lead or opportunity**.</span></span>

2. <span data-ttu-id="68d90-231">Om du vill anpassa fält mappningar för CRM (baserat på fält mappnings guide) för skapa händelser väljer du **om den är ny delad affärs möjlighet och sedan**.</span><span class="sxs-lookup"><span data-stu-id="68d90-231">To customize CRM field mappings (based on field mappings guide) for create events, select **If it’s new Shared opportunity, then**.</span></span> <span data-ttu-id="68d90-232">Välj under steget **om ja** och expandera sedan **skapa en ny affärs möjlighet i CRM**.</span><span class="sxs-lookup"><span data-stu-id="68d90-232">Select the substep **if yes** and then expand **Creating a new opportunity in the CRM**.</span></span> <span data-ttu-id="68d90-233">Du kan redigera mappningarna i det här avsnittet med hjälp av fält mappnings guiden.</span><span class="sxs-lookup"><span data-stu-id="68d90-233">You can edit the mappings in this section using the Field Mapping Guide.</span></span>

    <span data-ttu-id="68d90-234">d.</span><span class="sxs-lookup"><span data-stu-id="68d90-234">d.</span></span> <span data-ttu-id="68d90-235">För att anpassa fält mappningar för CRM (baserat på fält mappnings guide) för uppdaterings händelser, klicka på steget "(omfattning) synkronisera lead eller affärs möjlighet".</span><span class="sxs-lookup"><span data-stu-id="68d90-235">For customizing CRM field mappings (based on field mappings guide) for update events, click on the step “(Scope) Synchronize the lead or opportunity”.</span></span>

    <span data-ttu-id="68d90-236">e.</span><span class="sxs-lookup"><span data-stu-id="68d90-236">e.</span></span> <span data-ttu-id="68d90-237">Välj **om det är en uppdatering av en affärs möjlighet och sedan**.</span><span class="sxs-lookup"><span data-stu-id="68d90-237">Select **If it’s an update to an opportunity, then**.</span></span> <span data-ttu-id="68d90-238">Välj under steget **om ja** och expandera sedan **differensen mellan affärs möjlighets objekt i Partner Center och CRM**.</span><span class="sxs-lookup"><span data-stu-id="68d90-238">Select the substep **if yes** and then expand **If difference between the opportunity objects in Partner Center and CRM, then**.</span></span>  

    <span data-ttu-id="68d90-239">f.</span><span class="sxs-lookup"><span data-stu-id="68d90-239">f.</span></span> <span data-ttu-id="68d90-240">Välj **om ja** följt av **Uppdatera befintlig affärs möjlighet**</span><span class="sxs-lookup"><span data-stu-id="68d90-240">Select **If yes** followed with **Update existing opportunity**</span></span>

3. <span data-ttu-id="68d90-241">Så här anpassar du fälten för CRM till PC referral-synkronisering för uppdaterings händelser:</span><span class="sxs-lookup"><span data-stu-id="68d90-241">To customize the fields for CRM to PC referral synchronization for update events:</span></span>

    <span data-ttu-id="68d90-242">a.</span><span class="sxs-lookup"><span data-stu-id="68d90-242">a.</span></span> <span data-ttu-id="68d90-243">Välj **Redigera**  för att redigera/anpassa det energi automatiserade flödet.</span><span class="sxs-lookup"><span data-stu-id="68d90-243">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

    <span data-ttu-id="68d90-244">b.</span><span class="sxs-lookup"><span data-stu-id="68d90-244">b.</span></span> <span data-ttu-id="68d90-245">Välj **(omfång) synkronisera affärs möjligheten**.</span><span class="sxs-lookup"><span data-stu-id="68d90-245">Select **(Scope) Synchronize the opportunity**.</span></span>

    <span data-ttu-id="68d90-246">c.</span><span class="sxs-lookup"><span data-stu-id="68d90-246">c.</span></span> <span data-ttu-id="68d90-247">Om du vill anpassa fält mappningar för CRM för uppdaterings händelser väljer du **om det finns skillnader mellan lead-objekten i Partner Center och CRM**.</span><span class="sxs-lookup"><span data-stu-id="68d90-247">To customize CRM field mappings for update events, select **If there is difference between the lead objects in Partner Center and CRM, then**.</span></span> 

    <span data-ttu-id="68d90-248">d.</span><span class="sxs-lookup"><span data-stu-id="68d90-248">d.</span></span> <span data-ttu-id="68d90-249">Välj under steget **om ja** och expandera sedan steget **Uppdatera en referens med affärs möjlighets data**.</span><span class="sxs-lookup"><span data-stu-id="68d90-249">Select the sub-step **if yes** and then expand the step **Update a referral with opportunity data**.</span></span>

   <span data-ttu-id="68d90-250">Du kan redigera mappningarna i det här avsnittet baserat på fält mappnings guiden.</span><span class="sxs-lookup"><span data-stu-id="68d90-250">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

4. <span data-ttu-id="68d90-251">Vill du anpassa fälten för synkronisering av CRM till PC-hänvisning för Create Events?</span><span class="sxs-lookup"><span data-stu-id="68d90-251">To customize the fields for CRM to PC referral synchronization for create events?</span></span>

   <span data-ttu-id="68d90-252">a.</span><span class="sxs-lookup"><span data-stu-id="68d90-252">a.</span></span> <span data-ttu-id="68d90-253">Välj **Redigera**  för att redigera/anpassa det energi automatiserade flödet.</span><span class="sxs-lookup"><span data-stu-id="68d90-253">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   <span data-ttu-id="68d90-254">b.</span><span class="sxs-lookup"><span data-stu-id="68d90-254">b.</span></span> <span data-ttu-id="68d90-255">Välj **(omfång)-synkronisering av referenser.**</span><span class="sxs-lookup"><span data-stu-id="68d90-255">Select **(Scope) Synchronizing Referrals.**</span></span>

   <span data-ttu-id="68d90-256">c.</span><span class="sxs-lookup"><span data-stu-id="68d90-256">c.</span></span> <span data-ttu-id="68d90-257">För att anpassa fält mappningar för CRM (baserat på fält mappnings guide) för skapa händelser väljer du **skapa Microsoft referral**.</span><span class="sxs-lookup"><span data-stu-id="68d90-257">For customizing CRM field mappings (based on field mappings guide) for create events, select **Create Microsoft Referral**.</span></span>

   <span data-ttu-id="68d90-258">Du kan redigera mappningarna i det här avsnittet baserat på fält mappnings guiden.</span><span class="sxs-lookup"><span data-stu-id="68d90-258">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

<span data-ttu-id="68d90-259">Två miljövariabler har skapats:</span><span class="sxs-lookup"><span data-stu-id="68d90-259">There are two environment variables created:</span></span>

- <span data-ttu-id="68d90-260">Bock: anger om du behöver en bock ikon förutom affärs möjligheter som synkroniseras i bi-riktning mellan partner Center och Dynamics 365 CRM.</span><span class="sxs-lookup"><span data-stu-id="68d90-260">Checkmark: Signifies whether you would need a checkmark icon besides opportunities that are synchronized bi-directionally between Partner Center and Dynamics 365 CRM.</span></span>

- <span data-ttu-id="68d90-261">Synkronisera samförsäljnings möjligheter endast: anger om du bara vill synkronisera samförsäljnings möjligheter.</span><span class="sxs-lookup"><span data-stu-id="68d90-261">Sync co-sell opportunities only: Signifies whether you want to synchronize only Co-sell opportunities.</span></span>

<span data-ttu-id="68d90-262">Du kan välja att redigera standardvärdet för miljövariablerna.</span><span class="sxs-lookup"><span data-stu-id="68d90-262">You can choose to edit the default value for the environment variables.</span></span>

:::image type="content" source="images/cosellconnectors/dynamics5.png" alt-text="Redigerings ruta för standardvärden":::

## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a><span data-ttu-id="68d90-264">Slutförd dubbelriktad referens synkronisering från slut punkt till slut punkt</span><span class="sxs-lookup"><span data-stu-id="68d90-264">End-to-end bi-directional co-sell referral synchronization</span></span>

<span data-ttu-id="68d90-265">När du har installerat, konfigurerat och anpassat den automatiserade lösningen för Energis par kan du testa synkroniseringen av samförsäljnings referenser mellan Dynamics 365 och partner Center.</span><span class="sxs-lookup"><span data-stu-id="68d90-265">Once you have installed, configured, and customized the Power Automate solution, you can test for Co-sell referrals synchronization between Dynamics 365 and Partner Center.</span></span>

### <a name="pre-requisites"></a><span data-ttu-id="68d90-266">Förutsättningar</span><span class="sxs-lookup"><span data-stu-id="68d90-266">Pre-requisites</span></span>

<span data-ttu-id="68d90-267">Om du vill synkronisera hänvisningarna mellan partner Center och Dynamics 365 CRM, kan du med hjälp av den automatiserade lösningen tydligt avgränsa Microsoft-/regionsspecifika hänvisnings fält.</span><span class="sxs-lookup"><span data-stu-id="68d90-267">To synchronize the referrals across Partner Center and Dynamics 365 CRM, the Power Automate solution clearly demarcates Microsoft-specific referral fields.</span></span> <span data-ttu-id="68d90-268">Den här identifieringen ger dina säljare möjlighet att bestämma vilka hänvisningar de vill dela med Microsoft för samförsäljning.</span><span class="sxs-lookup"><span data-stu-id="68d90-268">This identification gives your seller teams  the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

<span data-ttu-id="68d90-269">En uppsättning anpassade fält är tillgänglig som en del av entiteten **affärs möjlighet** .</span><span class="sxs-lookup"><span data-stu-id="68d90-269">A set of custom fields is available as part of the **Opportunity** entity.</span></span> <span data-ttu-id="68d90-270">En administratörs användare i CRM måste skapa ett separat CRM-avsnitt med anpassade **affärs möjlighets** fält.</span><span class="sxs-lookup"><span data-stu-id="68d90-270">A CRM admin user will need to create a separate CRM section with the **Opportunity** custom fields.</span></span>

<span data-ttu-id="68d90-271">Följande anpassade fält ska ingå i CRM-avsnittet:</span><span class="sxs-lookup"><span data-stu-id="68d90-271">The following custom fields should be part of the CRM section:</span></span>

- <span data-ttu-id="68d90-272">**Synkronisera med partner Center**: om du vill synkronisera affärs möjligheten med Microsoft Partner Center</span><span class="sxs-lookup"><span data-stu-id="68d90-272">**Sync with Partner Center**: Whether to sync the opportunity with Microsoft Partner Center</span></span>

- <span data-ttu-id="68d90-273">**Hänvisnings-ID**: ett skrivskyddat ID-fält för Microsoft Partner Center-hänvisning</span><span class="sxs-lookup"><span data-stu-id="68d90-273">**Referral Identifier**: A read-only identifier field for Microsoft Partner Center referral</span></span>

- <span data-ttu-id="68d90-274">**Hänvisnings länk**: en skrivskyddad länk till hänvisningen i Microsoft Partner Center</span><span class="sxs-lookup"><span data-stu-id="68d90-274">**Referral Link**: A read-only link to the referral in Microsoft Partner Center</span></span>

- <span data-ttu-id="68d90-275">**Hur kan Microsoft hjälpa?**: hjälp krävs från Microsoft för hänvisning</span><span class="sxs-lookup"><span data-stu-id="68d90-275">**How can Microsoft help?**: Help required from Microsoft for the referral</span></span>

- <span data-ttu-id="68d90-276">**Produkter**: lista över produkter som är kopplade till den här affärs möjligheten</span><span class="sxs-lookup"><span data-stu-id="68d90-276">**Products**: List of products associated with this opportunity</span></span>

- <span data-ttu-id="68d90-277">**Granskning**: en skrivskyddad Gransknings logg för synkronisering med partner Center-hänvisningar</span><span class="sxs-lookup"><span data-stu-id="68d90-277">**Audit**: A read-only audit trail for syncing with Partner Center referrals</span></span>

<span data-ttu-id="68d90-278">Uppdatera affärs möjlighets formuläret i Dynamics 365 CRM för att ta med lösningar för fältet produkter.</span><span class="sxs-lookup"><span data-stu-id="68d90-278">Update the opportunity form in Dynamics 365 CRM to include Solutions for Products field.</span></span>

:::image type="content" source="images/cosellconnectors/dynamics6.png" alt-text="Affärs möjlighets formulär":::

:::image type="content" source="images/cosellconnectors/dynamics7.png" alt-text="{alt-text}":::

### <a name="scenarios"></a><span data-ttu-id="68d90-281">OLIKA</span><span class="sxs-lookup"><span data-stu-id="68d90-281">SCENARIOS:</span></span>

1. <span data-ttu-id="68d90-282">Hänvisnings-synkronisering när hänvisning skapas eller uppdateras i CRM och synkroniseras i Partner Center:</span><span class="sxs-lookup"><span data-stu-id="68d90-282">Referral synchronization when referral is created or updated in CRM and synced in Partner Center:</span></span>

   1. <span data-ttu-id="68d90-283">Logga in på din Dynamics 365 CRM-miljö med användare som har synlighet i avsnittet **affärs möjlighet** i CRM.</span><span class="sxs-lookup"><span data-stu-id="68d90-283">Sign into your Dynamics 365 CRM environment with user who has visibility in the **Opportunity** section of the CRM.</span></span>

   2. <span data-ttu-id="68d90-284">Se till att följande avsnitt finns när du skapar en "ny affärs möjlighet" i Dynamics 365-miljön</span><span class="sxs-lookup"><span data-stu-id="68d90-284">Ensure that the following section is present when you create a “New Opportunity” in Dynamics 365 environment</span></span>

      :::image type="content" source="images/cosellconnectors/opportunity.png" alt-text="Avsnittet exempel på möjlighet som visar information om Microsoft Partner Center i Dynamics 365.":::

   3. <span data-ttu-id="68d90-286">För att synkronisera den här affärs möjligheten med Microsoft Partner Center, se till att du anger följande fält i kort vyn:</span><span class="sxs-lookup"><span data-stu-id="68d90-286">To synchronize this opportunity with Microsoft Partner Center, ensure that you set the following fields in the card view:</span></span>

      - <span data-ttu-id="68d90-287">**Synkronisera med partner Center**: Ja</span><span class="sxs-lookup"><span data-stu-id="68d90-287">**Sync with Partner Center**: Yes</span></span>

      - <span data-ttu-id="68d90-288">**Hur kan Microsoft hjälpa?**: Välj bland följande:</span><span class="sxs-lookup"><span data-stu-id="68d90-288">**How can Microsoft help?**: Select from the following:</span></span>

         :::image type="content" source="images/cosellconnectors/help.png" alt-text="Avsnittet exempel på en affärs möjlighet i Dynamics 365 som visar hjälp alternativ för Microsoft Partner Center bredvid ett fält som kallas hur kan Microsoft hjälpa dig?":::

      - <span data-ttu-id="68d90-290">**Produkter**: lösnings-ID för produkten</span><span class="sxs-lookup"><span data-stu-id="68d90-290">**Products**: Solution IDs of the product</span></span>

   4. <span data-ttu-id="68d90-291">När affärs möjligheten har skapats i Dynamics 365 med alternativet **Synkronisera med partner Center** inställt på **Ja**, vänta 10 minuter och logga sedan in på ditt partner Center-konto.</span><span class="sxs-lookup"><span data-stu-id="68d90-291">Once the opportunity is created in Dynamics 365 with **Sync with Partner Center** option set to **Yes**, wait 10 minutes, and then sign into your Partner Center account.</span></span> <span data-ttu-id="68d90-292">Dina referenser kommer att synkroniseras med Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="68d90-292">Your referrals will be synchronized with Dynamics 365.</span></span>

   5. <span data-ttu-id="68d90-293">För en affärs möjlighet som har alternativet "synkronisera med partner Center" inställt på "Ja", om du uppdaterar affärs möjligheten i Dynamics 365 CRM, kommer ändringarna att synkroniseras i ditt partner Center-konto.</span><span class="sxs-lookup"><span data-stu-id="68d90-293">Likewise, for an opportunity that had “Sync with Partner Center” option set to “Yes”, if you update the opportunity in Dynamics 365 CRM, the changes will be synchronized in your Partner Center account.</span></span>

   6. <span data-ttu-id="68d90-294">Möjligheter som har synkroniserats med partner Center identifieras med ✔-ikonen i Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="68d90-294">Opportunities that are synchronized successfully with Partner Center will be identified with ✔icon in Dynamics 365.</span></span>

2. <span data-ttu-id="68d90-295">Hänvisnings-synkronisering när hänvisning skapas eller uppdateras i Microsoft Partner Center och synkroniseras i Dynamics 365-miljön:</span><span class="sxs-lookup"><span data-stu-id="68d90-295">Referral Synchronization when referral is created or updated in Microsoft Partner Center and synchronized in Dynamics 365 environment:</span></span>

   1. <span data-ttu-id="68d90-296">Logga in på [instrument panelen](https://partner.microsoft.com/dashboard/home)för partner Center.</span><span class="sxs-lookup"><span data-stu-id="68d90-296">Sign into your Partner Center [dashboard](https://partner.microsoft.com/dashboard/home).</span></span>

   2. <span data-ttu-id="68d90-297">Välj **referenser** på menyn till vänster.</span><span class="sxs-lookup"><span data-stu-id="68d90-297">Select **Referrals** from the left-hand menu.</span></span>

   3. <span data-ttu-id="68d90-298">Skapa en ny samförsäljnings hänvisning från Partner Center genom att klicka på alternativet "nytt erbjudande".</span><span class="sxs-lookup"><span data-stu-id="68d90-298">Create a new Co-sell referral from Partner Center by clicking “New deal” option.</span></span>

   4. <span data-ttu-id="68d90-299">Logga in på din Dynamics 365 CRM-miljö.</span><span class="sxs-lookup"><span data-stu-id="68d90-299">Sign into your Dynamics 365 CRM environment.</span></span>

   5. <span data-ttu-id="68d90-300">Navigera till **Öppna affärs möjligheter**.</span><span class="sxs-lookup"><span data-stu-id="68d90-300">Navigate to **Open Opportunities**.</span></span> <span data-ttu-id="68d90-301">Den hänvisning som skapats i Microsoft Partner Center synkroniseras nu i Dynamics 365 CRM.</span><span class="sxs-lookup"><span data-stu-id="68d90-301">The referral created in Microsoft Partner Center is now synchronized in Dynamics 365 CRM.</span></span>

   6. <span data-ttu-id="68d90-302">När du väljer en synkroniserad referens fylls kort visnings informationen i.</span><span class="sxs-lookup"><span data-stu-id="68d90-302">When you select a synchronized referral, the card view details are populated.</span></span>

## <a name="next-steps"></a><span data-ttu-id="68d90-303">Nästa steg</span><span class="sxs-lookup"><span data-stu-id="68d90-303">Next steps</span></span>

- [<span data-ttu-id="68d90-304">Hantera leads</span><span class="sxs-lookup"><span data-stu-id="68d90-304">Manage leads</span></span>](manage-leads.md)

- [<span data-ttu-id="68d90-305">Hantera möjligheter till samförsäljning</span><span class="sxs-lookup"><span data-stu-id="68d90-305">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)

- [<span data-ttu-id="68d90-306">Mer om Microsoft Power Automated-plattform?</span><span class="sxs-lookup"><span data-stu-id="68d90-306">More about Microsoft Power Automate platform?</span></span>](/power-automate/)

- [<span data-ttu-id="68d90-307">Webhooks för partner Center</span><span class="sxs-lookup"><span data-stu-id="68d90-307">Partner Center webhooks</span></span>](/partner-center/develop/partner-center-webhooks)