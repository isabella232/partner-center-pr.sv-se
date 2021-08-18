---
title: Krediteras för källskatt
ms.topic: article
ms.date: 06/05/2020
description: Få kredit på ditt Partnercenter-konto för källskatt. Informationen omfattar steg för att skicka en begäran om källskatt.
ms.service: partner-dashboard
ms.subservice: partnercenter-billing
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 2d0c1e05ff0e0b9c807dfc7beb1136cec87b4069
ms.sourcegitcommit: 8fe3b0f22d548bc6bcc1b87636216cd4d42b3ede
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/17/2021
ms.locfileid: "122297155"
---
# <a name="receive-credit-on-your-partner-center-account-for-tax-withholding"></a>Få kredit på ditt Partnercenter-konto för källskatt

**Lämpliga roller:** Kontoadministratörsroller | Faktureringsadministratör

## <a name="overview"></a>Översikt

Molnlösningsleverantör (CSP)-partner i vissa länder får fakturabelopp som inkluderar skatter. Vissa av dessa partner betalar sin lokala skatteutfärdare i stället för Microsoft. Om du betalar din lokala skatteutfärdare måste du skicka en begäran om källskatt, inklusive ditt skattecertifikat, för att rensa det skattade beloppet från tidigare fakturor. Dessa rensade belopp visas i kolumnen **Senaste betalning** på sidan **Fakturering i** Partnercenter.

Partner som används för att skicka begäranden om källskatt genom att skapa tjänstbegäranden (partnersupportärenden) i Partnercenter. Den här processen ändrades i januari 2020. Nu bör CSP-partner skicka begäranden om källskatt på sidan **Fakturering i stället** för att skapa supportbegäranden.

> [!IMPORTANT]
> Partner kan endast skicka källskatteförfrågningar för delvis betalda fakturor. Om du vill ha fullständiga eller obevakade fakturor kontaktar du [supporten](report-problems-with-partner-center.md) med ditt källskattcertifikat.

## <a name="submit-a-tax-withholding-request"></a>Skicka en begäran om källskatt

Följ dessa steg för att skicka en ny källskatt:

