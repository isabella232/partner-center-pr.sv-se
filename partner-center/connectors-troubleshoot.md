---
title: Felsöka anslutningsappar för hänvisningar till säljförsäljning
ms.topic: how-to
ms.date: 09/21/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Få svar på vanliga frågor om hur du använder anslutningsappar för säljförsäljning. Läs dessa vanliga frågor och svar om hur du felsöker anslutningsappar för säljförsäljning.
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: 939654202a370f6d9ba15d9e62a11be44884b613
ms.sourcegitcommit: 1899307642f057070b1bdd647594fc46ba61fb08
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/30/2021
ms.locfileid: "108284221"
---
# <a name="troubleshoot-co-sell-referrals-connectors"></a><span data-ttu-id="7523d-104">Felsöka anslutningsappar för hänvisningar till säljförsäljning</span><span class="sxs-lookup"><span data-stu-id="7523d-104">Troubleshoot co-sell referrals connectors</span></span>

<span data-ttu-id="7523d-105">**Gäller för**</span><span class="sxs-lookup"><span data-stu-id="7523d-105">**Applies to**</span></span>

- <span data-ttu-id="7523d-106">Dynamics 365 CRM</span><span class="sxs-lookup"><span data-stu-id="7523d-106">Dynamics 365 CRM</span></span>
- <span data-ttu-id="7523d-107">Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="7523d-107">Salesforce CRM</span></span>

<span data-ttu-id="7523d-108">**Lämpliga roller**</span><span class="sxs-lookup"><span data-stu-id="7523d-108">**Appropriate roles**</span></span>

- <span data-ttu-id="7523d-109">Referensadministratör</span><span class="sxs-lookup"><span data-stu-id="7523d-109">Referrals admin</span></span>
- <span data-ttu-id="7523d-110">Systemadministratör eller systemanpassare för CRM</span><span class="sxs-lookup"><span data-stu-id="7523d-110">System admin or system customizer on the CRM</span></span>

 ## <a name="questions-and-answers-about-pre-requisites"></a><span data-ttu-id="7523d-111">Frågor och svar om förutsättningar</span><span class="sxs-lookup"><span data-stu-id="7523d-111">Questions and answers about pre-requisites</span></span>

1. <span data-ttu-id="7523d-112">Kan du använda en anslutningsapp för utvärderingsversionen av anslutningsappar för säljförsäljning för din miljö?</span><span class="sxs-lookup"><span data-stu-id="7523d-112">Can you use a trial co-sell referrals connectors solution for your environment?</span></span>

<span data-ttu-id="7523d-113">Om du använder test-/mellanlagringsmiljön kan du välja utvärderingslösning.</span><span class="sxs-lookup"><span data-stu-id="7523d-113">If you are on the test/staging environment, you can opt for trial solution.</span></span> <span data-ttu-id="7523d-114">Den betalda versionen av anslutningsapparna är tillgänglig i AppSource på US$ 15 per månad.</span><span class="sxs-lookup"><span data-stu-id="7523d-114">The paid version of the Connectors is available in AppSource at US$ 15/month.</span></span> <span data-ttu-id="7523d-115">Med den betalda anslutningen får du 10 000 API-anrop per dag.</span><span class="sxs-lookup"><span data-stu-id="7523d-115">With the paid connection, you will be getting 10K API calls per day.</span></span> <span data-ttu-id="7523d-116">Anslutningsapparna är omslutningar ovanpå Partner Center-hänvisnings-API:er.</span><span class="sxs-lookup"><span data-stu-id="7523d-116">The Connectors are wrappers on top of Partner Center referral APIs.</span></span> <span data-ttu-id="7523d-117">När anslutningslösningarna körs för en **skapa-** eller **uppdateringshändelse** på antingen Partner Center- eller CRM-sidan görs ett API-anrop.</span><span class="sxs-lookup"><span data-stu-id="7523d-117">Whenever the connector solutions run for a **Create** or **Update** event on the opportunities on either Partner Center or the CRM side, an API call is made.</span></span>

