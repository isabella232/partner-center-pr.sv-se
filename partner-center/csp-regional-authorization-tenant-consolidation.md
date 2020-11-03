---
title: CSP regional auktorisering av klient konsolidering
ms.topic: how-to
ms.date: 07/15/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Använd de här anvisningarna för att konsolidera klienter för olika länder/regioner. Detta inkluderar steg för att migrera kund konton och kund prenumerationer.
author: billLinzbach
ms.author: billLi
ms.localizationpriority: medium
robots: noindex,nofollow
ms.custom: SEOMAY.20
ms.openlocfilehash: 0ae107c005eaf6b8ff8a6d99a91075ebc560cf81
ms.sourcegitcommit: 940dad4527f51781f6f966e196b3aa08389613a2
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 10/13/2020
ms.locfileid: "92531853"
---
# <a name="instructions-for-csp-regional-authorization-tenant-consolidation"></a><span data-ttu-id="72c71-104">Instruktioner för CSP regional auktorisering av klient organisations konsolidering</span><span class="sxs-lookup"><span data-stu-id="72c71-104">Instructions for CSP regional authorization tenant consolidation</span></span>

<span data-ttu-id="72c71-105">**Gäller för**</span><span class="sxs-lookup"><span data-stu-id="72c71-105">**Applies to**</span></span>

-  <span data-ttu-id="72c71-106">Partnercenter</span><span class="sxs-lookup"><span data-stu-id="72c71-106">Partner Center</span></span>
-  <span data-ttu-id="72c71-107">Partner Center för Microsoft Cloud för amerikanska myndigheter</span><span class="sxs-lookup"><span data-stu-id="72c71-107">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="72c71-108">**Lämpliga roller**</span><span class="sxs-lookup"><span data-stu-id="72c71-108">**Appropriate roles**</span></span>

- <span data-ttu-id="72c71-109">Global administratör</span><span class="sxs-lookup"><span data-stu-id="72c71-109">Global admin</span></span>
- <span data-ttu-id="72c71-110">Administratörs agent</span><span class="sxs-lookup"><span data-stu-id="72c71-110">Admin agent</span></span>

