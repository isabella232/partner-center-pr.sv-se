---
title: Migrera från partner Sales Connect (PSC)
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Lär dig hur Microsoft-partner kan migrera från partner Sales Connect (PSC) till Partner Center och skapa eller hantera avtal som skickas av Microsofts säljare.
author: vikramb
ms.author: vikramb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 12/07/2020
ms.openlocfilehash: bbd2d1035bdcde691b0db620949d0e973667627b
ms.sourcegitcommit: 351c7ff4e6ebbb615a00190b2310156381f9cf03
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 12/07/2020
ms.locfileid: "96776924"
---
# <a name="guide-to-co-selling-in-partner-center-pc-for-partners-migrating-from-partner-sales-connect-psc"></a>Guide till samförsäljning i Partner Center (PC) för partners som migrerar från partner Sales Connect (PSC)

**Lämpliga roller**

- Kontoadministratör
- Referens administratör
- Säljare Sälj anslutning (PSC) säljare
- Administratör för partner Sales Connect (PSC)
- Avtals chef för partner Sales Connect (PSC)

Den här artikeln hjälper partners att migrera från partner Sales Connect till Partner Center så att de kan fortsätta att skapa och hantera samförsäljnings avtal i Partner Center.

Som du vet kommer företaget att förlora åtkomsten till PSC efter den 31 mars 2021. Men du kommer fortfarande att hitta allt du vill göra i Partner Center, till exempel skapa samförsäljnings avtal, hantera dina avtal och agera på avtal som skickas till dig av Microsofts säljare.

Det kommer dock att finnas skillnader. Följande rikt linjer hjälper dig att göra över gången till Partner Center mjukare och mer enkelt.

>[!Important]
> Om du är här eftersom du såg en banderoll i PSC om migreringen är du på rätt plats. Den här guiden gäller inte för lösnings bedömning (SA) och OEM IOT-partner som hanterar sina avtal i PSC.

## <a name="before-you-move-things-you-need-to-know"></a>Innan du flyttar, saker du behöver känna till

### <a name="if-you-are-a-psc-admin"></a>Om du är en PSC-administratör

