---
title: Anslutningsappen för säljförsäljning för Salesforce CRM Partner Center
ms.topic: how-to
ms.date: 01/06/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Synkronisera dina hänvisningar i Partnercenter med din Salesforce CRM. Säljare kan sedan samförsäljninga med Microsoft inifrån dina CRM-system.
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: fa9b35343e1251cfce5caff107de8dff344f4e68
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 05/19/2021
ms.locfileid: "110148422"
---
# <a name="co-sell-connector-for-salesforce-crm---overview"></a>Anslutningsapp för säljförsäljning för Salesforce CRM – översikt

**Lämpliga roller:** Referensadministratörsroller | Systemadministratör eller systemanpassare för CRM

PartnerCenter-anslutningsappen för säljpartner gör det möjligt för dina säljare att samarbeta med Microsoft inifrån dina CRM-system. De behöver inte tränas för att använda PartnerCenter för att hantera säljavtal. Med hjälp av anslutningsapparna för säljförsäljning kan du skapa en ny hänvisning till säljförsäljning för att engagera en Microsoft-säljare, få hänvisningar från Microsoft-säljaren, acceptera/avvisa hänvisningar, ändra avtalsdata som avtalsvärde och slutdatum.  Du kan också få uppdateringar från Microsoft-säljarna om dessa samförsäljningserbjudanden. Du kan göra så att alla dina hänvisningar fungerar när du arbetar i den CRM som du väljer i stället för i Partnercenter. 

Lösningen är baserad på Microsoft Power Automate Solution och använder Partner Center-API:er.

## <a name="before-you-install---pre-requisites"></a>Innan du installerar – förutsättningar