2. <span data-ttu-id="7523d-118">Vilken roll behöver du för att skapa avsnitt i CRM-miljön?</span><span class="sxs-lookup"><span data-stu-id="7523d-118">What role do you need to create sections in CRM environment?</span></span>

<span data-ttu-id="7523d-119">Användare som är systemadministratörer eller systemanpassare kan tillämpa ändringar för alla.</span><span class="sxs-lookup"><span data-stu-id="7523d-119">Users who are system admins or system customizers can apply changes for everyone.</span></span> <span data-ttu-id="7523d-120">Alla appanvändare kan dock anpassa systemet och även dela vissa av sina anpassningar med andra.</span><span class="sxs-lookup"><span data-stu-id="7523d-120">All app users, however,  can personalize the system and even share some of their customizations with others.</span></span> 

3. <span data-ttu-id="7523d-121">Behöver partnerförsäljare särskilda roller för att arbeta i Partnercenter?</span><span class="sxs-lookup"><span data-stu-id="7523d-121">Do partner sellers need special roles to work on Partner Center?</span></span>
 
<span data-ttu-id="7523d-122">Partner säljare måste tilldelas rollen referensadministratör.</span><span class="sxs-lookup"><span data-stu-id="7523d-122">Partner sellers must be assigned the “Referrals admin” role.</span></span> <span data-ttu-id="7523d-123">Mer information finns i Översikt [över behörigheter.](create-user-accounts-and-set-permissions.md)</span><span class="sxs-lookup"><span data-stu-id="7523d-123">For more information, see [Permissions overview](create-user-accounts-and-set-permissions.md).</span></span>

4. <span data-ttu-id="7523d-124">Vilka fält måste konfigureras först i din CRM-miljö?</span><span class="sxs-lookup"><span data-stu-id="7523d-124">What fields need to be set up first in your CRM environment?</span></span> 

<span data-ttu-id="7523d-125">• Kontrollera att din valuta är lämplig för din plats och att den är korrekt i DIN CRM-miljö.</span><span class="sxs-lookup"><span data-stu-id="7523d-125">• Make sure your currency is appropriate to your location and is in your CRM environment accurately.</span></span> <span data-ttu-id="7523d-126">• Säljteamet bör listas i din CRM-miljö som CRM-användare.</span><span class="sxs-lookup"><span data-stu-id="7523d-126">• Your sales team should be listed in your CRM environment as CRM users.</span></span>

5. <span data-ttu-id="7523d-127">Vilka förutsättningar krävs för att skapa Power Automate miljön?</span><span class="sxs-lookup"><span data-stu-id="7523d-127">What pre-requisites are required for Power Automate environment creation?</span></span>

<span data-ttu-id="7523d-128">Om du vill Power Automate en miljö behöver du:</span><span class="sxs-lookup"><span data-stu-id="7523d-128">To use the Power Automate environment, you need:</span></span>

- <span data-ttu-id="7523d-129">En Power Automate licens krävs.</span><span class="sxs-lookup"><span data-stu-id="7523d-129">A Power Automate license is required.</span></span>
- <span data-ttu-id="7523d-130">Minst 1 GB lagringsutrymme krävs.</span><span class="sxs-lookup"><span data-stu-id="7523d-130">A minimum of 1-GB storage is required.</span></span>

6.  <span data-ttu-id="7523d-131">Behöver du en Dynamics 365-prenumeration för att använda Salesforce Connectors-lösningen?</span><span class="sxs-lookup"><span data-stu-id="7523d-131">Do you need a Dynamics 365 subscription to use Salesforce Connectors solution?</span></span>

