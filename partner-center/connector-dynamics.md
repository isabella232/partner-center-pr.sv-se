---
title: Co-Sälj koppling för Dynamics 365 CRM-partner Center
ms.topic: how-to
ms.date: 05/27/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Synkronisera dina referenser i Partner Center med din co-sälje Connector för Dynamics 365 CRM. Säljare kan sedan sälja tillsammans med Microsoft från dina CRM-system.
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: c92938bbb4ffa6875419d06a9bbf23010ee60724
ms.sourcegitcommit: 7e32544cf91f932cbeb053c9de506ba9ee773fe2
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 11/20/2020
ms.locfileid: "94947826"
---
# <a name="co-sell-connector-for-dynamics-365-crm--overview"></a>Co-Sälj koppling för Dynamics 365 CRM – översikt

### <a name="appropriate-roles"></a>Lämpliga roller

- Referens administratör
- System administratör eller systemanpassare på CRM

Partner Center Co-sälje Connector gör det möjligt för dina säljare att sälja med Microsoft från dina CRM-system. De behöver inte tränas att använda Partner Center för att hantera samförsäljnings avtal. Använd Co-Sälj-anslutningarna för att skapa en ny samförsäljnings hänvisning för att engagera en Microsoft-säljare, ta emot hänvisningar från Microsoft-säljaren, acceptera/neka referenser, ändra avtals data som avtals värde och stängnings datum. Du kan också ta emot uppdateringar från Microsoft-säljarna om dessa samförsäljnings avtal. Du kan göra så att alla dina referenser fungerar i det valda CRM-nätverket i stället för i Partner Center. 

Lösningen baseras på Microsoft Power automatiserings lösning och använder API: er för partner Center.

## <a name="before-you-install---pre-requisites"></a>Innan du installerar-krav

