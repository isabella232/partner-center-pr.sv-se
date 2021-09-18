---
title: Migrera från Partner Sales Anslut (PSC)
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-referrals
description: Lär dig hur Microsoft-partner kan migrera från Partner Sales Anslut (PSC) till Partner Center och skapa eller hantera avtal som skickas av Microsoft-säljare.
author: vikramb
ms.author: vikramb
ms.localizationpriority: medium
ms.date: 09/08/2021
ms.openlocfilehash: 96106dd84d4889c9165daf41385d1092361101c4
ms.sourcegitcommit: 5abf065c8852a858a0aa7185176d3e117f2be7e5
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/18/2021
ms.locfileid: "127958903"
---
# <a name="guide-to-co-selling-in-partner-center-pc-for-partners-migrating-from-partner-sales-connect-psc"></a>Guide till säljpartner i Partnercenter (PC) för partner som migrerar från Partner Sales Anslut (PSC)

**Lämpliga roller:** Kontoadministratörsroller | Referenser admin | Partner Sales Anslut (PSC) | Partner Sales Anslut (PSC) admin | Avtalsansvarig Anslut Partner Sales Anslut (PSC)

Den här artikeln innehåller vägledning för partner som migrerar från Partner Sales Anslut (PSC) till Partner Center (PC) så att de kan fortsätta att skapa och hantera samförsäljningserbjudanden i Partnercenter.

> [!NOTE]
> Om du är här eftersom du såg en banderoll i PSC om migreringen är du på rätt plats. Den här guiden gäller inte för Solution Assessment (SA) och OEM-licensieringspartner som hanterar sina avtal i PSC.

