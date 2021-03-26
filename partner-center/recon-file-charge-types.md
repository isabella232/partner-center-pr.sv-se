---
title: Debiteringstyper i avstämningsfiler
ms.topic: article
ms.date: 06/05/2020
description: Identifiera typer av avgifter (till exempel licensbaserade, användnings och engångs), krediter och rabatter i filer för partner Center-avstämning.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: ba42ac5beb28a3cf819c54a86385fb79853cdcd0
ms.sourcegitcommit: 700150044ea4f1a0b96cb4caeb97d7197da29ef6
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/25/2021
ms.locfileid: "105549234"
---
# <a name="understand-the-different-charge-types-in-partner-center-reconciliation-files"></a><span data-ttu-id="e4661-103">Förstå de olika debiterings typerna i filer för partner Center-avstämning</span><span class="sxs-lookup"><span data-stu-id="e4661-103">Understand the different charge types in Partner Center reconciliation files</span></span>

<span data-ttu-id="e4661-104">**Gäller för**</span><span class="sxs-lookup"><span data-stu-id="e4661-104">**Applies to**</span></span>

- <span data-ttu-id="e4661-105">Partner Center för Microsoft myndighets moln</span><span class="sxs-lookup"><span data-stu-id="e4661-105">Partner Center for Microsoft Government cloud</span></span>

<span data-ttu-id="e4661-106">**Lämpliga roller**</span><span class="sxs-lookup"><span data-stu-id="e4661-106">**Appropriate roles**</span></span>

- <span data-ttu-id="e4661-107">Administratörs agent</span><span class="sxs-lookup"><span data-stu-id="e4661-107">Admin agent</span></span>
- <span data-ttu-id="e4661-108">Faktureringsadministratör</span><span class="sxs-lookup"><span data-stu-id="e4661-108">Billing admin</span></span>
- <span data-ttu-id="e4661-109">Global administratör</span><span class="sxs-lookup"><span data-stu-id="e4661-109">Global admin</span></span>

<span data-ttu-id="e4661-110">I den här artikeln beskrivs mappningarna mellan avsnittet faktura och tillhör ande avgifts typer som kan finnas i avstämnings filen.</span><span class="sxs-lookup"><span data-stu-id="e4661-110">This article describes the mappings between an invoice section and associated charge types that might be on your reconciliation file.</span></span> <span data-ttu-id="e4661-111">Fakturan innehåller en sammanfattning av avgifter.</span><span class="sxs-lookup"><span data-stu-id="e4661-111">Your invoice provides a summary of charges.</span></span> <span data-ttu-id="e4661-112">Din avstämnings fil innehåller en detaljerad uppdelning av rad artikel transaktioner, inklusive avgifts typer.</span><span class="sxs-lookup"><span data-stu-id="e4661-112">Your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span> <span data-ttu-id="e4661-113">Mer information om avstämnings filer finns i [så här använder du avstämnings filer](use-the-reconciliation-files.md).</span><span class="sxs-lookup"><span data-stu-id="e4661-113">For more information on reconciliation files, see [how to use reconciliation files](use-the-reconciliation-files.md).</span></span>

<span data-ttu-id="e4661-114">Både [användnings avstämnings filer](usage-based-recon-files.md) och [licensbaserade avstämnings filer](license-based-recon-files.md) visar bara användnings-relaterade transaktioner och avgifter (förbrukade enheter och relaterade avgifter).</span><span class="sxs-lookup"><span data-stu-id="e4661-114">Both [usage-based reconciliation files](usage-based-recon-files.md) and [license-based reconciliation files](license-based-recon-files.md) only show usage-related transactions and charges (units consumed and related charges).</span></span>

> [!NOTE]
> <span data-ttu-id="e4661-115">En eller flera krediter, rabatter eller åter betalningar som visas på fakturan när **justeringar** inte visas i avstämnings filen.</span><span class="sxs-lookup"><span data-stu-id="e4661-115">One-off credits, discounts or refunds that appear on the invoice as **Adjustments** are not shown in the reconciliation file.</span></span>