|**Ämnen**   |**Detaljer**   |**Länkar**   |
|--------------|--------------------|------|
|Microsoft Partner Network-ID |Du behöver ett giltigt MPN-ID|För att ansluta till [MPN](https://partner.microsoft.com/)|
|Samförsäljnings klar|Din lösning för IP/tjänster måste vara samförsäljnings klar.|[Sälj med Microsoft](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|Partnercenter-konto|Det MPN-ID som är kopplat till Partner Center-klienten måste vara samma som det MPN-ID som är kopplat till din co-Sälj-lösning. Kontrol lera att du kan se dina samförsäljnings referenser på Partner Center-portalen innan du distribuerar anslutningarna.|[Hantera ditt konto](create-user-accounts-and-set-permissions.md)|
|Användar roller för partner Center|Den medarbetare som ska installera och använda anslutningarna måste vara en referens administratör|[Tilldela användarroller och -behörigheter](create-user-accounts-and-set-permissions.md)| |Dynamics 365 CRM|Användar rollen CRM är system administratör eller systemanpassare|[Tilldela roller i Dynamics 365](/dynamics365/customerengagement/on-premises/customize/privileges-required-customization)|
|Flödes konto för automatiserad energi|Ett aktivt [energi automatiserat](https://flow.microsoft.com) konto för CRM-systemadministratören eller systemanpassaren. Användaren ska logga in i [energi spar läge](https://flow.microsoft.com) minst en gång före installationen.|

## <a name="install-partner-center-referrals-synchronization-for-dynamics-365-power-automate-solution"></a>Installera synkronisering av Partner Center-referenser för Dynamics 365 (energi automatiserings lösning)

1. Gå till [Power automatisera](https://flow.microsoft.com) och välj **miljöer** i det högra övre hörnet. I det här steget visas tillgängliga CRM-instanser.

2. Välj lämplig CRM-instans i list rutan i det högra övre hörnet.

3. Välj **lösningar** i det vänstra navigerings fältet.

4. Klicka på länken **Öppna AppSource** på den översta menyn.

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="Öppna AppSource":::

5. Sök efter **partner Center-referenser till kopplingar för Dynamics365** på popup-skärmen.  

6. Klicka på knappen **Hämta nu** och **Fortsätt** sedan.

7. Då öppnas sidan där du kan välja CRM-miljön (Dynamics 365) för att installera programmet.  Godkänn de allmänna villkoren.

8. Sedan dirigeras du till sidan **Hantera dina lösningar** .  Gå till "Partner Center-referenser" genom att använda pilknapparna längst ned på sidan. **Installationen är schemalagd** bör visas bredvid lösningen för partner Center-hänvisningar. Installationen tar 10-15 minuter. 

9. När installationen är klar navigerar du tillbaka till [Automatisera](https://flow.microsoft.com) och väljer **lösningar** från det vänstra navigerings fältet. Observera att **synkroniseringen av Partner Center för Dynamics 365** är tillgänglig i lösnings listan.

10. Välj **synkronisering av Partner Center-referenser för Dynamics 365**. Följande energi flöden och entiteter är tillgängliga:

    :::image type="content" source="images/cosellconnectors/dynamics-available-crms.png" alt-text="Tillgängliga CRMS":::

## <a name="best-practice-test-before-you-go-live"></a>Bästa praxis: testa innan du går live

Innan du installerar, konfigurerar och anpassar den automatiserade energi lösningen i produktions miljön måste du testa lösningen på en mellanlagringsplatsen CRM-instans.

- Installera Microsoft Power automatiserings lösning på en mellanlagringsplatss miljö/CRM-instans.
- Gör en kopia av lösningen och kör din konfiguration och automatisera automatiserade flödes anpassningar i mellanlagrings miljön.
- Testa lösningen på en mellanlagrings-/CRM-instans. 
- Vid lyckad, importera som hanterad lösning till produktions instansen. 

## <a name="configure-the-solution"></a>Konfigurera lösningen

1. När du har installerat lösningen i din CRM-instans går du tillbaka till [Energis par](https://flow.microsoft.com/).


2. I list rutan **miljöer** i det högra hörnet väljer du den CRM-instans där du installerade den automatiserade energi lösningen.

3. Du måste skapa anslutningar som associerar de tre användar kontona:

   - Partner Center-användare med referenser för administratörs behörighet

   - Partnercenter-händelser

   - CRM-administratören med de energi automatiserade flödena i lösningen.

      1. Välj **anslutningar** i det vänstra navigerings fältet och välj lösningen "Partner Center-hänvisningar" i listan.

      2. Skapa en anslutning genom att klicka på **skapa en anslutning**.

         :::image type="content" source="images/cosellconnectors/dynamics1.png" alt-text="Skapa anslutning":::

      3. Sök efter **partner Center-referenser (för hands version)** i Sök fältet i det övre högra hörnet.

      4. Skapa en anslutning för din partner Center-användare med rollen autentiseringsuppgifter för referral admin.

      5. Skapa sedan en anslutning för partner Center-händelser för din partner Center-användare med autentiseringsuppgifterna för referral admin.

      6. Skapa en anslutning för Common Data Service (aktuell miljö) för CRM-administratörens användare.
       
     
      7. När du har lagt till alla anslutningar bör du se följande anslutningar i din miljö:

:::image type="content" source="images/cosellconnectors/dynamics2.png" alt-text="Anslutningar":::
   
## <a name="edit-the-connections"></a>Redigera anslutningarna

1. Gå tillbaka till sidan **lösningar** och välj **standard lösning**. Välj **anslutnings referens (för hands version)** genom att klicka på **alla**.

:::image type="content" source="images/cosellconnectors/dynamics3.png" alt-text="Anslut":::

2. Redigera varje anslutning en i taget genom att välja ikonen tre punkter. Lägg till relevanta anslutningar.

:::image type="content" source="images/cosellconnectors/dynamics4.png" alt-text="Anslutningar i listan"::: 

3.  Aktivera flödena i följande ordning:
- Partner Center – registrering av webhook (Insider Preview)
- Skapa samförsäljnings hänvisning – Dynamics 365 till Partner Center (Insider Preview)
- Partner Center Microsoft Co-Sälj hänvisnings uppdateringar till Dynamics 365 (Insider Preview)
- Partner Center till Dynamics 365 (Insider Preview)
- Dynamics 365 till Partner Center (Insider Preview)
- Dynamics 365-möjlighet till Partner Center (Insider Preview)
- Dynamics 365 Microsoft-lösningar till Partner Center (Insider Preview)
 

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a>Använda webhook-API: er för att registrera för resurs ändrings händelser

Med API: er för webhook i Partner Center kan du registrera för resurs ändrings händelser. De här ändrings händelserna skickas till din URL som HTTP-inlägg.

1. Registrera din URL genom att välja **partner Center webhook Registration (Insider Preview)** energi automatisera flöde.

2. Lägg till anslutningar för (a.) partner Center användare med referenser admin-autentiseringsuppgifter (b.) partner Center-händelser som marker ATS nedan

   :::image type="content" source="images/cosellconnectors/triggerflow.png" alt-text="Utlösare":::

3. När du gör dessa uppdateringar visas

   :::image type="content" source="images/cosellconnectors/webhook1.png" alt-text="Webhooks":::

4. Spara ändringarna och välj **Aktivera**.

   Gör så här om du vill aktivera att Webhooks i Partner Center ska lyssna på händelse ändringar:

5. Välj **partner Center till Dynamics 365 (Insider Preview)**.

6. Välj **redigerings** ikonen och välj **när en http-begäran tas emot**.

7. Välj **kopierings** ikonen för att kopiera den tillhandahållna HTTP post-URL: en.

   :::image type="content" source="images/cosellconnectors/copyurl.png" alt-text="Kopiera URL":::

8. Välj nu "partner för webhook-registrering (Insider Preview)" i Power Center och välj **Kör**.

9. Se till att fönstret kör flöde visas i den högra rutan och klicka på **Fortsätt**.

10. Ange följande uppgifter:

    1. **Http-utlösare slut punkt**: URL kopierad från föregående steg

    2. **Händelser att registrera**: "referral-created" och "referral-updated"

    3. **Skriv över befintliga utlösare slut punkter om det finns**: Ja (detta skriver över alla befintliga slut punkter.)

11. Välj **Kör** och välj sedan **Slutför.**

Webhooken kan nu lyssna på att skapa och uppdatera händelser.

## <a name="customize-synchronization-steps"></a>Anpassa synkroniserings steg

När samförsäljnings hänvisningar synkroniseras mellan partner Center och ditt CRM-system, visas fälten som synkroniseras på Partner Center-datorn här.

CRM-system är ofta anpassade. Du kan anpassa automatiserade energi flöden. Följ guiden för fält mappning och om det behövs kan du göra lämpliga ändringar i stegen i de automatiserade energi flödena.  Microsoft Partner Center till CRM-mappningar tillhandahålls, men baserat på din CRM-miljö kan du välja att ytterligare anpassa fälten.

Flera steg i vart och ett av de automatiserade energi flödena kan anpassas efter dina behov. Följande är exempel på tillgängliga anpassningar:

1. Så här anpassar du fälten för Create-eller Update-händelserna i Partner Center till CRM referral Synchronization: 

    a. Välj Partner Center till Dynamics 365 (Insider Preview) eller partner Center till Salesforce (Insider Preview).

    b. Välj **Redigera** för att redigera/anpassa det energi automatiserade flödet.

    c. Välj **(omfång) synkronisera lead eller affärs möjlighet**.

2. Om du vill anpassa fält mappningar för CRM (baserat på fält mappnings guide) för skapa händelser väljer du **om den är ny delad affärs möjlighet och sedan**. Välj under steget **om ja** och expandera sedan **skapa en ny affärs möjlighet i CRM**. Du kan redigera mappningarna i det här avsnittet med hjälp av fält mappnings guiden.

    d. För att anpassa fält mappningar för CRM (baserat på fält mappnings guide) för uppdaterings händelser, klicka på steget "(omfattning) synkronisera lead eller affärs möjlighet".

    e. Välj **om det är en uppdatering av en affärs möjlighet och sedan**. Välj under steget **om ja** och expandera sedan **differensen mellan affärs möjlighets objekt i Partner Center och CRM**.  

    f. Välj **om ja** följt av **Uppdatera befintlig affärs möjlighet**

3. Så här anpassar du fälten för CRM till PC referral-synkronisering för uppdaterings händelser:

    a. Välj **Redigera**  för att redigera/anpassa det energi automatiserade flödet.

    b. Välj **(omfång) synkronisera affärs möjligheten**.

    c. Om du vill anpassa fält mappningar för CRM för uppdaterings händelser väljer du **om det finns skillnader mellan lead-objekten i Partner Center och CRM**. 

    d. Välj under steget **om ja** och expandera sedan steget **Uppdatera en referens med affärs möjlighets data**.

   Du kan redigera mappningarna i det här avsnittet baserat på fält mappnings guiden.

4. Vill du anpassa fälten för synkronisering av CRM till PC-hänvisning för Create Events?

   a. Välj **Redigera**  för att redigera/anpassa det energi automatiserade flödet.

   b. Välj **(omfång)-synkronisering av referenser.**

   c. För att anpassa fält mappningar för CRM (baserat på fält mappnings guide) för skapa händelser väljer du **skapa Microsoft referral**.

   Du kan redigera mappningarna i det här avsnittet baserat på fält mappnings guiden.

Två miljövariabler har skapats:

- Bock: anger om du behöver en bock ikon förutom affärs möjligheter som synkroniseras i bi-riktning mellan partner Center och Dynamics 365 CRM.

- Synkronisera samförsäljnings möjligheter endast: anger om du bara vill synkronisera samförsäljnings möjligheter.

Du kan välja att redigera standardvärdet för miljövariablerna.

:::image type="content" source="images/cosellconnectors/dynamics5.png" alt-text="Redigerings ruta för standardvärden":::

## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a>Slutförd dubbelriktad referens synkronisering från slut punkt till slut punkt

När du har installerat, konfigurerat och anpassat den automatiserade lösningen för Energis par kan du testa synkroniseringen av samförsäljnings referenser mellan Dynamics 365 och partner Center.

### <a name="pre-requisites"></a>Förutsättningar

Om du vill synkronisera hänvisningarna mellan partner Center och Dynamics 365 CRM, kan du med hjälp av den automatiserade lösningen tydligt avgränsa Microsoft-/regionsspecifika hänvisnings fält. Den här identifieringen ger dina säljare möjlighet att bestämma vilka hänvisningar de vill dela med Microsoft för samförsäljning.

En uppsättning anpassade fält är tillgänglig som en del av entiteten **affärs möjlighet** . En administratörs användare i CRM måste skapa ett separat CRM-avsnitt med anpassade **affärs möjlighets** fält.

Följande anpassade fält ska ingå i CRM-avsnittet:

- **Synkronisera med partner Center**: om du vill synkronisera affärs möjligheten med Microsoft Partner Center

- **Hänvisnings-ID**: ett skrivskyddat ID-fält för Microsoft Partner Center-hänvisning

- **Hänvisnings länk**: en skrivskyddad länk till hänvisningen i Microsoft Partner Center

- **Hur kan Microsoft hjälpa?**: hjälp krävs från Microsoft för hänvisning

- **Produkter**: lista över produkter som är kopplade till den här affärs möjligheten

- **Granskning**: en skrivskyddad Gransknings logg för synkronisering med partner Center-hänvisningar

Uppdatera affärs möjlighets formuläret i Dynamics 365 CRM för att ta med lösningar för fältet produkter.

:::image type="content" source="images/cosellconnectors/dynamics6.png" alt-text="Affärs möjlighets formulär":::

:::image type="content" source="images/cosellconnectors/dynamics7.png" alt-text="{alt-text}":::

### <a name="scenarios"></a>OLIKA

1. Hänvisnings-synkronisering när hänvisning skapas eller uppdateras i CRM och synkroniseras i Partner Center:

   1. Logga in på din Dynamics 365 CRM-miljö med användare som har synlighet i avsnittet **affärs möjlighet** i CRM.

   2. Se till att följande avsnitt finns när du skapar en "ny affärs möjlighet" i Dynamics 365-miljön

      :::image type="content" source="images/cosellconnectors/opportunity.png" alt-text="Avsnittet exempel på möjlighet som visar information om Microsoft Partner Center i Dynamics 365.":::

   3. För att synkronisera den här affärs möjligheten med Microsoft Partner Center, se till att du anger följande fält i kort vyn:

      - **Synkronisera med partner Center**: Ja

      - **Hur kan Microsoft hjälpa?**: Välj bland följande:

         :::image type="content" source="images/cosellconnectors/help.png" alt-text="Avsnittet exempel på en affärs möjlighet i Dynamics 365 som visar hjälp alternativ för Microsoft Partner Center bredvid ett fält som kallas hur kan Microsoft hjälpa dig?":::

      - **Produkter**: lösnings-ID för produkten

   4. När affärs möjligheten har skapats i Dynamics 365 med alternativet **Synkronisera med partner Center** inställt på **Ja**, vänta 10 minuter och logga sedan in på ditt partner Center-konto. Dina referenser kommer att synkroniseras med Dynamics 365.

   5. För en affärs möjlighet som har alternativet "synkronisera med partner Center" inställt på "Ja", om du uppdaterar affärs möjligheten i Dynamics 365 CRM, kommer ändringarna att synkroniseras i ditt partner Center-konto.

   6. Möjligheter som har synkroniserats med partner Center identifieras med ✔-ikonen i Dynamics 365.

2. Hänvisnings-synkronisering när hänvisning skapas eller uppdateras i Microsoft Partner Center och synkroniseras i Dynamics 365-miljön:

   1. Logga in på [instrument panelen](https://partner.microsoft.com/dashboard/home)för partner Center.

   2. Välj **referenser** på menyn till vänster.

   3. Skapa en ny samförsäljnings hänvisning från Partner Center genom att klicka på alternativet "nytt erbjudande".

   4. Logga in på din Dynamics 365 CRM-miljö.

   5. Navigera till **Öppna affärs möjligheter**. Den hänvisning som skapats i Microsoft Partner Center synkroniseras nu i Dynamics 365 CRM.

   6. När du väljer en synkroniserad referens fylls kort visnings informationen i.

## <a name="next-steps"></a>Nästa steg

- [Hantera leads](manage-leads.md)

- [Hantera möjligheter till samförsäljning](manage-co-sell-opportunities.md)

- [Mer om Microsoft Power Automated-plattform?](/power-automate/)

- [Webhooks för partner Center](/partner-center/develop/partner-center-webhooks)