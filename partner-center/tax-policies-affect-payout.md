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
# <a name="how-tax-policies-affect-payout-for-azure-marketplace"></a><span data-ttu-id="035b0-103">Så här påverkar skatte principer utbetalning för Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="035b0-103">How tax policies affect payout for Azure Marketplace</span></span>

<span data-ttu-id="035b0-104">**Lämpliga roller**</span><span class="sxs-lookup"><span data-stu-id="035b0-104">**Appropriate roles**</span></span>
-    <span data-ttu-id="035b0-105">Global administratör</span><span class="sxs-lookup"><span data-stu-id="035b0-105">Global admin</span></span>
-    <span data-ttu-id="035b0-106">Användaradministratör</span><span class="sxs-lookup"><span data-stu-id="035b0-106">User admin</span></span>
-    <span data-ttu-id="035b0-107">Administratörs agent</span><span class="sxs-lookup"><span data-stu-id="035b0-107">Admin agent</span></span>

## <a name="introduction"></a><span data-ttu-id="035b0-108">Introduktion</span><span class="sxs-lookup"><span data-stu-id="035b0-108">Introduction</span></span>

<span data-ttu-id="035b0-109">Microsofts kommersiella marknads plats har global räckvidd.</span><span class="sxs-lookup"><span data-stu-id="035b0-109">The Microsoft commercial marketplace has global reach.</span></span> <span data-ttu-id="035b0-110">Transaktioner sker över gränserna och beroende på var ISV och kund finns kan skatte konsekvenserna variera.</span><span class="sxs-lookup"><span data-stu-id="035b0-110">Transactions occur across borders and depending on where the ISV and the customer are located, tax implications can vary.</span></span> <span data-ttu-id="035b0-111">Microsoft AppSource och Azure Marketplace använder partner Centers skatte profil information för att fastställa ISV: s land.</span><span class="sxs-lookup"><span data-stu-id="035b0-111">Microsoft AppSource and Azure Marketplace use the Partner Center Tax Profile Information to determine the ISV's country.</span></span> <span data-ttu-id="035b0-112">För att fastställa kundens land kan du antingen använda kundens fakturerings information eller, om kunden är i EU, använda två olika informations delar.</span><span class="sxs-lookup"><span data-stu-id="035b0-112">To determine the customer's country, either use the customer's billing information or, if the customer is in the EU, we use two different pieces of information.</span></span>

<span data-ttu-id="035b0-113">För att bättre förstå följande scenarier, se tabellen med [skatte information](tax-details-marketplace.md) , som visar om Microsoft samlar in och betalar skatt för utgivarens räkning eller om detta ansvar tillhör utgivaren.</span><span class="sxs-lookup"><span data-stu-id="035b0-113">To better understand the following scenarios, refer to the [Tax details](tax-details-marketplace.md) table, which shows whether Microsoft collects and pays taxes on behalf of the publisher or if that responsibility belongs to the publisher.</span></span>

> [!NOTE]
> <span data-ttu-id="035b0-114">Alla exempel på försäljnings värden och skatte procent satser i det här avsnittet är endast avsedda som exempel, inte exakta siffror.</span><span class="sxs-lookup"><span data-stu-id="035b0-114">All examples sale values and tax percentages in this topic are for illustrative purposes only, not exact figures.</span></span>

## <a name="publisher-transacts-in-microsoft-managed-tax-country"></a><span data-ttu-id="035b0-115">Utgivaren agerar i Microsoft-hanterade skatte länder</span><span class="sxs-lookup"><span data-stu-id="035b0-115">Publisher Transacts in Microsoft-managed Tax Country</span></span>