- Du behöver ett e-postmeddelande för arbetet för att logga in på [partner Center](https://partner.microsoft.com/).
- Konfigurera ditt konto med hjälp av [konto administratören](permissions-overview.md)för partner Center.
- Lär dig att samsälja i Partner Center genom att läsa det här dokumentet.
- Konfigurera användar konton i Partner Center för alla dina PSC-användare (admin, avtals chef och säljar roller) och tilldela dem [referenser till administratörs roller](permissions-overview.md).

>[!IMPORTANT]
> Kontrol lera att MPN-ID: t som visas i PSC-banderollen är tillgängligt i listan över MPN-platser i Partner Center.

:::image type="content" source="images/pscmigration/mpnidcheck.png" alt-text="Bild som visar den PSC-banderoll där partner kan hitta MPN-ID: t.":::

 Om du vill kontrol lera att MPN-ID visas som en MPN-plats för partner Center loggar du in på Partner Center- [instrumentpanelen](https://partner.microsoft.com/dashboard)och väljer sedan **Inställningar** (kugg hjuls ikonen) längst upp till höger på skärmen, följt av **konto inställningar**. På den andra nivån på vänster-navigerings meny väljer du **platser** för att se en lista över alla MPN-ID: n och platser som är kopplade till Partner Center-kontot.

### <a name="if-you-are-a-psc-deal-manager-or-seller"></a>Om du är en PSC-chef eller säljare

- Du behöver en e-postadress för arbetet för att logga in på Partner Center- [instrumentpanelen](https://partner.microsoft.com/dashboard).
- Om du använder ett icke-arbetskonto i PSC eller om din e-postadress för arbetet är för ett annat företag än partner företaget, kontaktar du PSC-administratören för att få hjälp med att konfigurera konton.
- Kontrol lera med PSC-administratören om ditt konto för partner Center-kontot är klart oberoende av det konto som du använder för att logga in på PSC.
- Kontrol lera att du har åtkomst till Partner Center och avsnittet om referenser.
- Läs det här dokumentet för att förstå arbets flöden och ändringar i Partner Center.

## <a name="as-an-admin-in-psc-these-are-your-next-steps"></a>Som administratör i PSC är dessa nästa steg

Välj alternativet **hänvisningar** från menyn i den vänstra navigerings menyn i Partner Center. Bekräfta att du har åtkomst till sidorna med hänvisningar.

  >[!Note]
  > Du kan behöva logga ut från Partner Center och logga in igen för att uppdatera dina autentiseringsuppgifter för åtkomst till sidorna med referenser.

Om du inte ser alternativet " **referenser** " på menyn för partner Center eller hänvisnings sidor kontaktar du företagets [konto administratör](permissions-overview.md) och ber dem att ge dig åtkomst till alternativet för **referenser** och relaterat utrymme.

Så här hittar du ditt företags konto administratör:

1. Välj **konto inställningar** från kugg hjuls ikonen längst upp till höger i instrument panelen för partner Center.

1. Välj **användar hantering** från den andra menyn i den vänstra navigerings menyn.

1. Välj den nedrullningsbara menyn **filter** högst upp i listan användare. Ändra alternativet till **konto administratör**.

   På sidan visas alla konto administratörer med deras respektive e-postadresser. Skicka ett e-postmeddelande till en av dem och be dem att tilldela rollen som referens administratör för ditt arbets konto.

  :::image type="content" source="images/pscmigration/account-admin.png" alt-text="Bild som visar konto administratörer på sidan användar hantering för partner inställningar.":::

>[!Important]
>- Om din roll bara omfattar hantering av användare i PSC, be ditt företags konto administratör att tilldela dig rollen som [konto administratör](permissions-overview.md#manage-mpn-membership-and-your-company) i Partner Center. 
>- Om din roll även omfattar att hantera samförsäljnings möjligheter, ber vi dig tilldela rollen som [referens administratör](permissions-overview.md#manage-referrals) .
> - Det är en bra idé att även utse ett lead för ändrings hantering bland PSC-administratörerna. Om du gör det hindras alla PSC-administratörer från att kontakta sig individuellt för partner Center-konto administratörer. I stället kan ett lead för ändrings hantering vara den primära personen som arbetar med partner Center-kontots administratör.

## <a name="user-migration"></a>Användarmigrering

När du har konfigurerat ditt konto i Partner Center använder du guiden användarmigrering på sidan samförsäljnings möjligheter för att automatiskt tilldela Partner Center roller till anställda i företaget.

>[!Note]
> Användarmigrering kan bara utföras av [konto administratörer](permissions-overview.md#manage-mpn-membership-and-your-company) för ditt företag. Om du inte har rollen konto administratör kan du söka efter en konto administratör som kan hjälpa dig att skapa användar konton med hjälp av guiden Migrera användare. Funktionen för användarmigrering kommer att vara tillgänglig från den 18 november 2020.

:::image type="content" source="images/pscmigration/psc-user-migration.png" alt-text="Bild som visar guiden användarmigrering.":::

Konto administratörer ser en länk till guiden PSC-användarmigrering på sidan samförsäljnings möjligheter bredvid instruktions guiden. Användaren kan initiera migreringen genom att välja länken. Administratörer kan välja länken för att initiera användarmigrering. De kan utföra det här steget för migrering flera gånger tills alla användare har tilldelats lämpliga roller i Partner Center.

Tabellen User migration innehåller följande information:

- Användar konto – e-post-ID för medarbetaren
- PSC-partner konto – kontot som medarbetaren är associerad med i PSC
- PSC-användargrupp – en av de tre roller som har tilldelats i PSC.
- PC MPN-plats – den plats där användaren får relevanta dator roller. PSC-MPN används för att hitta motsvarande MPN-plats i Partner Center för att tilldela behörigheter. Hela organisationen anger vOrg MPN-ID.
- PC-användargrupp – medarbetare tilldelas roller baserat på deras PSC-användarkonton. Administratör i PSC tilldelas referenser till administratörs roller i PC. Säljaren tilldelas en hänvisnings användar roll i PC. Lär dig mer om dator roller och vilka användare med dessa roller kan göra i Partner Center [här](permissions-overview.md#manage-referrals)
- PC AAD-klient – klienten som användarna är tilldelade till i Partner Center
- Status – det finns tre möjliga tillstånd för migreringens status
    - **Inte migrerad** – användaren har ingen kopplad roll för PC-referenser
    - **Migrerad** – användaren har migrerats med relevant roll som har tilldelats som visas i tabellen
    - **Fel** -det gick inte att slutföra migreringen på grund av ett fel

Ibland kan migreringen misslyckats och resultera i fel. Här följer några orsaker till varför en migrering kan orsaka ett fel och några av sätten att lösa problemet:

1. PSC-användare kan använda ett konto som inte är arbets konto.

2. PSC-användaren kan använda ett konto från en annan domän än den som du använder i Partner Center.

   Om du vill lösa fel som rör scenarier 1 och 2 ber du användaren att logga in på Partner Center med hjälp av sitt arbets konto som är kopplat till din Azure AD-klient. Din [globala administratör](permissions-overview.md#manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles) kan hjälpa dig.
   
   Så här hittar du din globala administratör: 
   - Logga in på Partner Center- [instrumentpanelen](https://partner.microsoft.com/dashboard) och välj **konto inställningar** från kugg hjuls ikonen längst upp till höger.
   - Välj **användar hantering** från den andra nivån i det vänstra navigerings fältet.
   - Längst upp i listan användare väljer du List rutan **filter** och ändrar alternativet till **Global administratör**. Sidan visar sedan alla globala administratörer med deras respektive e-postadresser. Be en av dem att tilldela rollen som referens administratör för ditt arbets konto.
   
      Den globala administratören kan antingen skapa ett nytt användar konto i din Azure AD-klient eller tilldela gäst användare åtkomst till andra domän konto användare. När kontona har kon figurer ATS för alla PSC-chefer och användare måste de logga in på Partner Center, välja **referenser** på menyn till vänster-navigering och bekräfta att de kan se sidan hänvisningar.

3. Användaren har redan en hänvisnings roll tilldelad i Partner Center.
    - Du kan verifiera användarens befintliga roll. I det övre högra hörnet av Partner Center väljer du **Inställningar** (kugg hjuls ikonen) och sedan **konto inställningar**. När du ser en andra vänster-navigerings meny väljer du **användar hantering** och söker efter användaren.

När du är klar med migreringen av användare kan du använda följande vägledning för att bestämma strategin för migreringen:

Om ditt företag har en partner utvecklings chef (PDM) – när ditt partner Center-konto har kon figurer ATS och dina användare har flyttat och har roller och behörigheter, kan du flytta dina samförsäljnings aktiviteter till Partner Center. Informera PDM för att göra växeln i stället för att vänta tills migreringen har slutförts, vilket gör det möjligt för alla nya avtal att flöda till Partner Center.

>[!Note]
>När du har gjort den här växeln kommer du bara att kunna agera på befintliga aktiva avtal i PSC. Du kan varken skapa nya eller få några avtal från Microsofts säljare i PSC.

Om ditt företag inte har en PDM – se till att alla användar konton är inställda och verifierade av alla användare. Du kommer att meddelas via ett e-postmeddelande och en banderoll i PSC om det exakta datumet när du kan påbörja samförsäljning i Partner Center. Kom ihåg att du fortfarande måste hantera befintliga aktiva avtal i PSC.

>[!Important]
>Aktiva avtal kommer inte att migreras till datorn. Du har fram till den 31 mars 2021 att stänga och registrera avtalen.

## <a name="next-steps-for-psc-admins-psc-deal-managers-and-psc-sellers"></a>Nästa steg för PSC-administratörer, PSC-chefer och PSC-säljare

Lär dig att samsälja i Partner Center.
Det här är ett viktigt steg som hjälper dig att förbereda för samförsäljning i Partner Center. Förstå arbets flödena och ändringarna i Partner Center så att du effektivt kan samsälja omedelbart. Börja med att läsa det här dokumentet helt. Det finns också en utmärkt uppsättning resurser i [galleriet för co-försäljnings upplevelser](https://aka.ms/cosellexperience).

## <a name="major-differences-between-psc-and-pc-workflows"></a>Större skillnader mellan PSC-och PC-arbetsflöden

|**Scenario**|**Partner Sälj anslutning**|**Partnercenter**|
|-----|:-----|:-----|
|Användarroller|PSC har rollen administratör, avtals chef och säljare.|DATORN har bara [referens administratörs](permissions-overview.md#manage-referrals) rollen som ger både Läs-och Skriv behörighet för alla avtal.|
|Att bjuda in Microsoft på ett co-försäljnings avtal|Som initieras av Microsoft-säljaren finns det ingen uttrycklig fråga från partner.|Partner måste göra en [uttrycklig begäran](manage-co-sell-opportunities.md#add-solutions) om en Microsoft-säljares hjälp krävs för ett erbjudande. Microsoft-säljaren har möjlighet att avvisa begäran.|
|Upphörande|Det finns inget begrepp för en avtals utgång.|Partners ingående avtal upphör att gälla om 14 dagar om de inte godkänns av partnern. Samma sak gäller för partner utgående avtal där de kan gå in till utgången tillstånd om Microsoft-säljaren inte agerar på dem inom 14 dagar.|
|Microsoft-säljar information|Visas så fort ett avtal skapas.|Microsofts säljar information delas med endast partner om säljaren uttryckligen accepterar inbjudan till samförsäljning från partner.|
|[Privat pipeline](manage-co-sell-opportunities.md#types-of-co-sell-opportunities)|Inte tillgängligt.|Partner kan dela sin pipeline utan att ge dig insyn i Microsofts säljare.|
|Lösningar|Lösningar som tillhör en pris lista kan läggas till i ett avtal.|Partner kan lägga till [lösningar](manage-co-sell-opportunities.md#add-solutions) som tillhör följande listor. a) lösningar för egna lösningar b-lösningar från Microsofts första parts katalog (liknar transaktions avtals rollen i PSC) och c) samförsäljnings lösningar från andra partner från tredje part (liknar rollen för ISV-erbjudandet i PSC).|
|Avtals tilldelning|Endast tilldelade säljare kan visa och agera på avtalen.|Grupp medlemmar kan läggas till i ett avtal för att ange de personer som arbetar på ett avtal, det finns ingen spärr av andra hänvisnings administratörer från att visa eller agera på dessa avtal.|
|Kund organisation|Text inmatning med fritext.|Du kan söka i [kund organisationen](manage-co-sell-opportunities.md#select-your-customer) mot [D&B-databasen](https://www.dnb.com/) genom att bara skriva några tecken. Det juridiska namnet och adressen fylls i automatiskt baserat på valet.|
|Kund kontakt|Inte obligatoriskt.|Inte obligatoriskt för delning av privat pipeline. Krävs om Microsoft-säljaren bjuds in att delta i en samförsäljnings förfrågan.|
|Offentligt API|Inte tillgängligt.|[Offentligt API](/partner/develop/referrals) för att hantera Partner Center-hänvisningar via programmering.|

## <a name="map-the-fields-in-psc-to-the-corresponding-fields-in-partner-center"></a>Mappa fälten i PSC till motsvarande fält i Partner Center

I det här avsnittet jämförs (eller "Maps") valda skärm bilder som visas för PSC mot motsvarande vy i avsnittet om samarbets möjligheter i Partner Center.

Du kommer att se numrerade, gula eller röda cirklar på varje skärm bilds par:

- **Vad betyder gula cirklar?** Numrerade, gula cirklar visas först på varje PSC-skärm. Sedan hittar du en skärm bild av en medföljande partner Center under den med många av samma siffror.

   Om du vill se hur varje fält eller attribut i PSC mappar till dess motsvarighet i Partner Center matchar du de numrerade cirklarna i de två relaterade skärm bilderna. Du kan till exempel matcha det numrerade, gula "1" i den första PSC-bildskärmen till den numrerade, gula "1" i den andra, skärm bilden för partner Center.

- **Vad betyder en röd cirkel?** Om du ser en röd cirkel på en skärm bild, betyder det att PSC-fältet inte är tillgängligt i Partner Center.

Fält mappningar för PSC-till-Partner-Center visas för följande områden:

1. PSC-startsida som är mappad till standard visningen för partner Center-samförsäljnings möjligheter
1. Vyn PSC-rutnät som är mappad till Partner Center-vyn för avtal
1. Översikt över PSC-information mappad till vyn information om Partner Center
1. PSC-vyn Lägg till produkter mappad till vyn Partner Center Lägg till lösningar
1. PSC-vy för användar hantering mappad till vyn användar hantering i Partner Center
1. Uppslagsvy för roll tilldelning för PSC mappas till Roll tilldelnings vyn Partner Center
1. Vyn PSC-meddelanden mappad till vyn Partner Center-meddelanden

### <a name="1---psc-home-page-mapped-to-the-partner-center-co-sell-opportunities-default-view"></a>1 – PSC-startsida som är mappad till standard visningen för partner Center-samförsäljnings möjligheter

Jämför matchande, numrerade cirklar mellan den övre PSC-bildskärmen och skärm bilden för partner Center. Matchnings nummer visar var du kan hitta den PSC-relaterade funktionen eller attributet i Partner Center. Röda cirklar visar att det inte finns något matchande Partner Center-fält.  

:::image type="content" source="images/pscmigration/homepage.png" alt-text="Bild som visar fält mappningar mellan start sidan för partner Sales Connect och standard visningen av samförsäljnings möjligheter i Partner Center." lightbox="images/pscmigration/home-page-expanded.png":::

### <a name="2---psc-grid-view-mapped-to-the-partner-center-deal-view"></a>2 – vy för PSC-rutnät som är mappat till Partner Center-vyn för avtal

Jämför matchande, numrerade cirklar mellan den övre PSC-bildskärmen och skärm bilden för partner Center. Matchnings nummer visar var du kan hitta den PSC-relaterade funktionen eller attributet i Partner Center. Röda cirklar visar att det inte finns något matchande Partner Center-fält.  

> [!NOTE]
> Andra överväganden visas under skärm bilderna.

:::image type="content" source="images/pscmigration/gridview.png" alt-text="Bild som visar fält mappningar mellan den PSC-rutnätsvy (partner Sales Connect) och vyn Partner Center." lightbox="images/pscmigration/grid-view-expanded.png":::

**Särskilda överväganden:**

- Det finns ingen listvy i Partner Center som i PSC.  Alla avtal visas utifrån det senaste mottagna eller skapade datumet med kund informationen och typen av avtal. Det första erbjudandet i vyn är valt som standard. De flesta av de värden som visas i formatet PSC är tillgängliga i vyn detaljerad information för affären i PC.
- Avtals roll är inte ett obligatoriskt fält i PC. Den visas eller registreras inte i någon av arbets flödena. Den härleds automatiskt på Microsofts säljare sida baserat på de lösningar som lagts till i affären.
- Datumet för senaste ändring visas inte på sidan med hänvisnings information i PC. Partner kan använda sorterings funktionen för att sortera avtalen utifrån det senaste uppdaterade datumet.

### <a name="3---psc-deal-details-view-mapped-to-partner-center"></a>3 – PSC-vyn avtals information mappad till Partner Center

Jämför matchande, numrerade cirklar på den översta skärm bilden (PSC) med partner Center skärm bilden. Matchnings nummer visar var du kan hitta den PSC-relaterade funktionen eller attributet i Partner Center. Röda cirklar visar att det inte finns något matchande fält eller område i Partner Center.

> [!NOTE]
> Andra överväganden visas under skärm bilderna.

:::image type="content" source="images/pscmigration/dealdetails.png" alt-text="Bild som visar fält mappningar mellan vyn PSC-avtal (partner Sales Connect) och vyn information om Partner Center." lightbox="images/pscmigration/deal-details-expanded.png":::

**Särskilda överväganden:**

- Partner kan redigera ett avtal genom att välja knappen Redigera i vyn partner avtals information (6). När du har valt knappen Redigera går alla fält att redigera. Du kan sedan välja att antingen Spara eller avbryta ändringarna som gjorts i affären.
- Det finns inget alternativ för att stänga affären som dubblett i Partner Center.
- Kund resultatet är inte tillgängligt i Partner Center. All information som rör kund interaktioner kan uppdateras i avsnittet anteckningar i PC.
- Den uppskattade lösningens stängnings datum är bara tillgängligt för OEM IOT-avtal i Partner Center. Den här informationen visas inte för några andra avtals typer.
- Licens programmet krävs inte i PC. Den här informationen härleds automatiskt baserat på de lösningar som valts i affären.

>[!Note]
>Alla avtal som marker ATS som vunna eller förlorade kan inte redige ras efteråt. Var försiktig när du flyttar ett avtal till något av dessa terminaler-tillstånd.

### <a name="4---psc-add-products-view-mapped-to-the-partner-center-add-solutions-view"></a>4 – PSC-vyn Lägg till produkter som är mappad till Partner Center-vyn Lägg till lösningar

Jämför matchande, numrerade cirklar på den översta skärm bilden (PSC) med partner Center skärm bilden. Matchnings nummer visar var du kan hitta den PSC-relaterade funktionen eller attributet i Partner Center. Röda cirklar visar att det inte finns något matchande fält eller område i Partner Center.
  
:::image type="content" source="images/pscmigration/products.png" alt-text="Bild som visar fält mappningarna mellan vyn för att lägga till produkter i partner Sales Connect (PSC) och vyn Lägg till lösningar i Partner Center." lightbox="images/pscmigration/products-expanded.png":::

### <a name="5---user-management-in-psc-versus-partner-center"></a>5 – användar hantering i PSC jämfört med partner Center

Jämför matchande, numrerade cirklar på den översta skärm bilden (PSC) med partner Center skärm bilden. Matchnings nummer visar var du kan hitta den PSC-relaterade funktionen eller attributet i Partner Center. Röda cirklar visar att det inte finns något matchande fält eller område i Partner Center.  

 :::image type="content" source="images/pscmigration/usermanagement.png" alt-text="Bild som visar fält mappningarna mellan webbplatsen för användar hantering i partner Sales Connect (PSC) och användar hanterings sidan för partner Center i området konto inställningar."  lightbox="images/pscmigration/user-management-expanded.png":::

### <a name="6---user-role-assignment-in-psc-versus-partner-center"></a>6-användar roll tilldelning i PSC jämfört med partner Center

Jämför matchande, numrerade cirklar på den översta skärm bilden (PSC) med partner Center skärm bilden. Matchnings nummer visar var du kan hitta den PSC-relaterade funktionen eller attributet i Partner Center. Röda cirklar visar att det inte finns något matchande fält eller område i Partner Center.  

:::image type="content" source="images/pscmigration/roles.png" alt-text="Bild som visar fält mappningar mellan vyn PSC-roll tilldelning för partner Sälj Connect (PSC) och roll tilldelningen Partner Center." lightbox="images/pscmigration/roles-expanded.png":::

**Särskilda överväganden:**

- Rollen som motsvarighet för PSC-administratör är rollen konto administratör i Partner Center.
- Det finns bara en roll i Partner Center för avtals hantering i Co-försäljning. Den här rollen är referens administratörs rollen.

### <a name="7---notifications-in-psc-versus-partner-center"></a>7 – meddelanden i PSC jämfört med partner Center

Jämför matchande, numrerade cirklar på den översta skärm bilden (PSC) med partner Center skärm bilden. Matchnings nummer visar var du kan hitta den PSC-relaterade funktionen eller attributet i Partner Center. Röda cirklar visar att det inte finns något matchande fält eller område i Partner Center.  

:::image type="content" source="images/pscmigration/notifications.png" alt-text="Bild som visar mappningen mellan en PSC-avisering (partner Sales Connect) och vyn meddelande för partner Center."  lightbox="images/pscmigration/notifications-expanded.png":::

## <a name="moving-from-psc-to-partner-center---frequently-asked-questions"></a>Flytta från PSC till Partner Center – vanliga frågor och svar

I följande avsnitt besvaras vanliga frågor om migreringen.

### <a name="1---what-should-i-do-if-i-dont-have-access-to-partner-center"></a>1 – Vad ska jag göra om jag inte har åtkomst till Partner Center?

Du kan kontakta dina administratörer på sidan "ingen åtkomst" för att hämta de roller som har tilldelats. Du behöver rollen som [referens administratör](permissions-overview.md#manage-referrals) för Läs-och Skriv behörighet i avsnittet hänvisningar. Om du bara hanterar affärs profiler behöver du rollen affärs profil administratör i Partner Center.

:::image type="content" source="images/pscmigration/noaccess.png" alt-text="Bild som visar ingen åtkomst upplevelse i Partner Center.":::

### <a name="2---who-can-grant-me-access-to-the-referrals-section-in-partner-center"></a>2 – vem kan ge mig åtkomst till avsnittet referenser i Partner Center?

Din [konto administratör](permissions-overview.md#manage-mpn-membership-and-your-company) kan ge dig åtkomst till fliken hänvisningar. Om du vill hitta din konto administratör väljer du **konto inställningar** från kugg hjuls ikonen längst upp till höger i [instrument panelen](https://partner.microsoft.com/dashboard)för partner Center. Välj sedan **användar hantering** från den andra nivån i det vänstra navigerings fältet. Längst upp i listan användare väljer du List rutan **filter** och ändrar alternativet till **konto administratör**. På sidan visas alla konto administratörer med deras respektive e-postadresser. Be en av dem att tilldela rollen som referens administratör för ditt arbets konto.

### <a name="3---the-new-deal-button-is-greyed-out-for-our-account-what-should-i-do-to-start-creating-deals"></a>3 – knappen + ny affär är nedtonad för vårt konto. Vad ska jag göra om jag vill börja skapa avtal?

Detta sker bara om det inte finns några samförsäljnings klara lösningar som är kopplade till MPN-organisationen som du använder i Partner Center. Kontakta din PDM för att få MPN-ID: t för dina lösningar korrigerade eller skapa ett support ärende som nämner problemet, "ny avtals knapp som är nedtonad efter PSC-migreringen".

### <a name="4---can-i-assign-deals-to-a-specific-person-from-our-organization-like-psc"></a>4 – kan jag tilldela avtal till en speciell person från vår organisation som PSC?

Du kan tilldela team medlemmar till ett bestämt avtal. Den blockerar inte andra hänvisnings administratörer från att visa eller agera på dessa avtal.

### <a name="5---is-there-a-view-of-all-the-deals-assigned-to-me"></a>5 – finns det en vy över alla tilldelade avtal?

Du kan använda funktionen favoriter, som är en flik på användar nivå. Du kan markera alla avtal som har tilldelats dig som favoriter för att få en snabb till gång till avtalen.

### <a name="6---is-there-a-read-only-view-for-the-deals"></a>6 – finns det en skrivskyddad vy för avtalen?

Nej, det finns ingen skrivskyddad vy över avtalen i avsnittet om referenser. Alla referens administratörer får fullständig Läs-och Skriv behörighet för alla avtal.

### <a name="7---how-can-i-register-a-deal-after-marking-it-as-won"></a>7 – Hur kan jag registrera ett avtal när jag har markerat det som vunnit?

Om avtalet uppfyller nedanstående villkor visar vi ett popup-fönster för att börja [avtals registreringen](./register-deals.md).

- Det finns en incitaments berättigad lösning som är kopplad till affären.
- Microsoft-säljaren bjuds in att delta i affären eller bjuds in till affären.
- Microsoft-kortet har godkänts eller vunnit status i Partner Center.

### <a name="8---i-get-an-error-message-when-i-select-the-new-deal-registration-button-in-the-deal-registration-section-how-can-i-register-my-deals"></a>8 – jag får ett fel meddelande när jag väljer knappen "+ ny avtals registrering" i avsnittet avtals registrering. Hur kan jag registrera mina avtal?

Knappen **+ ny avtals registrering** ska endast användas av de partner som är registrerade i ISV Connect-programmet för att registrera ett avtal utan motsvarande samförsäljnings möjlighet i Partner Center. För att registrera avtal med en samförsäljnings möjlighet visas ett popup-fönster när affären är markerat som vunnen och om det uppfyller villkoren för avtals registrering.

### <a name="9---is-adding-a-customer-organization-mandatory"></a>9 – lägger till en kund organisation obligatorisk?

Ja, det är obligatoriskt att lägga till en [kund organisation](./manage-co-sell-opportunities.md#select-your-customer) i Partner Center. Börja med att söka efter platsen där kunden är plats. Utifrån den information som du har. Du kan vara speciell, inklusive det exakta namnet på byggnaden eller bara ge information om ort. Organisations sökningen hämtar alla juridiska entiteter som matchar det namn som du anger så att du inte behöver ange någon adress information. All information fylls i automatiskt baserat på vald organisation.

### <a name="10---are-customer-contact-details-mandatory"></a>10 – är kundens kontakt uppgifter obligatorisk?

Beror på vilken [typ av avtal](./manage-co-sell-opportunities.md#types-of-co-sell-opportunities) du skapar. Om du bara delar din pipeline och inte behöver någon hjälp från Microsoft Sales-organisationen kan du välja att inte ge kund kontakt uppgifter. Om du är samförsäljnings plats där du aktivt söker efter hjälp från Microsoft-säljaren måste du ange kundens kontakt uppgifter. Du bör få ett uttryckligt medgivande från kunden innan du skapar en samförsäljnings förfrågan i Partner Center.

### <a name="11---how-many-solutions-can-i-add-to-a-deal"></a>11 – Hur många lösningar kan jag lägga till i ett avtal?

Du kan lägga till upp till 50 lösningar (analoga till "produkter" i PSC) i ett avtal. Till skillnad från PSC kan du blanda lösningar från dina egna samsäljande lösningar, Microsofts första parts SKU: er och andra utomstående kvalificerade lösningar från tredje part. Det finns ingen avtals roll som ska väljas eller vara tillgänglig i Partner Center. För Microsoft SKU: er kan du välja att lägga till kvantitet och pris för varje SKU som läggs till i affären.

### <a name="12---when-will-i-get-to-know-the-microsoft-seller-details-after-creating-a-deal"></a>12 – När får jag veta Microsofts säljar information när jag har skapat ett avtal?

Microsoft-säljare tilldelas endast efter att ha matchat det exakta hjälp kravet som anges när du skapar affären med den berörda säljaren persona på Microsoft-sidan. Även efter tilldelningen har Microsoft-säljare ett alternativ för att acceptera eller avvisa inbjudan till co-försäljning. Om en säljare har accepterat en gemensam inbjudan kommer affären att uppdateras med kontakt uppgifterna för Microsoft-säljaren. Service avtalet för Microsoft-säljarna för att agera med erbjudandet är 14 dagar. Det är samma service avtal som partners måste vidta för att agera i affären innan det går in i det tillstånd som gått ut.

### <a name="13---where-can-i-find-the-opportunity-id"></a>13 – var kan jag hitta ett affärs möjlighets-ID?

Affärs möjlighets-ID i PSC är detsamma som i avsnittet om avtals-ID i PC. Du kan hitta avtals-ID: t bredvid avtals namnet när du öppnar ett avtal.

### <a name="14---how-can-my-pdm-get-access-to-pc"></a>14 – Hur kan mitt PDM få åtkomst till datorn?

Det går inte att komma åt Partner Center från PDM direkt till skillnad från PSC. Det finns flera alternativ för att aktivera funktionen, som nämns nedan.

- OCP Insights – om PDM bara visar de avtal och framsteg som är relaterade till dem kan de använda OCP Insights-portalen för att få din organisations vy. Det här är ett internt verktyg som endast är tillgängligt för PDM. Observera att OCP Insights inte är tillgängliga för ditt företags användare.
- Gäst användare i Partner Center – du kan lägga till ditt PDM- @microsoft.com konto som gäst användare i Partner Center och tilldela rollen som referens administratör så att de kan visa och agera på hänvisningar.
- Skapa en [ny användare](./create-user-accounts-and-set-permissions.md#add-a-new-user) i din klient organisation – du kan skapa en ny användare i din egen klient och dela den informationen med PDM så att de kan visa och agera på referenser som liknar andra hänvisnings användare i ditt konto.

## <a name="resources-to-help-you-create-and-manage-your-deals-in-partner-center"></a>Resurser som hjälper dig att skapa och hantera dina avtal i Partner Center

Om du inte redan har läst de samsäljiga hjälp avsnitten kan följande resurser hjälpa dig att hantera avtal i Partner Center.

|**För att göra detta**   |**Läs detta**   |
|-----------------------|:-----------------------|
|Förstå flikarna och navigeringen på sidan affärs möjligheter för samförsäljning|[Navigera i avsnittet Co-Sälj](./manage-co-sell-opportunities.md#navigating-the-co-sell-section)|
|Välja en kund organisation från D&B-listan |[Välj din kund](./manage-co-sell-opportunities.md#select-your-customer)|
|Ändra fälten i avsnittet om avtals information|[Information om avtal](./manage-co-sell-opportunities.md#deal-details)|
|Lägga till team medlemmar i ett avtals lag|[Lägg till dina anställda](./manage-co-sell-opportunities.md#add-team-members)|
|Svara på ett samförsäljnings avtal|[Hantera samförsäljnings avtal](./manage-co-sell-opportunities.md#responding-to-a-co-sell-opportunity)
|Registrera erbjudanden som du har vunnit i Partner Center |[Registrera ett nytt avtal](./register-deals.md)
|Kom igång med referral Insights och ta reda på hur dina hänvisningar fungerar |[Hänvisningsinsikter](./referral-insights.md)
|Skapa och hantera företags profil|[Hantera företagsprofil](./create-a-marketing-profile.md)
|Hantera leads för din företags profil |[Hantera leads](./manage-leads.md)|

## <a name="next-steps"></a>Nästa steg

Följ dessa ytterligare resurser:

- [Partner försäljning Anslut till Partner Center arbets bok](https://partner.microsoft.com/resources/detail/partner-sales-connect-to-partner-center-transition-workbook-pptx) – arbets bok för att anpassa partners försäljnings processer och roller med nya försäljnings processer via partner Center eller partner Sales Connect.
- [Samarbets guide för partner Center](https://partner.microsoft.com/resources/detail/co-sell-operating-model-guide-pptx) – rikt linjer för att identifiera en drifts modell via partner Center för att hantera leads eller samförsäljnings möjligheter och registrera avtal.
- [Referens hanterings däck](https://partner.microsoft.com/resources/detail/referral-management-in-partner-center-pptx) – visualiserade steg-för-steg-instruktioner för att hantera leads och samförsäljnings möjligheter via partner Center.
- [Publicera och hantera i den kommersiella Marketplace](https://partner.microsoft.com/resources/detail/publishing-and-managing-co-sell-offers-in-commercial-marketplace-pptx) – visualiserade steg-för-steg-instruktioner för att skapa, hantera och publicera erbjudanden via partner Center på den kommersiella marknaden.