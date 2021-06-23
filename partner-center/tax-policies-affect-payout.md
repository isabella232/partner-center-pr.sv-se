---
title: Hur skatteprinciper påverkar utbetalningen för Azure Marketplace
description: Lär dig hur skatteprinciper påverkar utbetalning för Azure Marketplace.
ms.topic: conceptual
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
author: mingshen-ms
ms.author: mingshen
ms.date: 02/09/2021
ms.openlocfilehash: 32c5cda9558aaaeddaf194eb8258ba732e2ac698
ms.sourcegitcommit: 09eabb559aae25518caf3f2a59ef16a3e123c207
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/23/2021
ms.locfileid: "112489976"
---
# <a name="how-tax-policies-affect-payout-for-azure-marketplace"></a><span data-ttu-id="552ba-103">Hur skatteprinciper påverkar utbetalningen för Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="552ba-103">How tax policies affect payout for Azure Marketplace</span></span>

<span data-ttu-id="552ba-104">**Lämpliga roller:** Global | Administratörsbehörighet för användarhantering | Administratörsagent</span><span class="sxs-lookup"><span data-stu-id="552ba-104">**Appropriate roles**: Global admin | User management admin | Admin agent</span></span>

## <a name="introduction"></a><span data-ttu-id="552ba-105">Introduktion</span><span class="sxs-lookup"><span data-stu-id="552ba-105">Introduction</span></span>

<span data-ttu-id="552ba-106">Microsofts kommersiella marknadsplats har global räckvidd.</span><span class="sxs-lookup"><span data-stu-id="552ba-106">The Microsoft commercial marketplace has global reach.</span></span> <span data-ttu-id="552ba-107">Transaktioner sker över gränser och beroende på var den oberoende programvaruleverantören (ISV) och kunden finns kan skattekonsekvenserna variera.</span><span class="sxs-lookup"><span data-stu-id="552ba-107">Transactions occur across borders and depending on where the independent software vendor (ISV) and the customer are located, tax implications can vary.</span></span> <span data-ttu-id="552ba-108">Microsoft AppSource och Azure Marketplace du använda skatteprofilinformationen för Partnercenter för att fastställa ISV:ens land.</span><span class="sxs-lookup"><span data-stu-id="552ba-108">Microsoft AppSource and Azure Marketplace use the Partner Center Tax Profile Information to determine the ISV's country.</span></span> <span data-ttu-id="552ba-109">För att fastställa kundens land använder vi antingen kundens faktureringsinformation eller, om kunden är i EU, två olika typer av information.</span><span class="sxs-lookup"><span data-stu-id="552ba-109">To determine the customer's country, either use the customer's billing information or, if the customer is in the EU, we use two different pieces of information.</span></span>

<span data-ttu-id="552ba-110">Mer information om följande scenarier [](tax-details-marketplace.md) finns i tabellen Skatteinformation, som visar om Microsoft samlar in och betalar skatter åt utgivaren eller om ansvaret tillhör utgivaren.</span><span class="sxs-lookup"><span data-stu-id="552ba-110">To better understand the following scenarios, refer to the [Tax details](tax-details-marketplace.md) table, which shows whether Microsoft collects and pays taxes on behalf of the publisher or if that responsibility belongs to the publisher.</span></span>

> [!NOTE]
> <span data-ttu-id="552ba-111">Alla exempel på försäljningsvärden och skatteprocent i det här avsnittet är endast avsedda för illustrerande syfte, inte exakta siffror.</span><span class="sxs-lookup"><span data-stu-id="552ba-111">All examples sale values and tax percentages in this topic are for illustrative purposes only, not exact figures.</span></span>

## <a name="publisher-transacts-in-microsoft-managed-tax-country"></a><span data-ttu-id="552ba-112">Utgivartransacts i Microsoft-hanterat skatteland</span><span class="sxs-lookup"><span data-stu-id="552ba-112">Publisher Transacts in Microsoft-managed Tax Country</span></span>

