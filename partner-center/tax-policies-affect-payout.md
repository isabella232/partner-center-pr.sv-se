---
title: Hur skatteprinciper påverkar utbetalningen för Azure Marketplace
description: Lär dig hur skatteprinciper påverkar utbetalning för Azure Marketplace.
ms.topic: conceptual
ms.service: partner-dashboard
ms.subservice: partnercenter-payouts
author: mingshen-ms
ms.author: mingshen
ms.date: 02/09/2021
ms.openlocfilehash: ef6520ff6ed4439e975dddaeff0b89ea2a912678c3871f1fc14bfb3cbe6bbff2
ms.sourcegitcommit: 121f1b9cbd88faeba60dc9b475f9c0647cdc933c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/06/2021
ms.locfileid: "115691546"
---
# <a name="how-tax-policies-affect-payout-for-azure-marketplace"></a>Hur skatteprinciper påverkar utbetalningen för Azure Marketplace

**Lämpliga roller:** Global | Administratörsbehörighet för användarhantering | Administratörsagent

## <a name="introduction"></a>Introduktion

Microsofts kommersiella marknadsplats har global räckvidd. Transaktioner sker över gränser och beroende på var den oberoende programvaruleverantören (ISV) och kunden finns kan skattekonsekvenserna variera. Microsoft AppSource och Azure Marketplace du använda skatteprofilinformationen för Partnercenter för att fastställa ISV:ens land. För att fastställa kundens land använder vi antingen kundens faktureringsinformation eller, om kunden är i EU, två olika typer av information.

Mer information om följande scenarier [](tax-details-marketplace.md) finns i tabellen Skatteinformation, som visar om Microsoft samlar in och betalar skatter åt utgivaren eller om ansvaret tillhör utgivaren.

> [!NOTE]
> Alla exempel på försäljningsvärden och skatteprocent i det här avsnittet är endast avsedda för illustrerande syfte, inte exakta siffror.

## <a name="publisher-transacts-in-microsoft-managed-tax-country"></a>Publisher Transaktioner i Microsoft-hanterat skatteland

**Scenario A** – Transaktioner som sker mellan en utgivare och en kund i ett [Microsoft-hanterat skatteland](tax-details-marketplace.md#microsoft-managed-countries). Dessa transaktioner kommer att ha en tillämplig skatt som läggs till vid tidpunkten för försäljningen och Microsoft skickar den skatt till det tillämpliga landet. Inga skatter från utbetalnings- och utbetalningsberäkningar är skattese exklusiva.

Se [Scenario D](#foreign-publisher-transacts-with-us-customer) för transaktioner mellan en icke-amerikansk utgivare och en amerikansk kund.

:::image type="content" source="images/tax-policies/payout-scenario-a.png" alt-text="Visar arbetsflödet för utbetalningsprocessscenario A.":::

## <a name="publisher-transacts-in-microsoft-managed-tax-country-where-marketplace-fee-is-taxable-service"></a>Publisher Transaktioner i Microsoft-hanterat skatteland där Marketplace-avgiften är en taxerbar tjänst

**Scenario B** – Transaktioner som äger rum mellan en amerikansk utgivare (enligt definitionen i deras skatteprofilinformation för Partnercenter) till en kund i ett Microsoft-hanterat skatteland där landet inför en skatt på Marketplace-avgiften (en taxerbar tjänst). I det här scenariot subtraheras avgiften för butikstjänsten från utgivarens utbetalning.

:::image type="content" source="images/tax-policies/payout-scenario-b.png" alt-text="Visar arbetsflödet för utbetalningsprocessens scenario B.":::

## <a name="publisher-transacts-in-publisher-managed-tax-country"></a>Publisher Transaktioner i Publisher skatteland

**Scenario C** – Transaktioner som sker mellan en utgivare och en kund i ett utgivar-hanterat skatteland som inte inför källskatt för kunder. Kunder betalar ingen skatt vid försäljningsplatsen och det är utgivarens ansvar att betala alla tillämpliga skatter.

Mer information om landsspecifika priser (till exempel för att motverka kommande skatteförskjutning) finns i Planer och priser för [erbjudanden på den kommersiella marknadsplatsen.](/azure/marketplace/plans-pricing#custom-prices)

:::image type="content" source="images/tax-policies/payout-scenario-c.png" alt-text="Visar arbetsflödet för utbetalningsprocessens scenario C.":::

## <a name="foreign-publisher-transacts-with-us-customer"></a>Foreign Publisher Transacts with US Customer

**Scenario D** – Alla externa utgivare (definieras av sin Skatteprofilinformation i Partnercenter) i länder utan amerikanskt konto (se [Scenario E](#foreign-publisher-with-a-treaty-transacts-with-us-customer)) som gör en försäljning till en USA-baserad kund (enligt definitionen av kundens kontoadress). Amerikanska myndigheter kräver att Microsoft använder källskatt för utgivarens räkning. Skatt från utbetalning till utgivare beräknas baserat på erbjudandets pris.

:::image type="content" source="images/tax-policies/payout-scenario-d.png" alt-text="Visar arbetsflödet för utbetalningsprocessens scenario D.":::

## <a name="foreign-publisher-with-a-treaty-transacts-with-us-customer"></a>Främmande utgivare med transacts för transacts med amerikansk kund

**Scenario E** – Alla externa utgivare (definieras av sin Skatteprofilinformation i Partnercenter) i länder där en amerikansk utgivare gör en försäljning till en USA-baserad kund (enligt definitionen av kundens kontoadress). Amerikanska myndigheter kräver inte att Microsoft källskatt för utgivarens räkning.

:::image type="content" source="images/tax-policies/payout-scenario-e.png" alt-text="Visar arbetsflödet för utbetalningsprocessscenario E.":::

## <a name="foreign-publisher-sells-to-an-eu-vat-registered-customer-in-a-microsoft-managed-country-outside-ireland"></a>En extern utgivare säljer till en momsregistrerad kund i EU i ett Microsoft-hanterat land (utanför Irland)

**Scenario F** – Alla transaktioner mellan externa utgivare och EU-registrerade kunder (moms) (utanför Irland) i ett Microsoft-Managed land. Kunden betalar inte skatt för försäljningen.

:::image type="content" source="images/tax-policies/payout-scenario-f.png" alt-text="Visar arbetsflödet för utbetalningsprocessens scenario F.":::

## <a name="foreign-publisher-sells-to-an-eu-vat-registered-customer-in-a-microsoft-managed-country-in-ireland"></a>En främmande utgivare säljer till en momsregistrerad kund i EU i ett Microsoft-hanterat land (i Irland)

**Scenario G** – Alla transaktioner mellan externa utgivare och EU-momsregistrerade kunder (i Irland) i ett Microsoft-Managed land. Kunden betalar Moms och Microsoft betalar den här momsen till myndigheter i Usa.

:::image type="content" source="images/tax-policies/payout-scenario-g.png" alt-text="Visar arbetsflöde för utbetalningsprocessscenario G.":::

## <a name="next-steps"></a>Nästa steg

- [Publisher Faq](/azure/marketplace/marketplace-faq-publisher-guide)
- [Anvisningar för att skapa betalnings- och skatteprofiler](./set-up-your-payout-account.md?context=%2fazure%2fmarketplace%2fcontext%2fcontext#create-a-payment-profile)