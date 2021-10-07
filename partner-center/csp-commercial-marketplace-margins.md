---
title: Identifiera marginaler – kommersiell marknadsplats
ms.topic: how-to
ms.date: 10/06/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
description: Lär dig Molnlösningsleverantör (CSP)-partner kan använda Partnercenter för att identifiera marginaler som konfigurerats av oberoende programvaruleverantörer (ISV).
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 8d7b5f077b3ea3f98f87121634427842db0a0f03
ms.sourcegitcommit: 77737d8f986a1afb3d923c130936e2f73ce07879
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 10/07/2021
ms.locfileid: "129661380"
---
# <a name="discover-margins-configured-by-independent-software-vendors-isvs"></a>Identifiera marginaler som konfigurerats av oberoende programvaruleverantörer (ISV: er)

**Lämpliga roller:** Globala | Faktureringsadministratörskonto | Administratörsagent | Försäljningsagent | Supportagent

Oberoende programvaruleverantörer (ISV: er) kan erbjuda marginalrabatter för vissa erbjudanden på den kommersiella marknadsplatsen till specifika molnlösningsleverantörer (CPS). Dessa marginaler ger CPS incitament att sälja dessa erbjudanden till sina kunder.

> [!NOTE]
> Funktionen rabatter för ISV till CSP-marginal är för närvarande tillgänglig som en offentlig förhandsversion medan vi fortsätter att samla in feedback och förbättra upplevelsen. 

## <a name="notes-about-the-public-preview"></a>Information om den offentliga förhandsversionen

Med funktionen ISV-till-CSP-marginaler kan ISV:en skapa riktade rabatter till specifika CSP:er. Den här funktionen är tillgänglig nu men i offentlig förhandsversion. Det innebär att funktionen är fullt funktionell och användbar medan vi fortsätter att förbättra den övergripande CSP-marknadsplatsupplevelsen. Funktionen deklareras inte längre i förhandsversion när vi förbättrar partnerupplevelsen. Det finns inga specifika tidslinjer för detta och CSP-partner kan fortsätta att använda funktionen rabatter som den är.

### <a name="public-preview-improvement-areas"></a>Förbättringsområden för den offentliga förhandsversionen

- Tillgänglighet för AppSource-erbjudanden: Vissa CSP Marketplace-erbjudanden, främst AppSource-erbjudanden, tar längre tid att integrera och göra tillgängliga i Partnercenter. Vissa partner kanske letar efter AppSource-erbjudanden, men de kan behöva vänta tills de blir tillgängliga. Allt eftersom tiden går kommer Partnercenter-teamet att förbättra svarstiden mellan den tidpunkt då en ISV skapar ett erbjudande och när det är tillgängligt.
- Marginaler definieras för närvarande som procentuella rabatter för en CSP Marketplace-produkt-SKU. Framöver finns det önskemål om att integrera prispunkten i framtida prislistor. Tills detta händer kan partner koppla ihop produkt-SKU:n i marginallistan (och associerade API:er) med produkt-SKU:er för Marketplace-prislistan för att skapa prognoser för avgiftsbelopp.
- Vissa Marketplace-erbjudanden med utvärderingsversionen aktiverad, inte relaterad till marginalrabatter, visas som **00 USD** i belopp på Marketplace-bläddringsupplevelsen. Partner bör vara noga med att förstå att dessa utvärderingsversioner förnyas till betalda belopp i slutet av deras period. 
- Exklusiva erbjudanden kan vara tillgängliga för partner. För närvarande finns dessa inte i marketplace-prislistorna. Tills de är det måste partner hitta prissättningen för dem med hjälp av Marketplace-bläddringsupplevelsen för den produkt som de vill ha prissättning för.

## <a name="view-margins-in-partner-center"></a>Visa marginaler i Partnercenter

En CSP kan visa marginaler som ISV:er har konfigurerat för dem på marginalsidan:

> [!NOTE]
> Mer information om gränssnittet för arbetsytor finns i [Getting around Partner Center (Ta sig runt i Partnercenter).](get-around-partner-center.md#turn-workspaces-on-and-off)

#### <a name="workspaces-view"></a>[Vyn Arbetsytor](#tab/workspaces-view)

1. Logga in på [instrumentpanelen i Partnercenter](https://partner.microsoft.com/dashboard) och välj **panelen** Prissättning.

2. Välj **Marginaler.** Partner ser en lista över Marketplace-erbjudanden som ISV:er har konfigurerat marginaler för.

3. CSP-partner kan bläddra i listan över tillgängliga **marginaler eller** ladda ned data i kommaavgränsat format.

#### <a name="current-view"></a>[Aktuell vy](#tab/current-view)

1. Logga in på instrumentpanelen [i Partnercenter](https://partner.microsoft.com/dashboard)och välj **CSP** på den vänstra navigeringsmenyn.

2. Välj **Sälj** följt av **Marginaler.** Partner ser en lista över Marketplace-erbjudanden som ISV:er har konfigurerat marginaler för.

3. CSP-partner kan bläddra i listan över tillgängliga **marginaler eller** ladda ned data i kommaavgränsat format.

* * *

## <a name="margins-overview"></a>Översikt över marginaler

ISV:er som har etablerade relationer med CSP-partner kanske vill erbjuda marginalrabatter för att ge CSP-partnern incitament att sälja erbjudandena till sina kunder. I dessa fall förhandlar CSP-partnern ofta en marginal med en ISV, eller så kan ISV:en tillhandahålla en marginal utan att kontakta en CSP-partner. ISV:en kan erbjuda en marginal på antingen licensbaserade eller förbrukningsbaserade erbjudanden. Förbrukningsbaserade marginaler gäller endast för ISV-produkterna, inte för azure-förbrukningsprodukter som ISV-produkten kan fungera med.

## <a name="margins-and-pricing"></a>Marginaler och priser

Partnercenters marketplace-prislista innehåller den ursprungliga CSP-prissättningen för erbjudanden. CSP Marketplace-prislistor delas mellan alla partner och innehåller återförsäljarpriser. Partner tillämpar sedan rabatten på marginalprocenten för den produkt-SKU som de vill köpa för att förstå det slutliga priset för objektet innan de köper den. CSP-partner ser även återförsäljarpriser i Azure-prisbladet via Azure Portal (endast för förbrukningsbaserade produkter). De ser också detaljer om marginalen som har utökats till dem i det här prisbladet. 

## <a name="purchasing-offers"></a>Köperbjudanden

CSP-partner får sin konfigurerade marginal genom att helt enkelt köpa Marketplace-erbjudandet i [Partnercenter](https://partner.microsoft.com) eller distribuera produkten från Microsoft [Azure Portal](https://portal.azure.com). Den handlingspartner som gör det får marginalrabatten utan att behöva vidta ytterligare ett steg. Partner kan inte välja bort marginalen. Om ISV:en har konfigurerat den för CSP:en tillämpas rabatten.

Marginaler gäller för alla transaktioner som partnern kör och gäller för alla sina kunder. CSP-partnern behöver inte godkänna ett förslag och är inte skyldig att göra en överträdelse av ett ISV-erbjudande, men om de gör det och de har en marginal tillämpas det automatiskt. 

## <a name="margins-and-indirect-resellers"></a>Marginaler och indirekta återförsäljare

Marginaler görs endast tillgängliga för partner som debiteras av Microsoft, och de kan även användas av partner som indirekta leverantörer och direktfaktureringspartner. En ISV kan inte ge en marginal till en indirekt återförsäljare direkt, men den indirekta leverantören kan välja att skicka en marginal vidare till den indirekta återförsäljaren. Indirekta leverantörer kan välja att överföra marginalen till den indirekta återförsäljaren, men de är inte förtjänstgivare. 

## <a name="terms-and-billing"></a>Villkor och fakturering

Partner kan kontrollera att marginalen har tillämpats för förbrukningsbaserade erbjudanden med hjälp av Azures kostnadshanteringsfunktioner i Azure Portal. Partner kan kontrollera att marginalen har tillämpats för licensbaserade erbjudanden genom att granska avstämningsfilen i slutet av faktureringsperioden.

Varje marginal har ett start- och slutdatum. Prisminskningen baserat på marginalrabatten tillämpas på inköpperioden. En partner kan köpa om samma erbjudande efter sin period för att få en ny period med marginal. Förnyelser tillämpar marginalen om förnyelsen sker inom marginalens start- och slutdatum. Slutdatum för en marginal justeras alltid till slutet av månaden. 

## <a name="margins-for-metered-billing"></a>Marginaler för förbrukningsfakturering

Vissa CSP-produkter har förbrukningsfakturering. Om CSP-partnern ökar antalet platser för erbjudanden med förbrukningsbaserad fakturering behålls rabatten för den berättigandebaserade delen av avgifterna fram till slutet av den årliga prenumerationsperioden, men marginalen som tillämpas på priset för den avgiftsbelade faktureringen behålls inte efter marginalens slutperiod. Lösningen här är att ISV:er skapar en ny marginal för denna CSP-partner till slutet av prenumerationsperioden. 

## <a name="margins-notifications"></a>Marginalmeddelanden

Det finns inga proaktiva meddelanden såvida inte ISV:en kontaktar CSP:en via e-post och bekräftar att de har utökat en marginal. CSP-partnern kommer att kunna visa alla marginaler som är tillgängliga för dem via fliken Marginaler i Partnercenter.   

### <a name="recon-files"></a>Rekognoseringsfiler

CSP-partnern hittar information om marginalerna som har utökats till dem i **rekognoseringsfilen Återkommande** och engångsköp när de har genererats. Viktiga data i rekognoseringsfilen som förklarar marginalerna:

- Enhetspris förblir enligt det pris som angetts av ISV:en.  

- EffectiveUnitPrice visar priset när marginalen har tillämpats.  

- PriceAdjustmentDescription innehåller information om hur mycket av en marginal som har tillhandahållits till CSP-partnern. 

## <a name="discover-and-operationalize-margins-using-the-partner-center-apis"></a>Identifiera och operationalisera marginaler med partnercenter-API:er

Partner kan använda antingen Partner Center-användargränssnittet eller API:er för att visa eller exportera marginaler som är tillgängliga för dem.

### <a name="apis-to-retrieve-margins"></a>API:er för att hämta marginaler

Partner kan operationalisera data genom att anropa API:erna nedan. Vart och ett av dessa API:er returnerar en lista över marginaler som partnern har åtkomst till, definierad av ISV:en. Båda API:erna returnerar samma data.

- [Hämta marginaler](/partner-center/develop/get-margins) returnerar data i API-resultatformat

- [Nedladdningsmarginaler](/partner-center/develop/download-margins) returnerar data i ett kommaavgränsat format

### <a name="apis-to-discover-marketplace-offers"></a>API:er för att upptäcka Marketplace-erbjudanden

CSP-programpartner kan också använda API:er för att returnera en lista över marginaler som är tillgängliga för dem. Berättigade erbjudanden är endast de SaaS ISV-erbjudanden som är tillgängliga för partnern att sälja via Partner Center Marketplace. Partner kan hämta en lista över Marketplace SaaS-erbjudanden genom [att hämta en lista över erbjudanden för en marknad.](/partner-center/develop/create-subscription-azure-marketplace-products#get-a-list-of-offers-for-a-market)

CSP-partner kan använda Partner Center-API:er för att hämta listan över transakterbara SaaS-erbjudanden (programvara som en tjänst) och skicka beställningar till sina kunder. Mer information finns i Skapa [en prenumeration för produkter på den kommersiella marknadsplatsen.](/partner-center/develop/create-subscription-azure-marketplace-products)

CSP-partner kan använda Azure Portal UX för att visa alla Marketplace-erbjudanden. De kan använda följande API:er för att hämta listan över marketplace-erbjudanden för virtuella datorer och skicka beställningar till sina kunder.  
- [Virtuella datorer: Hämta en lista över API:er för erbjudanden för virtuella datorer](/azure/virtual-machines/windows/cli-ps-findimage)
- [Virtuella datorer: Köpa API:er (CLI, PowerShell, ARM)](/azure/virtual-machines/linux/quick-create-cli) 

Det finns inget filter i Azure Portal för erbjudanden som säljs via CSP. Partner måste granska prislistan för att förstå vilka erbjudanden som kan göras via CSP. Det finns för närvarande Azure Portal TILLGÄNGLIGA API:er för att hantera SaaS- eller Managed Application Marketplace-erbjudanden. 

Mer information om CSP-upplevelsen på marketplace finns i Översikt [över kommersiell marknadsplats.](csp-commercial-marketplace-overview.md)

## <a name="next-steps"></a>Nästa steg

- [Översikt över kommersiell marknadsplats](csp-commercial-marketplace-overview.md)
- [Köpa erbjudanden på den kommersiella marknadsplatsen](csp-commercial-marketplace-purchase.md)
- [Guide för CSP-incitament](https://aka.ms/partnerincentives)
