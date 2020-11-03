---
title: Co-Sälj koppling för Salesforce CRM-partner Center
ms.topic: how-to
ms.date: 09/29/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Synkronisera dina referenser i Partner Center med Salesforce CRM. Säljare kan sedan sälja tillsammans med Microsoft från dina CRM-system.
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: 4b3817dafbd05edf0c50b062b52ac4814c767d04
ms.sourcegitcommit: a8adb5f044f06bd684a5b7a06c8efe9f8b03d2db
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 10/14/2020
ms.locfileid: "92531893"
---
# <a name="co-sell-connector-for-salesforce-crm---overview"></a>Co-Sälj koppling för Salesforce CRM – översikt

### <a name="appropriate-roles"></a>Lämpliga roller

- Referens administratör
- System administratör eller systemanpassare på CRM

Partner Center Co-sälje Connector gör det möjligt för dina säljare att sälja med Microsoft från dina CRM-system. De behöver inte tränas att använda Partner Center för att hantera samförsäljnings avtal. Med hjälp av samförsäljnings kopplingarna kan du skapa en ny samförsäljnings hänvisning för att engagera en Microsoft-säljare, ta emot hänvisningar från Microsoft-säljaren, acceptera/neka referenser, ändra avtals data som avtals värde och stängnings datum.  Du kan också ta emot uppdateringar från Microsoft-säljarna om dessa samförsäljnings avtal. Du kan göra så att alla dina referenser fungerar när du arbetar i valfri CRM i stället för i Partner Center. 

Lösningen baseras på Microsoft Power automatiserings lösning och använder API: er för partner Center.

## <a name="before-you-install---pre-requisites"></a>Innan du installerar-krav

