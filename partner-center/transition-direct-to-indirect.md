---
title: Växla direkt fakturerings partner till indirekt åter försäljare
ms.topic: how-to
ms.date: 06/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Lär dig hur en CSP-programpartner kan använda Partner Center för att övergå från direkt fakturerings partner till indirekt åter försäljare.
author: aarzh-AaronZhang
ms.author: v-aarzh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 0e7676df62aa6ea91492f9904ac810397fb0e5aa
ms.sourcegitcommit: 35fe0fdc41886f6f5af71ec74e4a4ebd245dfe1d
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/22/2021
ms.locfileid: "104768762"
---
# <a name="transition-from-cloud-solution-provider-csp-direct-bill-partner-to-csp-indirect-reseller"></a>Övergå från en CSP-partner med direktfakturering till en indirekt CSP-återförsäljare

**Lämpliga roller**

- Global administratör

>[!Note]
>Den här artikeln är avsedd för direkta fakturerings partner som har valt att övergå till indirekta åter försäljare. Men även om du inte har gjort ett explicit beslut än att registrera sig som en indirekt åter försäljare, kommer direkta fakturerings partner som inte uppfyller de nya [kraven](direct-partner-new-requirements.md) för fakturerings programmet för CSP: n att informeras av Microsoft när deras [direkta fakturerings kapacitet är begränsad](restricted-direct-bill-capabilities.md).
<br>Från och med januari 2021 kommer ett nytt intäkts krav att läggas till. Partner som har registrerats som en direkt fakturerings partner måste ha överfört minst USD $ över 300 000 i moln lösnings leverantörens program intäkt till en global partner global konto nivå under de föregående 12 månaderna.

Du kommer att kunna registrera i det indirekta åter försäljar programmet med din befintliga direkt fakturerings klient.

## <a name="get-started"></a>Kom igång

1. Se till att din partner profil i Partner Center och MPN-ID är aktuella.

2. Logga in på Partner Center som global administratör för den direkta fakturerings klient som du översätter till indirekt åter försäljare.

   :::image type="content" source="images/direct/direct1.png" alt-text="Översikt":::

3. Granska din partner information i registrerings formuläret.

   :::image type="content" source="images/direct/direct2a.png" alt-text="Registrera dig nu":::

4. Välj Registrera nu. Den indirekta åter försäljaren kommer att använda samma AAD-klient som du använder för din direkta verksamhet.

    > [!NOTE]
    > Inlednings vis är den här nya över gångs funktionen tillgänglig för partner med datum från september till december. Om du inte har ett jubileums datum mellan september och december visas inte funktionen för tillfället. Partner med jubileums datum i december 2018 kommer att meddelas senare när funktionen har Aktiver ATS för partner.

5. När registreringen är godkänd loggar du in på Partner Center igen.

    > [!NOTE]
    > Även om godkännandet ofta är omedelbart kan det ta upp till fem arbets dagar. När den har godkänts får du ett meddelande till den e-postadress som du har angett under primär kontakt i registrerings formuläret. Du kan också kontrol lera registrerings statusen under **Inställningar**  >  **konto inställningar**  >  **partner profil** > program information.

6. På sidan **Översikt** visas avtalet om indirekt åter försäljare. Välj **Godkänn och fortsätt**. Den här åtgärden aktiverar funktioner för indirekt åter försäljare.

När du har godkänt avtalet för den indirekta åter försäljaren ser du att din partner profil identifierar dig som **både** en direkt fakturerings-och indirekt åter försäljare.

:::image type="content" source="images/direct/direct3.png" alt-text="Indirekt åter försäljar avtal":::

> [!IMPORTANT]
> När du har registrerat dig som en indirekt åter försäljare med den nya funktionen finns det inget alternativ för att återställa till en direkt fakturerings klient. Se till att du utvärderar dina affärs behov fullständigt innan du registrerar dig som en indirekt åter försäljare.

## <a name="while-you-transition-from-direct-to-indirect-reseller"></a>När du övergår från direkt till indirekt åter försäljare

Under den här fasen kommer du fortsätta att hantera dina direkta kunders prenumerations behov, inklusive fakturerings processen. Du kan också börja acceptera kunder från den indirekta leverantören och arbeta som en indirekt åter försäljare.

:::image type="content" source="images/direct/direct4.png" alt-text="Du är både en direkt fakturerings-och indirekt åter försäljare":::

