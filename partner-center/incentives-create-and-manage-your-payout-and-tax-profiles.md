---
title: Utbetalnings- och skatteprofiler i Partnercenter
ms.topic: how-to
ms.date: 04/15/2021
description: Skapa och hantera din utbetalnings- och skatteprofil så att du kan få betalt för ditt incitamentsarbete. Omfattar att skapa, hantera och använda olika profiler.
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
author: Karthic83
ms.author: kashanum
ms.localizationpriority: medium
ms.openlocfilehash: a6d578c2ad09e1f8bb03f520d659f1a9b1e199a9
ms.sourcegitcommit: 37eac16c4339cb97831eb2a86d156c45bdf6a531
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/13/2021
ms.locfileid: "126249040"
---
# <a name="create-and-manage-incentives-payout-and-tax-profiles-in-partner-center"></a>Skapa och hantera incitament för utbetalnings- och skatteprofiler i Partnercenter

**Lämpliga roller:** Incitamentsadministratörsroller | Kontoadministratörsbehörighet | Global administratör

Innan du kan erhålla betalningar för dina incitamentprogram för en viss MPN-plats måste du slutföra registreringen genom att associera en giltig utbetalnings- och skatteprofil med programmet och MPN-platsen. Microsoft använder den här utbetalnings- och skatteprofilen för att utfärda betalningar. Eventuellt kan du välja att använda elektronisk banköverföring eller en kreditfaktura för betalningar, beroende på reglerna för incitamentprogrammet. 

## <a name="roles-currencies-and-multiple-microsoft-incentive-programs"></a>Roller, valutor och flera Microsoft-incitamentprogram

Det är viktigt att du förstår informationen nedan innan du börjar med din utbetalnings- och skatteprofil.

### <a name="roles-and-permissions"></a>Roller och behörigheter

Du måste vara incitamentsadministratör för att ange bank- och skatteinformation för incitamentbetalningar. Om du är MPN-/kontoadministratör kan du tilldela dig själv och/eller en kollega som incitamentsadministratör.