<span data-ttu-id="7523d-132">Salesforce Connector-lösningen är av typen "Dynamics Flow" som stöder synkronisering med andra CRM-system.</span><span class="sxs-lookup"><span data-stu-id="7523d-132">The Salesforce Connector solution is of type “Dynamics Flow” that supports synchronizing with other CRM systems.</span></span> <span data-ttu-id="7523d-133">Lösningen kräver inte att du har en Dynamics 365-instans eller en prenumeration.</span><span class="sxs-lookup"><span data-stu-id="7523d-133">The solution doesn’t require you to have a Dynamics 365 instance or a subscription.</span></span> <span data-ttu-id="7523d-134">När du installerar Salesforce-lösningen kan en listrutan med befintlig CDS-miljö i ditt företag visas.</span><span class="sxs-lookup"><span data-stu-id="7523d-134">While installing the Salesforce solution, a drop-down with existing CDS environment in your company may appear.</span></span> <span data-ttu-id="7523d-135">Du måste välja den miljön.</span><span class="sxs-lookup"><span data-stu-id="7523d-135">You need to select that environment.</span></span> <span data-ttu-id="7523d-136">Om du dessutom får felet "Det gick inte att hitta en Dynamics 365-organisation som är ansluten till den inloggade användaren" måste du skapa en ny miljö för anslutning.</span><span class="sxs-lookup"><span data-stu-id="7523d-136">In addition, if you get the error "We couldn't find a Dynamics 365 organization connected to signed-in user", then you will need to create new environment for connector.</span></span>

## <a name="questions-and-answers-about-configuration"></a><span data-ttu-id="7523d-137">Frågor och svar om konfiguration</span><span class="sxs-lookup"><span data-stu-id="7523d-137">Questions and answers about configuration</span></span>

1. <span data-ttu-id="7523d-138">Vad ska du göra om du får följande fel när du aktiverar flöden i Power Automate Platform?</span><span class="sxs-lookup"><span data-stu-id="7523d-138">What should you do if you face the following error while activating flows in Power Automate Platform?</span></span>

<span data-ttu-id="7523d-139">Fel: Begäran till Azure Resource Manager misslyckades med fel: "{"error":{"code":"WorkflowTriggerNotFound","message":"Arbetsflödet "e14d00f1-1fdf-4b1b-aaac-54a5064093d3" utlösaren "manual" kunde inte hittas."}}".</span><span class="sxs-lookup"><span data-stu-id="7523d-139">Error: Request to Azure Resource Manager failed with error: '{"error":{"code":"WorkflowTriggerNotFound","message":"The workflow 'e14d00f1-1fdf-4b1b-aaac-54a5064093d3' trigger 'manual' could not be found."}}'.</span></span> 

<span data-ttu-id="7523d-140">Följ dessa felsökningssteg:</span><span class="sxs-lookup"><span data-stu-id="7523d-140">Follow these troubleshooting steps:</span></span>

- <span data-ttu-id="7523d-141">Ta bort CDS-anslutningen och återskapa sedan CDS-anslutningarna.</span><span class="sxs-lookup"><span data-stu-id="7523d-141">Delete the CDS connection and then recreate the CDS connections.</span></span>
- <span data-ttu-id="7523d-142">Inaktivera och aktivera det underordnade flödet</span><span class="sxs-lookup"><span data-stu-id="7523d-142">Turn the child flow off and on</span></span> 
- <span data-ttu-id="7523d-143">Ta bort lösningen och installera sedan om lösningen.</span><span class="sxs-lookup"><span data-stu-id="7523d-143">Delete solution and then reinstall the solution.</span></span> 

2.  <span data-ttu-id="7523d-144">Vad ska du göra om du får felet "Logga in" när du lägger till en Partner Center-anslutning i Power Automate Platform?</span><span class="sxs-lookup"><span data-stu-id="7523d-144">What should you do if you face the "Sign in" error while adding a Partner Center connector in Power Automate Platform?</span></span>

:::image type="content" source="images/cosellconnectors/failure.png" alt-text="Felmeddelande som kräver inloggning":::

<span data-ttu-id="7523d-146">Följ det här felsökningssteget:</span><span class="sxs-lookup"><span data-stu-id="7523d-146">Follow this troubleshooting step:</span></span>

