---
title: Använd dina avstämnings filer
ms.topic: article
ms.date: 03/10/2021
description: Lär dig mer om avstämnings filer i Partner Center och hur du tolkar de detaljerade vyerna för rad artikel med debiteringar för en fakturerings period.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: e6b9e466402d71c988729052bd72ba2346a9d977
ms.sourcegitcommit: 868f90c54f26a037eee29749c207a7316bb4b475
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/11/2021
ms.locfileid: "103022782"
---
# <a name="learn-how-to-read-the-line-items-in-your-partner-center-reconciliation-files"></a><span data-ttu-id="58eac-103">Lär dig hur du läser rad objekt i dina avstämnings filer för partner Center</span><span class="sxs-lookup"><span data-stu-id="58eac-103">Learn how to read the line items in your Partner Center reconciliation files</span></span>

<span data-ttu-id="58eac-104">**Lämpliga roller**</span><span class="sxs-lookup"><span data-stu-id="58eac-104">**Appropriate roles**</span></span>

- <span data-ttu-id="58eac-105">Faktureringsadministratör</span><span class="sxs-lookup"><span data-stu-id="58eac-105">Billing admin</span></span>
- <span data-ttu-id="58eac-106">Global administratör</span><span class="sxs-lookup"><span data-stu-id="58eac-106">Global admin</span></span>

<span data-ttu-id="58eac-107">Du kan ladda ned dina avstämnings filer från Partner Center för en detaljerad, rad objekt visning av varje debitering i en fakturerings period.</span><span class="sxs-lookup"><span data-stu-id="58eac-107">You can download your reconciliation files from Partner Center for a detailed, line-item view of each charge in a billing cycle.</span></span> <span data-ttu-id="58eac-108">Information om rad objekt inkluderar avgifter för varje kunds prenumerationer och detaljerade händelser (till exempel ett omslags kort tillägg av licenser till en prenumeration).</span><span class="sxs-lookup"><span data-stu-id="58eac-108">Line-item details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of licenses to a subscription).</span></span>

<span data-ttu-id="58eac-109">Information om hur du läser fakturan finns i [läsa din](read-your-bill.md) **faktura**.</span><span class="sxs-lookup"><span data-stu-id="58eac-109">For information on how to read your **invoice**, see [Read your bill](read-your-bill.md).</span></span>

## <a name="understand-reconciliation-file-fields"></a><span data-ttu-id="58eac-110">Förstå fält för avstämnings fil</span><span class="sxs-lookup"><span data-stu-id="58eac-110">Understand reconciliation file fields</span></span>

- [<span data-ttu-id="58eac-111">Fält för licensbaserad avstämningsfil</span><span class="sxs-lookup"><span data-stu-id="58eac-111">License-based reconciliation file fields</span></span>](license-based-recon-files.md)
- [<span data-ttu-id="58eac-112">Fält för användningsbaserad avstämningsfil</span><span class="sxs-lookup"><span data-stu-id="58eac-112">Usage-based reconciliation file fields</span></span>](usage-based-recon-files.md)
- [<span data-ttu-id="58eac-113">Fält i fil för dagligt beräknad användningsavstämning</span><span class="sxs-lookup"><span data-stu-id="58eac-113">Daily-rated usage reconciliation file fields</span></span>](daily-rated-usage-recon-files.md)
- [<span data-ttu-id="58eac-114">Fil fält för CSP-avstämning för inköp vid ett tillfälle</span><span class="sxs-lookup"><span data-stu-id="58eac-114">One-time purchase CSP reconciliation file fields</span></span>](modern-invoice-reconciliation-file.md)

## <a name="understand-charge-types-in-reconciliation-files"></a><span data-ttu-id="58eac-115">Förstå debiterings typer i avstämnings filer</span><span class="sxs-lookup"><span data-stu-id="58eac-115">Understand charge types in reconciliation files</span></span>

