---
title: Hur skatteprinciper påverkar utbetalningen för Azure Marketplace
description: Lär dig hur skatteprinciper påverkar utbetalning för Azure Marketplace.
ms.topic: conceptual
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
author: mingshen-ms
ms.author: mingshen
ms.date: 02/09/2021
ms.openlocfilehash: 343db43633245030a5eba213cb5c8b79d09a7dee
ms.sourcegitcommit: 08a175c06ff4c6a2b12713f081adfa489e16e7a1
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 05/10/2021
ms.locfileid: "109686321"
---
# <a name="how-tax-policies-affect-payout-for-azure-marketplace"></a><span data-ttu-id="89211-103">Hur skatteprinciper påverkar utbetalningen för Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="89211-103">How tax policies affect payout for Azure Marketplace</span></span>

<span data-ttu-id="89211-104">**Lämpliga roller**</span><span class="sxs-lookup"><span data-stu-id="89211-104">**Appropriate roles**</span></span>

- <span data-ttu-id="89211-105">Global administratör</span><span class="sxs-lookup"><span data-stu-id="89211-105">Global admin</span></span>
- <span data-ttu-id="89211-106">Administratör för användarhantering</span><span class="sxs-lookup"><span data-stu-id="89211-106">User management admin</span></span>
- <span data-ttu-id="89211-107">Administratörsagent</span><span class="sxs-lookup"><span data-stu-id="89211-107">Admin agent</span></span>

## <a name="introduction"></a><span data-ttu-id="89211-108">Introduktion</span><span class="sxs-lookup"><span data-stu-id="89211-108">Introduction</span></span>

<span data-ttu-id="89211-109">Microsofts kommersiella marknadsplats har global räckvidd.</span><span class="sxs-lookup"><span data-stu-id="89211-109">The Microsoft commercial marketplace has global reach.</span></span> <span data-ttu-id="89211-110">Transaktioner sker över gränser och beroende på var ISV:en och kunden finns kan skattekonsekvenserna variera.</span><span class="sxs-lookup"><span data-stu-id="89211-110">Transactions occur across borders and depending on where the ISV and the customer are located, tax implications can vary.</span></span> <span data-ttu-id="89211-111">Microsoft AppSource och Azure Marketplace du använda skatteprofilinformationen för Partnercenter för att fastställa ISV:ens land.</span><span class="sxs-lookup"><span data-stu-id="89211-111">Microsoft AppSource and Azure Marketplace use the Partner Center Tax Profile Information to determine the ISV's country.</span></span> <span data-ttu-id="89211-112">För att fastställa kundens land använder vi antingen kundens faktureringsinformation eller, om kunden är i EU, två olika uppgifter.</span><span class="sxs-lookup"><span data-stu-id="89211-112">To determine the customer's country, either use the customer's billing information or, if the customer is in the EU, we use two different pieces of information.</span></span>

<span data-ttu-id="89211-113">Mer information om följande scenarier [](tax-details-marketplace.md) finns i tabellen Skatteinformation, som visar om Microsoft samlar in och betalar skatter åt utgivaren eller om ansvaret tillhör utgivaren.</span><span class="sxs-lookup"><span data-stu-id="89211-113">To better understand the following scenarios, refer to the [Tax details](tax-details-marketplace.md) table, which shows whether Microsoft collects and pays taxes on behalf of the publisher or if that responsibility belongs to the publisher.</span></span>

> [!NOTE]
> <span data-ttu-id="89211-114">Alla exempel på försäljningsvärden och skatteprocent i det här avsnittet är endast avsedda för illustrerande syfte, inte exakta siffror.</span><span class="sxs-lookup"><span data-stu-id="89211-114">All examples sale values and tax percentages in this topic are for illustrative purposes only, not exact figures.</span></span>

## <a name="publisher-transacts-in-microsoft-managed-tax-country"></a><span data-ttu-id="89211-115">Utgivartransacts i Microsoft-hanterat skatteland</span><span class="sxs-lookup"><span data-stu-id="89211-115">Publisher Transacts in Microsoft-managed Tax Country</span></span>

