---
title: Kundsida för MCI-engagemang
description: Använd sidan Kunder i avsnittet Microsoft Commerce Incentive (MCI)-program Engagements för att hantera kunder.
author: Karthic83
ms.author: kashanum
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
ms.topic: how-to
ms.date: 09/29/2021
ms.custom: template-how-to
ms.openlocfilehash: bfa3185213abe5e166c3049602d3ca2dc16be70c
ms.sourcegitcommit: 6d29e7e6d700ee5638ba10ee12f75e37f993dae9
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 10/01/2021
ms.locfileid: "129365143"
---
# <a name="customers-page-for-mci-engagements"></a>Kundsida för MCI-engagemang

**Lämpliga roller:** Incitamentsadministratörsroller | Incitamentsanvändare

>[!NOTE]
>Detta gäller endast för att skapa avsiktsinteragemang, det vill säga studiekurser. 

Sidan **Kunder** sorterar kunder efter berättigade, icke-berättigade och fullständiga för varje engagemang. Sidan är förindelad med alla kunder som har gett sitt medgivande för en workshop i Partnercenter. 

:::image type="content" source="images/incentives/customers-page.png" alt-text="Skärmbild av sidan Kunder." lightbox="images/incentives/customers-page.png":::

- Fliken **Berättigade** visar alla kunder som är berättigade till workshoppen. 
   - I **kolumnen** Typ visas kunder som "aktiva" om du har fått medgivande från kunden. Fram till dess kommer det att visas som "inte startat".
- Fliken **Ineligible** visar alla kunder som inte är justerade för workshopen av någon av tre skäl:  
   - Kunden uppfyller inte villkoren för berättigande för åtagandet, 
   - Kunden har gett sitt medgivande till en annan partner, eller 
   - Kunden har redan deltagit i workshoppen med en annan partner. 
- Fliken **Slutför** visar alla kunder som du har slutfört den här workshopen för. Du kan se information om ditt anspråk med den här kunden genom att välja **Visa workshop-anspråk** under **kolumnen** Åtgärd.

För alla engagemang måste du antingen lägga till en kund eller göra anspråk på en kund (inte båda).

## <a name="add-a-customer"></a>Lägga till en kund 
1. Välj **+ Lägg till kund** på sidan **Kunder** i relevant workshop-engagemang med hjälp av **fliken Berättigade.**
2. Ange ett MPN-plats-ID för workshopen och kundens e-postadress. Fältet **Kundens TPID/klient-ID** är valfritt. Endast MPN-plats-ID:er som båda har registrerats i MCI-programmet och som är berättigade till det här engagemanget visas. Välj **Nästa**.
   - Om du inte anger något klientorganisations-ID eller ett överordnat ID (TPID) för kunden kommer systemet att härleda klient-ID:t från kundens e-postadress. Den kör sedan kundberättigandekontrollen för workshopen.
   - Om kundens klientorganisations-ID inte kan hittas med hjälp av e-postadressen uppmanas du att ange en annan e-postadress eller klient-ID/TPID.
   - Om klient-ID/TPID anges ser systemet till att e-postdomänen matchar klientorganisationens ID. Om ett matchningsfel hittas ber systemet dig att ange en orsak.

   :::image type="content" source="images/incentives/add-customer-1.png" alt-text="Skärmbild 1 av 3 som visar hur du lägger till en kund." lightbox="images/incentives/add-customer-1.png":::

3. Välj den eller de workshopar som du vill lägga till kunden för. Endast de studiekurser kan väljas för vilka både du och din kund är berättigade. Välj **Nästa**.

:::image type="content" source="images/incentives/add-customer-2.png" alt-text="Skärmbild 2 av 3 som visar hur du lägger till en kund." lightbox="images/incentives/add-customer-2.png":::

4. Granska informationen och välj Lägg **till kund.** Du får en bekräftelse på att kunden har lagts till.

