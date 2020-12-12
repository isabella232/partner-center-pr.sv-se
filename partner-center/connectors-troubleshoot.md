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
ms.openlocfilehash: b8977f7c602b8587a619236b37a760a55bf87e53
ms.sourcegitcommit: 22d79fb31cce852ae809078ea2310ebc80030739
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 12/12/2020
ms.locfileid: "97354550"
---
# <a name="troubleshoot-co-sell-referrals-connectors"></a><span data-ttu-id="20803-104">Felsöka samsäljande referral-kopplingar</span><span class="sxs-lookup"><span data-stu-id="20803-104">Troubleshoot co-sell referrals connectors</span></span>

<span data-ttu-id="20803-105">**Gäller för:**</span><span class="sxs-lookup"><span data-stu-id="20803-105">**Applies to:**</span></span>

- <span data-ttu-id="20803-106">Dynamics 365 CRM</span><span class="sxs-lookup"><span data-stu-id="20803-106">Dynamics 365 CRM</span></span>
- <span data-ttu-id="20803-107">Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="20803-107">Salesforce CRM</span></span>

<span data-ttu-id="20803-108">**Lämpliga roller**</span><span class="sxs-lookup"><span data-stu-id="20803-108">**Appropriate roles**</span></span>

- <span data-ttu-id="20803-109">Referens administratör</span><span class="sxs-lookup"><span data-stu-id="20803-109">Referrals admin</span></span>
- <span data-ttu-id="20803-110">System administratör eller systemanpassare på CRM</span><span class="sxs-lookup"><span data-stu-id="20803-110">System admin or system customizer on the CRM</span></span>

 ## <a name="questions-and-answers-about-pre-requisites"></a><span data-ttu-id="20803-111">Frågor och svar om krav</span><span class="sxs-lookup"><span data-stu-id="20803-111">Questions and answers about pre-requisites</span></span>

1. <span data-ttu-id="20803-112">Kan du använda en lösning för att använda en utvärderings version av referral Connector för din miljö?</span><span class="sxs-lookup"><span data-stu-id="20803-112">Can you use a trial co-sell referrals connectors solution for your environment?</span></span>

<span data-ttu-id="20803-113">Om du är i test-/Staging-miljön kan du välja en utvärderings lösning.</span><span class="sxs-lookup"><span data-stu-id="20803-113">If you are on the test/staging environment, you can opt for trial solution.</span></span> <span data-ttu-id="20803-114">Den betalda versionen av kopplingarna är tillgänglig i AppSource till USA $15/månad.</span><span class="sxs-lookup"><span data-stu-id="20803-114">The paid version of the Connectors is available in AppSource at US$ 15/month.</span></span> <span data-ttu-id="20803-115">Med den betalda anslutningen kommer du att få 10 000 API-anrop per dag.</span><span class="sxs-lookup"><span data-stu-id="20803-115">With the paid connection, you will be getting 10K API calls per day.</span></span> <span data-ttu-id="20803-116">Kopplingarna är omslutningar ovanpå partner Centers hänvisnings-API: er.</span><span class="sxs-lookup"><span data-stu-id="20803-116">The Connectors are wrappers on top of Partner Center referral APIs.</span></span> <span data-ttu-id="20803-117">När kopplings lösningarna körs för att **skapa** eller **Uppdatera** en händelse för affärs möjligheter i antingen Partner Center eller på CRM-sidan, görs ett API-anrop.</span><span class="sxs-lookup"><span data-stu-id="20803-117">Whenever the connector solutions run for a **Create** or **Update** event on the opportunities on either Partner Center or the CRM side, an API call is made.</span></span>

2. <span data-ttu-id="20803-118">Vilken roll behöver du för att skapa avsnitt i CRM-miljön?</span><span class="sxs-lookup"><span data-stu-id="20803-118">What role do you need to create sections in CRM environment?</span></span>

<span data-ttu-id="20803-119">Användare som är system administratörer eller systemanpassare kan tillämpa ändringar för alla.</span><span class="sxs-lookup"><span data-stu-id="20803-119">Users who are system admins or system customizers can apply changes for everyone.</span></span> <span data-ttu-id="20803-120">Alla App-användare kan dock anpassa systemet och till och med dela vissa av deras anpassningar med andra.</span><span class="sxs-lookup"><span data-stu-id="20803-120">All app users, however,  can personalize the system and even share some of their customizations with others.</span></span> 

