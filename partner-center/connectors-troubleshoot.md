---
title: Felsöka samsäljande referral-kopplingar
ms.topic: how-to
ms.date: 09/21/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Lär dig svar på vanliga frågor om att använda samförsäljnings anslutningar. Läs vanliga frågor och svar om hur du felsöker samförsäljnings anslutningar.
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: 988a696a8a0a0abb4d37e3915c76f905ec5b35b0
ms.sourcegitcommit: a8adb5f044f06bd684a5b7a06c8efe9f8b03d2db
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 10/14/2020
ms.locfileid: "92531889"
---
# <a name="troubleshoot-co-sell-referrals-connectors"></a><span data-ttu-id="385b5-104">Felsöka samsäljande referral-kopplingar</span><span class="sxs-lookup"><span data-stu-id="385b5-104">Troubleshoot co-sell referrals connectors</span></span>

<span data-ttu-id="385b5-105">**Gäller för:**</span><span class="sxs-lookup"><span data-stu-id="385b5-105">**Applies to:**</span></span>

- <span data-ttu-id="385b5-106">Partnercenter</span><span class="sxs-lookup"><span data-stu-id="385b5-106">Partner Center</span></span>
- <span data-ttu-id="385b5-107">Dynamics 365 CRM</span><span class="sxs-lookup"><span data-stu-id="385b5-107">Dynamics 365 CRM</span></span>
- <span data-ttu-id="385b5-108">Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="385b5-108">Salesforce CRM</span></span>

<span data-ttu-id="385b5-109">**Lämpliga roller**</span><span class="sxs-lookup"><span data-stu-id="385b5-109">**Appropriate roles**</span></span>

- <span data-ttu-id="385b5-110">Referens administratör</span><span class="sxs-lookup"><span data-stu-id="385b5-110">Referrals admin</span></span>
- <span data-ttu-id="385b5-111">System administratör eller systemanpassare på CRM</span><span class="sxs-lookup"><span data-stu-id="385b5-111">System admin or system customizer on the CRM</span></span>

 ## <a name="questions-and-answers-about-pre-requisites"></a><span data-ttu-id="385b5-112">Frågor och svar om krav</span><span class="sxs-lookup"><span data-stu-id="385b5-112">Questions and answers about pre-requisites</span></span>

1. <span data-ttu-id="385b5-113">Kan du använda en lösning för att använda en utvärderings version av referral Connector för din miljö?</span><span class="sxs-lookup"><span data-stu-id="385b5-113">Can you use a trial co-sell referrals connectors solution for your environment?</span></span>

<span data-ttu-id="385b5-114">Om du är i test-/Staging-miljön kan du välja en utvärderings lösning.</span><span class="sxs-lookup"><span data-stu-id="385b5-114">If you are on the test/staging environment, you can opt for trial solution.</span></span> <span data-ttu-id="385b5-115">Den betalda versionen av kopplingarna är tillgänglig i AppSource till USA $15/månad.</span><span class="sxs-lookup"><span data-stu-id="385b5-115">The paid version of the Connectors is available in AppSource at US$ 15/month.</span></span> <span data-ttu-id="385b5-116">Med den betalda anslutningen kommer du att få 10 000 API-anrop per dag.</span><span class="sxs-lookup"><span data-stu-id="385b5-116">With the paid connection, you will be getting 10K API calls per day.</span></span> <span data-ttu-id="385b5-117">Kopplingarna är omslutningar ovanpå partner Centers hänvisnings-API: er.</span><span class="sxs-lookup"><span data-stu-id="385b5-117">The Connectors are wrappers on top of Partner Center referral APIs.</span></span> <span data-ttu-id="385b5-118">När kopplings lösningarna körs för att **skapa** eller **Uppdatera** en händelse för affärs möjligheter i antingen Partner Center eller på CRM-sidan, görs ett API-anrop.</span><span class="sxs-lookup"><span data-stu-id="385b5-118">Whenever the connector solutions run for a **Create** or **Update** event on the opportunities on either Partner Center or the CRM side, an API call is made.</span></span>

