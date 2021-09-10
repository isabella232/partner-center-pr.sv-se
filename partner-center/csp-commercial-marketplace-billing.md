---
title: Fakturering för produkter på den kommersiella marknadsplatsen
ms.topic: article
ms.date: 05/12/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-billing
description: Lär dig hur fakturering fungerar för ISV SaaS-produkter eller -prenumerationer som köpts för kunder från den kommersiella marknadsplatsen i Partnercenter.
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 102f13530ece08cd813412a44897ece0186e7cbb
ms.sourcegitcommit: 1161d5bcb345e368348c535a7211f0d353c5a471
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/09/2021
ms.locfileid: "123960086"
---
# <a name="billing-for-commercial-marketplace-products-and-subscriptions-in-partner-center"></a>Fakturering för produkter och prenumerationer på den kommersiella marknadsplatsen i Partnercenter


**Lämpliga roller:** Globala | Faktureringsadministratör

Som partner i CSP-programmet kan du använda Partnercenter för att köpa licensbaserade SaaS-produkter från ISV-utgivare på den kommersiella marknadsplatsen. När du har gjort det kan du få åtkomst till en faktura för dessa typer av inköp. Faktureringsperioden börjar den första dagen i kalendermånaden och slutar den sista dagen i kalendermånaden. Fakturor görs tillgängliga den 8:e dagen i efterföljande månad.

