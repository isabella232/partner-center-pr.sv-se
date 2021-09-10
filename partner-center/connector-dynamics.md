---
title: Anslutningsappen för säljförsäljning för Dynamics 365 CRM Partner Center
description: Synkronisera hänvisningar i PartnerCenter med din säljpartner för Dynamics 365 CRM. Du kan sedan samförsäljninga med Microsoft inifrån ditt CRM-system.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-referrals
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.date: 03/01/2021
ms.openlocfilehash: 798a8a7d26480e8a1fc23bca3af45bd6a0e44778
ms.sourcegitcommit: 1161d5bcb345e368348c535a7211f0d353c5a471
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/09/2021
ms.locfileid: "123960306"
---
# <a name="co-sell-connector-for-dynamics-365-crm-overview"></a>Översikt över anslutningsappen för säljförsäljning för Dynamics 365 CRM

**Lämpliga roller:** Referensadministratörsroller | Systemadministratör eller systemanpassare för CRM

Partnercenter- och säljkopplingar gör det möjligt för säljarna att samförsäljninga med Microsoft inifrån dina CRM-system (Customer Relationship System). De behöver inte tränas för att använda Partner Center för att hantera samförsäljningserbjudanden. Använd anslutningsapparna för säljförsäljning för att skapa en ny hänvisning till säljförsäljning för att:

- Engagera en Microsoft-säljare
- Ta emot hänvisningar från Microsoft-säljaren
- Acceptera eller avvisa hänvisningar
- Ändra avtalsdata, till exempel avtalsvärde och slutdatum 
 
Du kan också få uppdateringar från Microsofts säljare om dessa samförsäljningserbjudanden. Du kan hantera alla hänvisningar som fungerar i valfri CRM i stället för i Partnercenter.

Lösningen är baserad på Power Automate och använder Partner Center-API:er.

## <a name="prerequisites"></a>Förutsättningar

Kontrollera att du uppfyller följande krav innan du installerar lösningen.

