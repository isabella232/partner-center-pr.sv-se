---
title: Migrera från partner Sales Connect (PSC)
ms.topic: article
ms.date: 08/27/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Lär dig hur Microsoft-partner kan migrera från partner Sales Connect (PSC) till Partner Center och skapa eller hantera avtal som skickas av Microsofts säljare.
author: vikramb
ms.author: vikramb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: dc131991826a6428d613aa34e2e99c19e3efde05
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/22/2020
ms.locfileid: "92531548"
---
# <a name="guide-to-co-selling-in-partner-center-pc-for-partners-migrating-from-partner-sales-connect-psc"></a>Guide till samförsäljning i Partner Center (PC) för partners som migrerar från partner Sales Connect (PSC)

**Gäller för**

- Partnercenter

**Lämpliga roller**

- Kontoadministratör
- Referens administratör
- Säljare Sälj anslutning (PSC) säljare
- Administratör för partner Sales Connect (PSC)
- Avtals chef för partner Sales Connect (PSC)

Som du vet kommer företaget att förlora åtkomsten till PSC-inlägget 31 december 2020. Men du hittar allt du vill göra för att skapa samförsäljnings avtal, hantera dina avtal och agera på avtal som skickas av Microsoft-säljare till dig i Partner Center. Det kommer dock att finnas skillnader och följande rikt linjer hjälper dig att göra din över gång till Partner Center mjukare och rakt framåt.

>[!Important]
> Om du är här eftersom du såg en banderoll i PSC om migreringen är du på rätt plats. Den här guiden gäller inte för lösnings bedömning (SA) och OEM IOT-partner som hanterar sina avtal i PSC.

## <a name="before-you-move-things-you-need-to-know"></a>Innan du flyttar, saker du behöver känna till

### <a name="if-you-are-psc-admin"></a>Om du är PSC-administratör