> [!IMPORTANT]
> Från och med den 1 april 2021 kommer ditt företag inte att kunna skapa eller redigera avtal i PSC. **Du kommer fortfarande att kunna ladda ned befintliga avtalsdata med hjälp av massexport-funktionen i PSC. Du kan också [migrera öppna avtal](psc-to-pc.md#psc-deals-migration) från PSC till Partnercenter efter detta datum.**
> 
> Om det finns avtal som du aktivt arbetar med som innehåller berättigade IP-säljerbjudanden har du två alternativ:
> 
> 1. Markera avtalet som vunnit och slutför avtalsregistreringen i PSC före den 31 mars 2021.
> 2. [Migrera erbjudandena](psc-to-pc.md#psc-deals-migration) till Partnercenter så att du får mer tid att arbeta med avtalet och starta avtalsregistreringen.

Även om ditt företag förlorar åtkomst till PSC efter den 30 april 2021 hittar du fortfarande allt du vill göra i Partner Center, till exempel att skapa samförsäljningserbjudanden, hantera dina avtal och agera på avtal som skickas till dig av Microsoft-säljare.

Det kommer dock att finnas skillnader. Följande riktlinjer kan hjälpa dig att göra övergången till Partnercenter smidigare och enklare.

## <a name="things-to-know-before-moving"></a>Saker att känna till innan du flyttar

### <a name="if-you-are-a-psc-admin"></a>Om du är PSC-administratör

- Du behöver ett e-postmeddelande för arbetet för att logga in [på Partnercenter.](https://partner.microsoft.com/)
- Konfigurera ditt konto med hjälp av kontoadministratören [i Partnercenter.](permissions-overview.md)
- Lär dig hur du säljs samförsäljning i Partnercenter genom att läsa det här dokumentet.
- Konfigurera användarkonton i Partnercenter för alla dina PSC-användare (administratörs-, avtalshanterare- och säljarroller) och tilldela dem [referensadministratörsroller.](permissions-overview.md)

>[!IMPORTANT]
> Kontrollera att det Microsoft Partner Network (MPN) ID som visas i PSC-banderollen är tillgängligt i listan över MPN-platser i Partnercenter.

:::image type="content" source="images/pscmigration/mpnidcheck.png" alt-text="Bild som visar PSC-banderollen där partner kan hitta MPN-ID:t.":::

 Kontrollera att MPN-ID:t visas som en MPN-plats i Partnercenter genom att logga in på instrumentpanelen i [Partnercenter](https://partner.microsoft.com/dashboard)och sedan välja **Inställningar** (kugghjulsikonen) längst upp till höger på skärmen, följt av **Konto Inställningar**. I den vänstra navigeringsmenyn på  den andra nivån väljer du Platser för att se listan över alla MPN-ID:er och platser som är associerade med Partnercenter-kontot.

### <a name="if-you-are-a-psc-deal-manager-or-seller"></a>Om du är PSC-avtalsansvarig eller säljare

- Du behöver ett e-postmeddelande för arbetet för att logga in på instrumentpanelen i [Partnercenter.](https://partner.microsoft.com/dashboard)
- Om du använder ett icke-arbetskonto i PSC, eller om din e-postadress till arbetet är för ett annat företag än partnerföretaget, kontaktar du PSC-administratören för att få hjälp med att konfigurera kontot.
- Kontakta PSC-administratören om ditt partnercenterkonto har ställts in, oavsett vilket konto du använder för att logga in på PSC.
- Kontrollera om du har åtkomst till Partnercenter och avsnittet Referenser.
- Läs det här dokumentet för att förstå arbetsflödena och ändringarna i Partnercenter.

## <a name="as-an-admin-in-psc-these-are-your-next-steps"></a>Som administratör i PSC är det här nästa steg

I den vänstra navigeringsmenyn i Partnercenter väljer **du alternativet Referenser.** Bekräfta att du kan komma åt referenssidorna.

  >[!Note]
  > Du kan behöva logga ut från Partnercenter och logga in igen för att uppdatera dina autentiseringsuppgifter för åtkomst till referenssidorna.

Om du inte ser alternativet Referenser på Partnercenter-menyn eller hänvisningsrelaterade sidor [](permissions-overview.md) kontaktar du företagets kontoadministratör och  ber dem ge dig åtkomst till alternativet Referenser och relaterat område. 

Så här hittar du företagets kontoadministratör:

1. Välj **Kontoinställningar** från kugghjulsikonen längst upp till höger på instrumentpanelen i Partnercenter.

1. Välj **Användarhantering** på den vänstra navigeringsmenyn på den andra nivån.

1. Längst upp i användarlistan väljer du **listrutan** Filter. Ändra alternativet till **Kontoadministratör.**

   Sidan visar alla kontoadministratörer med sina respektive e-postadresser. Skicka ett e-postmeddelande till en av dem och be dem att tilldela referensadministratörsrollen för ditt arbetskonto.

  :::image type="content" source="images/pscmigration/account-admin.gif" alt-text="Bild som visar kontoadministratörerna på användarhanteringssidan för partnerinställningar.":::

>[!Important]
>- Om din roll endast omfattar hantering av användare i PSC ber du företagets kontoadministratör att tilldela dig [kontoadministratörsrollen](permissions-overview.md#manage-mpn-membership-and-your-company) i Partnercenter. 
>- Om din roll även omfattar hantering av möjligheter till säljförsäljning ber du om att [tilldelas administratörsrollen för hänvisningar.](permissions-overview.md#manage-referrals)
> - Det är en bra idé att även nominera en ändringshanteringsledning bland PSC-administratörerna. Detta förhindrar att alla PSC-administratörer behöver kontakta partnercenterkontoadministratörer individuellt. Ändringshanteringsledningen kan i stället vara den primära personen som arbetar med kontoadministratören i Partnercenter.

## <a name="user-migration"></a>Användarmigrering

När du har ställt in ditt konto i Partnercenter använder du guiden för användarmigrering på sidan möjligheter till säljförsäljning för att automatiskt tilldela Partnercenter-roller till anställda i företaget.

>[!Note]
> Användarmigrering kan bara utföras [av kontoadministratörer](permissions-overview.md#manage-mpn-membership-and-your-company) för ditt företag. Om du inte har rollen som kontoadministratör hittar du en kontoadministratör som kan hjälpa dig att konfigurera användarkontona med hjälp av guiden för användarmigrering.

:::image type="content" source="images/pscmigration/user-migration.gif" alt-text="Bild som visar guiden för användarmigrering.":::

Kontoadministratörer ser en länk i guiden för PSC-användarmigrering på sidan möjligheter till säljförsäljning bredvid referensguiden. De kan initiera användarmigrering genom att välja länken. Administratörer kan välja länken för att initiera användarmigrering. De kan utföra det här användarmigreringssteget flera gånger tills alla användare har tilldelats rätt roller i Partnercenter.

Tabellen för användarmigrering innehåller följande information:

- Användarkonto – Medarbetarens e-post-ID
- PSC-partnerkonto – Det konto som medarbetaren är associerad med i PSC
- PSC-användarroll – en av de tre rollerna som tilldelats i PSC.
- PLATS för DATOR-MPN – Den plats där användaren får relevanta Roller i Partnercenter (PC). MPN för PSC-partnerkontot används för att hitta motsvarande MPN-plats i Partnercenter för att tilldela behörigheter. Hela organisationen anger DET virtuella MPN-ID:t.
- Datoranvändarroll – Anställda tilldelas roller baserat på sina PSC-användarroller. Administratören i PSC tilldelas referensadministratörsroller i Partnercenter. Säljaren tilldelas användarrollen referenser i Partnercenter. Läs mer om Partnercenter-roller och vad användare med dessa roller kan göra i Partnercenter i avsnittet Hantera referenser i Tilldela användarroller och behörigheter för ett företags användare som behöver arbeta i [Partnercenter.](permissions-overview.md#manage-referrals)
- PC AAD-klient – den Microsoft Azure Active Directory (Azure AD)-klient som användarna är tilldelade till i Partnercenter
- Status – Det finns tre möjliga tillstånd för migreringens status
    - **Inte migrerad** – användaren har inte tilldelats någon referensroll i Partnercenter
    - **Migrerad** – Användaren har migrerats med relevant roll tilldelad enligt tabellen
    - **Fel** – Det gick inte att slutföra migreringen på grund av ett fel

Ibland kan migreringen misslyckas och resultera i fel. Här är några orsaker till varför en migrering kan orsaka ett fel och några av sätten att lösa problemet:

1. PSC-användare kan använda ett icke-arbetskonto.

2. PSC-användaren kanske använder ett konto från en annan domän än den du använder i Partnercenter.

   För att lösa fel som rör scenarier 1 och 2 ber du användaren att logga in på Partnercenter med sitt arbetskonto som är kopplat till din Azure AD-klientorganisation. Din [globala administratör](permissions-overview.md#manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles) kan vara till hjälp.
   
   Så här hittar du din globala administratör: 
   - Logga in på [instrumentpanelen i Partnercenter](https://partner.microsoft.com/dashboard) och **välj Kontoinställningar** från kugghjulsikonen längst upp till höger.
   - Välj **Användarhantering** i det vänstra navigeringsfältet på den andra nivån.
   - Längst upp i användarlistan väljer du **listrutan Filter** och ändrar alternativet till **Global administratör.** Sidan visar sedan alla globala administratörer med sina respektive e-postadresser. Be en av dem att tilldela referensadministratörsrollen för ditt arbetskonto.
   
      Den globala administratören kan antingen skapa ett nytt användarkonto i din Azure AD-klientorganisation eller tilldela gästanvändaråtkomst till de andra domänkontoanvändarna. När kontona har ställts in för alla PSC-avtalshanterare och -användare måste de logga in på Partnercenter, välja Referenser på den vänstra **navigeringsmenyn** och bekräfta att de kan se sidan Referenser.

3. Användaren har redan en referensroll tilldelad i Partnercenter.
    - Du kan verifiera användarens befintliga roll. I det övre högra hörnet i Partnercenter väljer **du Inställningar** (kugghjulsikonen) och sedan **Kontoinställningar**. När du ser en andra vänster navigeringsmeny väljer **du Användarhantering** och söker efter användaren.

## <a name="psc-deals-migration"></a>Migrering av PSC-avtal

När du har slutfört användarmigrering använder du avtalsmigreringsguiden på sidan möjligheter till säljförsäljning för att hämta alla berättigade öppna avtal från PSC till Partnercenter. **Migreringslänken visas bara för referensadministratörer med hela organisationens omfång i Partnercenter.** Länken för **PSC-avtalsmigrering** visas längst upp till höger på sidan med möjligheter till säljsamarbete och öppnar avtalsmigreringsguiden.

Läs det här avsnittet innan du påbörjar avtalsmigrering.

**Berättigad till migrering**

Endast vissa avtal är berättigade till migrering från PSC till Partnercenter. Den här migreringsguiden är skapad för att hjälpa partner att få sina avtal till Partnercenter där de fortfarande arbetar aktivt med sina kunder för att stänga avtalet. **Endast avtal i öppet tillstånd som skapats från 1 januari 2020 med giltig partnerkontoinformation (giltigt MPN-ID) och som inte genomgår avtalsregistrering är berättigade till migrering.**

**Inte berättigad till migrering**

- Lösningsutvärderingsavtal är inte berättigade till avtalsmigrering
- OEM-licensieringsaffärsavtal är inte berättigade till avtalsmigrering
- Avtal som har markerats som vann i PSC är inte berättigade till migrering. Avtalsregistrering om det är berättigat till de avtal som markerats som won ska slutföras i PSC.

## <a name="pre-requisites-for-deal-migration"></a>Förutsättningar för avtalsmigrering

Innan du påbörjar avtalsmigrering från Partnercenter följer du anvisningarna nedan för att konfigurera avtal i PSC för en lyckad migrering.

1. Alla medlemmar i säljteamet i företaget som arbetar med öppna avtal informeras om migreringen.
2. Säljteamets medlemmar tränas att använda Partnercenter för avtalshantering.
3. Avtal har all nödvändig information enligt beskrivningen nedan.
    - Kundens företagsinformation, inklusive namn och adress
    - Kundens kontaktuppgifter om det är ett samförsäljningsavtal
    - Minst en lösning
    - Minst en teammedlem med all information – förnamn, efternamn, e-post-ID och telefonnummer
    - Avtalsvärde
    - Beräknat avtalsdatum
    - Partneranteckningar

Du kan använda funktionerna för massnedladdning och uppladdning i PSC för att lägga till all information som saknas i avtalet för alla berättigade avtal.

>[!Note]
> Avtalsmigrering lyckas även om ovanstående krav inte uppfylls. Men du kan inte ändra tillståndet för avtalet om något av ovanstående obligatoriska fält i Partnercenter inte är tillgängligt. Du måste sedan ange all nödvändig information som saknas i avtal i Partnercenter för att börja arbeta med dem. **Vi rekommenderar starkt att du rensar kvalificerande avtal i PSC innan du migrerar dem till Partnercenter.**

Avtalsmigrering i Partnercenter har skapats med ett klick. Allt du behöver göra är att välja **knappen "Migrera avtal"** när ditt företag är redo att migrera de berättigade erbjudandena. **Du kan inte välja de avtal som du vill migrera från PSC. Om du inte vill migrera några avtal till Partnercenter flyttar du dem till stängt tillstånd i PSC innan du påbörjar migreringen.**

>[!Note]
> När du har initierat **migreringen kan det ta upp till 24 timmar innan avtal migreras**.

När migreringen är klar ändras banderollmeddelandets status för att slutföras med en länk till migreringsrapporten. Ladda ned rapporten för att visa information om avtal som har migrerats från PSC till Partnercenter.

Rapporten innehåller informationen nedan.

1. **Engagemangs-ID för Partnercenter** – Den unika identifieraren i Partnercenter för alla avtal i ett engagemang. Det finns två avtal – ett för partnern och ett för Microsoft i ett engagemang för säljförsäljning i Partnercenter.
2. **Referens-ID för Partnercenter** – Den unika identifieraren i Partnercenter för avtalet som tillhör partnern.
3. **Avtalsnamn** – Identifierare som anges för avtalet i PSC.
4. **PSC-avtals-ID** – Den unika identifieraren i PSC för avtalet.
5. **Fel –** för att ange om det finns några fel vid migrering av ett specifikt avtal.

Alla avtal som har migrerats visas inte i PSC. Du kan fortsätta att arbeta med migrerade avtal i Partnercenter, inklusive slutföra avtalsregistrering i Partnercenter. Det kommer inte att ske några ändringar i interaktionerna med Microsoft-säljarna för säljavtal.

Avtal som migreras från PSC kommer att vara tillgängliga på flikarna Inkommande och Utgående baserat på avtalets källa. Alla avtal som delas av ditt företag kommer att vara tillgängliga på fliken Utgående och Microsoft-initierade avtal kommer att vara tillgängliga på fliken Inkommande i Partnercenter. Det kommer att finnas två typer av avtal som skapas efter migreringen.

1. **Säljavtal –** Avtal som markeras som samförsäljning i PSC skapas som samförsäljningserbjudanden i Partnercenter.
2. **Partnerledda avtal** – Avtal som inte har markerats som samförsäljning skapas som partnerledda avtal i Partnercenter. Partnerledda avtal är synliga för Microsoft-säljare och kan uppgraderas till säljavtal innan de når terminaltillståndet (won, lost). Dessutom är partnerledda avtal berättigade till avtalsregistrering om det finns en berättigad incitamentslösning i avtalet.

>[!Important]
> Om det finns fel som gör att vissa avtal inte kunde migreras kan du initiera om avtalsmigrering genom att klicka på knappen **"Migrera avtal".** Det aktiveras bara om det finns vissa berättigade avtal som ännu inte har migrerats. Detta är också användbart om du befinner dig i övergångsfasen där vissa nya avtal skapas i PSC efter att du har initierat avtalsmigrering.

När alla avtal har migrerats visas en banderoll som visar "Inga avtal **att migrera"** med knappen **"Migrera avtal"** **inaktiverad.**

När du har slutfört användarmigrering och/eller avtalsmigrering kan du använda följande vägledning för att bestämma migreringsstrategin:

Om ditt företag har en Partner Development Manager (PDM) – När ditt Partnercenter-konto har ställts in och dina användare har flyttats över och har roller och behörigheter kan du flytta dina säljaktiviteter till Partnercenter. Informera PDM om att göra övergången i stället för att vänta tills migreringen har slutförts, vilket gör att alla dina nya avtal kan flöda till Partnercenter.

>[!Note]
>När du har gjort den här växlingen kan du bara agera på befintliga aktiva avtal i PSC. Du kan varken skapa nya avtal eller få avtal från Microsoft-säljare i PSC.

Om ditt företag inte har någon PDM – Kontrollera att alla användarkonton har ställts in och verifierats av alla användare. Du får ett meddelande via e-post och en banderoll i PSC om det exakta datumet då du kan börja samförsäljning i Partnercenter. Kom ihåg att du fortfarande måste hantera befintliga aktiva avtal i PSC.

>[!Important]
> Du har fram till den 30 april 2021 på dig att registrera de avtal som markeras som vann.

## <a name="next-steps-for-psc-admins-psc-deal-managers-and-psc-sellers"></a>Nästa steg för PSC-administratörer, PSC-avtalshanterare och PSC-säljare

Lär dig hur du säljs samförsäljning i Partnercenter.
Det här är ett viktigt steg som hjälper dig att förbereda dig för samförsäljning i Partnercenter. Förstå arbetsflödena och ändringarna i Partnercenter så att du effektivt kan samarbeta direkt. Börja med att läsa det här dokumentet helt. En bra uppsättning resurser finns också i galleriet [Sälj säljupplevelse.](https://aka.ms/cosellexperience)

## <a name="major-differences-between-psc-and-partner-center-workflows"></a>Större skillnader mellan PSC- och Partner Center-arbetsflöden

|**Scenario**|**Partnerförsäljnings-Anslut**|**Partnercenter**|
|-----|:-----|:-----|
|Användarroller|PSC har administratörs-, avtalshanterare- och säljarroller.|Partnercenter har endast [administratörsrollen](permissions-overview.md#manage-referrals) hänvisning som ger både läs- och skrivbehörighet för alla avtal.|
|Bjuda in Microsoft på ett samförsäljningsavtal|Det finns ingen uttrycklig fråga från partnern som initierats av Microsoft-säljaren.|Partnern måste göra en [explicit begäran om](manage-co-sell-opportunities.md#add-solutions) en Microsoft-säljhjälp krävs för ett avtal. Microsoft-säljaren har ett alternativ för att neka begäran.|
|Upphörande|Det finns inget begrepp om att ett avtal upphör att gälla.|Partnerns inkommande avtal går ut om 14 dagar om de inte godkänns av partnern. Samma sak gäller för partnerns utgående avtal där de kan gå in i ett utgånget tillstånd om Microsoft-säljaren inte agerar på dem på 14 dagar.|
|Microsofts säljarinformation|Synligt så fort ett avtal skapas.|Microsofts säljarinformation delas endast med partner om säljaren uttryckligen godkänner inbjudan till säljpartner.|
|[Privat pipeline](manage-co-sell-opportunities.md#types-of-co-sell-opportunities)|Inte tillgängligt.|Partner kan dela sin pipeline utan att ge insyn till Microsofts säljare.|
|Lösningar|Lösningar som endast tillhör en prislista kan läggas till i ett avtal.|Partner kan lägga [till](manage-co-sell-opportunities.md#add-solutions) lösningar som tillhör följande listor. a) Deras egna lösningar b) Lösningar från Microsofts katalog från första part (liknar rollen Transaktionsavtal i PSC) och c) Säljavtalslösningar från andra tredjepartspartner (liknar ISV-avtalsrollen i PSC).|
|Avtalstilldelning|Endast en tilldelad säljare kan visa och agera på affärerna.|Gruppmedlemmar kan läggas till i ett avtal för att ange vilka personer som arbetar med ett avtal, det finns ingen blockering av andra hänvisningsadministratörer från att visa eller agera på dessa avtal.|
|Kundorganisation|Fritextpost.|Du kan söka i [kundorganisationen](manage-co-sell-opportunities.md#select-your-customer) mot [D-&B-databasen](https://www.dnb.com/) genom att bara skriva några tecken. Det juridiska namnet och adressen fylls i automatiskt baserat på valet.|
|Kundkontakt|Inte obligatoriskt.|Inte obligatoriskt för delning av privata pipelines. Krävs om Microsoft-säljare bjuds in att delta i en begäran om säljförsäljning.|
|Offentligt API|Inte tillgängligt.|[Offentligt API](/partner/develop/referrals) för att programmatiskt hantera partnercenterreferenser.|

## <a name="map-the-fields-in-psc-to-the-corresponding-fields-in-partner-center"></a>Mappa fälten i PSC till motsvarande fält i Partnercenter

I det här avsnittet jämförs (eller "kartor") valda skärmbilder som visas för PSC med motsvarande vy i avsnittet Möjligheter till samförsäljning i Partnercenter.

Du ser numrerade, gula eller röda cirklar på varje par av skärmbilder:

- **Vad betyder gula cirklar?** Numrerade gula cirklar visas först på varje PSC-skärmbild. Du hittar sedan en tillhörande Partnercenter-skärmbild under den med många av samma siffror.

   Om du vill se hur varje fält eller attribut i PSC mappar till sin motsvarighet i Partnercenter, matchar du de numrerade cirklarna tillsammans i de två relaterade skärmbilderna. Matcha till exempel den numrerade, gula "1" i den första PSC-skärmbilden med den numrerade, gula "1" i den andra, partnercenter-skärmbilden nedanför.

- **Vad betyder en röd cirkel?** Om du ser en röd cirkel på en skärmbild innebär det att PSC-fältet inte är tillgängligt i Partnercenter.

Fältmappningar för PSC-till-Partner Center visas för följande områden:

1. PSC-startsida mappad till standardvyn för möjligheter till säljförsäljning i Partnercenter
1. PSC-rutnätsvy mappad till partnercenter-avtalsvyn
1. Vy över PSC-avtalsinformation som är mappad till partnercenter-avtalsinformationsvyn
1. PSC-vyn Lägg till produkter mappad till vyn Lägg till lösningar i Partnercenter
1. PSC-användarhanteringsvy mappad till användarhanteringsvyn i Partnercenter
1. Vy för PSC-användarrolltilldelning mappad till vyn För Partnercenter-rolltilldelning
1. Vy för PSC-meddelanden som är mappad till meddelandevyn i Partnercenter

### <a name="1---psc-home-page-mapped-to-the-partner-center-co-sell-opportunities-default-view"></a>1 – PSC-startsidan mappas till standardvyn för möjligheter till säljförsäljning i Partnercenter

Jämför matchande numrerade cirklar mellan den översta PSC-skärmbilden och Partnercenter-skärmbilden under den. Matchande tal visar var du hittar den PSC-relaterade funktionen eller attributet i Partnercenter. Röda cirklar visar att det inte finns något matchande Partnercenter-fält.  

:::image type="content" source="images/pscmigration/homepage.png" alt-text="Bild som visar fältmappningarna mellan startsidan för Partner Sales Anslut och standardvyn för Möjligheter till säljpartner i Partnercenter." lightbox="images/pscmigration/home-page-expanded.png":::

### <a name="2---psc-grid-view-mapped-to-the-partner-center-deal-view"></a>2 – PSC-rutnätsvy mappad till partnercenter-avtalsvyn

Jämför matchande numrerade cirklar mellan den översta PSC-skärmbilden och Partnercenter-skärmbilden under den. Matchande tal visar var du hittar den PSC-relaterade funktionen eller attributet i Partnercenter. Röda cirklar visar att det inte finns något matchande Partnercenter-fält.  

> [!NOTE]
> Andra överväganden visas under skärmbilderna.

:::image type="content" source="images/pscmigration/gridview.png" alt-text="Bild som visar fältmappningarna mellan rutnätsvyn Partner sales Anslut (PSC) och vyn Partnercenter-avtal." lightbox="images/pscmigration/grid-view-expanded.png":::

**Särskilda överväganden:**

- Det finns ingen listvy i Partnercenter som för PSC.  Alla avtal visas baserat på det senaste mottagna eller skapade datumet med kundinformationen och typen av avtal. Det första avtalet i vyn är valt som standard. De flesta av de värden som visas i PSC-tabellformatet är tillgängliga i detaljvyn för avtalet i Partnercenter.
- Avtalsrollen är inte ett obligatoriskt fält i Partnercenter. Den visas eller avbildas inte i något av arbetsflödena. Den härleds automatiskt på Microsofts säljarsida baserat på de lösningar som lagts till i avtalet.
- Datumet för senaste ändring visas inte på sidan med hänvisningsinformation i Partnercenter. Partner kan använda sorteringsfunktionen för att sortera avtal baserat på datum för senaste uppdatering.

### <a name="3---psc-deal-details-view-mapped-to-partner-center"></a>3 – Informationsvy för PSC-avtal mappad till Partnercenter

Jämför den matchande, numrerade cirklarna längst upp (PSC)-skärmbilden med Partnercenter-skärmbilden nedanför. Matchande tal visar var du hittar den PSC-relaterade funktionen eller attributet i Partnercenter. Röda cirklar visar att det inte finns något matchande fält eller område i Partnercenter.

> [!NOTE]
> Andra överväganden visas under skärmbilderna.

:::image type="content" source="images/pscmigration/dealdetails.png" alt-text="Bild som visar fältmappningarna mellan vyn partnerförsäljnings- Anslut (PSC)-avtalsinformation och vyn Partnercenter-avtalsinformation." lightbox="images/pscmigration/deal-details-expanded.png":::

**Särskilda överväganden:**

- Partner kan redigera ett avtal genom att välja redigeringsknappen i detaljvyn för partneravtal (6). När redigeringsknappen har valts blir alla fält redigerbara. Sedan kan du välja att antingen spara eller avbryta de ändringar som gjorts i avtalet.
- Det finns inget alternativ för att stänga avtalet som en dubblett i Partnercenter.
- Kundresultat är inte tillgängligt i Partnercenter. All information som rör kundinteraktioner kan uppdateras i avsnittet Anteckningar i Partnercenter.
- Beräknat lösningsslutdatum är endast tillgängligt för OEM IOT-avtal i Partnercenter. Den här informationen visas inte för andra avtalstyper.
- Licensieringsprogram krävs inte i Partnercenter. Den här informationen härförs automatiskt baserat på de lösningar som valts i avtalet.

>[!Note]
>Ett avtal som markerats som won eller lost (förlorat) kan inte redigeras efteråt. Var försiktig när du flyttar ett avtal till något av dessa terminaler.

### <a name="4---psc-add-products-view-mapped-to-the-partner-center-add-solutions-view"></a>4 – PSC-vyn "Lägg till produkter" mappad till vyn Lägg till lösningar i Partnercenter

Jämför den matchande, numrerade cirklarna längst upp (PSC)-skärmbilden med Partnercenter-skärmbilden nedanför. Matchande tal visar var du hittar den PSC-relaterade funktionen eller attributet i Partnercenter. Röda cirklar visar att det inte finns något matchande fält eller område i Partnercenter.
  
:::image type="content" source="images/pscmigration/products.png" alt-text="Bild som visar fältmappningarna mellan vyn Partner sales Anslut (PSC) lägga till produkter och vyn Lägg till lösningar i Partnercenter." lightbox="images/pscmigration/products-expanded.png":::

### <a name="5---user-management-in-psc-versus-partner-center"></a>5 – Användarhantering i PSC jämfört med Partnercenter

Jämför den matchande, numrerade cirklarna längst upp (PSC)-skärmbilden med Partnercenter-skärmbilden nedanför. Matchande tal visar var du hittar den PSC-relaterade funktionen eller attributet i Partnercenter. Röda cirklar visar att det inte finns något matchande fält eller område i Partnercenter.  

 :::image type="content" source="images/pscmigration/usermanagement.png" alt-text="Bild som visar fältmappningarna mellan användarhanteringsplatsen Anslut partnerförsäljning (PSC) och användarhanteringssidan i området Kontoinställningar i Partnercenter."  lightbox="images/pscmigration/user-management-expanded.png":::

### <a name="6---user-role-assignment-in-psc-versus-partner-center"></a>6 – Tilldelning av användarroller i PSC jämfört med Partnercenter

Jämför den matchande, numrerade cirklarna längst upp (PSC)-skärmbilden med Partnercenter-skärmbilden nedanför. Matchande tal visar var du hittar den PSC-relaterade funktionen eller attributet i Partnercenter. Röda cirklar visar att det inte finns något matchande fält eller område i Partnercenter.  

:::image type="content" source="images/pscmigration/roles.png" alt-text="Bild som visar fältmappningarna mellan rolltilldelningsvyn Anslut partnerförsäljning (PSC) och rolltilldelningsvyn i Partnercenter." lightbox="images/pscmigration/roles-expanded.png":::

**Särskilda överväganden:**

- Motsvarande roll för PSC-administratören är kontoadministratörsrollen i Partnercenter.
- Det finns bara en roll i Partnercenter för hantering av säljavtal. Den här rollen är referensadministratörsrollen.

### <a name="7---notifications-in-psc-versus-partner-center"></a>7 – Meddelanden i PSC jämfört med Partnercenter

Jämför den matchande, numrerade cirklarna längst upp (PSC)-skärmbilden med Partnercenter-skärmbilden nedanför. Matchande tal visar var du hittar den PSC-relaterade funktionen eller attributet i Partnercenter. Röda cirklar visar att det inte finns något matchande fält eller område i Partnercenter.  

:::image type="content" source="images/pscmigration/notifications.png" alt-text="Bild som visar mappningen mellan PSC-meddelanden (Partner Sales Anslut) och meddelandevyn i Partnercenter."  lightbox="images/pscmigration/notifications-expanded.png":::

## <a name="moving-from-psc-to-partner-center---frequently-asked-questions"></a>Flytta från PSC till Partnercenter – vanliga frågor och svar

Följande avsnitt besvarar vanliga frågor om migreringen.

### <a name="1---what-should-i-do-if-i-dont-have-access-to-partner-center"></a>1 – Vad ska jag göra om jag inte har åtkomst till Partnercenter?

Du kan kontakta dina administratörer på sidan "Ingen åtkomst" för att få rollerna tilldelade. Du behöver [referensadministratörsrollen](permissions-overview.md#manage-referrals) för läs- och skrivbehörighet under referensavsnittet. Om du bara hanterar företagsprofiler behöver du rollen som företagsprofiladministratör i Partnercenter.

:::image type="content" source="images/pscmigration/noaccess.png" alt-text="Bild som visar ingen åtkomstupplevelse i Partnercenter.":::

### <a name="2---who-can-grant-me-access-to-the-referrals-section-in-partner-center"></a>2 – Vem kan ge mig åtkomst till avsnittet Referenser i Partnercenter?

[Kontoadministratören](permissions-overview.md#manage-mpn-membership-and-your-company) kan ge dig åtkomst till fliken Referenser. Du hittar kontoadministratören genom att **välja Kontoinställningar** från kugghjulsikonen längst upp till höger på instrumentpanelen i [Partnercenter.](https://partner.microsoft.com/dashboard) Välj sedan **Användarhantering i** det vänstra navigeringsfältet på den andra nivån. Längst upp i användarlistan väljer du **listrutan Filter** och ändrar alternativet till **kontoadministratör.** Sidan visar alla kontoadministratörer med sina respektive e-postadresser. Be en av dem att tilldela referensadministratörsrollen för ditt arbetskonto.

### <a name="3---the-new-deal-button-is-greyed-out-for-our-account-what-should-i-do-to-start-creating-deals"></a>3 – Knappen +nytt avtal är nedtonad för vårt konto. Vad ska jag göra för att börja skapa avtal?

Detta inträffar bara om det inte finns några lösningar för säljförsäljning som är kopplade till DEN MPN-organisation som du använder i Partnercenter. Kontakta PDM för att få MPN-ID:t för dina lösningar korrigerade eller skapa ett support ärende som nämner problemet "Knappen Nytt avtal är nedtonat efter PSC-migreringen".

### <a name="4---can-i-assign-deals-to-a-specific-person-from-our-organization-like-psc"></a>4 – Kan jag tilldela avtal till en viss person från vår organisation som PSC?

Du kan tilldela teammedlemmar till ett visst avtal. Det blockerar inte andra hänvisningsadministratörer från att visa eller agera på dessa avtal.

### <a name="5---is-there-a-view-of-all-the-deals-assigned-to-me"></a>5 – Finns det någon vy över alla avtal som tilldelats mig?

Du kan använda funktionen Favoriter, som är en flik på användarnivå. Du kan markera alla avtal som har tilldelats dig som favoriter för att få en snabb åtkomst till erbjudandena.

### <a name="6---is-there-a-read-only-view-for-the-deals"></a>6 – Finns det en skrivskyddade vy för avtal?

Nej, det finns ingen skrivskyddade vy över avtal i referensavsnittet. Alla referensadministratörer har fullständig läs- och skrivåtkomst till alla avtal.

### <a name="7---how-can-i-register-a-deal-after-marking-it-as-won"></a>7 – Hur kan jag registrera ett avtal när jag har märkt det som vunnit?

Om avtalet uppfyller villkoren nedan visas ett popup-fönster för att starta [avtalsregistreringen.](./register-deals.md)

- Det finns en berättigad incitamentslösning kopplad till avtalet.
- Microsofts säljare bjuds in att delta i avtalet, eller så har de bjudit in dig till avtalet.
- Microsoft-kortet har statusen Godkänt eller Vunnit i Partnercenter.

### <a name="8---i-get-an-error-message-when-i-select-the-new-deal-registration-button-in-the-deal-registration-section-how-can-i-register-my-deals"></a>8 – Jag får ett felmeddelande när jag väljer knappen "+Ny avtalsregistrering" i avsnittet Avtalsregistrering. Hur registrerar jag mina avtal?

Knappen **+Ny avtalsregistrering** ska endast användas av partner som är registrerade i ISV-anslutningsprogrammet för att registrera ett avtal utan motsvarande möjligheter till säljförsäljning i Partnercenter. För registrering av avtal med en möjlighet till säljförsäljning visas ett popup-fönster när avtalet markeras som won (vunnit) och om det uppfyller villkoren för avtalsregistrering.

### <a name="9---is-adding-a-customer-organization-mandatory"></a>9 – Är det obligatoriskt att lägga till en kundorganisation?

Ja, det är [obligatoriskt att lägga](./manage-co-sell-opportunities.md#select-your-customer) till en kundorganisation i Partnercenter. Börja med att söka efter den plats där kunden befinner sig. Baserat på den information som du har; du kan vara specifik, inklusive det exakta byggnamnet eller bara ge information om staden. Organisationssökningen hämtar alla juridiska personer som matchar det namn som du anger så att du inte behöver ange någon adressinformation. All information fylls i automatiskt baserat på den valda organisationen.

### <a name="10---are-customer-contact-details-mandatory"></a>10 – Är kundens kontaktuppgifter obligatoriska?

Beror på [vilken typ av avtal](./manage-co-sell-opportunities.md#types-of-co-sell-opportunities) du skapar. Om du bara delar din pipeline och inte behöver hjälp från Microsofts säljorganisation kan du välja att inte ge kunden kontaktinformation. Om du samförsäljningar där du aktivt söker hjälp från Microsoft-säljare måste du ange kundens kontaktuppgifter. Du bör få ett uttryckligt medgivande från kunden innan du skapar en begäran om säljförsäljning i Partnercenter.

### <a name="11---how-many-solutions-can-i-add-to-a-deal"></a>11 – Hur många lösningar kan jag lägga till i ett avtal?

Du kan lägga till upp till 50 lösningar (detsamma som "produkter" i PSC) till ett avtal. Till skillnad från PSC kan du blanda lösningar från dina egna berättigade lösningar för säljförsäljning, SKU:er från Microsofts första part och andra lösningar som är berättigade till säljförsäljning från tredje part. Det finns ingen avtalsroll som ska väljas eller vara tillgänglig i Partnercenter. För Microsoft-SKU:er kan du välja att lägga till kvantitet och pris för varje SKU som läggs till i avtalet.

### <a name="12---when-will-i-get-to-know-the-microsoft-seller-details-after-creating-a-deal"></a>12 – När får jag information om Microsofts säljare när jag har skapat ett avtal?

Microsoft-säljare tilldelas först efter att ha matchat det exakta hjälpkrav som angavs när avtalet med relevant säljare på Microsoft-sidan har förhandlats. Även efter tilldelningen har Microsoft-säljare möjlighet att antingen godkänna eller avvisa inbjudan till säljinbjudan. Endast om en säljinbjudan godkänns av en säljare, uppdateras avtalet med Microsofts kontaktuppgifter för försäljning. SLA för Microsoft-säljare att agera på avtalet är 14 dagar. Det är samma serviceavtal som partner måste agera på avtalet innan det förfaller.

### <a name="13---where-can-i-find-the-opportunity-id"></a>13 – Var hittar jag affärsmöjlighets-ID:t?

Affärsmöjlighets-ID i PSC är samma som avtals-ID:t i Partnercenter. Du hittar avtals-ID:t bredvid avtalsnamnet när du öppnar ett avtal.

### <a name="14---how-can-my-pdm-get-access-to-partner-center"></a>14 – Hur får min PDM åtkomst till Partnercenter?

Partnercenter kan inte nås av dina PDU:er direkt till skillnad från PSC. Det finns flera alternativ för att aktivera den funktionen, som anges nedan.

- OCP Insights – Om PDM bara visar de avtal och framsteg som rör dem kan de använda OCP-portalen (One Commercial Partner) Insights för att få din organisationsvy. Det här är ett internt verktyg som endast är tillgängligt för PDM. OCP-insikter är inte tillgängliga för företagets användare.
- Gästanvändare i Partnercenter – Du kan lägga till ditt PDM-konto som gästanvändare i Partnercenter och tilldela referensadministratörsrollen till dem så att de kan visa och agera @microsoft.com på hänvisningar.
- Skapa en [ny användare](./create-user-accounts-and-set-permissions.md#add-a-new-user) i din klientorganisation – Du kan skapa en ny användare i din egen klientorganisation och dela informationen med PDM så att de kan visa och agera på hänvisningar som liknar andra hänvisningsanvändare i ditt konto.

## <a name="finding-the-correct-mpn-id-if-your-account-in-psc-is-not-associated-with-a-valid-mpn"></a>Hitta rätt MPN-ID om ditt konto i PSC inte är associerat med ett giltigt MPN

Om du är här eftersom du såg en banderoll i PSC som nämner "PROBLEM med ogiltig MPN-ID-association för PSC" är du på rätt plats. Ditt konto kan ha länkats till ett ogiltigt MPN-ID av följande skäl

- Ditt företag har inget Partnercenter-konto.
- PDM gjorde ett misstag när du skulle ange MPN-ID:t för ditt konto i de interna system som länkar psc-kontot till ditt Partnercenter-konto (MPN-ID).
- Ditt företag slutförde inte migreringen från Partner Membership Center (PMC) till Partnercenter.

Leta först reda på rätt MPN-ID genom att följa stegen nedan.

1. Logga in på ditt [Partnercenter-konto](https://partner.microsoft.com/dashboard).
2. Använd vägledningen i dokumentationen för [kontoinställningar för att](./partner-center-account-setup.md#locate-your-mpn-id) hitta MPN-ID:t.

Nedan visas en skärmbild som visar den exakta platsen där du kan hitta ditt MPN-ID för Partnercenter.

:::image type="content" source="images/pscmigration/finding-mpn-id.png" alt-text="Bild som visar kontoinställningarna där partnern kan hitta sitt MPN-ID."  lightbox="images/pscmigration/finding-mpn-id.png":::

- Om du har en PDM ber du dem att få ditt MPN-ID korrigerat med rätt MPN-ID från ditt Partnercenter-konto.
- Om du inte har en PDM skickar du ett e-postmeddelande till den adress som anges i PSC-banderollen med både psc-kontoinformationen som visas i PSC-banderollen och rätt MPN-ID från ditt Partnercenter-konto.

## <a name="resources-to-help-you-create-and-manage-your-deals-in-partner-center"></a>Resurser som hjälper dig att skapa och hantera dina avtal i Partnercenter

Om du inte redan har läst hjälpavsnitten om säljförsäljning kan följande resurser hjälpa dig att hantera avtal i Partnercenter.

|**Så här gör du**   |**Läs detta**   |
|-----------------------|:-----------------------|
|Förstå flikarna och navigeringen på sidan Möjligheter till säljförsäljning|[Navigera i avsnittet om säljförsäljning](./manage-co-sell-opportunities.md)|
|Välja en kundorganisation från listan D&B |[Välj din kund](./manage-co-sell-opportunities.md#select-your-customer)|
|Ändra fälten i avsnittet med avtalsinformation|[Avtalsinformation](./manage-co-sell-opportunities.md#deal-details)|
|Lägga till dina teammedlemmar i ett avtalsteam|[Lägga till dina anställda](./manage-co-sell-opportunities.md#add-team-members)|
|Svara på ett samförsäljningsavtal|[Hantera säljavtal](./manage-co-sell-opportunities.md#respond-to-a-co-sell-opportunity)
|Registrera avtal som du har vunnit i Partnercenter |[Registrera ett nytt avtal](./register-deals.md)
|Få referensinsikter och ta reda på hur dina hänvisningar fungerar |[Hänvisningsinsikter](./referral-insights.md)
|Skapa och hantera företagsprofil|[Hantera företagsprofil](./create-a-marketing-profile.md)
|Hantera leads för din företagsprofil |[Hantera leads](./manage-leads.md)|

## <a name="next-steps"></a>Nästa steg


- [Arbetsbok för Anslut partnerförsäljning](https://partner.microsoft.com/resources/detail/partner-sales-connect-to-partner-center-transition-workbook-pptx) till Partnercenter – arbetsbok för att justera partnerns försäljningsprocesser och roller med nya försäljningsprocesser via Partnercenter jämfört med Partner sales Anslut.
- [Guide för sälj- och säljpartnercenter](https://partner.microsoft.com/resources/detail/co-sell-operating-model-guide-pptx) – vägledning för att identifiera en driftsmodell via Partnercenter för att hantera leads eller möjligheter till säljförsäljning och registrera avtal.
- [Hänvisningshantering –](https://partner.microsoft.com/resources/detail/referral-management-in-partner-center-pptx) visualiserade stegvisa instruktioner för att hantera leads och möjligheter till säljförsäljning via Partnercenter.
- [Publicera och hantera på den kommersiella](https://partner.microsoft.com/resources/detail/publishing-and-managing-co-sell-offers-in-commercial-marketplace-pptx) marknadsplatsen – visualiserade stegvisa instruktioner för att skapa, hantera och publicera erbjudanden via Partnercenter på den kommersiella marknadsplatsen.
