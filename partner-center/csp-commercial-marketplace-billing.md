---
title: Fakturering för kommersiella Marketplace-produkter
ms.topic: article
ms.date: 05/12/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Lär dig hur faktureringen fungerar för ISV SaaS-produkter eller prenumerationer som köpts för kunder från den kommersiella marknads platsen i Partner Center.
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 10592c7f8a3b1f075bc726161603859552b29961
ms.sourcegitcommit: a78dd3c532860d01867d116bfb4e2c88b84bcd25
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 01/08/2021
ms.locfileid: "97979540"
---
# <a name="billing-for-commercial-marketplace-products-and-subscriptions-in-partner-center"></a>Fakturering för produkter och prenumerationer på kommersiella platser i Partner Center


**Lämpliga roller**

- Global administratör
- Faktureringsadministratör

Som partner i CSP-programmet kan du använda Partner Center för att köpa licensbaserade SaaS-produkter från ISV-utgivare på den kommersiella marknaden. När du har gjort det kan du komma åt en faktura för dessa typer av inköp. Fakturerings perioden börjar på den första dagen i kalender månaden och slutar den sista dagen i kalender månaden. Fakturor görs tillgängliga den åttonde dagen i följande månad.

Du kan komma åt fakturor från antingen [instrument panelen](https://partner.microsoft.com/dashboard/) för partner Center eller genom att använda [API: er för partner Center](/partner-center/develop/).

Partner i CSP-programmet debiteras för ISV-lösningar för kommersiella marknads platser som köpts för en kund när de köper dessa produkter från antingen Partner Center eller från Azure Portal (med hjälp av kundens tidigare CSP-köpta Azure-klient).

>[!NOTE]
>Om kunderna använder sin egen Azure AD-klient (inte en som köpts från en partner i CSP-programmet) kan kunderna också välja att köpa sin egen ISV SaaS-lösning direkt från ([Microsoft AppSource](https://appsource.microsoft.com/) eller [Azure Marketplace](https://azuremarketplace.microsoft.com/)). Om de gör det kommer de att få sin egen faktura direkt från Microsoft. Om en partner i CSP-programmet säljer en Azure-prenumeration eller den nya Azure-prenumerationen till kunden och ger kunden (eller den indirekta åter försäljaren) [rollbaserad åtkomst](/azure/role-based-access-control/built-in-roles) till den innehavaren (tilldela en roll till kunden förutom **läsaren**) kan den kunden (eller indirekta åter försäljaren) även köpa kommersiella Marketplace-erbjudanden utan föregående godkännande eller meddelande till CSP-partnern. I dessa fall kommer Microsoft inte att meddela partners i CSP-programmet om köp som görs av deras kunder. Microsoft erbjuder dock en valfri [Azure Monitor](/azure/azure-monitor/platform/alerts-activity-log) mekanism som du kan använda för att ställa in aviseringar eller meddelanden om aktiviteter på en Azure-prenumeration.

## <a name="access-billing-information-for-commercial-marketplace-products"></a>Få åtkomst till fakturerings information för kommersiella Marketplace-produkter

Den globala administratörs-eller fakturerings administratören för ditt företag får ett e-postmeddelande när en faktura är klar att visa. För att få åtkomst till den senaste fakturan och avstämnings filen för produkt inköp på kommersiella platser:

1. Logga in på Partner Center- [instrumentpanelen](https://partner.microsoft.com/dashboard/).

2. Från menyn Partner Center väljer du **fakturering**. 

    Du kommer att se två flikar överst på sidan fakturering: **återkommande** och **återkommande och engångs köp**. På varje flik kan du komma åt faktura-och avstämnings-filer (rekognoseringar) för olika Marketplace-produkter:

    - Fliken **återkommande** : visar faktura-och avstämnings filer för prenumerationer relaterade till Office 365, Microsoft 365, Dynamics 365, Azure Active Directory, Power BI Pro och Microsoft Azure.

    - Fliken **återkommande och engångs inköp** : visar faktura-och avstämnings filer för Azure-prenumeration, Azure-reservationer, program vara och kommersiella Marketplace-produkter.
  
3. Välj fliken **återkommande och en-tid-inköp** . Om du har köpt prenumerationer för en kund i en annan valuta, visas en flik för varje valuta. Du kan göra några saker fr: om den här sidan:

    - Om du vill se den senaste fakturan och avstämnings filen väljer du **faktura** eller **avstämnings fil**. (Om du vill kan du också komma åt de senaste faktura-och rekognoseringar-fildata med hjälp av [API: er för partner Center](/partner-center/develop/).

    - Om du vill se tidigare fakturor och rekognoseringar-filer expanderar du raden för **fakturerings historiken** nedan.

    - Välj en länk under rubriken **uppskattningar** för att kontrol lera uppskattat saldo eller faktura när som helst baserat på den senaste konto aktiviteten.  

    >[!NOTE]
    > När vi publicerar din faktura den åttonde dagen i månaden inkluderar den skatter och eventuella andra tillämpliga kostnader och krediter. Det innebär att den slutliga förfallo mängden kan skilja sig från vad du ser under fakturerings perioden.

## <a name="more-about-invoices-and-recon-files-for-commercial-marketplace-products"></a>Mer om fakturor och rekognoseringar-filer för kommersiella Marketplace-produkter

Det här avsnittet innehåller mer information om faktura-och avstämnings filer för SaaS-prenumerationer från tredje part som köpts av kunder från tredjeparts ISV-utgivare.

När du väljer **återkommande och engångs köp** från **fakturerings** alternativet på Partner Center-menyn får du till gång till fakturor och avstämnings filer för avgifter som rör både Microsoft (första och från tredje part) inköp. Dessa inköp kan associeras med:

- SaaS-prenumerationer (från antingen Microsoft eller ISV-utgivare)

- Azure-plan

- Azure-reservationer

- Annan prenumeration baserad på program vara (från antingen Microsoft eller ISV-utgivare)

Exempel på sådana inköp kan vara SUSE Linux-programvara (en program varu prenumeration) eller en Azure ISV SaaS-produkt prenumeration.

>[!NOTE]
> Mer information om hur du läser faktura-och rekognoseringar-filer finns även i [fakturerings översikt](billing.md).

### <a name="tips-on-reading-your-invoice"></a>Tips om att läsa din faktura

När du köper en licensbaserade SaaS-produkt från en tredjeparts ISV-utgivare kan du bara se avgifter för licens avgiften på din faktura. Detta gäller även när ISV: s SaaS-produkt använder (eller använder) underliggande infrastruktur resurser i Azure. Det beror på att din kunds användnings avgift för Azure-infrastruktur för en ISV: s SaaS-produkt faktureras direkt till ISV. (ISV: er kommer att se tillhör ande Azure förbruknings avgifter i sin egen Azure-användning dagligt Beräknad faktura avstämnings fil.)

Din faktura kommer att innehålla flera sidor:

- **Sidan 1 på fakturan:** Innehåller en översikt över fakturerings information för CSP-programpartnern. Detta inkluderar en sammanfattning av debiteringar för fakturerings perioden, ett faktura nummer, betalnings villkor (netto 60 dagar) och fakturerings betalnings metoder som ska betalas per tråd eller av kontroll.

- **Sidan 2 (och eventuella efterföljande sidor) av fakturan:** Information debiteras för både första köp av Microsoft-inköp och ISV-baserade (licensbaserade) inköp från den kommersiella marknads platsen. Du kan identifiera ISV licensbaserade inköp av **utgivar** raden under varje produkt namn. Den associerade avstämnings filen ger ytterligare fakturerings information för vissa faktura avgifter.

- **Sista sidan i fakturan:** Om du debiteras för licensbaserade Marketplace-produkter från en ISV visas mer information om namnet och adressen för ISV-utgivaren på den sista sidan.

### <a name="tips-on-reading-your-reconciliation-file"></a>Tips om att läsa din avstämnings fil

Den **återkommande och en** avstämnings fil för inköp innehåller flera kolumner med ytterligare information som mappar till avgifterna i din faktura. I kolumnen **PublisherName** visas om köpet är från Microsoft eller en tredjeparts-ISV-utgivare.

Vissa kostnader i avstämnings filen kan visas med en kostnad på $0. Detta kan bero på ett kostnads fritt erbjudande om kostnads fri utvärdering (vanligt vis 30 eller 60 dagar) eller ett eget licens erbjudande.

Om du har en kostnads fri utvärderings version av ISV:

- Den kostnads fria utvärderings perioden omfattar kostnaden för ISV: s licensbaserade SaaS-produkt under den tiden. Du kommer inte heller att debiteras för associerad Azure-infrastrukturs användning av den SaaS produkten.  Om du använder ett användnings oberoende ISV-erbjudande omfattar den kostnads fria utvärderings versionen inte kostnaden för den underliggande användningen av Azure-infrastrukturen. I det här fallet kommer Azure Infrastructure Usage-kostnader att visas i en separat Azure-avstämnings fil.

- När du köper och distribuerar en ISV: s kostnads fria utvärderings produkt för din kund registreras kunden automatiskt i den kostnads fria utvärderings versionen av ISV-utgivaren. Den kostnads fria utvärderings perioden upphör automatiskt efter den period som har definierats av ISV-utgivaren. När perioden är slut kommer kunden att debiteras. Det innebär att avstämnings filen kan visa två rader för en berättigad produkt: en som spårar utvärderings perioden och en som spårar det betalda erbjudandet (som visar kostnaden $0 fram till dess att utvärderings perioden är slut). När utvärderings versionen är slut börjar raden som visar det betalda erbjudandet att Visa avgifter. 

Mer information om vad varje kolumn representerar finns i [Använd dina avstämnings filer](use-the-reconciliation-files.md). Se även [typer av fakturering i Partner Center](billing-different-types.md)

## <a name="next-steps"></a>Nästa steg

- [Hantera kommersiella Marketplace-produkter för kunder](csp-commercial-marketplace-manage.md)
- [Lär dig mer om stöd för kommersiella Marketplace-produkter](csp-commercial-marketplace-support.md)