2. <span data-ttu-id="385b5-119">Vilken roll behöver du för att skapa avsnitt i CRM-miljön?</span><span class="sxs-lookup"><span data-stu-id="385b5-119">What role do you need to create sections in CRM environment?</span></span>

<span data-ttu-id="385b5-120">Användare som är system administratörer eller systemanpassare kan tillämpa ändringar för alla.</span><span class="sxs-lookup"><span data-stu-id="385b5-120">Users who are system admins or system customizers can apply changes for everyone.</span></span> <span data-ttu-id="385b5-121">Alla App-användare kan dock anpassa systemet och till och med dela vissa av deras anpassningar med andra.</span><span class="sxs-lookup"><span data-stu-id="385b5-121">All app users, however,  can personalize the system and even share some of their customizations with others.</span></span> 

3. <span data-ttu-id="385b5-122">Behöver partner leverantörer särskilda roller för att arbeta med partner Center?</span><span class="sxs-lookup"><span data-stu-id="385b5-122">Do partner sellers need special roles to work on Partner Center?</span></span>
 
<span data-ttu-id="385b5-123">Partner säljare måste tilldelas rollen "hänvisnings administratör".</span><span class="sxs-lookup"><span data-stu-id="385b5-123">Partner sellers must be assigned the “Referrals admin” role.</span></span> <span data-ttu-id="385b5-124">Mer information finns i följande [behörigheter översikt) (Create-User-Accounts-and-set-Permissions).</span><span class="sxs-lookup"><span data-stu-id="385b5-124">For more information, refer to the following [Permissions overview)(create-user-accounts-and-set-permissions).</span></span>

4. <span data-ttu-id="385b5-125">Vilka fält måste konfigureras först i din CRM-miljö?</span><span class="sxs-lookup"><span data-stu-id="385b5-125">What fields need to be set up first in your CRM environment?</span></span> 

<span data-ttu-id="385b5-126">• Kontrol lera att din valuta passar din plats och att den är korrekt i din CRM-miljö.</span><span class="sxs-lookup"><span data-stu-id="385b5-126">• Make sure your currency is appropriate to your location and is in your CRM environment accurately.</span></span> <span data-ttu-id="385b5-127">• Ditt säljteam bör visas i din CRM-miljö som CRM-användare.</span><span class="sxs-lookup"><span data-stu-id="385b5-127">• Your sales team should be listed in your CRM environment as CRM users.</span></span>

5. <span data-ttu-id="385b5-128">Vilka krav krävs för att skapa en automatisk miljö?</span><span class="sxs-lookup"><span data-stu-id="385b5-128">What pre-requisites are required for Power Automate environment creation?</span></span>

<span data-ttu-id="385b5-129">Om du vill använda Energis par miljön behöver du:</span><span class="sxs-lookup"><span data-stu-id="385b5-129">To use the Power Automate environment, you need:</span></span>

- <span data-ttu-id="385b5-130">En energi automatiserad licens krävs.</span><span class="sxs-lookup"><span data-stu-id="385b5-130">A Power Automate license is required.</span></span>
- <span data-ttu-id="385b5-131">Minst 1 GB lagring krävs.</span><span class="sxs-lookup"><span data-stu-id="385b5-131">A minimum of 1-GB storage is required.</span></span>

6.  <span data-ttu-id="385b5-132">Behöver du en Dynamics 365-prenumeration för att använda Salesforce Connector-lösningen?</span><span class="sxs-lookup"><span data-stu-id="385b5-132">Do you need a Dynamics 365 subscription to use Salesforce Connectors solution?</span></span>

