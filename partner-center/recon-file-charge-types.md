---
title: Debiteringstyper i avstämningsfiler
ms.topic: article
ms.date: 06/05/2020
description: Identifiera typer av avgifter (till exempel licensbaserade, användningsbaserade och en-gång), krediter och rabatter i Partner Center-avstämningsfiler.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 5a1f45de59fc9dac6a443bb8a14c3a80b36ba3f7
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 05/13/2021
ms.locfileid: "109855887"
---
# <a name="understand-the-different-charge-types-in-partner-center-reconciliation-files"></a><span data-ttu-id="49039-103">Förstå de olika avgiftstyperna i Avstämningsfiler för Partnercenter</span><span class="sxs-lookup"><span data-stu-id="49039-103">Understand the different charge types in Partner Center reconciliation files</span></span>

<span data-ttu-id="49039-104">**Gäller för:** Partner Center-| Partnercenter för Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="49039-104">**Applies to**: Partner Center | Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="49039-105">**Lämpliga roller:** Administratörsagent | Faktureringsadministratörskonto | Global administratör</span><span class="sxs-lookup"><span data-stu-id="49039-105">**Appropriate roles**: Admin agent | Billing admin | Global admin</span></span>

<span data-ttu-id="49039-106">I den här artikeln beskrivs mappningarna mellan ett fakturaavsnitt och associerade avgiftstyper som kan finnas i avstämningsfilen.</span><span class="sxs-lookup"><span data-stu-id="49039-106">This article describes the mappings between an invoice section and associated charge types that might be on your reconciliation file.</span></span> <span data-ttu-id="49039-107">Din faktura innehåller en sammanfattning av avgifterna.</span><span class="sxs-lookup"><span data-stu-id="49039-107">Your invoice provides a summary of charges.</span></span> <span data-ttu-id="49039-108">Avstämningsfilen innehåller en detaljerad analys av radobjekttransaktioner, inklusive avgiftstyper.</span><span class="sxs-lookup"><span data-stu-id="49039-108">Your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span> <span data-ttu-id="49039-109">Mer information om avstämningsfiler finns i [använda avstämningsfiler](use-the-reconciliation-files.md).</span><span class="sxs-lookup"><span data-stu-id="49039-109">For more information on reconciliation files, see [how to use reconciliation files](use-the-reconciliation-files.md).</span></span>

<span data-ttu-id="49039-110">Både [användningsbaserade avstämningsfiler](usage-based-recon-files.md) [och licensbaserade](license-based-recon-files.md) avstämningsfiler visar endast användningsrelaterade transaktioner och avgifter (förbrukade enheter och relaterade avgifter).</span><span class="sxs-lookup"><span data-stu-id="49039-110">Both [usage-based reconciliation files](usage-based-recon-files.md) and [license-based reconciliation files](license-based-recon-files.md) only show usage-related transactions and charges (units consumed and related charges).</span></span>

> [!NOTE]
> <span data-ttu-id="49039-111">Krediter, rabatter eller återbetalningar som visas på fakturan som Justeringar visas inte i **avstämningsfilen.**</span><span class="sxs-lookup"><span data-stu-id="49039-111">One-off credits, discounts or refunds that appear on the invoice as **Adjustments** are not shown in the reconciliation file.</span></span>

## <a name="map-charge-types-to-invoice-charges"></a><span data-ttu-id="49039-112">Mappa avgiftstyper till fakturaavgifter</span><span class="sxs-lookup"><span data-stu-id="49039-112">Map charge types to invoice charges</span></span>

<span data-ttu-id="49039-113">Om du vill korsreferensa avgiftsbeloppen mellan din faktura och avstämningsfil använder du filteralternativen i Microsoft Excel.</span><span class="sxs-lookup"><span data-stu-id="49039-113">To cross-reference charge amounts between your invoice and reconciliation file, use the filter options in Microsoft Excel.</span></span> <span data-ttu-id="49039-114">Filtrera efter avgiftstyper i avstämningsfilen för att mappa fakturade avgifterna till en uppsättning uppdelningar av avgifter i avstämningsfilen.</span><span class="sxs-lookup"><span data-stu-id="49039-114">Filter by charge types on your reconciliation file to map the invoice charges to a set of charge breakdowns on the reconciliation file.</span></span>