Om du behöver begära behörighet som incitamentsadministratör kontaktar du MPN-administratören eller den globala administratören. Du kan ta reda på vem i företaget som har dessa roller genom att logga in på [instrumentpanelen i Partnercenter.](https://partner.microsoft.com/dashboard/) Från ikonen **Inställningar** längst upp till höger väljer du **Användarhantering** och filtrerar sedan på Global administratör.

Incitament Användare kan visa incitamentsintäkter, betalningsinformation och rapporter, men kan inte redigera bank- och skatteinformation.

### <a name="choose-your-disbursement-currency"></a>Välj din valuta för bidrag

Incitamentbetalningar görs i den valuta som du valde när du konfigurerade din betalningsprofil. Betalningar beräknas med hjälp av en växelkurs som anges varje månad av Microsoft. Du ansvarar för ändringar i värdet på grund av den valda valutan.

### <a name="using-different-profiles-for-different-microsoft-programs"></a>Använda olika profiler för olika Microsoft-program

Om ditt företag har registrerats i flera incitamentprogram kan du använda samma betalningskonto för alla eller välja att använda olika betalningsmetoder för olika program.

## <a name="create-and-manage-payout-and-tax-profiles-in-partner-center"></a>Skapa och hantera utbetalnings- och skatteprofiler i Partnercenter

Avsnitten nedan beskriver steg för steg hur du skapar och hanterar betalnings- och skatteprofiler i Partnercenter.

>[!IMPORTANT]
>Du måste vara incitamentsadministratör för att skapa eller hantera betalnings- och skatteprofiler i Partnercenter. Incitamentroller måste tilldelas till varje MPN-plats under varje incitamentprogram. Mer information om hur du lägger till incitamentadministratörer i Partnercenter finns [i Skapa användarkonton.](create-user-accounts-and-set-permissions.md)

## <a name="access-the-payout-and-tax-section-in-partner-center"></a>Få åtkomst till utbetalnings- och skatteavsnittet i Partnercenter

1. Logga in på [instrumentpanelen i Partnercenter](https://partner.microsoft.com/dashboard/) med ditt Azure Active Directory-konto (Azure AD) (företagskonto) eller lämplig e-postadress om en sådan har tilldelats.

   - Flera domäner kan registreras i ett Azure AD-konto. Kontakta den globala administratören för att ta reda på vilka domäner som är associerade.
   - Om du bara kan logga in med domänen och du behöver ytterligare domäner kontaktar du kontoadministratören för att lägga till ytterligare domäner @onmicrosoft.com i Azure AD-kontot.
   - Om du uppmanas att välja **Arbets- eller skolkonto eller** **Personligt konto** väljer du **Arbets- eller skolkonto.**

2. Välj kugghjulsikonen för att **öppna Inställningar** och välj sedan **Kontoinställningar.**

3. I menyn **Kontoinställningar** väljer du **Utbetalning och skatt.**

## <a name="assign-payout-and-tax-profiles-to-individual-programs"></a>Tilldela utbetalnings- och skatteprofiler till enskilda program

1. Logga in på [instrumentpanelen i Partnercenter](https://partner.microsoft.com/dashboard/)och välj sedan kugghjulsikonen för att **öppna Inställningar** menyn. 

2. Välj **Kontoinställningar**, expandera avsnittet **Utbetalning och skatt och** välj sedan Tilldelning av **utbetalnings- och skatteprofil.** 
   
   En lista över dina program visas. Välj pilen bredvid ett program för att visa profilinformation. 

3. I **listrutan Skatteprofil** väljer du den skatteprofil som du vill använda eller väljer alternativet för att skapa en ny profil. När du väljer alternativet för att skapa en ny profil omdirigeras du på rätt sätt.  Välj **Fortsätt** i popup-fönstret. Processen för att skapa en ny skatteprofil anges nedan.

4. Välj **Betalningsmetod**.

   - Om du har valt **Elektronisk banköverföring** som betalningsmetod väljer du den betalningsprofil som du vill använda eller väljer alternativet för att skapa en ny profil. När du väljer alternativet för att skapa en ny profil omdirigeras du på rätt sätt. Välj Fortsätt i popup-fönstret. Processen för att skapa en ny betalningsprofil har angetts nedan.

   - Om du har valt **Kreditfaktura** som betalningsmetod slutför du verifieringen. Detta bekräftar att det refererade SAP-numret tillhör din organisation.

    >[!NOTE]
    >Om flera Microsoft-affärsenheter visas måste du välja en betalningsprofil för varje entitet.

    >[!NOTE]
    >Tillgängligheten för betalningsmetoden beror på reglerna för incitamentprogrammet.

    - Om ditt PLATS-MPN-ID betalas av ett lokalt Dotterbolag till Microsoft för ett visst incitamentprogram och tillåter LRD-kreditnota (begränsad riskdistributör) som betalningsmetod, fylls din betalningsprofil i förväg med betalningsmetoden LRD Credit Note. På raden med betalningsmetoden för LRD-kreditnotan för respektive incitamentprogram och  platsens MPN-ID visas **Bekräftad** eller Verifiering krävs som status i avsnittet för betalningsprofil.
    
       Välj **Verifiering krävs för** att bekräfta och verifiera CSP-klientorganisations-ID:t som är associerade med platsens MPN och betalningsmetod för att ta emot betalningen av kreditfakturan. I dialogrutan **Information om kreditnota** granskar och kontrollerar du att klientorganisations-ID och tillhandahållen information för CSP är korrekta. Om du ser fler än ett klientorganisations-ID väljer du noggrant det CSP-klient-ID som du vill ta emot betalningar för. Välj sedan Bekräfta **för** att bekräfta att företagets information är korrekt och att incitamentsbetalningen ska göras till det CSP-klient-ID som du har valt.
 
      Om statusen visar **Bekräftad** har tilldelningen av CSP-klient-ID:t slutförts och ingen ytterligare åtgärd krävs. Du kan fortfarande välja Bekräftad för att se information om tilldelningen.
   
      I länder som kräver att partner uttryckligen begär att ett skattebefrielse ska tillämpas, finns det ett alternativ för att tillämpa skattebefrielse bredvid skatteprofilen i skatteprofilavsnittet i incitamentprogrammet och platsen för MPN. Om du markera den här rutan tillämpas momsbefrielseförmåner på din anteckning om incitamentkredit. 
   
      För närvarande är betalningsmetoden LRD Credit Note endast tillgänglig för partner i Australien, Nya Zeeland och Kanada för Microsoft Commerce Incentive-programmet. Om du är en partner för direktfakturering eller indirekt leverantör i dessa tre länder som registrerats för MCI-programmet och du inte ser LRD-kreditnotan som tillgänglig betalningsmetod, bekräftar du att ditt klientorganisations-ID är associerat med relevant mpn-platskonto för partner. Mer information om detta finns i [Så här uppdaterar du din organisationsprofil.](update-your-partner-profile.md)

    
5. Välj **Valuta.**

6. När du har slutfört alla betalningsfält väljer du **Skicka**.

## <a name="set-up-a-default-bank-profile"></a>Konfigurera en standardbankprofil

Du kan konfigurera standardbankprofiler och tilldela dem till MPN-platser. Dessa standardprofiler används av Microsoft för efterföljande registreringar för den MPN-platsen. 

1. Logga in på [instrumentpanelen i Partnercenter](https://partner.microsoft.com/dashboard/)och välj sedan kugghjulsikonen för att **öppna Inställningar**   menyn. 

2. Välj **Kontoinställningar**, expandera avsnittet **Utbetalning och** skatt och välj sedan **Utbetalnings- och skatteprofiler.** 

3. Välj **Hantera standardprofiler** under **avsnittet Betalningsprofiler.** 

4. Om du vill skapa en standardbankprofil väljer du **Lägg till en standardbankprofil.** 

5. Välj en bankprofil i listan över tillgängliga bankprofiler för ditt företag, välj den valuta som ska användas med den här bankprofilen och välj sedan listan över MPN-platser som du vill att standardprofilen ska gälla för.

6. Välj **Klar** när du har slutfört valen. Knappen Klar går inte att klicka på förrän alla obligatoriska fält har slutförts. 

>[!NOTE]
>Samma bank- och valutakoppling kan tillämpas på flera platser. Om platsens MPN har tilldelats en standardprofil och valutakombination en gång visas den inte längre i listrutan plats för framtida standardprofiltilldelningar. Om standardvalet tas bort visas platsens MPN igen för framtida standardprofiltilldelningar. Varje bankprofil och valutakombination läggs till som en unik, redigerbar rad.

7. När alla nödvändiga ändringar har lagts till väljer du **Spara.**  

## <a name="create-your-bank-profile"></a>Skapa din bankprofil

Bankprofiler skapas på företagsnivå. Detta gör att en bankprofil kan tilldelas över flera MPN-ID:n och incitamentprogram i ett företag. Det kan finnas undantag när du tillämpar bankprofilen på olika länder, eftersom olika bank- och skatteregler kan tillämpas.

>[!NOTE]
>På följande sidor krävs fält med en asterisk. Om du inte vet vad ett fält är väljer du informationsikonen. 

1. På sidan **Information** fyller du i följande fält: **Profilnamn: Ange ett** unikt namn för att identifiera den här betalningsprofilen.
    **Bankkontoplats:** Det land där företagets bank finns.
    **Betalningsmetod:** Den föredragna betalningsmetoden för Partnercenter är elektronisk banköverföring.

2. Välj **Nästa**.

3. Ange **din information på** sidan Bankkonto. Fält som visas på den här sidan varierar beroende på land. 

4. Välj **Nästa**.

5. Ange **lämplig** information på sidan Förser dig med information. Personen i företaget som banken kontaktar om han/hon behöver diskutera ditt konto.

6. När fälten har slutförts väljer du **Slutför** och sedan Bekräfta **för** att skapa din bankprofil.

Du omdirigeras till sidan **utbetalnings- och skatteprofiler.** Statusen för den nya profilen återspeglar **Väntande Microsoft-validering tills** verifieringen har slutförts. Den här processen kan ta upp till 48 timmar. När verifieringen har slutförts återspeglar din profilstatus antingen **Godkänd eller** Åtgärd **som krävs.** Om **åtgärden krävs** upprepar du stegen ovan och ger nödvändig information. 

## <a name="create-your-tax-profile"></a>Skapa din skatteprofil

Använd följande procedur för att förse Microsoft med den skatteinformation som krävs för din organisation. Sidorna i det här avsnittet är dynamiska och varierar beroende på land eller region. Om du behöver hjälp med att identifiera rätt skatteinformation kontaktar du lämpliga myndighetskällor i ditt land.

Om du behöver information om hur du fyller i W8- eller W9-formulären för partnerföretag i Nord- och Sydamerika tar följande adresser dig till IRS-webbplatsen:

- [http://www.irs.gov/pub/irs-pdf/iw8.pdf](http://www.irs.gov/pub/irs-pdf/iw8.pdf)
- [http://www.irs.gov/pub/irs-pdf/iw9.pdf](http://www.irs.gov/pub/irs-pdf/iw9.pdf)

>[!IMPORTANT]
> Ange endast information för ditt företag. Ange aldrig personlig information.

1. På sidan **Företagsprofil** fyller du i de obligatoriska fälten och väljer **sedan Nästa.** 

2. På **sidan Installation** väljer du det alternativ som gäller för ditt företag.

   - Välj alternativet till vänster om ditt företag ingår endast i USA, eller om profilen är för en enskild person.
   - Välj alternativet till höger om ditt företag ingår utanför USA och välj sedan ditt land/din region i listan.

3. Välj **Nästa**. 

4. På sidan **Skattestatus** anger du nödvändig information och väljer sedan **Nästa.** Fälten på den här sidan varierar beroende på land. din information. 

5. På sidan **Ytterligare dokumentation,** fälten som krävs och välj **Nästa.** 

6. Välj **Bläddra för** att ladda upp dokument som krävs av ditt land eller din region. När dokumentnamnet visas väljer du **Upload**. 

7. Om du behöver ta bort dokumentet väljer du Ta **bort**.

8. Om du vill spara och fortsätta väljer du **Slutför**.

9. Välj **Bekräfta** i popup-meddelandet. Du kommer tillbaka till sidan för **utbetalnings- och skattekonfiguration.**
 
## <a name="update-expired-tax-profiles"></a>Uppdatera skatteprofiler som har upphört att gälla

1. Logga in på [instrumentpanelen i Partnercenter](https://partner.microsoft.com/dashboard/)och välj sedan kugghjulsikonen för att **öppna Inställningar** menyn.

1. Välj **Kontoinställningar,** expandera avsnittet **Utbetalning och** skatt och välj sedan **Utbetalnings- och skatteprofil.**

1. Välj **Skatteprofil**.

1. Kontrollera kolumnen Förfallodatum **och gå** till skatteprofilen som har upphört att gälla eller snart upphör att gälla.

1. Välj **Redigera**.

1. I avsnittet skatteformulär uppdaterar du skatteformulären genom att ange den nya informationen. 

## <a name="next-steps"></a>Nästa steg

- [Vanliga frågor om utbetalning och skatter](payout-faq.yml)
