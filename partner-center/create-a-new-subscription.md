---
title: Skapa kund prenumerationer i Partner Center
ms.topic: how-to
ms.date: 07/22/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 'Lär dig hur du säljer dina kund prenumerationer till produkter som publicerats av Microsoft samt SaaS-produkter som publicerats av tredjeparts-ISV: er.'
author: BillLinzbach
ms.author: BillLi
ms.custom: SEOAPR.20
ms.localizationpriority: medium
ms.openlocfilehash: 8c3cfc2a6576029a8fdfb902a7b3889b4ea6c628
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/22/2020
ms.locfileid: "92531692"
---
# <a name="create-suspend-or-cancel-customer-subscriptions"></a>Skapa, pausa eller avbryta kundprenumerationer

**Gäller för**

- Partnercenter
- Partner Center för Microsoft Cloud för amerikanska myndigheter
- CSP-partner

**Lämpliga roller**

- Administratörs agent
- Faktureringsadministratör
- Global administratör
- Support agent
- Försäljnings agent

När du har skapat en post för din kund i Partner Center kan du sälja prenumerationer till produkter i katalogen. Detta inkluderar produkter som publicerats av Microsoft samt SaaS-produkter (program vara som en tjänst) som publicerats av oberoende program varu leverantörer från tredje part till den [kommersiella marknads platsen](https://azuremarketplace.microsoft.com/marketplace).

Vissa erbjudanden är begränsade till en prenumeration per kund. Om du vill se en lista över vilka erbjudanden som är begränsade besöker du sidan priser och erbjudanden för partner Center.

> [!IMPORTANT]
> Som partner i CSP-programmet kan du bara köpa **licensbaserade** SaaS-prenumerationer från ISV-utgivare i Partner Center. Det innebär att du kan köpa alla **licensbaserade** SaaS-erbjudanden som ISV-utgivare har gjort tillgängligt för dig, inklusive [exklusiva erbjudanden](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) som du har åtkomst till. För att köpa eller hantera andra erbjudanden från kommersiell marknads plats från ISV: er (till exempel **användnings** , avgiftsbelagda eller konsumtions erbjudanden som rör Azure-program, behållare eller virtuella datorer) måste du gå till [Azure-hanteringsportalen](https://portal.azure.com/). Mer information finns i [köpa kommersiella Marketplace-produkter](csp-commercial-marketplace-purchase.md).

## <a name="create-a-new-subscription"></a>Skapa en ny prenumeration

1. Logga in på [instrumentpanelen i Partnercenter](https://partner.microsoft.com/dashboard).

2. Från menyn Partner Center väljer du **kunder** och väljer sedan en kund i listan.

3. Välj **Lägg till prenumeration** . På fliken **online tjänster** visas alla tillgängliga Marketplace SaaS-erbjudanden.

4. Om du bara vill se vissa typer av prenumerationer gör du inställningarna i de tillgängliga filtren:
   - **Utgivare** : Välj **Microsoft** om du bara vill se erbjudanden från Microsoft eller **partner** för att se produkter för kommersiella Marketplace som publicerats av ISV: er.
   - **Fakturerings typ** : Välj den typ av prenumerations fakturering som du vill använda: **licens** eller **användning** . Se [licensbaserade fakturerings](license-based-billing.md) information som hjälper dig att välja mellan månads-och års fakturerings frekvens.
   - **Kategori** : Välj **företag** , **små företag** eller **utvärderings version** . Information om utvärderings prenumerationer finns i [erbjuda dina kunders utvärdering av Microsoft-produkter](offer-your-customers-trials-of-microsoft-products.md).

5. Välj de produkt prenumerationer som du vill köpa för kunden. Vilka produkter som visas beror på typen av kund segment (utbildning, myndigheter osv.) och de filter som du har tillämpat. Vissa erbjudanden som visas på Marketplace kanske inte alltid är tillgängliga för en viss kund eller en specifik CSP-partner. Detta kan bero på att:

   - Kunden har redan en prenumeration på produkten och är bara tillåten en

   - Kundens prenumeration kan ha inaktiverats (i det här fallet kan du återaktivera prenumerationen i stället för att köpa en ny.)

   - För ISV SaaS-erbjudanden kan det finnas några skäl till varför erbjudandet inte kan köpas: ISV kanske inte har stöd för kundens fakturerings land eller region. ISV: n kanske har valt att inte göra erbjudandet tillgängligt via CSP-programmet. eller så kan ISV: n ha gjort erbjudandet [exklusivt](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) för vissa CSP-partner. Det går inte heller att använda ISV-erbjudandet via partner Center (till exempel behållare eller vissa användnings erbjudanden).  

6. Ange antalet licenser (om det behövs) för varje prenumeration som du vill lägga till och välj **Lägg till i kundvagn** .

7. När du har lagt till prenumerationerna väljer du **Granska** och granska din beställning.

8. När du har granskat dina beställningar och är redo att köpa dessa prenumerationer väljer du **köp** .

9. När du har köpt en prenumeration för en kund görs följande:

    - Du kan granska eller redigera prenumerationen genom att välja prenumerations namnet från kund **prenumerations** sidan. Härifrån kan du välja tilläggs licenser om de är tillgängliga, ändra antalet licenser eller pausa prenumerationen.

    **För ISV SaaS (licensbaserade) prenumerationer:**
    - Du får en länk till ISV-utgivarens webbplats. Den här länken bör hjälpa dig att slutföra distributions-eller konto konfigurationen för kundens prenumeration.
      
    >[!NOTE]
    > Varken du eller din kund får ett e-postmeddelande med instruktioner för att slutföra konto konfigurationen/etableringen för den här typen av ISV-prenumeration.)

    - Om din prenumeration kommer med en 30-dagars kostnads fri utvärderings period, kommer den kostnads fria utvärderings perioden att tillämpas automatiskt. Som partner i CSP-programmet kan du inte avstå från den kostnads fria utvärderings perioden på erbjudanden som du köper för kunder. När den kostnads fria utvärderings perioden är slut börjar prenumerations perioden och prenumerationen kommer att konverteras till betald status. Prenumerationen förnyas då automatiskt enligt samma schema.
   
## <a name="update-subscriptions-with-add-ons"></a>Uppdatera prenumerationer med tillägg 

För att kunna köpa ett tillägg måste kunden först ha en aktiv basprenumeration.  Det går inte att köpa tillägg via katalogen.

1. Logga in på [instrument panelen](https://partner.microsoft.com/dashboard)för partner Center.

2. Från menyn Partner Center väljer du **kunder** och väljer sedan en kund i listan.

3. Välj den prenumeration som du vill hantera.

4. Under avsnittet **status** finns en lista över tillgängliga tilläggs komponenter för prenumerationen.  

5. Uppdatera antalet licenser för varje nödvändigt tillägg. **Skicka** sedan dina ändringar.

Möjligheten att köpa tillägg via partner Center är bara tillgänglig för direkta fakturerings-och indirekta leverantörer.
Endast kvalificerade tillägg visas baserat på grundläggande krav och regional tillgänglighet. I erbjudandematrisen för molnåterförsäljare finns mer information om priser och erbjudanden.  Om du avbryter basprenumerationen inaktiveras även eventuella associerade tillägg.

Startdatumen för tillägg följer basprenumerationen och avgifterna beräknas utifrån startdatumet för debitering och slutdatumet för debitering med proportionella avgifter på den första fakturan. Mer information finns i [licensbaserade fakturering](license-based-billing.md).


## <a name="suspend-or-cancel-a-subscription"></a>Pausa eller avbryta en prenumeration

Partner kan pausa eller avbryta en prenumeration om det begärs av kunden, eller i fall av inbetalning eller bedrägerier.

### <a name="suspend-a-subscription"></a>Pausa en prenumeration

När du ändrar status för en prenumeration till **inaktive** rad kan användarna inte logga in eller komma åt tjänster.

1. Logga in på [instrument panelen](https://partner.microsoft.com/dashboard)för partner Center.

2. Från menyn Partner Center väljer du **kunder** och väljer sedan en kund i listan.

3. Välj den prenumeration som du vill hantera.

4. I avsnittet **Status** väljer du **Tillfälligt avbruten** . **Skicka** sedan dina ändringar.

5. Alla data tas bort om inte prenumerationen återaktiveras inom 90 dagar, eller 90 dagar plus antalet dagar mellan den tidpunkt då kontot öppnades och den första fakturerings perioden (maximalt 120 dagar).

När du pausar en prenumeration visar datumet som visas under den **nedbrutna** knappen när prenumerationen upphör att gälla automatiskt om du inte återaktiverar den. 

### <a name="cancel-a-subscription"></a>Avbryta en prenumeration

Du kan välja att avbryta licensbaserade SaaS-prenumerationer från tredjeparts ISV-utgivare i Partner Center [handels Marketplace](csp-commercial-marketplace-overview.md). Så länge som du avbryter inom uppsägnings perioden får du en fullständig åter betalning.

För ISV-erbjudanden faktureras månads vis:

- Om du avbryter mindre än 24 timmar efter att du har placerat beställningen får du en fullständig kredit på nästa faktura.

- Om du avbryter senare än 24 timmar efter att du har placerat ordern schemaläggs annulleringen till att ske vid förnyelse.

För fakturerade per år:

- Om du avbryter mindre än 14 dagar efter att du har placerat beställningen får du en fullständig kredit på nästa faktura.

- Om du avbryter senare än 14 dagar efter att du har placerat ordern schemaläggs annulleringen till att ske vid förnyelse.

När dessa perioder är över visas inte längre alternativet för att avbryta prenumerationen.

> [!NOTE]
> Användnings och avgiftsbelagda ISV-tjänster (som använder virtuella datorer eller behållare, till exempel) är inte tillgängliga för retur. Användnings tjänster kan avetableras som en avbrotts metod. Eftersom avgifter faktureras efter användningen är dessa tjänster inte berättigade till åter betalning.

Så här avbryter du en licensbaserad SaaS-prenumeration från en ISV-utgivare:

1. Logga in på [instrument panelen](https://partner.microsoft.com/dashboard)för partner Center.

2. Från menyn Partner Center väljer du **kunder** och väljer sedan en kund i listan.

3. Leta upp den prenumeration som du vill avbryta.

4. I kolumnen **status** väljer du **Avbryt** . **Skicka** sedan dina ändringar.

5. Om en dialog ruta visas, Fyll i all relevant information och välj sedan **Skicka** .

6. Bekräfta annulleringen genom att välja **Ja, Avbryt** .

> [!NOTE]
> Du kan också välja att avbryta en Azure Marketplace-prenumeration med hjälp av API: er. För att göra det, se [avbryta en prenumeration på Azure Marketplace](/partner-center/develop/cancel-an-azure-marketplace-subscription).

### <a name="choose-whether-to-automatically-renew-a-commercial-marketplace-subscription"></a>Välj om du vill förnya en prenumeration på en extern Marketplace automatiskt

Som standard förnyas prenumerationer automatiskt när prenumerationstiden går ut. För [prenumerationer på kommersiella Marketplace-produkter](csp-commercial-marketplace-overview.md)kan du välja att inte förnya prenumerationen automatiskt.

Så här stoppar du en aktiv prenumeration på kommersiell marknads plats från automatisk förnyelse:

1. Logga in på [instrument panelen](https://partner.microsoft.com/dashboard)för partner Center.

2. Från menyn Partner Center väljer du **kunder** och väljer sedan en kund i listan.

3. Välj **Prenumerationer** . Här listas alla licensbaserade prenumerationer som du har köpt för kunden.

4. I kolumnen **prenumeration** väljer du den prenumeration som du vill ändra.

5. På sidan prenumerations information letar du reda på avsnittet **status** och avmarkerar rutan **förnya automatiskt** .

6. Välj **Skicka** .

## <a name="next-steps"></a>Nästa steg

- [Köp kommersiella Marketplace-produkter för dina kunder](csp-commercial-marketplace-purchase.md)

- [Hantera kommersiella Marketplace-produkter för dina kunder](csp-commercial-marketplace-manage.md)

- [Översikt över kommersiell Marketplace](csp-commercial-marketplace-overview.md)