## <a name="license-based-charges"></a><span data-ttu-id="49039-115">Licensbaserade avgifter</span><span class="sxs-lookup"><span data-stu-id="49039-115">License-based charges</span></span>

<span data-ttu-id="49039-116">Om du vill mappa dessa licensbaserade avgifter till din faktura summerar **du kolumnen Amount** från den licensbaserade filen.</span><span class="sxs-lookup"><span data-stu-id="49039-116">To map these license-based charges to your invoice, sum the **Amount** column from the license-based file.</span></span>

| <span data-ttu-id="49039-117">Avgiftsbeskrivning (kolumnen ChargeType i avstämningsfilen)</span><span class="sxs-lookup"><span data-stu-id="49039-117">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="49039-118">Förklaring av avgifter</span><span class="sxs-lookup"><span data-stu-id="49039-118">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="49039-119">Aktiveringsavgift</span><span class="sxs-lookup"><span data-stu-id="49039-119">Activation fee</span></span> | <span data-ttu-id="49039-120">Det belopp som debiteras kunden när de använder prenumerationen efter köpet.</span><span class="sxs-lookup"><span data-stu-id="49039-120">The amount charged to the customer when they use the subscription after purchase.</span></span> |
| <span data-ttu-id="49039-121">Avbokningsavgift</span><span class="sxs-lookup"><span data-stu-id="49039-121">Cancel fee</span></span> | <span data-ttu-id="49039-122">Återbetalade avgifter till kunden när associerade licenser ändras.</span><span class="sxs-lookup"><span data-stu-id="49039-122">Prorated charges refunded to the customer when associated licenses are changed.</span></span> |
| <span data-ttu-id="49039-123">Avbryta instansprorate</span><span class="sxs-lookup"><span data-stu-id="49039-123">Cancel instance prorate</span></span> | <span data-ttu-id="49039-124">Avgiftsberäknade avgifter avbröts när en kund med månadsprenumeration pausade och associerade licenser ändrades under samma månad.</span><span class="sxs-lookup"><span data-stu-id="49039-124">Prorated charges canceled when customer with monthly subscription has subscription suspended and associated licenses changed within the same month.</span></span> |
| <span data-ttu-id="49039-125">Cykelavgift</span><span class="sxs-lookup"><span data-stu-id="49039-125">Cycle fee</span></span> | <span data-ttu-id="49039-126">Periodiska avgifter för en prenumeration.</span><span class="sxs-lookup"><span data-stu-id="49039-126">Periodic charges for a subscription.</span></span> |
| <span data-ttu-id="49039-127">Cykelinstansprorate</span><span class="sxs-lookup"><span data-stu-id="49039-127">Cycle instance prorate</span></span> | <span data-ttu-id="49039-128">Taxerade avgifter som utvärderas från kunden när associerade licenser ändras.</span><span class="sxs-lookup"><span data-stu-id="49039-128">Prorated charges assessed from the customer when associated licenses are changed.</span></span> |
| <span data-ttu-id="49039-129">Betala avgifter när du avbryter</span><span class="sxs-lookup"><span data-stu-id="49039-129">Prorate fees when cancel</span></span> | <span data-ttu-id="49039-130">Återbetalas i procent för oanvänd del av tjänsten vid annullering.</span><span class="sxs-lookup"><span data-stu-id="49039-130">Prorated refund for unused portion of service upon cancellation.</span></span> |
| <span data-ttu-id="49039-131">Prorate fees when convert away from current offering (Prorate-avgifter när de konverteras bort från det aktuella erbjudandet)</span><span class="sxs-lookup"><span data-stu-id="49039-131">Prorate fees when convert away from current offering</span></span> | <span data-ttu-id="49039-132">Räknade avgifter efter att ha konverterat bort från den aktuella månadsprenumerationen till en årlig prenumeration.</span><span class="sxs-lookup"><span data-stu-id="49039-132">Prorated charges after converting away from the current monthly subscription to an annual subscription.</span></span> |
| <span data-ttu-id="49039-133">Betala avgifter när du konverterar till ett nytt erbjudande</span><span class="sxs-lookup"><span data-stu-id="49039-133">Prorate fees when convert to a new offering</span></span> | <span data-ttu-id="49039-134">Prorerade avgifter efter konvertering av en månatlig prenumeration till en ny årsprenumeration.</span><span class="sxs-lookup"><span data-stu-id="49039-134">Prorated charges after converting a monthly subscription to a new annual subscription.</span></span> |
| <span data-ttu-id="49039-135">Betala avgifter vid köp</span><span class="sxs-lookup"><span data-stu-id="49039-135">Prorate fees when purchase</span></span> | <span data-ttu-id="49039-136">Avgiftstypen för en prenumeration när du använder både månatlig eller årlig fakturering.</span><span class="sxs-lookup"><span data-stu-id="49039-136">The charge type for a subscription when using both monthly or annual billing.</span></span> |
| <span data-ttu-id="49039-137">Betala avgifter vid förnyelse</span><span class="sxs-lookup"><span data-stu-id="49039-137">Prorate fee when renew</span></span> | <span data-ttu-id="49039-138">Prorerade avgifter vid prenumerationsförnyelse.</span><span class="sxs-lookup"><span data-stu-id="49039-138">Prorated fees upon subscription renewal.</span></span> |
| <span data-ttu-id="49039-139">Förnya avgift</span><span class="sxs-lookup"><span data-stu-id="49039-139">Renew fee</span></span> | <span data-ttu-id="49039-140">Avgift för att förnya en prenumeration</span><span class="sxs-lookup"><span data-stu-id="49039-140">Charge for renewing a subscription</span></span> |
| <span data-ttu-id="49039-141">Prorate fees when activate (Gå ut med avgifter när du aktiverar)</span><span class="sxs-lookup"><span data-stu-id="49039-141">Prorate fees when activate</span></span> | <span data-ttu-id="49039-142">Fakturerade avgifter från aktivering till slutet av faktureringsperioden.</span><span class="sxs-lookup"><span data-stu-id="49039-142">Prorated fees from activation until end of billing period.</span></span> |