|**Ämnen**   |**Detaljer**   |**Länkar**   |
|--------------|--------------------|------|
|Microsoft Partner Network-ID |Du behöver ett giltigt MPN-ID|För att ansluta till [MPN](https://partner.microsoft.com/)|
|Färdiga försäljnings produkter|Din lösning för IP/tjänster måste vara samförsäljnings klar.|[Sälj med Microsoft](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|Partnercenter-konto|Det MPN-ID som är kopplat till Partner Center-klienten måste vara samma som det MPN-ID som är kopplat till din co-Sälj-lösning. Kontrol lera att du kan se dina samförsäljnings referenser på Partner Center-portalen innan du distribuerar anslutningarna.|[Hantera ditt konto](create-user-accounts-and-set-permissions.md)|
|Användar roller för partner Center|Den medarbetare som ska installera och använda anslutningarna måste vara en referens administratör|[Tilldela användarroller och -behörigheter](create-user-accounts-and-set-permissions.md)|
|Salesforce CRM|Användar rollen CRM är system administratör eller systemanpassare|[Tilldela roller i Salesforce CRM](https://help.salesforce.com/articleView?id=assigning_users_to_roles.htm&type=5)|
|Flödes konto för automatiserad energi|Ett aktivt [energi automatiserat](https://flow.microsoft.com) konto för CRM-systemadministratören eller systemanpassaren. Användaren ska logga in i [energi spar läge](https://flow.microsoft.com) minst en gång före installationen.|

## <a name="installation-of-salesforce-package-for-microsoft-custom-fields"></a>Installation av Salesforce-paket för anpassade Microsoft-fält 

Om du vill synkronisera hänvisningarna över partner Center och Salesforce CRM måste den automatiserade lösningen för att tydligt identifiera Microsoft-speciella hänvisnings fält. Denna avgränsning ger partner säljares team möjlighet att bestämma vilka hänvisningar de vill dela med Microsoft för samförsäljning.

1. I Salesforce aktiverar du **anteckningar** och lägger till det i listan relaterade affärs möjligheter. 
[Referens](https://help.salesforce.com/articleView?err=1&id=notes_admin_setup.htm&type=5)

2. Aktivera **affärs möjlighets team** genom att följa stegen: 
    - I installations programmet använder du rutan **snabb sökning** för att hitta team inställningar för affärs möjligheter.
    - Definiera inställningarna efter behov.
[Referens](https://help.salesforce.com/articleView?id=teamselling_enabling.htm&type=5]) 

3. I Salesforce installerar du anpassade fält och objekt med hjälp av Package Installer nedan.
  
Gå [hit](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t2w000006Vs9a) om du vill installera paketet i valfritt företag:


Obs! Om du installerar i ett begränsat läge måste du ersätta den inledande delen av URL: en med http://test.salesforce.com

4. I Salesforce lägger du till Microsoft-lösningar i listan relaterad **affärs möjlighet** . När du har lagt till klickar du på **SKIFT nyckel** ikonen och uppdaterar egenskaperna

## <a name="best-practice-test-before-you-go-live"></a>Bästa praxis: testa innan du går live

Innan du installerar, konfigurerar och anpassar den automatiserade energi lösningen i produktions miljön måste du testa lösningen på en mellanlagringsplatsen CRM-instans.

- Installera Microsoft Power automatiserings lösning på en mellanlagringsplatss miljö/CRM-instans.

- Gör en kopia av lösningen och kör din konfiguration och automatisera automatiserade flödes anpassningar i mellanlagrings miljön.

- Testa lösningen på en mellanlagrings-/CRM-instans.

- Vid lyckad import importerar du som en hanterad lösning till produktions instansen.

## <a name="install-partner-center-referrals-synchronization-for-salesforce-crm"></a>Installera synkronisering av Partner Center-referenser för Salesforce CRM

1. Gå till [Power automatisera](https://flow.microsoft.com) och välj **miljöer** i det högra övre hörnet. Då visas tillgängliga CRM-instanser.

2. Välj lämplig CRM-instans i list rutan i det högra övre hörnet.

3. Välj **lösningar** i det vänstra navigerings fältet.

4. Klicka på länken **Öppna AppSource** på den översta menyn.

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="Öppna AppSource":::

5. Sök efter **partner Center-referenser för Salesforce** i popup-fönstret.  

   :::image type="content" source="images/salesforce/salesforce1.png" alt-text="Öppna AppSource":::

6. Klicka på knappen **Hämta nu** och **Fortsätt** sedan.

7. Då öppnas sidan där du kan välja Salesforce CRM-miljön för att installera programmet.  Godkänn de allmänna villkoren.

   :::image type="content" source="images/salesforce/available-crm.png" alt-text="Öppna AppSource" genom att använda pilknapparna längst ned på sidan. **Installationen är schemalagd** bör visas bredvid lösningen för partner Center-hänvisningar. Installationen tar 10-15 minuter.

9. När installationen är klar navigerar du tillbaka till [Automatisera](https://flow.microsoft.com) och väljer **lösningar** från det vänstra navigerings fältet. Observera att **synkronisering av Partner Center för Salesforce** är tillgängligt i lösnings listan.

10. Välj **synkronisering av Partner Center-referenser för Salesforce** . Följande energi flöden och entiteter är tillgängliga:

    :::image type="content" source="images/cosellconnectors/salesforce10.png" alt-text="Öppna AppSource":::



## <a name="configure-the-solution"></a>Konfigurera lösningen

1. När du har installerat lösningen i din CRM-instans går du tillbaka till [Energis par](https://flow.microsoft.com/).

2. I list rutan **miljöer** i det högra hörnet väljer du den CRM-instans där du installerade den automatiserade energi lösningen.
3. Du måste skapa anslutningar som associerar de tre användar kontona:
    - Partner Center-användare med referenser för administratörs behörighet
    - Partnercenter-händelser
    - CRM-administratören med de energi automatiserade flödena i lösningen.
4. Välj **anslutningar** i det vänstra navigerings fältet och välj lösningen "Partner Center-hänvisningar" i listan.

5. Skapa en anslutning genom att klicka på **skapa en anslutning** .

:::image type="content" source="images/cosellconnectors/salesforce12.png" alt-text="Öppna AppSource":::

- Sök efter partner Center-referenser (för hands version) i Sök fältet i det övre högra hörnet.

- Skapa en anslutning för din partner Center-användare med rollen autentiseringsuppgifter för referral admin.

-  Skapa sedan en anslutning för partner Center-händelser för din partner Center-användare med autentiseringsuppgifterna för referral admin.

- Skapa en anslutning för Common Data Service (aktuell miljö) för CRM-administratörens användare.

-  När du har lagt till alla anslutningar bör du se följande anslutningar i din miljö:

 :::image type="content" source="images/cosellconnectors/salesforce13.png" alt-text="Öppna AppSource":::

### <a name="edit-the-connections"></a>Redigera anslutningarna

1. Gå tillbaka till sidan lösningar och välj **standard lösning** .  Välj **anslutnings referens (för hands version)** genom att klicka på **alla** .
 
:::image type="content" source="images/cosellconnectors/salesforce14.png" alt-text="Öppna AppSource":::

2. Redigera varje anslutning en i taget genom att välja ikonen tre punkter. Lägg till relevanta anslutningar.

:::image type="content" source="images/cosellconnectors/salesforce15.png" alt-text="Öppna AppSource":::

3. Aktivera flödena i följande ordning:

- Partner Center – registrering av webhook (Insider Preview)
- Skapa Co-sälje referral-Salesforce till Partner Center (Insider Preview)
- Partner Center Microsoft Co-Sälj hänvisnings uppdateringar till Salesforce (Insider Preview)
- Partner Center till Salesforce (Insider Preview)
- Salesforce till Partner Center (Insider Preview)
- Salesforce-möjlighet till Partner Center (Insider Preview)
- Salesforce Microsoft-lösningar till Partner Center (Insider Preview)

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a>Använda webhook-API: er för att registrera för resurs ändrings händelser

Med API: er för webhook i Partner Center kan du registrera för resurs ändrings händelser. De här ändrings händelserna skickas till din URL som HTTP-inlägg.

1. Registrera din URL genom att välja **partner Center webhook Registration (Insider Preview)** energi automatisera flöde.

2. Lägg till anslutningar för (a.) partner Center användare med referenser admin-autentiseringsuppgifter (b.) partner Center-händelser som marker ATS nedan

   :::image type="content" source="images/cosellconnectors/triggerflow.png" alt-text="Öppna AppSource":::

3. När du gör dessa uppdateringar visas

   :::image type="content" source="images/cosellconnectors/webhook1.png" alt-text="Öppna AppSource":::

4. Spara ändringarna och välj **Aktivera** .

   Gör så här om du vill att Webhooks i Partner Center ska lyssna på händelse ändringar:

5. Välj **partner Center till Salesforce CRM (Insider Preview)** .

6. Välj **redigerings** ikonen och välj **när en http-begäran tas emot** .

7. Välj **kopierings** ikonen för att kopiera den tillhandahållna HTTP post-URL: en.

   :::image type="content" source="images/salesforce/copy-url.png" alt-text="Öppna AppSource"

    3. **Skriv över befintliga utlösare slut punkter om det finns** : Ja (detta skriver över alla befintliga slut punkter.)

11. Välj **Kör** och välj sedan **Slutför.**

Webhooken kan nu lyssna på att skapa och uppdatera händelser.

## <a name="customize-synchronization-steps"></a>Anpassa synkroniserings steg

När samförsäljnings hänvisningar synkroniseras mellan partner Center och ditt CRM-system, visas fälten som synkroniseras på Partner Center-datorn här.

CRM-system är ofta anpassade. Du kan anpassa automatiserade energi flöden. Följ guiden för fält mappning och om det behövs kan du göra lämpliga ändringar i stegen i de automatiserade energi flödena.  Microsoft Partner Center till CRM-mappningar tillhandahålls, men baserat på din CRM-miljö kan du välja att ytterligare anpassa fälten.

Flera steg i vart och ett av de automatiserade energi flödena kan anpassas efter dina behov. Följande är exempel på tillgängliga anpassningar:

1. Så här anpassar du fälten för Create-eller Update-händelserna i Partner Center till CRM referral Synchronization:

   1. Välj Partner Center till Salesforce CRM (Insider Preview).

   2. Välj **Redigera** för att redigera/anpassa det energi automatiserade flödet.

   3. Välj **(omfång) synkronisera lead eller affärs möjlighet** .

2. Om du vill anpassa fält mappningar för CRM för skapa händelser väljer du **om den är ny delad affärs möjlighet och sedan** . Välj under steget **om ja** och expandera sedan **skapa en ny affärs möjlighet i CRM** . Du kan redigera mappningarna i det här avsnittet med hjälp av fält mappnings guiden.

   1. Om du vill anpassa fält mappningar för CRM för uppdaterings händelser klickar du på steget "(omfattning) synkronisera lead eller affärs möjlighet".

   2. Välj **om det är en uppdatering av en affärs möjlighet och sedan** . Välj under steget **om ja** och expandera sedan **differensen mellan affärs möjlighets objekt i Partner Center och CRM** .  

   3. Välj **om ja** följt av **Uppdatera befintlig affärs möjlighet**

3. Så här anpassar du fälten för CRM till PC referral-synkronisering för uppdaterings händelser:

   1. Välj **Redigera**  för att redigera/anpassa det energi automatiserade flödet.

   2. Välj **(omfång) synkronisera affärs möjligheten** .

   3. För att anpassa fält mappningar för CRM (baserat på fält mappnings guide) för uppdaterings händelser väljer du **om det finns skillnader mellan lead-objekten i Partner Center och CRM** .

   4. Välj under steget **om ja** och expandera sedan steget **Uppdatera en referens med affärs möjlighets data** .

   Du kan redigera mappningarna i det här avsnittet baserat på fält mappnings guiden.

4. Vill du anpassa fälten för synkronisering av CRM till PC-hänvisning för Create Events?

   1. Välj **Redigera**  för att redigera/anpassa det energi automatiserade flödet.

   2. Välj **(omfång)-synkronisering av referenser.**

   3. För att anpassa fält mappningar för CRM (baserat på fält mappnings guide) för skapa händelser väljer du **skapa Microsoft referral** .

Du kan redigera mappningarna i det här avsnittet baserat på fält mappnings guiden.


## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a>Slutförd dubbelriktad referens synkronisering från slut punkt till slut punkt

När du har installerat, konfigurerat och anpassat den automatiserade lösningen för Energis par kan du testa synkroniseringen av referenser för samförsäljning mellan Salesforce CRM och partner Center.

### <a name="pre-requisites"></a>Förutsättningar

Om du vill synkronisera hänvisningarna över partner Center och Salesforce CRM måste den automatiserade lösningen för automatisk avgränsning av de Microsoft-speciella hänvisnings fälten. Den här identifieringen ger dina säljar grupper möjlighet att bestämma vilka hänvisningar de vill dela med Microsoft för samförsäljning.

En uppsättning anpassade fält är tillgänglig som en del av-synkroniseringen av Partner Center-referenser för Salesforce CRM-lösning för **affärs möjlighet** . En administratörs användare i CRM måste skapa ett separat CRM-avsnitt med anpassade **affärs möjlighets** fält.

Följande anpassade fält ska ingå i CRM-avsnittet:

- **Synkronisera med partner Center** : om du vill synkronisera affärs möjligheten med Microsoft Partner Center

- **Hänvisnings-ID** : ett skrivskyddat ID-fält för Microsoft Partner Center-hänvisning

- **Hänvisnings länk** : en skrivskyddad länk till hänvisningen i Microsoft Partner Center

- **Hur kan Microsoft hjälpa** : hjälp som krävs från Microsoft för hänvisning

- **Produkter** : lista över produkter som är kopplade till den här affärs möjligheten

- **Granskning** : en skrivskyddad Gransknings logg för synkronisering med partner Center-hänvisningar

### <a name="scenarios"></a>OLIKA

1. Hänvisnings-synkronisering när hänvisning skapas eller uppdateras i CRM och synkroniseras i Partner Center:

   1. Logga in på din Salesforce CRM-miljö med användare som har synlighet i avsnittet **affärs möjlighet** i CRM.

   2. Se till att följande avsnitt finns när du skapar en "ny affärs möjlighet" i Salesforce CRM-miljön

      :::image type="content" source="images/salesforce/salesforce-scenario-1.png" alt-text="Öppna AppSource" är inställt på "Ja", kommer ändringarna att synkroniseras med ditt partner Center-konto om du uppdaterar affärs möjligheten i Salesforce CRM.

   6. Affärs möjligheter som har synkroniserats med partner Center identifieras med ✔-ikonen i Salesforce CRM.

2. Hänvisnings-synkronisering när hänvisning skapas eller uppdateras i Microsoft Partner Center och synkroniseras i Salesforce CRM-miljö:

    1. Logga in på [instrument panelen](https://partner.microsoft.com/dashboard/home)för partner Center.

    2. Välj **referenser** på menyn till vänster.

    3. Skapa en ny samförsäljnings hänvisning från Partner Center genom att klicka på alternativet "nytt erbjudande".

    4. Logga in på din Salesforce CRM-miljö.

    5. Navigera till **Öppna affärs möjligheter** . Den hänvisning som skapats i Microsoft Partner Center synkroniseras nu i Salesforce CRM.

       :::image type="content" source="images/salesforce/salesforce-casino-e.png" alt-text="Öppna AppSource":::

    6. När du väljer en synkroniserad referens fylls kort visnings informationen i.

## <a name="next-steps"></a>Nästa steg

- [Hantera leads](manage-leads.md)

- [Hantera möjligheter till samförsäljning](manage-co-sell-opportunities.md)

- [Webhooks för partner Center](/partner-center/develop/partner-center-webhooks)