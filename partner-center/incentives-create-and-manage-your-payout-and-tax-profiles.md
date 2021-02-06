---
title: Utbetalnings- och skatteprofiler i Partnercenter
ms.topic: how-to
ms.date: 11/12/2020
description: Skapa och hantera din utbetalnings-och skatte profil så att du kan betala för dina stimulans arbeten. Inkluderar att skapa, hantera och använda olika profiler.
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
author: Karthic83
ms.author: kashanum
ms.localizationpriority: medium
ms.openlocfilehash: 282fdacc8689ff71e885a2f0ea01ce9570611707
ms.sourcegitcommit: d37a3f353426e52dfbbac577b7576f9c3f6d2ddf
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 02/06/2021
ms.locfileid: "99624246"
---
# <a name="create-and-manage-incentives-payout-and-tax-profiles-in-partner-center"></a>Skapa och hantera incitaments utbetalningar och skatte profiler i Partner Center


**Lämpliga roller:**

- Incitaments administratör
- Kontoadministratör
- Global administratör

Innan du kan erhålla betalningar för dina incitamentprogram för en viss MPN-plats måste du slutföra registreringen genom att associera en giltig utbetalnings- och skatteprofil med programmet och MPN-platsen. Microsoft använder den här utbetalnings- och skatteprofilen för att utfärda betalningar. Eventuellt kan du välja att använda elektronisk banköverföring eller en kreditfaktura för betalningar, beroende på reglerna för incitamentprogrammet. 

## <a name="roles-currencies-and-other-microsoft-programs"></a>Roller, valutor och andra Microsoft-program

Det är viktigt att förstå informationen nedan innan du börjar med din utbetalnings-och skatte profil.

### <a name="roles-and-permissions"></a>Roller och behörigheter

Du måste vara en incitaments administratör för att ange bank-och skatte information för incitaments betalningar. Om du är MPN-/konto administratör kan du tilldela dig själv och/eller en kollega som incitaments administratör.