<span data-ttu-id="72c71-111">\[Viss information relaterar till en för hands fri produkt som kan ändras avsevärt innan den släpps kommersiellt.</span><span class="sxs-lookup"><span data-stu-id="72c71-111">\[Some information relates to pre-released product which may be substantially modified before it's commercially released.</span></span> <span data-ttu-id="72c71-112">Microsoft lämnar inga garantier, uttryckliga eller underförstådda, avseende informationen som visas här.\]</span><span class="sxs-lookup"><span data-stu-id="72c71-112">Microsoft makes no warranties, express or implied, with respect to the information provided here.\]</span></span>

<span data-ttu-id="72c71-113">Du kan konsolidera klienter för ditt företag.</span><span class="sxs-lookup"><span data-stu-id="72c71-113">You can consolidate tenants for your business.</span></span> <span data-ttu-id="72c71-114">Använd de här anvisningarna för att konsolidera klienter för olika länder/regioner.</span><span class="sxs-lookup"><span data-stu-id="72c71-114">Use these instructions to consolidate tenants for different country/regions.</span></span>

>[!NOTE]  
><span data-ttu-id="72c71-115">Du måste vara medveten om alla etablerade prenumerationer och licens antal för var och en av dina kunder i kontot som du övergår från.</span><span class="sxs-lookup"><span data-stu-id="72c71-115">You must be aware of all of the provisioned subscriptions and license counts for each of your customers in the account you are transitioning from.</span></span> <span data-ttu-id="72c71-116">Du kommer att etablera om samma exakta prenumerationer med samma licens antal under det nya centrala CSP-kontot som en del av migreringsprocessen.</span><span class="sxs-lookup"><span data-stu-id="72c71-116">You will be re-provisioning those same exact subscriptions with the same license counts under the new central CSP account as part of the migration process.</span></span> <span data-ttu-id="72c71-117">Använd funktionen Exportera lista för att skapa en lista över kunder att gå över till den centraliserade klienten.</span><span class="sxs-lookup"><span data-stu-id="72c71-117">Use the export list feature to help create a list of customers to move over to the centralized tenant.</span></span>  <span data-ttu-id="72c71-118">När konsolideringen är klar kan du inte återgå till det tidigare klient organisations läget.</span><span class="sxs-lookup"><span data-stu-id="72c71-118">Once consolidation is complete, you can't revert to the previous tenant state.</span></span> <span data-ttu-id="72c71-119">Det kan också krävas en kund åtgärd.</span><span class="sxs-lookup"><span data-stu-id="72c71-119">Customer action may also be required.</span></span>

## <a name="prepare-for-migration"></a><span data-ttu-id="72c71-120">Förbereda för migrering</span><span class="sxs-lookup"><span data-stu-id="72c71-120">Prepare for migration</span></span>

- <span data-ttu-id="72c71-121">Logga in på **partner Center**  med hjälp av kontot för **över gång** (det som du kommer att övergå till det nya kontot) och granska alla kunder och alla tjänster som tillhandahålls för dessa kunder.</span><span class="sxs-lookup"><span data-stu-id="72c71-121">Sign in to **Partner Center**  using the **Transitioning** account (the one you will transition to the new account), and review of all customers and all of the services provisioned for those customers.</span></span>

- <span data-ttu-id="72c71-122">Logga ut från det här kontot.</span><span class="sxs-lookup"><span data-stu-id="72c71-122">Sign out of this account.</span></span>

## <a name="migrate-customer-accounts"></a><span data-ttu-id="72c71-123">Migrera kund konton</span><span class="sxs-lookup"><span data-stu-id="72c71-123">Migrate customer accounts</span></span>

1. <span data-ttu-id="72c71-124">Logga in på **partner Center** **med det nya kontot (det** som du använder för att överföra kunder till).</span><span class="sxs-lookup"><span data-stu-id="72c71-124">Sign in to **Partner Center**  with the **Transitioning** (new) account (the one you are transitioning customers into).</span></span>

2. <span data-ttu-id="72c71-125">Välj **Kunder** .</span><span class="sxs-lookup"><span data-stu-id="72c71-125">Select **Customers** .</span></span>

3. <span data-ttu-id="72c71-126">Klicka på **begär en åter försäljare relation** .</span><span class="sxs-lookup"><span data-stu-id="72c71-126">Click **Request a reseller relationship** .</span></span> <span data-ttu-id="72c71-127">Du får ett e-postmeddelande som standard för att skicka till dina kunder.</span><span class="sxs-lookup"><span data-stu-id="72c71-127">You are presented with a default email message to send to your customers.</span></span> <span data-ttu-id="72c71-128">Det här meddelandet innehåller en URL med det org-ID som är unikt för ditt nya partner Center-konto.</span><span class="sxs-lookup"><span data-stu-id="72c71-128">This message contains a URL with the org ID unique to your new Partner Center account.</span></span>

4. <span data-ttu-id="72c71-129">**Kund åtgärd:** Se till att alla aktiva kunder som du vill migrera besöker den här URL: en.</span><span class="sxs-lookup"><span data-stu-id="72c71-129">**Customer Action:** Ensure that each of the active customers you want to migrate visits this URL.</span></span> <span data-ttu-id="72c71-130">När du öppnar webb adressen uppmanas kunden att logga in på Office 365-portalen.</span><span class="sxs-lookup"><span data-stu-id="72c71-130">When opening the URL, the customer is prompted to sign in to the Office 365 portal.</span></span> <span data-ttu-id="72c71-131">Kunden loggar in med samma organisations-ID som de använder för att få åtkomst till Azure-och Office 365-administrations portalerna.</span><span class="sxs-lookup"><span data-stu-id="72c71-131">The customer signs in using the same Org ID that they use to access the Azure and Office 365 admin portals.</span></span>

5. <span data-ttu-id="72c71-132">När du har loggat in uppmanas den globala administratören för **kund kontot** att skicka ett avtal som ger delegerad administratörs behörighet till det nya CSP-kontot.</span><span class="sxs-lookup"><span data-stu-id="72c71-132">After signing in, the Global Admin for the **customer account** is prompted to submit an agreement that gives delegated admin privileges to the new CSP account.</span></span> <span data-ttu-id="72c71-133">Om de samtycker väljer kunden kryss rutan och accepterar att auktorisera relationen.</span><span class="sxs-lookup"><span data-stu-id="72c71-133">If they agree, the customer selects the checkbox and agrees to authorize the relationship.</span></span>

<span data-ttu-id="72c71-134">Kunderna kommer att visas i partnerns kund lista när de har skickat in avtalet, ett i taget.</span><span class="sxs-lookup"><span data-stu-id="72c71-134">The customers will appear in the partner's customer list after they have submitted the agreement, one by one.</span></span>

## <a name="migrating-office-365-and-non-azure-usage-based-subscriptions"></a><span data-ttu-id="72c71-135">Migrera Office 365 och användnings prenumerationer som inte använder Azure</span><span class="sxs-lookup"><span data-stu-id="72c71-135">Migrating Office 365 and non-Azure usage-based subscriptions</span></span>

1. <span data-ttu-id="72c71-136">När din kund har undertecknat avtalet kan du återskapa deras prenumerationer under din centraliserade partner klient.</span><span class="sxs-lookup"><span data-stu-id="72c71-136">Once your customer has signed the agreement, you can recreate their subscriptions under your Centralized Partner Tenant.</span></span>

2. <span data-ttu-id="72c71-137">Välj **kunder** från **partner Center** .</span><span class="sxs-lookup"><span data-stu-id="72c71-137">From **Partner Center** select **Customers** .</span></span>

3. <span data-ttu-id="72c71-138">Öppna företags namnet för den kund som du vill migrera.</span><span class="sxs-lookup"><span data-stu-id="72c71-138">Open the company name for the customer you want to migrate.</span></span>

4. <span data-ttu-id="72c71-139">Välj **Lägg till prenumeration** .</span><span class="sxs-lookup"><span data-stu-id="72c71-139">Select **Add subscription** .</span></span>

5. <span data-ttu-id="72c71-140">Lägg till rätt prenumerationer och licens antal från katalogen.</span><span class="sxs-lookup"><span data-stu-id="72c71-140">Add the correct subscriptions and license counts from the catalog.</span></span> <span data-ttu-id="72c71-141">Kontrol lera med den information som finns i **över gången från** partner konton.</span><span class="sxs-lookup"><span data-stu-id="72c71-141">Verify with the information provided in the **Transitioning From** partner accounts.</span></span>

   :::image type="content" source="images/regionalcustomer2.png" alt-text="kund lista":::

6. <span data-ttu-id="72c71-143">Klicka på **Skicka.**</span><span class="sxs-lookup"><span data-stu-id="72c71-143">Click **Submit.**</span></span>

   <span data-ttu-id="72c71-144">Tjänsterna tillhandahålls nu till kunden från **över gången till** partner kontot.</span><span class="sxs-lookup"><span data-stu-id="72c71-144">The services are now provided to the customer from the **Transitioning To** partner account.</span></span>

7. <span data-ttu-id="72c71-145">Upprepa de här stegen för att migrera prenumerationer för alla ytterligare kunder.</span><span class="sxs-lookup"><span data-stu-id="72c71-145">Repeat these steps to migrate subscriptions for all additional customers.</span></span>

<span data-ttu-id="72c71-146">Innan du fortsätter till nästa avsnitt bör du se till att alla kund prenumerationer som finns under **över gången från** partner konton etableras på nytt under **över gången till** partner kontot.</span><span class="sxs-lookup"><span data-stu-id="72c71-146">Before proceeding to the next section, ensure all customer subscriptions existing under the **Transitioning From** partner accounts are re-provisioned under the **Transitioning To** partner account.</span></span>

> [!NOTE]
> <span data-ttu-id="72c71-147">Partners måste pausa prenumerationer på **över gången från** partner klient kontot i Partner Center samma dag som prenumerationerna övergår till och konfigureras under **över gången till** partner klient kontot i partner centret för att säkerställa att dubbel fakturering inte sker.</span><span class="sxs-lookup"><span data-stu-id="72c71-147">Partners must suspend subscriptions on the **Transitioning From** Partner Tenant account in Partner Center the same day that those subscriptions are transitioned and set up under the **Transitioning To** Partner Tenant account in the Partner Center to ensure double billing does not occur.</span></span> <span data-ttu-id="72c71-148">Support förfrågningar kommer att nekas för krediter på grund av eventuella överlappningar i faktureringen som sker från att inte inaktivera **över gången från** prenumerationer.</span><span class="sxs-lookup"><span data-stu-id="72c71-148">Support requests will be denied for credits due to any overlap in billing that occurs from not correctly disabling the **Transitioning From** subscriptions.</span></span>

## <a name="disabling-the-office-365-subscriptions-under-the-transitioning-from-partner-account"></a><span data-ttu-id="72c71-149">Inaktiverar Office 365-prenumerationer under över gång från partner konto</span><span class="sxs-lookup"><span data-stu-id="72c71-149">Disabling the Office 365 subscriptions under the Transitioning From partner account</span></span>

<span data-ttu-id="72c71-150">Om du inaktiverar CSP-prenumerationen under **över gången från** partner konton avbryts eventuell framtida fakturering.</span><span class="sxs-lookup"><span data-stu-id="72c71-150">Disabling the CSP subscription under the **Transitioning From** partner accounts stops any future billing.</span></span> <span data-ttu-id="72c71-151">Du behöver inte inaktivera Azure-prenumerationer manuellt, eftersom Azure-prenumerationer inaktive ras automatiskt under migreringsprocessen.</span><span class="sxs-lookup"><span data-stu-id="72c71-151">You don't have to manually disable Azure subscriptions, because Azure subscriptions are automatically disabled during the migration process.</span></span>

1. <span data-ttu-id="72c71-152">Logga in på **partner Center** med **över gång från** CSP-konto och navigera till kund listan.</span><span class="sxs-lookup"><span data-stu-id="72c71-152">Sign in to the **Partner Center** with the **Transitioning From** CSP account and navigate to the customer list.</span></span>

2. <span data-ttu-id="72c71-153">Öppna kunden med prenumerationer som du vill inaktivera och välj sedan det första erbjudandet som ska inaktive ras.</span><span class="sxs-lookup"><span data-stu-id="72c71-153">Open the customer with subscriptions to disable, and then select the first offer to disable.</span></span>

3. <span data-ttu-id="72c71-154">Ställ in prenumerationen på **pausad** och klicka sedan på **Skicka** .</span><span class="sxs-lookup"><span data-stu-id="72c71-154">Set the subscription to **suspended** , and then click **submit** .</span></span>

   >[!Note]
   ><span data-ttu-id="72c71-155">Om du avbryter prenumerationen säkerställs dubbel fakturering.</span><span class="sxs-lookup"><span data-stu-id="72c71-155">Suspending the subscription ensures double billing does not occur.</span></span>

   <span data-ttu-id="72c71-156">Prenumerationen visar **inaktive** rad i prenumerations listan.</span><span class="sxs-lookup"><span data-stu-id="72c71-156">The subscription shows **suspended** on the subscriptions list.</span></span>

4. <span data-ttu-id="72c71-157">Upprepa de här stegen för alla prenumerationer under kunden.</span><span class="sxs-lookup"><span data-stu-id="72c71-157">Repeat these steps for all subscriptions under the customer.</span></span> <span data-ttu-id="72c71-158">Kontrol lera att alla visas **inaktiverade.**</span><span class="sxs-lookup"><span data-stu-id="72c71-158">Verify all show **suspended.**</span></span>

5. <span data-ttu-id="72c71-159">Välj nästa kund i listan och upprepa processen för att inaktivera alla prenumerationer.</span><span class="sxs-lookup"><span data-stu-id="72c71-159">Select the next customer on the list and repeat the process of disabling all subscriptions.</span></span>

## <a name="migrating-azure-usage-based-subscriptions"></a><span data-ttu-id="72c71-160">Migrera Azure Usage-baserade prenumerationer</span><span class="sxs-lookup"><span data-stu-id="72c71-160">Migrating Azure usage-based subscriptions</span></span>

<span data-ttu-id="72c71-161">Till skillnad från Office 365 CSP-prenumerationer behöver Azure, användnings CSP-prenumerationer inte migreras manuellt.</span><span class="sxs-lookup"><span data-stu-id="72c71-161">Unlike the Office 365 CSP subscriptions, Azure, usage-based CSP subscriptions do not need to be migrated manually.</span></span> <span data-ttu-id="72c71-162">Microsoft Azure-support migrerar Azure-prenumerationerna samt alla distribuerade tjänster eller resurser från **över gången från** CSP: er åter försäljar konton till kontot för **över gång till** CSP-återförsäljare.</span><span class="sxs-lookup"><span data-stu-id="72c71-162">Microsoft Azure Support will migrate the Azure subscriptions as well as all deployed services or resources from the **Transitioning From** CSP reseller accounts to the **Transitioning To** CSP reseller account.</span></span> <span data-ttu-id="72c71-163">Det sker ingen avbrott i tjänsten för kunden under över gången.</span><span class="sxs-lookup"><span data-stu-id="72c71-163">There will be no disruption of service to the customer during this transition.</span></span>

1. <span data-ttu-id="72c71-164">Se till att de kund konton som kommer att ha Azure-prenumerationer migrerats har godkänt att avtalet associeras med den nya **över gången till** CSP-kontot.</span><span class="sxs-lookup"><span data-stu-id="72c71-164">Ensure that the customer accounts that will have Azure subscriptions migrated have accepted the agreement to be associated with the new **Transitioning To** CSP account.</span></span>

2. <span data-ttu-id="72c71-165">Du kommer att meddela Microsoft om vilka kund konton som är redo att migrera och ange kundens företags namn.</span><span class="sxs-lookup"><span data-stu-id="72c71-165">You will notify Microsoft of which customer accounts are ready to migrate, and provide those customer's company names.</span></span>

3. <span data-ttu-id="72c71-166">Microsoft migrerar Azure Usage-baserade prenumerationer och meddelar dig när migreringen är klar.</span><span class="sxs-lookup"><span data-stu-id="72c71-166">Microsoft migrates the Azure usage-based subscriptions and notifies you when the migration is complete.</span></span>

4. <span data-ttu-id="72c71-167">Du måste bekräfta att Azure-prenumerationen under **över gången från** CSP Reporting-kontot nu har marker ATS som **inaktive** rad i Partner Center i avsnittet kund prenumerationer.</span><span class="sxs-lookup"><span data-stu-id="72c71-167">You need to confirm that the Azure subscription under the **Transitioning From** CSP reseller account now is marked **suspended** in Partner Center under the customer subscriptions section.</span></span>

5. <span data-ttu-id="72c71-168">Bekräfta att Azure-prenumerationen under **över gången till** CSP Reporting-kontot nu visar statusen **aktiv** i Partner Center i avsnittet kund prenumerationer.</span><span class="sxs-lookup"><span data-stu-id="72c71-168">Confirm that the Azure subscription under the **Transitioning To** CSP reseller account now shows a status of **active** in Partner Center under the customer subscriptions section.</span></span>

   >[!Note]
   > <span data-ttu-id="72c71-169">Om du inaktiverar prenumerationerna under kunden ändras inte utseendet på kunden i listan kunder.</span><span class="sxs-lookup"><span data-stu-id="72c71-169">Disabling the subscriptions under the customer does not change the appearance of the customer in the Customers list.</span></span> <span data-ttu-id="72c71-170">Det finns för närvarande inget alternativ att ta bort kunder från listan.</span><span class="sxs-lookup"><span data-stu-id="72c71-170">There is currently no option to remove customers from the list.</span></span> <span data-ttu-id="72c71-171">Partner bör undvika att lägga till prenumerationer till dessa kunder från deras **över gång från** konto i framtiden.</span><span class="sxs-lookup"><span data-stu-id="72c71-171">Partners should avoid adding subscriptions back to these customers from their **Transitioning From** account in the future.</span></span>

6. <span data-ttu-id="72c71-172">Upprepa de här stegen för alla prenumerationer under alla kunder för att stoppa framtida avgifter på **över gången från** konton.</span><span class="sxs-lookup"><span data-stu-id="72c71-172">Repeat these steps for all subscriptions under all of your customers to stop future charges on the **Transitioning From** account(s).</span></span> <span data-ttu-id="72c71-173">Partnern får en sista faktura med en kredit för antalet oanvända dagar mellan dagen för annullering och den sista dagen i fakturerings perioden.</span><span class="sxs-lookup"><span data-stu-id="72c71-173">The partner will receive one final invoice with a credit for the number of unused days between the day of cancellation and the last day of the billing period.</span></span> <span data-ttu-id="72c71-174">Inga framtida fakturor skapas efter den sista fakturerings perioden.</span><span class="sxs-lookup"><span data-stu-id="72c71-174">No future invoices will generate after that final billing period.</span></span>

### <a name="additional-information"></a><span data-ttu-id="72c71-175">Ytterligare information</span><span class="sxs-lookup"><span data-stu-id="72c71-175">Additional information</span></span>

- <span data-ttu-id="72c71-176">Inaktive ring av prenumerationen från **över gång från** CSP-konto påverkar inte den slutliga kundens tjänst så länge tjänsten etablerades från **över gången till** CSP-konto innan prenumerationen inaktiverades.</span><span class="sxs-lookup"><span data-stu-id="72c71-176">Disabling the subscription from the **Transitioning From** CSP account does not impact end customer's service as long as the service was provisioned from the **Transitioning To** CSP account prior to disabling the subscription.</span></span>

- <span data-ttu-id="72c71-177">Prenumerationer kan inte användas av kunden och genererar inga kostnader när de pausas eller avbryts.</span><span class="sxs-lookup"><span data-stu-id="72c71-177">Subscriptions cannot be used by the customer and do not generate charges when suspended or canceled.</span></span>

- <span data-ttu-id="72c71-178">Det finns för närvarande inget sätt att ta bort en kund helt från listan **kunder** .</span><span class="sxs-lookup"><span data-stu-id="72c71-178">There is currently no way to remove a customer completely from the **Customers** list.</span></span>
- 
    >[!Note]
    > <span data-ttu-id="72c71-179">Partners måste pausa prenumerationer på **över gången från** partner klient kontot i Partner Center samma dag som dessa prenumerationer överförs till och konfigureras under **över gången till** konto för att säkerställa dubbel fakturering.</span><span class="sxs-lookup"><span data-stu-id="72c71-179">Partners must suspend subscriptions on the **Transitioning From** partner tenant account in Partner Center the same day those subscriptions are transitioned to and set up under the **Transitioning To** account to ensure double billing does not occur.</span></span> <span data-ttu-id="72c71-180">Microsoft stöder inte förfrågningar om krediter på grund av eventuella överlappningar i faktureringen som sker från att inte ställa in **över gången från** prenumerationer till pausad.</span><span class="sxs-lookup"><span data-stu-id="72c71-180">Microsoft will not support requests for credits due to any overlap in billing that occurs from not correctly setting the **Transitioning From** subscriptions to suspended.</span></span>

### <a name="simplify-migration-using-export"></a><span data-ttu-id="72c71-181">Förenkla migreringen med hjälp av export</span><span class="sxs-lookup"><span data-stu-id="72c71-181">Simplify migration using Export</span></span>

<span data-ttu-id="72c71-182">Med hjälp av **funktionen Exportera** kan du samla in de prenumerationer som du behöver använda i din nya konsoliderade struktur:</span><span class="sxs-lookup"><span data-stu-id="72c71-182">Using the **Export Function** , you can capture the subscriptions you need to use in your new consolidated structure:</span></span>

1. <span data-ttu-id="72c71-183">Klicka på **kunder** i Partner Center för att se listan över kunder.</span><span class="sxs-lookup"><span data-stu-id="72c71-183">Click **Customers** on Partner Center to see the list of customers.</span></span> 

2. <span data-ttu-id="72c71-184">Öppna det önskade kund namnet.</span><span class="sxs-lookup"><span data-stu-id="72c71-184">Open the desired customer name.</span></span>

3. <span data-ttu-id="72c71-185">På sidan **prenumerationer** klickar du på **Exportera prenumerationer** för att exportera information om prenumerationer till en Excel-fil.</span><span class="sxs-lookup"><span data-stu-id="72c71-185">On the **Subscriptions** page, click **Export Subscriptions** to export details of subscriptions to an Excel file.</span></span>

4. <span data-ttu-id="72c71-186">Använd den här listan för att återskapa prenumerationerna i den nya konsoliderade klienten.</span><span class="sxs-lookup"><span data-stu-id="72c71-186">Use this list to recreate the subscriptions in your new consolidated tenant.</span></span>

### <a name="api-registration"></a><span data-ttu-id="72c71-187">API-registrering</span><span class="sxs-lookup"><span data-stu-id="72c71-187">API registration</span></span>

<span data-ttu-id="72c71-188">Mer information om API-registrering finns i [Konfigurera API-åtkomst i Partner Center](/partner-center/develop/set-up-api-access-in-partner-center).</span><span class="sxs-lookup"><span data-stu-id="72c71-188">For more information about API registration, see [Set up API access in Partner Center](/partner-center/develop/set-up-api-access-in-partner-center).</span></span>

## <a name="next-steps"></a><span data-ttu-id="72c71-189">Nästa steg</span><span class="sxs-lookup"><span data-stu-id="72c71-189">Next steps</span></span>

- [<span data-ttu-id="72c71-190">Cloud Solution Provider program regionala marknader och valutor där du kan sälja CSP-erbjudanden</span><span class="sxs-lookup"><span data-stu-id="72c71-190">Cloud Solution Provider program regional markets and currencies where you can sell CSP offers</span></span>](regional-authorization-overview.md)