3. <span data-ttu-id="20803-121">Behöver partner leverantörer särskilda roller för att arbeta med partner Center?</span><span class="sxs-lookup"><span data-stu-id="20803-121">Do partner sellers need special roles to work on Partner Center?</span></span>
 
<span data-ttu-id="20803-122">Partner säljare måste tilldelas rollen "hänvisnings administratör".</span><span class="sxs-lookup"><span data-stu-id="20803-122">Partner sellers must be assigned the “Referrals admin” role.</span></span> <span data-ttu-id="20803-123">Mer information finns i följande [behörigheter översikt) (Create-User-Accounts-and-set-Permissions).</span><span class="sxs-lookup"><span data-stu-id="20803-123">For more information, refer to the following [Permissions overview)(create-user-accounts-and-set-permissions).</span></span>

4. <span data-ttu-id="20803-124">Vilka fält måste konfigureras först i din CRM-miljö?</span><span class="sxs-lookup"><span data-stu-id="20803-124">What fields need to be set up first in your CRM environment?</span></span> 

<span data-ttu-id="20803-125">• Kontrol lera att din valuta passar din plats och att den är korrekt i din CRM-miljö.</span><span class="sxs-lookup"><span data-stu-id="20803-125">• Make sure your currency is appropriate to your location and is in your CRM environment accurately.</span></span> <span data-ttu-id="20803-126">• Ditt säljteam bör visas i din CRM-miljö som CRM-användare.</span><span class="sxs-lookup"><span data-stu-id="20803-126">• Your sales team should be listed in your CRM environment as CRM users.</span></span>

5. <span data-ttu-id="20803-127">Vilka krav krävs för att skapa en automatisk miljö?</span><span class="sxs-lookup"><span data-stu-id="20803-127">What pre-requisites are required for Power Automate environment creation?</span></span>

<span data-ttu-id="20803-128">Om du vill använda Energis par miljön behöver du:</span><span class="sxs-lookup"><span data-stu-id="20803-128">To use the Power Automate environment, you need:</span></span>

- <span data-ttu-id="20803-129">En energi automatiserad licens krävs.</span><span class="sxs-lookup"><span data-stu-id="20803-129">A Power Automate license is required.</span></span>
- <span data-ttu-id="20803-130">Minst 1 GB lagring krävs.</span><span class="sxs-lookup"><span data-stu-id="20803-130">A minimum of 1-GB storage is required.</span></span>

6.  <span data-ttu-id="20803-131">Behöver du en Dynamics 365-prenumeration för att använda Salesforce Connector-lösningen?</span><span class="sxs-lookup"><span data-stu-id="20803-131">Do you need a Dynamics 365 subscription to use Salesforce Connectors solution?</span></span>

<span data-ttu-id="20803-132">Salesforce Connector-lösningen är av typen "Dynamics Flow" som stöder synkronisering med andra CRM-system.</span><span class="sxs-lookup"><span data-stu-id="20803-132">The Salesforce Connector solution is of type “Dynamics Flow” that supports synchronizing with other CRM systems.</span></span> <span data-ttu-id="20803-133">Lösningen kräver inte att du har en Dynamics 365-instans eller en prenumeration.</span><span class="sxs-lookup"><span data-stu-id="20803-133">The solution doesn’t require you to have a Dynamics 365 instance or a subscription.</span></span> <span data-ttu-id="20803-134">När du installerar Salesforce-lösningen kan det hända att en listruta med befintlig CD-miljö i företaget visas.</span><span class="sxs-lookup"><span data-stu-id="20803-134">While installing the Salesforce solution, a drop-down with existing CDS environment in your company may appear.</span></span> <span data-ttu-id="20803-135">Du måste välja den miljön.</span><span class="sxs-lookup"><span data-stu-id="20803-135">You need to select that environment.</span></span> <span data-ttu-id="20803-136">Om du får felet "vi kunde inte hitta en Dynamics 365-organisation som är ansluten till den inloggade användaren" måste du dessutom skapa en ny miljö för anslutnings tjänsten.</span><span class="sxs-lookup"><span data-stu-id="20803-136">In addition, if you get the error "We couldn't find a Dynamics 365 organization connected to signed-in user", then you will need to create new environment for connector.</span></span>