## <a name="map-charge-types-to-invoice-charges"></a><span data-ttu-id="e4661-116">Mappa avgifts typer till faktura avgifter</span><span class="sxs-lookup"><span data-stu-id="e4661-116">Map charge types to invoice charges</span></span>

<span data-ttu-id="e4661-117">Använd filter alternativen i Microsoft Excel för att välja mellan referenser mellan fakturor och avstämnings fil.</span><span class="sxs-lookup"><span data-stu-id="e4661-117">To cross-reference charge amounts between your invoice and reconciliation file, use the filter options in Microsoft Excel.</span></span> <span data-ttu-id="e4661-118">Filtrera efter debiterings typer i avstämnings filen för att mappa faktura avgifterna till en uppsättning med debiterings nivåer i avstämnings filen.</span><span class="sxs-lookup"><span data-stu-id="e4661-118">Filter by charge types on your reconciliation file to map the invoice charges to a set of charge breakdowns on the reconciliation file.</span></span>

## <a name="license-based-charges"></a><span data-ttu-id="e4661-119">Licensbaserade avgifter</span><span class="sxs-lookup"><span data-stu-id="e4661-119">License-based charges</span></span>

<span data-ttu-id="e4661-120">För att mappa dessa licensbaserade avgifter till din faktura, summerar du kolumnen **mängd** från den licensierade filen.</span><span class="sxs-lookup"><span data-stu-id="e4661-120">To map these license-based charges to your invoice, sum the **Amount** column from the license-based file.</span></span>

