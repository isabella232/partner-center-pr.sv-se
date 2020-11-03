---
title: Avstämnings fil debiterings typer
ms.topic: article
ms.date: 06/05/2020
description: Identifiera typer av avgifter (till exempel licensbaserade, användnings och engångs), krediter och rabatter i filer för partner Center-avstämning.
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: f65c4a6496082934e8c38fbd924b96ef969be95b
ms.sourcegitcommit: e7931fbe7ce16a62124e00b2802520a17d7285b8
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 07/31/2020
ms.locfileid: "92531116"
---
# <a name="understand-the-different-charge-types-in-partner-center-reconciliation-files"></a><span data-ttu-id="cf3f3-103">Förstå de olika debiterings typerna i filer för partner Center-avstämning</span><span class="sxs-lookup"><span data-stu-id="cf3f3-103">Understand the different charge types in Partner Center reconciliation files</span></span>

<span data-ttu-id="cf3f3-104">**Gäller för**</span><span class="sxs-lookup"><span data-stu-id="cf3f3-104">**Applies to**</span></span>

- <span data-ttu-id="cf3f3-105">Partnercenter</span><span class="sxs-lookup"><span data-stu-id="cf3f3-105">Partner Center</span></span>
- <span data-ttu-id="cf3f3-106">Partner Center för Microsoft Cloud för amerikanska myndigheter</span><span class="sxs-lookup"><span data-stu-id="cf3f3-106">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="cf3f3-107">**Lämpliga roller**</span><span class="sxs-lookup"><span data-stu-id="cf3f3-107">**Appropriate roles**</span></span>

- <span data-ttu-id="cf3f3-108">Administratörs agent</span><span class="sxs-lookup"><span data-stu-id="cf3f3-108">Admin agent</span></span>
- <span data-ttu-id="cf3f3-109">Faktureringsadministratör</span><span class="sxs-lookup"><span data-stu-id="cf3f3-109">Billing admin</span></span>
- <span data-ttu-id="cf3f3-110">Global administratör</span><span class="sxs-lookup"><span data-stu-id="cf3f3-110">Global admin</span></span>

<span data-ttu-id="cf3f3-111">I det här avsnittet beskrivs mappningarna mellan avsnittet faktura och associerade avgifts typer som kan finnas i avstämnings filen.</span><span class="sxs-lookup"><span data-stu-id="cf3f3-111">This topic describes the mappings between an invoice section and associated charge types that might be on your reconciliation file.</span></span> <span data-ttu-id="cf3f3-112">Fakturan innehåller en sammanfattning av avgifter.</span><span class="sxs-lookup"><span data-stu-id="cf3f3-112">Your invoice provides a summary of charges.</span></span> <span data-ttu-id="cf3f3-113">Din avstämnings fil innehåller en detaljerad uppdelning av rad artikel transaktioner, inklusive avgifts typer.</span><span class="sxs-lookup"><span data-stu-id="cf3f3-113">Your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span> <span data-ttu-id="cf3f3-114">Mer information om avstämnings filer finns i [så här använder du avstämnings filer](use-the-reconciliation-files.md).</span><span class="sxs-lookup"><span data-stu-id="cf3f3-114">For more information on reconciliation files, see [how to use reconciliation files](use-the-reconciliation-files.md).</span></span>

<span data-ttu-id="cf3f3-115">Både [användnings avstämnings filer](usage-based-recon-files.md) och [licensbaserade avstämnings filer](license-based-recon-files.md) visar bara användnings-relaterade transaktioner och avgifter (förbrukade enheter och relaterade avgifter).</span><span class="sxs-lookup"><span data-stu-id="cf3f3-115">Both [usage-based reconciliation files](usage-based-recon-files.md) and [license-based reconciliation files](license-based-recon-files.md) only show usage-related transactions and charges (units consumed and related charges).</span></span>

> [!NOTE]
> <span data-ttu-id="cf3f3-116">En eller flera krediter, rabatter eller åter betalningar som visas på fakturan när **justeringar** inte visas i avstämnings filen.</span><span class="sxs-lookup"><span data-stu-id="cf3f3-116">One-off credits, discounts or refunds that appear on the invoice as **Adjustments** are not shown in the reconciliation file.</span></span>

