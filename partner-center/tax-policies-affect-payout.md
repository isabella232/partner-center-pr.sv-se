---
title: Så här påverkar skatte principer utbetalning för Azure Marketplace
description: Lär dig hur skatte principer påverkar utbetalning för Azure Marketplace.
ms.topic: conceptual
ms.service: partner-dashboard
author: mingshen-ms
ms.author: mingshen
ms.date: 02/09/2021
ms.openlocfilehash: 19acb085b601212f1bf94316aab2b72c54aecc1a
ms.sourcegitcommit: e8e8362d2777d25efac3e1076af5939765ed13d0
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/20/2021
ms.locfileid: "104712961"
---
# <a name="how-tax-policies-affect-payout-for-azure-marketplace"></a>Så här påverkar skatte principer utbetalning för Azure Marketplace

**Lämpliga roller**
-    Global administratör
-    Användaradministratör
-    Administratörs agent

## <a name="introduction"></a>Introduktion

Microsofts kommersiella marknads plats har global räckvidd. Transaktioner sker över gränserna och beroende på var ISV och kund finns kan skatte konsekvenserna variera. Microsoft AppSource och Azure Marketplace använder partner Centers skatte profil information för att fastställa ISV: s land. För att fastställa kundens land kan du antingen använda kundens fakturerings information eller, om kunden är i EU, använda två olika informations delar.

För att bättre förstå följande scenarier, se tabellen med [skatte information](tax-details-marketplace.md) , som visar om Microsoft samlar in och betalar skatt för utgivarens räkning eller om detta ansvar tillhör utgivaren.

> [!NOTE]
> Alla exempel på försäljnings värden och skatte procent satser i det här avsnittet är endast avsedda som exempel, inte exakta siffror.

## <a name="publisher-transacts-in-microsoft-managed-tax-country"></a>Utgivaren agerar i Microsoft-hanterade skatte länder

**Scenario A** – transaktioner som sker mellan en utgivare och en kund i ett [Microsoft-hanterat skatte land](tax-details-marketplace.md#microsoft-managed-countries). De här transaktionerna kommer att ha en avgift som lagts till vid försäljnings tillfället och Microsoft skickar skatten till det tillämpliga landet. Inga skatter från utbetalnings-och utbetalnings beräkningar är skattemässiga exklusive moms.

Se [scenario D](#foreign-publisher-transacts-with-us-customer) för transaktioner mellan en icke-amerikansk utgivare och en kund hos oss.

:::image type="content" source="images/tax-policies/payout-scenario-a.png" alt-text="Visar arbets flöde för utbetalnings process scenariot A.":::

## <a name="publisher-transacts-in-microsoft-managed-tax-country-where-marketplace-fee-is-taxable-service"></a>Utgivaren agerar i Microsoft-hanterade skattemyndigheter där Marketplace-avgiften är momspliktig

**Scenario B** – transaktioner som sker mellan en USA-baserad utgivare (enligt definitionen i deras skatte profil information för partner Center) till en kund i ett Microsoft-hanterat skatte land där landet tillämpar en skatt på Marketplace-avgiften (en momspliktig tjänst). I det här scenariot subtraheras skatten på butiks tjänst avgiften från utbetalningen av utgivaren.

:::image type="content" source="images/tax-policies/payout-scenario-b.png" alt-text="Visar arbets flöde för process scenario B för utbetalning.":::

## <a name="publisher-transacts-in-publisher-managed-tax-country"></a>Utgivaren agerar i Publisher-hanterat skatte land

**Scenario C** – transaktioner som sker mellan en utgivare och en kund i ett Publisher-hanterat skatte land som inte har någon käll skatt för kunder. Kunderna betalar ingen skatt vid inköps tillfället och det är utgivarens skyldighet att betala alla tillämpliga skatter.

Mer information om landsspecifika priser (till exempel för att förskjuta kommande beskattning) finns i [planer och priser för kommersiella Marketplace-erbjudanden](/azure/marketplace/plans-pricing#custom-prices).

:::image type="content" source="images/tax-policies/payout-scenario-c.png" alt-text="Visar arbets flöde för utbetalnings process scenario C.":::

## <a name="foreign-publisher-transacts-with-us-customer"></a>Utländska utgivare samverkar med oss-kund

**Scenario D** – alla externa utgivare (enligt definitionen i deras skatte profil information för partner Center) i länder utan ett amerikanskt avtal (se [scenario E](#foreign-publisher-with-a-treaty-transacts-with-us-customer)) som gör en försäljning till en USA-baserad kund (enligt definitionen i deras kund konto adress). AMERIKANSKA myndigheter kräver att Microsoft undanhålle skatt för utgivarens räkning. Skatte deklaration från utbetalning till utgivare beräknas utifrån erbjudande priset.

:::image type="content" source="images/tax-policies/payout-scenario-d.png" alt-text="Visar arbets flöde för process scenario för utbetalning D.":::

## <a name="foreign-publisher-with-a-treaty-transacts-with-us-customer"></a>Utländsk utgivare med ett fördrag samverkar med oss-kund

**Scenario E** – alla externa utgivare (enligt definitionen i deras skatte profil information för partner Center) i länder med ett amerikanska fördrag som gör en försäljning till en amerikansk kund (enligt definitionen i deras kund konto adress). AMERIKANSKA myndigheter behöver inte Microsoft för att betala för utgivarens räkning.

:::image type="content" source="images/tax-policies/payout-scenario-e.png" alt-text="Visar ett arbets flöde för utbetalnings process scenario E.":::

## <a name="foreign-publisher-sells-to-an-eu-vat-registered-customer-in-a-microsoft-managed-country-outside-ireland"></a>Utländsk utgivare säljer till en kund som registrerats av EU i ett Microsoft-hanterat land (utanför Irland)

**Scenario F** – alla transaktioner mellan utländska utgivare och moms register som registrerats av EU (utanför Irland) i ett Microsoft-Managed land. Kunden betalar inte skatt på försäljningen.

:::image type="content" source="images/tax-policies/payout-scenario-f.png" alt-text="Visar arbets flöde för utbetalnings process scenario F.":::

## <a name="foreign-publisher-sells-to-an-eu-vat-registered-customer-in-a-microsoft-managed-country-in-ireland"></a>Utländsk utgivare säljer till en kund som registrerats av EU i ett Microsoft-hanterat land (i Irland)

**Scenario G** – alla transaktioner mellan utländska utgivare och moms register som registrerats av EU (i Irland) i ett Microsoft-Managed land. Kunden betalar irländsk moms och Microsoft betalar skatten till den irländska regeringen.

:::image type="content" source="images/tax-policies/payout-scenario-g.png" alt-text="Visar arbets flöde för process scenario för utbetalnings processen G.":::

## <a name="next-steps"></a>Nästa steg

- [Vanliga frågor och svar om Publisher](/azure/marketplace/marketplace-faq-publisher-guide)
- [Instruktioner för att skapa betalnings-och skatte profiler](./set-up-your-payout-account.md?context=%2fazure%2fmarketplace%2fcontext%2fcontext#create-a-payment-profile)