<span data-ttu-id="552ba-113">**Scenario A** – Transaktioner som sker mellan en utgivare och en kund i ett [Microsoft-hanterat skatteland](tax-details-marketplace.md#microsoft-managed-countries).</span><span class="sxs-lookup"><span data-stu-id="552ba-113">**Scenario A** – Transactions that take place between a publisher and a customer in a [Microsoft-managed tax country](tax-details-marketplace.md#microsoft-managed-countries).</span></span> <span data-ttu-id="552ba-114">Dessa transaktioner kommer att ha en tillämplig skatt som läggs till vid tidpunkten för försäljningen och Microsoft skickar den skatt till det tillämpliga landet.</span><span class="sxs-lookup"><span data-stu-id="552ba-114">These transactions will have applicable tax added at the time of sale and Microsoft sends that tax to the applicable country.</span></span> <span data-ttu-id="552ba-115">Inga skatter från utbetalnings- och utbetalningsberäkningar är skattese exklusiva.</span><span class="sxs-lookup"><span data-stu-id="552ba-115">No taxes are withheld from payout and payout calculations are tax exclusive.</span></span>

<span data-ttu-id="552ba-116">Se [Scenario D](#foreign-publisher-transacts-with-us-customer) för transaktioner mellan en icke-amerikansk utgivare och en amerikansk kund.</span><span class="sxs-lookup"><span data-stu-id="552ba-116">See [Scenario D](#foreign-publisher-transacts-with-us-customer) for transactions between a non-US publisher and a US customer.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-a.png" alt-text="Visar arbetsflödet för utbetalningsprocessscenario A.":::

## <a name="publisher-transacts-in-microsoft-managed-tax-country-where-marketplace-fee-is-taxable-service"></a><span data-ttu-id="552ba-118">Utgivartransacts i Microsoft-hanterat skatteland där Marketplace-avgiften är en taxerbar tjänst</span><span class="sxs-lookup"><span data-stu-id="552ba-118">Publisher Transacts in Microsoft-managed Tax Country where Marketplace Fee is Taxable Service</span></span>

<span data-ttu-id="552ba-119">**Scenario B** – Transaktioner som äger rum mellan en amerikansk utgivare (enligt definitionen i deras skatteprofilinformation för Partnercenter) till en kund i ett Microsoft-hanterat skatteland där landet inför en skatt på Marketplace-avgiften (en skattebar tjänst).</span><span class="sxs-lookup"><span data-stu-id="552ba-119">**Scenario B** – Transactions that take place between a US-based publisher (as defined by their Partner Center Tax Profile Information) to a customer in a Microsoft-managed tax country where the country imposes a tax on the Marketplace Fee (a taxable service).</span></span> <span data-ttu-id="552ba-120">I det här scenariot subtraheras avgiften för butikstjänsten från utgivarens utbetalning.</span><span class="sxs-lookup"><span data-stu-id="552ba-120">In this scenario, the tax on the store service fee is subtracted from the publisher's payout.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-b.png" alt-text="Visar arbetsflödet för utbetalningsprocessscenario B.":::

## <a name="publisher-transacts-in-publisher-managed-tax-country"></a><span data-ttu-id="552ba-122">Utgivartransacts i utgivar-hanterat skatteland</span><span class="sxs-lookup"><span data-stu-id="552ba-122">Publisher Transacts in Publisher-managed Tax Country</span></span>

<span data-ttu-id="552ba-123">**Scenario C** – Transaktioner som sker mellan en utgivare och en kund i ett utgivar-hanterat skatteland som inte inför källskatt för kunder.</span><span class="sxs-lookup"><span data-stu-id="552ba-123">**Scenario C** – Transactions that take place between a publisher and a customer in a publisher-managed tax country that does not impose a withholding tax on customers.</span></span> <span data-ttu-id="552ba-124">Kunder betalar ingen skatt vid försäljningsplatsen och det är utgivarens ansvar att betala alla tillämpliga skatter.</span><span class="sxs-lookup"><span data-stu-id="552ba-124">Customers pay no tax at the point of sale and it is the publisher's obligation to pay all applicable taxes.</span></span>

<span data-ttu-id="552ba-125">Mer information om landsspecifika priser (till exempel för att motverka kommande skatteförskjutning) finns i Planer och priser för [erbjudanden på den kommersiella marknadsplatsen.](/azure/marketplace/plans-pricing#custom-prices)</span><span class="sxs-lookup"><span data-stu-id="552ba-125">For more information on country-specific pricing (for example, to offset upcoming taxation) see [Plans and pricing for commercial marketplace offers](/azure/marketplace/plans-pricing#custom-prices).</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-c.png" alt-text="Visar arbetsflödet för utbetalningsprocessens scenario C.":::

## <a name="foreign-publisher-transacts-with-us-customer"></a><span data-ttu-id="552ba-127">Transaktioner från en främmande utgivare med en amerikansk kund</span><span class="sxs-lookup"><span data-stu-id="552ba-127">Foreign Publisher Transacts with US Customer</span></span>

<span data-ttu-id="552ba-128">**Scenario D** – Alla externa utgivare (enligt definitionen i sin Skatteprofilinformation för Partnercenter) i länder utan amerikanskt konto (se [Scenario E](#foreign-publisher-with-a-treaty-transacts-with-us-customer)) som gör en försäljning till en USA-baserad kund (enligt definitionen av kundens kontoadress).</span><span class="sxs-lookup"><span data-stu-id="552ba-128">**Scenario D** – All foreign publishers (as defined by their Partner Center Tax Profile Information) in countries without a US treaty (see [Scenario E](#foreign-publisher-with-a-treaty-transacts-with-us-customer)) making a sale to a US-based customer (as defined by their customer account address).</span></span> <span data-ttu-id="552ba-129">Amerikanska myndigheter kräver att Microsoft tar ut källskatt åt utgivaren.</span><span class="sxs-lookup"><span data-stu-id="552ba-129">US government requires that Microsoft withhold tax on behalf of the publisher.</span></span> <span data-ttu-id="552ba-130">Skatt från utbetalning till utgivare beräknas baserat på erbjudandepris.</span><span class="sxs-lookup"><span data-stu-id="552ba-130">Tax withheld from payout to publisher is calculated based on offer price.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-d.png" alt-text="Visar arbetsflödet för utbetalningsprocessens scenario D.":::

## <a name="foreign-publisher-with-a-treaty-transacts-with-us-customer"></a><span data-ttu-id="552ba-132">Främmande utgivare med transacts för transacts med amerikansk kund</span><span class="sxs-lookup"><span data-stu-id="552ba-132">Foreign publisher with a Treaty Transacts with US customer</span></span>

<span data-ttu-id="552ba-133">**Scenario E** – Alla externa utgivare (definieras av sin Skatteprofilinformation i Partnercenter) i länder där en amerikansk utgivare gör en försäljning till en USA-baserad kund (enligt definitionen av kundens kontoadress).</span><span class="sxs-lookup"><span data-stu-id="552ba-133">**Scenario E** – All foreign publishers (as defined by their Partner Center Tax Profile Information) in countries with a US treaty making a sale to a US-based customer (as defined by their customer account address).</span></span> <span data-ttu-id="552ba-134">Amerikanska myndigheter kräver inte att Microsoft källskatt för utgivarens räkning.</span><span class="sxs-lookup"><span data-stu-id="552ba-134">US government does not require Microsoft to withhold tax on behalf of the publisher.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-e.png" alt-text="Visar arbetsflödet för utbetalningsprocessscenario E.":::

## <a name="foreign-publisher-sells-to-an-eu-vat-registered-customer-in-a-microsoft-managed-country-outside-ireland"></a><span data-ttu-id="552ba-136">En extern utgivare säljer till en momsregistrerad kund i EU i ett Microsoft-hanterat land (utanför Irland)</span><span class="sxs-lookup"><span data-stu-id="552ba-136">Foreign publisher sells to an EU VAT-registered customer in a Microsoft-managed country (outside Ireland)</span></span>

<span data-ttu-id="552ba-137">**Scenario F** – Alla transaktioner mellan externa utgivare och EU-registrerade kunder (moms) (utanför Irland) i ett Microsoft-Managed land.</span><span class="sxs-lookup"><span data-stu-id="552ba-137">**Scenario F** – All transactions between foreign publishers and EU value-added tax (VAT)-registered customers (outside Ireland) in a Microsoft-Managed country.</span></span> <span data-ttu-id="552ba-138">Kunden betalar inte skatt för försäljningen.</span><span class="sxs-lookup"><span data-stu-id="552ba-138">The customer does not pay tax on the sale.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-f.png" alt-text="Visar arbetsflödet för utbetalningsprocessens scenario F.":::

## <a name="foreign-publisher-sells-to-an-eu-vat-registered-customer-in-a-microsoft-managed-country-in-ireland"></a><span data-ttu-id="552ba-140">En främmande utgivare säljer till en momsregistrerad kund i EU i ett Microsoft-hanterat land (i Irland)</span><span class="sxs-lookup"><span data-stu-id="552ba-140">Foreign publisher sells to an EU VAT-registered customer in a Microsoft-managed country (in Ireland)</span></span>

<span data-ttu-id="552ba-141">**Scenario G** – Alla transaktioner mellan externa utgivare och EU-momsregistrerade kunder (i Irland) i ett Microsoft-Managed land.</span><span class="sxs-lookup"><span data-stu-id="552ba-141">**Scenario G** – All transactions between foreign publishers and EU VAT-registered customers (inside Ireland) in a Microsoft-Managed country.</span></span> <span data-ttu-id="552ba-142">Kunden betalar Vat vat och Microsoft betalar den här momsen till den amerikanska staten.</span><span class="sxs-lookup"><span data-stu-id="552ba-142">The customer pays Irish VAT and Microsoft pays this tax to the Irish government.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-g.png" alt-text="Visar arbetsflöde för utbetalningsprocessscenario G.":::

## <a name="next-steps"></a><span data-ttu-id="552ba-144">Nästa steg</span><span class="sxs-lookup"><span data-stu-id="552ba-144">Next steps</span></span>

- [<span data-ttu-id="552ba-145">Vanliga frågor och svar om utgivare</span><span class="sxs-lookup"><span data-stu-id="552ba-145">Publisher FAQ</span></span>](/azure/marketplace/marketplace-faq-publisher-guide)
- [<span data-ttu-id="552ba-146">Anvisningar för att skapa betalnings- och skatteprofiler</span><span class="sxs-lookup"><span data-stu-id="552ba-146">Instructions to create payment and tax profiles</span></span>](./set-up-your-payout-account.md?context=%2fazure%2fmarketplace%2fcontext%2fcontext#create-a-payment-profile)