| <span data-ttu-id="e4661-121">Avgifts Beskrivning (ChargeType-kolumnen i avstämnings filen)</span><span class="sxs-lookup"><span data-stu-id="e4661-121">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="e4661-122">Avgifts förklaring</span><span class="sxs-lookup"><span data-stu-id="e4661-122">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="e4661-123">Aktiverings avgift</span><span class="sxs-lookup"><span data-stu-id="e4661-123">Activation fee</span></span> | <span data-ttu-id="e4661-124">Det belopp som debiteras kunden när de använder prenumerationen efter köpet.</span><span class="sxs-lookup"><span data-stu-id="e4661-124">The amount charged to the customer when they use the subscription after purchase.</span></span> |
| <span data-ttu-id="e4661-125">Annullera avgift</span><span class="sxs-lookup"><span data-stu-id="e4661-125">Cancel fee</span></span> | <span data-ttu-id="e4661-126">Proportionella avgifter som återbetalas till kunden när tillhör ande licenser ändras.</span><span class="sxs-lookup"><span data-stu-id="e4661-126">Prorated charges refunded to the customer when associated licenses are changed.</span></span> |
| <span data-ttu-id="e4661-127">Avbryt instans prograden</span><span class="sxs-lookup"><span data-stu-id="e4661-127">Cancel instance prorate</span></span> | <span data-ttu-id="e4661-128">Proportionella avgifter annulleras när kunden med en månatlig prenumeration har inaktiverat prenumerationen och tillhör ande licenser har ändrats inom samma månad.</span><span class="sxs-lookup"><span data-stu-id="e4661-128">Prorated charges canceled when customer with monthly subscription has subscription suspended and associated licenses changed within the same month.</span></span> |
| <span data-ttu-id="e4661-129">Cykel avgift</span><span class="sxs-lookup"><span data-stu-id="e4661-129">Cycle fee</span></span> | <span data-ttu-id="e4661-130">Periodiska avgifter för en prenumeration.</span><span class="sxs-lookup"><span data-stu-id="e4661-130">Periodic charges for a subscription.</span></span> |
| <span data-ttu-id="e4661-131">Prograder för cykel instans</span><span class="sxs-lookup"><span data-stu-id="e4661-131">Cycle instance prorate</span></span> | <span data-ttu-id="e4661-132">Beräknad kostnad som bedöms från kunden när tillhör ande licenser ändras.</span><span class="sxs-lookup"><span data-stu-id="e4661-132">Prorated charges assessed from the customer when associated licenses are changed.</span></span> |
| <span data-ttu-id="e4661-133">Betala avgifter när du avbryter</span><span class="sxs-lookup"><span data-stu-id="e4661-133">Prorate fees when cancel</span></span> | <span data-ttu-id="e4661-134">Proportionellt åter betalning för oanvänd del av tjänst vid annullering.</span><span class="sxs-lookup"><span data-stu-id="e4661-134">Prorated refund for unused portion of service upon cancellation.</span></span> |
| <span data-ttu-id="e4661-135">Prorate-avgifter vid omvandling bort från aktuellt erbjudande</span><span class="sxs-lookup"><span data-stu-id="e4661-135">Prorate fees when convert away from current offering</span></span> | <span data-ttu-id="e4661-136">Proportionella avgifter efter konvertering från den aktuella månads prenumerationen till en års prenumeration.</span><span class="sxs-lookup"><span data-stu-id="e4661-136">Prorated charges after converting away from the current monthly subscription to an annual subscription.</span></span> |
| <span data-ttu-id="e4661-137">Protaxa-avgifter vid konvertering till ett nytt erbjudande</span><span class="sxs-lookup"><span data-stu-id="e4661-137">Prorate fees when convert to a new offering</span></span> | <span data-ttu-id="e4661-138">Proportionella avgifter efter konvertering av en månatlig prenumeration till en ny års prenumeration.</span><span class="sxs-lookup"><span data-stu-id="e4661-138">Prorated charges after converting a monthly subscription to a new annual subscription.</span></span> |
| <span data-ttu-id="e4661-139">Betala avgifter vid köp</span><span class="sxs-lookup"><span data-stu-id="e4661-139">Prorate fees when purchase</span></span> | <span data-ttu-id="e4661-140">Avgifts typen för en prenumeration när du använder både månatlig eller årlig fakturering.</span><span class="sxs-lookup"><span data-stu-id="e4661-140">The charge type for a subscription when using both monthly or annual billing.</span></span> |
| <span data-ttu-id="e4661-141">Protaxa-avgift vid förnyelse</span><span class="sxs-lookup"><span data-stu-id="e4661-141">Prorate fee when renew</span></span> | <span data-ttu-id="e4661-142">Debiterade avgifter vid förnyelse av prenumerationen.</span><span class="sxs-lookup"><span data-stu-id="e4661-142">Prorated fees upon subscription renewal.</span></span> |
| <span data-ttu-id="e4661-143">Förnya avgift</span><span class="sxs-lookup"><span data-stu-id="e4661-143">Renew fee</span></span> | <span data-ttu-id="e4661-144">Avgift för att förnya en prenumeration</span><span class="sxs-lookup"><span data-stu-id="e4661-144">Charge for renewing a subscription</span></span> |
| <span data-ttu-id="e4661-145">Taxa för avgifter vid aktivering</span><span class="sxs-lookup"><span data-stu-id="e4661-145">Prorate fees when activate</span></span> | <span data-ttu-id="e4661-146">Debiteras avgifter från aktivering till slutet av fakturerings perioden.</span><span class="sxs-lookup"><span data-stu-id="e4661-146">Prorated fees from activation until end of billing period.</span></span> |

## <a name="one-time-charges"></a><span data-ttu-id="e4661-147">Engångs kostnader</span><span class="sxs-lookup"><span data-stu-id="e4661-147">One-time charges</span></span>

<span data-ttu-id="e4661-148">Om du vill mappa dessa engångs kostnader till din faktura, summerar du kolumnen **mängd** från den licensierade filen.</span><span class="sxs-lookup"><span data-stu-id="e4661-148">To map these one-time charges to your invoice, sum the **Amount** column from the license-based file.</span></span>