## <a name="one-time-charges"></a><span data-ttu-id="49039-143">Avgifter för en gång</span><span class="sxs-lookup"><span data-stu-id="49039-143">One-time charges</span></span>

<span data-ttu-id="49039-144">Om du vill mappa dessa engångsavgifter till din faktura summerar **du kolumnen Amount** från den licensbaserade filen.</span><span class="sxs-lookup"><span data-stu-id="49039-144">To map these one-time charges to your invoice, sum the **Amount** column from the license-based file.</span></span>

| <span data-ttu-id="49039-145">Avgiftsbeskrivning (kolumnen ChargeType i avstämningsfilen)</span><span class="sxs-lookup"><span data-stu-id="49039-145">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="49039-146">Förklaring av avgifter</span><span class="sxs-lookup"><span data-stu-id="49039-146">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="49039-147">Ny</span><span class="sxs-lookup"><span data-stu-id="49039-147">New</span></span> | <span data-ttu-id="49039-148">Används när ett nytt köp skapas.</span><span class="sxs-lookup"><span data-stu-id="49039-148">Used when a new purchase is created.</span></span> |
| <span data-ttu-id="49039-149">addQuantity</span><span class="sxs-lookup"><span data-stu-id="49039-149">addQuantity</span></span> | <span data-ttu-id="49039-150">Används i både återbetalningen av det ursprungliga köpet och den nya kvantiteten efter en ökning.</span><span class="sxs-lookup"><span data-stu-id="49039-150">Used in both the refund of the original purchase and the new quantity after an increase.</span></span> |
| <span data-ttu-id="49039-151">removeQuantity</span><span class="sxs-lookup"><span data-stu-id="49039-151">removeQuantity</span></span> | <span data-ttu-id="49039-152">Används i både återbetalningen av det ursprungliga köpet och den nya kvantiteten efter en minskning.</span><span class="sxs-lookup"><span data-stu-id="49039-152">Used in both the refund of the original purchase and the new quantity after a decrease.</span></span> |
| <span data-ttu-id="49039-153">Avbryt</span><span class="sxs-lookup"><span data-stu-id="49039-153">Cancel</span></span> | <span data-ttu-id="49039-154">Används när en prenumeration avbryts.</span><span class="sxs-lookup"><span data-stu-id="49039-154">Used when a subscription is canceled.</span></span> |
| <span data-ttu-id="49039-155">Konvertera</span><span class="sxs-lookup"><span data-stu-id="49039-155">Convert</span></span> | <span data-ttu-id="49039-156">Används när en licens uppgraderas men antalet licenser förblir oförändrat.</span><span class="sxs-lookup"><span data-stu-id="49039-156">Used when a license is upgraded but the number of licenses remains unchanged.</span></span> |

