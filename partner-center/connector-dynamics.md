---
title: Co-Sälj koppling för Dynamics 365 CRM-partner Center
description: Synkronisera referenser i Partner Center med ditt Co-sälje Connector för Dynamics 365 CRM. Säljare kan sedan sälja tillsammans med Microsoft från dina CRM-system.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.date: 03/01/2021
ms.openlocfilehash: 1b0f8f12cf60db0dcc03aae24316e869cbf34376
ms.sourcegitcommit: d7fbaff51c7ac29fbf700d7f7fdef798fd97c6fa
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/10/2021
ms.locfileid: "102619417"
---
# <a name="co-sell-connector-for-dynamics-365-crm--overview"></a>Co-Sälj koppling för Dynamics 365 CRM – översikt

### <a name="appropriate-roles"></a>Lämpliga roller

- Referens administratör
- System administratör eller systemanpassare på CRM

Partner Center Co-sälje Connector gör det möjligt för dina säljare att sälja med Microsoft från dina CRM-system. De behöver inte tränas att använda Partner Center för att hantera samförsäljnings avtal. Använd Co-Sälj-anslutningarna för att skapa en ny samförsäljnings hänvisning för att engagera en Microsoft-säljare, ta emot hänvisningar från Microsoft-säljaren, acceptera/neka referenser, ändra avtals data som avtals värde och stängnings datum. Du kan också ta emot uppdateringar från Microsoft-säljarna om dessa samförsäljnings avtal. Du kan hantera alla dina referenser på önskat alternativ i CRM och inte i Partner Center. 

Lösningen baseras på Microsoft Power automatiserings lösning och använder API: er för partner Center.

## <a name="before-you-install---pre-requisites"></a>Innan du installerar-krav