Kontakta MPN-administratören eller den globala administratören om du behöver begära att be om administratörs behörighet. Du kan ta reda på vem i företaget som har dessa roller genom att logga in på [partner Center-instrumentpanelen](https://partner.microsoft.com/dashboard/). Från **inställnings** ikonen längst upp till höger väljer du **användar hantering** och filtrerar sedan på global administratör.

Incitaments användare kan se incitaments vinster och betalnings information och rapporter, men kan inte redigera bank-och skatte information.

### <a name="choose-your-disbursement-currency"></a>Välj din utbetalnings valuta

Incitaments betalningar görs i den valuta som du valde när du konfigurerade din betalnings profil. Betalningarna beräknas med en växelkurs som ställs in månatlig av Microsoft. Du ansvarar för alla ändringar i värdet på grund av vald valuta.

### <a name="using-different-profiles-for-different-microsoft-programs"></a>Använda olika profiler för olika Microsoft-program

Om ditt företag är registrerat i flera incitaments program kan du använda samma betalnings konto för alla, eller välja att använda olika betalnings konton för olika program.

## <a name="create-and-manage-payout-and-tax-profiles-in-partner-center"></a>Skapa och hantera utbetalnings-och skatte profiler i Partner Center

I avsnitten nedan får du stegvisa anvisningar genom processen att skapa och hantera betalnings-och skatte profiler i Partner Center.

>[!IMPORTANT]
>Du måste vara en incitaments administratör för att skapa eller hantera betalnings profiler i Partner Center. Stimulans roller måste tilldelas till varje MPN-plats under varje incitaments program. Mer information om hur du lägger till stimulans administratörer i Partner Center finns i [skapa användar konton](create-user-accounts-and-set-permissions.md).

## <a name="access-the-payout-and-tax-section-in-partner-center"></a>Gå till avsnittet utbetalnings-och skatte avsnitt i Partner Center

1. Logga in på [partner Center-instrumentpanelen](https://partner.microsoft.com/dashboard/) med ditt Azure Active Directory (Azure AD)-konto (företags konto) eller lämplig e-postadress om ett har tilldelats.

   - Flera domäner kan registreras i ett Azure AD-konto. Kontakta din globala administratör för att avgöra vilka domäner som är associerade.
   - Om du bara kan logga in med @onmicrosoft.com domänen kontaktar du konto administratören för att lägga till ytterligare domäner i Azure AD-kontot.
   - Om du uppmanas att välja **arbets-eller skol konto** eller **personligt konto** väljer du **arbets-eller skol konto**.

2. Välj kugg hjuls ikonen för att öppna menyn **Inställningar** och välj sedan **konto inställningar**.

3. I menyn **konto inställningar** väljer du **utbetalning och skatt**. 

## <a name="assign-payout-and-tax-profiles-to-individual-programs"></a>Tilldela utbetalnings-och skatte profiler till enskilda program

1. Logga in på [partner Center-instrumentpanelen](https://partner.microsoft.com/dashboard/)och välj sedan kugg hjuls ikonen för att öppna menyn **Inställningar** . 

2. Välj **konto inställningar**, expandera **avsnittet utbetalning och skatt** och välj sedan **utbetalning och skatte profil tilldelning**. 
   
   En lista över dina program kommer att visas. Välj pilen bredvid ett program om du vill se profil information. 

3. I list rutan **skatte profil** väljer du den skatte profil du vill använda, eller så väljer du alternativet för att skapa en ny profil. När du väljer alternativet för att skapa en ny profil kommer du att omdirigeras på rätt sätt.  Välj Fortsätt i popup-fönstret. Processen för att skapa en ny skatte profil har angetts nedan.

4. Välj **betalnings sätt**.

   - Om du har valt **elektronisk bank överföring** som betalnings metod väljer du den betalnings profil som du vill använda, eller så väljer du alternativet för att skapa en ny profil. När du väljer alternativet för att skapa en ny profil kommer du att omdirigeras på rätt sätt. Välj Fortsätt i popup-fönstret. Processen för att skapa en ny betalnings profil har angetts nedan.

   - Om du har valt **kredit anteckning** som betalnings metod slutför du verifieringen. Detta bekräftar att det refererade SAP-numret tillhör din organisation.

    >[!NOTE]
    >Om det finns flera Microsoft Business-entiteter i listan måste du välja en betalnings profil för varje entitet.

    >[!NOTE]
    >Tillgängligheten för betalnings metoden är beroende av reglerna i stimulans programmet.
    
5. Välj **valuta**.

6. När du har slutfört alla betalnings fält väljer du **Skicka**.

## <a name="create-your-bank-profile"></a>Skapa din bank profil

Bank profiler skapas på organisations nivå. Detta gör att en bank profil kan tilldelas över flera MPN-ID: n och incitaments program inom en organisation. Det kan finnas undantag när du tillämpar bank profilen på olika länder, eftersom olika bank-och skatte regler kan tillämpas.

>[!NOTE]
>På följande sidor krävs fält med en asterisk. Om du inte vet vad ett fält är väljer du informations ikonen. 

1. På sidan **information** fyller du i följande fält: **profil namn:** ange ett unikt namn för att identifiera betalnings profilen.
    **Bank konto plats:** Det land där ditt företags bank befinner sig.
    **Betalnings metod:** Den prioriterade betalnings metoden för partner Center är elektronisk bank överföring.

2. Välj **Nästa**.

3. Ange din information på sidan **bank konto** . Fälten som visas på den här sidan varierar efter land. 

4. Välj **Nästa**.

5. Ange lämplig information på sidan **mottagare** . Mottagaren är den person i företaget som banken kontaktar om de behöver diskutera ditt konto.

6. När fälten har slutförts väljer du **Slutför** och väljer sedan **Bekräfta** för att skapa din bank profil.

Du omdirigeras till sidan **utbetalnings-och skatte profiler** . Status för din nya profil återspeglar **väntande Microsoft-verifiering** tills verifieringen har slutförts. Den här processen kan ta upp till 48 timmar. När verifieringen har slutförts visas din profil status antingen **godkänd** eller **åtgärd krävs**. Om **åtgärden krävs** upprepar du stegen ovan för att ange den information som krävs. 

## <a name="create-your-tax-profile"></a>Skapa din skatte profil

Använd följande procedur för att förse Microsoft med den skatte information som krävs för din organisation. Sidorna i det här avsnittet är dynamiska och varierar beroende på ditt land eller din region. Om du behöver hjälp med att identifiera rätt skatte information kontaktar du rätt myndighets källor i ditt land.

För partner företag i Amerika, om du behöver information om hur du fyller i W8-eller W9-formulär, tar följande adresser till IRS-webbplatsen:

- [http://www.irs.gov/pub/irs-pdf/iw8.pdf](http://www.irs.gov/pub/irs-pdf/iw8.pdf)
- [http://www.irs.gov/pub/irs-pdf/iw9.pdf](http://www.irs.gov/pub/irs-pdf/iw9.pdf)

>[!IMPORTANT]
> Ange endast information för ditt företag. Ange aldrig personlig information.

1. Fyll i de obligatoriska fälten på sidan **företags profil** och välj sedan **Nästa**. 

2. På sidan **installation** väljer du det alternativ som gäller för ditt företag.

   - Välj alternativet till vänster om ditt företag ingår i endast USA, eller om profilen är för en person.
   - Välj alternativet till höger om ditt företag är införlivat utanför USA och välj sedan land/region i listan.

3. Välj **Nästa**. 

4. Ange den information som krävs på sidan **moms status** och välj sedan **Nästa**. Fälten på den här sidan varierar efter land. din information. 

5. På sidan **Ytterligare dokumentation** , de obligatoriska fälten och välj **Nästa**. 

6. Välj **Bläddra** för att ladda upp dokument som krävs av ditt land eller din region. När dokument namnet visas väljer du **överför**. 

7. Om du behöver ta bort dokumentet väljer du **ta bort**.

8. Välj **Slutför** för att spara och fortsätta.

9. Välj **Bekräfta** i popup-meddelandet. Du kommer tillbaka till sidan för **utbetalning och skatte inställningar** .

## <a name="next-steps"></a>Nästa steg

- [Vanliga frågor om utbetalningar och skatter](payout-faq.md)