## <a name="map-charge-types-to-invoice-charges"></a><span data-ttu-id="cf3f3-117">Mappa avgifts typer till faktura avgifter</span><span class="sxs-lookup"><span data-stu-id="cf3f3-117">Map charge types to invoice charges</span></span>

<span data-ttu-id="cf3f3-118">Använd filter alternativen i Microsoft Excel för att välja mellan referenser mellan fakturor och avstämnings fil.</span><span class="sxs-lookup"><span data-stu-id="cf3f3-118">To cross-reference charge amounts between your invoice and reconciliation file, use the filter options in Microsoft Excel.</span></span> <span data-ttu-id="cf3f3-119">Filtrera efter debiterings typer i avstämnings filen för att mappa faktura avgifterna till en uppsättning med debiterings nivåer i avstämnings filen.</span><span class="sxs-lookup"><span data-stu-id="cf3f3-119">Filter by charge types on your reconciliation file to map the invoice charges to a set of charge breakdowns on the reconciliation file.</span></span>

## <a name="license-based-charges"></a><span data-ttu-id="cf3f3-120">Licensbaserade avgifter</span><span class="sxs-lookup"><span data-stu-id="cf3f3-120">License-based charges</span></span>

<span data-ttu-id="cf3f3-121">För att mappa dessa licensbaserade avgifter till din faktura, summerar du kolumnen **mängd** från den licensierade filen.</span><span class="sxs-lookup"><span data-stu-id="cf3f3-121">To map these license-based charges to your invoice, sum the **Amount** column from the license-based file.</span></span>

