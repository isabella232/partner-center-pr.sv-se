---
title: Migrering från Partner Sales Anslut (PSC) för IOT-partner
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-referrals
description: Lär dig hur Microsoft IOT-partner kan migrera från Partner Sales Anslut (PSC) till Partnercenter och skapa eller hantera avtal.
author: vikramb
ms.author: vikramb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 07/07/2021
ms.openlocfilehash: 2b05046118c83c0d398272da68054a8a0c9c48e4
ms.sourcegitcommit: 23ba623b50b06c866703fd876f1b40f3a49ce504
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/22/2021
ms.locfileid: "128074639"
---
# <a name="guide-to-create-and-manage-iot-deals-in-partner-center-pc-for-iot-partners-migrating-from-partner-sales-connect-psc"></a>Guide för att skapa och hantera IOT-avtal i Partnercenter (PC) för IOT-partner som migrerar från Partner Sales Anslut (PSC)

**Lämpliga roller:** Kontoadministratörsroller | Referensadministratörsbehörighet | Partner Sales Anslut (PSC)-| Administratörsadministratör Anslut partnerförsäljning (PSC) | Partner Sales Anslut (PSC)-avtalschef

Den här artikeln innehåller vägledning för IOT-partner som migrerar från Partner Sales Anslut (PSC) till Partner Center (PC) så att de kan fortsätta att skapa och hantera avtal i Partnercenter.

>[!Note]
> Den här guiden **gäller endast för IOT-affärspartner som** hanterar sina avtal i PSC.