:::image type="content" source="images/incentives/add-customer-3.png" alt-text="Skärmbild 3 av 3 som visar hur du lägger till en kund." lightbox="images/incentives/add-customer-3.png":::

Du bör nu se kunden som du har lagt till på respektive **kundsida** för de workshopgemang som valdes i steg 3.

## <a name="claim-a-customer"></a>Begära en kund 
Fliken **Berättigade** på sidan **Kunder** är förindelad med en lista över kunder som är kända för dig, partnern, via andra engagemang. Du kan starta en workshop med någon av dessa kunder. 
1. Välj Claim customer (Anspråkskund) **i kolumnen** Åtgärd.  
2. Välj ett MPN-plats-ID för workshopen. Endast MPN-plats-ID:erna som har registrerats i MCI-programmet och som är berättigade till det här engagemanget visas. Välj **Nästa**.

   :::image type="content" source="images/incentives/claim-customer-1.png" alt-text="Skärmbild 1 av 3 som visar hur du begär kund." lightbox="images/incentives/claim-customer-1.png":::

3. Välj de workshop(er) som du vill lägga till och välj sedan **Nästa.**

   :::image type="content" source="images/incentives/claim-customer-2.png" alt-text="Skärmbild 2 av 3 som visar hur du begär kund." lightbox="images/incentives/claim-customer-2.png":::

4. Granska informationen och välj Lägg **till kund.** Du får en bekräftelse på att kunden har begärts.

   :::image type="content" source="images/incentives/claim-customer-3.png" alt-text="Skärmbild 3 av 3 som visar hur du begär kund." lightbox="images/incentives/claim-customer-3.png":::

## <a name="ask-for-customer-consent"></a>Be om kundens medgivande 
Om du vill genomföra en workshop med en kund måste du be kunden om medgivande, vilket är deras avtal för att delta i workshopen. Du har totalt 30 dagar på dig att få medgivande när du har lagt till eller gjort anspråk på kunden.

När du har lagt till eller begärt en kund ser du hur många dagar du har lämnat för att få medgivande i statuskolumnen på **sidan** Kunder.
1. Välj **Utlöst kundmedgivande** i **kolumnen** Åtgärd. 
2. Ange kundens e-post och kontaktinformation, tillsammans med kontaktinformation för ditt eget företag. Välj sedan **Nästa**.

   :::image type="content" source="images/incentives/ask-consent-1.png" alt-text="Skärmbild 1 av 2 som visar hur du begär kundens medgivande." lightbox="images/incentives/ask-consent-1.png":::

3. Granska informationen och välj **Skicka för medgivande.** Ett e-postmeddelande skickas till kunden så att de kan godkänna eller avvisa workshopen.
   - Om du inte har fått ditt medgivande kan du skicka en påminnelse genom att klicka på länken Skicka om **kundens medgivande** under **kolumnen** Åtgärd.
   - Om en kund nyligen har lagts till men avböjer deltagande i workshopen eller inte svarar inom den tidslinje som krävs, visas de inte längre på **sidan** Kunder för det engagemanget.

   :::image type="content" source="images/incentives/ask-consent-2.png" alt-text="Skärmbild 2 av 2 som visar hur du begär kundens medgivande." lightbox="images/incentives/ask-consent-2.png":::

När kunden har gett sitt medgivande har du 90 dagar på dig att genomföra workshopen.

## <a name="next-steps"></a>Nästa steg
[Skicka ett workshop-anspråk](/partner-center/mci-engagements-workshop)

[Översikt över och behörighet för MCI-engagemang](/partner-center/mci-engagements)

[Använd de här resurserna för att komma igång med incitament](/partner-center/incentives-get-started-intro)

[Fastställa behörighet för incitamentsprogrammet](/partner-center/incentives-determined-your-program-eligibility)

[Registrering och användarhantering i incitamentsprogrammet](/partner-center/incentives-enroll)