| <span data-ttu-id="e4661-149">Avgifts Beskrivning (ChargeType-kolumnen i avstämnings filen)</span><span class="sxs-lookup"><span data-stu-id="e4661-149">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="e4661-150">Avgifts förklaring</span><span class="sxs-lookup"><span data-stu-id="e4661-150">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="e4661-151">Ny</span><span class="sxs-lookup"><span data-stu-id="e4661-151">New</span></span> | <span data-ttu-id="e4661-152">Används när ett nytt inköp skapas.</span><span class="sxs-lookup"><span data-stu-id="e4661-152">Used when a new purchase is created.</span></span> |
| <span data-ttu-id="e4661-153">addQuantity</span><span class="sxs-lookup"><span data-stu-id="e4661-153">addQuantity</span></span> | <span data-ttu-id="e4661-154">Används både i åter betalningen av det ursprungliga köpet och den nya kvantiteten efter en ökning.</span><span class="sxs-lookup"><span data-stu-id="e4661-154">Used in both the refund of the original purchase and the new quantity after an increase.</span></span> |
| <span data-ttu-id="e4661-155">removeQuantity</span><span class="sxs-lookup"><span data-stu-id="e4661-155">removeQuantity</span></span> | <span data-ttu-id="e4661-156">Används både i åter betalningen av det ursprungliga köpet och den nya kvantiteten efter en minskning.</span><span class="sxs-lookup"><span data-stu-id="e4661-156">Used in both the refund of the original purchase and the new quantity after a decrease.</span></span> |
| <span data-ttu-id="e4661-157">Avbryt</span><span class="sxs-lookup"><span data-stu-id="e4661-157">Cancel</span></span> | <span data-ttu-id="e4661-158">Används när en prenumeration avbryts.</span><span class="sxs-lookup"><span data-stu-id="e4661-158">Used when a subscription is canceled.</span></span> |
| <span data-ttu-id="e4661-159">Konvertera</span><span class="sxs-lookup"><span data-stu-id="e4661-159">Convert</span></span> | <span data-ttu-id="e4661-160">Används när en licens uppgraderas men antalet licenser förblir oförändrat.</span><span class="sxs-lookup"><span data-stu-id="e4661-160">Used when a license is upgraded but the number of licenses remains unchanged.</span></span> |

## <a name="usage-charges"></a><span data-ttu-id="e4661-161">Avgifter för användning</span><span class="sxs-lookup"><span data-stu-id="e4661-161">Usage charges</span></span>

<span data-ttu-id="e4661-162">Om du vill mappa dessa användnings kostnader till din faktura, summerar du kolumnen **PretaxCharges** från den användnings filen.</span><span class="sxs-lookup"><span data-stu-id="e4661-162">To map these usage charges to your invoice, sum the **PretaxCharges** column from the usage-based file.</span></span>

| <span data-ttu-id="e4661-163">Avgifts Beskrivning (ChargeType-kolumnen i avstämnings filen)</span><span class="sxs-lookup"><span data-stu-id="e4661-163">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="e4661-164">Avgifts förklaring</span><span class="sxs-lookup"><span data-stu-id="e4661-164">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="e4661-165">Utvärdera användnings avgiften när du avbryter</span><span class="sxs-lookup"><span data-stu-id="e4661-165">Assess usage fee when cancel</span></span> | <span data-ttu-id="e4661-166">Åtkomst användnings avgift vid annullering för obetald användning under den aktuella fakturerings perioden.</span><span class="sxs-lookup"><span data-stu-id="e4661-166">Access usage fee upon cancellation for unpaid usage during the current billing period.</span></span> |
| <span data-ttu-id="e4661-167">Utvärdera användnings avgiften för den aktuella cykeln</span><span class="sxs-lookup"><span data-stu-id="e4661-167">Assess usage fee for current cycle</span></span> | <span data-ttu-id="e4661-168">Åtkomst användnings avgift för den aktuella fakturerings perioden.</span><span class="sxs-lookup"><span data-stu-id="e4661-168">Access usage fee for the current billing period.</span></span> |

### <a name="credits"></a><span data-ttu-id="e4661-169">Krediter</span><span class="sxs-lookup"><span data-stu-id="e4661-169">Credits</span></span>

<span data-ttu-id="e4661-170">För att mappa dessa krediter till din faktura:</span><span class="sxs-lookup"><span data-stu-id="e4661-170">To map these credits to your invoice:</span></span>

- <span data-ttu-id="e4661-171">Summera **TotalForCustomer** från den licensierade filen.</span><span class="sxs-lookup"><span data-stu-id="e4661-171">Sum the **TotalForCustomer** from the license-based file.</span></span>
- <span data-ttu-id="e4661-172">Summera kolumnen **PostTaxTotal** från den Usage-baserade filen.</span><span class="sxs-lookup"><span data-stu-id="e4661-172">Sum the **PostTaxTotal** column from the usage-based file.</span></span>