## <a name="questions-and-answers-about-configuration"></a><span data-ttu-id="20803-137">Frågor och svar om konfigurationen</span><span class="sxs-lookup"><span data-stu-id="20803-137">Questions and answers about configuration</span></span>

1. <span data-ttu-id="20803-138">Vad bör du göra om följande fel uppstår när du aktiverar flöden i en automatiserad plattform?</span><span class="sxs-lookup"><span data-stu-id="20803-138">What should you do if you face the following error while activating flows in Power Automate Platform?</span></span>

<span data-ttu-id="20803-139">Fel: begäran till Azure Resource Manager misslyckades med felet: {"fel": {"Code": "WorkflowTriggerNotFound", "meddelande": "Det gick inte att hitta" e14d00f1-1fdf-4b1b-aaac-54a5064093d3 "-utlösaren för arbets flödet."}}.</span><span class="sxs-lookup"><span data-stu-id="20803-139">Error: Request to Azure Resource Manager failed with error: '{"error":{"code":"WorkflowTriggerNotFound","message":"The workflow 'e14d00f1-1fdf-4b1b-aaac-54a5064093d3' trigger 'manual' could not be found."}}'.</span></span> 

<span data-ttu-id="20803-140">Följ dessa fel söknings steg:</span><span class="sxs-lookup"><span data-stu-id="20803-140">Follow these troubleshooting steps:</span></span>

- <span data-ttu-id="20803-141">Ta bort CD-anslutningen och återskapa sedan CD-anslutningarna.</span><span class="sxs-lookup"><span data-stu-id="20803-141">Delete the CDS connection and then recreate the CDS connections.</span></span>
- <span data-ttu-id="20803-142">Aktivera och inaktivera det underordnade flödet</span><span class="sxs-lookup"><span data-stu-id="20803-142">Turn the child flow off and on</span></span> 
- <span data-ttu-id="20803-143">Ta bort lösningen och installera sedan om lösningen.</span><span class="sxs-lookup"><span data-stu-id="20803-143">Delete solution and then reinstall the solution.</span></span> 

2.  <span data-ttu-id="20803-144">Vad bör du göra om du kommer till fel meddelandet "logga in" när jag lägger till en partner Center-koppling i en automatiserad plattform?</span><span class="sxs-lookup"><span data-stu-id="20803-144">What should you do if you face the "Sign in" error while adding a Partner Center connector in Power Automate Platform?</span></span>

:::image type="content" source="images/cosellconnectors/failure.png" alt-text="Fel meddelande som kräver inloggning":::

<span data-ttu-id="20803-146">Följ det här fel söknings steget:</span><span class="sxs-lookup"><span data-stu-id="20803-146">Follow this troubleshooting step:</span></span>

- <span data-ttu-id="20803-147">Använd dina partner Center-autentiseringsuppgifter för att logga in i Flow-miljön en gång (flow.microsoft.com).</span><span class="sxs-lookup"><span data-stu-id="20803-147">Use your Partner Center credentials to sign into the flow environment once (flow.microsoft.com).</span></span>


3. <span data-ttu-id="20803-148">Vad ska du göra om du får följande fel meddelande när du aktiverar Partner Center till CRM-flödet i en automatiserad plattform?</span><span class="sxs-lookup"><span data-stu-id="20803-148">What should you do if you receive the following error while activating the Partner Center to CRM flow in Power Automate Platform?</span></span>
 
:::image type="content" source="images/cosellconnectors/powererror.png" alt-text="Fel meddelande som kräver uppdateringar":::

<span data-ttu-id="20803-150">Följ dessa fel söknings steg:</span><span class="sxs-lookup"><span data-stu-id="20803-150">Follow these troubleshooting steps:</span></span>