<span data-ttu-id="58eac-116">Information om vilka typer av kostnader som finns i avstämnings filer (kolumnen **ChargeType** ) finns i [fil avgifts typer för avstämning](recon-file-charge-types.md).</span><span class="sxs-lookup"><span data-stu-id="58eac-116">To understand the types of charges in reconciliation files (the **ChargeType** column), see [Reconciliation file charge types](recon-file-charge-types.md).</span></span>

## <a name="fix-formatting-issues"></a><span data-ttu-id="58eac-117">Åtgärda problem med formatering</span><span class="sxs-lookup"><span data-stu-id="58eac-117">Fix formatting issues</span></span>

<span data-ttu-id="58eac-118">Ibland kan en avstämnings fil innehålla formateringsfel.</span><span class="sxs-lookup"><span data-stu-id="58eac-118">Occasionally, a reconciliation file might contain formatting issues.</span></span> <span data-ttu-id="58eac-119">Det här problemet kan till exempel inträffa om en-US locale inte används.</span><span class="sxs-lookup"><span data-stu-id="58eac-119">For example, this issue might occur if the en-US locale is not used.</span></span>

<span data-ttu-id="58eac-120">Följ dessa steg för att åtgärda eventuella formateringsfel i dina avstämnings filer:</span><span class="sxs-lookup"><span data-stu-id="58eac-120">Follow these steps for fix any formatting issues in your reconciliation files:</span></span>

1. <span data-ttu-id="58eac-121">Öppna avstämnings filen (i CSV-format) i Microsoft Excel.</span><span class="sxs-lookup"><span data-stu-id="58eac-121">Open the reconciliation file (in .csv format) in Microsoft Excel.</span></span>
2. <span data-ttu-id="58eac-122">Markera den första kolumnen i filen.</span><span class="sxs-lookup"><span data-stu-id="58eac-122">Select the first column in the file.</span></span>
3. <span data-ttu-id="58eac-123">Öppna **guiden Omvandla text till kolumner**.</span><span class="sxs-lookup"><span data-stu-id="58eac-123">Open the **Convert Text to Columns Wizard**.</span></span> <span data-ttu-id="58eac-124">Välj **data** i menyfliksområdet och välj sedan **text till kolumner**.</span><span class="sxs-lookup"><span data-stu-id="58eac-124">On the ribbon, select **Data**, then select **Text to Columns**.</span></span>
4. <span data-ttu-id="58eac-125">Välj **avgränsad filtyp** i guiden.</span><span class="sxs-lookup"><span data-stu-id="58eac-125">In the wizard, select **Delimited file type**.</span></span> <span data-ttu-id="58eac-126">Välj **Nästa**.</span><span class="sxs-lookup"><span data-stu-id="58eac-126">Then, select **Next**.</span></span>
5. <span data-ttu-id="58eac-127">I fältet **avgränsare** väljer du **kommatecken**.</span><span class="sxs-lookup"><span data-stu-id="58eac-127">In the **Delimiters** field, select **Comma**.</span></span> <span data-ttu-id="58eac-128">(Om **fliken** redan har valts kan du lämna det här alternativet markerat.) Välj sedan **Nästa**.</span><span class="sxs-lookup"><span data-stu-id="58eac-128">(If **Tab** is already selected, you can leave this option selected.) Then, select **Next**.</span></span>
6. <span data-ttu-id="58eac-129">I fältet **kolumn data format** väljer du **datum: MDÅ**.</span><span class="sxs-lookup"><span data-stu-id="58eac-129">In the **Column data format** field, select **Date:MDY**.</span></span> <span data-ttu-id="58eac-130">Välj **Nästa**.</span><span class="sxs-lookup"><span data-stu-id="58eac-130">Then, select **Next**.</span></span>
7. <span data-ttu-id="58eac-131">I fältet **kolumn data format** väljer du **text** för alla belopps kolumner.</span><span class="sxs-lookup"><span data-stu-id="58eac-131">In the **Column data format** field, select **Text** for all amount columns.</span></span> <span data-ttu-id="58eac-132">Välj sedan **Slutför**.</span><span class="sxs-lookup"><span data-stu-id="58eac-132">Then, select **Finish**.</span></span>