1. Logga in i Partnercenter och gå till [instrumentpanelen](https://partner.microsoft.com/dashboard/home).

2. I den vänstra menyn väljer du Fakturering **och** går till **Faktureringshistorik.**

3. Välj **Skicka ny** bredvid den faktura som du vill skicka ett tillstånd för. Länken Skicka ny tar dig till sidan **Ny begäran om källskatt.**

   :::image type="content" source="images/wht1.png" alt-text="Skicka ny källskatt för en faktura.":::

4. Granska fakturainformationen för att se till att du skickar begäran om rätt faktura.

   :::image type="content" source="images/wht2.png" alt-text="Fyll i källskattsinformation för en faktura.":::

5. Ange "Källskattesumma" under **Information om källskatt.** "Källbelopp" är det belopp som du förväntar dig att krediteras.

6. **Bifoga** ett skattecertifikat. Du måste inkludera en **digital kopia** av **källskattecertifikatet** i begäran om källskatt. Du har fått det här certifikatet från ditt lokala skatteorgan när du betalar dina skatter till din lokala skatteutfärdare. Fakturaskattebeloppet i källskattecertifikatet måste matcha det totala beloppet i begäran om källskatt.

   > [!IMPORTANT]
   > Summan som partnern tillhandahåller ska matcha fakturaradsposten från det bifogade skattecertifikatet. Bifogade skattecertifikatfiler måste ha något av följande filformat: endast .PDF eller Bild (. JPEG, .PNG och .GIF). Dessutom får inte namn på filer innehålla blanksteg eller specialtecken. Filstorlekar får inte överskrida 1 MB.

7. **Skicka** begäran om källskatt.

   När den har skickats går den vidare till godkännandeprocessen där den godkänns för slutförande eller skickas tillbaka till dig om det behövs korrigeringar. Visa begärande-ID och status för dina begäranden och i **faktureringshistoriken** som du skickade den nya begäran från.

   Om din begäran skickas tillbaka till dig kan du ändra källbeloppet och ersätta certifikatet om det är problem med det.

## <a name="update-request-and-resubmit"></a>Uppdatera begäran och skicka igen

Granskningsteamet kan kräva att du gör ändringar och skickar en begäran igen innan den kan godkännas. De ändrar statusen till **Väntande partneråtgärd**. Så här korrigerar och skickar du begäran:

1. Logga in i Partnercenter och gå till [instrumentpanelen](https://partner.microsoft.com/dashboard/home).

2. I den vänstra menyn väljer du **Fakturering**

3. På sidan **Faktureringshistorik** **hittar du** begäran om källskatt. Begäranden som behöver din uppmärksamhet får statusen "Väntande partneråtgärd".

4. Välj ID och status för begäran om källskatt som tar dig till begärans sida.

5. Välj **Uppdatera och skicka igen** under **Status**.

6. Granska kommentarerna som granskarna lämnar och markera vad som behöver ändras.

7. Gör korrigeringarna genom att antingen skicka ett uppdaterat certifikat på nytt eller justera källbeloppen.

8. **Skicka** begäran.

Om du skickar begäran skickas den tillbaka till granskningsteamet där de antingen godkänner eller ber om fler ändringar.

### <a name="approved-requests"></a>Godkända begäranden

Godkända begäranden om källskatt körs mot nästa faktura och skriver av det belopp som ska betalas. Begäranden som flaggas som **Slutförda** ska tillämpas inom 10 arbetsdagar. 

Rensade belopp visas i avsnittet **Faktureringshistorik** på sidan Fakturering. De belopp som rensas visas i **kolumnen Senaste betalning** bredvid fakturan som begäran skickades mot.

   > [!IMPORTANT]
   > Tidigare fakturor återskapas inte eller återskapas inte. Beloppsbeloppet tillämpas helt enkelt på de föregående månadernas betalningar.

Bearbetningen av begäranden om källskatt bör ta två dagar att slutföra, förutsatt att skattecertifikatet och beloppet är korrekta. Om det krävs ändringar tar det längre tid på grund av de korrigeringar som måste göras och skickas igen.

Om du har frågor om processen för begäran om källskattekredit skickar du en begäran till partnersupporten. Du behöver begärande-ID:t för källskatt för att lösa frågor.

## <a name="german-tax-withholding"></a>Tyska källskatter

Partner som skickar begäranden om källskatt i Tyskland bör komma ihåg att skicka papperskopior av källskattecertifikatet till följande adress:

- ATTN: EOC-skatteteamet För skatteteamet
- Microsoft EMEA Operations Centre
- One Microsoft Place,
- South County Business Park
- Harten, Dublin 18, Irland

### <a name="questions-and-assistance-for-tax-withholding-requests"></a>Frågor och hjälp med begäranden om källskatt

Partner bör använda den nya processen som beskrivs ovan för att skicka nya begäranden och inte längre använda skapande av supportbegäran för nya källskattbegäranden. Partner med fler frågor om begäranden om källskatt kan skicka [supportbegäranden.](https://partner.microsoft.com/dashboard/support/csp/servicerequests/create?stage=2&topicid=9227afa6-babf-3917-acee-67db7860f5ed) Supportbegäranden är avsedda att hjälpa partner för befintliga begäranden så att de måste ha sitt **begärande-ID för** att skicka en ny supportbegäran. Om partner inte kan skicka en begäran med hjälp av den nya processen ska de ange ett visst antal (alla 1:ar) i formuläret för supportbegäran. 

   > [!IMPORTANT]
   > Partner behöver inte kontakta supporten om deras begärandestatus är **Slutfört.** Den här statusen visas **i faktureringshistoriken** bredvid fakturan för överföringen. **De senaste** betalningsbeloppen bredvid fakturan ska återspegla källskattebeloppet inom tio dagar efter att begäran har markerats som **Slutförd.**
