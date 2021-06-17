---
title: CSP regional auktorisering klientkonsolidering
ms.topic: how-to
ms.date: 07/15/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Använd de här instruktionerna för att konsolidera klienter för olika länder/regioner. Detta omfattar steg för att migrera kundkonton och kundprenumerationer.
author: billLinzbach
ms.author: billLi
ms.localizationpriority: medium
robots: noindex,nofollow
ms.custom: SEOMAY.20
ms.openlocfilehash: 84e5f7f2674e9b2f3c3c26ed2ea49f9bba0e96e0
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/17/2021
ms.locfileid: "112276883"
---
# <a name="instructions-for-csp-regional-authorization-tenant-consolidation"></a><span data-ttu-id="2ed79-104">Instruktioner för CSP-auktorisering för konsolidering av klientorganisationer</span><span class="sxs-lookup"><span data-stu-id="2ed79-104">Instructions for CSP regional authorization tenant consolidation</span></span>

<span data-ttu-id="2ed79-105">**Gäller för**: Partner Center-| Partnercenter för Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="2ed79-105">**Applies to**: Partner Center | Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="2ed79-106">**Lämpliga roller:** Global | Administratörsagent</span><span class="sxs-lookup"><span data-stu-id="2ed79-106">**Appropriate roles**: Global admin | Admin agent</span></span>