>[!Important]
> Från och med 15 augusti 2021 kommer ditt företag inte att kunna skapa eller redigera avtal i PSC. **Du kommer fortfarande att kunna ladda ned befintliga avtalsdata med funktionen för massexport i PSC. Du kan också [migrera öppna avtal](partner-sales-connect-to-partner-center-iot.md#psc-deals-migration) från PSC till Partner Center efter detta datum.**

Som du vet **förlorar ditt företag åtkomst till PSC efter den 30 augusti 2021.** Du hittar dock fortfarande allt du vill göra i Partnercenter, till exempel att skapa och hantera avtal.

Det kommer dock att finnas skillnader. Följande riktlinjer kan hjälpa dig att göra övergången till Partnercenter smidigare och enklare.

## <a name="before-you-move-things-you-need-to-know"></a>Innan du flyttar behöver du känna till saker som du behöver känna till

### <a name="if-you-are-a-psc-admin"></a>Om du är PSC-administratör

- Du behöver ett e-postmeddelande för arbetet för att logga in [på Partnercenter.](https://partner.microsoft.com/)
- Konfigurera ditt konto med hjälp av [Partnercenter-kontoadministratören.](permissions-overview.md)
- Lär dig hur du skapar och hanterar IOT-avtal i Partnercenter genom att läsa det här dokumentet.
- Konfigurera användarkonton i Partnercenter för alla dina PSC-användare (administratörs-, avtalshanterare- och säljarroller) och tilldela dem referensadministratörs- eller [referensanvändarroller.](permissions-overview.md)

### <a name="if-you-are-a-psc-deal-manager-or-seller"></a>Om du är PSC-avtalschef eller säljare

- Du behöver ett e-postmeddelande för arbetet för att logga in på instrumentpanelen i [Partnercenter.](https://partner.microsoft.com/dashboard)
- Om du använder ett icke-arbetskonto i PSC, eller om din e-postadress till arbetet gäller ett annat företag än partnerföretaget, kontaktar du PSC-administratören för att få hjälp med att konfigurera kontot.
- Kontakta PSC-administratören om ditt Partnercenter-konto har ställts in, oavsett vilket konto du använder för att logga in på PSC.
- Kontrollera om du har åtkomst till Partnercenter och avsnittet Referenser.
- Läs det här dokumentet för att förstå arbetsflödena och ändringarna i Partnercenter.

## <a name="as-an-admin-in-psc-these-are-your-next-steps"></a>Som administratör i PSC är det här nästa steg

I den vänstra navigeringsmenyn i Partnercenter väljer **du alternativet** Referenser. Bekräfta att du kan komma åt sidan Möjligheter till säljförsäljning.

  >[!Note]
  > Du kan behöva logga ut från Partnercenter och logga in igen för att uppdatera dina autentiseringsuppgifter för åtkomst till referenssidorna.

**Om** du inte ser  alternativet Referenser på Partnercenter-menyn eller referensrelaterade sidor kontaktar [](permissions-overview.md) du ditt företags kontoadministratör och ber dem ge dig åtkomst till alternativet Referenser och det relaterade området.

Så här hittar du ditt företags kontoadministratör:

1. Välj **Kontoinställningar** från kugghjulsikonen längst upp till höger på instrumentpanelen i Partnercenter.

1. Välj **Användarhantering** på den vänstra navigeringsmenyn på den andra nivån.

1. Längst upp i användarlistan väljer du **listrutan** Filter. Ändra alternativet till **Kontoadministratör.**

   Sidan visar alla kontoadministratörer med sina respektive e-postadresser. Skicka ett e-postmeddelande till en av dem och be dem att tilldela referensadministratörsrollen för ditt arbetskonto.

  :::image type="content" source="images/pscmigration/account-admin.gif" alt-text="Bild som visar kontoadministratörerna på sidan för användarhantering i partnerinställningar.":::

>[!Important]
>- Om din roll endast omfattar hantering av användare i PSC ber [](permissions-overview.md#manage-mpn-membership-and-your-company) du företagets kontoadministratör att tilldela dig kontoadministratörsrollen i Partnercenter enligt företagets princip.
>- Om din roll även omfattar hantering av ioT-avtal kan du be att [tilldelas referensadministratören eller referensanvändarrollen](permissions-overview.md#manage-referrals) efter behov.
> - Det är en bra idé att även nominera en ändringshanteringsledning bland PSC-administratörerna. Detta förhindrar att alla PSC-administratörer behöver kontakta partnercenter-kontoadministratörer individuellt. I stället kan ändringshanteringsledningen sedan vara den primära personen som arbetar med kontoadministratören i Partnercenter.

## <a name="user-migration"></a>Användarmigrering

När du har ställt in ditt konto i Partnercenter använder du guiden för användarmigrering på sidan möjligheter till säljförsäljning för att automatiskt tilldela Partnercenter-roller till anställda i ditt företag.

>[!Note]
> Användarmigrering kan bara utföras [av kontoadministratörer](permissions-overview.md#manage-mpn-membership-and-your-company) i ditt företag. Om du inte har rollen som kontoadministratör kan du hitta en kontoadministratör som kan hjälpa dig att konfigurera användarkontona med hjälp av guiden för användarmigrering.

:::image type="content" source="images/pscmigration/user-migration.gif" alt-text="Bild som visar guiden för användarmigrering.":::

Kontoadministratörer ser en länk i guiden för PSC-användarmigrering på sidan möjligheter till säljförsäljning bredvid referensguiden. De kan initiera användarmigrering genom att välja länken. Administratörer kan välja länken för att initiera användarmigrering. De kan utföra det här användarmigreringssteget flera gånger tills alla användare har tilldelats rätt roller i Partnercenter.

Tabellen för användarmigrering innehåller följande information:

- Användarkonto – Medarbetarens e-post-ID
- PSC-partnerkonto – Kontot som medarbetaren är associerad med i PSC
- PSC-användarroll – en av de tre rollerna som tilldelats i PSC.
- PLATS för DATOR-MPN – Den plats där användaren får relevanta Partner Center-roller (PC). MPN för PSC-partnerkontot används för att hitta motsvarande MPN-plats i Partnercenter för att tilldela behörigheter. Hela organisationen anger det virtuella MPN-ID:t.
- Datoranvändarroll – Anställda tilldelas roller baserat på sina PSC-användarroller. Administratören i PSC tilldelas administratörsroller för hänvisningar i Partnercenter. Säljaren tilldelas referensanvändarrollen i Partnercenter. Läs mer om Partner center-roller och vad användare med dessa roller kan göra i Tilldela användarroller och behörigheter för ett företags användare som behöver [arbeta i Partnercenter.](permissions-overview.md#manage-referrals)
- PC AAD-klient – den Microsoft Azure Active Directory (Azure AD)-klient som användarna är tilldelade till i Partnercenter
- Status – Det finns tre möjliga tillstånd för migreringens status
    - **Inte migrerad** – användaren har inte tilldelats någon referensroll i Partnercenter
    - **Migrerad** – Användaren har migrerats med relevant roll tilldelad enligt tabellen
    - **Fel** – Det gick inte att slutföra migreringen på grund av ett fel

Ibland kan migreringen misslyckas och resultera i fel. Här är några orsaker till varför en migrering kan orsaka ett fel och några av sätten att lösa problemet:

1. PSC-användarna kanske använder ett icke-arbetskonto.

2. PSC-användaren kanske använder ett konto från en annan domän än den du använder i Partnercenter.

   För att lösa fel som rör scenarier 1 och 2 ber du användaren att logga in på Partnercenter med sitt arbetskonto som är kopplat till din Azure AD-klientorganisation. Din [globala administratör](permissions-overview.md#manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles) kan vara till hjälp.
   
   Så här hittar du din globala administratör: 
   1. Logga in på [instrumentpanelen i Partnercenter](https://partner.microsoft.com/dashboard) **och välj Kontoinställningar** från kugghjulsikonen längst upp till höger.
   2. Välj **Användarhantering** i det vänstra navigeringsfältet på den andra nivån.
   3. Längst upp i användarlistan väljer du **listrutan Filter** och ändrar alternativet till **Global administratör.** Sidan visar sedan alla globala administratörer med sina respektive e-postadresser. Be en av dem att tilldela referensadministratörsrollen för ditt arbetskonto.
   
      Den globala administratören kan antingen skapa ett nytt användarkonto i din Azure AD-klientorganisation eller tilldela gästanvändaråtkomst till de andra domänkontoanvändarna. När kontona har ställts in för alla PSC-avtalshanterare och användare måste de logga in på Partnercenter, välja Referenser på den vänstra **navigeringsmenyn** och bekräfta att de kan se sidan Referenser.

3. Användaren har redan en referensroll tilldelad i Partnercenter.
    - Du kan verifiera användarens befintliga roll. I det övre högra hörnet i Partnercenter väljer du **Inställningar** (kugghjulsikonen) och sedan **Kontoinställningar**. När du ser en andra vänster navigeringsmeny väljer **du Användarhantering** och söker efter användaren.

## <a name="psc-deals-migration"></a>Migrering av PSC-avtal

När du har slutfört användarmigrering använder du avtalsmigreringsguiden på sidan möjligheter till säljförsäljning för att ta med alla berättigade öppna avtal från PSC till Partnercenter. **Hanterar migreringslänken visas endast för referensadministratörer med hela organisationens omfång i Partnercenter.** Länken för **PSC-avtalsmigrering** visas längst upp till höger på sidan med möjligheter till säljsamarbete och öppnar avtalsmigreringsguiden.

Läs det här avsnittet innan du påbörjar avtalsmigrering.

**Berättigad till migrering**

Endast vissa avtal är berättigade till migrering från PSC till PartnerCenter. Den här migreringsguiden har skapats för att hjälpa partner att få sina avtal till Partnercenter där de fortfarande arbetar aktivt med sina kunder för att stänga avtalet. **Endast avtal i öppet tillstånd som skapats från 1 januari 2020 med giltig partnerkontoinformation (giltigt MPN-ID) är berättigade till migrering.**

## <a name="pre-requisites-for-deal-migration"></a>Förutsättningar för avtalsmigrering

Innan du påbörjar avtalsmigrering från Partnercenter följer du anvisningarna nedan för att konfigurera avtal i PSC för en lyckad migrering.

- Alla medlemmar i säljteamet i företaget som arbetar med öppna avtal informeras om migreringen.
- Säljteamets medlemmar tränas att använda Partnercenter för avtalshantering.
- Avtal har all nödvändig information enligt beskrivningen nedan.
    - Kundens företagsinformation, inklusive namn och adress
    - Minst en lösning
    - Minst en teammedlem med all information – förnamn, efternamn, e-post-ID och telefonnummer
    - Avtalsvärde
    - Beräknat avtalsdatum
    - Partneranteckningar

Du kan använda funktionerna för massnedladdning och uppladdning i PSC för att lägga till all information som saknas i avtalet för alla berättigade avtal.

>[!Note]
> Avtalsmigrering lyckas även om ovanstående krav inte uppfylls. Men du kan inte ändra tillståndet för avtalet om något av ovanstående obligatoriska fält i Partnercenter inte är tillgängligt. Du måste sedan ange all nödvändig information som saknas i avtal i Partnercenter för att börja arbeta med dem. **Vi rekommenderar starkt att du rensar kvalificerande avtal i PSC innan du migrerar dem till Partnercenter.**

Avtalsmigrering i Partnercenter har skapats med ett klick. Allt du behöver göra är att klicka på **knappen "Migrera avtal"** när ditt företag är redo att migrera de berättigade erbjudandena. **Du kan inte välja de avtal som du vill migrera från PSC. Om du inte vill migrera några avtal till Partnercenter flyttar du dem till stängt tillstånd i PSC innan du påbörjar migreringen.**

>[!Note]
> När du har initierat **migreringen kan det ta upp till 24 timmar innan avtal migreras**.

När migreringen är klar ändras banderollmeddelandets status för att slutföras med en länk till migreringsrapporten. Ladda ned rapporten för att visa information om avtal som har migrerats från PSC till Partnercenter.

Rapporten innehåller informationen nedan.

- **Engagemangs-ID för Partnercenter** – Den unika identifieraren i Partnercenter för alla avtal i ett engagemang. Det finns två avtal – ett för partnern och ett för Microsoft i ett engagemang för säljförsäljning i Partnercenter.
- **Referens-ID för Partnercenter** – Den unika identifieraren i Partnercenter för avtalet som tillhör partnern.
- **Avtalsnamn** – Identifierare som anges för avtalet i PSC.
- **PSC-avtals-ID** – Den unika identifieraren i PSC för avtalet.
- **Fel –** för att ange om det finns några fel vid migrering av ett specifikt avtal.

Alla avtal som har migrerats visas inte i PSC. Du kan fortsätta att arbeta med migrerade avtal i Partnercenter.

Avtal som migreras från PSC kommer att vara tillgängliga på fliken Utgående på sidan Möjligheter till säljförsäljning. Alla avtal skapas som partnerledda avtal. De är synliga för Microsoft-säljare.

>[!Important]
> Om det finns fel som gör att vissa avtal inte kunde migreras kan du initiera om avtalsmigrering genom att klicka på knappen **"Migrera avtal".** Det aktiveras bara om det finns vissa berättigade avtal som ännu inte har migrerats. Detta är också användbart om du befinner dig i övergångsfasen där vissa nya avtal skapas i PSC efter att du har initierat avtalsmigrering.

När alla avtal har migrerats visas en banderoll som visar "Inga avtal **att migrera"** med knappen **"Migrera avtal"** **inaktiverad.**

## <a name="next-steps"></a>Nästa steg

Lär dig hur du skapar och hanterar IOT-avtal i Partnercenter.
Det här är ett viktigt steg som hjälper dig att förbereda dig för IOT-avtalshantering i Partnercenter. Förstå arbetsflödena och ändringarna i Partnercenter så att du effektivt kan skapa och hantera avtal. Börja med att läsa det här dokumentet helt.

## <a name="differences-between-psc-and-pc-workflows"></a>Skillnader mellan PSC- och PC-arbetsflöden

|**Scenario**|**Partnerförsäljnings-Anslut**|**Partnercenter**|
|-----|:-----|:-----|
|Användarroller|PSC har administratörs-, avtalshanterare- och säljarroller.|Partnercenter har [referensadministratörs- och referensanvändarroller](permissions-overview.md#manage-referrals) som ger både läs- och skrivbehörighet baserat på platsomfånget.|
|Microsofts säljarinformation|Synligt så fort ett avtal skapas.|Microsofts säljarinformation är inte synlig för partner eftersom avtalstypen är partnerledd.
|Lösningar|Ett val annat antal lösningar kan läggas till i avtalet.|Partner kan lägga till högst 50 lösningar i avtalet.
|Avtalstilldelning|Endast en tilldelad säljare kan visa och agera på affärerna.|Hänvisningsanvändare som lagts till i teamavsnittet i ett avtal kan se och agera på avtalet. Referensadministratörer för DEN MPN-plats där avtalet har skapats kan visa och agera på avtalet.|
|Kundorganisation|Fritextpost.|Du kan söka i [kundorganisationen](manage-co-sell-opportunities.md#select-your-customer) mot [D-&B-databasen](https://www.dnb.com/) genom att bara skriva några tecken. Det juridiska namnet och adressen fylls i automatiskt baserat på valet.|

## <a name="moving-from-psc-to-pc---faq"></a>Flytta från PSC till PC – Vanliga frågor och svar

Följande avsnitt besvarar vanliga frågor om migreringen.

### <a name="1---what-should-i-do-if-i-dont-have-access-to-partner-center"></a>1 – Vad ska jag göra om jag inte har åtkomst till Partnercenter?

Du kan kontakta dina administratörer på sidan "Ingen åtkomst" för att få rollerna tilldelade. Du behöver [referensadministratörsrollen](permissions-overview.md#manage-referrals) för läs- och skrivbehörighet under referensavsnittet. Om du bara hanterar företagsprofiler behöver du rollen som företagsprofiladministratör i Partnercenter.

:::image type="content" source="images/pscmigration/noaccess.png" alt-text="Bild som visar ingen åtkomstupplevelse i Partnercenter.":::

### <a name="2---who-can-grant-me-access-to-the-referrals-section-in-partner-center"></a>2 – Vem kan ge mig åtkomst till avsnittet Referenser i Partnercenter?

[Kontoadministratören](permissions-overview.md#manage-mpn-membership-and-your-company) kan ge dig åtkomst till fliken Referenser. Du hittar kontoadministratören genom att **välja Kontoinställningar** från kugghjulsikonen längst upp till höger på instrumentpanelen i [Partnercenter.](https://partner.microsoft.com/dashboard) Välj sedan **Användarhantering i** det vänstra navigeringsfältet på den andra nivån. Längst upp i användarlistan väljer du **listrutan Filter** och ändrar alternativet till **kontoadministratör.** Sidan visar alla kontoadministratörer med sina respektive e-postadresser. Be en av dem att tilldela referensadministratörsrollen för ditt arbetskonto.

### <a name="3---the-new-deal-button-is-greyed-out-for-our-account-what-should-i-do-to-start-creating-deals"></a>3 – Knappen +nytt avtal är nedtonad för vårt konto. Vad ska jag göra för att börja skapa avtal?

Detta inträffar bara om det MPN-ID som är associerat med ditt konto inte har aktiverats för att skapa IOT-avtal. Kontakta IOT-affärsteamet via e-post under utbildningssessionerna eller skapa en supportbiljett för att få ditt MPN-ID aktiverat för IOT-avtal."

### <a name="4---can-i-assign-deals-to-a-specific-person-from-our-organization-like-psc"></a>4 – Kan jag tilldela avtal till en viss person från vår organisation, till exempel PSC?

Du kan tilldela teammedlemmar till ett visst avtal. Det blockerar inte andra hänvisningsadministratörer från att visa eller agera på dessa avtal.

### <a name="5---is-there-a-view-of-all-the-deals-assigned-to-me"></a>5 – Finns det någon vy över alla avtal som tilldelats mig?

Du kan använda funktionen Favoriter, som är en flik på användarnivå. Du kan markera alla avtal som har tilldelats dig som favoriter för att få en snabb åtkomst till erbjudandena.

### <a name="6---is-there-a-read-only-view-for-the-deals"></a>6 – Finns det en skrivskyddade vy för avtal?

Nej, det finns ingen skrivskyddade vy över avtal i hänvisningsavsnittet.

### <a name="7---is-adding-a-customer-organization-mandatory"></a>7 – Är det obligatoriskt att lägga till en kundorganisation?

Ja, det är [obligatoriskt att lägga](./manage-co-sell-opportunities.md#select-your-customer) till en kundorganisation i Partnercenter. Börja med att söka efter den plats där kunden befinner sig. Baserat på den information som du har; Du kan lägga till specifik information, inklusive det exakta byggnamnet eller bara ge information om staden. Organisationssökningen hämtar alla juridiska personer som matchar det namn som du anger så att du inte behöver ange någon adressinformation. All information fylls i automatiskt baserat på den organisation som valts.

### <a name="8---are-customer-contact-details-mandatory"></a>8 – Är kundens kontaktuppgifter obligatoriska?

Ja, kundkontaktinformation är obligatorisk för att skapa IOT-avtal.

### <a name="9---how-many-solutions-can-i-add-to-a-deal"></a>9 – Hur många lösningar kan jag lägga till i ett avtal?

Du kan lägga till upp till 50 lösningar (detsamma som "produkter" i PSC) i ett avtal. Både kvantitet och beräknat stängningsdatum för lösningarna är obligatoriskt och det uppskattade stängningsdatumet för lösningarna bör vara tidigare än det uppskattade stängningsdatumet i avsnittet med avtalsinformation.

### <a name="10---where-can-i-find-the-opportunity-id"></a>10 – Var hittar jag affärsmöjlighets-ID:t?

Affärsmöjlighets-ID i PSC är samma som hänvisnings-ID:t i Partnercenter. Du hittar referens-ID:t bredvid avtalsnamnet när du öppnar ett avtal.
