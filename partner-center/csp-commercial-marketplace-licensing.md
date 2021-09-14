---
title: Hantera licensiering i Marketplace-erbjudanden
ms.topic: how-to
ms.date: 04/29/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
description: Lär dig hur du ställer in och hanterar licensiering för dina erbjudanden på den kommersiella ISV-marknadsplatsen.
author: petand123
ms.author: v-petand
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 73a02a0a6cad28939d21800c726811c8969ce9a2
ms.sourcegitcommit: 37eac16c4339cb97831eb2a86d156c45bdf6a531
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/13/2021
ms.locfileid: "126246895"
---
# <a name="manage-licensing-in-marketplace-offers"></a>Hantera licensiering i Marketplace-erbjudanden

**Lämpliga roller:** Globala | Kontoadministratör

Den här artikeln beskriver steg för steg hur du ställer in ett erbjudande i Partnercenter, gör det tillgängligt i Microsoft AppSource och sedan hanterar licenser för erbjudandet.  

>[!IMPORTANT]
>Funktionerna i den här artikeln är för närvarande i allmänt tillgänglig förhandsversion.

## <a name="before-you-begin"></a>Innan du börjar

### <a name="commercial-marketplace-basics"></a>Grundläggande om den kommersiella marknadsplatsen

Innan du påbörjar den här processen bör du bekanta dig med grunderna i den kommersiella marknadsplatsen. Artiklarna i tabellen nedan hjälper dig att komma igång. 

| Avsnitt  | Artikel  |
|-------|--------|
|Planer för den kommersiella marknadsplatsen | [Planer och priser för erbjudanden på den kommersiella marknadsplatsen](/azure/marketplace/plans-pricing)    |
|Erbjudanden på den kommersiella marknadsplatsen  | [Lista typer](/azure/marketplace/determine-your-listing-type)    |
|Konton på den kommersiella marknadsplatsen |  [Skapa ett konto för den kommersiella marknadsplatsen i Partnercenter](/azure/marketplace/create-account) |

### <a name="determine-your-offer-id"></a>Fastställa ditt erbjudande-ID

I procedurerna nedan uppmanas du att ange ett erbjudande-ID. Ta dig tid att ta fram ett lämpligt erbjudande-ID, med följande i åtanke:

- Det här ID:t är synligt för kunder i webbadressen för Marketplace-erbjudandet och Azure Resource Manager mallar, om tillämpligt.
- Erbjudande-ID i kombination med Publisher-ID måste vara under 40 tecken långt.
- Använd bara gemena bokstäver och siffror. Erbjudande-ID:t kan innehålla bindestreck och understreck, men inga blanksteg. Om ditt id för Publisher är `testpublisherid` och du anger blir `test-offer-1` erbjudandets webbadress `https://appsource.microsoft.com/product/dynamics-365/testpublisherid.test-offer-1` .
- Det här ID:t kan inte ändras när du har valt **Skapa**.

### <a name="determine-your-offer-alias"></a>Fastställa ditt erbjudandealias

Erbjudandets alias är det namn som används för erbjudandet i Partnercenter. Du behöver också ett lämpligt erbjudandealias som följer riktlinjerna nedan:

- Det här namnet används inte på Marketplace och skiljer sig från erbjudandets namn och andra värden som visas för kunder.
- Det går inte att ändra det här namnet när du har valt Skapa.

## <a name="create-your-offer"></a>Skapa ditt erbjudande

Det första steget i licensieringsprocessen är att skapa ditt erbjudande på den kommersiella marknadsplatsen. 