<span data-ttu-id="2ed79-107">\[En del information gäller för frisläppt produkt som kan ändras avsevärt innan den släpps kommersiellt.</span><span class="sxs-lookup"><span data-stu-id="2ed79-107">\[Some information relates to pre-released product which may be substantially modified before it's commercially released.</span></span> <span data-ttu-id="2ed79-108">Microsoft lämnar inga garantier, uttryckliga eller underförstådda, avseende informationen som visas här.\]</span><span class="sxs-lookup"><span data-stu-id="2ed79-108">Microsoft makes no warranties, express or implied, with respect to the information provided here.\]</span></span>

<span data-ttu-id="2ed79-109">Du kan konsolidera klienter för din verksamhet.</span><span class="sxs-lookup"><span data-stu-id="2ed79-109">You can consolidate tenants for your business.</span></span> <span data-ttu-id="2ed79-110">Använd de här instruktionerna för att konsolidera klienter för olika länder/regioner.</span><span class="sxs-lookup"><span data-stu-id="2ed79-110">Use these instructions to consolidate tenants for different country/regions.</span></span>

>[!NOTE]  
><span data-ttu-id="2ed79-111">Du måste vara medveten om alla etablerade prenumerationer och licensantal för var och en av dina kunder i det konto som du övergår från.</span><span class="sxs-lookup"><span data-stu-id="2ed79-111">You must be aware of all of the provisioned subscriptions and license counts for each of your customers in the account you are transitioning from.</span></span> <span data-ttu-id="2ed79-112">Du kommer att ometablering av samma exakta prenumerationer med samma licensantal under det nya centrala CSP-kontot som en del av migreringsprocessen.</span><span class="sxs-lookup"><span data-stu-id="2ed79-112">You will be re-provisioning those same exact subscriptions with the same license counts under the new central CSP account as part of the migration process.</span></span> <span data-ttu-id="2ed79-113">Använd exportlistefunktionen för att skapa en lista över kunder som ska flyttas över till den centraliserade klientorganisationen.</span><span class="sxs-lookup"><span data-stu-id="2ed79-113">Use the export list feature to help create a list of customers to move over to the centralized tenant.</span></span>  <span data-ttu-id="2ed79-114">När konsolideringen är klar kan du inte återgå till det tidigare klienttillståndet.</span><span class="sxs-lookup"><span data-stu-id="2ed79-114">Once consolidation is complete, you can't revert to the previous tenant state.</span></span> <span data-ttu-id="2ed79-115">Kundåtgärd kan också krävas.</span><span class="sxs-lookup"><span data-stu-id="2ed79-115">Customer action may also be required.</span></span>

## <a name="prepare-for-migration"></a><span data-ttu-id="2ed79-116">Förbereda för migrering</span><span class="sxs-lookup"><span data-stu-id="2ed79-116">Prepare for migration</span></span>

- <span data-ttu-id="2ed79-117">Logga in på **Partnercenter** med övergångskontot (det som du kommer att övergå till det nya kontot) och granska alla kunder och alla tjänster som etablerats för dessa kunder. </span><span class="sxs-lookup"><span data-stu-id="2ed79-117">Sign in to **Partner Center**  using the **Transitioning** account (the one you will transition to the new account), and review of all customers and all of the services provisioned for those customers.</span></span>

- <span data-ttu-id="2ed79-118">Logga ut från det här kontot.</span><span class="sxs-lookup"><span data-stu-id="2ed79-118">Sign out of this account.</span></span>

## <a name="migrate-customer-accounts"></a><span data-ttu-id="2ed79-119">Migrera kundkonton</span><span class="sxs-lookup"><span data-stu-id="2ed79-119">Migrate customer accounts</span></span>

1. <span data-ttu-id="2ed79-120">Logga in på **Partnercenter**  med **övergångskontot** (nytt) (det som du övergår kunder till).</span><span class="sxs-lookup"><span data-stu-id="2ed79-120">Sign in to **Partner Center**  with the **Transitioning** (new) account (the one you are transitioning customers into).</span></span>

2. <span data-ttu-id="2ed79-121">Välj **Kunder**.</span><span class="sxs-lookup"><span data-stu-id="2ed79-121">Select **Customers**.</span></span>

3. <span data-ttu-id="2ed79-122">Välj **Begär en återförsäljarrelation**.</span><span class="sxs-lookup"><span data-stu-id="2ed79-122">Select **Request a reseller relationship**.</span></span> <span data-ttu-id="2ed79-123">Du får ett standardmeddelande som du kan skicka till dina kunder.</span><span class="sxs-lookup"><span data-stu-id="2ed79-123">You are presented with a default email message to send to your customers.</span></span> <span data-ttu-id="2ed79-124">Det här meddelandet innehåller en URL med organisations-ID:t som är unikt för ditt nya Partnercenter-konto.</span><span class="sxs-lookup"><span data-stu-id="2ed79-124">This message contains a URL with the org ID unique to your new Partner Center account.</span></span>

4. <span data-ttu-id="2ed79-125">**Kundåtgärd:** Se till att var och en av de aktiva kunder som du vill migrera besöker denna URL.</span><span class="sxs-lookup"><span data-stu-id="2ed79-125">**Customer Action:** Ensure that each of the active customers you want to migrate visits this URL.</span></span> <span data-ttu-id="2ed79-126">När du öppnar URL:en uppmanas kunden att logga in på Office 365-portalen.</span><span class="sxs-lookup"><span data-stu-id="2ed79-126">When opening the URL, the customer is prompted to sign in to the Office 365 portal.</span></span> <span data-ttu-id="2ed79-127">Kunden loggar in med samma organisations-ID som de använder för att få åtkomst till Azure- och Office 365-administratörsportalerna.</span><span class="sxs-lookup"><span data-stu-id="2ed79-127">The customer signs in using the same Org ID that they use to access the Azure and Office 365 admin portals.</span></span>

5. <span data-ttu-id="2ed79-128">När du har loggat  in uppmanas den globala administratören för kundkontot att skicka ett avtal som ger delegerade administratörsbehörigheter till det nya CSP-kontot.</span><span class="sxs-lookup"><span data-stu-id="2ed79-128">After signing in, the Global Admin for the **customer account** is prompted to submit an agreement that gives delegated admin privileges to the new CSP account.</span></span> <span data-ttu-id="2ed79-129">Om kunden accepterar markerar kunden kryssrutan och godkänner att relationen godkänns.</span><span class="sxs-lookup"><span data-stu-id="2ed79-129">If they agree, the customer selects the checkbox and agrees to authorize the relationship.</span></span>

<span data-ttu-id="2ed79-130">Kunderna visas i partnerns kundlista när de har skickat avtalet, en i rad.</span><span class="sxs-lookup"><span data-stu-id="2ed79-130">The customers will appear in the partner's customer list after they have submitted the agreement, one by one.</span></span>

## <a name="migrating-office-365-and-non-azure-usage-based-subscriptions"></a><span data-ttu-id="2ed79-131">Migrera office 365- och icke-Azure-användningsbaserade prenumerationer</span><span class="sxs-lookup"><span data-stu-id="2ed79-131">Migrating Office 365 and non-Azure usage-based subscriptions</span></span>

1. <span data-ttu-id="2ed79-132">När kunden har signerat avtalet kan du återskapa deras prenumerationer under din centraliserade partnerklientorganisation.</span><span class="sxs-lookup"><span data-stu-id="2ed79-132">Once your customer has signed the agreement, you can recreate their subscriptions under your Centralized Partner Tenant.</span></span>

2. <span data-ttu-id="2ed79-133">Från **Partnercenter** väljer du **Kunder.**</span><span class="sxs-lookup"><span data-stu-id="2ed79-133">From **Partner Center**, select **Customers**.</span></span>

3. <span data-ttu-id="2ed79-134">Öppna företagsnamnet för den kund som du vill migrera.</span><span class="sxs-lookup"><span data-stu-id="2ed79-134">Open the company name for the customer you want to migrate.</span></span>

4. <span data-ttu-id="2ed79-135">Välj **Lägg till prenumeration.**</span><span class="sxs-lookup"><span data-stu-id="2ed79-135">Select **Add subscription**.</span></span>

5. <span data-ttu-id="2ed79-136">Lägg till rätt prenumerationer och licensantal från katalogen.</span><span class="sxs-lookup"><span data-stu-id="2ed79-136">Add the correct subscriptions and license counts from the catalog.</span></span> <span data-ttu-id="2ed79-137">Kontrollera med informationen som anges i **Övergång från** partnerkonton.</span><span class="sxs-lookup"><span data-stu-id="2ed79-137">Verify with the information provided in the **Transitioning From** partner accounts.</span></span>

   :::image type="content" source="images/regionalcustomer2.png" alt-text="kundlista.":::

6. <span data-ttu-id="2ed79-139">Välj **Skicka.**</span><span class="sxs-lookup"><span data-stu-id="2ed79-139">Select **Submit.**</span></span>

   <span data-ttu-id="2ed79-140">Tjänsterna tillhandahålls nu till kunden från **övergångskontot till** partnerkontot.</span><span class="sxs-lookup"><span data-stu-id="2ed79-140">The services are now provided to the customer from the **Transitioning To** partner account.</span></span>

7. <span data-ttu-id="2ed79-141">Upprepa de här stegen för att migrera prenumerationer för alla ytterligare kunder.</span><span class="sxs-lookup"><span data-stu-id="2ed79-141">Repeat these steps to migrate subscriptions for all additional customers.</span></span>

<span data-ttu-id="2ed79-142">Innan du fortsätter till nästa avsnitt ser du till att alla kundprenumerationer som finns under Övergångs från **partnerkonton** etableras på nytt under **övergångskontot till** partnerkontot.</span><span class="sxs-lookup"><span data-stu-id="2ed79-142">Before proceeding to the next section, ensure all customer subscriptions existing under the **Transitioning From** partner accounts are re-provisioned under the **Transitioning To** partner account.</span></span>

> [!NOTE]
> <span data-ttu-id="2ed79-143">Partner måste inaktivera  prenumerationer på kontot för övergång från partnerklientorganisation i Partnercenter samma dag som prenumerationerna övergår och konfigureras under övergångskontot till **partnerklientorganisationen** i Partnercenter för att säkerställa att dubbel fakturering inte sker.</span><span class="sxs-lookup"><span data-stu-id="2ed79-143">Partners must suspend subscriptions on the **Transitioning From** Partner Tenant account in Partner Center the same day that those subscriptions are transitioned and set up under the **Transitioning To** Partner Tenant account in the Partner Center to ensure double billing does not occur.</span></span> <span data-ttu-id="2ed79-144">Supportbegäranden nekas för krediter på grund av eventuell överlappning i faktureringen som inträffar när övergången från prenumerationer **inte inaktiveras** korrekt.</span><span class="sxs-lookup"><span data-stu-id="2ed79-144">Support requests will be denied for credits due to any overlap in billing that occurs from not correctly disabling the **Transitioning From** subscriptions.</span></span>

## <a name="disabling-the-office-365-subscriptions-under-the-transitioning-from-partner-account"></a><span data-ttu-id="2ed79-145">Inaktivera Office 365-prenumerationer under övergångskontot från partner</span><span class="sxs-lookup"><span data-stu-id="2ed79-145">Disabling the Office 365 subscriptions under the Transitioning From partner account</span></span>

<span data-ttu-id="2ed79-146">Om du inaktiverar CSP-prenumerationen under **övergången från** partnerkonton stoppas eventuell framtida fakturering.</span><span class="sxs-lookup"><span data-stu-id="2ed79-146">Disabling the CSP subscription under the **Transitioning From** partner accounts stops any future billing.</span></span> <span data-ttu-id="2ed79-147">Du behöver inte inaktivera Azure-prenumerationer manuellt eftersom Azure-prenumerationer inaktiveras automatiskt under migreringsprocessen.</span><span class="sxs-lookup"><span data-stu-id="2ed79-147">You don't have to manually disable Azure subscriptions, because Azure subscriptions are automatically disabled during the migration process.</span></span>

1. <span data-ttu-id="2ed79-148">Logga in på **Partnercenter med** **övergångskontot från** CSP och gå till kundlistan.</span><span class="sxs-lookup"><span data-stu-id="2ed79-148">Sign in to the **Partner Center** with the **Transitioning From** CSP account and navigate to the customer list.</span></span>

2. <span data-ttu-id="2ed79-149">Öppna kunden med prenumerationer att inaktivera och välj sedan det första erbjudandet att inaktivera.</span><span class="sxs-lookup"><span data-stu-id="2ed79-149">Open the customer with subscriptions to disable, and then select the first offer to disable.</span></span>

3. <span data-ttu-id="2ed79-150">Ställ in prenumerationen **på pausad** och välj **sedan Skicka**.</span><span class="sxs-lookup"><span data-stu-id="2ed79-150">Set the subscription to **suspended**, and then select **submit**.</span></span>

   >[!Note]
   ><span data-ttu-id="2ed79-151">Om du pausar prenumerationen säkerställer du att dubbel fakturering inte sker.</span><span class="sxs-lookup"><span data-stu-id="2ed79-151">Suspending the subscription ensures double billing does not occur.</span></span>

   <span data-ttu-id="2ed79-152">Prenumerationen visas **som inaktiverad** i prenumerationslistan.</span><span class="sxs-lookup"><span data-stu-id="2ed79-152">The subscription shows **suspended** on the subscriptions list.</span></span>

4. <span data-ttu-id="2ed79-153">Upprepa dessa steg för alla prenumerationer under kunden.</span><span class="sxs-lookup"><span data-stu-id="2ed79-153">Repeat these steps for all subscriptions under the customer.</span></span> <span data-ttu-id="2ed79-154">Kontrollera att alla visas som **pausade.**</span><span class="sxs-lookup"><span data-stu-id="2ed79-154">Verify all show **suspended.**</span></span>

5. <span data-ttu-id="2ed79-155">Välj nästa kund i listan och upprepa processen för att inaktivera alla prenumerationer.</span><span class="sxs-lookup"><span data-stu-id="2ed79-155">Select the next customer on the list and repeat the process of disabling all subscriptions.</span></span>

## <a name="migrating-azure-usage-based-subscriptions"></a><span data-ttu-id="2ed79-156">Migrera azure-användningsbaserade prenumerationer</span><span class="sxs-lookup"><span data-stu-id="2ed79-156">Migrating Azure usage-based subscriptions</span></span>

<span data-ttu-id="2ed79-157">Till skillnad från Office 365 CSP-prenumerationer behöver inte användningsbaserade CSP-prenumerationer migreras manuellt i Azure.</span><span class="sxs-lookup"><span data-stu-id="2ed79-157">Unlike the Office 365 CSP subscriptions, Azure, usage-based CSP subscriptions do not need to be migrated manually.</span></span> <span data-ttu-id="2ed79-158">Microsoft Azure-supporten migrerar Azure-prenumerationerna och alla distribuerade  tjänster eller resurser från övergångskontot från CSP-återförsäljare till kontot för övergång till CSP-återförsäljare. </span><span class="sxs-lookup"><span data-stu-id="2ed79-158">Microsoft Azure Support will migrate the Azure subscriptions and all deployed services or resources from the **Transitioning From** CSP reseller accounts to the **Transitioning To** CSP reseller account.</span></span> <span data-ttu-id="2ed79-159">Det kommer inte att ske några avbrott i tjänsten för kunden under den här övergången.</span><span class="sxs-lookup"><span data-stu-id="2ed79-159">There will be no disruption of service to the customer during this transition.</span></span>

1. <span data-ttu-id="2ed79-160">Se till att de kundkonton som kommer att ha Azure-prenumerationer migrerade har godkänt avtalet för att associeras med det nya **övergångskontot till** CSP.</span><span class="sxs-lookup"><span data-stu-id="2ed79-160">Ensure that the customer accounts that will have Azure subscriptions migrated have accepted the agreement to be associated with the new **Transitioning To** CSP account.</span></span>

2. <span data-ttu-id="2ed79-161">Du meddelar Microsoft vilka kundkonton som är redo att migreras och anger kundens företagsnamn.</span><span class="sxs-lookup"><span data-stu-id="2ed79-161">You will notify Microsoft of which customer accounts are ready to migrate, and provide those customer's company names.</span></span>

3. <span data-ttu-id="2ed79-162">Microsoft migrerar azure-användningsbaserade prenumerationer och meddelar dig när migreringen är klar.</span><span class="sxs-lookup"><span data-stu-id="2ed79-162">Microsoft migrates the Azure usage-based subscriptions and notifies you when the migration is complete.</span></span>

4. <span data-ttu-id="2ed79-163">Du måste bekräfta att Azure-prenumerationen under kontot för övergång  från  CSP-återförsäljare nu har markerats som inaktiverat i Partnercenter under avsnittet kundprenumerationer.</span><span class="sxs-lookup"><span data-stu-id="2ed79-163">You need to confirm that the Azure subscription under the **Transitioning From** CSP reseller account now is marked **suspended** in Partner Center under the customer subscriptions section.</span></span>

5. <span data-ttu-id="2ed79-164">Bekräfta att Azure-prenumerationen under **kontot för övergång** till  CSP-återförsäljare nu visar statusen aktiv i Partnercenter under avsnittet kundprenumerationer.</span><span class="sxs-lookup"><span data-stu-id="2ed79-164">Confirm that the Azure subscription under the **Transitioning To** CSP reseller account now shows a status of **active** in Partner Center under the customer subscriptions section.</span></span>

   >[!Note]
   > <span data-ttu-id="2ed79-165">Om du inaktiverar prenumerationerna under kunden ändras inte utseendet på kunden i kundlistan.</span><span class="sxs-lookup"><span data-stu-id="2ed79-165">Disabling the subscriptions under the customer does not change the appearance of the customer in the Customers list.</span></span> <span data-ttu-id="2ed79-166">Det finns för närvarande inget alternativ för att ta bort kunder från listan.</span><span class="sxs-lookup"><span data-stu-id="2ed79-166">There is currently no option to remove customers from the list.</span></span> <span data-ttu-id="2ed79-167">Partner bör undvika att lägga till prenumerationer till dessa kunder från **övergången från** konto i framtiden.</span><span class="sxs-lookup"><span data-stu-id="2ed79-167">Partners should avoid adding subscriptions back to these customers from their **Transitioning From** account in the future.</span></span>

6. <span data-ttu-id="2ed79-168">Upprepa de här stegen för alla prenumerationer under alla dina kunder för att stoppa framtida avgifter för **övergång från** konto.</span><span class="sxs-lookup"><span data-stu-id="2ed79-168">Repeat these steps for all subscriptions under all of your customers to stop future charges on the **Transitioning From** account(s).</span></span> <span data-ttu-id="2ed79-169">Partnern får en slutlig faktura med en kredit för antalet oanvända dagar mellan annulleringsdagen och den sista dagen i faktureringsperioden.</span><span class="sxs-lookup"><span data-stu-id="2ed79-169">The partner will receive one final invoice with a credit for the number of unused days between the day of cancellation and the last day of the billing period.</span></span> <span data-ttu-id="2ed79-170">Inga framtida fakturor genereras efter den sista faktureringsperioden.</span><span class="sxs-lookup"><span data-stu-id="2ed79-170">No future invoices will generate after that final billing period.</span></span>

### <a name="additional-information"></a><span data-ttu-id="2ed79-171">Ytterligare information</span><span class="sxs-lookup"><span data-stu-id="2ed79-171">Additional information</span></span>

- <span data-ttu-id="2ed79-172">Om du inaktiverar prenumerationen från kontot för övergång från **CSP** påverkas inte slutanvändarens tjänst så länge tjänsten etablerades från övergångskontot till **CSP** innan prenumerationen inaktiverades.</span><span class="sxs-lookup"><span data-stu-id="2ed79-172">Disabling the subscription from the **Transitioning From** CSP account does not impact end customer's service as long as the service was provisioned from the **Transitioning To** CSP account prior to disabling the subscription.</span></span>

- <span data-ttu-id="2ed79-173">Prenumerationer kan inte användas av kunden och genererar inte avgifter när de pausas eller avbryts.</span><span class="sxs-lookup"><span data-stu-id="2ed79-173">Subscriptions cannot be used by the customer and do not generate charges when suspended or canceled.</span></span>

- <span data-ttu-id="2ed79-174">Det finns för närvarande inget sätt att ta bort en kund helt från **kundlistan.**</span><span class="sxs-lookup"><span data-stu-id="2ed79-174">There is currently no way to remove a customer completely from the **Customers** list.</span></span>
- 
    >[!Note]
    > <span data-ttu-id="2ed79-175">Partner måste inaktivera prenumerationer på kontot för övergång från **partnerklientorganisation** i Partnercenter samma  dag som prenumerationerna övergår till och konfigureras under övergångskontot för att säkerställa att dubbel fakturering inte sker.</span><span class="sxs-lookup"><span data-stu-id="2ed79-175">Partners must suspend subscriptions on the **Transitioning From** partner tenant account in Partner Center the same day those subscriptions are transitioned to and set up under the **Transitioning To** account to ensure double billing does not occur.</span></span> <span data-ttu-id="2ed79-176">Microsoft kommer inte att stödja begäranden om krediter på grund av överlappande fakturering som inträffar från att inte korrekt ställa in övergången **från** prenumerationer till pausad.</span><span class="sxs-lookup"><span data-stu-id="2ed79-176">Microsoft will not support requests for credits due to any overlap in billing that occurs from not correctly setting the **Transitioning From** subscriptions to suspended.</span></span>

### <a name="simplify-migration-using-export"></a><span data-ttu-id="2ed79-177">Förenkla migrering med export</span><span class="sxs-lookup"><span data-stu-id="2ed79-177">Simplify migration using Export</span></span>

<span data-ttu-id="2ed79-178">Med hjälp **av exportfunktionen** kan du avbilda de prenumerationer som du behöver använda i din nya konsoliderade struktur:</span><span class="sxs-lookup"><span data-stu-id="2ed79-178">Using the **Export Function**, you can capture the subscriptions you need to use in your new consolidated structure:</span></span>

1. <span data-ttu-id="2ed79-179">Välj **Kunder** i Partnercenter för att se listan över kunder.</span><span class="sxs-lookup"><span data-stu-id="2ed79-179">Select **Customers** on Partner Center to see the list of customers.</span></span> 

2. <span data-ttu-id="2ed79-180">Öppna önskat kundnamn.</span><span class="sxs-lookup"><span data-stu-id="2ed79-180">Open the desired customer name.</span></span>

3. <span data-ttu-id="2ed79-181">På sidan **Prenumerationer väljer** du Exportera **prenumerationer för** att exportera information om prenumerationer till en Excel-fil.</span><span class="sxs-lookup"><span data-stu-id="2ed79-181">On the **Subscriptions** page, select **Export Subscriptions** to export details of subscriptions to an Excel file.</span></span>

4. <span data-ttu-id="2ed79-182">Använd den här listan för att återskapa prenumerationerna i din nya konsoliderade klientorganisation.</span><span class="sxs-lookup"><span data-stu-id="2ed79-182">Use this list to recreate the subscriptions in your new consolidated tenant.</span></span>

### <a name="api-registration"></a><span data-ttu-id="2ed79-183">API-registrering</span><span class="sxs-lookup"><span data-stu-id="2ed79-183">API registration</span></span>

<span data-ttu-id="2ed79-184">Mer information om API-registrering finns i [Konfigurera API-åtkomst i Partnercenter.](/partner-center/develop/set-up-api-access-in-partner-center)</span><span class="sxs-lookup"><span data-stu-id="2ed79-184">For more information about API registration, see [Set up API access in Partner Center](/partner-center/develop/set-up-api-access-in-partner-center).</span></span>

## <a name="next-steps"></a><span data-ttu-id="2ed79-185">Nästa steg</span><span class="sxs-lookup"><span data-stu-id="2ed79-185">Next steps</span></span>

- [<span data-ttu-id="2ed79-186">Molnlösningsleverantör program regionala marknader och valutor där du kan sälja CSP-erbjudanden</span><span class="sxs-lookup"><span data-stu-id="2ed79-186">Cloud Solution Provider program regional markets and currencies where you can sell CSP offers</span></span>](regional-authorization-overview.md)
