---
title: Skapa kundprenumerationer i Partnercenter
ms.topic: how-to
ms.date: 09/27/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-customers
description: Lär dig hur du säljer prenumerationer till dina kunder för produkter som publicerats av Microsoft samt SaaS-produkter som publicerats av isv:er från tredje part.
author: BillLinzbach
ms.author: BillLi
ms.custom: SEOAPR.20
ms.localizationpriority: medium
ms.openlocfilehash: c42e2e8dbc98bdf9ed0e2994bfb7ad49848aad76
ms.sourcegitcommit: b78e85a0bc62e3536b067417cb3db7899cda4f97
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 10/06/2021
ms.locfileid: "129565339"
---
# <a name="manage-customer-subscriptions"></a>Hantera kundprenumerationer

**Gäller för:** Partner Center | Partnercenter för Microsoft Cloud for US Government

**Lämpliga roller:** Administratörsagent | Faktureringsadministratörskonto | Global | Supportagent | Försäljningsagent

När du har skapat en post för kunden i Partnercenter kan du sälja dem prenumerationer till produkter i katalogen. Detta omfattar produkter som publicerats av Microsoft och SaaS-produkter (Software as a Service) som publicerats av oberoende programvaruleverantörer (ISV) från tredje part på den [kommersiella marknadsplatsen.](https://azuremarketplace.microsoft.com/marketplace)

Vissa erbjudanden är begränsade till en prenumeration per kund. Om du vill se en lista över vilka erbjudanden som är begränsade går du till sidan **Prislistor för** Partnercenter.

> [!IMPORTANT]
> Som partner i CSP-programmet kan du köpa  licensbaserade eller uppmätta SaaS-prenumerationer från **ISV-utgivare** i Partnercenter. Det innebär att du kan köpa alla licensbaserade eller **uppmätta** SaaS-erbjudanden [](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) som **ISV-utgivaren** har gjort tillgängliga för dig, inklusive exklusiva erbjudanden som du har åtkomst till. Om du vill köpa eller hantera andra erbjudanden på den kommersiella marknadsplatsen från ISV:er (till exempel användningsbaserade erbjudanden som rör Azure-program, containrar eller virtuella datorer) måste du [gå till Azure Portal](https://portal.azure.com/).

> [!NOTE]
> Alla datum och tider i Partnercenter anges i utc-tidsstandarden (Universal Time Coordinated). Detta kan skilja sig med upp till 24 timmar från din lokala tid.

## <a name="create-a-new-subscription"></a>Skapa en ny prenumeration

> [!NOTE]
> Mer information om gränssnittet för arbetsytor finns i [Getting around Partner Center (Ta sig runt i Partnercenter).](get-around-partner-center.md#turn-workspaces-on-and-off)

#### <a name="workspaces-view"></a>[Vy över arbetsytor](#tab/workspaces-view)

1. På [instrumentpanelen i Partnercenter](https://partner.microsoft.com/dashboard)väljer **du panelen** Kunder och väljer sedan kunden i listan Kund.

2. Välj **Lägg till prenumeration.** På **fliken Onlinetjänster** visas alla tillgängliga Marketplace SaaS-erbjudanden.

3. Om du bara vill se vissa typer av prenumerationer gör du val i de tillgängliga filtren:
   - **Publisher: Välj** **Microsoft om du** bara vill se erbjudanden från Microsoft eller Partner **för** att se produkter från den kommersiella marknadsplatsen som publicerats av ISV:er.
   - **Faktureringstyp:** Välj den typ av prenumerationsfakturering som du vill använda: **Licens** eller **Användning.** Se [Licensbaserad fakturering för](license-based-billing.md) information som hjälper dig att välja mellan månatlig och årlig faktureringsfrekvens.
   - **Kategori:** Välj **Företag,** **Litet företag** eller **Utvärderingsversion.** Information om utvärderingsprenumerationer finns [i Offer your customers trials of Microsoft products (Erbjuda dina kunder utvärderingsversioner av Microsoft-produkter).](offer-your-customers-trials-of-microsoft-products.md)

4. Välj de produktprenumerationer som du vill köpa för kunden. Vilka produkter du ser beror på typen av kundsegment (utbildning, myndigheter osv.) och de filter som du har tillämpat. Vissa erbjudanden som visas på Marketplace kanske inte alltid är tillgängliga för en specifik kund eller en specifik CSP-partner. Det kan vara så här:
   - Kunden har redan en prenumeration på produkten och tillåts bara en
   - Kundens prenumeration kan ha inaktiverats (i det här fallet kan du återaktivera prenumerationen i stället för att köpa en ny.)
   - För ISV SaaS-erbjudanden kan det finnas några orsaker till varför erbjudandet inte är tillgängligt att köpa: ISV:en kanske inte stöder kundens faktureringsland eller region; ISV:en kan ha valt att inte göra erbjudandet tillgängligt via CSP-programmet, eller så kan ISV:en ha gjort erbjudandet [exklusivt för](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) vissa CSP-partner. ISV-erbjudandet kanske inte heller kan göras via Partnercenter (till exempel containrar eller vissa användningsbaserade erbjudanden).  

5. För varje prenumeration som du vill lägga till anger du antalet licenser (om det behövs) och väljer Lägg **till i kundvagn.**

6. När du är klar med att lägga till prenumerationer väljer **du Granska** och granskar din beställning.

7. När du har granskat dina beställningar och är redo att köpa dessa prenumerationer väljer du **Köp.**

8. När du har köpt en prenumeration för en kund sker följande:

    - Du kan granska eller redigera prenumerationen genom att välja prenumerationsnamnet på kundens **prenumerationssida.** Härifrån kan du välja tilläggslicenser om det finns några, ändra antalet licenser eller pausa prenumerationen.

    **För ISV SaaS-prenumerationer (licensbaserade och uppmätta):**
    - Du får en länk till ISV-utgivarens webbplats. Den här länken hjälper dig att slutföra distributionen eller kontokonfigurationen av kundens prenumeration.

    > [!NOTE]
    > Varken du eller kunden får ett e-postmeddelande med instruktioner för att slutföra kontouppsättningen/etableringen för den här typen av ISV-prenumeration.)

    - Om din prenumeration har en 30-dagars kostnadsfri utvärderingsversion tillämpas den kostnadsfria utvärderingsperioden automatiskt. Som partner i CSP-programmet kan du inte undanta den kostnadsfria utvärderingsperioden för erbjudanden som du köper till kunder. När den kostnadsfria utvärderingsperioden har avslutats börjar prenumerationsperioden och prenumerationen konverteras till betald status. Prenumerationen förnyas sedan automatiskt enligt samma schema.

#### <a name="current-view"></a>[Aktuell vy](#tab/current-view)

1. På [instrumentpanelen i Partnercenter](https://partner.microsoft.com/dashboard) **väljer du** Kunder och sedan kunden i listan Kund.

2. Välj **Lägg till prenumeration.** På **fliken Onlinetjänster** visas alla tillgängliga Marketplace SaaS-erbjudanden.

3. Om du bara vill se vissa typer av prenumerationer gör du val i de tillgängliga filtren:
   - **Publisher: Välj** **Microsoft om du** bara vill se erbjudanden från Microsoft eller Partner **för** att se produkter från den kommersiella marknadsplatsen som publicerats av ISV:er.
   - **Faktureringstyp:** Välj den typ av prenumerationsfakturering som du vill använda: **Licens** eller **Användning.** Se [Licensbaserad fakturering för](license-based-billing.md) information som hjälper dig att välja mellan månatlig och årlig faktureringsfrekvens.
   - **Kategori:** Välj **Företag,** **Litet företag** eller **Utvärderingsversion.** Information om utvärderingsprenumerationer finns [i Offer your customers trials of Microsoft products (Erbjuda dina kunder utvärderingsversioner av Microsoft-produkter).](offer-your-customers-trials-of-microsoft-products.md)

4. Välj de produktprenumerationer som du vill köpa för kunden. Vilka produkter du ser beror på typen av kundsegment (utbildning, myndigheter osv.) och de filter som du har tillämpat. Vissa erbjudanden som visas på Marketplace kanske inte alltid är tillgängliga för en specifik kund eller en specifik CSP-partner. Det kan vara så här:
   - Kunden har redan en prenumeration på produkten och tillåts bara en
   - Kundens prenumeration kan ha inaktiverats (i det här fallet kan du återaktivera prenumerationen i stället för att köpa en ny.)
   - För ISV SaaS-erbjudanden kan det finnas några orsaker till varför erbjudandet inte är tillgängligt att köpa: ISV:en kanske inte stöder kundens faktureringsland eller region; ISV:en kan ha valt att inte göra erbjudandet tillgängligt via CSP-programmet, eller så kan ISV:en ha gjort erbjudandet [exklusivt för](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) vissa CSP-partner. ISV-erbjudandet kanske inte heller kan göras via Partnercenter (till exempel containrar eller vissa användningsbaserade erbjudanden).  

5. För varje prenumeration som du vill lägga till anger du antalet licenser (om det behövs) och väljer Lägg **till i kundvagn.**

6. När du är klar med att lägga till prenumerationer väljer **du Granska** och granskar din beställning.

7. När du har granskat dina beställningar och är redo att köpa dessa prenumerationer väljer du **Köp.**

8. När du har köpt en prenumeration för en kund sker följande:

    - Du kan granska eller redigera prenumerationen genom att välja prenumerationsnamnet på kundens **prenumerationssida.** Härifrån kan du välja tilläggslicenser om det finns några, ändra antalet licenser eller pausa prenumerationen.

    **För ISV SaaS-prenumerationer (licensbaserade och uppmätta):**
    - Du får en länk till ISV-utgivarens webbplats. Den här länken hjälper dig att slutföra distributionen eller kontokonfigurationen av kundens prenumeration.

    > [!NOTE]
    > Varken du eller kunden får ett e-postmeddelande med instruktioner för att slutföra kontouppsättningen/etableringen för den här typen av ISV-prenumeration.)

    - Om din prenumeration har en 30-dagars kostnadsfri utvärderingsversion tillämpas den kostnadsfria utvärderingsperioden automatiskt. Som partner i CSP-programmet kan du inte undanta den kostnadsfria utvärderingsperioden för erbjudanden som du köper till kunder. När den kostnadsfria utvärderingsperioden har avslutats börjar prenumerationsperioden och prenumerationen konverteras till betald status. Prenumerationen förnyas sedan automatiskt enligt samma schema.

* * *

## <a name="update-subscriptions-with-add-ons"></a>Uppdatera prenumerationer med tillägg

För att kunna köpa ett tillägg måste kunden först ha en aktiv basprenumeration.  Det går inte att köpa tillägg via katalogen.

1. Logga in på instrumentpanelen i [Partnercenter.](https://partner.microsoft.com/dashboard)

2. I menyn i Partnercenter väljer **du Kunder** och sedan en kund i listan.

3. Välj den prenumeration som du vill hantera.

4. Under **avsnittet Status** finns en lista över tillgängliga tillägg för prenumerationen.  

5. Uppdatera antalet licenser för varje nödvändigt tillägg. **Skicka** sedan dina ändringar.

Möjligheten att köpa tillägg via Partnercenter är endast tillgänglig för direkta fakturerade och indirekta leverantörer.
Endast berättigade tillägg visas baserat på grundläggande krav och regional tillgänglighet. Mer information om priser och erbjudanden finns i erbjudandematrisen för molnåterförsäljare. Om du avbryter basprenumerationen inaktiveras även eventuella associerade tillägg.

Startdatumen för tillägg följer basprenumerationen och avgifterna beräknas utifrån startdatumet för debitering och slutdatumet för debitering med proportionella avgifter på den första fakturan. Mer information finns i [Licensbaserad fakturering.](license-based-billing.md)


## <a name="suspend-or-cancel-a-subscription"></a>Pausa eller avbryta en prenumeration

Partner kan inaktivera eller avbryta en prenumeration om kunden begär det, eller vid utebliven betalning eller bedrägeri.

### <a name="suspend-a-subscription"></a>Inaktivera en prenumeration

När du ändrar statusen för en prenumeration **till Inaktiverad** kan användarna inte logga in eller komma åt tjänster.

1. Logga in på instrumentpanelen i [Partnercenter.](https://partner.microsoft.com/dashboard)

2. I menyn i Partnercenter väljer **du Kunder** och sedan en kund i listan.

3. Välj den prenumeration som du vill hantera.

4. I avsnittet **Status** väljer du **Tillfälligt avbruten**. **Skicka** sedan dina ändringar.

5. Alla data tas bort om inte prenumerationen återaktiveras inom 90 dagar, eller 90 dagar plus antalet dagar mellan den tidpunkt då kontot öppnades och den första faktureringsperioden (högst 120 dagar).

När du pausar en prenumeration anger  det datum som visas under knappen Pausad när prenumerationen upphör att gälla automatiskt om du inte återaktiverar den. 

> [!NOTE]
> CSP-prenumerationer har inte någon utgången period (så som web-direct-prenumerationer gör) när tjänsterna fortfarande fungerar men prenumerationen genererar inga faktureringsavgifter. CSP-prenumerationer är antingen aktiva eller inaktiverade (eller helt borttagna).

> [!NOTE]
> Nya handelsändringar är för närvarande endast tillgängliga för partner som ingår i den tekniska förhandsversionen av Microsoft 365/Dynamics 365.

Om du vill pausa nya handelsprenumerationer eller återaktivera inaktiverade nya handelsprenumerationer skapar du en tjänstbegäran och kontaktar supporten.


### <a name="cancel-a-subscription"></a>Avbryta en prenumeration

Du kan avbryta licensbaserade SaaS-prenumerationer från tredjeparts-ISV-utgivare på den kommersiella marknadsplatsen [i Partnercenter.](csp-commercial-marketplace-overview.md) Så länge du avbryter inom annulleringsperioden får du en fullständig återbetalning.

För ISV-erbjudanden som faktureras månadsvis:

- Om du avbryter mindre än 24 timmar efter att du har gjort beställningen får du en fullständig kredit på nästa faktura.

- Om du avbryter senare än 24 timmar efter att du har gjort beställningen schemaläggs annulleringen att ske vid förnyelsen.

För erbjudanden som faktureras per år:

- Om du avbryter mindre än 14 dagar efter att du har beställt får du en fullständig kredit på nästa faktura.

- Om du avbryter senare än 14 dagar efter att du har beställt kommer annulleringen att ske vid förnyelsen.

När dessa perioder är över visas inte längre alternativet att avbryta prenumerationen.

> [!NOTE]
> Användningsbaserade och uppmätta ISV-tjänster från tredje part (som till exempel använder virtuella datorer eller containrar) är inte berättigade till retur. Användningsbaserade tjänster kan avetableeras som en annulleringsmetod. Eftersom avgifter debiteras efter användning är dessa tjänster inte berättigade till återbetalning.

Så här avbryter du en licensbaserad SaaS-prenumeration från en ISV-utgivare:

1. Logga in på instrumentpanelen i [Partnercenter.](https://partner.microsoft.com/dashboard)

2. I menyn i Partnercenter väljer **du Kunder** och sedan en kund i listan.

3. Leta upp den prenumeration som du vill avbryta.

4. I kolumnen **Status** väljer du **Avbryt**. **Skicka** sedan dina ändringar.

5. Om en dialogruta visas fyller du i relevant information och väljer sedan **Skicka**.

6. Bekräfta annulleringen genom att välja **Ja, avbryt**.

> [!NOTE]
> Du kan också välja att avbryta en prenumeration Azure Marketplace med hjälp av API:er. Om du vill göra det kan [du läsa Avbryta en Azure Marketplace prenumeration.](/partner-center/develop/cancel-an-azure-marketplace-subscription)

## <a name="suspend-or-cancel-a-new-commerce-subscription"></a>Pausa eller avbryta en ny handelsprenumeration

### <a name="suspend-a-new-commerce-subscription"></a>Pausa en ny handelsprenumeration

> [!NOTE]
> Nya handelsändringar är för närvarande endast tillgängliga för partner som ingår i den tekniska förhandsversionen av Microsoft 365/Dynamics 365.

Vid utebliven betalning från kunden, som ibland kallas "dunningscenario", kan partner pausa och återuppta sin prenumeration för att omedelbart blockera kundens åtkomst till prenumerationens tjänster.

Partner kan pausa och återuppta en prenumeration när som helst utan avbrott. Partnerfakturering fortsätter dock under indragningen. 

Om du pausar kundens prenumerationer inaktiveras möjligheten att logga in och använda deras tjänster tills prenumerationen återupptas. Alla data som rör prenumerationen tas bort om inte prenumerationen återaktiveras inom 90 dagar.

Du kan pausa en prenumeration med hjälp av Partnercenter:

1. Gå till kundens prenumerationssida och välj den prenumeration som du vill pausa.

2. Välj **alternativknappen** Pausa.

3. I popup-dialogrutan väljer du **OK**.

4. Prenumerationen är nu i pausläge och partnern fortsätter att debiteras för prenumerationen.

Pausning kan ångras via Partner Center-användargränssnittet eller API:er som omedelbart återställer en kunds åtkomst till en prenumerations tjänster.

> [!IMPORTANT]
> När du pausar en prenumeration inaktiveras eventuella inställningar för automatisk förnyelse och eventuella befintliga schemalagda ändringar tas bort. Om du pausar en prenumeration påverkas endast kundens tjänståtkomst, och partnerfakturering fortsätter i pausläge.

### <a name="cancel-a-new-commerce-subscription"></a>Avbryta en ny handelsprenumeration

> [!Note] 
> Nya handelsändringar är för närvarande endast tillgängliga för partner som ingår i den tekniska förhandsversionen av Microsoft 365/Dynamics 365.

För nya handelserbjudanden kan partner avbryta sin prenumeration med en beräknad återbetalning inom de **första 72** timmarna för en period **(beräknas per dag).**  

Efter 72 timmar är annulleringen inte längre tillgänglig och partnern debiteras för hela perioden, även om kunden slutar betala för eller använder prenumerationen (gäller för alla faktureringsplan).

När en annullering är klar förlorar kunden omedelbart åtkomst till tjänsten och tjänsten kan inte återställas. Tillståndet för prenumerationen kan inte återställas.  

Om licenser läggs till efter halva tiden gäller samma princip på 72 timmar för eventuell minskning av ytterligare licenser. Minskning av tillagda licenser måste göras via **supportbegäranden.**

## <a name="subscription-renewals"></a>Prenumerationsförnyelse

> [!NOTE]
> Nya handelsändringar är för närvarande endast tillgängliga för partner som ingår i den tekniska förhandsversionen av Microsoft 365/Dynamics 365.

Som standard förnyas prenumerationer automatiskt när prenumerationstiden går ut. För [prenumerationer på kommersiella marknadsplatsprodukter](csp-commercial-marketplace-overview.md)eller nya handelsprenumerationer kan du välja att inte förnya prenumerationen automatiskt.

Så här stoppar du en aktiv prenumeration på den kommersiella marknadsplatsen eller nya handelsprenumerationer från att förnyas automatiskt:

1. Logga in på instrumentpanelen i [Partnercenter.](https://partner.microsoft.com/dashboard)

2. I menyn i Partnercenter väljer **du Kunder** och sedan en kund i listan.

3. Välj **Prenumerationer**. Här visas alla licensbaserade prenumerationer som du har köpt för kunden.

4. I kolumnen **Prenumeration** väljer du den prenumeration som du vill ändra.

5. På sidan med prenumerationsinformation letar du **upp avsnittet Status** och **avmarkerar rutan Förnya** automatiskt.

6. Välj **Skicka**.

### <a name="manage-new-commerce-renewals-with-scheduled-changes"></a>Hantera nya handelsförnyelse med schemalagda ändringar

> [!NOTE]
> Nya handelsändringar är för närvarande endast tillgängliga för partner som ingår i den tekniska förhandsversionen av Microsoft 365/Dynamics 365.

Vissa ändringar i prenumerationer kan bara ske i slutet av en period. Dessa ändringar kan schemaläggas så att de tillämpas praktiskt i slutet av termen. Exempel på ändringar som måste schemaläggas:

- licensminskningar
- Ändringar av faktureringsperiod
- Ändringar av faktureringsfrekvensen

Andra ändringar, till exempel uppgraderingar eller licensökningar, kan tillämpas under perioden.

Schemaändringar sker vid förnyelsen när prenumerationen förnyas för nästa period.

Förutsättningar för schemalagda ändringar:

- Prenumerationen är aktiv 
- Automatisk förnyelse är på
- SKU:n måste vara berättigad till uppgradering

Så här schemalägger du en ny ändring som ska ske vid förnyelse:

1. Logga in på instrumentpanelen i Partnercenter.

2. Välj en **kund** i kundlistan.

3. Välj den prenumeration som du vill hantera.

4. Välj **Hantera förnyelser.**

5. Välj ett annat värdeändring för SKU, kvantitet, period eller faktureringsfrekvens:

   - **Current** är det aktuella värdet för prenumerationen

   - **Ändra** till är det senast sparade värdet som du vill använda vid förnyelsen för den nya prenumerationen

6. Välj **Skicka**.

7. Ändringarna sker vid förnyelsen.

Partner kan komma åt **Hantera förnyelser för** att visa, uppdatera eller ta bort befintlig schemalagd ändring.

> [!NOTE]
> - Som standard konverteras utvärderingsversioner till den betalda motsvarande SKU:n i slutet av utvärderingsperioden.
> - Om licenskvantiteten inte ändras för schemalagda SKU-uppgraderingar sker omtilldeling av användarlicensen automatiskt. Annars måste den göras manuellt.
> - Sparade schemalagda ändringar tas bort om halvårsuppdateringar görs i prenumerationen.

Sparade schemalagda ändringar tas bort när följande ändringar efter halva tiden görs:  

- Automatisk förnyelse är inaktiverat 
- Antalet har ändrats 
- Prenumerationen har avbrutits 
- SKU har uppgraderats 
- Utvärderingsversionen konverteras 

## <a name="upgrades-in-new-commerce-subscriptions"></a>Uppgraderingar i nya handelsprenumerationer

För ny handel innebär uppgradering att gå från en betald prenumeration till en annan betald prenumeration. Med nya uppgraderingar som betalas via köp kan kunden omedelbart uppgradera från sin aktuella SKU till en med tillagda tjänster. 

Partner kan välja vilken prenumeration de vill uppgradera till när de konfigurerar licensantal. Partner kan välja **en Ny** prenumeration eller välja **en Befintlig** prenumeration om den är berättigad till uppgraderingen. 

Uppgraderingar kan vara av två typer: **fullständig uppgradering** och **partiell uppgradering.**

> [!NOTE]
> - Uppgraderingar kan schemaläggas att ske i slutet av en period eller kan initieras på medel sikt.
> - När du initierar en mellantidsuppgradering tas befintliga schemalagda uppgraderingar bort.
> - Uppgraderingar kan bara initieras från prenumerationer i **aktivt** tillstånd.

### <a name="full-upgrades"></a>Fullständiga uppgraderingar

En fullständig uppgradering är en uppgradering på plats, vilket innebär att alla eller flera licenser uppgraderas. I det här fallet förblir prenumerations-ID:t detsamma och licenserna tilldelas automatiskt. Men om kunden redan har köpt mål-SKU:n från en annan partner eller kanal över äldre, krävs manuell tilldelning. Om manuell tilldelning krävs visas ett varningsmeddelande i Partnercenter om att licenserna måste tilldelas manuellt. 

### <a name="partial-upgrades"></a>Partiella uppgraderingar

Partiella uppgraderingar gör det möjligt för en partner att utse vissa licenser från en SKU till en annan. Tidigare uppgraderingsfunktioner i traditionella licensbaserade prenumerationer aktiverade endast uppgradering av alla licenser. Med ny handel kan en partner flytta vissa licenser när det passar dem. Detta ger partnern mer kontroll över hanteringen av uppgraderingar, så att de kan flytta vissa användare till en ny SKU utan att flytta alla.

Information om partiell uppgradering:

- Definieras som partiellt om uppgraderingslicensantalet är mindre än det ursprungliga prenumerationsantalet.
- En ny prenumeration som skapas vid delvis uppgradering har samma slutdatum som prenumerationen som uppgraderingen kommer från.

## <a name="increasing-and-reducing-licenses-in-new-commerce-subscriptions"></a>Öka och minska licenser i nya handelsprenumerationer

Licensantalet för en prenumeration kan **ökas** när som helst, och faktureringsjusteringar visas på nästa faktura och avstämningsfil. 

Licensantalet för en prenumeration kan **minskas:**
- endast inom de första 72 timmarna efter det att prenumerationsbeställningen **först gjordes eller förnyades.** 
- via kundsupport inom 72 timmar för licenser som **lagts till efter halva tiden**

En minskning av licensantalet inom de första 72 timmarna av en prenumerationsperiod (efter det första köpet eller förnyelsen) kan göras via självbetjäning i Partnercenter eller via API:et.

En minskning av licensantalet för licenser som läggs till efter halva tiden kan bara göras via kundsupport inom de första 72 timmarna.

I båda fallen av licensminskning återbetalas hela beloppet **minus det beräknade** beloppet under de dagar som du använde prenumerationen   **(beräknas per dag).** 

Om **mer än 72** timmar har gått sedan prenumerationsbeställningen gjordes  eller ytterligare licenser lades till kan licensantalet inte minskas förrän nästa annulleringsperiod vid förnyelsen.

## <a name="switching-billing-plans"></a>Växla faktureringsplaner

Partner har flexibiliteten att växla sin faktureringsplan och faktureringsperiod tillsammans. De kan också välja att bara byta faktureringsplan efter halva tiden, utan att återställa faktureringsperioden helt och hållet.

### <a name="just-changing-billing-frequency-scheduled-change"></a>Bara att ändra faktureringsfrekvens (schemalagd ändring)

Partner kan bara ändra faktureringsplanen via Partnercenter i några få steg, vilket börjar gälla i nästa faktureringsperiod:

1. Gå till kundens prenumerationssida och välj den prenumeration som du vill ändra.

2. Välj länken **Hantera faktureringsfrekvens.**

3. En sidopanel öppnas som visar den aktuella faktureringsfrekvensen och en listrutan som innehåller alternativen för att ändra frekvensen till.

4. När ett nytt värde har valts sker de nya faktureringsändringarna i **nästa faktureringsperiod** (INTE en omedelbar ändring).

### <a name="changing-billing-frequency-along-with-billing-term-and-other-fields-immediate-change"></a>Ändra faktureringsfrekvens tillsammans med faktureringsperiod och andra fält (omedelbar ändring)

Partner kan även ändra faktureringsfrekvensen tillsammans med faktureringsperioden och andra fält via Partnercenter, vilket utlöser en omedelbar ändring:

1. Gå till kundens prenumerationssida och välj den prenumeration som du vill ändra.

2. Ändra termens varaktighet genom att välja ett alternativ i listrutan. Då öppnas en annan listrutan för att ändra faktureringsfrekvens.

3. Välj en annan faktureringsfrekvens i listrutan.

4. När du har gjort ändringarna och klickat på Skicka sker de nya faktureringsändringarna **omedelbart**.

## <a name="next-steps"></a>Nästa steg

- [Köpa produkter på den kommersiella marknadsplatsen för dina kunder](csp-commercial-marketplace-purchase.md)

- [Hantera produkter på den kommersiella marknadsplatsen för dina kunder](csp-commercial-marketplace-manage.md)

- [Översikt över kommersiell marknadsplats](csp-commercial-marketplace-overview.md)