| <span data-ttu-id="cf3f3-122">Avgifts Beskrivning (ChargeType-kolumnen i avstämnings filen)</span><span class="sxs-lookup"><span data-stu-id="cf3f3-122">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="cf3f3-123">Avgifts förklaring</span><span class="sxs-lookup"><span data-stu-id="cf3f3-123">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="cf3f3-124">Aktiverings avgift</span><span class="sxs-lookup"><span data-stu-id="cf3f3-124">Activation fee</span></span> | <span data-ttu-id="cf3f3-125">Det belopp som debiteras kunden när de använder prenumerationen efter köpet.</span><span class="sxs-lookup"><span data-stu-id="cf3f3-125">The amount charged to the customer when they use the subscription after purchase.</span></span> |
| <span data-ttu-id="cf3f3-126">Annullera avgift</span><span class="sxs-lookup"><span data-stu-id="cf3f3-126">Cancel fee</span></span> | <span data-ttu-id="cf3f3-127">Proportionella avgifter som återbetalas till kunden när tillhör ande licenser ändras.</span><span class="sxs-lookup"><span data-stu-id="cf3f3-127">Prorated charges refunded to the customer when associated licenses are changed.</span></span> |
| <span data-ttu-id="cf3f3-128">Avbryt instans prograden</span><span class="sxs-lookup"><span data-stu-id="cf3f3-128">Cancel instance prorate</span></span> | <span data-ttu-id="cf3f3-129">Proportionella avgifter annulleras när kunden med en månatlig prenumeration har inaktiverat prenumerationen och tillhör ande licenser har ändrats inom samma månad.</span><span class="sxs-lookup"><span data-stu-id="cf3f3-129">Prorated charges canceled when customer with monthly subscription has subscription suspended and associated licenses changed within the same month.</span></span> |
| <span data-ttu-id="cf3f3-130">Cykel avgift</span><span class="sxs-lookup"><span data-stu-id="cf3f3-130">Cycle fee</span></span> | <span data-ttu-id="cf3f3-131">Periodiska avgifter för en prenumeration.</span><span class="sxs-lookup"><span data-stu-id="cf3f3-131">Periodic charges for a subscription.</span></span> |
| <span data-ttu-id="cf3f3-132">Prograder för cykel instans</span><span class="sxs-lookup"><span data-stu-id="cf3f3-132">Cycle instance prorate</span></span> | <span data-ttu-id="cf3f3-133">Beräknad kostnad som bedöms från kunden när tillhör ande licenser ändras.</span><span class="sxs-lookup"><span data-stu-id="cf3f3-133">Prorated charges assessed from the customer when associated licenses are changed.</span></span> |
| <span data-ttu-id="cf3f3-134">Betala avgifter när du avbryter</span><span class="sxs-lookup"><span data-stu-id="cf3f3-134">Prorate fees when cancel</span></span> | <span data-ttu-id="cf3f3-135">Proportionellt åter betalning för oanvänd del av tjänst vid annullering.</span><span class="sxs-lookup"><span data-stu-id="cf3f3-135">Prorated refund for unused portion of service upon cancellation.</span></span> |
| <span data-ttu-id="cf3f3-136">Prorate-avgifter vid omvandling bort från aktuellt erbjudande</span><span class="sxs-lookup"><span data-stu-id="cf3f3-136">Prorate fees when convert away from current offering</span></span> | <span data-ttu-id="cf3f3-137">Proportionella avgifter efter konvertering från den aktuella månads prenumerationen till en års prenumeration.</span><span class="sxs-lookup"><span data-stu-id="cf3f3-137">Prorated charges after converting away from the current monthly subscription to an annual subscription.</span></span> |
| <span data-ttu-id="cf3f3-138">Protaxa-avgifter vid konvertering till ett nytt erbjudande</span><span class="sxs-lookup"><span data-stu-id="cf3f3-138">Prorate fees when convert to a new offering</span></span> | <span data-ttu-id="cf3f3-139">Proportionella avgifter efter konvertering av en månatlig prenumeration till en ny års prenumeration.</span><span class="sxs-lookup"><span data-stu-id="cf3f3-139">Prorated charges after converting a monthly subscription to a new annual subscription.</span></span> |
| <span data-ttu-id="cf3f3-140">Betala avgifter vid köp</span><span class="sxs-lookup"><span data-stu-id="cf3f3-140">Prorate fees when purchase</span></span> | <span data-ttu-id="cf3f3-141">Avgifts typen för en prenumeration när du använder både månatlig eller årlig fakturering.</span><span class="sxs-lookup"><span data-stu-id="cf3f3-141">The charge type for a subscription when using both monthly or annual billing.</span></span> |
| <span data-ttu-id="cf3f3-142">Protaxa-avgift vid förnyelse</span><span class="sxs-lookup"><span data-stu-id="cf3f3-142">Prorate fee when renew</span></span> | <span data-ttu-id="cf3f3-143">Debiterade avgifter vid förnyelse av prenumerationen.</span><span class="sxs-lookup"><span data-stu-id="cf3f3-143">Prorated fees upon subscription renewal.</span></span> |
| <span data-ttu-id="cf3f3-144">Förnya avgift</span><span class="sxs-lookup"><span data-stu-id="cf3f3-144">Renew fee</span></span> | <span data-ttu-id="cf3f3-145">Avgift för att förnya en prenumeration</span><span class="sxs-lookup"><span data-stu-id="cf3f3-145">Charge for renewing a subscription</span></span> |
| <span data-ttu-id="cf3f3-146">Taxa för avgifter vid aktivering</span><span class="sxs-lookup"><span data-stu-id="cf3f3-146">Prorate fees when activate</span></span> | <span data-ttu-id="cf3f3-147">Debiteras avgifter från aktivering till slutet av fakturerings perioden.</span><span class="sxs-lookup"><span data-stu-id="cf3f3-147">Prorated fees from activation until end of billing period.</span></span> |

## <a name="one-time-charges"></a><span data-ttu-id="cf3f3-148">Engångs kostnader</span><span class="sxs-lookup"><span data-stu-id="cf3f3-148">One-time charges</span></span>

<span data-ttu-id="cf3f3-149">Om du vill mappa dessa engångs kostnader till din faktura, summerar du kolumnen **mängd** från den licensierade filen.</span><span class="sxs-lookup"><span data-stu-id="cf3f3-149">To map these one-time charges to your invoice, sum the **Amount** column from the license-based file.</span></span>

