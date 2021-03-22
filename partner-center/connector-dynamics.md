---
title: Co-Sälj koppling för Dynamics 365 CRM-partner Center
description: Synkronisera referenser i Partner Center med ditt Co-sälje Connector för Dynamics 365 CRM. Du kan sedan samsälja med Microsoft från ditt CRM-system.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.date: 03/01/2021
ms.openlocfilehash: 2082424f8203f0d9c50726e1e5ef7b3e3c39d6c2
ms.sourcegitcommit: 35fe0fdc41886f6f5af71ec74e4a4ebd245dfe1d
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/22/2021
ms.locfileid: "104768779"
---
# <a name="co-sell-connector-for-dynamics-365-crm-overview"></a>Översikt över Co-Sälj koppling för Dynamics 365 CRM

### <a name="appropriate-roles"></a>Lämpliga roller

- Referens administratör
- System administratör eller systemanpassare på CRM

Partner Center Co-Sälj anslutningar gör det möjligt för dina säljare att sälja med Microsoft från dina CRM-system. De behöver inte tränas att använda Partner Center för att hantera samförsäljnings avtal. Använd Co-sälja-kopplingarna för att skapa en ny samförsäljnings hänvisning för att engagera en Microsoft-säljare, ta emot hänvisningar från Microsoft-säljaren, acceptera eller neka referenser och ändra avtals data, till exempel avtals värde och stängnings datum. Du kan också ta emot uppdateringar från Microsoft-säljarna om dessa samförsäljnings avtal. Du kan hantera alla dina referenser på önskat alternativ i CRM och inte i Partner Center.

Lösningen baseras på energi automatisering och använder API: er för partner Center.

## <a name="prerequisites"></a>Förutsättningar

Se till att uppfylla följande krav innan du installerar lösningen.

