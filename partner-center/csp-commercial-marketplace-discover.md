---
title: Upptäck erbjudanden – kommersiell marknads plats
ms.topic: article
ms.date: 05/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Lär dig hur CSP-partner kan använda Partner Center för att visa eller söka i Marketplace efter SaaS erbjudanden eller priser från oberoende program varu leverantörer (ISV).
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: cb7b4ffdb4edf75e3e121e4ddea6b9de191ddbbf
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/22/2020
ms.locfileid: "92531661"
---
# <a name="discover-offers-and-pricing-in-the-partner-center-commercial-marketplace"></a>Identifiera erbjudanden och priser i Partner Center handels Marketplace

**Gäller för**

- Partnercenter
- Partner i CSP-programmet

**Lämpliga roller**

- Global administratör
- Administratörs agent

När oberoende program varu leverantörer (ISV) väljer att publicera ett erbjudande i den kommersiella marknads platsen kan de också avgöra om de vill att erbjudandet ska göras tillgängligt i CSP-programmet. Om de väljer att sälja erbjudandet via CSP-programmet, bör CSP-partners se erbjudandet i Marketplace-regionen för partner Center.

Om ett ISV-erbjudande inte visas som du förväntar dig i partner centret kan det bero på att:

- ISV valde att inte sälja erbjudandet via CSP-programmet. Vissa ISV-produkter kan till exempel ha gjorts tillgängliga i andra områden av den kommersiella marknads platsen (till exempel i [Microsoft AppSource](https://appsource.microsoft.com/) och [Azure Marketplace](https://azuremarketplace.microsoft.com/)), men kanske inte visas för kryptografiproviders på Partner Center Marketplace.

- ISV valde att göra erbjudandet exklusivt till endast ett SELECT-antal CSP-partner. Mer information om exklusiva erbjudanden finns längre fram i det här hjälp avsnittet.

- Erbjudande typen kanske inte går att använda i ett läge via partner centret eller Azure Portal (t. ex. behållare eller vissa användnings erbjudanden).

- Fakturerings landet för dina associerade kunder kanske inte stöds för det här ISV-erbjudandet.

## <a name="view-marketplace-offers-in-partner-center"></a>Visa Marketplace-erbjudanden i Partner Center

För att visa tillgängliga kommersiella Marketplace-erbjudanden i CSP-programmet: 

1. Logga in på Partner Center- [instrumentpanelen](https://partner.microsoft.com/dashboard)och välj **CSP** i den vänstra navigerings menyn.

2. Välj **Sälj** , följt av **Marketplace** . Som standard visas produkter av alla typer och kategorier.

3. Välj ett filter efter typ eller kategori. Du kan också använda **Sök** för att hitta vissa nyckelord, erbjudande namn eller namn på ISV-utgivare.

4. Välj ett enskilt produkt erbjudande i listan. Detta tar dig till en produkt översikts flik där du kan lära dig mer om erbjudandet. Informationen på den här fliken kan vara: 

    - En beskrivning av produkten eller erbjudandet

    - Mer information om ISV-utgivaren

    - Länkar till dokumentation eller marknadsförings material som laddas upp av ISV-utgivaren

    - Andra möjliga ISV-kontakter för kund support, teknik eller en kontakt för CSP-programmet

5. Om du vill se mer information om erbjudanden, SKU: er eller priser för erbjudandet väljer du fliken **abonnemang + prissättning** . På den här fliken visas:

    - De marknader där det här erbjudandet är tillgängligt för dig

    - En lista över SKU: er eller planer som är tillgängliga för erbjudandet

    - Prissättning för varje SKU eller abonnemang som är tillgängligt

## <a name="view-marketplace-offers-via-partner-center-apis"></a>Visa Marketplace-erbjudanden via API: er för partner Center

CSP-programpartner kan också använda API: er för att returnera en lista över berättigade erbjudanden. Berättigade erbjudanden är bara de SaaS ISV-erbjudanden som är tillgängliga för partnern att sälja via partner Center Marketplace. För partner som använder API: er för att identifiera erbjudanden i katalogen, se rikt linjerna för att [få en lista över erbjudanden för en marknad](/partner-center/develop/create-subscription-azure-marketplace-products#get-a-list-of-offers-for-a-market).

## <a name="view-the-latest-marketplace-offer-pricing-in-partner-center"></a>Visa den senaste prissättningen för Marketplace i Partner Center

Följ de här stegen för de senaste pris uppgifter som är associerade med ett erbjudande:

1. Logga in på Partner Center- [instrumentpanelen](https://partner.microsoft.com/dashboard)och välj **CSP** i den vänstra navigerings menyn.

2. Välj **försäljning** följt av **priser och erbjudanden** .

3. Rulla ned till **Marketplace** -avsnittet, Välj en plats och ladda ned **Marketplace-priser** . Detta genererar ett kalkyl blad med de senaste pris uppgifterna för SaaS, licensbaserade erbjudanden som är tillgängliga från ISV-utgivare. Vissa priser för Azure-program kan också visas här. Den här informationen uppdateras varje dag, så du kan kontrol lera den efter aktuella priser så ofta som du väljer.

4. Om en ISV-produkt innehåller en kostnads fri utvärderings period visar kalkyl bladet två rader för produkten:

    - En rad visar den kostnads fria utvärderings versionen på noll. Det innebär att en kostnads fri utvärderings period är tillgänglig.

    - Den andra raden visar priset och villkoren som ska gälla när den kostnads fria utvärderings perioden är över.

Som CSP-programpartner kan du vara berättigad till andra incitament som är kopplade till vissa kommersiella Marketplace-erbjudanden. Mer information om andra incitament finns i [stimulans guiden för CSP](https://aka.ms/partnerincentives) (kräver CSP-inloggning).

## <a name="learn-about-marketplace-exclusive-offers"></a>Läs om exklusiva erbjudanden för Marketplace

ISV: er har möjlighet att göra sina erbjudanden tillgängliga enbart för vissa partner i CSP-programmet. Detta kallas för ett exklusivt erbjudande. Alla partner i CSP-programmet kan fortfarande Visa alla ISV-erbjudanden i partner Centers kommersiella marknads platser, inklusive de som har marker ATS som exklusiva.

Om ett erbjudande **inte** har marker ATS som exklusiv kan alla partner köpa det erbjudandet (förutsatt att den valda kundens fakturerings land matchar landets tillgänglighet för ISV: s erbjudande).

För alla erbjudanden som marker ATS som exklusiva, kommer dock bara de partner som valts av ISV att kunna köpa det erbjudandet.

> [!NOTE]
> Om du ser ett erbjudande som marker ATS som du vill sälja till dina kunder kan du kontakta ISV direkt och be om tillåtelse att sälja erbjudandet exklusivt. När du visar information om ett exklusivt erbjudande kan du se en kontakt- **ISV** -länk som du kan välja.

Läs mer om ISV-upplevelsen på den kommersiella marknads platsen genom att läsa [leverantörer av moln lösningar](/azure/marketplace/cloud-solution-providers).

Mer information om CSP-upplevelsen på Marketplace finns i [Översikt över kommersiella marknads platser](csp-commercial-marketplace-overview.md).

## <a name="next-steps"></a>Nästa steg

- [Köp kommersiella Marketplace-erbjudanden](csp-commercial-marketplace-purchase.md)