| <span data-ttu-id="cf3f3-150">Avgifts Beskrivning (ChargeType-kolumnen i avstämnings filen)</span><span class="sxs-lookup"><span data-stu-id="cf3f3-150">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="cf3f3-151">Avgifts förklaring</span><span class="sxs-lookup"><span data-stu-id="cf3f3-151">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="cf3f3-152">Ny</span><span class="sxs-lookup"><span data-stu-id="cf3f3-152">New</span></span> | <span data-ttu-id="cf3f3-153">Används när ett nytt inköp skapas.</span><span class="sxs-lookup"><span data-stu-id="cf3f3-153">Used when a new purchase is created.</span></span> |
| <span data-ttu-id="cf3f3-154">addQuantity</span><span class="sxs-lookup"><span data-stu-id="cf3f3-154">addQuantity</span></span> | <span data-ttu-id="cf3f3-155">Används både i åter betalningen av det ursprungliga köpet och den nya kvantiteten efter en ökning.</span><span class="sxs-lookup"><span data-stu-id="cf3f3-155">Used in both the refund of the original purchase and the new quantity after an increase.</span></span> |
| <span data-ttu-id="cf3f3-156">removeQuantity</span><span class="sxs-lookup"><span data-stu-id="cf3f3-156">removeQuantity</span></span> | <span data-ttu-id="cf3f3-157">Används både i åter betalningen av det ursprungliga köpet och den nya kvantiteten efter en minskning.</span><span class="sxs-lookup"><span data-stu-id="cf3f3-157">Used in both the refund of the original purchase and the new quantity after a decrease.</span></span> |
| <span data-ttu-id="cf3f3-158">Avbryt</span><span class="sxs-lookup"><span data-stu-id="cf3f3-158">Cancel</span></span> | <span data-ttu-id="cf3f3-159">Används när en prenumeration avbryts.</span><span class="sxs-lookup"><span data-stu-id="cf3f3-159">Used when a subscription is canceled.</span></span> |
| <span data-ttu-id="cf3f3-160">Konvertera</span><span class="sxs-lookup"><span data-stu-id="cf3f3-160">Convert</span></span> | <span data-ttu-id="cf3f3-161">Används när en licens uppgraderas men antalet licenser förblir oförändrat.</span><span class="sxs-lookup"><span data-stu-id="cf3f3-161">Used when a license is upgraded but the number of licenses remains unchanged.</span></span> |

## <a name="usage-charges"></a><span data-ttu-id="cf3f3-162">Avgifter för användning</span><span class="sxs-lookup"><span data-stu-id="cf3f3-162">Usage charges</span></span>

<span data-ttu-id="cf3f3-163">Om du vill mappa dessa användnings kostnader till din faktura, summerar du kolumnen **PretaxCharges** från den användnings filen.</span><span class="sxs-lookup"><span data-stu-id="cf3f3-163">To map these usage charges to your invoice, sum the **PretaxCharges** column from the usage-based file.</span></span>

| <span data-ttu-id="cf3f3-164">Avgifts Beskrivning (ChargeType-kolumnen i avstämnings filen)</span><span class="sxs-lookup"><span data-stu-id="cf3f3-164">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="cf3f3-165">Avgifts förklaring</span><span class="sxs-lookup"><span data-stu-id="cf3f3-165">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="cf3f3-166">Utvärdera användnings avgiften när du avbryter</span><span class="sxs-lookup"><span data-stu-id="cf3f3-166">Assess usage fee when cancel</span></span> | <span data-ttu-id="cf3f3-167">Åtkomst användnings avgift vid annullering för obetald användning under den aktuella fakturerings perioden.</span><span class="sxs-lookup"><span data-stu-id="cf3f3-167">Access usage fee upon cancellation for unpaid usage during the current billing period.</span></span> |
| <span data-ttu-id="cf3f3-168">Utvärdera användnings avgiften för den aktuella cykeln</span><span class="sxs-lookup"><span data-stu-id="cf3f3-168">Assess usage fee for current cycle</span></span> | <span data-ttu-id="cf3f3-169">Åtkomst användnings avgift för den aktuella fakturerings perioden.</span><span class="sxs-lookup"><span data-stu-id="cf3f3-169">Access usage fee for the current billing period.</span></span> |

### <a name="credits"></a><span data-ttu-id="cf3f3-170">Krediter</span><span class="sxs-lookup"><span data-stu-id="cf3f3-170">Credits</span></span>

<span data-ttu-id="cf3f3-171">För att mappa dessa krediter till din faktura:</span><span class="sxs-lookup"><span data-stu-id="cf3f3-171">To map these credits to your invoice:</span></span>

- <span data-ttu-id="cf3f3-172">Summera **TotalForCustomer** från den licensierade filen.</span><span class="sxs-lookup"><span data-stu-id="cf3f3-172">Sum the **TotalForCustomer** from the license-based file.</span></span>
- <span data-ttu-id="cf3f3-173">Summera kolumnen **PostTaxTotal** från den Usage-baserade filen.</span><span class="sxs-lookup"><span data-stu-id="cf3f3-173">Sum the **PostTaxTotal** column from the usage-based file.</span></span>