<span data-ttu-id="385b5-133">Salesforce Connector-lösningen är av typen "Dynamics Flow" som stöder synkronisering med andra CRM-system.</span><span class="sxs-lookup"><span data-stu-id="385b5-133">The Salesforce Connector solution is of type “Dynamics Flow” that supports synchronizing with other CRM systems.</span></span> <span data-ttu-id="385b5-134">Lösningen kräver inte att du har en Dynamics 365-instans eller en prenumeration.</span><span class="sxs-lookup"><span data-stu-id="385b5-134">The solution doesn’t require you to have a Dynamics 365 instance or a subscription.</span></span> <span data-ttu-id="385b5-135">När du installerar Salesforce-lösningen kan det hända att en listruta med befintlig CD-miljö i företaget visas.</span><span class="sxs-lookup"><span data-stu-id="385b5-135">While installing the Salesforce solution, a drop-down with existing CDS environment in your company may appear.</span></span> <span data-ttu-id="385b5-136">Du måste välja den miljön.</span><span class="sxs-lookup"><span data-stu-id="385b5-136">You need to select that environment.</span></span> <span data-ttu-id="385b5-137">Om du får felet "vi kunde inte hitta en Dynamics 365-organisation som är ansluten till den inloggade användaren" måste du dessutom skapa en ny miljö för anslutnings tjänsten.</span><span class="sxs-lookup"><span data-stu-id="385b5-137">In addition, if you get the error "We couldn't find a Dynamics 365 organization connected to signed-in user", then you will need to create new environment for connector.</span></span>

## <a name="questions-and-answers-about-configuration"></a><span data-ttu-id="385b5-138">Frågor och svar om konfigurationen</span><span class="sxs-lookup"><span data-stu-id="385b5-138">Questions and answers about configuration</span></span>

1. <span data-ttu-id="385b5-139">Vad bör du göra om följande fel uppstår när du aktiverar flöden i en automatiserad plattform?</span><span class="sxs-lookup"><span data-stu-id="385b5-139">What should you do if you face the following error while activating flows in Power Automate Platform?</span></span>

<span data-ttu-id="385b5-140">Fel: begäran till Azure Resource Manager misslyckades med felet: {"fel": {"Code": "WorkflowTriggerNotFound", "meddelande": "Det gick inte att hitta" e14d00f1-1fdf-4b1b-aaac-54a5064093d3 "-utlösaren för arbets flödet."}}.</span><span class="sxs-lookup"><span data-stu-id="385b5-140">Error: Request to Azure Resource Manager failed with error: '{"error":{"code":"WorkflowTriggerNotFound","message":"The workflow 'e14d00f1-1fdf-4b1b-aaac-54a5064093d3' trigger 'manual' could not be found."}}'.</span></span> 

<span data-ttu-id="385b5-141">Följ dessa fel söknings steg:</span><span class="sxs-lookup"><span data-stu-id="385b5-141">Follow these troubleshooting steps:</span></span>

- <span data-ttu-id="385b5-142">Ta bort CD-anslutningen och återskapa sedan CD-anslutningarna.</span><span class="sxs-lookup"><span data-stu-id="385b5-142">Delete the CDS connection and then recreate the CDS connections.</span></span>
- <span data-ttu-id="385b5-143">Aktivera och inaktivera det underordnade flödet</span><span class="sxs-lookup"><span data-stu-id="385b5-143">Turn the child flow off and on</span></span> 
- <span data-ttu-id="385b5-144">Ta bort lösningen och installera sedan om lösningen.</span><span class="sxs-lookup"><span data-stu-id="385b5-144">Delete solution and then reinstall the solution.</span></span> 

2.  <span data-ttu-id="385b5-145">Vad bör du göra om du kommer till fel meddelandet "logga in" när jag lägger till en partner Center-koppling i en automatiserad plattform?</span><span class="sxs-lookup"><span data-stu-id="385b5-145">What should you do if you face the "Sign in" error while adding a Partner Center connector in Power Automate Platform?</span></span>

:::image type="content" source="images/cosellconnectors/failure.png" alt-text="Fel meddelande som kräver inloggning":::

