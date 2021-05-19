---
title: Skapa kundprenumerationer i Partnercenter
ms.topic: how-to
ms.date: 05/17/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Lär dig hur du säljer prenumerationer till dina kunder för produkter som publicerats av Microsoft samt SaaS-produkter som publicerats av tredjeparts-ISV:er.
author: BillLinzbach
ms.author: BillLi
ms.custom: SEOAPR.20
ms.localizationpriority: medium
ms.openlocfilehash: 3269fa994d704c0a0dae067087bad8589a7ce031
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 05/19/2021
ms.locfileid: "110148213"
---
# <a name="create-suspend-or-cancel-customer-subscriptions"></a>Skapa, pausa eller avbryta kundprenumerationer

**Gäller för:** Partner Center-| Partnercenter för Microsoft Cloud for US Government

**Lämpliga roller:** Administratörsagent | Faktureringsadministratörskonto | Globala | Supportagent för | Försäljningsagent

När du har skapat en post för kunden i Partnercenter kan du sälja dem prenumerationer till produkter i katalogen. Detta omfattar produkter som publicerats av Microsoft och SaaS-produkter (Software as a Service) som publicerats av oberoende programvaruleverantörer (ISV: er) från tredje part på den [kommersiella marknadsplatsen.](https://azuremarketplace.microsoft.com/marketplace)

Vissa erbjudanden är begränsade till en prenumeration per kund. Om du vill se en lista över vilka erbjudanden som är begränsade går du till sidan Priser och erbjudanden för Partnercenter.

>[!IMPORTANT]
> Som partner i CSP-programmet kan du köpa  licensbaserade eller uppmätta SaaS-prenumerationer från **ISV-utgivare** i Partnercenter. Det innebär att du kan köpa alla licensbaserade eller uppmätta SaaS-erbjudanden [](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) som  **ISV-utgivaren** har gjort tillgängliga för dig, inklusive exklusiva erbjudanden som du har åtkomst till. Om du vill köpa eller hantera andra erbjudanden på den kommersiella marknadsplatsen från ISV:er (till exempel användningsbaserade erbjudanden som rör Azure-program, containrar eller virtuella datorer) [måste du gå till Azure Portal](https://portal.azure.com/).

## <a name="create-a-new-subscription"></a>Skapa en ny prenumeration

1. Logga in på [instrumentpanelen i Partnercenter](https://partner.microsoft.com/dashboard).

2. I menyn i Partnercenter väljer **du Kunder** och sedan en kund i listan.

3. Välj **Lägg till prenumeration.** På **fliken Onlinetjänster** visas alla tillgängliga SaaS-erbjudanden på Marketplace.

4. Om du bara vill se vissa typer av prenumerationer gör du val i de tillgängliga filtren:
   - **Utgivare:** Välj **Microsoft om** du bara vill se erbjudanden från Microsoft eller Partner om **du vill** se produkter från den kommersiella marknadsplatsen som publicerats av ISV:er.
   - **Faktureringstyp:** Välj vilken typ av prenumerationsfakturering du vill använda: **Licens** eller **Användning.** Se [Licensbaserad fakturering för](license-based-billing.md) information som hjälper dig att välja mellan månatlig och årlig faktureringsfrekvens.
   - **Kategori:** Välj **Företag,** **Litet företag** eller **Utvärderingsversion.** Information om utvärderingsprenumerationer finns [i Offer your customers trials of Microsoft products (Erbjuda dina kunder utvärderingsversioner av Microsoft-produkter).](offer-your-customers-trials-of-microsoft-products.md)

5. Välj de produktprenumerationer som du vill köpa för kunden. Vilka produkter du ser beror på typen av kundsegment (utbildning, myndigheter osv.) och de filter som du har tillämpat. Vissa erbjudanden som visas på Marketplace kanske inte alltid är tillgängliga för en specifik kund eller en specifik CSP-partner. Det kan vara så här:

   - Kunden har redan en prenumeration på produkten och tillåts bara en

   - Kundens prenumeration kan ha inaktiverats (i det här fallet kan du återaktivera prenumerationen i stället för att köpa en ny.)

   - För ISV SaaS-erbjudanden kan det finnas några orsaker till varför erbjudandet inte är tillgängligt att köpa: ISV:en kanske inte stöder kundens faktureringsland eller region; ISV:en kan ha valt att inte göra erbjudandet tillgängligt via CSP-programmet, eller så kan ISV:en ha gjort erbjudandet [exklusivt för](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) vissa CSP-partner. ISV-erbjudandet kanske inte heller kan göras via Partnercenter (till exempel containrar eller vissa användningsbaserade erbjudanden).  

6. För varje prenumeration som du vill lägga till anger du antalet licenser (om det behövs) och väljer Lägg **till i kundvagn.**

7. När du är klar med att lägga till prenumerationer väljer **du Granska** och granskar din beställning.

8. När du har granskat dina beställningar och är redo att köpa dessa prenumerationer väljer du **Köp.**

9. När du har köpt en prenumeration för en kund sker följande:

    - Du kan granska eller redigera prenumerationen genom att välja prenumerationsnamnet på kundens **prenumerationssida.** Härifrån kan du välja tilläggslicenser om det finns några, ändra antalet licenser eller pausa prenumerationen.

    **För ISV SaaS-prenumerationer (licensbaserade och uppmätta):**
    - Du får en länk till ISV-utgivarens webbplats. Den här länken hjälper dig att slutföra distributionen eller kontokonfigurationen av kundens prenumeration.
      
    >[!NOTE]
    > Varken du eller kunden får ett e-postmeddelande med instruktioner för att slutföra konto set up/provisioning för den här typen av ISV-prenumeration.)

    - Om din prenumeration har en 30-dagars kostnadsfri utvärderingsversion tillämpas den kostnadsfria utvärderingsperioden automatiskt. Som partner i CSP-programmet kan du inte undanta den kostnadsfria utvärderingsperioden för erbjudanden som du köper till kunder. När den kostnadsfria utvärderingsperioden har avslutats börjar prenumerationsperioden och prenumerationen konverteras till betald status. Prenumerationen förnyas sedan automatiskt enligt samma schema.
   
## <a name="update-subscriptions-with-add-ons"></a>Uppdatera prenumerationer med tillägg 

För att kunna köpa ett tillägg måste kunden först ha en aktiv basprenumeration.  Det går inte att köpa tillägg via katalogen.

1. Logga in på instrumentpanelen i [Partnercenter.](https://partner.microsoft.com/dashboard)

2. I menyn i Partnercenter väljer **du Kunder** och sedan en kund i listan.

3. Välj den prenumeration som du vill hantera.

4. Under **avsnittet Status** finns en lista över tillgängliga tillägg för prenumerationen.  

5. Uppdatera antalet licenser för varje obligatoriskt tillägg. **Skicka** sedan dina ändringar.

Möjligheten att köpa tillägg via Partnercenter är endast tillgänglig för direkta fakturerade och indirekta leverantörer.
Endast berättigade tillägg visas baserat på grundkraven och regional tillgänglighet. Mer information om priser och erbjudanden finns i erbjudandematrisen för molnåterförsäljare. Om du avbryter basprenumerationen inaktiveras även eventuella associerade tillägg.

Startdatumen för tillägg följer basprenumerationen och avgifterna beräknas utifrån startdatumet för debitering och slutdatumet för debitering med proportionella avgifter på den första fakturan. Mer information finns i [Licensbaserad fakturering.](license-based-billing.md)


## <a name="suspend-or-cancel-a-subscription"></a>Pausa eller avbryta en prenumeration

Partner kan inaktivera eller avbryta en prenumeration om det begärs av kunden, eller i fall av utebliven betalning eller bedrägeri.

### <a name="suspend-a-subscription"></a>Inaktivera en prenumeration

När du ändrar statusen för en prenumeration **till Inaktiverad** kan användarna inte logga in eller komma åt tjänster.

1. Logga in på instrumentpanelen i [Partnercenter.](https://partner.microsoft.com/dashboard)

2. I menyn i Partnercenter väljer **du Kunder** och sedan en kund i listan.

3. Välj den prenumeration som du vill hantera.

4. I avsnittet **Status** väljer du **Tillfälligt avbruten**. **Skicka** sedan dina ändringar.

5. Alla data tas bort om inte prenumerationen återaktiveras inom 90 dagar, eller 90 dagar plus antalet dagar mellan den tidpunkt då kontot öppnades och den första faktureringsperioden (högst 120 dagar).

När du inaktiverar en prenumeration anger  datumet under knappen Pausad när prenumerationen upphör att gälla automatiskt om du inte återaktiverar den. 

>[!NOTE]
>CSP-prenumerationer har inte en förfallen period (så som web-direct-prenumerationer gör) då tjänsterna fortfarande fungerar men prenumerationen genererar inga faktureringsavgifter. CSP-prenumerationer är antingen aktiva eller inaktiverade (eller helt borttagna).

### <a name="cancel-a-subscription"></a>Avbryta en prenumeration

Du kan avbryta licensbaserade SaaS-prenumerationer från isv-utgivare från tredje part på den kommersiella marknadsplatsen [i Partnercenter.](csp-commercial-marketplace-overview.md) Så länge du avbryter inom annulleringsperioden får du en fullständig återbetalning.

För ISV-erbjudanden som faktureras månadsvis:

- Om du avbryter mindre än 24 timmar efter att du har gjort beställningen får du en fullständig kredit på nästa faktura.

- Om du avbryter senare än 24 timmar efter att du har gjort beställningen schemaläggs annulleringen att ske vid förnyelsen.

För erbjudanden som faktureras per år:

- Om du avbryter mindre än 14 dagar efter att du har beställt får du en fullständig kredit på nästa faktura.

- Om du avbryter senare än 14 dagar efter att du har beställt kommer annulleringen att schemaläggas att ske vid förnyelsen.

När dessa perioder är över ser du inte längre alternativet att avbryta prenumerationen.

> [!NOTE]
> Användningsbaserade och uppmätta ISV-tjänster från tredje part (som till exempel använder virtuella datorer eller containrar) är inte berättigade till retur. Användningsbaserade tjänster kan avetableas som en annulleringsmetod. Eftersom avgifter debiteras efter användning är dessa tjänster inte berättigade till återbetalning.

Så här avbryter du en licensbaserad SaaS-prenumeration från en ISV-utgivare:

1. Logga in på instrumentpanelen i [Partnercenter.](https://partner.microsoft.com/dashboard)

2. I menyn i Partnercenter väljer **du Kunder** och sedan en kund i listan.

3. Leta upp den prenumeration som du vill avbryta.

4. I kolumnen **Status** väljer du **Avbryt**. **Skicka** sedan dina ändringar.

5. Om en dialogruta visas fyller du i relevant information och väljer sedan **Skicka**.

6. Bekräfta annulleringen genom att välja **Ja, avbryt**.

> [!NOTE]
> Du kan också välja att avbryta en prenumeration Azure Marketplace med hjälp av API:er. Om du vill göra det kan [du läsa Avbryta en Azure Marketplace prenumeration.](/partner-center/develop/cancel-an-azure-marketplace-subscription)

### <a name="choose-whether-to-automatically-renew-a-commercial-marketplace-subscription"></a>Välj om du vill förnya en prenumeration på den kommersiella marknadsplatsen automatiskt

Som standard förnyas prenumerationer automatiskt när prenumerationstiden går ut. För [prenumerationer på kommersiella marknadsplatsprodukter](csp-commercial-marketplace-overview.md)kan du välja att inte förnya prenumerationen automatiskt.

Så här stoppar du en aktiv prenumeration på den kommersiella marknadsplatsen från att förnyas automatiskt:

1. Logga in på instrumentpanelen i [Partnercenter.](https://partner.microsoft.com/dashboard)

2. I menyn i Partnercenter väljer **du Kunder** och sedan en kund i listan.

3. Välj **Prenumerationer**. Här visas alla licensbaserade prenumerationer som du har köpt för kunden.

4. I kolumnen **Prenumeration** väljer du den prenumeration som du vill ändra.

5. På sidan med prenumerationsinformation letar du **upp avsnittet Status** och **avmarkerar rutan Förnya** automatiskt.

6. Välj **Skicka**.

## <a name="next-steps"></a>Nästa steg

- [Köpa produkter på den kommersiella marknadsplatsen för dina kunder](csp-commercial-marketplace-purchase.md)

- [Hantera produkter på den kommersiella marknadsplatsen för dina kunder](csp-commercial-marketplace-manage.md)

- [Översikt över kommersiell marknadsplats](csp-commercial-marketplace-overview.md)