- <span data-ttu-id="7523d-147">Använd dina autentiseringsuppgifter för Partnercenter för att logga in i flödesmiljön en gång (flow.microsoft.com).</span><span class="sxs-lookup"><span data-stu-id="7523d-147">Use your Partner Center credentials to sign into the flow environment once (flow.microsoft.com).</span></span>


3. <span data-ttu-id="7523d-148">Vad ska du göra om du får följande fel när du aktiverar PartnerCenter till CRM-flödet i Power Automate Platform?</span><span class="sxs-lookup"><span data-stu-id="7523d-148">What should you do if you receive the following error while activating the Partner Center to CRM flow in Power Automate Platform?</span></span>
 
:::image type="content" source="images/cosellconnectors/powererror.png" alt-text="Felmeddelande som kräver uppdateringar":::

<span data-ttu-id="7523d-150">Följ dessa felsökningssteg:</span><span class="sxs-lookup"><span data-stu-id="7523d-150">Follow these troubleshooting steps:</span></span>

- <span data-ttu-id="7523d-151">Aktivera följande två underordnade flöden först innan du aktiverar Partnercenter till CRM-flödet.</span><span class="sxs-lookup"><span data-stu-id="7523d-151">Activate the following two child flows first before you activate the Partner Center to CRM flow.</span></span>
      - <span data-ttu-id="7523d-152">Partner Center till CRM – Helper (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="7523d-152">Partner Center to CRM - Helper (Insider Preview)</span></span>
      - <span data-ttu-id="7523d-153">Partner Center Microsoft Co-sell Referral Updates to CRM (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="7523d-153">Partner Center Microsoft Co-sell Referral Updates to CRM (Insider Preview)</span></span>

4. <span data-ttu-id="7523d-154">Vad ska du göra när du inte kan lägga till anslutningar till flödet när du försöker redigera flödet?</span><span class="sxs-lookup"><span data-stu-id="7523d-154">What should you do when you aren't able to add connections to the flow when you try to edit the flow?</span></span>

<span data-ttu-id="7523d-155">Du lägger till anslutningar till flödet medan flödet körs och lägger till i varje flöde separat.</span><span class="sxs-lookup"><span data-stu-id="7523d-155">You add connections to the flow while the flow is running, and you add to each flow separately.</span></span>  <span data-ttu-id="7523d-156">Om dialogrutan för att lägga till anslutningar inte öppnas automatiskt när du redigerar flödet kan du redigera vart och ett av stegen och understegen för flödena individuellt.</span><span class="sxs-lookup"><span data-stu-id="7523d-156">If the dialog to add connections doesn't open up automatically while editing the flow, then you can edit each of the steps and sub steps of the flows individually.</span></span>

- <span data-ttu-id="7523d-157">Markera varje flöde och redigera dem individuellt.</span><span class="sxs-lookup"><span data-stu-id="7523d-157">Select each flow and edit them individually.</span></span>
- <span data-ttu-id="7523d-158">Expandera alla steg i flödet</span><span class="sxs-lookup"><span data-stu-id="7523d-158">Expand all the steps in the flow</span></span> 

:::image type="content" source="images/cosellconnectors/flowsteps.png" alt-text="Steg som behöver anslutningar":::

- <span data-ttu-id="7523d-160">Välj de steg där du ser en varningsikon där du uppmanas att associera anslutningar och lägga till anslutningar.</span><span class="sxs-lookup"><span data-stu-id="7523d-160">Select the steps where you see a warning icon asking to associate connections, and add connections.</span></span> 

:::image type="content" source="images/cosellconnectors/editflow.png" alt-text="Redigera flödet steg för steg":::


5. <span data-ttu-id="7523d-162">Vad ska du göra om flödena i lösningen för anslutningsappar för säljförsäljning inte är på?</span><span class="sxs-lookup"><span data-stu-id="7523d-162">What should you do if the flows of the Co-sell Referrals Connectors solution don’t turn on?</span></span>

<span data-ttu-id="7523d-163">A.</span><span class="sxs-lookup"><span data-stu-id="7523d-163">A.</span></span> <span data-ttu-id="7523d-164">I Power Automate måste du redigera flöden i följande ordning och uppdatera dem så att de använder rätt anslutningar:</span><span class="sxs-lookup"><span data-stu-id="7523d-164">In Power Automate, you'll need to edit flows in the following order and update them to use the correct connections:</span></span>

- <span data-ttu-id="7523d-165">Partner Center Webhook Registration (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="7523d-165">Partner Center Webhook Registration (Insider Preview)</span></span>
- <span data-ttu-id="7523d-166">Skapa hänvisning till säljpartner – Salesforce till Partner Center (insiderförhandsvisning)</span><span class="sxs-lookup"><span data-stu-id="7523d-166">Create Co-sell Referral - Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="7523d-167">Partner center Microsoft co-sell hänvisningsuppdateringar till Salesforce (insiderförhandsvisning)</span><span class="sxs-lookup"><span data-stu-id="7523d-167">Partner Center Microsoft Co-sell Referral Updates to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="7523d-168">Partner center till Salesforce (insiderförhandsvisning)</span><span class="sxs-lookup"><span data-stu-id="7523d-168">Partner Center to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="7523d-169">Salesforce till Partner Center (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="7523d-169">Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="7523d-170">Salesforce Opportunity to Partner Center (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="7523d-170">Salesforce Opportunity to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="7523d-171">Salesforce Microsoft Solutions to Partner Center (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="7523d-171">Salesforce Microsoft Solutions to Partner Center (Insider Preview)</span></span>

 <span data-ttu-id="7523d-172">B.</span><span class="sxs-lookup"><span data-stu-id="7523d-172">B.</span></span> <span data-ttu-id="7523d-173">För vart och ett av flödena **väljer du alternativet Kör endast** användare.</span><span class="sxs-lookup"><span data-stu-id="7523d-173">For each of flow, select **Run only users** option.</span></span> <span data-ttu-id="7523d-174">Välj **Använd anslutning i** stället för Tillhandahålls av den **körbaserade användaren**.</span><span class="sxs-lookup"><span data-stu-id="7523d-174">Select **Use connection** instead of **Provided by run-only user**.</span></span>  

:::image type="content" source="images/cosellconnectors/runonly.png" alt-text="Så här aktiverar du ett flöde":::


<span data-ttu-id="7523d-176">C.</span><span class="sxs-lookup"><span data-stu-id="7523d-176">C.</span></span> <span data-ttu-id="7523d-177">Aktivera dessa nedanstående flöden:</span><span class="sxs-lookup"><span data-stu-id="7523d-177">Activate these below mentioned flows:</span></span>

 - <span data-ttu-id="7523d-178">Partner center Microsoft co-sell hänvisningsuppdateringar till Salesforce (insiderförhandsvisning)</span><span class="sxs-lookup"><span data-stu-id="7523d-178">Partner Center Microsoft Co-sell Referral Updates to Salesforce (Insider Preview)</span></span>

- <span data-ttu-id="7523d-179">Salesforce till Partner Center (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="7523d-179">Salesforce to Partner Center (Insider Preview)</span></span>

    
<span data-ttu-id="7523d-180">D.</span><span class="sxs-lookup"><span data-stu-id="7523d-180">D.</span></span> <span data-ttu-id="7523d-181">Aktivera alla återstående flöden.</span><span class="sxs-lookup"><span data-stu-id="7523d-181">Activate all the remaining flows.</span></span>

<span data-ttu-id="7523d-182">E.</span><span class="sxs-lookup"><span data-stu-id="7523d-182">E.</span></span> <span data-ttu-id="7523d-183">Välj Kör i flödet Partner center Webhook Registration (Registrering av Partnercenter-webhook).</span><span class="sxs-lookup"><span data-stu-id="7523d-183">At flow Partner Center Webhook Registration, select **Run**.</span></span> <span data-ttu-id="7523d-184">Ange **HTTP-URL:en** från den första åtgärden **i Partnercenter till Salesforce-flödet.**</span><span class="sxs-lookup"><span data-stu-id="7523d-184">Provide the **http url** from the first action in **Partner Center to Salesforce** flow.</span></span> <span data-ttu-id="7523d-185">Välj alla fyra alternativen under **Händelser att registrera** och välj **Ja** för Overwrite (Skriva över).</span><span class="sxs-lookup"><span data-stu-id="7523d-185">Select all four options under **Events to register** and select **yes** for Overwrite.</span></span>

## <a name="questions-and-answers-about-runmaintenance"></a><span data-ttu-id="7523d-186">Frågor och svar om körning/underhåll</span><span class="sxs-lookup"><span data-stu-id="7523d-186">Questions and answers about Run/Maintenance</span></span>

1. <span data-ttu-id="7523d-187">Hur felsöker du fel Power Automate körningen av flödet?</span><span class="sxs-lookup"><span data-stu-id="7523d-187">How do you troubleshoot failures during Power Automate flow execution?</span></span>

<span data-ttu-id="7523d-188">Information om hur du Power Automate körs som förväntat och felsöker fel under körningen finns i Åtgärda [flödesfel.](/power-automate/fix-flow-failures)</span><span class="sxs-lookup"><span data-stu-id="7523d-188">To ensure that your Power Automate flows run as you expect and to troubleshoot failures during execution, refer to [Fix flow failures](/power-automate/fix-flow-failures).</span></span>

2. <span data-ttu-id="7523d-189">Vad ska du göra om du ser referenser som inte synkroniseras korrekt i Partner Center eller CRM-miljön?</span><span class="sxs-lookup"><span data-stu-id="7523d-189">What should you do if you see referrals that aren't synchronized properly in Partner Center or CRM environment?</span></span>
 
<span data-ttu-id="7523d-190">Välj Granska för att fastställa statusen för **referenssynkronisering.**</span><span class="sxs-lookup"><span data-stu-id="7523d-190">To determine the status of referral synchronization, select **Audit**.</span></span> 

:::image type="content" source="images/cosellconnectors/synch.png" alt-text="Så här synkroniserar du referenser":::

<span data-ttu-id="7523d-192">Kontrollera att följande villkor är uppfyllda:</span><span class="sxs-lookup"><span data-stu-id="7523d-192">Ensure that the following conditions are met:</span></span>

- <span data-ttu-id="7523d-193">Lösnings-ID anges som en del av affärsmöjligheten.</span><span class="sxs-lookup"><span data-stu-id="7523d-193">Solution ID is provided as part of the opportunity.</span></span>

- <span data-ttu-id="7523d-194">Landskod med två bokstäver krävs.</span><span class="sxs-lookup"><span data-stu-id="7523d-194">Two letter country code is required.</span></span>

- <span data-ttu-id="7523d-195">När hjälp från Microsoft har valts för affärsmöjligheten krävs kundens kontaktinformation.</span><span class="sxs-lookup"><span data-stu-id="7523d-195">When help from Microsoft is selected for the opportunity, customer contact information is required.</span></span>

3. <span data-ttu-id="7523d-196">Hur ser du till att en hänvisning synkroniseras i dubbelriktad riktning?</span><span class="sxs-lookup"><span data-stu-id="7523d-196">How to ensure that a referral will synchronize bi-directionally?</span></span>

<span data-ttu-id="7523d-197">Gör följande:</span><span class="sxs-lookup"><span data-stu-id="7523d-197">Do the following steps:</span></span>

- <span data-ttu-id="7523d-198">Partnerförsäljare måste se till att de har aktiverat alternativet **Synkronisera med Partnercenter** i CRM-avsnittet.</span><span class="sxs-lookup"><span data-stu-id="7523d-198">Partner sellers need to ensure that they have enabled **Sync with Partner Center** option in the CRM section.</span></span>

:::image type="content" source="images/cosellconnectors/enablesynch.png" alt-text="Kontrollera att du har aktiverat Synch":::

- <span data-ttu-id="7523d-200">Säljare måste ange intäkter och slutdatum när de kvalificerar en lead.</span><span class="sxs-lookup"><span data-stu-id="7523d-200">Sellers need to provide revenue and closing date when qualifying a lead.</span></span>

- <span data-ttu-id="7523d-201">Om CRM-ID anges  i  fasen skapa eller uppdatera samförsäljningsmöjlighet, men en lead-affärsmöjlighet med det ID:t inte hittas i CRM, ignoreras uppdatering eller skapa.</span><span class="sxs-lookup"><span data-stu-id="7523d-201">If CRM ID is provided in the **create** or **update** stage of co-sell opportunity, but a lead opportunity with that ID is not found in CRM, then update or create will be ignored.</span></span>

- <span data-ttu-id="7523d-202">Se till att hänvisningsvalutafältet har konfigurerats i Salesforce-miljön.</span><span class="sxs-lookup"><span data-stu-id="7523d-202">Ensure that referral currency field is configured on Salesforce environment.</span></span> 

4. <span data-ttu-id="7523d-203">Vad ska du göra om anslutningsappen kopplas från och du missar en hänvisningssynkronisering.?</span><span class="sxs-lookup"><span data-stu-id="7523d-203">What should you do if the connector gets disconnected and you miss a referral synchronization.?</span></span>

<span data-ttu-id="7523d-204">Följande är några av de alternativ som du kan prova:</span><span class="sxs-lookup"><span data-stu-id="7523d-204">Following are few of the options that you can try out:</span></span>

- <span data-ttu-id="7523d-205">Kontrollera om användarnamnet eller lösenordet har upphört att gälla för Partnercenter-användaren med referensadministratörsroller.</span><span class="sxs-lookup"><span data-stu-id="7523d-205">Check whether username or password has expired for the Partner Center user with referral admin roles.</span></span>

- <span data-ttu-id="7523d-206">Du kan gå till den icke-synkroniserade affärsmöjligheten, göra en mindre uppdatering och se om hänvisningen har synkroniserats.</span><span class="sxs-lookup"><span data-stu-id="7523d-206">You can go to the un-synchronized opportunity, make a minor update, and observe whether the referral has synchronized.</span></span>

- <span data-ttu-id="7523d-207">Om flödena har körts och misslyckats väljer du flödet och skickar om körningen som misslyckades.</span><span class="sxs-lookup"><span data-stu-id="7523d-207">If the flows have run and failed, then select the flow and re-submit the run that has failed.</span></span>

5. <span data-ttu-id="7523d-208">Vad ska du göra när du får felmeddelanden om nekad åtkomst?</span><span class="sxs-lookup"><span data-stu-id="7523d-208">What should you do when you get access denied errors?</span></span>

<span data-ttu-id="7523d-209">Kontrollera att rätt roller finns</span><span class="sxs-lookup"><span data-stu-id="7523d-209">Make sure the appropriate roles exist</span></span>

- <span data-ttu-id="7523d-210">Referensadministratörsroll för Partner Center-säljare</span><span class="sxs-lookup"><span data-stu-id="7523d-210">Referral Administrator role for Partner Center seller</span></span> 
 
- <span data-ttu-id="7523d-211">Rollen Systemadministratör eller Systemanpassare på din CRM-instans</span><span class="sxs-lookup"><span data-stu-id="7523d-211">System Administrator or System Customizer role on your CRM instance</span></span>

- <span data-ttu-id="7523d-212">Kontrollera att Power Automate flödeskontoanvändare loggar in https://flow.microsoft.com på minst en gång i förväg</span><span class="sxs-lookup"><span data-stu-id="7523d-212">Ensure that the Power Automate flow account user logs into https://flow.microsoft.com at least once beforehand</span></span>

6. <span data-ttu-id="7523d-213">Vad ska du göra **om du** ser att landskoden för kundkontot saknas när du skapar en möjlighet till säljförsäljning?</span><span class="sxs-lookup"><span data-stu-id="7523d-213">If you see that **Customer account country code** is missing while creating a Co-sell opportunity, what should you do?</span></span>

<span data-ttu-id="7523d-214">Du måste lägga till ISO-landskoden med två bokstäver till kundkontot i CRM.</span><span class="sxs-lookup"><span data-stu-id="7523d-214">You will need to add the ISO two-letter country code to the Customer account in CRM.</span></span>

7. <span data-ttu-id="7523d-215">Vad ska du göra om du ser felet att **lösnings-ID krävs när** du skapar en möjlighet till säljförsäljning?</span><span class="sxs-lookup"><span data-stu-id="7523d-215">What should you do if you see the error that **Solution ID is required** while creating a Co-sell opportunity?</span></span>

<span data-ttu-id="7523d-216">För att kunna skapa en hänvisning till säljförsäljning behöver du en lösning som är redo för Microsofts säljförsäljning.</span><span class="sxs-lookup"><span data-stu-id="7523d-216">In order to create a co-sell referral, you need a Microsoft co-sell ready solution.</span></span> 

8. <span data-ttu-id="7523d-217">Vad ska du göra när du ser möjligheter till säljförsäljning som skapats i Partnercenter och som inte synkroniseras med CRM trots att det inte finns några flödesfel?</span><span class="sxs-lookup"><span data-stu-id="7523d-217">What should you do when you see Co-sell opportunities created in Partner Center that aren't synchronized to CRM even though there are no flow errors?</span></span>

<span data-ttu-id="7523d-218">Gör följande:</span><span class="sxs-lookup"><span data-stu-id="7523d-218">Do the following:</span></span>

- <span data-ttu-id="7523d-219">När du har skapat ett nytt samförsäljningsavtal i Partnercenter kontrollerar du om Flödet Partnercenter till Dynamics 365 anropas (det kan anropas flera gånger).</span><span class="sxs-lookup"><span data-stu-id="7523d-219">After you have created a new co-sell deal in Partner Center, check if Partner Center to Dynamics 365 flow gets invoked (it might get invoked multiple times).</span></span>

- <span data-ttu-id="7523d-220">Om flödet anropas kontrollerar du alla anropade flöden och identifierar flödeskörningen som uppdaterar CRM.</span><span class="sxs-lookup"><span data-stu-id="7523d-220">If the flow gets invoked, check all invoked flows, and identify the flow run which that would update the CRM.</span></span> <span data-ttu-id="7523d-221">Du kan följa åtgärderna och kontrollera om CRM har uppdaterats eller om ett problem har uppstått.</span><span class="sxs-lookup"><span data-stu-id="7523d-221">You can follow the actions and verify if it did update the CRM or encountered a problem.</span></span>

- <span data-ttu-id="7523d-222">Markera **Nytt avtal i** Partnercenter för att se om det fylls med CRM-ID.</span><span class="sxs-lookup"><span data-stu-id="7523d-222">Check **New deal** in Partner Center to see if it gets populated with CRM ID.</span></span>

- <span data-ttu-id="7523d-223">Kontrollera att avtalet inte har stängts av misstag som **won (vunnits)** **eller Lost (förlorad)** i Partnercenter.</span><span class="sxs-lookup"><span data-stu-id="7523d-223">Make sure that the deal is not accidentally closed as **Won** or **Lost** in Partner Center.</span></span>

## <a name="next-steps"></a><span data-ttu-id="7523d-224">Nästa steg</span><span class="sxs-lookup"><span data-stu-id="7523d-224">Next steps</span></span>

- [<span data-ttu-id="7523d-225">Hantera leads</span><span class="sxs-lookup"><span data-stu-id="7523d-225">Manage leads</span></span>](manage-leads.md)
 
- [<span data-ttu-id="7523d-226">Hantera möjligheter till samförsäljning</span><span class="sxs-lookup"><span data-stu-id="7523d-226">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)
