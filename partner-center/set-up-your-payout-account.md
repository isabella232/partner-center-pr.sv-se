---
title: Konfigurera utbetalnings- och skatteprofiler på den kommersiella marknadsplatsen
description: Om du vill få pengar från erbjudandeförsäljningen på den kommersiella marknadsplatsen kan du läsa om hur du ställer in ditt utbetalningskonto och fyller i de skatteformulär som krävs.
ms.topic: conceptual
ms.service: partner-dashboard
ms.subservice: partnercenter-payouts
author: mingshen-ms
ms.author: mingshen
ms.date: 09/27/2021
ms.openlocfilehash: 8b29cd1d80947991c8dca95c45d682734cb0c173
ms.sourcegitcommit: b35ed0a247c3316d2f1a4e9664f4a21f6e713650
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 10/07/2021
ms.locfileid: "129663401"
---
# <a name="set-up-commercial-marketplace-payout-and-tax-profiles"></a>Konfigurera utbetalnings- och skatteprofiler på den kommersiella marknadsplatsen

**Lämpliga roller:** Kontoadministratörsroller | Global administratör

För att kunna ta emot pengar från erbjudandeförsäljning på den kommersiella marknadsplatsen måste du konfigurera ditt utbetalningskonto och fylla i de nödvändiga skatteformulären i [Partnercenter.](https://partner.microsoft.com/dashboard)

Om du bara planerar att lista kostnadsfria erbjudanden (och inte planerar att erbjuda köp i appen eller använda Microsoft Advertising) behöver du inte konfigurera ett utbetalningskonto eller fylla i några skatteformulär. Om du ändrar dig senare och bestämmer dig för att sälja erbjudanden (eller tillägg) kan du konfigurera ditt utbetalningskonto och fylla i skatteformulär vid den tidpunkten. Du kommer inte att kunna skicka några betalda erbjudanden eller tillägg förrän ditt utbetalningskonto och din skatteprofil har slutförts.

> [!NOTE]
> På vissa marknader kan utgivare endast skicka in kostnadsfria erbjudanden. Om ditt konto är registrerat på någon av dessa marknader har du inte möjlighet att konfigurera ett utbetalningskonto.

När du har ställt in ditt konto finns det två saker du behöver göra innan du kan sälja erbjudandet (eller tillägg) på den kommersiella marknadsplatsen:

- [Fyll i skatteformulär](#tax-forms)
- [Konfigurera ditt utbetalningskonto](#payout-account)

> [!NOTE]
> Mer information om hur och när du får betalt för de pengar som ditt erbjudande tjänar finns i [Få betalt på den kommersiella marknadsplatsen.](marketplace-get-paid.md)

## <a name="tax-forms"></a>Skatteformulär

Du hanterar din skatteprofil och skatteformulär på sidan **Utbetalning och** skatt i Partnercenter. Din organisations behörigheter avgör vilka profiler och vilken information du ser.

### <a name="create-or-update-your-tax-profile"></a>Skapa eller uppdatera din skatteprofil

Först måste du skapa en skatteprofil och tilldela den till de program som du deltar i. Använd följande steg för att skapa eller uppdatera din *skatteprofil* i Partnercenter. Du kan fylla i och skicka skatteformulär elektroniskt på instrumentpanelen i Partnercenter. I de flesta fall behöver du inte skriva ut och skicka några formulär via e-post.

> [!IMPORTANT]
> Olika länder och regioner har olika skattekrav. Exakt hur mycket du måste betala i skatt beror på vilka länder och regioner där du säljer ditt erbjudande. Se Microsoft Azure [Marketplace Publisher för](/legal/marketplace/msft-publisher-agreement) att ta reda på vilka länder/regioner Microsoft erbjuder försäljning och använder skatt för din räkning. I andra länder/regioner kan du, beroende på var du är registrerad, behöva överföra försäljning och använda skatt för din erbjudandeförsäljning direkt till den lokala skatteutfärdaren. Dessutom kan appförsäljningen som du får vara momsbar som inkomst. Vi rekommenderar starkt att du kontaktar relevant myndighet för ditt land eller din region och som på bästa sätt kan hjälpa dig att fastställa rätt skatteinformation för dina aktiviteter på den kommersiella marknadsplatsen.

1. Logga in på [instrumentpanelen i Partnercenter,](https://partner.microsoft.com/dashboard)välj Inställningar kugghjulsikon och välj **sedan Kontoinställningar.**

2. Välj **Utbetalning och skatt** och välj sedan **Utbetalnings- och skattetilldelningar.**

3. Välj den kombination av program- och säljar-ID som du vill konfigurera skatteinformation för.

4. Om du vill använda en befintlig skatteprofil väljer du den i listrutan. Annars väljer du **Skapa ny profil och** trycker på **Skicka**. Du kommer till sidan skatteprofiler.

5. Välj knappen **Redigera** för att redigera din skatteinformation.

6. Välj lämplig alternativknapp och välj land/region om du uppmanas att göra det. Det här steget avgör vilken Microsoft-affärsenhet som ska användas för att göra utbetalning på ditt konto.

7. Beroende på dina val i steg 6 uppmanas du att ange den skatteinformation som krävs för ditt land/din region.

   > [!NOTE]
   > Oavsett vilket land/region du har när det gäller hem eller moms måste du fylla i USA skatteformulär för att sälja ett erbjudande eller tillägg via den kommersiella marknadsplatsen. Utgivare som uppfyller vissa krav USA måste fylla i ett IRS W-9-formulär. Andra utgivare utanför USA fylla i ett IRS W-8-formulär. Du kan fylla i dessa formulär online när du fyller i din skatteprofil.

### <a name="withholding-rates"></a>Källskattefrekvens

Den information som du skickar i dina skatteformulär avgör lämplig källskatt. Källpriset gäller endast för försäljning som du gör i USA; försäljning som görs till icke-amerikanska platser omfattas inte av källskatt. Källskattefrekvensen varierar, men för de flesta utgivare som registrerar sig utanför USA är standardfrekvensen 30 %. Du kan välja att minska den här frekvensen om ditt land/din region har samtyckt till en inkomstskatt med USA.

### <a name="tax-treaty-benefits"></a>Förmåner vid skatteförmåner

Om du är utanför USA kan du eventuellt dra nytta av skatteförmåner. Dessa förmåner varierar från land/region till land/region och kan göra att du kan minska den mängd skatter som den kommersiella marknadsplatsen innehåller. Du kan begära skatteförmåner genom att fylla i del II av W-8BEN-formuläret. Vi rekommenderar att du kommunicerar med lämpliga resurser i ditt land eller din region för att avgöra om dessa förmåner gäller för dig.

> [!NOTE]
> Ett USA individuellt identifieringsnummer (eller ITIN) behöver inte ta emot betalningar från Microsoft eller kräva skatteförmåner.

## <a name="payout-account"></a>Utbetalningskonto

Ett utbetalningskonto är det bankkonto som vi skickar intäkter från din försäljning till. Du kan visa alla betalningskonton som du har angett på profilsidan.

> [!NOTE]
> På vissa marknader kan PayPal användas för ditt utbetalningskonto. Mer information PayPal information om hur du PayPal för en viss marknad finns i [Tröskelvärden,](payment-thresholds-methods-timeframes.md) metoder och tidsramar för betalning och PayPal [information](#paypal-information) nedan.

### <a name="create-a-payment-profile"></a>Skapa en betalningsprofil

1. Logga in på [instrumentpanelen i Partnercenter,](https://partner.microsoft.com/dashboard) **välj Inställningar** kugghjulsikon och välj **sedan Kontoinställningar.**

2. Under rubriken *Utbetalning och skatt väljer* du **Utbetalnings- och skatteprofiltilldelning**.

    > [!NOTE]
    > Eftersom det här är känslig information kan du uppmanas att logga in igen.

3. Välj den betalningsmetod som du vill konfigurera.

4. Välj en befintlig betalningsprofil eller välj Skapa **en ny betalningsprofil för** att skapa en ny profil för den valda betalningsmetoden.

### <a name="create-a-bank-based-payment-profile"></a>Skapa en bankbaserad betalningsprofil

Om du valde att använda ett bankkonto för att få utbetalning slutför du följande process för att konfigurera ditt bankkonto.

1. På sidan *Bankprofil* anger du nödvändig information om din bank.

2. Ange information om ditt bankkonto.

    > [!NOTE]
    > De fält som du använder för att ange din kontoinformation accepterar endast alfanumeriska tecken.

3. Ange detaljerad information.

4. När du är *tillbaka på sidan* Profiltilldelning väljer du den valuta som du vill att vi ska använda när vi utfärdar dina utbetalningar.

    > [!WARNING]
    > Se till att din bank accepterar utbetalningsvalutan som du väljer.

5. Du måste välja en betalningsprofil för varje program som du deltar i, men du kan använda samma profil för flera program.

6. Välj Skicka för att spara ändringarna.

   > [!NOTE]
   > Microsoft kan ta upp till 48 timmar att verifiera informationen i din profil. När den här processen är *klar visas verifieringsstatusen* **Slutförd**

För att säkerställa att utbetalningen lyckas ser du till att:

- Namnet **på kontoinnehavaren** som anges för ditt utbetalningskonto i Partnercenter måste vara exakt samma namn som är associerat med ditt bankkonto. Om ditt bankkontonamn till exempel innehåller ett mellannamn lägger du till ett mellannamn i namnet **på kontoinnehavaren.**
- Utbetalningar överförs direkt från Microsoft till ditt bankkonto i USD-valuta.
- Bankinformation som anges i Partner Center med latinska tecken översätts till kyrilliska tecken.

### <a name="editing-existing-payment-profiles"></a>Redigera befintliga betalningsprofiler

Du kan redigera befintliga betalningsprofiler om du behöver göra ändringar eller korrigera felaktig information.

1. Logga in på [instrumentpanelen i Partnercenter,](https://partner.microsoft.com/dashboard) **välj Inställningar** kugghjulsikon och välj **sedan Kontoinställningar.**

2. Under rubriken *Utbetalning och skatt väljer* du **Utbetalnings- och skatteprofiler**.

3. Dina betalningsprofiler visas tillsammans med deras status. Hitta den profil som du vill redigera och **välj Redigera** längst till höger

> [!IMPORTANT]
> Om du ändrar ditt utbetalningskonto kan du fördröja dina betalningar med upp till en betalningscykel. Den här fördröjningen beror på att vi behöver verifiera kontoändringen, precis som vi gjorde när du först konfigurerade utbetalningskontot. Du får fortfarande betalt för hela beloppet när ditt konto har verifierats. eventuella betalningar som förfaller för den aktuella betalningscykeln läggs till i nästa. Mer [information finns i Få betalt på](marketplace-get-paid.md)den kommersiella marknadsplatsen.

### <a name="paypal-information"></a>PayPal information

I utvalda länder och regioner kan du skapa ett betalningskonto genom att ange PayPal information. Men innan du väljer PayPal som ett betalningsalternativ:

- Kontrollera [Tröskelvärden, metoder och](payment-thresholds-methods-timeframes.md) tidsramar för betalning för att PayPal är en betalningsmetod som stöds i ditt land eller din region.
- Läs följande vanliga frågor och svar. Beroende på din situation PayPal kanske inte det bästa alternativet för ditt konto, och ett bankkonto kan vara att föredra.

Vanliga frågor om PayPal som betalningsmetod:

- **Vilka PayPal inställningar måste jag ha för att kunna ta emot betalningar?** Kontrollera att ditt PayPal inte blockerar eCheck-betalningar. Den här inställningen hanteras PayPal på sidan Betalningstagandeinställningar. Mer [PayPal finns på PayPal](https://go.microsoft.com/fwlink/?linkid=2162542) sidan för kontokonfiguration.

- **Stöds mitt land/min region?** Se [Betalningströsklar, metoder och tidsramar för](payment-thresholds-methods-timeframes.md) att ta reda på PayPal är en betalningsmetod som stöds.

- **Måste mitt PayPal vara registrerat i samma land/region som mitt Partnercenter-konto?** Nej. När du ställer in ett PayPal-konto kan du acceptera standardkonfigurationen. Du bör inte ha några problem med andra länder/regioner och valutor om du inte har blockerat betalningen i vissa valutor. Den här inställningen hanteras PayPal på sidan Betalningstagandeinställningar.

- **Måste jag acceptera PayPal betalningar manuellt?** Nej. PayPal är som standard inställda på att kräva att användarna accepterar betalningar manuellt, vilket innebär att om du inte accepterar betalningen inom 30 dagar returneras den. Du kan ändra den här inställningen genom att stänga av "Fråga mig" PayPal sidan Mer Inställningar fråga.

- **Vilka valutor har PayPal stöd för?** Se [PayPal supportsidan för](https://developer.paypal.com/docs/classic/api/currency-codes/#paypal) den aktuella listan

### <a name="specific-requirements-for-certain-countriesregions"></a>Särskilda krav för vissa länder/regioner

I vissa länder och regioner måste ytterligare krav för utbetalningskonton följas. Observera följande krav om du är hemmahörande i Gränsen, Ryssland eller På vilket sätt du vill.

#### <a name="pakistan"></a>Pakistan

Form-R är ett regelkrav för Bankväsende. Den används för att ange syfte och orsak till att ta emot pengar från en 10-åring. När du är berättigad till en månatlig utbetalning från Microsoft måste du därför skicka ett formulär R till din bank innan utbetalningen kan släppas på ditt konto. Kontakta din lokala bankavdelning för instruktioner om hur du hämtar en kopia av Form-R.

Du måste skicka ett formulär-R till din bank varje månad som du är berättigad till en utbetalning. Om du till exempel förväntar dig att få en utbetalning varje månad på året måste du skicka en Form-R 12 gånger (en gång i månaden).

När utbetalningen har skickats till din bank har du 30 dagar på dig att skicka ett Formulär-R. Om den inte skickas inom 30 dagar returneras medel till Microsoft.

#### <a name="russia"></a>Ryssland

Om du är utgivare och bor i Ryssland kan du behöva uppge dokumentation till din bank innan din bank sätter in pengar på ditt konto. När du är berättigad till betalning ger vi dig följande dokumentation i ett e-postmeddelande:

- Godkännandecertifikat (AC) – innehåller den mängd utbetalning som överförs till ditt konto.
- [Microsoft Azure Marketplace Publisher –](/legal/marketplace/msft-publisher-agreement) en signerad kopia av utgivaravtalet som måste motskrivas.

För att säkerställa att utbetalningen lyckas ser du till att:

- **Kontoinnehavarens namn som** anges för ditt utbetalningskonto i Partnercenter måste vara exakt samma namn som är associerat med ditt bankkonto. Om ditt bankkontonamn till exempel innehåller ett mellannamn lägger du till ett mellannamn i namnet **på kontoinnehavaren.**
- Utbetalningar överförs direkt från Microsoft till ditt bankkonto i en valuta som du betalar för.
- Bankinformation som anges i Partner Center med latinska tecken översätts till kyrilliska tecken.
- Utbetalningar måste göras till ett bankkonto och inte till ett bankkort.

#### <a name="ukraine"></a>Ukraina

Om du är en utgivare som bor i Påse kan du behöva tillhandahålla dokumentation till din bank innan din bank sätter in pengar på ditt konto. När du är berättigad till betalning ger vi dig följande dokumentation i ett e-postmeddelande:

- Godkännandecertifikat (AC) – innehåller den mängd utbetalning som överförs till ditt konto.
- [Microsoft Azure Marketplace Publisher –](/legal/marketplace/msft-publisher-agreement) en signerad kopia av utgivaravtalet som måste motskrivas.
- Ändringsavtal (AA) – det här dokumentet kan användas av din bank för att identifiera dina utbetalningsmedel.

Microsoft tillhandahåller alla tre dokumenten när din första utbetalningsförsök görs. För efterföljande utbetalningar får du endast AC-dokumentet. Behåll ADA- och AA-dokumenten om du behöver dem för att få framtida utbetalning från din bank.

### <a name="create-a-paypal-payment-profile"></a>Skapa en PayPal-betalningsprofil

Om du valde att använda ett bankkonto för att få utbetalning slutför du följande process för att konfigurera ditt bankkonto.

1. På sidan **PayPal** anger du nödvändig information om ditt PayPal konto.

2. Ange din PayPal kontoinformation.

    > [!NOTE]
    > De fält som du använder för att ange din kontoinformation accepterar endast alfanumeriska tecken.

3. Ange detaljerad information.
 
4. På sidan **Profiltilldelning** väljer du den valuta som du vill att vi ska använda när vi utfärdar dina utbetalningar.
 
5. Du måste välja en betalningsprofil för varje program som du deltar i, men du kan använda samma profil för flera program.

6. Välj **Skicka** för att spara ändringarna.

## <a name="next-steps"></a>Nästa steg

[Få betalt på den kommersiella marknadsplatsen](marketplace-get-paid.md)