<span data-ttu-id="385b5-147">Följ det här fel söknings steget:</span><span class="sxs-lookup"><span data-stu-id="385b5-147">Follow this troubleshooting step:</span></span>

- <span data-ttu-id="385b5-148">Använd dina partner Center-autentiseringsuppgifter för att logga in i Flow-miljön en gång (flow.microsoft.com).</span><span class="sxs-lookup"><span data-stu-id="385b5-148">Use your Partner Center credentials to sign into the flow environment once (flow.microsoft.com).</span></span>


3. <span data-ttu-id="385b5-149">Vad ska du göra om du får följande fel meddelande när du aktiverar Partner Center till CRM-flödet i en automatiserad plattform?</span><span class="sxs-lookup"><span data-stu-id="385b5-149">What should you do if you receive the following error while activating the Partner Center to CRM flow in Power Automate Platform?</span></span>
 
:::image type="content" source="images/cosellconnectors/powererror.png" alt-text="Fel meddelande som kräver uppdateringar":::

<span data-ttu-id="385b5-151">Följ dessa fel söknings steg:</span><span class="sxs-lookup"><span data-stu-id="385b5-151">Follow these troubleshooting steps:</span></span>

- <span data-ttu-id="385b5-152">Aktivera följande två underordnade flöden innan du aktiverar Partner Center till CRM-flödet.</span><span class="sxs-lookup"><span data-stu-id="385b5-152">Activate the following two child flows first before you activate the Partner Center to CRM flow.</span></span>
      - <span data-ttu-id="385b5-153">Partner Center till CRM – Helper (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="385b5-153">Partner Center to CRM - Helper (Insider Preview)</span></span>
      - <span data-ttu-id="385b5-154">Partner Center Microsoft Co-Sälj hänvisnings uppdateringar till CRM (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="385b5-154">Partner Center Microsoft Co-sell Referral Updates to CRM (Insider Preview)</span></span>

4. <span data-ttu-id="385b5-155">Vad bör du göra när du inte kan lägga till anslutningar i flödet när du försöker redigera flödet?</span><span class="sxs-lookup"><span data-stu-id="385b5-155">What should you do when you aren't able to add connections to the flow when you try to edit the flow?</span></span>

<span data-ttu-id="385b5-156">Du lägger till anslutningar till flödet när flödet körs och du lägger till varje flöde separat.</span><span class="sxs-lookup"><span data-stu-id="385b5-156">You add connections to the flow while the flow is running, and you add to each flow separately.</span></span>  <span data-ttu-id="385b5-157">Om dialog rutan för att lägga till anslutningar inte öppnas automatiskt när du redigerar flödet kan du redigera vart och ett av stegen och under stegen för flödena individuellt.</span><span class="sxs-lookup"><span data-stu-id="385b5-157">If the dialog to add connections doesn't open up automatically while editing the flow, then you can edit each of the steps and sub steps of the flows individually.</span></span>

- <span data-ttu-id="385b5-158">Välj varje flöde och redigera dem individuellt.</span><span class="sxs-lookup"><span data-stu-id="385b5-158">Select each flow and edit them individually.</span></span>
- <span data-ttu-id="385b5-159">Expandera alla steg i flödet</span><span class="sxs-lookup"><span data-stu-id="385b5-159">Expand all the steps in the flow</span></span> 

:::image type="content" source="images/cosellconnectors/flowsteps.png" alt-text="Steg som behöver anslutningar":::

- <span data-ttu-id="385b5-161">Välj de steg där du ser en varnings ikon som uppmanar dig att associera anslutningar och lägga till anslutningar.</span><span class="sxs-lookup"><span data-stu-id="385b5-161">Select the steps where you see a warning icon asking to associate connections, and add connections.</span></span> 

:::image type="content" source="images/cosellconnectors/editflow.png" alt-text="Redigera flöde-steg per steg":::


5. <span data-ttu-id="385b5-163">Vad ska jag göra om flödena för den samsälje referral Connector-lösningen inte aktive ras?</span><span class="sxs-lookup"><span data-stu-id="385b5-163">What should you do if the flows of the Co-sell Referrals Connectors solution don’t turn on?</span></span>

<span data-ttu-id="385b5-164">A.</span><span class="sxs-lookup"><span data-stu-id="385b5-164">A.</span></span> <span data-ttu-id="385b5-165">I energi spar läge måste du redigera flöden i följande ordning och uppdatera dem så att de använder rätt anslutningar:</span><span class="sxs-lookup"><span data-stu-id="385b5-165">In Power Automate, you'll need to edit flows in the following order and update them to use the correct connections:</span></span>

- <span data-ttu-id="385b5-166">Partner Center – registrering av webhook (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="385b5-166">Partner Center Webhook Registration (Insider Preview)</span></span>
- <span data-ttu-id="385b5-167">Skapa Co-sälje referral-Salesforce till Partner Center (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="385b5-167">Create Co-sell Referral - Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="385b5-168">Partner Center Microsoft Co-Sälj hänvisnings uppdateringar till Salesforce (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="385b5-168">Partner Center Microsoft Co-sell Referral Updates to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="385b5-169">Partner Center till Salesforce (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="385b5-169">Partner Center to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="385b5-170">Salesforce till Partner Center (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="385b5-170">Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="385b5-171">Salesforce-möjlighet till Partner Center (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="385b5-171">Salesforce Opportunity to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="385b5-172">Salesforce Microsoft-lösningar till Partner Center (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="385b5-172">Salesforce Microsoft Solutions to Partner Center (Insider Preview)</span></span>

 <span data-ttu-id="385b5-173">B.</span><span class="sxs-lookup"><span data-stu-id="385b5-173">B.</span></span> <span data-ttu-id="385b5-174">För varje flöde väljer du alternativet **Kör endast användare** .</span><span class="sxs-lookup"><span data-stu-id="385b5-174">For each of flow, select **Run only users** option.</span></span> <span data-ttu-id="385b5-175">Välj **Använd anslutning** i stället för att **tillhandahållas av endast körnings användare** .</span><span class="sxs-lookup"><span data-stu-id="385b5-175">Select **Use connection** instead of **Provided by run-only user** .</span></span>  

:::image type="content" source="images/cosellconnectors/runonly.png" alt-text="Aktivera ett flöde":::


<span data-ttu-id="385b5-177">C.</span><span class="sxs-lookup"><span data-stu-id="385b5-177">C.</span></span> <span data-ttu-id="385b5-178">Aktivera följande flöden:</span><span class="sxs-lookup"><span data-stu-id="385b5-178">Activate these below mentioned flows:</span></span>

 - <span data-ttu-id="385b5-179">Partner Center Microsoft Co-Sälj hänvisnings uppdateringar till Salesforce (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="385b5-179">Partner Center Microsoft Co-sell Referral Updates to Salesforce (Insider Preview)</span></span>

- <span data-ttu-id="385b5-180">Salesforce till Partner Center (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="385b5-180">Salesforce to Partner Center (Insider Preview)</span></span>

    
<span data-ttu-id="385b5-181">D.</span><span class="sxs-lookup"><span data-stu-id="385b5-181">D.</span></span> <span data-ttu-id="385b5-182">Aktivera alla återstående flöden.</span><span class="sxs-lookup"><span data-stu-id="385b5-182">Activate all the remaining flows.</span></span>

<span data-ttu-id="385b5-183">E.</span><span class="sxs-lookup"><span data-stu-id="385b5-183">E.</span></span> <span data-ttu-id="385b5-184">I Flow Partner Center-webhook-registrering väljer du **Kör** .</span><span class="sxs-lookup"><span data-stu-id="385b5-184">At flow Partner Center Webhook Registration, select **Run** .</span></span> <span data-ttu-id="385b5-185">Ange **http-URL:** en från den första åtgärden i **partner Center till Salesforce** -flöde.</span><span class="sxs-lookup"><span data-stu-id="385b5-185">Provide the **http url** from the first action in **Partner Center to Salesforce** flow.</span></span> <span data-ttu-id="385b5-186">Välj alla fyra alternativen under **händelser som ska registreras** och välj **Ja** för Skriv över.</span><span class="sxs-lookup"><span data-stu-id="385b5-186">Select all four options under **Events to register** and select **yes** for Overwrite.</span></span>

## <a name="questions-and-answers-about-runmaintenance"></a><span data-ttu-id="385b5-187">Frågor och svar om körning/underhåll</span><span class="sxs-lookup"><span data-stu-id="385b5-187">Questions and answers about Run/Maintenance</span></span>

1. <span data-ttu-id="385b5-188">Hur felsöker jag om fel uppstår under automatisk flödes körning?</span><span class="sxs-lookup"><span data-stu-id="385b5-188">How do you troubleshoot in case of failures during Power Automate flow execution?</span></span>

<span data-ttu-id="385b5-189">För att se till att dina energi scheman körs som du förväntar dig och Felsök fel under körningen, se [åtgärda flödes fel](/power-automate/fix-flow-failures).</span><span class="sxs-lookup"><span data-stu-id="385b5-189">To ensure that your Power Automate flows run as you expect and to troubleshoot failures during execution, refer to [Fix flow failures](/power-automate/fix-flow-failures).</span></span>

2. <span data-ttu-id="385b5-190">Vad bör du göra om du ser referenser som inte har synkroniserats korrekt i Partner Center eller i en CRM-miljö?</span><span class="sxs-lookup"><span data-stu-id="385b5-190">What should you do if you see referrals that aren't synchronized properly in Partner Center or CRM environment?</span></span>
 
<span data-ttu-id="385b5-191">Välj **granskning** för att fastställa status för referens synkroniseringen.</span><span class="sxs-lookup"><span data-stu-id="385b5-191">To determine the status of referral synchronization, select **Audit** .</span></span> 

:::image type="content" source="images/cosellconnectors/synch.png" alt-text="Så här synkroniserar du referenser":::

<span data-ttu-id="385b5-193">Se till att följande villkor är uppfyllda:</span><span class="sxs-lookup"><span data-stu-id="385b5-193">Ensure that the following conditions are met:</span></span>

- <span data-ttu-id="385b5-194">Lösnings-ID tillhandahålls som en del av affärs möjligheten.</span><span class="sxs-lookup"><span data-stu-id="385b5-194">Solution id is provided as part of the opportunity.</span></span>

- <span data-ttu-id="385b5-195">Landskod för två bokstäver måste anges.</span><span class="sxs-lookup"><span data-stu-id="385b5-195">Two letter country code is required.</span></span>

- <span data-ttu-id="385b5-196">När hjälp från Microsoft väljs för affärs möjligheten krävs kundens kontakt uppgifter.</span><span class="sxs-lookup"><span data-stu-id="385b5-196">When help from Microsoft is selected for the opportunity, customer contact information is required.</span></span>

3. <span data-ttu-id="385b5-197">Hur ser du till att en hänvisning synkroniseras i dubbelriktad riktning?</span><span class="sxs-lookup"><span data-stu-id="385b5-197">How to ensure that a referral will synchronize bi-directionally?</span></span>

<span data-ttu-id="385b5-198">Gör så här:</span><span class="sxs-lookup"><span data-stu-id="385b5-198">Do the following steps:</span></span>

- <span data-ttu-id="385b5-199">Partner leverantörer måste se till att de har aktiverat alternativet **Synkronisera med alternativet för partner Center** i avsnittet CRM.</span><span class="sxs-lookup"><span data-stu-id="385b5-199">Partner sellers need to ensure that they have enabled **Sync with Partner Center** option in the CRM section.</span></span>

:::image type="content" source="images/cosellconnectors/enablesynch.png" alt-text="Se till att du har aktiverat Synch":::

- <span data-ttu-id="385b5-201">Säljare måste ange intäkter och UB-datum när de kvalificerar sig för ett lead.</span><span class="sxs-lookup"><span data-stu-id="385b5-201">Sellers need to provide revenue and closing date when qualifying a lead.</span></span>

- <span data-ttu-id="385b5-202">Om CRM-ID: t anges i steget **skapa** eller **Uppdatera** stadium av samförsäljning, men det inte gick att hitta en lead-möjlighet med detta ID i CRM, så ignoreras uppdatering eller skapande.</span><span class="sxs-lookup"><span data-stu-id="385b5-202">If CRM ID is provided in the **create** or **update** stage of co-sell opportunity, but a lead opportunity with that ID is not found in CRM, then update or create will be ignored.</span></span>

- <span data-ttu-id="385b5-203">Se till att fältet hänvisnings valuta har kon figurer ATS i Salesforce-miljö.</span><span class="sxs-lookup"><span data-stu-id="385b5-203">Ensure that referral currency field is configured on Salesforce environment.</span></span> 

4. <span data-ttu-id="385b5-204">Vad gör du om anslutningen kopplas från och du saknar en referens synkronisering.</span><span class="sxs-lookup"><span data-stu-id="385b5-204">What should you do if the connector gets disconnected and you miss a referral synchronization.</span></span> 

<span data-ttu-id="385b5-205">Nedan följer några av de alternativ som du kan prova:</span><span class="sxs-lookup"><span data-stu-id="385b5-205">Following are few of the options that you can try out:</span></span>

- <span data-ttu-id="385b5-206">Kontrol lera om användar namnet eller lösen ordet har upphört att gälla för partner Center-användaren med referens administratörs roller.</span><span class="sxs-lookup"><span data-stu-id="385b5-206">Check whether username or password has expired for the Partner Center user with referral admin roles.</span></span>

- <span data-ttu-id="385b5-207">Du kan gå till den icke-synkroniserade möjligheten, göra en mindre uppdatering och kontrol lera om hänvisningen har synkroniserats.</span><span class="sxs-lookup"><span data-stu-id="385b5-207">You can go to the un-synchronized opportunity, make a minor update, and observe whether the referral has synchronized.</span></span>

- <span data-ttu-id="385b5-208">Om flödena har körts och misslyckats väljer du flödet och skickar om körningen som har misslyckats.</span><span class="sxs-lookup"><span data-stu-id="385b5-208">If the flows have run and failed, then select the flow and re-submit the run which has failed.</span></span>

5. <span data-ttu-id="385b5-209">Vad bör du göra när du får åtkomst nekade fel?</span><span class="sxs-lookup"><span data-stu-id="385b5-209">What should you do when you get access denied errors?</span></span>

<span data-ttu-id="385b5-210">Kontrol lera att rätt roller finns</span><span class="sxs-lookup"><span data-stu-id="385b5-210">Make sure the appropriate roles exist</span></span>

- <span data-ttu-id="385b5-211">Referens administratörs roll för partner Center-säljaren</span><span class="sxs-lookup"><span data-stu-id="385b5-211">Referral Administrator role for Partner Center seller</span></span> 
 
- <span data-ttu-id="385b5-212">Rollen system administratör eller systemanpassare på din CRM-instans</span><span class="sxs-lookup"><span data-stu-id="385b5-212">System Administrator or System Customizer role on your CRM instance</span></span>

- <span data-ttu-id="385b5-213">Se till att energischemat flödes konto användare loggar in https://flow.microsoft.com minst en gång på förhand</span><span class="sxs-lookup"><span data-stu-id="385b5-213">Ensure that the Power Automate flow account user logs into https://flow.microsoft.com at least once beforehand</span></span>

6. <span data-ttu-id="385b5-214">Vad gör du om du ser att **land koden för kund kontot** saknas när du skapar en samförsäljnings möjlighet?</span><span class="sxs-lookup"><span data-stu-id="385b5-214">If you see that **Customer account country code** is missing while creating a Co-sell opportunity, what should you do?</span></span>

<span data-ttu-id="385b5-215">Du måste lägga till ISO-koden med två bokstäver till kund kontot i CRM.</span><span class="sxs-lookup"><span data-stu-id="385b5-215">You will need to add the ISO two-letter country code to the Customer account in CRM.</span></span>

7. <span data-ttu-id="385b5-216">Vad bör du göra om du ser felet att **lösnings-ID krävs** när du skapar en samförsäljnings möjlighet?</span><span class="sxs-lookup"><span data-stu-id="385b5-216">What should you do if you see the error that **Solution ID is required** while creating a Co-sell opportunity?</span></span>

<span data-ttu-id="385b5-217">För att kunna skapa en samförsäljnings hänvisning behöver du en Microsoft Co-försäljnings klar lösning.</span><span class="sxs-lookup"><span data-stu-id="385b5-217">In order to create a co-sell referral, you need a Microsoft co-sell ready solution.</span></span> 

8. <span data-ttu-id="385b5-218">Vad bör du göra när du ser samförsäljnings möjligheter som skapats i Partner Center som inte synkroniseras till CRM trots att det inte finns några Flow-fel:</span><span class="sxs-lookup"><span data-stu-id="385b5-218">What should you do when you see Co-sell opportunities created in Partner Center that aren't synchronized to CRM even though there are no flow errors:</span></span>

<span data-ttu-id="385b5-219">Gör följande:</span><span class="sxs-lookup"><span data-stu-id="385b5-219">Do the following:</span></span>

- <span data-ttu-id="385b5-220">När du har skapat en ny co-sälje-affär i Partner Center kontrollerar du om Partner Center till Dynamics 365 Flow anropas (det kan komma att anropas flera gånger).</span><span class="sxs-lookup"><span data-stu-id="385b5-220">After you have created a new co-sell deal in Partner Center, check if Partner Center to Dynamics 365 flow gets invoked (it might get invoked multiple times).</span></span>

- <span data-ttu-id="385b5-221">Om flödet anropas kontrollerar du alla anropade flöden och identifierar körningen av flödet som uppdaterar CRM.</span><span class="sxs-lookup"><span data-stu-id="385b5-221">If the flow gets invoked, check all invoked flows, and identify the flow run which would update the CRM.</span></span> <span data-ttu-id="385b5-222">Du kan följa instruktionerna och kontrol lera om det har uppdaterats i CRM eller ett problem har uppstått.</span><span class="sxs-lookup"><span data-stu-id="385b5-222">You can follow the actions and verify if it did update the CRM or encountered a problem.</span></span>

- <span data-ttu-id="385b5-223">Titta på *nytt erbjudande* \* i Partner Center för att se om det fylls med CRM-ID.</span><span class="sxs-lookup"><span data-stu-id="385b5-223">Check *New deal* \* in Partner Center to see if it gets populated with CRM ID.</span></span>

- <span data-ttu-id="385b5-224">Se till att affären inte stängs av misstag som "vunnen" eller "förlorad" i Partner Center.</span><span class="sxs-lookup"><span data-stu-id="385b5-224">Make sure that the deal is not accidentally closed as “Won” or “Lost” in Partner Center.</span></span>

## <a name="next-steps"></a><span data-ttu-id="385b5-225">Nästa steg</span><span class="sxs-lookup"><span data-stu-id="385b5-225">Next steps</span></span>

- [<span data-ttu-id="385b5-226">Hantera leads</span><span class="sxs-lookup"><span data-stu-id="385b5-226">Manage leads</span></span>](manage-leads.md)
 
- [<span data-ttu-id="385b5-227">Hantera möjligheter till samförsäljning</span><span class="sxs-lookup"><span data-stu-id="385b5-227">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)