|**Ämnen**   |**Information**   |**Länkar**   |
|--------------|--------------------|------|
|Microsoft Partner Network (MPN) ID |Du behöver ett giltigt MPN-ID.|[Anslut till partner nätverket](https://partner.microsoft.com/)|
|Färdiga försäljnings produkter|Din lösning för IP/tjänster måste vara samförsäljnings klar.|[Sälj med Microsoft](https://partner.microsoft.com/membership/sell-with-microsoft)|
|Partnercenter-konto|Det MPN-ID som är kopplat till Partner Center-klienten måste vara samma som det MPN-ID som är kopplat till din co-Sälj-lösning. Kontrol lera att du kan se dina samförsäljnings referenser i Partner Center-portalen innan du distribuerar anslutningarna.|[Hantera ditt konto](create-user-accounts-and-set-permissions.md)|
|Användar roller för partner Center|Den medarbetare som ska installera och använda anslutningarna måste vara en referens administratör.|[Tilldela användarroller och -behörigheter](create-user-accounts-and-set-permissions.md)|
|Dynamics 365 CRM|Användar rollen CRM är system administratör eller systemanpassare.|[Tilldela roller i Dynamics 365](/dynamics365/customerengagement/on-premises/customize/privileges-required-customization)|
|Flödes konto för automatiserad energi|Skapa en ny produktions miljö med en databas för testning, mellanlagring och produktion. Om du har en befintlig produktions miljö med en databas kan den återanvändas. Den användare som ska installera anslutnings lösningen måste ha en energi automatiserings licens och åtkomst till den här miljön. Du kan övervaka förloppet och få mer information i [energi spar](https://flow.microsoft.com/) läge om installationen Miss lyckas. Välj **Se historik** under **lösningar**.|[Skapa eller hantera miljö](/power-platform/admin/create-environment#create-an-environment-with-a-database)|

## <a name="install-partner-center-referrals-synchronization-for-dynamics-365-power-automate-solution"></a>Installera synkronisering av Partner Center-referenser för Dynamics 365 (energi automatiserings lösning)

1. Gå till [energi automatisering](https://flow.microsoft.com)och välj **miljöer** i det övre högra hörnet. I det här steget visas tillgängliga CRM-instanser.

1. Välj lämplig CRM-instans i list rutan i det övre högra hörnet.

1. Välj **lösningar** till vänster.

1. Välj länken **Öppna AppSource** på den översta menyn.

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="Skärm bild som visar Open AppSource.":::

1. Sök efter **partner Center-referenser till kopplingar för Dynamics 365** på popup-skärmen.  

1. Välj knappen **Hämta nu** och välj sedan **Fortsätt**.

1. En sida visas där du kan välja en CRM-miljö (Dynamics 365) för att installera programmet. Godkänn de allmänna villkoren.

1. Du kan övervaka förloppet och om installationen Miss lyckas kan du få mer information i automatiserat läge genom att välja **Se historik** under **lösningar**.

1. När installationen är klar går du tillbaka till [Energis par](https://flow.microsoft.com) och väljer **lösningar** till vänster. **Synkronisering av Partner Center för Dynamics 365** är nu tillgängligt i **lösnings** listan.

1. Välj **synkronisering av Partner Center-referenser för Dynamics 365**. Följande energi flöden och entiteter är tillgängliga.

    :::image type="content" source="images/cosellconnectors/dynamics-available-crms.png" alt-text="Skärm bild som visar tillgängliga CRMs.":::

## <a name="test-before-you-go-live"></a>Testa innan du går live

Innan du installerar, konfigurerar och anpassar den automatiserade energi lösningen i produktions miljön måste du testa lösningen på en mellanlagringsplatsen CRM-instans. Du måste:

- Installera den automatiserade automatiserade lösningen på en instans av en utvecklings miljö för CRM.
- Konfigurera och anpassa den automatiserade lösningen för Energis par i en mellanlagrings miljö.
- Testa lösningen på en mellanlagringsplats av CRM-instansen.
- När testet är klart kan du importera som en hanterad lösning till produktions instansen.

## <a name="configure-the-solution"></a>Konfigurera lösningen

1. När du har installerat lösningen i din CRM-instans går du tillbaka till automatisk [energi](https://flow.microsoft.com/).

1. I list rutan **miljöer** i det övre högra hörnet väljer du den CRM-instans där du installerade den automatiserade energi lösningen.

1. Du måste skapa anslutningar som associerar de tre användar kontona:

   - Partner Center-användare med referenser för administratörs behörighet
   - Partnercenter-händelser
   - CRM-administratör med de energi automatiserade flödena i lösningen

   1. Välj **anslutningar** till vänster och välj lösningen **partner Center referral** i listan.

   1. Skapa en anslutning genom att välja **skapa en anslutning**.

         :::image type="content" source="images/cosellconnectors/dynamics-1.png" alt-text="Skärm bild som visar skapa en anslutning.":::

   1. Sök efter **partner Center-referenser (för hands version)** i Sök fältet i det övre högra hörnet.

   1. Skapa en anslutning för din partner Center-användare med rollen autentiseringsuppgifter för referral admin.

   1. Skapa sedan en anslutning för partner Center-händelser för din partner Center-användare med referenserna admin-autentiseringsuppgifter.

   1. Skapa en anslutning för Common Data Service (aktuell miljö) för CRM-administratörens användare.
     
   1. När du har lagt till alla anslutningar bör du se följande anslutningar i din miljö.

      :::image type="content" source="images/cosellconnectors/dynamics-2.png" alt-text="Skärm bild som visar anslutningar.":::

## <a name="edit-the-connections"></a>Redigera anslutningarna

1. Gå tillbaka till sidan **lösningar** och välj **standard lösning**. Välj **anslutnings referens (för hands version)** genom att markera **alla**.

   :::image type="content" source="images/connection-reference-video.gif" alt-text="Skärm bild som visar redigering av anslutningar.":::

1. Redigera varje anslutning en i taget genom att välja ikonen med tre punkter. Lägg till relevanta anslutningar.

   :::image type="content" source="images/cosellconnectors/dynamics-4.png" alt-text="Skärm bild som visar anslutningar i listan.":::

1.  Gå tillbaka till sidan **lösningar** , Välj **partner Center-synkronisering för Dynamics 365** och aktivera flödet genom att välja ikonen med tre punkter bredvid varje flöde i följande ordning. Om du stöter på problem när du aktiverar flödet, se [anpassnings steg](connector-dynamics.md#customize-synchronization-steps) och [fel söknings steg](connectors-troubleshoot.md).

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

Du kan använda API: er för webhook för partner Center för att registrera dig för resurs ändrings händelser. De här ändrings händelserna skickas till din URL som HTTP-inlägg.

1. Välj **partner Center till Dynamics 365 (Insider Preview)**.

1. Välj **redigerings** ikonen och välj **när en http-begäran tas emot**.

1. Välj **kopierings** ikonen för att kopiera den tillhandahållna HTTP post-URL: en.

   :::image type="content" source="images/webhook-video.gif" alt-text="Skärm bild som visar hur du använder Webhooks för att registrera resurs ändringar.":::

1. Välj **partner Center-webhook-registrering (Insider Preview)** automatisera flödet och välj sedan **Kör**.

1. Se till att **Kör flödes** fönstret öppnas i den högra rutan och välj **Fortsätt**.

1. Ange följande information:

   - **Http-utlösare slut punkt**: den här URL: en kopierades från ett tidigare steg.
   - **Händelser att registrera**: Välj alla tillgängliga händelser (**hänvisning – skapad**, **hänvisning-uppdaterad**, **relaterad-referens-skapad** och **relaterad-referral-uppdaterad**).
   - Vill du **skriva över befintliga trigger-slutpunkter om det finns?**: Ja. Det går bara att registrera en URL för en viss webhook-händelse.

1. Välj **Kör flöde** och välj sedan **färdig.**

Webhooken kan nu lyssna på, skapa och uppdatera händelser.

## <a name="customize-synchronization-steps"></a>Anpassa synkroniserings steg

CRM-systemen är mycket anpassade och du kan anpassa den automatiserade lösningen baserat på din CRM-installation. När samförsäljnings hänvisningar synkroniseras mellan partner Center och ditt CRM-system, visas fälten som synkroniseras på Partner Center-datorn i den [anpassade fält mappnings guiden](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWxL6S).

Följ guiden för fält mappning och om det behövs kan du göra lämpliga ändringar i **[anpassa] skapa eller hämta information från Dynamics 365 Flow** -eller miljövariabler. Uppdatera inte andra flöden i den automatiserade energi lösningen eftersom det kan påverka framtida lösnings uppgraderingar.

Följande anpassningar är tillgängliga:

- **Visa markering i affärs möjlighets namnet**: som standard visas en bock bredvid namnet på affärs möjligheten för att ange att synkroniseringen mellan partner Center och Dynamics 365 CRM sker. På samma sätt visas en kryss markering om det inte går att synkronisera. För att undvika att lägga till en kryss markering eller ett kryss markering i affärs möjlighets namnet anger du det aktuella värdet för **Visa markering i miljövariabeln affärs möjlighets namn** till Nej.
- **Avtals värde**: som standard synkroniseras det avtalade värdet från Partner Center till och från **estimatedvalue** i CRM. Om du har ett annat fält i CRM för att det avtalade värdet ska synkroniseras från:

  - Uppdatera fält namnet för **avtals värde** i Dynamics 365-miljövariabeln med CRM: s fält namn. Se till att du anger fältets namn, inte dess visnings namn.
  - Redigera **[anpassa] skapa eller hämta information från Dynamics 365-flödet** och gå till **skapa eller uppdatera affärs möjlighet** i CRM och uppdatera **skapa en ny affärs möjlighet** och **Uppdatera befintliga affärs möjlighets** åtgärder för att tilldela **DealValue** -värdet till rätt fält i CRM. Ta också bort **DealValue** -tilldelningen från fältet **Beräknad intäkt** .

- **Landskod för kund konto**: det är obligatoriskt att ange en landskod på två bokstäver (ISO 3166) när du skapar en ny hänvisning. Som standard kommer lands koden att synkroniseras till och från kontots **address1_country** fält i CRM. Om du har ett annat fält i CRM för lands koden som ska synkroniseras från:

   - För ett fält för lands koder som inte är uppslag i kontot som innehåller en kod med två bokstäver:
     - Uppdatera namnet på fältet **kund konto lands kod** i Dynamics 365-miljövariabeln med CRM: s fält namn. Se till att du anger fältets namn, inte dess visnings namn.
     - Redigera **[anpassa] skapa eller hämta information från Dynamics 365-flödet** och gå till **skapa eller hämta kund konto** i CRM-åtgärden för att tilldela ett **lands** värde till rätt fält i CRM. Ta också bort värdet för **lands** tilldelning från fältet **adress 1: land/region** .

   - För ett söknings-baserat lands kod fält i kontot:
     - Lägg till ett nytt anpassat fält i kontot och fyll i det automatiskt med en landskod på två bokstäver (ISO 3166) baserat på värdet som valts i det sökbaserade fältet och vice versa.
     - Följ föregående steg för fältet kod för land som inte är uppslag för att synkronisera ett nytt anpassat fält från CRM till och från Partner Center.

- **Affärs möjlighets fält**: om det finns obligatoriska fält i **affärs möjlighet** som måste fyllas i, redigerar du **[anpassa] skapa eller hämta information från Dynamics 365-flödet** och går till **skapa eller uppdatera affärs möjlighet** i CRM och uppdatera **skapa en ny affärs möjlighets åtgärd** för att tilldela värden till de obligatoriska fälten utifrån dina affärs behov.
- **Lead-fält**: om det finns obligatoriska fält i **lead** som måste fyllas i, redigera **[anpassa] skapa eller hämta information från Dynamics 365-flödet** och gå till **skapa eller uppdatera lead** i CRM och uppdatera **skapa en ny lead-åtgärd** för att tilldela värden till de obligatoriska fälten utifrån dina affärs behov.
- **Kund konto**: när en ny hänvisning synkroniseras från Partner Center till CRM försöker den automatiserade lösningen att söka efter ett befintligt konto i CRM genom att använda kundens företags namn och post nummer. Om den inte hittar något skapas ett nytt kund konto i CRM. Om du vill uppdatera Sök villkoren och information om hur du skapar ett nytt konto, redigera **[anpassa] skapa eller hämta information från Dynamics 365-flödet** och gå till **skapa eller hämta kund konto** i CRM och **Skapa kund konto åtgärd**.

## <a name="update-environment-variable"></a>Uppdatera miljö variabel

Så här uppdaterar du ett miljö variabel värde:

1. Gå till sidan **lösningar** och välj **standard lösning**. Välj **miljö variabel** genom att markera **alla**.

1. Välj miljövariabeln för det värde som behöver uppdateras och välj **Redigera** med hjälp av ikonen med tre punkter.

1. Uppdatera **aktuellt värde** (uppdatera inte **standardvärdet**) genom att använda alternativet **nytt värde** och ange värdet. Värdet måste överensstämma med data typen för variabeln. Till exempel accepterar data typen Ja eller nej antingen värdet Ja eller nej.

   :::image type="content" source="images/environment-variables-video.gif" alt-text="Skärm bild som visar uppdatering av miljövariabler.":::

## <a name="end-to-end-bidirectional-co-sell-referral-synchronization"></a>Slutpunkt-till-slutpunkt-dubbelriktad referens för samförsäljning

När du har installerat, konfigurerat och anpassat den automatiserade lösningen för Energis par kan du testa synkroniseringen av samförsäljnings referenser mellan Dynamics 365 och partner Center.

### <a name="prerequisites"></a>Förutsättningar

Om du vill synkronisera hänvisningarna mellan partner Center och Dynamics 365 CRM, kan du med hjälp av den automatiserade lösningen tydligt avgränsa Microsoft-/regionsspecifika hänvisnings fält. Den här identifieringen ger dina säljare möjlighet att bestämma vilka hänvisningar de vill dela med Microsoft för samförsäljning.

En uppsättning anpassade fält och objekt kommer att läggas till som en del av lösnings installationen. En administratörs användare i CRM måste skapa ett separat CRM-avsnitt med anpassade **affärs möjlighets** fält.

Följande anpassade fält ska ingå i CRM-avsnittet:

- **Synkronisera med partner Center**: om du vill synkronisera affärs möjligheten med partner Center. Som standard är värdet för det här fältet Nej och måste uttryckligen anges till Ja av din säljare för att dela en affärs möjlighet med Microsoft. Nya hänvisningar som delas från Partner Center till CRM har detta fält värde inställt på Ja.
- **Hänvisnings-ID**: ett skrivskyddat ID-fält för partner Center-referensen.
- **Hänvisnings länk**: en skrivskyddad länk till hänvisningen i Partner Center.
- **Hur kan Microsoft hjälpa?**: hjälp krävs från Microsoft för hänvisning. Om du vill skapa en samförsäljnings hänvisning väljer du lämplig hjälp från Microsoft. En kund kontakt måste vara kopplad till möjligheten att skapa en samförsäljnings hänvisning. Välj inte det här fältet om du vill skapa en icke-samförsäljnings hänvisning. En icke-samförsäljnings hänvisning kan konverteras till en samförsäljnings hänvisning när som helst genom att välja lämplig hjälp – obligatoriskt alternativ.
- **Microsoft Partner Center hänvisnings synlighet**: Välj synlighet för partner Center-referensen. Genom att göra det synligt för Microsofts säljare kan en icke-samförsäljnings hänvisning konverteras till medförsäljning. När Microsoft-hjälpen krävs är hänvisningen synlig för Microsofts säljare som standard. När det här fältet är markerat som synligt går det inte att återställa.
- **Microsoft CRM-identifierare**: när en samförsäljnings hänvisning skapas och godkänns av Microsoft kommer det här fältet att fyllas i med Microsoft CRM-identifieraren.
- **Produkter: föråldrade**: Använd inte det här fältet eller Lägg till det i CRM-avsnittet. Den är endast tillgänglig för bakåtkompatibilitet. Använd partner Center-lösningar i stället.
- **Granskning**: en skrivskyddad Gransknings logg för synkronisering med partner Center-hänvisningar.
- **Microsoft Partner Center-lösningar**: ett anpassat objekt för att associera försäljnings färdiga lösningar eller Microsoft-lösningar med affärs möjligheten. Det går att lägga till eller ta bort en eller flera lösningar från affärs möjligheten. Det är obligatoriskt att lägga till minst en samförsäljnings-eller Microsoft-lösning som är färdig till affärs möjligheten innan du delar den med Microsoft. Om du vill associera objektet med affärs möjligheten uppdaterar du **affärs möjlighets** formuläret i CRM.

  Välj lämplig flik i **affärs möjlighets** formuläret och Lägg till ett under rutnät som visas här.

  :::image type="content" source="images/cosellconnectors/dynamics-6.png" alt-text="Skärm bild som visar affärs möjlighets formuläret.":::

  :::image type="content" source="images/cosellconnectors/dynamics-7.png" alt-text="Skärm bild som visar Microsoft-lösningar.":::

- När du har lagt till Microsoft-lösningar kan du fylla i samförsäljnings färdiga lösnings information så att säljarna inte behöver lägga till dem. Om du vill lägga till en ny lösnings information går du till Microsoft Solution information-objektet i CRM och väljer **Lägg till post** för att lägga till en post eller använda **Excel upload** för att lägga till flera poster.

  :::image type="content" source="images/dynamic-1a.png" alt-text="Skärm bild som visar ny Microsoft-lösnings information.":::

### <a name="scenarios"></a>Scenarier

1. Hänvisnings-synkronisering när hänvisning skapas eller uppdateras i CRM och synkroniseras i Partner Center:

   1. Logga in på din Dynamics 365 CRM-miljö med användaren som har synlighet i avsnittet **affärs möjlighet** i CRM.

   1. Se till att avsnittet **Microsoft Partner Center** finns när du skapar en ny affärs möjlighet i Dynamics 365-miljön.

      :::image type="content" source="images/dynamic-2a.png" alt-text="Skärm bild som visar ny affärs möjlighet.":::

   1. För att synkronisera den här affärs möjligheten med partner Center, se till att du anger följande fält i kort vyn:

      - **Hur kan Microsoft hjälpa?**: om du vill skapa en samförsäljnings referens väljer du ett lämpligt hjälp alternativ.

         :::image type="content" source="images/dynamic-3a.png" alt-text="Skärm bild som visar hur du hämtar lämpliga fält i kort visning.":::

      - **Kund kontakt**: om du vill skapa en samförsäljnings referens lägger du till en kund kontakt i affärs möjligheten.
      - **Synkronisera med partner Center**: Ja.
      - **Microsoft-lösningar**: om du vill dela en hänvisning med Microsoft lägger du till en giltig försäljnings-eller Microsoft-lösning i Co-försäljningen för affärs möjligheten.
      
        :::image type="content" source="images/dynamic-4a.png" alt-text="Skärm bild som visar lösnings-ID.":::

   1. När affärs möjligheten har skapats i Dynamics 365 med alternativet **Synkronisera med partner Center** inställt på Ja, vänta 10 minuter. Logga sedan in på ditt partner Center-konto. Dina referenser kommer att synkroniseras med Dynamics 365 och **hänvisnings-ID**. **Länken hänvisning** kommer att fyllas i. Om det uppstår ett fel så fylls **gransknings** fältet med fel information.
     
    1. På samma sätt kommer ändringarna att synkroniseras i ditt partner Center-konto för en affärs möjlighet som hade alternativet **Synkronisera med partner Center** inställt på Ja, om du uppdaterar affärs möjligheten i Dynamics 365 CRM.

    1. Möjligheter som har synkroniserats med partner Center identifieras med ✔-ikonen i Dynamics 365.

1. Hänvisnings-synkronisering när hänvisningen skapas eller uppdateras i Partner Center och synkroniseras i Dynamics 365-miljön:

   1. Logga in på [instrument panelen](https://partner.microsoft.com/dashboard/home)för partner Center.

   1. Välj **referenser** på den vänstra menyn.

   1. Skapa en ny co-sälje-hänvisning från Partner Center genom att välja alternativet **nytt erbjudande** .

   1. Logga in på din Dynamics 365 CRM-miljö.

   1. Gå till **Öppna affärs möjligheter**. Den hänvisning som skapats i Partner Center synkroniseras nu i Dynamics 365 CRM.

   1. När du väljer en synkroniserad referens fylls kort visnings informationen i.

## <a name="next-steps"></a>Nästa steg

- [Hantera leads](manage-leads.md)
- [Hantera möjligheter till samförsäljning](manage-co-sell-opportunities.md)
- [Mer om Microsoft Power automatiserings plattform](/power-automate/)
- [Partnercenter – webhooks](/partner-center/develop/partner-center-webhooks)