1. Logga in på [instrumentpanelen i Partnercenter](https://partner.microsoft.com/dashboard/).
2. I den vänstra navigeringsmenyn väljer du **Kommersiell marknadsplats/Översikt.**
3. Längst upp på sidan Översikt väljer du **Nytt erbjudande** och sedan **Dynamics 365 for Customer Engagement & PowerApps**.
4. Ange det **erbjudande-ID och** **erbjudandealias** som du skapade tidigare.
5. Välj **Skapa** för att generera erbjudandet och fortsätta.
6. Välj dina licensieringsalternativ.

    - Om du vill aktivera licenshantering för ditt erbjudande väljer **du Aktivera applicenshantering via Microsoft**. Det här är en enda inställning och du kan inte ändra den när ditt erbjudande har publicerats.

    - Du kan också låta kunder köra appens grundläggande funktioner utan licens och köra Premium-funktioner när de har köpt en licens. Det gör du genom att **välja Tillåt att kunder installerar min app även om licenserna inte har tilldelats**.

    - Om du inte vill att ditt erbjudande ska ha licenshantering aktiverat väljer du Hämta nu **(kostnadsfri)**, **Kostnadsfri utvärderingsversion** eller **Kontakta mig.**

## <a name="create-your-plan"></a>Skapa din plan

I de här stegen definierar du den plan eller de planer som du vill aktivera för ditt erbjudande.

1. I den vänstra navigeringsmenyn väljer **du Planera översikt** och sedan Skapa ny **plan.**
2. Ange ett **plan-ID** **och ett plannamn** och välj sedan **Skapa.**
3. På sidan **Planlista** anger du din **planbeskrivning.**
4. Om du vill spara beskrivningen och avsluta senare väljer du **Spara utkast.**

5. När du är klar väljer du **Granska och publicera**. Informationen om planen visas nu på sidan appsource.microsoft.com under erbjudandelistan (avsnittet med planer).

6. När du har skapat alla planer för det här erbjudandet måste du kopiera tjänst-ID:t för varje plan. Välj **Översikt över** plan överst på sidan Planlista. Kopiera tjänst-ID:t för varje plan till en säker plats.

## <a name="add-service-ids-to-your-solution"></a>Lägga till tjänst-ID:er i din lösning

Nästa steg är att uppdatera din lösning genom att lägga till tjänst-ID:erna för varje plan som du nyss kopierade. Vägledning om detta finns i [Skapa ett AppSource-paket för din lösning.](/powerapps/developer/data-platform/create-package-app-appsource)

## <a name="upload-your-package-and-publish-your-offer"></a>Upload ditt paket och publicera ditt erbjudande

1. I det vänstra navigeringsfönstret väljer du **Kommersiell marknadsplats** och sedan **Teknisk konfiguration.**
2. Under **Baslicensmodell** väljer du **Användare.**
3. Under **CRM-paket** anger du URL:en för din paketplats.
4. Använd de andra flikarna i det vänstra navigeringsfönstret för att ange annan nödvändig information. När du är klar väljer du **Granska och publicerar**.

När du har publicerat erbjudandet granskar och verifierar vi din information. Om det finns några problem med den här processen meddelar vi dig. När alla problem har lösts får du ett meddelande om att ditt erbjudande är tillgängligt i AppSource. Då kan du göra det live.

## <a name="make-your-offer-live-in-partner-center"></a>Gör ditt erbjudande live i Partnercenter

Proceduren nedan går igenom processen för att göra ditt erbjudande live i AppSource. Mer information om den här processen finns i [Introduktion till listalternativ.](/azure/marketplace/determine-your-listing-type)

>[!NOTE]
>När du har publicerat ditt erbjudande tar det 4–6 timmar att publicera det.

1. Logga in på [instrumentpanelen i Partnercenter](https://partner.microsoft.com/dashboard/).
2. I den vänstra navigeringsmenyn väljer du **Kommersiell marknadsplats/Översikt.**
3. På **sidan** Översikt letar du reda på det erbjudande som du letar efter. Erbjudanden som är klara att publiceras har statusen **Förhandsversion.** Välj erbjudandet.
4. På sidan **Översikt över** erbjudande väljer du **Go live**.
Erbjudandet är live om 4–6 timmar.
5. Om du vill se din erbjudandelista på AppSource väljer du **länken AppSource** längst ned på **översiktssidan för** erbjudandet.

    - **För licensaktiverade erbjudanden:** Om ditt erbjudande kräver en licenskontroll kan användarna bara ange ett lead genom att klicka på **Kontakta** mig så att du kan kommunicera med dem.

    - **För licensaktiverade** erbjudanden med alternativet för kostnadsfri installation: Om ditt erbjudande  inte kräver en licenskontroll ser administratörsanvändarna knappen Hämta nu utöver **Kontakta mig.** Användare som vill testa ditt kostnadsfria installationsalternativ bör klicka på **Hämta** nu, vilket gör att de kan installera erbjudandet i Power Platform Administrationscenter. Användarna kan fortfarande använda **Kontakta mig** om de har frågor eller om de vill uppgradera till en betald plan.

## <a name="register-isv-connect-deal-in-deal-registration"></a>Registrera ISV Anslut avtal i Avtalsregistrering

Innan du kan tilldela licenser till en kund måste varje försäljning registreras i Partnercenter. Information om hur du gör detta finns [i Registrera dina avtal.](register-deals.md)

## <a name="invite-the-customer"></a>Bjud in kunden

Använd följande procedur för att bjuda in kunden att delta i detta avtal.  

1. Logga in på [instrumentpanelen i Partnercenter](https://partner.microsoft.com/dashboard/).
2. I den vänstra navigeringsmenyn väljer du **Kommersiell marknadsplats/Översikt.**
3. I den vänstra navigeringsmenyn **väljer du Referenser** och sedan **Avtalsregistrering.**
4. Filtrera på **Skickade** avtal, välj **fliken Pågår** och välj sedan det avtal som du vill ha.
5. På översiktssidan för det här avtalet väljer du **Hantera licenser.**
6. I fönstret **Hantera** licenser väljer du kunden i **listrutan Kundinformation.** Om kundrelationen inte finns ännu väljer du **+Bjud in en ny kund att godkänna**.
7. Kopiera länken som visas.
8. Skicka den här länken via e-post till din kunds faktureringsadministratör eller globala administratör och be dem använda den här länken för att komma åt admin.microsoft.com och godkänna och auktorisera relationen som du upprättar.

    >[!NOTE]
    >Relationen upprättas inte förrän kunden utför det här steget.

## <a name="activate-manage-and-remove-your-licenses"></a>Aktivera, hantera och ta bort dina licenser

När kunden har godkänt relationen med dig kan du börja lägga till planer från ditt erbjudande och tilldela licenser till varje plan.

1. I fönstret Hantera licenser för det här avtalet väljer du **+Lägg till en plan**.
2. Slutför fälten **Planer för den här** lösningen och **Antal** licenser och välj sedan **Uppdatera licenser.** Licenserna blir tillgängliga på admin.microsoft.com kunder kan hantera och tilldela till anställda.

    - Om du vill ändra antalet licenser för en befintlig plan anger du det nya numret i fältet Antal **licenser** och väljer sedan **Uppdatera licenser.**

    - Om du vill inaktivera eller ta bort licenser för ett avtal väljer du papperskorgsikonen **i fältet Åtgärder** och väljer sedan Uppdatera **licenser.**

## <a name="next-steps"></a>Nästa steg

[Licensieringsresurser](support-resources-licensing.md)