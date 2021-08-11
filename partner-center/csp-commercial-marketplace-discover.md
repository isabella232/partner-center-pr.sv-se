---
title: Upptäck erbjudanden – kommersiell marknadsplats
ms.topic: how-to
ms.date: 05/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
description: Lär dig hur CSP-partner kan använda Partnercenter för att visa eller söka på marknadsplatsen efter SaaS-erbjudanden eller priser från oberoende programvaruleverantörer (ISV).
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 0b0e5e56a73a77d20c70468740653e99419dea6dea900b043730ed9a4524d85b
ms.sourcegitcommit: 121f1b9cbd88faeba60dc9b475f9c0647cdc933c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/06/2021
ms.locfileid: "115690961"
---
# <a name="discover-offers-and-pricing-in-partner-center-commercial-marketplace"></a>Upptäck erbjudanden och priser på den kommersiella marknadsplatsen i Partnercenter

**Lämpliga roller:** Global | Administratörsagent

När oberoende programvaruleverantörer väljer att publicera ett erbjudande på den kommersiella marknadsplatsen kan de också avgöra om de vill att erbjudandet ska göras tillgängligt i CSP-programmet. Om de väljer att sälja erbjudandet via CSP-programmet bör CSP-partner se erbjudandet i Partnercenter Marketplace-området.

Om ett ISV-erbjudande inte visas som förväntat i Partnercenter kan det beror på att:

- ISV:en valde att inte sälja erbjudandet via CSP-programmet. Vissa ISV-produkter kan till exempel ha gjorts tillgängliga på andra områden på den kommersiella marknadsplatsen (till exempel [i Microsoft AppSource](https://appsource.microsoft.com/) och [Azure Marketplace](https://azuremarketplace.microsoft.com/)), men de kanske inte visas för partner i CSP-programmet på Partner Center Marketplace.

- ISV:en bestämde sig för att göra erbjudandet exklusivt för ett visst antal CSP-partner. Mer information om exklusiva erbjudanden finns längre fram i det här hjälpavsnittet.

- Erbjudandetypen kanske inte kan användas via Partnercenter eller Azure Portal (t.ex. containrar eller vissa användningsbaserade erbjudanden).

- Faktureringsland för dina associerade kunder kanske inte stöds för det här ISV-erbjudandet.

## <a name="view-marketplace-offers-in-partner-center"></a>Visa Marketplace-erbjudanden i Partnercenter

Så här visar du tillgängliga erbjudanden på den kommersiella marknadsplatsen i CSP-programmet:

1. Logga in på instrumentpanelen [i Partnercenter](https://partner.microsoft.com/dashboard)och välj **sedan CSP** på den vänstra navigeringsmenyn.

2. Välj **Sälj** följt av **Marketplace.** Som standard visas produkter av alla typer och kategorier.

3. Välj ett filter efter typ eller kategori. Du kan också använda **Sök för** att hitta specifika nyckelord, erbjudandenamn eller namnen på ISV-utgivare.

4. Välj ett specifikt produkterbjudande i listan. Då kommer du till produktöversiktsfliken där du kan lära dig mer om erbjudandet. Informationen på den här fliken kan vara: 

    - En beskrivning av produkten eller erbjudandet

    - Mer information om ISV-utgivaren

    - Länkar till dokumentation eller marknadsföringsmaterial som laddats upp av ISV-utgivaren

    - Andra möjliga ISV-kontakter för kundsupport, teknik eller en kontakt för CSP-programmet

5. Om du vill se mer information om ett erbjudandes tillgängliga planer, SKU:er eller priser väljer du **fliken Planer +** priser. På den här fliken visas:

    - De marknader där det här erbjudandet är tillgängligt för dig

    - En lista över SKU:er eller planer som är tillgängliga för erbjudandet

    - Prissättning för varje tillgänglig SKU eller plan

## <a name="view-marketplace-offers-via-partner-center-apis"></a>Visa Marketplace-erbjudanden via Partner Center-API:er

CSP-programpartner kan också använda API:er för att returnera en lista över berättigade erbjudanden. Berättigade erbjudanden är endast de SaaS ISV-erbjudanden som är tillgängliga för partnern att sälja via Partner Center Marketplace. För partner som använder API:er för att identifiera erbjudanden i katalogen, se vägledningen för [att hämta en lista över erbjudanden för en marknad.](/partner-center/develop/create-subscription-azure-marketplace-products#get-a-list-of-offers-for-a-market)

## <a name="view-the-latest-marketplace-offer-pricing-in-partner-center"></a>Visa de senaste priserna för Marketplace-erbjudanden i Partnercenter

Följ de här stegen för den senaste prisinformationen som är associerad med ett erbjudande:

1. Logga in på instrumentpanelen [i Partnercenter](https://partner.microsoft.com/dashboard)och välj **sedan CSP** på den vänstra navigeringsmenyn.

2. Välj **Sälj** följt av **Priser och erbjudanden.**

3. Rulla ned till **avsnittet Marketplace,** välj en plats och ladda ned **Marketplace-priser.** Detta genererar ett kalkylblad med de senaste prisdata för SaaS, licensbaserade erbjudanden och uppmätta erbjudanden som är tillgängliga från ISV-utgivare. Vissa priser för Azure-program kan också visas här. Den här informationen uppdateras dagligen, så du kan kontrollera den för aktuella priser så ofta du väljer.

4. Om en ISV-produkt innehåller en kostnadsfri utvärderingsperiod visar kalkylbladet två rader för den produkten:

    - En rad visar priset för den kostnadsfria utvärderingsversionen på noll. Det innebär att en kostnadsfri utvärderingsperiod är tillgänglig.

    - Den andra raden visar det pris och de villkor som gäller när den kostnadsfria utvärderingsperioden är slut.

Som CSP-programpartner kan du vara berättigad till andra incitament som är associerade med vissa erbjudanden på den kommersiella marknadsplatsen. Mer information om andra incitament finns i [CSP-incitamentguiden (kräver](https://aka.ms/partnerincentives) CSP-inloggning).

## <a name="learn-about-marketplace-exclusive-offers"></a>Läs mer om marketplace-exklusiva erbjudanden

ISV:er har möjlighet att endast göra sina erbjudanden tillgängliga för specifika partner i CSP-programmet. Detta kallas för ett exklusivt erbjudande. Alla partner i CSP-programmet kan fortfarande visa alla ISV-erbjudanden på den kommersiella marknadsplatsen i Partnercenter, inklusive de erbjudanden som har markerats som Exklusiva.

Om ett erbjudande inte **är** markerat som Exklusivt kan alla partner köpa erbjudandet (förutsatt att den valda kundens faktureringsland matchar land tillgängligheten för ISV:ns erbjudande).

För ett erbjudande som är markerat som Exklusivt kan dock endast de partner som väljs av ISV:en köpa erbjudandet.

> [!NOTE]
> Om du ser ett erbjudande som är markerat som Exklusivt som du vill sälja till dina kunder kan du kontakta ISV direkt och be om tillstånd att sälja det exklusiva erbjudandet. När du visar information om ett exklusivt erbjudande kan du se en **kontakt-ISV-länk** som du kan välja.

Mer information om ISV-upplevelsen på den kommersiella marknadsplatsen finns i [Molnlösningsleverantörer.](/azure/marketplace/cloud-solution-providers)

Mer information om CSP-upplevelsen på marketplace finns i Översikt [över kommersiell marknadsplats.](csp-commercial-marketplace-overview.md)

## <a name="next-steps"></a>Nästa steg

- [Köpa erbjudanden på den kommersiella marknadsplatsen](csp-commercial-marketplace-purchase.md)