Du kan komma åt fakturor från Partnercenter-instrumentpanelen [eller](https://partner.microsoft.com/dashboard/) med hjälp av [Partner Center-API:er.](/partner-center/develop/)

Partner i CSP-programmet debiteras för isv-lösningar på den kommersiella marknadsplatsen som köpts för en kund när de köper dessa produkter från antingen Partnercenter eller från Azure Portal (med hjälp av kundens tidigare CSP-köpta Azure-klient).

>[!NOTE]
>Om kunderna använder sin egen Azure AD-klientorganisation (inte en som köpts från en partner i CSP-programmet) kan kunderna också välja att köpa sin egen ISV SaaS-lösning direkt från ([Microsoft AppSource](https://appsource.microsoft.com/) eller [Azure Marketplace](https://azuremarketplace.microsoft.com/)). Om de gör det får de sin egen faktura direkt från Microsoft. På samma sätt gäller att om en partner i CSP-programmet säljer en Azure-prenumeration eller den nya Azure-planen till kunden och ger kunden (eller den indirekta återförsäljaren) rollbaserad åtkomst till den klientorganisationen (genom att tilldela en roll till kunden förutom Läsare) kan kunden (eller den indirekta återförsäljaren) också köpa erbjudanden på den kommersiella marknadsplatsen utan förhandsgodkännande eller avisering till [CSP-partnern.](/azure/role-based-access-control/built-in-roles) I dessa fall meddelar Microsoft inte direkt partner i CSP-programmet om inköp som görs av deras kunder. Microsoft erbjuder dock en valfri metod [Azure Monitor](/azure/azure-monitor/platform/alerts-activity-log) du kan använda för att ställa in aviseringar eller meddelanden om aktivitet i en Azure-prenumeration.

## <a name="access-billing-information-for-commercial-marketplace-products"></a>Få åtkomst till faktureringsinformation för produkter på den kommersiella marknadsplatsen

Den globala administratören eller faktureringsadministratören för ditt företag får ett e-postmeddelande när en faktura är redo att visas. Så här kommer du åt den senaste fakturan och avstämningsfilen för produktinköp på den kommersiella marknadsplatsen:

1. Logga in i Partnercenter och gå till [instrumentpanelen](https://partner.microsoft.com/dashboard/).

2. I menyn i Partnercenter väljer du **Fakturering.** 

    Två flikar visas överst på sidan Fakturering: **Återkommande och** **Återkommande samt engångsköp.** Med varje flik kan du komma åt faktura- och avstämningsfiler (rekognosering) för olika Marketplace-produkter:

    - **Fliken Återkommande:** Visar faktura- och avstämningsfiler för prenumerationer relaterade till Office 365, Microsoft 365, Dynamics 365, Azure Active Directory, Power BI Pro och Microsoft Azure.

    - **Fliken Återkommande och engångsköp:** Visar faktura- och avstämningsfiler för Azure-plan, Azure-reservationer, programvara och produkter på den kommersiella marknadsplatsen.
  
3. Välj fliken **Återkommande och engångsköp.** Om du har köpt prenumerationer för en kund i en annan valuta visas en flik för varje valuta. Du kan göra några saker från den här sidan:

    - Om du vill se den senaste fakturan och avstämningsfilen väljer **du Faktura** eller **avstämningsfil**. (Om du vill kan du också komma åt den senaste fakturan och rekognoseringsdata med hjälp av [Partner Center-API:er.](/partner-center/develop/)

    - Om du vill se tidigare fakturor och rekognoseringsfiler **expanderar du raden Faktureringshistorik** nedan.

    - Om du vill kontrollera ditt beräknade kontosaldo eller din faktura när som helst baserat på den senaste kontoaktiviteten väljer du en länk under **rubriken Uppskattningar.**  

    >[!NOTE]
    > När vi publicerar din faktura den 8:e dagen i månaden inkluderar den skatter och andra tillämpliga avgifter och krediter. Det innebär att det slutliga förfallna beloppet kan skilja sig från det du ser under faktureringsperioden.

## <a name="more-about-invoices-and-recon-files-for-commercial-marketplace-products"></a>Mer om fakturor och rekognoseringsfiler för produkter på den kommersiella marknadsplatsen

Det här avsnittet innehåller mer information om faktura- och avstämningsfiler för SaaS-prenumerationer på den kommersiella marknadsplatsen som köpts för kunder från ISV-utgivare från tredje part.

När du väljer Återkommande och  engångsköp från alternativet Fakturering i **Partnercenter-menyn** får du åtkomst till fakturor och avstämningsfiler för avgifter som rör både Microsoft-köp (förstapart) och ISV-inköp (tredje part). Dessa inköp kan associeras med:

- SaaS-prenumerationer (från Microsoft eller ISV-utgivare)

- Azure-plan

- Azure-reservationer

- Annan prenumerationsbaserad programvara (från Microsoft eller ISV-utgivare)

Exempel på dessa inköp kan vara SUSE Linux-programvara (en programvaruprenumeration) eller en Azure ISV SaaS-produktprenumeration.

>[!NOTE]
> Mer information om hur du läser faktura- och rekognoseringsfiler finns även i [Faktureringsöversikt.](billing.md)

### <a name="tips-on-reading-your-invoice"></a>Tips på att läsa din faktura

När du köper en licensbaserad SaaS-produkt från en ISV-utgivare från tredje part visas endast avgifter för licensavgiften på din faktura. Detta gäller även när ISV:ns SaaS-produkt använder (eller förbrukar) underliggande Azure-infrastrukturresurser. Det beror på att dina kunders användningsavgifter för Azure-infrastrukturen för en ISV:s SaaS-produkt debiteras direkt till ISV:en. (ISV:er ser associerade Kostnader för Azure-förbrukning i sin egen dagliga fakturaavstämningsfil för Azure-användning.)

Din faktura kommer att innehålla flera sidor:

- **Sida 1 på fakturan:** Innehåller en översikt över faktureringsinformationen för CSP-programpartnern. Detta inkluderar en sammanfattning av avgifterna för faktureringsperioden, ett fakturanummer, betalningsvillkor (60 dagar) och faktureringsmetoder för betalning via banköverföring eller check.

- **Sida 2 (och eventuella efterföljande sidor) på fakturan:** Information om avgifter för både Microsoft-inköp från första part och isv-köp från tredje part (licensbaserade) från den kommersiella marknadsplatsen. Du kan identifiera ISV-licensbaserade inköp efter **Publisher** under varje produktnamn. Den associerade avstämningsfilen ger mer faktureringsinformation för specifika fakturaavgifter.

- **Sista sidan på fakturan:** Om du har debiterats för licensbaserade Marketplace-produkter från en ISV visas mer information om ISV-utgivarens namn och adress på den här sista sidan.

### <a name="tips-on-reading-your-reconciliation-file"></a>Tips på att läsa avstämningsfilen

**Avstämningsfilen för återkommande och** engångsköp innehåller flera kolumner med ytterligare information som mappar till avgifterna på din faktura. Kolumnen **PublisherName** visar om köpet kommer från Microsoft eller en ISV-utgivare från tredje part.

Vissa avgifter i avstämningsfilen kan visas med en kostnad på 0 USD. Detta kan bero på ett erbjudande om "kostnadsfri utvärderingsversion" av isv:en (vanligtvis 30 eller 60 dagar) eller ett Bring Your Own License-erbjudande.

När det gäller isv-erbjudanden för kostnadsfria utvärderingsversion:

- Den kostnadsfria utvärderingsperioden omfattar kostnaden för ISV:ens licensbaserade SaaS-produkt under den tiden. Du debiteras heller inte för associerad Användning av SaaS-produkten i Azure-infrastrukturen.  Om du använder ett användningsbaserat ISV-erbjudande inkluderar den kostnadsfria utvärderingsversionen dock inte kostnaden för underliggande användning av Azure-infrastrukturen. I det här fallet visas användningsavgifter för Azure-infrastruktur i en separat Azure-avstämningsfil.

- När du köper och distribuerar en ISV:s kostnadsfria utvärderingsversion för kunden registreras kunden automatiskt i den kostnadsfria utvärderingsversionen av ISV-utgivaren. Den kostnadsfria utvärderingsperioden upphör automatiskt efter den period som definierats av ISV-utgivaren. När perioden är slut debiteras kunden. Det innebär att avstämningsfilen kan visa två rader för en utvärderingsberättigad produkt: En som spårar utvärderingsperioden och en som spårar det betalda erbjudandet (som visar en kostnad på 0 USD tills utvärderingsperioden har avslutats). När utvärderingsversionen är slut börjar raden som visar det betalda erbjudandet att visa avgifter. 

Mer information om vad varje kolumn representerar finns i Använda [avstämningsfilerna.](use-the-reconciliation-files.md) Se även [Typer av fakturering i Partnercenter](./billing-basics.md)

## <a name="next-steps"></a>Nästa steg

- [Hantera produkter på den kommersiella marknadsplatsen för kunder](csp-commercial-marketplace-manage.md)
- [Läs mer om support för produkter på den kommersiella marknadsplatsen](csp-commercial-marketplace-support.md)