## <a name="usage-charges"></a><span data-ttu-id="49039-157">Avgifter för användning</span><span class="sxs-lookup"><span data-stu-id="49039-157">Usage charges</span></span>

<span data-ttu-id="49039-158">Om du vill mappa dessa användningsavgifter till din faktura summerar du kolumnen **PretaxCharges** från den användningsbaserade filen.</span><span class="sxs-lookup"><span data-stu-id="49039-158">To map these usage charges to your invoice, sum the **PretaxCharges** column from the usage-based file.</span></span>

| <span data-ttu-id="49039-159">Avgiftsbeskrivning (kolumnen ChargeType i avstämningsfilen)</span><span class="sxs-lookup"><span data-stu-id="49039-159">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="49039-160">Förklaring av avgifter</span><span class="sxs-lookup"><span data-stu-id="49039-160">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="49039-161">Utvärdera användningsavgiften när du avbryter</span><span class="sxs-lookup"><span data-stu-id="49039-161">Assess usage fee when cancel</span></span> | <span data-ttu-id="49039-162">Åtkomstanvändningsavgift vid annullering för obetalt användning under den aktuella faktureringsperioden.</span><span class="sxs-lookup"><span data-stu-id="49039-162">Access usage fee upon cancellation for unpaid usage during the current billing period.</span></span> |
| <span data-ttu-id="49039-163">Utvärdera användningsavgiften för den aktuella cykeln</span><span class="sxs-lookup"><span data-stu-id="49039-163">Assess usage fee for current cycle</span></span> | <span data-ttu-id="49039-164">Åtkomstanvändningsavgift för den aktuella faktureringsperioden.</span><span class="sxs-lookup"><span data-stu-id="49039-164">Access usage fee for the current billing period.</span></span> |

### <a name="credits"></a><span data-ttu-id="49039-165">Krediter</span><span class="sxs-lookup"><span data-stu-id="49039-165">Credits</span></span>

<span data-ttu-id="49039-166">Så här mappar du dessa krediter till din faktura:</span><span class="sxs-lookup"><span data-stu-id="49039-166">To map these credits to your invoice:</span></span>

- <span data-ttu-id="49039-167">Summera **TotalForCustomer** från den licensbaserade filen.</span><span class="sxs-lookup"><span data-stu-id="49039-167">Sum the **TotalForCustomer** from the license-based file.</span></span>
- <span data-ttu-id="49039-168">Summera **kolumnen PostTaxTotal** från den användningsbaserade filen.</span><span class="sxs-lookup"><span data-stu-id="49039-168">Sum the **PostTaxTotal** column from the usage-based file.</span></span>

