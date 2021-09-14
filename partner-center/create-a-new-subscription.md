---
title: Skapa kundprenumerationer i Partnercenter
ms.topic: how-to
ms.date: 08/25/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-customers
description: Lär dig hur du säljer prenumerationer till dina kunder för produkter som publicerats av Microsoft samt SaaS-produkter som publicerats av isv:er från tredje part.
author: BillLinzbach
ms.author: BillLi
ms.custom: SEOAPR.20
ms.localizationpriority: medium
ms.openlocfilehash: 5276f5bcc201633865fd8f226d52630919530982
ms.sourcegitcommit: 37eac16c4339cb97831eb2a86d156c45bdf6a531
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/13/2021
ms.locfileid: "126246930"
---
# <a name="create-suspend-or-cancel-customer-subscriptions"></a>Skapa, pausa eller avbryta kundprenumerationer

**Gäller för**: Partner Center-| Partnercenter för Microsoft Cloud for US Government

**Lämpliga roller:** Administratörsagent | Faktureringsadministratörskonto | Global | Supportagent | Försäljningsagent

När du har skapat en post för kunden i Partnercenter kan du sälja dem prenumerationer till produkter i katalogen. Detta omfattar produkter som publicerats av Microsoft och SaaS-produkter (Software as a Service) som publicerats av oberoende programvaruleverantörer (ISV) från tredje part på den [kommersiella marknadsplatsen.](https://azuremarketplace.microsoft.com/marketplace)

Vissa erbjudanden är begränsade till en prenumeration per kund. Om du vill se en lista över vilka erbjudanden som är begränsade går du till sidan Priser och erbjudanden för Partnercenter.

>[!IMPORTANT]
> Som partner i CSP-programmet kan du köpa  licensbaserade eller uppmätta SaaS-prenumerationer från **ISV-utgivare** i Partnercenter. Det innebär att du kan köpa alla licensbaserade eller **uppmätta** SaaS-erbjudanden [](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) som **ISV-utgivaren** har gjort tillgängliga för dig, inklusive exklusiva erbjudanden som du har åtkomst till. Om du vill köpa eller hantera andra erbjudanden på den kommersiella marknadsplatsen från ISV:er (till exempel användningsbaserade erbjudanden som rör Azure-program, containrar eller virtuella datorer) måste du [gå till Azure Portal](https://portal.azure.com/).

>[!NOTE]
>Alla datum och tider i Partnercenter anges i utc-tidsstandarden (Universal Time Coordinated). Detta kan skilja sig med upp till 24 timmar från din lokala tid.

## <a name="create-a-new-subscription"></a>Skapa en ny prenumeration

1. Logga in på [instrumentpanelen i Partnercenter](https://partner.microsoft.com/dashboard).

2. I menyn i Partnercenter väljer **du Kunder** och sedan en kund i listan.

3. Välj **Lägg till prenumeration.** På **fliken Onlinetjänster** visas alla tillgängliga Marketplace SaaS-erbjudanden.

4. Om du bara vill se vissa typer av prenumerationer gör du val i de tillgängliga filtren:
   - **Publisher: Välj** **Microsoft om** du bara vill se erbjudanden från Microsoft eller **Partner för** att se produkter från den kommersiella marknadsplatsen som publicerats av ISV:er.
   - **Faktureringstyp:** Välj den typ av prenumerationsfakturering som du vill använda: **Licens** eller **Användning.** Se [Licensbaserad fakturering för](license-based-billing.md) information som hjälper dig att välja mellan månatlig och årlig faktureringsfrekvens.
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
    > Varken du eller kunden får ett e-postmeddelande med instruktioner för att slutföra kontouppsättningen/etableringen för den här typen av ISV-prenumeration.)

    - Om din prenumeration har en 30-dagars kostnadsfri utvärderingsversion tillämpas den kostnadsfria utvärderingsperioden automatiskt. Som partner i CSP-programmet kan du inte undanta den kostnadsfria utvärderingsperioden för erbjudanden som du köper till kunder. När den kostnadsfria utvärderingsperioden har avslutats börjar prenumerationsperioden och prenumerationen konverteras till betald status. Prenumerationen förnyas sedan automatiskt enligt samma schema.
   
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

När du inaktiverar en prenumeration anger  datumet som visas under knappen Pausad när prenumerationen upphör att gälla automatiskt om du inte återaktiverar den. 

> [!Note] 
> Nya handelsändringar är för närvarande endast tillgängliga för partner som ingår i den tekniska förhandsversionen av Microsoft 365/Dynamics 365.

Om du vill inaktivera nya handelsprenumerationer eller återaktivera inaktiverade nya handelsprenumerationer skapar du en tjänstbegäran och kontaktar supporten. 

Aktivering och återaktivering av självbetjäning från instrumentpanelen och API:erna i Partnercenter kan vara tillgängliga i framtiden.

> [!NOTE]
> CSP-prenumerationer har inte någon förfallen period (så som web-direct-prenumerationer gör) då tjänsterna fortfarande fungerar, men prenumerationen genererar inga faktureringsavgifter. CSP-prenumerationer är antingen aktiva eller inaktiverade (eller helt borttagna).

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

4. I kolumnen **Status** väljer du **Avbryt.** **Skicka** sedan dina ändringar.

5. Om en dialogruta visas fyller du i relevant information och väljer sedan **Skicka**.

6. Bekräfta annulleringen genom att välja **Ja, avbryt**.

> [!NOTE]
> Du kan också välja att avbryta en prenumeration Azure Marketplace med hjälp av API:er. Det gör du genom att läsa [Avbryt en Azure Marketplace prenumeration.](/partner-center/develop/cancel-an-azure-marketplace-subscription)

### <a name="cancel-a-new-commerce-subscription"></a>Avbryta en ny handelsprenumeration

> [!Note] 
> Nya handelsändringar är för närvarande endast tillgängliga för partner som ingår i den tekniska förhandsversionen av Microsoft 365/Dynamics 365.

För nya handelserbjudanden kan du avbryta prenumerationen när som helst före perioden för åtagandeperioden. När du avbryter en prenumeration förlorar kunden omedelbart åtkomst till tjänsten. Åtkomsten kan inte återställas efter annulleringen. Följande alternativ för annullering är tillgängliga för en partner när prenumerationen har köpts: 

- Inom 24 timmar efter prenumerationens startdatum: Du kan avbryta hela prenumerationen inom 24 timmar för fullständig återbetalning.  
- Inom 30 dagar efter prenumerationens startdatum: Du kan avbryta hela prenumerationen inom de första 30 dagarna. Du får tillbaka hela beloppet minus det prodelade beloppet under de dagar då du använde prenumerationen.
- Efter 30 dagars prenumerationens startdatum: Du kan inte avbryta prenumerationen.

### <a name="pause-and-resume-a-new-commerce-subscriptions"></a>Pausa och återuppta en ny handelsprenumerationer 

> [!Note] 
> Nya handelsändringar är för närvarande endast tillgängliga för partner som ingår i den tekniska förhandsversionen av Microsoft 365/Dynamics 365.

Vid utebliven betalning från kunden, som ibland kallas "dunning", kan partner pausa och återuppta sin prenumeration för att omedelbart blockera kundens åtkomst till prenumerationens tjänster.

Om du pausar kundens prenumerationer inaktiveras möjligheten att logga in och använda deras tjänster tills prenumerationen återupptas.   

Du kan pausa en prenumeration med partnercenter:

1. Gå till kundens prenumerationssida och välj den prenumeration som du vill pausa

2. Välj **alternativknappen Pausa**

3. Läs popup-modal och välj **OK**

4. Prenumerationen har nu pausats och partnern fortsätter att debiteras för prenumerationen

Pausning är ett återställningsbart tillstånd via partnercentrets användargränssnitt eller API:er som omedelbart återställer en kunds åtkomst till en prenumerations tjänster. 

>[!IMPORTANT] 
> När du pausar en prenumeration inaktiveras eventuella inställningar för automatisk förnyelse och eventuella befintliga sceheduled-ändringar tas bort. Om du använder en prenumeration påverkar det bara kundens tjänståtkomst, partnerfakturering fortsätter medan den är i pausat tillstånd.

### <a name="choose-whether-to-automatically-renew-a-commercial-marketplace-subscription-or-a-new-commerce-subscription"></a>Välj om du vill förnya en prenumeration på den kommersiella marknadsplatsen automatiskt eller en ny handelsprenumeration

> [!Note] 
> Nya handelsändringar är för närvarande endast tillgängliga för partner som ingår i den tekniska förhandsversionen av Microsoft 365/Dynamics 365.

Som standard förnyas prenumerationer automatiskt när prenumerationstiden går ut. För [prenumerationer på produkter på den kommersiella](csp-commercial-marketplace-overview.md)marknadsplatsen, eller nya handelsprenumerationer, kan du välja att inte förnya prenumerationen automatiskt.

Så här stoppar du en aktiv prenumeration på den kommersiella marknadsplatsen eller nya handelsprenumerationer från att förnyas automatiskt:

1. Logga in på instrumentpanelen i [Partnercenter.](https://partner.microsoft.com/dashboard)

2. I menyn i Partnercenter väljer **du Kunder** och sedan en kund i listan.

3. Välj **Prenumerationer**. Här visas alla licensbaserade prenumerationer som du har köpt för kunden.

4. I kolumnen **Prenumeration** väljer du den prenumeration som du vill ändra.

5. På sidan med prenumerationsinformation letar du **upp avsnittet Status** och **avmarkerar rutan Förnya** automatiskt.

6. Välj **Skicka**.

### <a name="manage-new-commerce-renewals-with-scheduled-changes"></a>Hantera nya handelsförnyelse med schemalagda ändringar

> [!Note] 
> Nya handelsändringar är för närvarande endast tillgängliga för partner som ingår i den tekniska förhandsversionen av Microsoft 365/Dynamics 365.

Vissa ändringar i prenumerationer kan bara ske i slutet av en period. De här ändringarna kan schemaläggas så att de tillämpas praktiskt i slutet av perioden. Exempel på ändringar som måste schemaläggas:

- SKU nedgraderas
- Minskning av platser
- Ändringar av olika villkor
- Ändringar i faktureringsfrekvensen

Andra ändringar, till exempel uppgraderingar eller platsökningar, kan tillämpas under perioden.

Schemaändringar sker vid förnyelse när prenumerationen förnyas för nästa period.

Förutsättningar för schemalagda ändringar:

- Prenumerationen är aktiv 
- Automatisk förnyelse är på
- SKU:n måste vara berättigad till uppgradering för schemalagda uppgraderingar

Schemalägga en ny ändring som ska ske vid förnyelse

1. Logga in på instrumentpanelen i Partnercenter.

2. Välj en **kund** i kundlistan.

3. Välj den prenumeration som du vill hantera.

4. Välj **Hantera förnyelser.**

5. Välj ett annat Värdeändring för SKU, kvantitet, period eller faktureringsfrekvens:

   - **Aktuell** är det aktuella värdet för prenumerationen 

   - **Ändra** till är det senast sparade värdet som du vill använda vid förnyelsen för den nya prenumerationen 

6. Välj **Skicka**

7. Ändringarna sker vid förnyelsen. 

Partner kan komma åt **Hantera förnyelser för** att visa, uppdatera eller ta bort befintlig schemalagd ändring.

> [!Note] 
>- Utvärderingsversioner är schema för konvertering till den betalda SKU:n i slutet av deras period som standard. 
>- För schemalagda SKU-uppgraderingar/nedgradering av användarlicens måste omtilldeling göras manuellt.
>- Sparade schemalagda ändringar tas bort om följande uppdateringar efter halva tiden görs i prenumerationen.

### <a name="partial-upgrades-in-new-commerce-subscriptions"></a>Partiella uppgraderingar i nya handelsprenumerationer

> [!Note] 
> Nya handelsändringar är för närvarande endast tillgängliga för partner som ingår i den tekniska förhandsversionen av Microsoft 365/Dynamics 365.

Partiella uppgraderingar gör det möjligt för en partner att ange vissa licenser från en SKU till en annan. Tidigare uppgradering i traditionella licensbaserade prenumerationer gjorde att endast alla licenser kunde uppgraderas. Med ny handel kan en partner flytta vissa licenser när det passar dem. Detta ger partnern mer kontroll över hanteringen av uppgraderingar, så att de kan flytta vissa användare till en ny SKU utan att flytta alla. 

Partiella uppgraderingar kan schemaläggas att ske i slutet av en period eller initieras på medel sikt. 

Information om partiell uppgradering:

- Definieras som partiellt om antalet uppgraderingslicens är annorlunda än den ursprungliga prenumerationen.
- När du initierar en mellantidsuppgraderingar tas befintliga schemalagda uppgraderingar bort.
- Uppgraderingar kan bara initieras från prenumerationer i **aktivt** tillstånd.
- En ny prenumeration som skapas när du uppgraderar har samma slutdatum för perioden som den prenumeration som uppgraderingen kom från.

Partner kan komma åt vilken prenumeration de vill uppgradera till när de konfigurerar antal licenser och prenumerationer som de vill uppgradera till. Partner kan välja en **Ny** prenumeration eller välja en befintlig prenumeration.

## <a name="next-steps"></a>Nästa steg

- [Köpa produkter på den kommersiella marknadsplatsen för dina kunder](csp-commercial-marketplace-purchase.md)

- [Hantera produkter på den kommersiella marknadsplatsen för dina kunder](csp-commercial-marketplace-manage.md)

- [Översikt över kommersiell marknadsplats](csp-commercial-marketplace-overview.md)
