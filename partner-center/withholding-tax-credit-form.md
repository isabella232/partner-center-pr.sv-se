---
title: Få krediter ATS för käll skatt
ms.topic: article
ms.date: 06/05/2020
description: Ta emot kredit på ditt partner Center-konto för käll skatt. Informationen omfattar steg för att skicka en begäran om moms käll förfrågan.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 064a5ea1e712ca66504536652543c0523fc73eae
ms.sourcegitcommit: bff907bdbddc769716c7418a2b4a94ca37c2d590
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/03/2021
ms.locfileid: "101755728"
---
# <a name="receive-credit-on-your-partner-center-account-for-tax-withholding"></a>Ta emot kredit på ditt partner Center-konto för käll skatt

**Lämpliga roller**

- Kontoadministratör
- Faktureringsadministratör

## <a name="overview"></a>Översikt

CSP-partner i vissa länder får faktura belopp som inkluderar skatter. Några av dessa partner betalar sin lokala skattemyndighet i stället för Microsoft. Om du betalar din lokala skattemyndighet måste du skicka en begäran om moms avdrag, inklusive ditt skatte certifikat för att rensa den skattepliktiga mängden från föregående fakturor. Dessa rensade belopp visas i den **sista betalnings** kolumnen på **fakturerings sidan** i Partner Center.

Partner som används för att skicka begäran om käll skatter genom att skapa tjänst begär Anden (partner support biljetter) i Partner Center. Den här processen ändrades i januari 2020. Nu ska CSP-partner skicka begäran om käll skatter på **fakturerings sidan** i stället för att skapa support förfrågningar.

> [!IMPORTANT]
> Partner kan bara skicka käll skatte förfrågningar för **betalda** fakturor.

## <a name="submit-a-tax-withholding-request"></a>Skicka en begäran om moms käll förfrågan

Följ dessa steg om du vill skicka en ny käll indrags deklaration:

1. Logga in i Partnercenter och gå till [instrumentpanelen](https://partner.microsoft.com/dashboard/home).

2. Välj **fakturering** på menyn till vänster och gå till **fakturerings historiken**.

3. Klicka på **Skicka ny** bredvid fakturan som du vill skicka en rensning för. Den nya länken skickas till sidan **ny begäran om käll-och käll begäran** .

   :::image type="content" source="images/wht1.png" alt-text="Skicka ny moms avdrag för en faktura":::

4. Granska faktura informationen för att se till att du skickar in begäran om rätt faktura.

   :::image type="content" source="images/wht2.png" alt-text="Fullständig information om moms avdrag för en faktura":::

5. Ange "käll total" under **moms käll information**. "Käll totalen" är den mängd du förväntar dig att kreditera.

6. **Bifoga** ett skatte certifikat. Du måste inkludera en **digital kopia** av ditt **käll skatte certifikat** i din begäran om moms inskrivning. Du har fått det här certifikatet från din lokala skatte byrå när du betalar dina skatter till din lokala skattemyndighet. Fakturans skatte belopp i käll skatte certifikatet måste matcha det totala antalet i din begäran om käll skatt.

   > [!IMPORTANT]
   > Antalet summor som partnern tillhandahåller måste matcha faktura rads objektet från det kopplade moms certifikatet. Bifogade skatte certifikat måste vara i något av följande fil format:. Endast PDF eller bild (. JPEG,. PNG och. GIF). Dessutom får filernas namn inte innehålla blank steg eller specialtecken. Fil storleken får inte överstiga 1 MB.

7. **Skicka** begäran om moms käll förfrågan.

   När begäran har skickats hamnar begäran i godkännande processen där den kommer att godkännas för slut för ande eller skickas tillbaka till dig om det behövs ändringar. Visa förfrågan-ID och status för dina begär Anden och i **fakturerings historiken** där du skickade den nya begäran från.

   Om din begäran skickas tillbaka till dig, kan du ändra käll beloppet och ersätta certifikatet om det är problem med det.

## <a name="update-request-and-resubmit"></a>Uppdatera begäran och skicka igen

Gransknings teamet kan kräva att du gör korrigeringar och skickar en begäran igen innan den kan godkännas. De ändrar statusen till den **väntande partner åtgärden**. Korrigera och skicka begäran på nytt:

1. Logga in i Partnercenter och gå till [instrumentpanelen](https://partner.microsoft.com/dashboard/home).

2. Välj **fakturering** på menyn till vänster.

3. På **fakturerings** sidans **fakturerings historik**, Sök efter begäran om moms inbetalning. Begär Anden som kräver din uppmärksamhet kommer att ha statusen "väntande partner åtgärd".

4. Klicka på begäran om käll-ID för begäran och status som tar dig till sidan för begäran.

5. Välj **Uppdatera och skicka** om under **status**.

6. Granska de kommentarer som lämnats av granskarna som markerar vad som behöver ändras.

7. Gör korrigeringarna genom att antingen skicka om ett uppdaterat certifikat eller justera käll beloppen.

8. **Skicka** begäran.

Om du skickar begäran skickas den tillbaka till gransknings teamet där de antingen godkänner eller ber om fler ändringar.

### <a name="approved-requests"></a>Godkända begär Anden

Godkända käll begär Anden för begäran kommer att utföras mot nästa faktura, vilket skriver av skulder-beloppet. Begär Anden som flaggats som **slutförda** ska tillämpas inom 10 arbets dagar. 

Rensade belopp visas på sidan fakturerings **historik för fakturerings sida**. De belopp som är rensade visas i den **sista betalnings** kolumnen bredvid fakturan som begäran skickades till.

   > [!IMPORTANT]
   > Tidigare fakturor återskapas inte eller återutfärdas. Clearace-beloppet tillämpas helt enkelt på föregående månads betalningar.

Bearbetning av moms käll begär Anden bör ta två dagar att slutföra förutsatt att skatte certifikat och belopp är korrekta. Om det krävs ändringar tar det längre tid på grund av de korrigeringar som måste göras och skickas igen.

Om du har frågor om kredit förfrågnings processen för käll skatt skickar du en biljett till partner support. Du behöver ID: t för skatte käll förfrågan för att lösa frågor.

## <a name="german-tax-withholding"></a>Tysk moms avdrag

Partner som skickar tyska skattemyndighets begär Anden bör komma ihåg att skicka hård kopior av ditt käll skatte certifikat till följande adress:

- ATTN: EOC Tax team Marianne Gannon
- Microsoft EMEA drifts Center
- En Microsoft-plats,
- Södra County Business Park
- Leopardstown, Dublin 18, Irland

### <a name="questions-and-assistance-for-tax-withholding-requests"></a>Frågor och hjälp vid begäran om skatte avdrag

Partner bör använda den nya processen som beskrivs ovan för att skicka nya begär Anden och inte längre använda support förfrågan för nya moms indrags begär Anden. Partner med ytterligare frågor om moms käll begär Anden kan [Skicka support förfrågningar](https://partner.microsoft.com/dashboard/support/csp/servicerequests/create?stage=2&topicid=9227afa6-babf-3917-acee-67db7860f5ed). Support förfrågningar är avsedda att hjälpa partners för befintliga begär Anden så att de måste ha sitt **begäran-ID** för att kunna skicka in en ny biljett. Om partners inte kan skicka en begäran med den nya processen, ska de ange ett värde (alla 1) i support förfrågnings formuläret. 

   > [!IMPORTANT]
   > Partners behöver inte kontakta supporten om deras status för begäran har **slutförts**. Den här statusen visas i **fakturerings historiken** bredvid fakturan för inlämningen. De **senaste betalnings** beloppen bredvid fakturan ska avspegla moms käll beloppet inom tio dagar efter det att begäran marker ATS som **slutförd**.