| <span data-ttu-id="cf3f3-174">Avgifts Beskrivning (ChargeType-kolumnen i avstämnings filen)</span><span class="sxs-lookup"><span data-stu-id="cf3f3-174">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="cf3f3-175">Avgifts förklaring</span><span class="sxs-lookup"><span data-stu-id="cf3f3-175">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="cf3f3-176">Förskjut ett linje objekt</span><span class="sxs-lookup"><span data-stu-id="cf3f3-176">Offset a line item</span></span> | <span data-ttu-id="cf3f3-177">Delvis eller fullständig åter betalning till ett rad objekt, inklusive skatt.</span><span class="sxs-lookup"><span data-stu-id="cf3f3-177">Partial or whole refund to a line item, including taxes.</span></span> |

### <a name="usage-based-discounts"></a><span data-ttu-id="cf3f3-178">Användnings rabatter</span><span class="sxs-lookup"><span data-stu-id="cf3f3-178">Usage-based discounts</span></span>

<span data-ttu-id="cf3f3-179">Om du vill mappa dessa användnings rabatter till din faktura, summerar du kolumnen **PretaxCharges** från den användnings filen.</span><span class="sxs-lookup"><span data-stu-id="cf3f3-179">To map these usage-based discounts to your invoice, sum the **PretaxCharges** column from the usage-based file.</span></span>

| <span data-ttu-id="cf3f3-180">Avgifts Beskrivning (ChargeType-kolumnen i avstämnings filen)</span><span class="sxs-lookup"><span data-stu-id="cf3f3-180">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="cf3f3-181">Avgifts förklaring</span><span class="sxs-lookup"><span data-stu-id="cf3f3-181">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="cf3f3-182">Aktiverings rabatt</span><span class="sxs-lookup"><span data-stu-id="cf3f3-182">Activation discount</span></span> | <span data-ttu-id="cf3f3-183">Rabatt som tillämpas när prenumerationen aktive ras.</span><span class="sxs-lookup"><span data-stu-id="cf3f3-183">Discount applied when subscription activated.</span></span> |
| <span data-ttu-id="cf3f3-184">Cykel rabatt</span><span class="sxs-lookup"><span data-stu-id="cf3f3-184">Cycle discount</span></span> | <span data-ttu-id="cf3f3-185">Rabatt som tillämpas på periodiska kostnader.</span><span class="sxs-lookup"><span data-stu-id="cf3f3-185">Discount applied on periodic charges.</span></span> |
| <span data-ttu-id="cf3f3-186">Förnya rabatt</span><span class="sxs-lookup"><span data-stu-id="cf3f3-186">Renew discount</span></span> | <span data-ttu-id="cf3f3-187">Rabatt som tillämpas när prenumerationen förnyas.</span><span class="sxs-lookup"><span data-stu-id="cf3f3-187">Discount applied when subscription renewed.</span></span> |
| <span data-ttu-id="cf3f3-188">Avbryt rabatt</span><span class="sxs-lookup"><span data-stu-id="cf3f3-188">Cancel discount</span></span> | <span data-ttu-id="cf3f3-189">Avgifter som tillämpas när rabatter annulleras.</span><span class="sxs-lookup"><span data-stu-id="cf3f3-189">Charges applied when discounts are canceled.</span></span> |

### <a name="license-based-discounts"></a><span data-ttu-id="cf3f3-190">Licensbaserade rabatter</span><span class="sxs-lookup"><span data-stu-id="cf3f3-190">License-based discounts</span></span>

<span data-ttu-id="cf3f3-191">Om du vill mappa licensbaserade rabatter till din faktura, summerar du kolumnen **TotalOtherDiscount** från den licensierade filen.</span><span class="sxs-lookup"><span data-stu-id="cf3f3-191">To map license-based discounts to your invoice, sum the **TotalOtherDiscount** column from the license-based file.</span></span>

<span data-ttu-id="cf3f3-192">*Licensbaserade rabatter kan tillämpas på flera debiterings typer.*</span><span class="sxs-lookup"><span data-stu-id="cf3f3-192">*License-based discounts may be applied to multiple charge types.*</span></span>