## <a name="download-reconciliation-files-programmatically"></a><span data-ttu-id="58eac-133">Ladda ned filer för avstämning program mässigt</span><span class="sxs-lookup"><span data-stu-id="58eac-133">Download reconciliation files programmatically</span></span>

<span data-ttu-id="58eac-134">Avstämnings filer kan vara mycket stora och är ibland svåra att ladda ned.</span><span class="sxs-lookup"><span data-stu-id="58eac-134">Reconciliation files can be very large and are sometimes difficult to download.</span></span> <span data-ttu-id="58eac-135">Information om hur du hämtar avstämnings filer program mässigt finns i [Hämta faktura rads objekt](/partner-center/develop/get-invoiceline-items).</span><span class="sxs-lookup"><span data-stu-id="58eac-135">To download reconciliation files programmatically, see [Get invoice line items](/partner-center/develop/get-invoiceline-items).</span></span>

## <a name="map-taxes-or-vat"></a><span data-ttu-id="58eac-136">Mappa skatter eller moms</span><span class="sxs-lookup"><span data-stu-id="58eac-136">Map taxes or VAT</span></span>

<span data-ttu-id="58eac-137">Så här mappar du skatter eller mervärdes skatt (moms) till din faktura:</span><span class="sxs-lookup"><span data-stu-id="58eac-137">To map Taxes or value-added tax (VAT) to your invoice:</span></span>

- <span data-ttu-id="58eac-138">Summera **moms** kolumnen från den licensbaserade filen.</span><span class="sxs-lookup"><span data-stu-id="58eac-138">Sum the **Tax** column from the license-based file.</span></span>
- <span data-ttu-id="58eac-139">Summera kolumnen **TaxAmount** från den Usage-baserade filen.</span><span class="sxs-lookup"><span data-stu-id="58eac-139">Sum the **TaxAmount** column from the usage-based file.</span></span>

## <a name="itemize-reconciliation-files-by-partner"></a><span data-ttu-id="58eac-140">Specificera avstämnings filer efter partner</span><span class="sxs-lookup"><span data-stu-id="58eac-140">Itemize reconciliation files by partner</span></span>

<span data-ttu-id="58eac-141">Partner i den **indirekta modellen** kan använda dessa ytterligare fält i både licensbaserade och användnings bara avstämnings filer för att specificera filerna efter åter försäljare.</span><span class="sxs-lookup"><span data-stu-id="58eac-141">Partners in the **indirect model** can use these additional fields in both license-based and usage-based reconciliation files to itemize the files by reseller.</span></span>