| Ämnen   | Information   | Länkar   |
|--------------|--------------------|------|
| MICROSOFT PARTNER NETWORK -ID (MPN) |Du behöver ett giltigt MPN-ID. | [Anslut till partnernätverket](https://partner.microsoft.com/) |
| Redo för säljförsäljning|Din IP-/tjänstlösning måste vara redo för säljförsäljning. | [Sälja med Microsoft](https://partner.microsoft.com/membership/sell-with-microsoft) |
| Partnercenter-konto | MPN-ID:t som är associerat med Partnercenter-klienten måste vara samma som det MPN-ID som är associerat med din säljpartnerlösning. Kontrollera att du kan se dina hänvisningar till säljförsäljning i Partnercenter-portalen innan du distribuerar anslutningsapparna. | [Hantera ditt konto](create-user-accounts-and-set-permissions.md) |
| Användarroller i Partnercenter | Medarbetaren som ska installera och använda anslutningsapparna måste vara referensadministratör.|[Tilldela användarroller och -behörigheter](create-user-accounts-and-set-permissions.md) |
| Dynamics 365 CRM|CRM-användarrollen är Systemadministratör eller Systemanpassare.|[Tilldela roller i Dynamics 365](/dynamics365/customerengagement/on-premises/customize/privileges-required-customization) |
| Power Automate flödeskonto|Skapa en ny produktionsmiljö med en databas för testning, mellanlagring och produktion. Om du har en befintlig produktionsmiljö med en databas kan den återanvändas. Den användare som ska installera anslutningslösningen måste ha en Power Automate och åtkomst till den här miljön. Du kan övervaka förloppet och få mer information [i Power Automate](https://flow.microsoft.com/) om installationen misslyckas. Välj **Visa historik** under **Lösningar**. | [Skapa eller hantera miljö](/power-platform/admin/create-environment#create-an-environment-with-a-database) |

## <a name="install-partner-center-referrals-synchronization-for-dynamics-365-power-automate-solution"></a>Installera synkronisering av partnercenterreferenser för Dynamics 365 (Power Automate lösning)

1. Gå [till Power Automate](https://flow.microsoft.com)och **välj Miljöer** i det övre högra hörnet. I det här steget visas de tillgängliga CRM-instanserna.

2. Välj lämplig CRM-instans i listrutan i det övre högra hörnet.

3. Välj **Lösningar** till vänster.

4. Välj länken **Öppna AppSource** på den översta menyn.

   :::image type="content" source="images/cosellconnectors/open-appsource.png" alt-text="Skärmbild som visar Open AppSource.":::

5. Sök efter **partnercenterreferenser för Dynamics 365** på popup-skärmen.  

6. Välj **knappen Hämta nu** och välj sedan **Fortsätt.**

7. En sida visas där du kan välja CRM-miljön (Dynamics 365) för att installera programmet. Godkänn villkoren.

8. Du kan övervaka förloppet och om installationen misslyckas kan du få mer information i Power Automate välja **Se historik** under **Lösningar**.

9. När installationen är klar går du tillbaka [till Power Automate](https://flow.microsoft.com) och **väljer Lösningar** till vänster. **Synkronisering av partnercenterreferenser för Dynamics 365** finns nu i **listan över** lösningar.

10. Välj **Synkronisering av referenssynkronisering i Partnercenter för Dynamics 365.** Följande flöden Power Automate och entiteter är tillgängliga.

    :::image type="content" source="images/cosellconnectors/dynamics-available-crms.png" alt-text="Skärmbild som visar tillgängliga CRM:er.":::

## <a name="test-before-you-go-live"></a>Testa innan du går live

Innan du installerar, konfigurerar och anpassar Power Automate-lösningen i produktionsmiljön testar du lösningen på en CRM-mellanlagringsinstans. Du måste:

- Installera lösningen Power Automate en CRM-instans i en mellanlagringsmiljö.
- Konfigurera och anpassa Power Automate i en mellanlagringsmiljö.
- Testa lösningen på en crm-mellanlagringsinstans.
- Efter ett lyckat test importerar du som en hanterad lösning till produktionsinstansen.

## <a name="configure-the-solution"></a>Konfigurera lösningen

1. När du har installerat lösningen i din CRM-instans går du tillbaka till [Power Automate](https://flow.microsoft.com/).

2. I **listrutan Miljöer** i det övre högra hörnet väljer du den CRM-instans där du installerade Power Automate lösningen.

3. Du måste skapa anslutningar som associerar de tre användarkontona:

   - PartnerCenter-användare med referensadministratörsautentiseringsuppgifter
   - Partnercenter-händelser
   - CRM-administratör med Power Automate flöden i lösningen

   a. Välj **Anslutningar** till vänster och välj lösningen **Partnercenter-referenser** i listan.

   b. Skapa en anslutning genom att välja **Skapa en anslutning.**

      :::image type="content" source="images/cosellconnectors/dynamics-1.png" alt-text="Skärmbild som visar Skapa en anslutning.":::

   c. Sök efter **Referenser till Partnercenter (förhandsversion)** i sökfältet i det övre högra hörnet.

   d. Skapa en anslutning för din Partnercenter-användare med rollen Referensadministratör.

   e. Skapa sedan en partnercenterhändelser-anslutning för din Partnercenter-användare med autentiseringsuppgifterna som referensadministratör.

   f. Skapa en anslutning för Common Data Service (aktuell miljö) för CRM-administratörsanvändaren.
     
   ex. När du har lagt till alla anslutningar bör du se följande anslutningar i din miljö.

      :::image type="content" source="images/cosellconnectors/dynamics-2.png" alt-text="Skärmbild som visar anslutningar.":::

## <a name="edit-the-connections"></a>Redigera anslutningarna

1. Gå tillbaka till **sidan** Lösningar och välj **Standardlösning.** Välj **Anslutningsreferens (förhandsversion) genom** att välja **Alla.**

   :::image type="content" source="images/connection-reference-video.gif" alt-text="Skärmbild som visar Redigering av anslutningarna.":::

2. Redigera var och en av anslutningarna individuellt genom att välja ellipsikonen. Lägg till relevanta anslutningar.

   :::image type="content" source="images/cosellconnectors/dynamics-4.png" alt-text="Skärmbild som visar anslutningar i listan.":::

3. Gå tillbaka till **sidan** Lösningar, välj Partnercenter-referenssynkronisering för **Dynamics 365** och aktivera flödet genom att välja ellipsikonen bredvid varje flöde i följande sekvens. Om du stöter på problem när du aktiverar flödet kan du gå till [Anpassningssteg](connector-dynamics.md#customize-synchronization-steps) och [Felsökningssteg.](connectors-troubleshoot.md)

   Aktivera flöden i följande ordning:

   a. Partner Center Webhook Registration (Insider Preview)
   
   b. [Anpassa] Skapa eller hämta information från Dynamics 365-flöde
   
   c. Skapa hänvisning till säljpartner – Dynamics 365 till PartnerCenter (Insider Preview)
   
   d. PartnerCenter till Dynamics 365 – Helper (Insider Preview)
   
   e. Partnercenter Microsoft Co-sell Hänvisningsuppdateringar till Dynamics 365 (Insider Preview)
   
   f. PartnerCenter till Dynamics 365 (Insider Preview)
   
   ex. Dynamics 365 till Partner Center (Insider Preview)
   
   h. Dynamics 365 Opportunity to Partner Center (Insider Preview)
   
   i. Dynamics 365 Microsoft Solutions to Partner Center (Insider Preview)
 
## <a name="use-webhook-apis-to-register-for-resource-change-events"></a>Använda webhook-API:er för att registrera för resursändringshändelser

Du kan använda Partner Center-webhook-API:er för att registrera dig för resursändringshändelser. Dessa ändringshändelser skickas till din URL som HTTP-inlägg.

1. Välj **Partnercenter till Dynamics 365 (Insider Preview).**

2. Välj ikonen **Redigera** och välj När **en HTTP-begäran tas emot.**

3. Välj ikonen **Kopiera för** att kopiera den angivna HTTP POST-URL:en.

   :::image type="content" source="images/webhook-video.gif" alt-text="Skärmbild som visar hur du registrerar resursändringar med hjälp av webhooks.":::

4. Välj flödet **Partnercenter Webhook Registration (Insider Preview)** Power Automate och välj sedan **Kör.**

5. Kontrollera att **fönstret Kör flöde** öppnas i den högra rutan och välj **Fortsätt.**

6. Ange följande information:

   - **Http-utlösarslutpunkt:** Den här URL:en kopierades från ett tidigare steg.
   - **Händelser att registrera:** Välj alla tillgängliga händelser ( hänvisningsskapade, hänvisnings-uppdaterade, **relaterade-hänvisningsskapade** och **relaterade-hänvisnings-uppdaterade**).
   - **Skriva över befintliga utlösarslutpunkter om de finns?**: Ja. Endast en URL kan registreras för en viss webhook-händelse.

7. Välj **Kör flöde** och välj sedan **Klar.**

Webhooken kan nu lyssna på, skapa och uppdatera händelser.

## <a name="customize-synchronization-steps"></a>Anpassa synkroniseringssteg

CRM-system är mycket anpassade och du kan anpassa Power Automate baserat på din CRM-konfiguration. När hänvisningar till säljförsäljning synkroniseras mellan Partner Center och ditt CRM-system visas fälten som synkroniseras på Partner Center-datorn i guiden Anpassad [fältmappning.](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWxL6S)

Följ guiden för fältmappning och gör vid behov lämpliga ändringar i [Anpassa] Skapa eller Hämta information från **Dynamics 365-flöde** eller miljövariabler. Uppdatera inte andra flöden i den här Power Automate eftersom det kan påverka framtida lösningsuppgraderingar.

Följande anpassningar är tillgängliga:

- **Visa bockmarkering** i affärsmöjlighetens namn: Som standard visas en bock bredvid affärsmöjlighetsnamnet för att indikera att synkroniseringen mellan Partner Center och Dynamics 365 CRM har genomförts. På samma sätt visas ett korsmarkering om synkroniseringen misslyckas. För att undvika att lägga till en bock eller korsmarkering i affärsmöjlighetens namn anger du det aktuella värdet för kryssmarkeringen Visa i **miljövariabeln affärsmöjlighetsnamn** till Nej.
- **Avtalsvärde:** Som standard synkroniseras avtalsvärdet från Partnercenter till och `estimatedvalue` från i CRM. Om du har ett annat fält i CRM som avtalsvärdet ska synkroniseras från:

  - Uppdatera fältet **Deal value** (Avtalsvärde) i Dynamics 365-miljövariabeln med CRM-fältnamnet. Se till att du anger fältets namn, inte dess visningsnamn.
  - Redigera [Anpassa] Skapa eller Hämta information från **Dynamics 365-flödet** och gå till Skapa  eller uppdatera **affärsmöjlighet** i CRM och uppdatera **Skapa** en ny affärsmöjlighet och Uppdatera befintliga affärsmöjlighetsåtgärder för att tilldela **DealValue-värdet** till rätt fält i CRM. Ta även bort **DealValue-tilldelningen** från **fältet Estimated Revenue (Beräknade** intäkter).

- **Landskod för kundkonto:** Du måste ange en landskod med två bokstäver (ISO 3166) när du skapar en ny referens. Som standard synkroniseras landskoden till och från kontots address1_country **i** CRM. Om du har ett annat fält i CRM som landskoden ska synkroniseras från:

  - För ett fält med landskod som inte är letar efter i kontot som innehåller en tvåbokstavskod uppdaterar du fältnamnet Customer **Account Country Code** i Dynamics 365-miljövariabeln med CRM-fältets fältnamn. Se till att du anger fältets namn, inte dess visningsnamn. Redigera [Anpassa] Skapa eller Hämta information från **Dynamics 365-flödet** och gå till Skapa eller hämta kundkonto i CRM-åtgärden för att tilldela ett **land-värde** till rätt fält i CRM.  Ta även bort **värdetilldelningen** Land från **fältet Adress 1: Land/region.**

  - För ett uppslagsbaserat landskodfält i kontot lägger du till ett nytt anpassat fält i kontot och fyller i det automatiskt med en landskod med två bokstäver (ISO 3166) baserat på det värde som valts i det uppslagsbaserade fältet och vice versa. Följ föregående steg för fältet landskod för icke-letarad för att synkronisera ett nytt anpassat fält från CRM till och från Partnercenter.

- **Affärsmöjlighetsfält:** Om det  finns obligatoriska fält i Affärsmöjlighet som måste fyllas i redigerar du [Anpassa]  Skapa eller Hämta information från **Dynamics 365-flödet** och går till Skapa eller uppdatera affärsmöjlighet i CRM och uppdaterar **Skapa** en ny affärsmöjlighetsåtgärd för att tilldela värden till de obligatoriska fälten baserat på dina affärsbehov.
- **Leadfält:** Om det finns  obligatoriska fält i Lead som måste fyllas i redigerar du [Anpassa] Skapa eller Hämta information från **Dynamics 365-flödet** och går till Skapa eller uppdatera **lead** i CRM och uppdatera Skapa en ny **leadåtgärd** för att tilldela värden till de obligatoriska fälten baserat på dina affärsbehov.
- **Kundkonto:** När en ny referens synkroniseras från PartnerCenter till CRM försöker Power Automate-lösningen söka efter ett befintligt konto i CRM med hjälp av kundens företagsnamn och postnummer. Om den inte hittar något skapas ett nytt kundkonto i CRM. Om du vill uppdatera sökvillkoren och information om skapande av nytt konto redigerar du [Anpassa] Skapa eller Hämta information från **Dynamics 365-flödet** och går till **Skapa** eller hämta kundkonto i CRM- och **Skapa kundkontoåtgärden**.

## <a name="update-environment-variable"></a>Uppdatera miljövariabel

Så här uppdaterar du ett miljövariabelvärde:

1. Gå till **sidan Lösningar** och välj **Standardlösning.** Välj **Miljövariabel** genom att välja **Alla.**

2. Välj miljövariabeln för det värde som behöver uppdateras och välj **Redigera med** hjälp av ellipsikonen.

3. Uppdatera **aktuellt värde** (uppdatera inte **standardvärdet**) med hjälp av **alternativet Nytt** värde och ange värdet. Värdet måste matcha variabelns datatyp. Till exempel accepterar datatypen Ja eller Nej antingen värdet Ja eller Nej.

   :::image type="content" source="images/cosellconnectors/environment-variables-video.gif" alt-text="Skärmbild som visar Uppdatera miljövariabler.":::

## <a name="end-to-end-bidirectional-co-sell-referral-synchronization"></a>Dubbelriktad synkronisering av säljförsäljningsreferenser från end till end

När du har installerat, konfigurerat och anpassat Power Automate-lösningen kan du testa synkroniseringen av hänvisningar till säljpartner mellan Dynamics 365 och Partnercenter.

### <a name="prerequisites"></a>Förutsättningar

För att synkronisera hänvisningarna i Partner Center och Dynamics 365 CRM avgränsar Power Automate-lösningen tydligt Microsoft-specifika referensfält. Den här identifieringen ger säljteamen möjlighet att bestämma vilka hänvisningar de vill dela med Microsoft för säljförsäljning.

En uppsättning anpassade fält och objekt läggs till som en del av lösningsinstallationen. En CRM-administratörsanvändare måste skapa ett separat CRM-avsnitt med de **anpassade affärsmöjlighetsfälten.**

Följande anpassade fält bör ingå i CRM-avsnittet:

- **Synkronisera med Partnercenter:** Om du vill synkronisera affärsmöjligheten med Partnercenter. Som standard är värdet för det här fältet Nej och måste uttryckligen anges till Ja av din säljare för att dela en affärsmöjlighet med Microsoft. Nya referenser som delas från Partner Center till CRM har det här fältvärdet inställt på Ja.
- **Hänvisningsidentifierare:** Ett skrivskyddade identifierarfält för PartnerCenter-hänvisningen.
- **Hänvisningslänk:** En skrivskyddade länk till hänvisningen i Partnercenter.
- **Hur kan Microsoft hjälpa till?**: Hjälp krävs av Microsoft för hänvisningen. Om du vill skapa en hänvisning om säljförsäljning väljer du lämplig hjälp som krävs av Microsoft. En kundkontakt måste kopplas till möjligheten att skapa en hänvisning för säljförsäljning. Välj inte det här fältet om du vill skapa en referens för icke-säljförsäljning. En hänvisning som inte gäller säljförsäljning kan konverteras till en hänvisning om säljförsäljning när som helst genom att välja lämpligt alternativ som krävs för hjälp.
- **Referenssynlighet för Microsoft Partner Center:** Välj synlighet för Partnercenter-hänvisningen. Genom att göra den synlig för Microsoft-säljare kan en hänvisning om icke-säljande kan konverteras till samförsäljning. När Microsoft-hjälp krävs är referensen synlig för Microsoft-säljare som standard. När det här fältet har markerats som synligt kan det inte återställas.
- **Microsoft CRM identifierare:** När en hänvisning om säljförsäljning skapas och godkänns av Microsoft fylls det här fältet i med Microsofts CRM-identifierare.
- **Produkter: Föråldrad:** Använd inte det här fältet eller lägg till det i CRM-avsnittet. Den är endast tillgänglig för bakåtkompatibilitet. Använd Partner Center-lösningar i stället.
- **Granskning:** En skrivskyddade granskningslogg för synkronisering med PartnerCenter-referenser.
- **Microsoft Partner Center-lösningar:** Ett anpassat objekt för att associera lösningar som är redo för säljförsäljning eller Microsoft-lösningar med affärsmöjligheten. En eller flera lösningar kan läggas till eller tas bort från affärsmöjligheten. Det är obligatoriskt att lägga till minst en säljklar eller Microsoft-lösning till affärsmöjligheten innan du delar den med Microsoft. Om du vill associera det här objektet med affärsmöjligheten uppdaterar du **formuläret Affärsmöjlighet** i CRM.

  Välj lämplig flik i formuläret **Affärsmöjlighet** och lägg till ett underrutnät enligt det som visas här.

  :::image type="content" source="images/cosellconnectors/dynamics-6.png" alt-text="Skärmbild som visar formuläret Affärsmöjlighet.":::

  :::image type="content" source="images/cosellconnectors/dynamics-7.png" alt-text="Skärmbild som visar Microsoft Solutions.":::

- När du har lagt till Microsoft-lösningar kan du fylla i information om säljklara lösningar i förväg så att säljarna inte behöver lägga till dem. Om du vill lägga till en ny lösningsinformation går  du till objektet Microsoft Solution Details i CRM och väljer Lägg till post för att lägga till en post eller använder **Excel upload** för att lägga till flera poster.

  :::image type="content" source="images/cosellconnectors/dynamics-solution-1.png" alt-text="Skärmbild som visar information om ny Microsoft-lösning.":::

### <a name="scenarios"></a>Scenarier

1. Hänvisningssynkronisering när hänvisning skapas eller uppdateras i CRM och synkroniseras i Partnercenter:

   1. Logga in på dynamics 365 CRM-miljön med den användare som har insyn i **avsnittet Affärsmöjlighet** i CRM.

   1. Se till att **avsnittet Microsoft Partner Center** visas när du skapar en ny affärsmöjlighet i Dynamics 365-miljön.

      :::image type="content" source="images/cosellconnectors/dynamics-solution-2.png" alt-text="Skärmbild som visar Ny affärsmöjlighet.":::

   1. Om du vill synkronisera den här affärsmöjligheten med Partnercenter måste du ange följande fält i kortvyn:

      - **Hur kan Microsoft hjälpa till?**: Om du vill skapa en hänvisning till säljförsäljning väljer du ett lämpligt hjälpalternativ.

         :::image type="content" source="images/cosellconnectors/dynamics-solution-3.png" alt-text="Skärmbild som visar hur du hämtar lämpliga fält i kortvyn.":::

      - **Kundkontakt:** Om du vill skapa en hänvisning till säljförsäljning lägger du till en kundkontakt till affärsmöjligheten.
      - **Synkronisera med Partnercenter:** Ja.
      - **Microsoft-lösningar:** Om du vill dela en hänvisning med Microsoft lägger du till en giltig säljklar eller Microsoft-lösning till affärsmöjligheten.

        :::image type="content" source="images/cosellconnectors/dynamics-solution-4.png" alt-text="Skärmbild som visar lösnings-ID.":::

   1. När affärsmöjligheten har skapats i Dynamics 365 med alternativet Synkronisera med **Partnercenter** inställt på Ja väntar du 10 minuter. Logga sedan in på ditt Partnercenter-konto. Dina hänvisningar synkroniseras med Dynamics 365 och **hänvisningsidentifieraren**. **Referenslänken** fylls i. Om det uppstår ett fel **fylls fältet** Granskning i med felinformation.

      1. På samma sätt synkroniseras ändringarna i ditt Partnercenter-konto för en affärsmöjlighet med alternativet Synkronisera med **Partnercenter** inställt på Ja. Om du uppdaterar affärsmöjligheten i Dynamics 365 CRM.

      1. Affärsmöjligheter som har synkroniserats med Partnercenter identifieras med ✔ikon i Dynamics 365.

1. Hänvisningssynkronisering när hänvisningen skapas eller uppdateras i Partnercenter och synkroniseras i Dynamics 365-miljön:

   1. Logga in på instrumentpanelen i [Partnercenter.](https://partner.microsoft.com/dashboard/home)

   1. Välj **Referenser på** den vänstra menyn.

   1. Skapa en ny hänvisning till säljförsäljning från Partnercenter genom att välja **alternativet Nytt** avtal.

   1. Logga in på din Dynamics 365 CRM-miljö.

   1. Gå till **Öppna affärsmöjligheter.** Hänvisningen som skapades i Partnercenter synkroniseras nu i Dynamics 365 CRM.

   1. När du väljer en synkroniserad referens fylls kortvisningsinformationen i.

## <a name="next-steps"></a>Nästa steg

- [Hantera leads](manage-leads.md)
- [Hantera möjligheter till samförsäljning](manage-co-sell-opportunities.md)
- [Mer om Microsoft Power Automate plattform](/power-automate/)
- [Partnercenter – webhooks](/partner-center/develop/partner-center-webhooks)