|**Ämnen**   |**Information**   |**Länkar**   |
|--------------|--------------------|------|
|Microsoft Partner Network-ID |Du behöver ett giltigt MPN-ID|Så här ansluter du [till MPN](https://partner.microsoft.com/)|
|Redo för säljförsäljning|Din IP/Services-lösning måste vara redo för säljförsäljning.|[Sälja med Microsoft](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|Partnercenter-konto|MPN-ID:t som är associerat med Partnercenter-klienten måste vara samma som det MPN-ID som är associerat med din säljförsäljningslösning. Kontrollera att du kan se dina hänvisningar till säljförsäljning i PartnerCenter-portalen innan du distribuerar anslutningsapparna.|[Hantera ditt konto](create-user-accounts-and-set-permissions.md)|
|Användarroller i Partnercenter|Medarbetaren som ska installera och använda anslutningsapparna måste vara referensadministratör|[Tilldela användarroller och -behörigheter](create-user-accounts-and-set-permissions.md)|
|Salesforce CRM|CRM-användarrollen är Systemadministratör eller Systemanpassare|[Tilldela roller i Salesforce CRM](https://help.salesforce.com/articleView?id=assigning_users_to_roles.htm&type=5)|
|Power Automate Flow-konto|Ett aktivt [Power Automate](https://flow.microsoft.com) konto för CRM-systemadministratören eller systemanpassaren. Användaren bör logga in på [Power Automate](https://flow.microsoft.com) minst en gång före installationen.|

## <a name="installation-of-salesforce-package-for-microsoft-custom-fields"></a>Installation av Salesforce-paket för Microsoft Custom Fields 

Om du vill synkronisera hänvisningarna i Partner Center och Salesforce CRM Power Automate lösningen tydligt identifiera Microsoft-specifika hänvisningsfält. Den här avgränsningen ger partnerförsäljningsteam möjlighet att bestämma vilka hänvisningar som de vill dela med Microsoft för samförsäljning.

1. I Salesforce aktiverar du **Anteckningar och** lägger till den i listan med affärsmöjligheter. 
[Referens](https://help.salesforce.com/articleView?err=1&id=notes_admin_setup.htm&type=5)

2. Aktivera **affärsmöjlighetsteam** genom att följa stegen: 
    - I installationsprogrammet använder du rutan **Snabb hitta** för att hitta inställningar för affärsmöjlighetsteam.
    - Definiera inställningarna efter behov.
[Referens](https://help.salesforce.com/articleView?id=teamselling_enabling.htm&type=5]) 

3. Installera anpassade fält och objekt i Salesforce med hjälp av [installationsprogrammet för paketet](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t2w000006WIwV). Använd det här om du vill installera paketet på ett företag.

>[!NOTE]
>Om du installerar i en sandbox-miljö måste du ersätta den första delen av URL:en med http://test.salesforce.com

4. I Salesforce lägger du till Microsoft Solutions i **listan Affärsmöjlighetsrelaterade.** När den har lagts till väljer **du ikonen** för ikonikonen och uppdaterar egenskaper

## <a name="best-practice-test-before-you-go-live"></a>Bästa praxis: Testa innan du går live

Innan du installerar, konfigurerar och anpassar Power Automate-lösningen i produktionsmiljön måste du testa lösningen på en CRM-mellanlagringsinstans.

- Installera Microsoft Power Automate lösning på en mellanlagringsmiljö/CRM-instans.

- Skapa en kopia av lösningen och kör konfigurationen och Power Automate av flödesanpassningar i mellanlagringsmiljön.

- Testa lösningen på en mellanlagrings-/CRM-instans.

- Vid lyckad import som en hanterad lösning till produktionsinstansen.

## <a name="install-partner-center-referrals-synchronization-for-salesforce-crm"></a>Installera synkronisering av partnercenterreferenser för Salesforce CRM

1. Gå till [Power Automate](https://flow.microsoft.com) och **välj Miljöer** i det övre högra hörnet. Då visas tillgängliga CRM-instanser.

2. Välj lämplig CRM-instans i listrutan i det högra övre hörnet.

3. Välj **Lösningar** i det vänstra navigeringsfältet.

4. Välj länken **Öppna AppSource** på den översta menyn.

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="Öppna AppSource":::

5. Sök efter **partnercenterreferenser för Salesforce** på popup-skärmen.  

   :::image type="content" source="images/salesforce/salesforce1.png" alt-text="Salesforce":::

6. Välj knappen **Hämta nu** och sedan **Fortsätt.**

7. Då öppnas sidan där du kan välja Salesforce CRM-miljön för att installera programmet.  Godkänn villkoren.

   :::image type="content" source="images/salesforce/available-crm.png" alt-text="Tillgängliga CRMS":::

8. Du dirigeras sedan till sidan **Hantera dina** lösningar.  Gå till "Partner Center-referenser" med hjälp av pilknapparna längst ned på sidan. **Schemalagd installation** bör visas bredvid referenslösningen i Partnercenter. Installationen tar 10–15 minuter.

9. När installationen är klar går du tillbaka till [Power Automate](https://flow.microsoft.com) väljer **Lösningar i** det vänstra navigeringsområdet. Observera att **Synkronisering av Referenser för Partnercenter för Salesforce** finns i listan Lösningar.

10. Välj **Synkronisering av partnercenterreferenser för Salesforce.** Följande flöden Power Automate och entiteter är tillgängliga:

    :::image type="content" source="images/cosellconnectors/salesforce10.png" alt-text="Salesforce-flöden":::



## <a name="configure-the-solution"></a>Konfigurera lösningen

1. När du har installerat lösningen i din CRM-instans går du tillbaka till [Power Automate](https://flow.microsoft.com/).

2. I **listrutan Miljöer** i det övre högra hörnet väljer du den CRM-instans där du installerade Power Automate lösningen.
3. Du måste skapa anslutningar som associerar de tre användarkontona:
    - PartnerCenter-användare med referenser för administratörsautentiseringsuppgifter
    - Partnercenter-händelser
    - CRM-administratör med Power Automate flöden i lösningen.
4. Välj **Anslutningar** i det vänstra navigeringsfältet och välj lösningen "PartnerCenter-referenser" i listan.

5. Skapa en anslutning genom att klicka **på Skapa en anslutning.**

:::image type="content" source="images/cosellconnectors/salesforce12.png" alt-text="Skapa anslutning":::

- Sök efter Referenser till Partnercenter (förhandsversion) i sökfältet i det övre högra hörnet.

- Skapa en anslutning för din Partnercenter-användare med rollen Referensadministratör.

-  Skapa sedan en partnercenterhändelser-anslutning för din Partnercenter-användare med autentiseringsuppgifterna för referensadministratören.

- Skapa en anslutning för Salesforce för CRM-administratörsanvändaren.

-  När du har lagt till alla anslutningar bör du se följande anslutningar i din miljö:

 :::image type="content" source="images/cosellconnectors/salesforce13.png" alt-text="Observera anslutningar":::

### <a name="edit-the-connections"></a>Redigera anslutningarna

1. Gå tillbaka till sidan Lösningar och välj **Standardlösning.**  Välj **Anslutningsreferens (förhandsversion) genom att** klicka på **Alla.**
 
:::image type="content" source="images/cosellconnectors/salesforce14.png" alt-text="Börja redigera anslutningsappen":::

2. Redigera var och en av anslutningarna individuellt genom att välja ikonen med tre punkter. Lägg till relevanta anslutningar.

:::image type="content" source="images/cosellconnectors/salesforce15.png" alt-text="Redigera anslutningsappar":::

3. Aktivera flöden i följande ordning:

- Registrering av Webhook i Partnercenter (insiderförhandsvisning)
- Skapa hänvisning till säljförsäljning – Salesforce till Partner Center (insiderförhandsvisning)
- Partner Center Microsoft Co-sell Referral Updates to Salesforce (Insider Preview)
- Partner Center till Salesforce (insiderförhandsvisning)
- Salesforce till Partner Center (Insider Preview)
- Salesforce Opportunity to Partner Center (Insider Preview)
- Salesforce Microsoft Solutions to Partner Center (Insider Preview)

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a>Använda Webhook-API:er för att registrera dig för resursändringshändelser

Med Partner Center Webhook-API:er kan du registrera dig för resursändringshändelser. Dessa ändringshändelser skickas till din URL som HTTP-inlägg.

1. Om du vill registrera din URL väljer **du PartnerCenter Webhook Registration (Insider Preview)** Power Automate flow.

2. Lägg till anslutningar för (a.) Partner Center-användare med referenser administratörsautentiseringsuppgifter (b.) Partner Center-händelser enligt nedan

   :::image type="content" source="images/cosellconnectors/triggerflow.png" alt-text="Utlösare":::

3. När du gör dessa uppdateringar visas

   :::image type="content" source="images/cosellconnectors/webhook1.png" alt-text="Webhooks":::

4. Spara ändringarna och välj **Aktivera**.

   Utför följande steg för att aktivera Partnercenter-webhooks för att lyssna på händelseändringar:

5. Välj **Partner Center till Salesforce CRM (Insider Preview).**

6. Välj ikonen **Redigera** och välj När **en HTTP-begäran tas emot.**

7. Välj ikonen **Kopiera för** att kopiera den angivna HTTP POST-URL:en.

   :::image type="content" source="images/salesforce/copy-url.png" alt-text="Kopiera URL":::

8. Välj nu flödet "Partner Center Webhook Registration (Insider Preview)" och Power Automate **kör**.

9. Kontrollera att fönstret "Kör flöde" öppnas i den högra rutan och välj **Fortsätt.**

10. Ange följande information:

    1. **Http-utlösarslutpunkt:** URL som kopierades från ett tidigare steg

    2. **Händelser att registrera:**"referral-created" och "referral-updated"

    3. **Skriva över befintliga utlösarslutpunkter om de finns**: Ja (detta skriver över befintliga slutpunkter.)

11. Välj **Kör** och sedan **Klar.**

Webhooken kan nu lyssna efter händelser som skapas och uppdateras.

## <a name="customize-synchronization-steps"></a>Anpassa synkroniseringssteg

När hänvisningar till säljförsäljning synkroniseras mellan Partner Center och ditt CRM-system visas fälten som synkroniseras på Partner Center-datorn här.

CRM-system är ofta mycket anpassade. Du kan anpassa Power Automate flöden. Följ guiden för fältmappning och gör vid behov lämpliga ändringar i stegen i Power Automate flöden.  Microsoft Partner Centers till CRM-mappningar tillhandahålls, men baserat på din CRM-miljö kan du välja att anpassa fälten ytterligare.

Flera steg i varje Power Automate kan anpassas efter dina behov. Följande är exempel på tillgängliga anpassningar:

1. Anpassa fälten för skapa eller uppdatera händelser i Partnercenter för CRM-referenssynkronisering:

   1. Välj Partner Center till Salesforce CRM (Insider Preview).

   2. Välj **Redigera** för att redigera/anpassa Power Automate flöde.

   3. Välj **(Omfång) Synkronisera leadet eller affärsmöjligheten**.

2. Om du vill anpassa CRM-fältmappningar för att skapa **händelser väljer du Om det är en ny delad affärsmöjlighet och sedan**. Välj understeget om **ja och** expandera sedan Skapa en ny affärsmöjlighet **i CRM.** Du kan redigera mappningarna i det här avsnittet med hjälp av guiden Fältmappning.

   1. Om du vill anpassa CRM-fältmappningar för uppdateringshändelser väljer du steget "(Omfång) Synkronisera leadet eller affärsmöjligheten".

   2. Välj **Om det är en uppdatering av en affärsmöjlighet, sedan**. Välj understeget **om ja och** expandera sedan If difference between the opportunity objects in Partner Center and CRM (Om skillnaden mellan **affärsmöjlighetsobjekten i Partnercenter och CRM) och sedan**.  

   3. Välj **Om ja följt** av Uppdatera befintlig **affärsmöjlighet**

3. Så här anpassar du fälten för referenssynkronisering för CRM till dator för uppdateringshändelser:

   1. Välj **Redigera**  för att redigera/anpassa Power Automate flöde.

   2. Välj **(Omfång) Synkronisera affärsmöjligheten**.

   3. Om du vill anpassa CRM-fältmappningar (baserat på guiden för fältmappningar) för uppdateringshändelser väljer du Om det är skillnad mellan leadobjekten i **Partnercenter och CRM och sedan**.

   4. Välj understeget **om ja och** expandera sedan steget Uppdatera en referens med **affärsmöjlighetsdata**.

   Du kan redigera mappningarna i det här avsnittet baserat på guiden Fältmappning.

4. Vill du anpassa fälten för referenssynkronisering för CRM till dator för att skapa händelser?

   1. Välj **Redigera**  för att redigera/anpassa Power Automate flöde.

   2. Välj **(Omfång) Synkronisera referenser.**

   3. Om du vill anpassa CRM-fältmappningar (baserat på guiden för fältmappningar) för att skapa händelser väljer **du Skapa Microsoft-hänvisning.**

Du kan redigera mappningarna i det här avsnittet baserat på guiden Fältmappning.


## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a>Dubbelriktad synkronisering av hänvisningar från end-to-end

När du har installerat, konfigurerat och anpassat Power Automate lösningen kan du testa synkroniseringen av hänvisningar till säljförsäljning mellan Salesforce CRM och Partner Center.

### <a name="pre-requisites"></a>Förutsättningar

För att synkronisera hänvisningarna mellan Partner Center och Salesforce CRM Power Automate lösningen tydligt avgränsa Microsoft-specifika hänvisningsfält. Den här identifieringen ger dina säljteam möjlighet att bestämma vilka hänvisningar som de vill dela med Microsoft för samförsäljning.

En uppsättning anpassade fält är tillgängliga som en del av partnercentrets referenssynkronisering för Salesforce CRM-lösningens **affärsmöjlighetsentitet.** En CRM-administratörsanvändare måste skapa ett separat CRM-avsnitt med de anpassade **fälten** Affärsmöjlighet.

Följande anpassade fält ska vara en del av CRM-avsnittet:

- **Synkronisera med Partnercenter:** Om du vill synkronisera affärsmöjligheten med Microsoft Partner Center

- **Hänvisningsidentifierare:** Ett fält för skrivskyddade identifierare för Microsoft Partner Center-hänvisning

- **Hänvisningslänk:** En skrivskyddade länk till hänvisningen i Microsoft Partner Center

- **Hur kan Microsoft hjälpa till:** Hjälp krävs från Microsoft för hänvisningen

- **Produkter:** Lista över produkter som är associerade med den här affärsmöjligheten

- **Granskning:** En skrivskyddade granskningslogg för synkronisering med Partner Center-referenser

### <a name="scenarios"></a>Scenarier:

1. Hänvisningssynkronisering när hänvisning skapas eller uppdateras i CRM och synkroniseras i Partnercenter:

   1. Logga in på salesforce CRM-miljön med användare som har insyn i **avsnittet Affärsmöjlighet** i CRM.

   2. Se till att följande avsnitt visas när du skapar en "Ny affärsmöjlighet" i Salesforce CRM-miljön

      :::image type="content" source="images/salesforce/salesforce-scenario-1.png" alt-text="Salesforce-miljö":::

   3. Om du vill synkronisera den här affärsmöjligheten med Microsoft Partner Center måste du ange följande fält i kortvyn:

       - "Synkronisera med Partnercenter": Ja
       - "Hur kan Microsoft hjälpa?": Välj bland följande alternativ:
       - Produkter: Produktens lösnings-ID:er

   4. När du har angett alternativet Synkronisera  **med Partnercenter** för affärsmöjlighet till **Ja,** vänta i 10 minuter och logga in på ditt Partnercenter-konto. Dina hänvisningar synkroniseras med Salesforce CRM.

   5. När alternativet "Synkronisera med Partnercenter" är inställt på "Ja", kommer ändringarna att synkroniseras med ditt Partnercenter-konto om du uppdaterar affärsmöjligheten i Salesforce CRM.

   6. Affärsmöjligheter som har synkroniserats med Partnercenter identifieras med ✔icon i Salesforce CRM.

2. Referenssynkronisering när hänvisningar skapas eller uppdateras i Microsoft Partner Center och synkroniseras i Salesforce CRM-miljön:

    1. Logga in på instrumentpanelen i [Partnercenter.](https://partner.microsoft.com/dashboard/home)

    2. Välj **Referenser** på menyn till vänster.

    3. Skapa en ny hänvisning för säljförsäljning från Partnercenter genom att klicka på alternativet "Nytt avtal".

    4. Logga in på Salesforce CRM-miljön.

    5. Gå till **Öppna affärsmöjligheter.** Hänvisningen som skapades i Microsoft Partner Center synkroniseras nu i Salesforce CRM.

       :::image type="content" source="images/salesforce/salesforce-casino-e.png" alt-text="Skärmen Salesforce-affärsmöjlighet":::

    6. När du väljer en synkroniserad referens fylls kortvisningsinformationen i.

## <a name="next-steps"></a>Nästa steg

- [Hantera leads](manage-leads.md)

- [Hantera möjligheter till samförsäljning](manage-co-sell-opportunities.md)

- [Partnercenter – webhooks](/partner-center/develop/partner-center-webhooks)