|**Ämnen**   |**Information**   |**Länkar**   |
|--------------|--------------------|------|
|Microsoft Partner Network-ID |Du behöver ett giltigt MPN-ID|För att ansluta till [MPN](https://partner.microsoft.com/)|
|Färdiga försäljnings produkter|Din lösning för IP/tjänster måste vara samförsäljnings klar.|[Sälj med Microsoft](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|Partnercenter-konto|Det MPN-ID som är kopplat till Partner Center-klienten måste vara samma som det MPN-ID som är kopplat till din co-Sälj-lösning. Kontrol lera att du kan se dina samförsäljnings referenser på Partner Center-portalen innan du distribuerar anslutningarna.|[Hantera ditt konto](create-user-accounts-and-set-permissions.md)|
|Användar roller för partner Center|Den medarbetare som ska installera och använda anslutningarna måste vara en referens administratör|[Tilldela användarroller och -behörigheter](create-user-accounts-and-set-permissions.md)| 
|Dynamics 365 CRM|Användar rollen CRM är system administratör eller systemanpassare|[Tilldela roller i Dynamics 365](/dynamics365/customerengagement/on-premises/customize/privileges-required-customization)|
|Flödes konto för automatiserad energi|Skapa en ny produktions miljö med databasen för test/mellanlagring och produktion. Om du har en befintlig produktions miljö med databas kan den användas igen. Användaren som ska installera anslutnings lösningen måste ha en automatisk energi licens och åtkomst till den här miljön. Du kan övervaka förloppet och få mer information om att installationen Miss kan [automatiseras](https://flow.microsoft.com/) genom att klicka på Visa historik under lösningar.|[Skapa eller hantera miljö](/power-platform/admin/create-environment#create-an-environment-with-a-database)|

## <a name="install-partner-center-referrals-synchronization-for-dynamics-365-power-automate-solution"></a>Installera synkronisering av Partner Center-referenser för Dynamics 365 (energi automatiserings lösning)

1. Gå till [Power automatisera](https://flow.microsoft.com) och välj **miljöer** i det högra övre hörnet. I det här steget visas tillgängliga CRM-instanser.

2. Välj lämplig CRM-instans i list rutan i det högra övre hörnet.

3. Välj **lösningar** i det vänstra navigerings fältet.

4. Klicka på länken **Öppna AppSource** på den översta menyn.

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="Öppna AppSource":::

5. Sök efter **partner Center-referenser till kopplingar för Dynamics365** på popup-skärmen.  

6. Klicka på knappen **Hämta nu** och **Fortsätt** sedan.

7. Då öppnas sidan där du kan välja CRM-miljön (Dynamics 365) för att installera programmet.  Godkänn de allmänna villkoren.

8. Du kan övervaka förloppet och få mer information om att installationen Miss kan automatiseras genom att klicka på **Visa historik** under **lösningar**.
 

9. När installationen är klar navigerar du tillbaka till [Automatisera](https://flow.microsoft.com) och väljer **lösningar** från det vänstra navigerings fältet. Observera att **synkroniseringen av Partner Center för Dynamics 365** är tillgänglig i lösnings listan.

10. Välj **synkronisering av Partner Center-referenser för Dynamics 365**. Följande energi flöden och entiteter är tillgängliga:

    :::image type="content" source="images/cosellconnectors/dynamics-available-crms.png" alt-text="Tillgängliga CRMS":::

## <a name="best-practice-test-before-you-go-live"></a>Bästa praxis: testa innan du går live

Innan du installerar, konfigurerar och anpassar den automatiserade energi lösningen i produktions miljön måste du testa lösningen på en mellanlagringsplatsen CRM-instans.

- Installera Microsoft Power automatiserings lösning på en mellanlagringsplatss miljö/CRM-instans.
- Konfigurera och anpassa Microsoft Power automatiserings lösning i mellanlagrings miljö.
- Testa lösningen på en mellanlagrings-/CRM-instans. 
- Vid lyckad, importera som hanterad lösning till produktions instansen. 

## <a name="configure-the-solution"></a>Konfigurera lösningen

1. När du har installerat lösningen i din CRM-instans går du tillbaka till [Energis par](https://flow.microsoft.com/).


2. I list rutan **miljöer** i det högra hörnet väljer du den CRM-instans där du installerade den automatiserade energi lösningen.

3. Du måste skapa anslutningar som associerar de tre användar kontona:

   - Partner Center-användare med referenser för administratörs behörighet

   - Partnercenter-händelser

   - CRM-administratören med de energi automatiserade flödena i lösningen.

      1. Välj **anslutningar** i det vänstra navigerings fältet och välj lösningen **partner Center referral** i listan.

      2. Skapa en anslutning genom att klicka på **skapa en anslutning**.

         :::image type="content" source="images/cosellconnectors/dynamics-1.png" alt-text="Skapa anslutning":::

      3. Sök efter **partner Center-referenser (för hands version)** i Sök fältet i det övre högra hörnet.

      4. Skapa en anslutning för din partner Center-användare med rollen autentiseringsuppgifter för referral admin.

      5. Skapa sedan en anslutning för partner Center-händelser för din partner Center-användare med autentiseringsuppgifterna för referral admin.

      6. Skapa en anslutning för Common Data Service (aktuell miljö) för CRM-administratörens användare.
     
      7. När du har lagt till alla anslutningar bör du se följande anslutningar i din miljö:

         :::image type="content" source="images/cosellconnectors/dynamics-2.png" alt-text="Anslutningar":::
   
## <a name="edit-the-connections"></a>Redigera anslutningarna

1. Gå tillbaka till sidan **lösningar** och välj **standard lösning**. Välj **anslutnings referens (för hands version)** genom att klicka på **alla**.

   :::image type="content" source="images/connection-reference-video.gif" alt-text="Redigera anslutningarna":::

2. Redigera varje anslutning en i taget genom att välja ikonen tre punkter. Lägg till relevanta anslutningar.

   :::image type="content" source="images/cosellconnectors/dynamics-4.png" alt-text="Anslutningar i listan"::: 

3.  Gå tillbaka till sidan lösningar, Välj Partner Center-synkronisering för Dynamics 365 och aktivera flödet genom att klicka på tre punkter-ikon bredvid varje flöde i följande ordning. Om du stöter på problem när du aktiverar flödet kan du läsa [anpassnings steg](connector-dynamics.md#customize-synchronization-steps) och [fel söknings steg](connectors-troubleshoot.md). 

Aktivera flödena i följande ordning:

- Partner Center – registrering av webhook (Insider Preview)
- Skapa samförsäljnings hänvisning – Dynamics 365 till Partner Center (Insider Preview)
- Anpassad Skapa eller hämta information från Dynamics 365-flödet 
- Partner Center till Dynamics 365-Helper (Insider Preview)
- Partner Center Microsoft Co-Sälj hänvisnings uppdateringar till Dynamics 365 (Insider Preview)
- Partner Center till Dynamics 365 (Insider Preview)
- Dynamics 365 till Partner Center (Insider Preview)
- Dynamics 365-möjlighet till Partner Center (Insider Preview)
- Dynamics 365 Microsoft-lösningar till Partner Center (Insider Preview)
 

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a>Använda webhook-API: er för att registrera för resurs ändrings händelser

Med API: er för webhook i Partner Center kan du registrera för resurs ändrings händelser. De här ändrings händelserna skickas till din URL som HTTP-inlägg.

1. Välj **partner Center till Dynamics 365 (Insider Preview)**.

2. Välj **redigerings** ikonen och välj **när en http-begäran tas emot**.

3. Välj **kopierings** ikonen för att kopiera den tillhandahållna HTTP post-URL: en.

   :::image type="content" source="images/webhook-video.gif" alt-text="Registrera resurs ändringar med hjälp av Webhooks":::

4. Välj flödet "partner för webhook-registrering (Insider Preview)" i Power Center och välj **Kör**.

5. Se till att fönstret kör flöde visas i den högra rutan och klicka på **Fortsätt**.

6. Ange följande information:

   - **Http-utlösare slut punkt**: URL kopierad från föregående steg

   - **Händelser att registrera**: Välj alla tillgängliga händelser ("referral-created", "referral-updated", "relaterad-referral-created", "relaterad-referral-updated")

   -**Skriv över befintliga utlösare slut punkter om** den är tillgänglig: Ja är det viktigt att Observera att endast en URL kan registreras för en viss webhook-händelse. Det är viktigt att Observera att endast en URL kan registreras för en viss webhook-händelse. 

7. Välj **Kör** och välj sedan **Slutför.**

Webhooken kan nu lyssna på att skapa och uppdatera händelser.

## <a name="customize-synchronization-steps"></a>Anpassa synkroniserings steg

CRM-systemen är mycket anpassade och du kan anpassa den automatiserade lösningen baserat på din CRM-installation.  När samförsäljnings hänvisningar synkroniseras mellan partner Center och ditt CRM-system visas fälten som synkroniseras på Partner Center-datorn i [Guide för anpassad fält mappning](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWxL6S).

Följ guiden för fält mappning och om det behövs kan du göra lämpliga ändringar i **[anpassa] skapa eller hämta information från Dynamics 365 Flow**  -eller miljövariabler. Vi rekommenderar att du inte uppdaterar andra flöden i automatiserad automatiserad lösning eftersom det kan påverka framtida lösnings uppgraderingar. 

Följande är tillgängliga anpassningar:

- Bock markering i namn på affärs möjlighet: som standard visas en bock bredvid namnet på affärs möjlighet för att ange att synkroniseringen mellan partner Center och Dynamics 365 CRM sker. På samma sätt visas en kryss markering om det inte går att synkronisera. För att undvika att lägga till markering eller kors markering i affärs möjlighets namn, anger du det aktuella värdet för Visa markering i miljövariabeln för affärs möjlighets namn till Nej.

- Avtals värde: som standard synkroniseras det avtalade värdet från Partner Center till och från **estimatedvalue** i CRM. Om du har ett annat fält i CRM för att behandlas som synkroniseras från:

  a. Uppdatera fältet för ett värde fält i Dynamics 365-miljövariabeln med CRM: s fält namn. Observera att du ska ange fältets namn utan visnings namn.

  b. Redigera **[anpassa] skapa eller hämta information från Dynamics 365-flödet**  och navigera till **skapa eller uppdatera** affärs möjlighet i CRM och uppdatera **skapa en ny affärs möjlighet** och **Uppdatera befintliga affärs möjlighets** åtgärder för att tilldela **DealValue** -värde till rätt fält i CRM. Ta också bort **DealValue tilldelning** från fältet **uppskattat intäkt** .

- Landskod för kund konto: det är obligatoriskt att ange en landskod på två bokstäver (ISO 3166) när du skapar en ny hänvisning. Som standard synkroniseras lands koden till och från kontots address1_country fält i CRM. Om du har ett annat fält i CRM för lands kod som ska synkroniseras från:

   a. För ett fält för lands koder som inte är uppslag i ett konto som innehåller två tecken:

   - Uppdatera kund kontot lands kod fält namn i Dynamics 365-miljövariabeln med CRM: s fält namn. Observera att du ska ange fältets namn utan visnings namn.

   - Redigera **[anpassa] skapa eller hämta information från Dynamics 365-flödet**  och gå till skapa eller hämta kund konto i CRM-åtgärden för att tilldela lands värde till rätt fält i CRM. Ta också bort lands värde tilldelning från adress 1: fältet land/region.

   b. För ett lookup-baserat lands kod fält i kontot:

   - Lägg till ett nytt anpassat fält i kontot och fyll i det automatiskt med lands koden i två bokstäver (ISO 3166) baserat på värdet som valts i det uppslagna fältet och vice versa.

   - Följ stegen ovan för fältet lands kods ökning som inte är uppslag för att synkronisera nya anpassade fält från CRM till och från Partner Center.

- Affärs möjlighets fält: om det finns obligatoriska fält i affärs möjlighet som måste fyllas i redigera **[anpassa] skapa eller hämta information från Dynamics 365-flödet**  och navigera till **skapa eller uppdatera affärs möjlighet** i CRM och uppdatera **skapa en ny affärs möjlighets åtgärd** för att tilldela värden till de obligatoriska fälten utifrån dina affärs behov.

- Lead-fält: om det finns obligatoriska fält i lead som måste fyllas i redigera **[anpassa] skapa eller hämta information från Dynamics 365-flödet**  och navigera till **skapa eller uppdatera lead** i CRM och uppdatera **skapa en ny lead-åtgärd** för att tilldela värden till de obligatoriska fälten utifrån dina affärs behov.

- Kund konto: när en ny hänvisning synkroniseras från Partner Center till CRM försöker Power automatiserad lösning söka efter ett befintligt konto i CRM med hjälp av kundens företags namn och post nummer. Om den inte hittar något skapas ett nytt kund konto i CRM. Om du vill uppdatera Sök kriterierna och information om hur du skapar ett nytt konto redigerar du **[anpassa] skapa eller hämta information från Dynamics 365-flödet** och navigera till **skapa eller hämta kund konto** i CRM och **Skapa kund konto åtgärd**.

## <a name="update-environment-variable"></a>Uppdatera miljö variabel

Så här uppdaterar du ett miljö variabel värde:

1. Gå till **lösnings** sidan och välj **standard lösning**. Välj **miljö variabel** genom att klicka på alla.

2. Välj miljövariabeln för det värde som behöver uppdateras och klicka på **Redigera** med tre punkter-ikon.

3. Uppdatera **aktuellt värde** (uppdatera inte standardvärdet) med alternativet **nytt värde** och ange värdet. Värdet måste matcha data typen för variabeln, t. ex. Ja/Nej-data typen accepterar antingen ja eller inget värde.

   :::image type="content" source="images/environment-variables-video.gif" alt-text="Uppdatera miljövariabler":::

- Slutförd dubbelriktad referens synkronisering från slut punkt till slut punkt

När du har installerat, konfigurerat och anpassat den automatiserade lösningen för Energis par kan du testa synkroniseringen av samförsäljnings referenser mellan Dynamics 365 och partner Center.

### <a name="pre-requisites"></a>Förutsättningar

Om du vill synkronisera hänvisningarna mellan partner Center och Dynamics 365 CRM, kan du med hjälp av den automatiserade lösningen tydligt avgränsa Microsoft-/regionsspecifika hänvisnings fält. Den här identifieringen ger dina säljare möjlighet att bestämma vilka hänvisningar de vill dela med Microsoft för samförsäljning.

En uppsättning anpassade fält och objekt läggs till som en del av lösnings installationen. En administratörs användare i CRM måste skapa ett separat CRM-avsnitt med anpassade **affärs möjlighets** fält.

Följande anpassade fält ska ingå i CRM-avsnittet:

- **Synkronisera med partner Center**: om du vill synkronisera affärs möjligheten med Microsoft Partner Center. Som standard är värdet för det här fältet Nej och måste uttryckligen anges till Ja av din säljare för att dela en affärs möjlighet med Microsoft. Nya hänvisningar som delas från Partner Center till CRM har detta fält värde inställt på Ja.

- **Hänvisnings-ID**: ett skrivskyddat ID-fält för Microsoft Partner Center-hänvisning

- **Hänvisnings länk**: en skrivskyddad länk till hänvisningen i Microsoft Partner Center
- **Hur kan Microsoft hjälpa?**: hjälp krävs från Microsoft för hänvisning. Om du vill skapa en samförsäljnings hänvisning väljer du lämplig hjälp från Microsoft. En kund kontakt måste vara kopplad till möjligheten att skapa en samförsäljnings hänvisning. Om du vill skapa en icke-samförsäljnings referens lämnar du fältet avmarkerat. En icke-försäljnings hänvisning kan konverteras till en samförsäljnings hänvisning när som helst genom att välja lämplig hjälp som krävs.

- **Microsoft Partner Center hänvisnings synlighet**: Välj synlighet för Microsoft Partner Center-referens. Genom att göra det synligt för Microsofts säljare kan en icke-försäljnings referens konverteras till medförsäljning. När Microsoft-hjälpen krävs är hänvisningen synlig för Microsofts säljare som standard. Det går inte att återställa det här fältet när det har marker ATS som synligt.

- **Microsoft CRM-identifierare**: när en samförsäljnings hänvisning skapas och godkänns av Microsoft kommer det här fältet att fyllas i med Microsoft CRM-identifieraren.

- **Produkter: föråldrade** – Använd inte det här fältet eller Lägg till det i CRM-avsnittet, det är endast tillgängligt för bakåtkompatibilitet. Använd Microsoft Partner Center-lösningar i stället.

- **Granskning**: en skrivskyddad Gransknings logg för synkronisering med partner Center-hänvisningar

- **Microsoft Partner Center-lösningar**: ett anpassat objekt för att associera försäljnings färdiga lösningar eller Microsoft-lösningar med affärs möjligheten. Du kan lägga till och/eller ta bort en eller flera lösningar från affärs möjligheten. Det är obligatoriskt att lägga till minst en färdig Microsoft-lösning eller Microsoft-lösning för affärs möjligheten innan du delar den med Microsoft. Om du vill koppla det här objektet till en affärs möjlighet uppdaterar du affärs möjlighets formuläret i CRM:

  Välj lämplig flik i affärs möjlighets formuläret och Lägg till ett under rutnät enligt nedan:

  :::image type="content" source="images/cosellconnectors/dynamics-6.png" alt-text="Affärs möjlighets formulär":::

  :::image type="content" source="images/cosellconnectors/dynamics-7.png" alt-text="{alt-text}":::

- När du har lagt till Microsoft-lösningar kan du fylla i samförsäljnings klara lösnings information så att säljarna inte behöver lägga till dem. Om du vill lägga till en ny lösnings information går du till Microsoft Solution information-objekt i CRM och klickar på **Lägg till post** för att lägga till en post eller använda **Excel upload** för att lägga till flera poster.

  :::image type="content" source="images/dynamic-1a.png" alt-text="Lösnings information":::

### <a name="scenarios"></a>Scenarier:

1. Hänvisnings-synkronisering när hänvisning skapas eller uppdateras i CRM och synkroniseras i Partner Center:

   1. Logga in på din Dynamics 365 CRM-miljö med användare som har synlighet i avsnittet **affärs möjlighet** i CRM.

   2. Se till att avsnittet Microsoft Partner Center finns när du skapar en "ny affärs möjlighet" i Dynamics 365-miljön

   :::image type="content" source="images/dynamic-2a.png" alt-text="Ny affärs möjlighet"::: 

   3. För att synkronisera den här affärs möjligheten med partner Center, se till att du anger följande fält i kort vyn:

      - **Hur kan Microsoft hjälpa?**: om du vill skapa en samförsäljnings hänvisning väljer du ett lämpligt hjälp alternativ.

         :::image type="content" source="images/dynamic-3a.png" alt-text="Så här hämtar du lämpliga fält i kort vy":::

      - **Kund kontakt**: om du vill skapa en samförsäljnings referens lägger du till en kund kontakt i affärs möjligheten.

      - **Synkronisera med partner Center**: Ja

      - Microsoft-lösningar: om du vill dela en hänvisning med Microsoft lägger du till en giltig samförsäljnings-eller Microsoft-lösning för affärs möjligheten.
       
      
      :::image type="content" source="images/dynamic-4a.png" alt-text="Lösnings-ID":::

   4. När affärs möjligheten har skapats i Dynamics 365 med alternativet Synkronisera med partner Center inställt på Ja, vänta 10 minuter och logga sedan in på ditt partner Center-konto. Dina referenser kommer att synkroniseras med Dynamics 365 och hänvisnings-ID. Länken hänvisning kommer att fyllas i. Om ett fel uppstår fylls gransknings fältet i med fel information.
     
    5. För en affärs möjlighet som har alternativet "synkronisera med partner Center" inställt på "Ja", om du uppdaterar affärs möjligheten i Dynamics 365 CRM, kommer ändringarna att synkroniseras i ditt partner Center-konto.

    6. Möjligheter som har synkroniserats med partner Center identifieras med ✔-ikonen i Dynamics 365.

2. Hänvisnings-synkronisering när hänvisning skapas eller uppdateras i Microsoft Partner Center och synkroniseras i Dynamics 365-miljön:

   1. Logga in på [instrument panelen](https://partner.microsoft.com/dashboard/home)för partner Center.

   2. Välj **referenser** på menyn till vänster.

   3. Skapa en ny co-sälje-hänvisning från Partner Center genom att välja alternativet  **nytt erbjudande** .

   4. Logga in på din Dynamics 365 CRM-miljö.

   5. Navigera till **Öppna affärs möjligheter**. Den hänvisning som skapats i Microsoft Partner Center synkroniseras nu i Dynamics 365 CRM.

   6. När du väljer en synkroniserad referens fylls kort visnings informationen i.

## <a name="next-steps"></a>Nästa steg

- [Hantera leads](manage-leads.md)

- [Hantera möjligheter till samförsäljning](manage-co-sell-opportunities.md)

- [Mer om Microsoft Power Automated-plattform?](/power-automate/)

- [Partnercenter – webhooks](/partner-center/develop/partner-center-webhooks)