## <a name="find-an-indirect-provider"></a>Hitta en indirekt leverantör

Efter registreringen visas en länk till indirekta leverantörer i det vänstra navigerings fältet. Som en indirekt åter försäljare upprättar du en relation med en indirekt provider som sedan kan hantera fakturerings-, inköps produkter för dina kunder och stödja infrastruktur.

Olika indirekta leverantörer erbjuder olika support och tjänster, så du bör utvärdera leverantörerna i ditt utrymme för att avgöra vilka som bäst motsvarar dina behov. I allmänhet kommer de flesta leverantörer att:

- Ge dig teknisk utbildning och hjälp
- Hjälp att marknadsföra dina produkter och tjänster
- Hantera dina finansierings-och kredit villkor

Sök i listan över officiella [Microsoft-indirekta leverantörer](https://partnercenter.microsoft.com/partner/find-a-provider).

Läs mer, Läs  [partner med indirekta leverantörer](indirect-reseller-tasks-in-partner-center.md)

## <a name="accept-a-partnership-invitation-from-your-indirect-provider"></a>Acceptera en inbjudan från din indirekta leverantör

När du hittar en indirekt Provider för partner med, upprätta ett partnerskap med den indirekta providern i Partner Center.

Den indirekta providern du väljer skickar dig via e-post till en länk för inbjudan till inbjudan som tar dig till deras inbjudan i Partner Center. Se till att din globala administratör loggar in på Partner Center och följer Inbjudnings länken. När du godkänner inbjudan visas leverantörens namn i listan över den indirekta providern.

## <a name="acquire-new-customers-as-indirect-reseller"></a>Skaffa nya kunder som indirekt åter försäljare

Både du och din indirekta leverantör måste ha åter försäljarnas relationer med kunderna. Med dessa relationer för åter försäljare kan du hantera en kunds prenumerationer och tjänster för deras räkning. Om du vill skaffa en ny kund som har en befintlig Azure AD-klient kan du bjuda in kunden att upprätta en åter försäljares relation med både du och din leverantör på samma tid.

Så här skapar du en indirekt åter försäljare-inbjudan:

1. Välj **indirekta leverantörer** från din partner Center vänstra navigerings fältet.

2. Välj **Bjud in nya kunder** för att bjuda in en kund att upprätta en åter försäljares relation med både du och den indirekta providern på samma tid. Leverantören måste ha en åter försäljar relation med din kund, så att de kan skicka beställningar på din kunds räkning när kunden vill köpa nya prenumerationer eller lägga till nya licenser i befintliga prenumerationer.

3. På nästa sida granskar du utkastet till e-postmeddelandet. Du kan öppna utkast meddelandet i ett e-postmeddelande, eller så kan du kopiera meddelandet till Urklipp och klistra in det i ett e-postmeddelande.

4. Redigera texten i e-postmeddelandet för att säga vad du behöver, men se till att inkludera länken som den är anpassad för att ansluta kunden direkt till både ditt konto och ditt leverantörs konto. Välj sedan **Done** (Klar).

5. När kunden har auktoriserat att du och din leverantör ska bli åter försäljare av poster, har du administratörs behörighet för att hantera prenumerationer, licenser och användare för deras räkning, och den indirekta leverantören kommer att kunna skicka beställningar för deras räkning.
6. Om du vill hantera kundens konto, tjänster, användare och licenser expanderar du kundens post genom att välja nedåtpilen nära sitt namn.

Till skillnad från direkta fakturerings partner kan indirekta åter försäljare inte skapa Azure AD-klienter för sina nya kunder i Partner Center. Leverantören skapar klienten och anger dig som den indirekta åter försäljaren för den här kunden. Detta säkerställer att kunden kommer att visas i kund listan i Partner Center.

>[!Note]
>Du kan inte använda din direkta fakturerings funktion för att skapa inköp för kunder som du får som en indirekt åter försäljare.

## <a name="managing-your-direct-bill-customers-and-your-indirect-reseller-customers"></a>Hantera dina kunder med direkt fakturering och dina indirekta åter försäljare

Du hanterar dina kunder med direkt fakturering och dina indirekta åter försäljar kunder på olika sätt.

### <a name="direct-bill-customers-things-you-wont-do-as-an-indirect-reseller"></a>Direkt fakturerings kunder (saker som du inte gör som en indirekt åter försäljare)

- Skapa beställningar för produkter
- Hantera Azure-reservationer
- Hantera deras order historik
- Köp program vara
- Fakturera kunder direkt

### <a name="indirect-reseller-customers"></a>Kunder med indirekt åter försäljare

- Din indirekta leverantör beställer produkter för dina kunder
- Hantera kunders licenser och användare
- Hantera prenumerations förnyelser

### <a name="to-identify-customers-that-you-acquired-as-a-direct-bill-partner"></a>Identifiera kunder som du har köpt som en direkt fakturerings partner

1. Välj **Kunder**.

2. Välj en kund om du vill visa information om dem.

3. Om den här kunden är en direkt fakturerings partner kan du se alternativ för att **lägga till** eller **Visa produkter** och du kommer att se deras prenumerationer.

4. Om kunden har en indirekt åter försäljare relation med dig är dessa alternativ inte tillgängliga.

## <a name="move-your-direct-bill-customers-to-your-indirect-provider"></a>Flytta dina direkt fakturerings kunder till din indirekta leverantör

Din indirekta Provider kan inte skicka beställningar eller befintliga prenumerations överföringar för dina befintliga kunder förrän de har en åter försäljares relation med dem. Du kan använda någon av följande metoder för att upprätta åter försäljarens relation mellan din indirekta leverantör och din befintliga direkta faktura.

- [Relations tillägg för åter försäljare](#reseller-relationship-extension)

- [Skicka en indirekt åter försäljares inbjudan till kunden](#send-an-indirect-reseller-invitation-to-the-customer)

En detaljerad översikt över steg för steg-processen finns i [dokumentet direkt till indirekt över gång](https://partner.microsoft.com/resources/collection/Direct-Bill-transition-to-Indirect-reseller#/)

### <a name="reseller-relationship-extension"></a>Relations tillägg för åter försäljare

Du kan använda funktionen för Relations tillägg för åter försäljare för att upprätta åter försäljarens relation mellan dina befintliga kunder med direkt fakturering och den indirekta providern med hjälp av instrument panelen för partner Center. Observera följande innan du använder funktionen:

- Den här funktionen är bara tillgänglig för direkta fakturerings partner som över gången till bli en indirekt åter försäljare har slutfört [registreringen av den indirekta åter försäljaren](#get-started).

- Du kan bara använda den här funktionen för befintliga kunder med direkt fakturering. Det gäller inte för [indirekta åter försäljar kunder](#acquire-new-customers-as-indirect-reseller).

- Du kan bara välja en indirekt Provider för vilken du har [accepterat en partner-inbjudan från den indirekta providern](#accept-a-partnership-invitation-from-your-indirect-provider).

- En kopia av den fakturerings information som du har för den här kunden kommer att göras tillgänglig för den indirekta leverantören. Du kan komma åt fakturerings informationen genom att gå till konto sidan för den här kunden i Partner Center-instrumentpanelen.

    > [!NOTE]
    > Genom att använda funktionen för Relations tillägg för åter försäljare godkänner du att du delar den fakturerings information som du har för den här kunden med den indirekta providern.

- Den indirekta providern kommer inte att tillhandahållas med [delegerad administrations behörighet](customers-revoke-admin-privileges.md) till kund klienten. Om den indirekta leverantören kräver delegerad administrations behörighet måste du skicka en indirekt åter försäljare-inbjudan till kunden i stället.

- När åter försäljarens relation har upprättats visas den indirekta providern som en CSP-partner till kunden på sidan partner relationer i [Microsoft 365 administrations Center](https://admin.microsoft.com/AdminPortal/Home#/partners) och [Microsoft Store för företag](/microsoft-store/work-with-partner-microsoft-store-business).

    > [!IMPORTANT]
    > För att undvika förvirring och missförstånd är du avtals enlig avtal av ditt partner avtal för att informera och erhålla medgivande från direkt fakturerings kunden innan du använder funktionen för Relations tillägg för att upprätta åter försäljarens relation mellan en befintlig direkt fakturerings kund och en indirekt leverantör.

Så här använder du den här funktionen på en befintlig kund klient organisation:

1. Logga in på Partner Center som **Administratörs agent**.

2. På **sidan kunder** väljer du en befintlig kund och klickar på dess **snabb länkars** ikon för att expandera kundens sammanfattningsvy.

3. Under **indirekta providers** klickar du på **överför kund på en indirekt Provider**.

    :::image type="content" source="images/direct/direct5-1.png" alt-text="Överför kunden till en indirekt Provider":::

4. I popup-dialogrutan väljer du den **indirekta providern** som du vill ha åter försäljarens relation med kunden.

5. Klicka på **Spara och fortsätt**.

6. Kontrol lera att den valda indirekta providern visas under **indirekta providers**.

    :::image type="content" source="images/direct/direct5-2.png" alt-text="Indirekt Provider listad":::

### <a name="send-an-indirect-reseller-invitation-to-the-customer"></a>Skicka en indirekt åter försäljares inbjudan till kunden

Din indirekta leverantör kan inte skicka in beställningar för dina befintliga kunder för direkt fakturering förrän de har en åter försäljares relation med dem. För att upprätta åter försäljarens relation mellan dina befintliga kunder och den indirekta leverantören, bjuder du in kunden med en indirekt åter försäljares inbjudan.

1. Välj **indirekta leverantörer** från din partner Center vänstra navigerings fältet.

2. Välj **Bjud in nya kunder** för att bjuda in en kund att upprätta en åter försäljares relation med både du och den indirekta providern på samma tid. Leverantören måste ha en åter försäljar relation med din kund, så att de kan skicka beställningar på din kunds räkning när kunden vill köpa nya prenumerationer eller lägga till nya licenser i befintliga prenumerationer.

    :::image type="content" source="images/direct/direct6.png" alt-text="Bjud in nya kunder":::

3. På nästa sida granskar du utkastet till e-postmeddelandet. Du kan öppna utkast meddelandet i ett e-postmeddelande, eller så kan du kopiera meddelandet till Urklipp och klistra in det i ett e-postmeddelande.

4. Redigera texten i e-postmeddelandet för att säga vad du behöver, men se till att inkludera länken som den är anpassad för att ansluta kunden direkt till både ditt konto och ditt leverantörs konto. Välj sedan **Done** (Klar).

5. När kunden har auktoriserat att du och din leverantör ska bli åter försäljare av poster, har du administratörs behörighet för att hantera prenumerationer, licenser och användare för deras räkning, och den indirekta leverantören kommer att kunna skicka beställningar för deras räkning.

6. Om du vill hantera kundens konto, tjänster, användare och licenser expanderar du kundens post genom att välja nedåtpilen nära sitt namn.

### <a name="microsoft-customer-agreement-acceptance"></a>Godkännande av Microsofts kund avtal

Microsoft Cloud avtalet gäller till och med 31 januari 2020. Efter det datumet måste alla kunder, befintliga och nya, signera det nya [Microsofts kund avtal](confirm-customer-agreement.md). Vid över gång av kunder, om:

- **Kunden har inte accepterat Microsofts kund avtal ännu**

   Arbeta med den indirekta leverantören för att låta kunden [godkänna Microsofts kund avtal](confirm-customer-agreement.md).

- **Kunden har accepterat Microsofts kund avtal med dig via Microsoft 365 administrations centret**

   Godkännandet kommer att behållas när åter försäljarens relation upprättas med den indirekta providern. Du behöver inte göra något.

- **Kunden har accepterat Microsofts kund avtal med dig genom partner attestering**

   Godkännandet kommer inte att behållas. Arbeta med den indirekta providern för att [Uppdatera kundens godkännande i Partner Center](confirm-customer-agreement.md#confirm-customer-acceptance-for-existing-customers).

## <a name="transfer-existing-direct-bill-subscriptions-to-indirect-provider"></a>Överför befintliga direkt fakturerings prenumerationer till en indirekt Provider

Under KRYPTOGRAFIPROVIDERns indirekta modell har indirekta åter försäljare inga fakturerings relationer med Microsoft. I stället får indirekta åter försäljare prenumerationer för sina kunder via sina indirekta leverantörer. Vid över gång från direkt fakturerings partner till indirekt åter försäljare måste du överföra de befintliga prenumerationerna som du har som direkt fakturerings partner till din indirekta leverantör. Du kan använda funktionen för att överföra prenumerationer på Partner Center-instrumentpanelen.

### <a name="prerequisites"></a>Förutsättningar

- Den här funktionen är bara tillgänglig för att överföra partner som har slutfört registreringen av den indirekta åter försäljaren med sina befintliga leverantörer av direkt fakturerings partner.

- Innan prenumerationer som är kopplade till en specifik kund överförs måste övergående partner flytta kunden till en indirekt Provider.

- Kunden måste ha [godkänt Microsofts kund avtal via den indirekta providern](#microsoft-customer-agreement-acceptance).

### <a name="how-to-transition-to-indirect-reseller-status"></a>Hur du övergår till en indirekt åter försäljares status

Funktionen är en fyra stegs process där:

- Över gångs partnern skapar en begäran om prenumerations överföring. Begäran innehåller en eller flera befintliga prenumerationer som är kopplade till samma kund och som är adresserad till en indirekt Provider.

- Den indirekta providern granskar och godkänner (eller avvisar) överföringsbegäran.

- Den indirekta providern verifierar att överföringsbegäran är slutförd.

- Över gångs partner verifierar att överföringsbegäran är slutförd.

### <a name="transitioning-partner"></a>Över gångs partner

> [!NOTE]
> Du kan också använda [partner Center API/SDK](/partner-center/develop/manage-customers) för att överföra befintliga prenumerationer till den indirekta providern.
>
> - [Hämta en kunds prenumerationers överföringsberättigande](/partner-center/develop/get-customer-s-subscriptions-transfer-eligibility)
> - [Skapa en kunds överföring](/partner-center/develop/create-a-transfer)
> - [Återkalla en kunds överföring](/partner-center/develop/withdraw-a-transfer)
> - [Acceptera en kunds överföring](/partner-center/develop/accept-a-transfer)
> - [Avvisa en kunds överföring](/partner-center/develop/reject-a-transfer)
> - [Hämta en kunds överföringar](/partner-center/develop/get-all-of-a-customer-s-transfers)
> - [Hämta överförings information per ID](/partner-center/develop/get-transfer-by-id)

### <a name="transitioning-partner---create-transfer-request"></a>Över gångs partner – skapa överföringsbegäran

Så här skapar du en överföringsbegäran som över gångs partner:

1. Logga in på Partner Center som **Administratörs agent**.

2. På sidan **kunder** väljer du den avsedda kunden och klickar på ikonen snabb Länkar för att expandera kundens sammanfattningsvy.

3. Under **indirekta providers** kontrollerar du att den avsedda indirekta providern visas.

4. Klicka på **Visa prenumerationer**.

5. På sidan **prenumerationer** söker du efter **prenumerations överföring**.

6. Under **prenumerations överföring** klickar du på **begär prenumerations överföring**.

    :::image type="content" source="images/direct/direct8.png" alt-text="Begär prenumerations överföring":::

7. I dialog rutan överför begäran väljer du en eller flera prenumerationer som ska överföras.

    :::image type="content" source="images/direct/direct9.png" alt-text="Skapa överföringsbegäran":::

8. Klicka på **Skapa**.

9. En aktiv begäran om prenumerations överföring visas under **prenumerations överföring**.

    :::image type="content" source="images/direct/direct10.png" alt-text="Lista över överförings begär Anden":::

10. Informera den indirekta leverantören att du har skapat en begäran om prenumerations överföring.

### <a name="indirect-provider---accept-transfer-request"></a>Indirekt Provider-Godkänn överföringsbegäran

Så här granskar och godkänner du en överföringsbegäran som den indirekta providern:

1. Logga in på Partner Center som **Administratörs** agent eller **försäljnings agent**.

2. På sidan **kunder** väljer du den avsedda kunden och klickar på dess snabb länkars ikon för att expandera kundens sammanfattningsvy.

3. Under **indirekta åter försäljare** bekräftar du att över gångs partnern visas.

4. Klicka på **Visa prenumerationer**.

5. På sidan **prenumerationer** söker du efter **prenumerations överföring**.

    :::image type="content" source="images/direct/direct11.png" alt-text="Visa överförings förfrågan":::

6. Under **prenumerations överföring** klickar du på den överföringsbegäran som ska granskas.

7. Klicka på **acceptera** (eller **avvisa**) efter behov.

    :::image type="content" source="images/direct/direct12.png" alt-text="Godkänn överföringsbegäran":::

8. Vänta tills överförings förfrågan har slutförts.

### <a name="indirect-provider---verify-transfer-request-is-complete"></a>Indirekt provider-Kontrol lera att överföringsbegäran har slutförts

1. När överföringsbegäran har slutförts kontrollerar du att du kan se att prenumerationerna visas under **prenumerationer**.

2. Informera över gångs partnern.

### <a name="transitioning-partner---verify-transfer-request-is-complete"></a>Övergående partner – kontrol lera att överföringsbegäran har slutförts

Över gångs partner bör göra följande:

1. Logga in på Partner Center som **Administratörs agent** eller **försäljnings agent**.

2. På sidan **kunder** väljer du den avsedda kunden och klickar på ikonen **snabb länkar** för att expandera kundens sammanfattningsvy.

3. Klicka på **Visa prenumerationer**.

4. På sidan **prenumerationer** söker du efter **prenumerations överföring**.

5. Kontrol lera att överföringsbegäran har marker ATS som **slutförd**.

6. Kontrol lera att prenumerationerna inte längre visas som aktiva på sidan **prenumerationer** :

   1. Om det här är en Azure-prenumeration (MS-AZR-0145P) visas den inte längre.

   2. Om det här är en licens baserad prenumeration (Office 365, Dynamics, Intune) visas den med tillståndet **pausad**.

   :::image type="content" source="images/direct/direct13.png" alt-text="Prenumerationen har pausats":::

### <a name="considerations"></a>Överväganden

- **Prenumerations-ID skiljer sig efter överföringen.** Om det är en Azure-prenumeration (MS-AZR-0145P) har dessutom ett ID för Azure-prenumeration, som är kvar från den tidigare ägaren, och kommer att visas i Azures hanterings Portal.

- **Det går inte att referera till samma prenumeration av flera överförings begär Anden.** När du har skapat en överföringsbegäran som innehåller en befintlig prenumeration kan du inte skapa ytterligare överförings begär Anden, inklusive samma prenumeration, tills den första överförings förfrågan har avbrutits.

- **Tilläggs komponenter för licensbaserade prenumerationer måste överföras tillsammans med deras bas prenumeration.** Om du väljer en befintlig prenumeration med ett eller flera tillägg tas tilläggen automatiskt med i överföringsbegäran när du skapar en överföringsbegäran.

- **Ändringar av licens antalet för en prenumeration visas inte i den befintliga överförings förfrågan.** När du har skapat en överföringsbegäran som innehåller en befintlig prenumeration bör du undvika att uppdatera licens antalet för prenumerationen (eller tillhör ande tillägg). Om du gör det visas inte den nya kvantiteten i överförings förfrågan. När den indirekta providern har accepterat överförings förfrågan kommer den resulterande prenumerationen att ha den gamla kvantiteten. Om du vill att den nya kvantiteten ska överföras till den indirekta providern måste du avbryta den befintliga överföringsbegäran och återskapa en ny.

- **Alla inköp kan inte överföras med hjälp av prenumerations överföring med egen prenumeration.** För närvarande kan du bara överföra O365-prenumerationer och Azure PAYG-prenumerationer (MS-AZR-0145P) med hjälp av den här funktionen. Andra köp, inklusive Azure-planer, reserverade Azure-instanser, Termbaserade prenumerationer och SaaS-prenumerationer för Azure Marketplace stöds inte. Du kommer att se en orsak till varför en prenumeration inte kan överföras på sidan skicka överförings förfrågan. Om du vill överföra dessa prenumerationer måste du [avbryta den befintliga prenumerationen](create-a-new-subscription.md#suspend-or-cancel-a-subscription) och köpa ett nytt erbjudande för kunden via den indirekta providern.

- **Kan inte testas med sandbox-miljö.**

## <a name="enroll-for-indirect-reseller-incentives"></a>Registrera dig för indirekta åter försäljares incitament

När du har registrerat dig som en indirekt åter försäljare på din befintliga leverantör av direkt fakturerings partner får du en inbjudan om att registrera sig för en indirekt åter försäljares stimulans inom 30 dagar. Inbjudan baseras på partner MPN-kontot som för närvarande är associerat med din CSP-partners klient. Inbjudan skickas till den e-postadress som är kopplad till partner MPN-kontot.

Du är också berättigad till att registrera sig för direkt fakturerings program med samma partner klient organisation. Du måste hantera programmen separat.

## <a name="next-steps"></a>Nästa steg

- [Ytterligare information om att bli en indirekt åter försäljare](https://assetsprod.microsoft.com/csp-directbill-to-indirect-transition.pdf)
- [CSP Direct-partner nya krav](direct-partner-new-requirements.md)
- [Begränsade direkta fakturerings funktioner](restricted-direct-bill-capabilities.md)