<span data-ttu-id="89211-116">**Scenario A** – Transaktioner som sker mellan en utgivare och en kund i ett [Microsoft-hanterat skatteland](tax-details-marketplace.md#microsoft-managed-countries).</span><span class="sxs-lookup"><span data-stu-id="89211-116">**Scenario A** – Transactions that take place between a publisher and a customer in a [Microsoft-managed tax country](tax-details-marketplace.md#microsoft-managed-countries).</span></span> <span data-ttu-id="89211-117">Dessa transaktioner kommer att ha en tillämplig skatt som läggs till vid tidpunkten för försäljningen och Microsoft skickar den skatt till det tillämpliga landet.</span><span class="sxs-lookup"><span data-stu-id="89211-117">These transactions will have applicable tax added at the time of sale and Microsoft sends that tax to the applicable country.</span></span> <span data-ttu-id="89211-118">Inga skatter från utbetalnings- och utbetalningsberäkningar är skattese exklusiva.</span><span class="sxs-lookup"><span data-stu-id="89211-118">No taxes are withheld from payout and payout calculations are tax exclusive.</span></span>

<span data-ttu-id="89211-119">Se [Scenario D](#foreign-publisher-transacts-with-us-customer) för transaktioner mellan en icke-amerikansk utgivare och en amerikansk kund.</span><span class="sxs-lookup"><span data-stu-id="89211-119">See [Scenario D](#foreign-publisher-transacts-with-us-customer) for transactions between a non-US publisher and a US customer.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-a.png" alt-text="Visar arbetsflödet för utbetalningsprocessscenario A.":::

## <a name="publisher-transacts-in-microsoft-managed-tax-country-where-marketplace-fee-is-taxable-service"></a><span data-ttu-id="89211-121">Utgivartransacts i Microsoft-hanterat skatteland där Marketplace-avgiften är en taxerbar tjänst</span><span class="sxs-lookup"><span data-stu-id="89211-121">Publisher Transacts in Microsoft-managed Tax Country where Marketplace Fee is Taxable Service</span></span>

<span data-ttu-id="89211-122">**Scenario B** – Transaktioner som äger rum mellan en amerikansk utgivare (enligt definitionen i deras skatteprofilinformation för Partnercenter) till en kund i ett Microsoft-hanterat skatteland där landet inför en skatt på Marketplace-avgiften (en taxerbar tjänst).</span><span class="sxs-lookup"><span data-stu-id="89211-122">**Scenario B** – Transactions that take place between a US-based publisher (as defined by their Partner Center Tax Profile Information) to a customer in a Microsoft-managed tax country where the country imposes a tax on the Marketplace Fee (a taxable service).</span></span> <span data-ttu-id="89211-123">I det här scenariot subtraheras avgiften för butikstjänsten från utgivarens utbetalning.</span><span class="sxs-lookup"><span data-stu-id="89211-123">In this scenario, the tax on the store service fee is subtracted from the publisher's payout.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-b.png" alt-text="Visar arbetsflödet för utbetalningsprocessens scenario B.":::

## <a name="publisher-transacts-in-publisher-managed-tax-country"></a><span data-ttu-id="89211-125">Utgivartransacts i utgivar-hanterat skatteland</span><span class="sxs-lookup"><span data-stu-id="89211-125">Publisher Transacts in Publisher-managed Tax Country</span></span>

<span data-ttu-id="89211-126">**Scenario C** – Transaktioner som sker mellan en utgivare och en kund i ett utgivar hanterat skatteland som inte inför källskatt på kunder.</span><span class="sxs-lookup"><span data-stu-id="89211-126">**Scenario C** – Transactions that take place between a publisher and a customer in a publisher-managed tax country that does not impose a withholding tax on customers.</span></span> <span data-ttu-id="89211-127">Kunder betalar ingen skatt vid försäljningsplatsen och det är utgivarens ansvar att betala alla tillämpliga skatter.</span><span class="sxs-lookup"><span data-stu-id="89211-127">Customers pay no tax at the point of sale and it is the publisher's obligation to pay all applicable taxes.</span></span>

<span data-ttu-id="89211-128">Mer information om landsspecifika priser (till exempel för att uppväga kommande skatteförskjutning) finns i Plans and pricing for commercial marketplace offers (Planer och [priser för erbjudanden på den kommersiella marknadsplatsen).](/azure/marketplace/plans-pricing#custom-prices)</span><span class="sxs-lookup"><span data-stu-id="89211-128">For more information on country-specific pricing (for example, to offset upcoming taxation) see [Plans and pricing for commercial marketplace offers](/azure/marketplace/plans-pricing#custom-prices).</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-c.png" alt-text="Visar arbetsflödet för utbetalningsprocessens scenario C.":::

## <a name="foreign-publisher-transacts-with-us-customer"></a><span data-ttu-id="89211-130">Transacts för utgivare med amerikansk kund</span><span class="sxs-lookup"><span data-stu-id="89211-130">Foreign Publisher Transacts with US Customer</span></span>

<span data-ttu-id="89211-131">**Scenario D** – Alla externa utgivare (enligt definitionen i partnercentrets skatteprofilinformation) i länder utan amerikanskt konto (se [Scenario E](#foreign-publisher-with-a-treaty-transacts-with-us-customer)) som gör en försäljning till en USA-baserad kund (enligt definitionen av kundens kontoadress).</span><span class="sxs-lookup"><span data-stu-id="89211-131">**Scenario D** – All foreign publishers (as defined by their Partner Center Tax Profile Information) in countries without a US treaty (see [Scenario E](#foreign-publisher-with-a-treaty-transacts-with-us-customer)) making a sale to a US-based customer (as defined by their customer account address).</span></span> <span data-ttu-id="89211-132">Amerikanska myndigheter kräver att Microsoft källskatt för utgivarens räkning.</span><span class="sxs-lookup"><span data-stu-id="89211-132">US government requires that Microsoft withhold tax on behalf of the publisher.</span></span> <span data-ttu-id="89211-133">Skatt som upphöjs från utbetalning till utgivare beräknas baserat på erbjudandepris.</span><span class="sxs-lookup"><span data-stu-id="89211-133">Tax withheld from payout to publisher is calculated based on offer price.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-d.png" alt-text="Visar arbetsflödet för utbetalningsprocessens scenario D.":::

## <a name="foreign-publisher-with-a-treaty-transacts-with-us-customer"></a><span data-ttu-id="89211-135">Utgivare med transacts för transacts med amerikansk kund</span><span class="sxs-lookup"><span data-stu-id="89211-135">Foreign publisher with a Treaty Transacts with US customer</span></span>

<span data-ttu-id="89211-136">**Scenario E** – Alla externa utgivare (enligt definitionen i partnercentrets skatteprofilinformation) i länder där en amerikansk utgivare gör en försäljning till en USA-baserad kund (enligt definitionen av deras kundkontoadress).</span><span class="sxs-lookup"><span data-stu-id="89211-136">**Scenario E** – All foreign publishers (as defined by their Partner Center Tax Profile Information) in countries with a US treaty making a sale to a US-based customer (as defined by their customer account address).</span></span> <span data-ttu-id="89211-137">Amerikanska myndigheter kräver inte att Microsoft källskatt för utgivarens räkning.</span><span class="sxs-lookup"><span data-stu-id="89211-137">US government does not require Microsoft to withhold tax on behalf of the publisher.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-e.png" alt-text="Visar arbetsflödet för utbetalningsprocessens scenario E.":::

## <a name="foreign-publisher-sells-to-an-eu-vat-registered-customer-in-a-microsoft-managed-country-outside-ireland"></a><span data-ttu-id="89211-139">En extern utgivare säljer till en momsregistrerad kund i ett Microsoft-hanterat land (utanför Irland)</span><span class="sxs-lookup"><span data-stu-id="89211-139">Foreign publisher sells to an EU VAT-registered customer in a Microsoft-managed country (outside Ireland)</span></span>

<span data-ttu-id="89211-140">**Scenario F** – Alla transaktioner mellan externa utgivare och EU-momsregistrerade kunder (utanför Irland) i ett Microsoft-Managed land.</span><span class="sxs-lookup"><span data-stu-id="89211-140">**Scenario F** – All transactions between foreign publishers and EU VAT-registered customers (outside Ireland) in a Microsoft-Managed country.</span></span> <span data-ttu-id="89211-141">Kunden betalar inte skatt för försäljningen.</span><span class="sxs-lookup"><span data-stu-id="89211-141">The customer does not pay tax on the sale.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-f.png" alt-text="Visar arbetsflödet för utbetalningsprocessens scenario F.":::

## <a name="foreign-publisher-sells-to-an-eu-vat-registered-customer-in-a-microsoft-managed-country-in-ireland"></a><span data-ttu-id="89211-143">En främmande utgivare säljer till en momsregistrerad kund i EU i ett Microsoft-hanterat land (i Irland)</span><span class="sxs-lookup"><span data-stu-id="89211-143">Foreign publisher sells to an EU VAT-registered customer in a Microsoft-managed country (in Ireland)</span></span>

<span data-ttu-id="89211-144">**Scenario G** – Alla transaktioner mellan externa utgivare och EU-momsregistrerade kunder (i Irland) i ett Microsoft-Managed land.</span><span class="sxs-lookup"><span data-stu-id="89211-144">**Scenario G** – All transactions between foreign publishers and EU VAT-registered customers (inside Ireland) in a Microsoft-Managed country.</span></span> <span data-ttu-id="89211-145">Kunden betalar Moms och Microsoft betalar den här momsen till myndigheter i Usa.</span><span class="sxs-lookup"><span data-stu-id="89211-145">The customer pays Irish VAT and Microsoft pays this tax to the Irish government.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-g.png" alt-text="Visar arbetsflöde för utbetalningsprocessscenario G.":::

## <a name="next-steps"></a><span data-ttu-id="89211-147">Nästa steg</span><span class="sxs-lookup"><span data-stu-id="89211-147">Next steps</span></span>

- [<span data-ttu-id="89211-148">Vanliga frågor och svar om utgivare</span><span class="sxs-lookup"><span data-stu-id="89211-148">Publisher FAQ</span></span>](/azure/marketplace/marketplace-faq-publisher-guide)
- [<span data-ttu-id="89211-149">Anvisningar för att skapa betalnings- och skatteprofiler</span><span class="sxs-lookup"><span data-stu-id="89211-149">Instructions to create payment and tax profiles</span></span>](./set-up-your-payout-account.md?context=%2fazure%2fmarketplace%2fcontext%2fcontext#create-a-payment-profile)