<span data-ttu-id="035b0-116">**Scenario A** – transaktioner som sker mellan en utgivare och en kund i ett [Microsoft-hanterat skatte land](tax-details-marketplace.md#microsoft-managed-countries).</span><span class="sxs-lookup"><span data-stu-id="035b0-116">**Scenario A** – Transactions that take place between a publisher and a customer in a [Microsoft-managed tax country](tax-details-marketplace.md#microsoft-managed-countries).</span></span> <span data-ttu-id="035b0-117">De här transaktionerna kommer att ha en avgift som lagts till vid försäljnings tillfället och Microsoft skickar skatten till det tillämpliga landet.</span><span class="sxs-lookup"><span data-stu-id="035b0-117">These transactions will have applicable tax added at the time of sale and Microsoft sends that tax to the applicable country.</span></span> <span data-ttu-id="035b0-118">Inga skatter från utbetalnings-och utbetalnings beräkningar är skattemässiga exklusive moms.</span><span class="sxs-lookup"><span data-stu-id="035b0-118">No taxes are withheld from payout and payout calculations are tax exclusive.</span></span>

<span data-ttu-id="035b0-119">Se [scenario D](#foreign-publisher-transacts-with-us-customer) för transaktioner mellan en icke-amerikansk utgivare och en kund hos oss.</span><span class="sxs-lookup"><span data-stu-id="035b0-119">See [Scenario D](#foreign-publisher-transacts-with-us-customer) for transactions between a non-US publisher and a US customer.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-a.png" alt-text="Visar arbets flöde för utbetalnings process scenariot A.":::

## <a name="publisher-transacts-in-microsoft-managed-tax-country-where-marketplace-fee-is-taxable-service"></a><span data-ttu-id="035b0-121">Utgivaren agerar i Microsoft-hanterade skattemyndigheter där Marketplace-avgiften är momspliktig</span><span class="sxs-lookup"><span data-stu-id="035b0-121">Publisher Transacts in Microsoft-managed Tax Country where Marketplace Fee is Taxable Service</span></span>

<span data-ttu-id="035b0-122">**Scenario B** – transaktioner som sker mellan en USA-baserad utgivare (enligt definitionen i deras skatte profil information för partner Center) till en kund i ett Microsoft-hanterat skatte land där landet tillämpar en skatt på Marketplace-avgiften (en momspliktig tjänst).</span><span class="sxs-lookup"><span data-stu-id="035b0-122">**Scenario B** – Transactions that take place between a US-based publisher (as defined by their Partner Center Tax Profile Information) to a customer in a Microsoft-managed tax country where the country imposes a tax on the Marketplace Fee (a taxable service).</span></span> <span data-ttu-id="035b0-123">I det här scenariot subtraheras skatten på butiks tjänst avgiften från utbetalningen av utgivaren.</span><span class="sxs-lookup"><span data-stu-id="035b0-123">In this scenario, the tax on the store service fee is subtracted from the publisher's payout.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-b.png" alt-text="Visar arbets flöde för process scenario B för utbetalning.":::

## <a name="publisher-transacts-in-publisher-managed-tax-country"></a><span data-ttu-id="035b0-125">Utgivaren agerar i Publisher-hanterat skatte land</span><span class="sxs-lookup"><span data-stu-id="035b0-125">Publisher Transacts in Publisher-managed Tax Country</span></span>

<span data-ttu-id="035b0-126">**Scenario C** – transaktioner som sker mellan en utgivare och en kund i ett Publisher-hanterat skatte land som inte har någon käll skatt för kunder.</span><span class="sxs-lookup"><span data-stu-id="035b0-126">**Scenario C** – Transactions that take place between a publisher and a customer in a publisher-managed tax country that does not impose a withholding tax on customers.</span></span> <span data-ttu-id="035b0-127">Kunderna betalar ingen skatt vid inköps tillfället och det är utgivarens skyldighet att betala alla tillämpliga skatter.</span><span class="sxs-lookup"><span data-stu-id="035b0-127">Customers pay no tax at the point of sale and it is the publisher's obligation to pay all applicable taxes.</span></span>

<span data-ttu-id="035b0-128">Mer information om landsspecifika priser (till exempel för att förskjuta kommande beskattning) finns i [planer och priser för kommersiella Marketplace-erbjudanden](/azure/marketplace/plans-pricing#custom-prices).</span><span class="sxs-lookup"><span data-stu-id="035b0-128">For more information on country-specific pricing (for example, to offset upcoming taxation) see [Plans and pricing for commercial marketplace offers](/azure/marketplace/plans-pricing#custom-prices).</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-c.png" alt-text="Visar arbets flöde för utbetalnings process scenario C.":::

## <a name="foreign-publisher-transacts-with-us-customer"></a><span data-ttu-id="035b0-130">Utländska utgivare samverkar med oss-kund</span><span class="sxs-lookup"><span data-stu-id="035b0-130">Foreign Publisher Transacts with US Customer</span></span>

<span data-ttu-id="035b0-131">**Scenario D** – alla externa utgivare (enligt definitionen i deras skatte profil information för partner Center) i länder utan ett amerikanskt avtal (se [scenario E](#foreign-publisher-with-a-treaty-transacts-with-us-customer)) som gör en försäljning till en USA-baserad kund (enligt definitionen i deras kund konto adress).</span><span class="sxs-lookup"><span data-stu-id="035b0-131">**Scenario D** – All foreign publishers (as defined by their Partner Center Tax Profile Information) in countries without a US treaty (see [Scenario E](#foreign-publisher-with-a-treaty-transacts-with-us-customer)) making a sale to a US-based customer (as defined by their customer account address).</span></span> <span data-ttu-id="035b0-132">AMERIKANSKA myndigheter kräver att Microsoft undanhålle skatt för utgivarens räkning.</span><span class="sxs-lookup"><span data-stu-id="035b0-132">US government requires that Microsoft withhold tax on behalf of the publisher.</span></span> <span data-ttu-id="035b0-133">Skatte deklaration från utbetalning till utgivare beräknas utifrån erbjudande priset.</span><span class="sxs-lookup"><span data-stu-id="035b0-133">Tax withheld from payout to publisher is calculated based on offer price.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-d.png" alt-text="Visar arbets flöde för process scenario för utbetalning D.":::

## <a name="foreign-publisher-with-a-treaty-transacts-with-us-customer"></a><span data-ttu-id="035b0-135">Utländsk utgivare med ett fördrag samverkar med oss-kund</span><span class="sxs-lookup"><span data-stu-id="035b0-135">Foreign publisher with a Treaty Transacts with US customer</span></span>

<span data-ttu-id="035b0-136">**Scenario E** – alla externa utgivare (enligt definitionen i deras skatte profil information för partner Center) i länder med ett amerikanska fördrag som gör en försäljning till en amerikansk kund (enligt definitionen i deras kund konto adress).</span><span class="sxs-lookup"><span data-stu-id="035b0-136">**Scenario E** – All foreign publishers (as defined by their Partner Center Tax Profile Information) in countries with a US treaty making a sale to a US-based customer (as defined by their customer account address).</span></span> <span data-ttu-id="035b0-137">AMERIKANSKA myndigheter behöver inte Microsoft för att betala för utgivarens räkning.</span><span class="sxs-lookup"><span data-stu-id="035b0-137">US government does not require Microsoft to withhold tax on behalf of the publisher.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-e.png" alt-text="Visar ett arbets flöde för utbetalnings process scenario E.":::

## <a name="foreign-publisher-sells-to-an-eu-vat-registered-customer-in-a-microsoft-managed-country-outside-ireland"></a><span data-ttu-id="035b0-139">Utländsk utgivare säljer till en kund som registrerats av EU i ett Microsoft-hanterat land (utanför Irland)</span><span class="sxs-lookup"><span data-stu-id="035b0-139">Foreign publisher sells to an EU VAT-registered customer in a Microsoft-managed country (outside Ireland)</span></span>

<span data-ttu-id="035b0-140">**Scenario F** – alla transaktioner mellan utländska utgivare och moms register som registrerats av EU (utanför Irland) i ett Microsoft-Managed land.</span><span class="sxs-lookup"><span data-stu-id="035b0-140">**Scenario F** – All transactions between foreign publishers and EU VAT-registered customers (outside Ireland) in a Microsoft-Managed country.</span></span> <span data-ttu-id="035b0-141">Kunden betalar inte skatt på försäljningen.</span><span class="sxs-lookup"><span data-stu-id="035b0-141">The customer does not pay tax on the sale.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-f.png" alt-text="Visar arbets flöde för utbetalnings process scenario F.":::

## <a name="foreign-publisher-sells-to-an-eu-vat-registered-customer-in-a-microsoft-managed-country-in-ireland"></a><span data-ttu-id="035b0-143">Utländsk utgivare säljer till en kund som registrerats av EU i ett Microsoft-hanterat land (i Irland)</span><span class="sxs-lookup"><span data-stu-id="035b0-143">Foreign publisher sells to an EU VAT-registered customer in a Microsoft-managed country (in Ireland)</span></span>

<span data-ttu-id="035b0-144">**Scenario G** – alla transaktioner mellan utländska utgivare och moms register som registrerats av EU (i Irland) i ett Microsoft-Managed land.</span><span class="sxs-lookup"><span data-stu-id="035b0-144">**Scenario G** – All transactions between foreign publishers and EU VAT-registered customers (inside Ireland) in a Microsoft-Managed country.</span></span> <span data-ttu-id="035b0-145">Kunden betalar irländsk moms och Microsoft betalar skatten till den irländska regeringen.</span><span class="sxs-lookup"><span data-stu-id="035b0-145">The customer pays Irish VAT and Microsoft pays this tax to the Irish government.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-g.png" alt-text="Visar arbets flöde för process scenario för utbetalnings processen G.":::

## <a name="next-steps"></a><span data-ttu-id="035b0-147">Nästa steg</span><span class="sxs-lookup"><span data-stu-id="035b0-147">Next steps</span></span>

- [<span data-ttu-id="035b0-148">Vanliga frågor och svar om Publisher</span><span class="sxs-lookup"><span data-stu-id="035b0-148">Publisher FAQ</span></span>](/azure/marketplace/marketplace-faq-publisher-guide)
- [<span data-ttu-id="035b0-149">Instruktioner för att skapa betalnings-och skatte profiler</span><span class="sxs-lookup"><span data-stu-id="035b0-149">Instructions to create payment and tax profiles</span></span>](./set-up-your-payout-account.md?context=%2fazure%2fmarketplace%2fcontext%2fcontext#create-a-payment-profile)