- Du behöver ett e-postmeddelande om arbetet för att logga in på [partner Center](https://partner.microsoft.com/).
- Konfigurera ditt konto med hjälp av [konto administratören](permissions-overview.md)för partner Center.
- Lär dig att samsälja i Partner Center genom att läsa det här dokumentet.
- Konfigurera användar konton i Partner Center för alla PSC-användare (admin, avtals chef och säljar roller) och tilldela dem [referenser till administratörs roller](permissions-overview.md).

>[!Important]
> Kontrol lera att MPN-ID: t som visas i PSC-banderollen är tillgängligt i listan över MPN-platser i Partner Center. Du kan kontrol lera att i Partner Center genom att gå till "konto inställningar" och "[platser](manage-locations.md)" under att hitta listan över alla MPNS som är associerade med partner Center-kontot.

 :::image type="content" source="images/pscmigration/mpnidcheck.png" alt-text="Bild som visar den PSC-banderoll där partner kan hitta MPN-ID: t.":::

### <a name="if-you-are-psc-deal-manager-or-seller"></a>Om du är PSC-ansvarig eller säljare

- Du behöver ett e-postmeddelande för arbetet för att logga in på [partner Center](https://partner.microsoft.com/).
- Om du använder ett icke-arbetskonto i PSC eller om din e-postadress för arbetet är för ett annat företag än partner företaget, kontaktar du PSC-administratören för att få hjälp med att konfigurera konton.
- Kontrol lera med PSC-administratören om ditt konto för partner Center-kontot är klart oberoende av det konto som du använder för att logga in på PSC.
- Kontrol lera att du har åtkomst till Partner Center och avsnittet om referenser.
- Läs det här dokumentet för att förstå arbets flöden och ändringar i Partner Center.

## <a name="as-an-admin-in-psc-these-are-your-next-steps"></a>Som administratör i PSC är dessa nästa steg

Om du inte ser fliken hänvisningar:

- Företagets [globala administratör](permissions-overview.md) kan ge dig åtkomst till fliken hänvisningar. Om du vill hitta din globala administratör går du till partner inställningar från kugg hjuls ikonen längst upp till höger i Partner Center. Välj sidan användar hantering på den andra nivån i det vänstra navigerings fältet. Klicka på list rutan som visar "alla användare" längst upp till höger på sidan och ändra till "globala administratörer". På sidan visas sedan alla globala administratörer med deras respektive e-post-ID. Kontakta dem för att få åtkomst till "referral admin" för ditt arbets konto.

>[!Important]
> Om din roll endast hanterar användare i PSC kan du få rollen som [konto administratör](permissions-overview.md#manage-mpn-membership-and-your-company) i Partner Center. Om din roll även omfattar att hantera samförsäljnings möjligheter bör du få [referensinformations administratörs](permissions-overview.md#manage-referrals) roll. Utse också ett lead för ändrings hantering bland PSC-administratörerna att arbeta med partner Center-kontots administratör i stället för alla PSC-administratörer som når ut till konto administratörerna på PC individuellt.

 :::image type="content" source="images/pscmigration/accountadmin.png" alt-text="Bild som visar den PSC-banderoll där partner kan hitta MPN-ID: t." längst upp till höger på sidan och ändra till "globala administratörer".
- Den globala administratören kan antingen skapa ett nytt användar konto i din Azure AD-klient eller tilldela gäst användare åtkomst till andra domän konto användare.
- När kontona har kon figurer ATS för alla PSC-chefer och användare måste de logga in på Partner Center, gå till fliken hänvisning i det vänstra navigerings fönstret och kontrol lera att de kan se sidan hänvisningar.

Om ditt företag har ett PDM – när ditt partner Center-konto har kon figurer ATS och dina användare har flyttat och har roller och behörigheter, kan du flytta dina samförsäljnings aktiviteter till Partner Center. Informera PDM för att göra växeln i stället för att vänta tills migreringen har slutförts, vilket gör det möjligt för alla nya avtal att flöda till Partner Center.
>[!Note]
>När du har gjort den här växeln kommer du bara att kunna agera på befintliga aktiva avtal i PSC. Du kan varken skapa nya eller få några avtal från Microsofts säljare i PSC.

Om ditt företag inte har en PDM – se till att alla användar konton är inställda och verifierade av alla användare. Du kommer att meddelas via ett e-postmeddelande och en banderoll i PSC om det exakta datumet när du kan påbörja samförsäljning i Partner Center. Kom ihåg att du fortfarande måste hantera befintliga aktiva avtal i PSC.

>[!Important]
>Aktiva avtal kommer inte att migreras till datorn. Du har till och med den 31 december 2020 att stänga och registrera avtalen.

## <a name="next-steps-for-psc-admins-psc-deal-managers-and-psc-sellers"></a>Nästa steg för PSC-administratörer, PSC-chefer och PSC-säljare

Lär dig att samsälja i Partner Center.
Det här är ett viktigt steg som hjälper dig att förbereda för samförsäljning i Partner Center. Förstå arbets flöden och ändringarna i Partner Center så att du effektivt kan samsälja från dag ett. Börja med att läsa det här dokumentet helt. Det finns också en utmärkt uppsättning resurser i avsnittet [Co-sälje Experience Gallery](https://aka.ms/cosellexperience).

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

## <a name="psc-and-partner-center-field-mapping"></a>Fält mappning för PSC och partner Center

I det här avsnittet visas exakt mappning av attribut mellan PSC-och partner Center. Varje skärm i PSC jämförs med den relevanta vyn i avsnittet om samarbets möjligheter i Partner Center. 

>[!Note]
>Följ talen i de gula bubblorna i PSC-skärmarna för att hitta motsvarande attribut i Partner Center. De röda bubblorna visar att det arkiverade inte är tillgängligt i Partner Center.

**Start sidan för PSC och standardvy för samförsäljnings möjligheterna i Partner Center**

 :::image type="content" source="images/pscmigration/homepage.png" alt-text="Bild som visar den PSC-banderoll där partner kan hitta MPN-ID: t.":::

**Vyn PSC-rutnät och vyn Partner Center**

- Det finns ingen listvy i Partner Center som i PSC.  Alla avtal visas utifrån det senaste mottagna eller skapade datumet med kund informationen och typen av avtal. Det första erbjudandet i vyn är valt som standard. De flesta av de värden som visas i formatet PSC är tillgängliga i vyn detaljerad information för affären i PC.
- Avtals roll är inte ett obligatoriskt fält i PC. Den visas varken eller har inte registrerats i någon av arbets flödena. Den härleds automatiskt på Microsofts säljare sida baserat på de lösningar som lagts till i affären.
- Datumet för senaste ändring visas inte på sidan med hänvisnings information i PC. Partner kan använda sorterings funktionen för att sortera avtalen utifrån det senaste uppdaterade datumet.

 :::image type="content" source="images/pscmigration/gridview.png" alt-text="Bild som visar den PSC-banderoll där partner kan hitta MPN-ID: t.":::

**Vyn avtals information i PSC och partner Center**

- Partner kan redigera ett avtal genom att klicka på knappen Redigera i vyn partner avtals information (6). När du har klickat på alla fält när du har klickat på knappen kan du antingen Spara eller avbryta ändringarna som gjorts i affären.
- Det finns inget alternativ för att stänga affären som dubblett i Partner Center.
- Kund resultatet är inte tillgängligt i Partner Center. All information som rör kund interaktioner kan uppdateras i avsnittet anteckningar i PC.
- Den uppskattade lösningens stängnings datum är bara tillgängligt för OEM IOT-avtal i Partner Center. Den visas inte för andra avtals typer.
- Licens programmet krävs inte i PC. Den härleds automatiskt baserat på de lösningar som valts i affären.

>[!Note]
>Alla avtal som marker ATS som vunna eller förlorade kan inte redige ras. Var försiktig när du flyttar en affär i ett av dessa terminaler-tillstånd.

 :::image type="content" source="images/pscmigration/dealdetails.png" alt-text="Bild som visar den PSC-banderoll där partner kan hitta MPN-ID: t." och vyn Partner Center "Lägg till lösningar"**

 :::image type="content" source="images/pscmigration/products.png" alt-text="Bild som visar den PSC-banderoll där partner kan hitta MPN-ID: t.":::

**Användar hantering i PSC-och partner Center**

 :::image type="content" source="images/pscmigration/usermanagement.png" alt-text="Bild som visar den PSC-banderoll där partner kan hitta MPN-ID: t.":::

**Tilldelning av användar roll i PSC och partner Center**

- Rollen som motsvarighet för PSC-administratör är rollen konto administratör i Partner Center.
- Det finns bara en roll i Partner Center för avtals hantering i samförsäljning som är administrations rollen för administratörer.

 :::image type="content" source="images/pscmigration/roles.png" alt-text="Bild som visar den PSC-banderoll där partner kan hitta MPN-ID: t.":::

**Meddelanden i PSC-och partner Center**

 :::image type="content" source="images/pscmigration/notifications.png" alt-text="Bild som visar den PSC-banderoll där partner kan hitta MPN-ID: t.":::

## <a name="moving-from-psc-to-partner-center---frequently-asked-questions"></a>Flytta från PSC till Partner Center – vanliga frågor och svar

**Bästa. Vad ska jag göra om jag inte har åtkomst till Partner Center?**

Du kan kontakta dina administratörer på sidan "ingen åtkomst" för att hämta de roller som har tilldelats. Du behöver rollen[hänvisnings administratör](permissions-overview.md#manage-referrals)för Läs-och Skriv behörighet i avsnittet hänvisningar. Om du bara hanterar affärs profiler måste du ha rollen företags profil administratör i Partner Center.

:::image type="content" source="images/pscmigration/noaccess.png" alt-text="Bild som visar den PSC-banderoll där partner kan hitta MPN-ID: t." i PSC) i ett avtal. Till skillnad från PSC kan du blanda lösningar från dina egna samsäljande lösningar, Microsofts första parts SKU: er och andra utomstående kvalificerade lösningar från tredje part. Det finns ingen avtals roll som ska väljas eller vara tillgänglig i Partner Center. För Microsoft SKU: er kan du välja att lägga till kvantitet och pris för varje SKU som läggs till i affären.

**Q12. När får jag veta mer om Microsofts säljar information när jag har skapat ett avtal?**

Microsoft-säljare tilldelas endast efter att ha matchat det exakta hjälp kravet som anges när du skapar affären med den berörda säljaren persona på Microsoft-sidan. Även efter tilldelningen har Microsoft-säljare ett alternativ för att acceptera eller avvisa inbjudan till co-försäljning. Om en säljare har accepterat en gemensam inbjudan kommer affären att uppdateras med kontakt uppgifterna för Microsoft-säljaren. Service avtalet för Microsoft-säljarna för att agera med erbjudandet är 14 dagar. Det är samma service avtal som partners måste vidta för att agera i affären innan det går in i det tillstånd som gått ut.

**Q13. Var kan jag hitta ett affärs möjlighets-ID?**

Affärs möjlighets-ID i PSC är detsamma som i avsnittet om avtals-ID i PC. Du kan hitta avtals-ID: t bredvid avtals namnet när du öppnar ett avtal.

**Q14. Hur får mitt PDM åtkomst till datorn?**

Det går inte att komma åt Partner Center från PDM direkt till skillnad från PSC. Det finns flera alternativ för att aktivera funktionen, som nämns nedan.

- OCP-insikter – om PDM bara visar de & förlopp som är relaterade till dem kan de använda OCP Insights-portalen för att få din organisations vy. Det här är ett internt verktyg som endast är tillgängligt för PDM. Observera att OCP Insights inte är tillgängliga för ditt företags användare.
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

## <a name="additional-resources"></a>Ytterligare resurser

- [Partner försäljning Anslut till Partner Center arbets bok](https://partner.microsoft.com/resources/detail/partner-sales-connect-to-partner-center-transition-workbook-pptx) – arbets bok för att anpassa partners försäljnings processer och roller med nya försäljnings processer via partner Center eller partner Sales Connect.
- [Samarbets guide för partner Center](https://partner.microsoft.com/resources/detail/co-sell-operating-model-guide-pptx) – rikt linjer för att identifiera en drifts modell via partner Center för att hantera leads eller samförsäljnings möjligheter och registrera avtal.
- [Referens hanterings däck](https://partner.microsoft.com/resources/detail/referral-management-in-partner-center-pptx) – visualiserade steg-för-steg-instruktioner för att hantera leads och samförsäljnings möjligheter via partner Center.
- [Publicera och hantera i den kommersiella Marketplace](https://partner.microsoft.com/resources/detail/publishing-and-managing-co-sell-offers-in-commercial-marketplace-pptx) – visualiserade steg-för-steg-instruktioner för att skapa, hantera och publicera erbjudanden via partner Center på den kommersiella marknaden.