| <span data-ttu-id="58eac-142">MPN-ID</span><span class="sxs-lookup"><span data-stu-id="58eac-142">MPN ID</span></span> | <span data-ttu-id="58eac-143">Beskrivning</span><span class="sxs-lookup"><span data-stu-id="58eac-143">Description</span></span> |
| ------ | ----------- |
| <span data-ttu-id="58eac-144">MPN-ID</span><span class="sxs-lookup"><span data-stu-id="58eac-144">MPN ID</span></span> | <span data-ttu-id="58eac-145">Microsoft Partner Network-ID (MPN) för Cloud Solution Provider (CSP)-partner (direkt eller indirekt).</span><span class="sxs-lookup"><span data-stu-id="58eac-145">The Microsoft Partner Network (MPN) identifier of the Cloud Solution Provider (CSP) partner (direct or indirect).</span></span> |
| [<span data-ttu-id="58eac-146">MPN-ID för åter försäljare</span><span class="sxs-lookup"><span data-stu-id="58eac-146">Reseller MPN ID</span></span>](#reseller-mpn-id) | <span data-ttu-id="58eac-147">[MPN identifierare för åter försäljaren av posten för prenumerationen](#reseller-mpn-id).</span><span class="sxs-lookup"><span data-stu-id="58eac-147">The [MPN identifier of the reseller of record for the subscription](#reseller-mpn-id).</span></span> <span data-ttu-id="58eac-148">Det här fältet motsvarar det åter försäljar-ID som anges för den aktuella prenumerationen i Partner Center.</span><span class="sxs-lookup"><span data-stu-id="58eac-148">This field corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span> <span data-ttu-id="58eac-149">Visas endast i avstämnings filer för partner i den indirekta modellen.</span><span class="sxs-lookup"><span data-stu-id="58eac-149">Only appears on reconciliation files for partners in the indirect model.</span></span> |

### <a name="reseller-mpn-id"></a><span data-ttu-id="58eac-150">MPN-ID för åter försäljare</span><span class="sxs-lookup"><span data-stu-id="58eac-150">Reseller MPN ID</span></span>

<span data-ttu-id="58eac-151">Om en CSP-partner sålde prenumerationen direkt till kunden visas deras **MPN-ID** två gånger, som både **MPN-ID** och **åter försäljarens MPN-ID**.</span><span class="sxs-lookup"><span data-stu-id="58eac-151">If a CSP partner sold the subscription directly to the customer, their **MPN ID** is listed twice, as both the **MPN ID** and the **Reseller MPN ID**.</span></span>

<span data-ttu-id="58eac-152">Om en CSP-partner har en åter försäljare utan **MPN-ID** är det här värdet inställt på partnerns **MPN-ID** i stället.</span><span class="sxs-lookup"><span data-stu-id="58eac-152">If a CSP partner has a reseller with no **MPN ID**, this value is set to the partner's **MPN ID** instead.</span></span>

<span data-ttu-id="58eac-153">Om CSP-partnern tar bort ett **MPN-ID för åter försäljaren** anges värdet *-1*.</span><span class="sxs-lookup"><span data-stu-id="58eac-153">If the CSP partner removes a **Reseller MPN ID**, this value will be set to *-1*.</span></span>

<span data-ttu-id="58eac-154">Visa eller uppdatera **MPN-ID: t för åter försäljaren**:</span><span class="sxs-lookup"><span data-stu-id="58eac-154">To view or update the **Reseller MPN ID**:</span></span>

1. <span data-ttu-id="58eac-155">Logga in på Partner Center.</span><span class="sxs-lookup"><span data-stu-id="58eac-155">Sign in to Partner Center.</span></span>
2. <span data-ttu-id="58eac-156">I menyn Partner Center väljer du **kunder**.</span><span class="sxs-lookup"><span data-stu-id="58eac-156">In the Partner Center menu, select **Customers**.</span></span>
3. <span data-ttu-id="58eac-157">Välj kund i listan.</span><span class="sxs-lookup"><span data-stu-id="58eac-157">Choose the customer from the list.</span></span>
4. <span data-ttu-id="58eac-158">I menyn kund väljer du **prenumerationer**.</span><span class="sxs-lookup"><span data-stu-id="58eac-158">In the customer menu, select **Subscriptions**.</span></span>
5. <span data-ttu-id="58eac-159">Välj prenumerationen i listan.</span><span class="sxs-lookup"><span data-stu-id="58eac-159">Choose the subscription from the list.</span></span>
6. <span data-ttu-id="58eac-160">Välj **Uppdatera** för att ändra **åter försäljaren (MPN-ID)**.</span><span class="sxs-lookup"><span data-stu-id="58eac-160">Select **update** to change the **Reseller (MPN ID)**.</span></span>

## <a name="next-steps"></a><span data-ttu-id="58eac-161">Nästa steg</span><span class="sxs-lookup"><span data-stu-id="58eac-161">Next steps</span></span>

- [<span data-ttu-id="58eac-162">Så här läser du rekognoseringar-filen för Bill &</span><span class="sxs-lookup"><span data-stu-id="58eac-162">How to read your bill & recon file</span></span>](read-your-bill.md) 