- <span data-ttu-id="20803-151">Aktivera följande två underordnade flöden innan du aktiverar Partner Center till CRM-flödet.</span><span class="sxs-lookup"><span data-stu-id="20803-151">Activate the following two child flows first before you activate the Partner Center to CRM flow.</span></span>
      - <span data-ttu-id="20803-152">Partner Center till CRM – Helper (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="20803-152">Partner Center to CRM - Helper (Insider Preview)</span></span>
      - <span data-ttu-id="20803-153">Partner Center Microsoft Co-Sälj hänvisnings uppdateringar till CRM (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="20803-153">Partner Center Microsoft Co-sell Referral Updates to CRM (Insider Preview)</span></span>

4. <span data-ttu-id="20803-154">Vad bör du göra när du inte kan lägga till anslutningar i flödet när du försöker redigera flödet?</span><span class="sxs-lookup"><span data-stu-id="20803-154">What should you do when you aren't able to add connections to the flow when you try to edit the flow?</span></span>

<span data-ttu-id="20803-155">Du lägger till anslutningar till flödet när flödet körs och du lägger till varje flöde separat.</span><span class="sxs-lookup"><span data-stu-id="20803-155">You add connections to the flow while the flow is running, and you add to each flow separately.</span></span>  <span data-ttu-id="20803-156">Om dialog rutan för att lägga till anslutningar inte öppnas automatiskt när du redigerar flödet kan du redigera vart och ett av stegen och under stegen för flödena individuellt.</span><span class="sxs-lookup"><span data-stu-id="20803-156">If the dialog to add connections doesn't open up automatically while editing the flow, then you can edit each of the steps and sub steps of the flows individually.</span></span>

- <span data-ttu-id="20803-157">Välj varje flöde och redigera dem individuellt.</span><span class="sxs-lookup"><span data-stu-id="20803-157">Select each flow and edit them individually.</span></span>
- <span data-ttu-id="20803-158">Expandera alla steg i flödet</span><span class="sxs-lookup"><span data-stu-id="20803-158">Expand all the steps in the flow</span></span> 

:::image type="content" source="images/cosellconnectors/flowsteps.png" alt-text="Steg som behöver anslutningar":::

- <span data-ttu-id="20803-160">Välj de steg där du ser en varnings ikon som uppmanar dig att associera anslutningar och lägga till anslutningar.</span><span class="sxs-lookup"><span data-stu-id="20803-160">Select the steps where you see a warning icon asking to associate connections, and add connections.</span></span> 

:::image type="content" source="images/cosellconnectors/editflow.png" alt-text="Redigera flöde-steg per steg":::


5. <span data-ttu-id="20803-162">Vad ska jag göra om flödena för den samsälje referral Connector-lösningen inte aktive ras?</span><span class="sxs-lookup"><span data-stu-id="20803-162">What should you do if the flows of the Co-sell Referrals Connectors solution don’t turn on?</span></span>

<span data-ttu-id="20803-163">A.</span><span class="sxs-lookup"><span data-stu-id="20803-163">A.</span></span> <span data-ttu-id="20803-164">I energi spar läge måste du redigera flöden i följande ordning och uppdatera dem så att de använder rätt anslutningar:</span><span class="sxs-lookup"><span data-stu-id="20803-164">In Power Automate, you'll need to edit flows in the following order and update them to use the correct connections:</span></span>

- <span data-ttu-id="20803-165">Partner Center – registrering av webhook (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="20803-165">Partner Center Webhook Registration (Insider Preview)</span></span>
- <span data-ttu-id="20803-166">Skapa Co-sälje referral-Salesforce till Partner Center (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="20803-166">Create Co-sell Referral - Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="20803-167">Partner Center Microsoft Co-Sälj hänvisnings uppdateringar till Salesforce (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="20803-167">Partner Center Microsoft Co-sell Referral Updates to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="20803-168">Partner Center till Salesforce (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="20803-168">Partner Center to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="20803-169">Salesforce till Partner Center (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="20803-169">Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="20803-170">Salesforce-möjlighet till Partner Center (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="20803-170">Salesforce Opportunity to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="20803-171">Salesforce Microsoft-lösningar till Partner Center (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="20803-171">Salesforce Microsoft Solutions to Partner Center (Insider Preview)</span></span>

 <span data-ttu-id="20803-172">B.</span><span class="sxs-lookup"><span data-stu-id="20803-172">B.</span></span> <span data-ttu-id="20803-173">För varje flöde väljer du alternativet **Kör endast användare** .</span><span class="sxs-lookup"><span data-stu-id="20803-173">For each of flow, select **Run only users** option.</span></span> <span data-ttu-id="20803-174">Välj **Använd anslutning** i stället för att **tillhandahållas av endast körnings användare**.</span><span class="sxs-lookup"><span data-stu-id="20803-174">Select **Use connection** instead of **Provided by run-only user**.</span></span>  

:::image type="content" source="images/cosellconnectors/runonly.png" alt-text="Aktivera ett flöde":::


<span data-ttu-id="20803-176">C.</span><span class="sxs-lookup"><span data-stu-id="20803-176">C.</span></span> <span data-ttu-id="20803-177">Aktivera följande flöden:</span><span class="sxs-lookup"><span data-stu-id="20803-177">Activate these below mentioned flows:</span></span>

 - <span data-ttu-id="20803-178">Partner Center Microsoft Co-Sälj hänvisnings uppdateringar till Salesforce (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="20803-178">Partner Center Microsoft Co-sell Referral Updates to Salesforce (Insider Preview)</span></span>

- <span data-ttu-id="20803-179">Salesforce till Partner Center (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="20803-179">Salesforce to Partner Center (Insider Preview)</span></span>

    
<span data-ttu-id="20803-180">D.</span><span class="sxs-lookup"><span data-stu-id="20803-180">D.</span></span> <span data-ttu-id="20803-181">Aktivera alla återstående flöden.</span><span class="sxs-lookup"><span data-stu-id="20803-181">Activate all the remaining flows.</span></span>

<span data-ttu-id="20803-182">E.</span><span class="sxs-lookup"><span data-stu-id="20803-182">E.</span></span> <span data-ttu-id="20803-183">I Flow Partner Center-webhook-registrering väljer du **Kör**.</span><span class="sxs-lookup"><span data-stu-id="20803-183">At flow Partner Center Webhook Registration, select **Run**.</span></span> <span data-ttu-id="20803-184">Ange **http-URL:** en från den första åtgärden i **partner Center till Salesforce** -flöde.</span><span class="sxs-lookup"><span data-stu-id="20803-184">Provide the **http url** from the first action in **Partner Center to Salesforce** flow.</span></span> <span data-ttu-id="20803-185">Välj alla fyra alternativen under **händelser som ska registreras** och välj **Ja** för Skriv över.</span><span class="sxs-lookup"><span data-stu-id="20803-185">Select all four options under **Events to register** and select **yes** for Overwrite.</span></span>

## <a name="questions-and-answers-about-runmaintenance"></a><span data-ttu-id="20803-186">Frågor och svar om körning/underhåll</span><span class="sxs-lookup"><span data-stu-id="20803-186">Questions and answers about Run/Maintenance</span></span>

1. <span data-ttu-id="20803-187">Hur felsöker jag om fel uppstår under automatisk flödes körning?</span><span class="sxs-lookup"><span data-stu-id="20803-187">How do you troubleshoot in case of failures during Power Automate flow execution?</span></span>

<span data-ttu-id="20803-188">För att se till att dina energi scheman körs som du förväntar dig och Felsök fel under körningen, se [åtgärda flödes fel](/power-automate/fix-flow-failures).</span><span class="sxs-lookup"><span data-stu-id="20803-188">To ensure that your Power Automate flows run as you expect and to troubleshoot failures during execution, refer to [Fix flow failures](/power-automate/fix-flow-failures).</span></span>

2. <span data-ttu-id="20803-189">Vad bör du göra om du ser referenser som inte har synkroniserats korrekt i Partner Center eller i en CRM-miljö?</span><span class="sxs-lookup"><span data-stu-id="20803-189">What should you do if you see referrals that aren't synchronized properly in Partner Center or CRM environment?</span></span>
 
<span data-ttu-id="20803-190">Välj **granskning** för att fastställa status för referens synkroniseringen.</span><span class="sxs-lookup"><span data-stu-id="20803-190">To determine the status of referral synchronization, select **Audit**.</span></span> 

:::image type="content" source="images/cosellconnectors/synch.png" alt-text="Så här synkroniserar du referenser":::

<span data-ttu-id="20803-192">Se till att följande villkor är uppfyllda:</span><span class="sxs-lookup"><span data-stu-id="20803-192">Ensure that the following conditions are met:</span></span>

- <span data-ttu-id="20803-193">Lösnings-ID tillhandahålls som en del av affärs möjligheten.</span><span class="sxs-lookup"><span data-stu-id="20803-193">Solution ID is provided as part of the opportunity.</span></span>

- <span data-ttu-id="20803-194">Landskod för två bokstäver måste anges.</span><span class="sxs-lookup"><span data-stu-id="20803-194">Two letter country code is required.</span></span>

- <span data-ttu-id="20803-195">När hjälp från Microsoft väljs för affärs möjligheten krävs kundens kontakt uppgifter.</span><span class="sxs-lookup"><span data-stu-id="20803-195">When help from Microsoft is selected for the opportunity, customer contact information is required.</span></span>

3. <span data-ttu-id="20803-196">Hur ser du till att en hänvisning synkroniseras i dubbelriktad riktning?</span><span class="sxs-lookup"><span data-stu-id="20803-196">How to ensure that a referral will synchronize bi-directionally?</span></span>

<span data-ttu-id="20803-197">Gör så här:</span><span class="sxs-lookup"><span data-stu-id="20803-197">Do the following steps:</span></span>

- <span data-ttu-id="20803-198">Partner leverantörer måste se till att de har aktiverat alternativet **Synkronisera med alternativet för partner Center** i avsnittet CRM.</span><span class="sxs-lookup"><span data-stu-id="20803-198">Partner sellers need to ensure that they have enabled **Sync with Partner Center** option in the CRM section.</span></span>

:::image type="content" source="images/cosellconnectors/enablesynch.png" alt-text="Se till att du har aktiverat Synch":::

- <span data-ttu-id="20803-200">Säljare måste ange intäkter och UB-datum när de kvalificerar sig för ett lead.</span><span class="sxs-lookup"><span data-stu-id="20803-200">Sellers need to provide revenue and closing date when qualifying a lead.</span></span>

- <span data-ttu-id="20803-201">Om CRM-ID: t anges i steget **skapa** eller **Uppdatera** stadium av samförsäljning, men det inte gick att hitta en lead-möjlighet med detta ID i CRM, så ignoreras uppdatering eller skapande.</span><span class="sxs-lookup"><span data-stu-id="20803-201">If CRM ID is provided in the **create** or **update** stage of co-sell opportunity, but a lead opportunity with that ID is not found in CRM, then update or create will be ignored.</span></span>

- <span data-ttu-id="20803-202">Se till att fältet hänvisnings valuta har kon figurer ATS i Salesforce-miljö.</span><span class="sxs-lookup"><span data-stu-id="20803-202">Ensure that referral currency field is configured on Salesforce environment.</span></span> 

4. <span data-ttu-id="20803-203">Vad gör du om anslutningen kopplas från och du saknar en referens synkronisering.</span><span class="sxs-lookup"><span data-stu-id="20803-203">What should you do if the connector gets disconnected and you miss a referral synchronization.</span></span> 

<span data-ttu-id="20803-204">Nedan följer några av de alternativ som du kan prova:</span><span class="sxs-lookup"><span data-stu-id="20803-204">Following are few of the options that you can try out:</span></span>

- <span data-ttu-id="20803-205">Kontrol lera om användar namnet eller lösen ordet har upphört att gälla för partner Center-användaren med referens administratörs roller.</span><span class="sxs-lookup"><span data-stu-id="20803-205">Check whether username or password has expired for the Partner Center user with referral admin roles.</span></span>

- <span data-ttu-id="20803-206">Du kan gå till den icke-synkroniserade möjligheten, göra en mindre uppdatering och kontrol lera om hänvisningen har synkroniserats.</span><span class="sxs-lookup"><span data-stu-id="20803-206">You can go to the un-synchronized opportunity, make a minor update, and observe whether the referral has synchronized.</span></span>

- <span data-ttu-id="20803-207">Om flödena har körts och misslyckats väljer du flödet och skickar om körningen som har misslyckats.</span><span class="sxs-lookup"><span data-stu-id="20803-207">If the flows have run and failed, then select the flow and re-submit the run which has failed.</span></span>

5. <span data-ttu-id="20803-208">Vad bör du göra när du får åtkomst nekade fel?</span><span class="sxs-lookup"><span data-stu-id="20803-208">What should you do when you get access denied errors?</span></span>

<span data-ttu-id="20803-209">Kontrol lera att rätt roller finns</span><span class="sxs-lookup"><span data-stu-id="20803-209">Make sure the appropriate roles exist</span></span>

- <span data-ttu-id="20803-210">Referens administratörs roll för partner Center-säljaren</span><span class="sxs-lookup"><span data-stu-id="20803-210">Referral Administrator role for Partner Center seller</span></span> 
 
- <span data-ttu-id="20803-211">Rollen system administratör eller systemanpassare på din CRM-instans</span><span class="sxs-lookup"><span data-stu-id="20803-211">System Administrator or System Customizer role on your CRM instance</span></span>

- <span data-ttu-id="20803-212">Se till att energischemat flödes konto användare loggar in https://flow.microsoft.com minst en gång på förhand</span><span class="sxs-lookup"><span data-stu-id="20803-212">Ensure that the Power Automate flow account user logs into https://flow.microsoft.com at least once beforehand</span></span>

6. <span data-ttu-id="20803-213">Vad gör du om du ser att **land koden för kund kontot** saknas när du skapar en samförsäljnings möjlighet?</span><span class="sxs-lookup"><span data-stu-id="20803-213">If you see that **Customer account country code** is missing while creating a Co-sell opportunity, what should you do?</span></span>

<span data-ttu-id="20803-214">Du måste lägga till ISO-koden med två bokstäver till kund kontot i CRM.</span><span class="sxs-lookup"><span data-stu-id="20803-214">You will need to add the ISO two-letter country code to the Customer account in CRM.</span></span>

7. <span data-ttu-id="20803-215">Vad bör du göra om du ser felet att **lösnings-ID krävs** när du skapar en samförsäljnings möjlighet?</span><span class="sxs-lookup"><span data-stu-id="20803-215">What should you do if you see the error that **Solution ID is required** while creating a Co-sell opportunity?</span></span>

<span data-ttu-id="20803-216">För att kunna skapa en samförsäljnings hänvisning behöver du en Microsoft Co-försäljnings klar lösning.</span><span class="sxs-lookup"><span data-stu-id="20803-216">In order to create a co-sell referral, you need a Microsoft co-sell ready solution.</span></span> 

8. <span data-ttu-id="20803-217">Vad bör du göra när du ser samförsäljnings möjligheter som skapats i Partner Center som inte synkroniseras till CRM trots att det inte finns några Flow-fel:</span><span class="sxs-lookup"><span data-stu-id="20803-217">What should you do when you see Co-sell opportunities created in Partner Center that aren't synchronized to CRM even though there are no flow errors:</span></span>

<span data-ttu-id="20803-218">Gör följande:</span><span class="sxs-lookup"><span data-stu-id="20803-218">Do the following:</span></span>

- <span data-ttu-id="20803-219">När du har skapat en ny co-sälje-affär i Partner Center kontrollerar du om Partner Center till Dynamics 365 Flow anropas (det kan komma att anropas flera gånger).</span><span class="sxs-lookup"><span data-stu-id="20803-219">After you have created a new co-sell deal in Partner Center, check if Partner Center to Dynamics 365 flow gets invoked (it might get invoked multiple times).</span></span>

- <span data-ttu-id="20803-220">Om flödet anropas kontrollerar du alla anropade flöden och identifierar körningen av flödet som uppdaterar CRM.</span><span class="sxs-lookup"><span data-stu-id="20803-220">If the flow gets invoked, check all invoked flows, and identify the flow run which would update the CRM.</span></span> <span data-ttu-id="20803-221">Du kan följa instruktionerna och kontrol lera om det har uppdaterats i CRM eller ett problem har uppstått.</span><span class="sxs-lookup"><span data-stu-id="20803-221">You can follow the actions and verify if it did update the CRM or encountered a problem.</span></span>

- <span data-ttu-id="20803-222">Titta på *nytt erbjudande*\* i Partner Center för att se om det fylls med CRM-ID.</span><span class="sxs-lookup"><span data-stu-id="20803-222">Check *New deal*\* in Partner Center to see if it gets populated with CRM ID.</span></span>

- <span data-ttu-id="20803-223">Se till att affären inte stängs av misstag som "vunnen" eller "förlorad" i Partner Center.</span><span class="sxs-lookup"><span data-stu-id="20803-223">Make sure that the deal is not accidentally closed as “Won” or “Lost” in Partner Center.</span></span>

## <a name="next-steps"></a><span data-ttu-id="20803-224">Nästa steg</span><span class="sxs-lookup"><span data-stu-id="20803-224">Next steps</span></span>

- [<span data-ttu-id="20803-225">Hantera leads</span><span class="sxs-lookup"><span data-stu-id="20803-225">Manage leads</span></span>](manage-leads.md)
 
- [<span data-ttu-id="20803-226">Hantera möjligheter till samförsäljning</span><span class="sxs-lookup"><span data-stu-id="20803-226">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)