| <span data-ttu-id="49039-169">Avgiftsbeskrivning (kolumnen ChargeType i avstämningsfilen)</span><span class="sxs-lookup"><span data-stu-id="49039-169">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="49039-170">Förklaring av avgifter</span><span class="sxs-lookup"><span data-stu-id="49039-170">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="49039-171">Förskjut ett radobjekt</span><span class="sxs-lookup"><span data-stu-id="49039-171">Offset a line item</span></span> | <span data-ttu-id="49039-172">Partiell eller hel återbetalning till ett radobjekt, inklusive skatter.</span><span class="sxs-lookup"><span data-stu-id="49039-172">Partial or whole refund to a line item, including taxes.</span></span> |

### <a name="usage-based-discounts"></a><span data-ttu-id="49039-173">Användningsbaserade rabatter</span><span class="sxs-lookup"><span data-stu-id="49039-173">Usage-based discounts</span></span>

<span data-ttu-id="49039-174">Om du vill mappa dessa användningsbaserade rabatter till din faktura summerar du kolumnen **PretaxCharges** från den användningsbaserade filen.</span><span class="sxs-lookup"><span data-stu-id="49039-174">To map these usage-based discounts to your invoice, sum the **PretaxCharges** column from the usage-based file.</span></span>

| <span data-ttu-id="49039-175">Avgiftsbeskrivning (kolumnen ChargeType i avstämningsfilen)</span><span class="sxs-lookup"><span data-stu-id="49039-175">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="49039-176">Förklaring av avgifter</span><span class="sxs-lookup"><span data-stu-id="49039-176">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="49039-177">Aktiveringsrabatt</span><span class="sxs-lookup"><span data-stu-id="49039-177">Activation discount</span></span> | <span data-ttu-id="49039-178">Rabatt som tillämpas när prenumerationen aktiveras.</span><span class="sxs-lookup"><span data-stu-id="49039-178">Discount applied when subscription activated.</span></span> |
| <span data-ttu-id="49039-179">Cykelrabatt</span><span class="sxs-lookup"><span data-stu-id="49039-179">Cycle discount</span></span> | <span data-ttu-id="49039-180">Rabatt som tillämpas på periodiska avgifter.</span><span class="sxs-lookup"><span data-stu-id="49039-180">Discount applied on periodic charges.</span></span> |
| <span data-ttu-id="49039-181">Förnya rabatt</span><span class="sxs-lookup"><span data-stu-id="49039-181">Renew discount</span></span> | <span data-ttu-id="49039-182">Rabatt som tillämpas när prenumerationen förnyas.</span><span class="sxs-lookup"><span data-stu-id="49039-182">Discount applied when subscription renewed.</span></span> |
| <span data-ttu-id="49039-183">Avbryta rabatt</span><span class="sxs-lookup"><span data-stu-id="49039-183">Cancel discount</span></span> | <span data-ttu-id="49039-184">Avgifter som tillämpas när rabatter avbryts.</span><span class="sxs-lookup"><span data-stu-id="49039-184">Charges applied when discounts are canceled.</span></span> |

### <a name="license-based-discounts"></a><span data-ttu-id="49039-185">Licensbaserade rabatter</span><span class="sxs-lookup"><span data-stu-id="49039-185">License-based discounts</span></span>

<span data-ttu-id="49039-186">Om du vill mappa licensbaserade rabatter till din faktura **summerar du kolumnen TotalOtherDiscount** från den licensbaserade filen.</span><span class="sxs-lookup"><span data-stu-id="49039-186">To map license-based discounts to your invoice, sum the **TotalOtherDiscount** column from the license-based file.</span></span>

<span data-ttu-id="49039-187">*Licensbaserade rabatter kan tillämpas på flera avgiftstyper.*</span><span class="sxs-lookup"><span data-stu-id="49039-187">*License-based discounts may be applied to multiple charge types.*</span></span>