| <span data-ttu-id="e4661-173">Avgifts Beskrivning (ChargeType-kolumnen i avstämnings filen)</span><span class="sxs-lookup"><span data-stu-id="e4661-173">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="e4661-174">Avgifts förklaring</span><span class="sxs-lookup"><span data-stu-id="e4661-174">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="e4661-175">Förskjut ett linje objekt</span><span class="sxs-lookup"><span data-stu-id="e4661-175">Offset a line item</span></span> | <span data-ttu-id="e4661-176">Delvis eller fullständig åter betalning till ett rad objekt, inklusive skatt.</span><span class="sxs-lookup"><span data-stu-id="e4661-176">Partial or whole refund to a line item, including taxes.</span></span> |

### <a name="usage-based-discounts"></a><span data-ttu-id="e4661-177">Användnings rabatter</span><span class="sxs-lookup"><span data-stu-id="e4661-177">Usage-based discounts</span></span>

<span data-ttu-id="e4661-178">Om du vill mappa dessa användnings rabatter till din faktura, summerar du kolumnen **PretaxCharges** från den användnings filen.</span><span class="sxs-lookup"><span data-stu-id="e4661-178">To map these usage-based discounts to your invoice, sum the **PretaxCharges** column from the usage-based file.</span></span>

| <span data-ttu-id="e4661-179">Avgifts Beskrivning (ChargeType-kolumnen i avstämnings filen)</span><span class="sxs-lookup"><span data-stu-id="e4661-179">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="e4661-180">Avgifts förklaring</span><span class="sxs-lookup"><span data-stu-id="e4661-180">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="e4661-181">Aktiverings rabatt</span><span class="sxs-lookup"><span data-stu-id="e4661-181">Activation discount</span></span> | <span data-ttu-id="e4661-182">Rabatt som tillämpas när prenumerationen aktive ras.</span><span class="sxs-lookup"><span data-stu-id="e4661-182">Discount applied when subscription activated.</span></span> |
| <span data-ttu-id="e4661-183">Cykel rabatt</span><span class="sxs-lookup"><span data-stu-id="e4661-183">Cycle discount</span></span> | <span data-ttu-id="e4661-184">Rabatt som tillämpas på periodiska kostnader.</span><span class="sxs-lookup"><span data-stu-id="e4661-184">Discount applied on periodic charges.</span></span> |
| <span data-ttu-id="e4661-185">Förnya rabatt</span><span class="sxs-lookup"><span data-stu-id="e4661-185">Renew discount</span></span> | <span data-ttu-id="e4661-186">Rabatt som tillämpas när prenumerationen förnyas.</span><span class="sxs-lookup"><span data-stu-id="e4661-186">Discount applied when subscription renewed.</span></span> |
| <span data-ttu-id="e4661-187">Avbryt rabatt</span><span class="sxs-lookup"><span data-stu-id="e4661-187">Cancel discount</span></span> | <span data-ttu-id="e4661-188">Avgifter som tillämpas när rabatter annulleras.</span><span class="sxs-lookup"><span data-stu-id="e4661-188">Charges applied when discounts are canceled.</span></span> |

### <a name="license-based-discounts"></a><span data-ttu-id="e4661-189">Licensbaserade rabatter</span><span class="sxs-lookup"><span data-stu-id="e4661-189">License-based discounts</span></span>

<span data-ttu-id="e4661-190">Om du vill mappa licensbaserade rabatter till din faktura, summerar du kolumnen **TotalOtherDiscount** från den licensierade filen.</span><span class="sxs-lookup"><span data-stu-id="e4661-190">To map license-based discounts to your invoice, sum the **TotalOtherDiscount** column from the license-based file.</span></span>

<span data-ttu-id="e4661-191">*Licensbaserade rabatter kan tillämpas på flera debiterings typer.*</span><span class="sxs-lookup"><span data-stu-id="e4661-191">*License-based discounts may be applied to multiple charge types.*</span></span>
