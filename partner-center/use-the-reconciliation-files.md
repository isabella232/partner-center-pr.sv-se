---
title: Använd dina avstämnings filer
ms.topic: article
ms.date: 06/08/2020
description: Lär dig mer om avstämnings filer i Partner Center och hur du tolkar de detaljerade vyerna för rad artikel med debiteringar för en fakturerings period.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: d09c1e57d16937c5656579f3932e9c8feb3ecf24
ms.sourcegitcommit: 95a5afdf68d88b6be848729830dcd114e3fb0c0f
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 11/11/2020
ms.locfileid: "94488099"
---
# <a name="learn-how-to-read-the-line-items-in-your-partner-center-reconciliation-files"></a><span data-ttu-id="9cab6-103">Lär dig hur du läser rad objekt i dina avstämnings filer för partner Center</span><span class="sxs-lookup"><span data-stu-id="9cab6-103">Learn how to read the line items in your Partner Center reconciliation files</span></span>

<span data-ttu-id="9cab6-104">Gäller för:</span><span class="sxs-lookup"><span data-stu-id="9cab6-104">Applies to:</span></span>

- <span data-ttu-id="9cab6-105">Partnercenter</span><span class="sxs-lookup"><span data-stu-id="9cab6-105">Partner Center</span></span>
- <span data-ttu-id="9cab6-106">Välkommen till Partnercenter för Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="9cab6-106">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="9cab6-107">Du kan ladda ned dina avstämnings filer från Partner Center för en detaljerad, rad objekt visning av varje debitering i en fakturerings period.</span><span class="sxs-lookup"><span data-stu-id="9cab6-107">You can download your reconciliation files from Partner Center for a detailed, line-item view of each charge in a billing cycle.</span></span> <span data-ttu-id="9cab6-108">Information om rad objekt inkluderar avgifter för varje kunds prenumerationer och detaljerade händelser (till exempel ett omslags kort tillägg av licenser till en prenumeration).</span><span class="sxs-lookup"><span data-stu-id="9cab6-108">Line-item details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of licenses to a subscription).</span></span>

<span data-ttu-id="9cab6-109">Lämpliga roller:</span><span class="sxs-lookup"><span data-stu-id="9cab6-109">Appropriate roles:</span></span>

- <span data-ttu-id="9cab6-110">Faktureringsadministratör</span><span class="sxs-lookup"><span data-stu-id="9cab6-110">Billing admin</span></span>
- <span data-ttu-id="9cab6-111">Global administratör</span><span class="sxs-lookup"><span data-stu-id="9cab6-111">Global admin</span></span>

<span data-ttu-id="9cab6-112">Information om hur du läser fakturan finns i [läsa din](read-your-bill.md) **faktura**.</span><span class="sxs-lookup"><span data-stu-id="9cab6-112">For information on how to read your **invoice** , see [Read your bill](read-your-bill.md).</span></span>

## <a name="understand-reconciliation-file-fields"></a><span data-ttu-id="9cab6-113">Förstå fält för avstämnings fil</span><span class="sxs-lookup"><span data-stu-id="9cab6-113">Understand reconciliation file fields</span></span>

- [<span data-ttu-id="9cab6-114">Fil fält för licensbaserade avstämning</span><span class="sxs-lookup"><span data-stu-id="9cab6-114">License-based reconciliation file fields</span></span>](license-based-recon-files.md)
- [<span data-ttu-id="9cab6-115">Fil fält för användnings-baserad avstämning</span><span class="sxs-lookup"><span data-stu-id="9cab6-115">Usage-based reconciliation file fields</span></span>](usage-based-recon-files.md)
- [<span data-ttu-id="9cab6-116">Fil fält för dagligt Beräknad användnings avstämning</span><span class="sxs-lookup"><span data-stu-id="9cab6-116">Daily-rated usage reconciliation file fields</span></span>](daily-rated-usage-recon-files.md)
- [<span data-ttu-id="9cab6-117">Fil fält för CSP-avstämning för inköp vid ett tillfälle</span><span class="sxs-lookup"><span data-stu-id="9cab6-117">One-time purchase CSP reconciliation file fields</span></span>](modern-invoice-reconciliation-file.md)

## <a name="understand-charge-types-in-reconciliation-files"></a><span data-ttu-id="9cab6-118">Förstå debiterings typer i avstämnings filer</span><span class="sxs-lookup"><span data-stu-id="9cab6-118">Understand charge types in reconciliation files</span></span>

<span data-ttu-id="9cab6-119">Information om vilka typer av kostnader som finns i avstämnings filer (kolumnen **ChargeType** ) finns i [fil avgifts typer för avstämning](recon-file-charge-types.md).</span><span class="sxs-lookup"><span data-stu-id="9cab6-119">To understand the types of charges in reconciliation files (the **ChargeType** column), see [Reconciliation file charge types](recon-file-charge-types.md).</span></span>

## <a name="fix-formatting-issues"></a><span data-ttu-id="9cab6-120">Åtgärda problem med formatering</span><span class="sxs-lookup"><span data-stu-id="9cab6-120">Fix formatting issues</span></span>

<span data-ttu-id="9cab6-121">Ibland kan en avstämnings fil innehålla formateringsfel.</span><span class="sxs-lookup"><span data-stu-id="9cab6-121">Occasionally, a reconciliation file might contain formatting issues.</span></span> <span data-ttu-id="9cab6-122">Det här problemet kan till exempel inträffa om en-US locale inte används.</span><span class="sxs-lookup"><span data-stu-id="9cab6-122">For example, this issue might occur if the en-US locale is not used.</span></span>

<span data-ttu-id="9cab6-123">Följ dessa steg för att åtgärda eventuella formateringsfel i dina avstämnings filer:</span><span class="sxs-lookup"><span data-stu-id="9cab6-123">Follow these steps for fix any formatting issues in your reconciliation files:</span></span>

1. <span data-ttu-id="9cab6-124">Öppna avstämnings filen (i CSV-format) i Microsoft Excel.</span><span class="sxs-lookup"><span data-stu-id="9cab6-124">Open the reconciliation file (in .csv format) in Microsoft Excel.</span></span>
2. <span data-ttu-id="9cab6-125">Markera den första kolumnen i filen.</span><span class="sxs-lookup"><span data-stu-id="9cab6-125">Select the first column in the file.</span></span>
3. <span data-ttu-id="9cab6-126">Öppna **guiden Omvandla text till kolumner**.</span><span class="sxs-lookup"><span data-stu-id="9cab6-126">Open the **Convert Text to Columns Wizard**.</span></span> <span data-ttu-id="9cab6-127">Välj **data** i menyfliksområdet och välj sedan **text till kolumner**.</span><span class="sxs-lookup"><span data-stu-id="9cab6-127">On the ribbon, select **Data** , then select **Text to Columns**.</span></span>
4. <span data-ttu-id="9cab6-128">Välj **avgränsad filtyp** i guiden.</span><span class="sxs-lookup"><span data-stu-id="9cab6-128">In the wizard, select **Delimited file type**.</span></span> <span data-ttu-id="9cab6-129">Välj **Nästa**.</span><span class="sxs-lookup"><span data-stu-id="9cab6-129">Then, select **Next**.</span></span>
5. <span data-ttu-id="9cab6-130">I fältet **avgränsare** väljer du **kommatecken**.</span><span class="sxs-lookup"><span data-stu-id="9cab6-130">In the **Delimiters** field, select **Comma**.</span></span> <span data-ttu-id="9cab6-131">(Om **fliken** redan har valts kan du lämna det här alternativet markerat.) Välj sedan **Nästa**.</span><span class="sxs-lookup"><span data-stu-id="9cab6-131">(If **Tab** is already selected, you can leave this option selected.) Then, select **Next**.</span></span>
6. <span data-ttu-id="9cab6-132">I fältet **kolumn data format** väljer du **datum: MDÅ**.</span><span class="sxs-lookup"><span data-stu-id="9cab6-132">In the **Column data format** field, select **Date:MDY**.</span></span> <span data-ttu-id="9cab6-133">Välj **Nästa**.</span><span class="sxs-lookup"><span data-stu-id="9cab6-133">Then, select **Next**.</span></span>
7. <span data-ttu-id="9cab6-134">I fältet **kolumn data format** väljer du **text** för alla belopps kolumner.</span><span class="sxs-lookup"><span data-stu-id="9cab6-134">In the **Column data format** field, select **Text** for all amount columns.</span></span> <span data-ttu-id="9cab6-135">Välj sedan **Slutför**.</span><span class="sxs-lookup"><span data-stu-id="9cab6-135">Then, select **Finish**.</span></span>

## <a name="download-reconciliation-files-programmatically"></a><span data-ttu-id="9cab6-136">Ladda ned filer för avstämning program mässigt</span><span class="sxs-lookup"><span data-stu-id="9cab6-136">Download reconciliation files programmatically</span></span>

<span data-ttu-id="9cab6-137">Avstämnings filer kan vara mycket stora och är ibland svåra att ladda ned.</span><span class="sxs-lookup"><span data-stu-id="9cab6-137">Reconciliation files can be very large and are sometimes difficult to download.</span></span> <span data-ttu-id="9cab6-138">Information om hur du hämtar avstämnings filer program mässigt finns i [Hämta faktura rads objekt](/partner-center/develop/get-invoiceline-items).</span><span class="sxs-lookup"><span data-stu-id="9cab6-138">To download reconciliation files programmatically, see [Get invoice line items](/partner-center/develop/get-invoiceline-items).</span></span>

## <a name="map-taxes-or-vat"></a><span data-ttu-id="9cab6-139">Mappa skatter eller moms</span><span class="sxs-lookup"><span data-stu-id="9cab6-139">Map taxes or VAT</span></span>

<span data-ttu-id="9cab6-140">Så här mappar du skatter eller mervärdes skatt (moms) till din faktura:</span><span class="sxs-lookup"><span data-stu-id="9cab6-140">To map Taxes or value-added tax (VAT) to your invoice:</span></span>

- <span data-ttu-id="9cab6-141">Summera **moms** kolumnen från den licensbaserade filen.</span><span class="sxs-lookup"><span data-stu-id="9cab6-141">Sum the **Tax** column from the license-based file.</span></span>
- <span data-ttu-id="9cab6-142">Summera kolumnen **TaxAmount** från den Usage-baserade filen.</span><span class="sxs-lookup"><span data-stu-id="9cab6-142">Sum the **TaxAmount** column from the usage-based file.</span></span>

## <a name="itemize-reconciliation-files-by-partner"></a><span data-ttu-id="9cab6-143">Specificera avstämnings filer efter partner</span><span class="sxs-lookup"><span data-stu-id="9cab6-143">Itemize reconciliation files by partner</span></span>

<span data-ttu-id="9cab6-144">Partner i den **indirekta modellen** kan använda dessa ytterligare fält i både licensbaserade och användnings bara avstämnings filer för att specificera filerna efter åter försäljare.</span><span class="sxs-lookup"><span data-stu-id="9cab6-144">Partners in the **indirect model** can use these additional fields in both license-based and usage-based reconciliation files to itemize the files by reseller.</span></span>

| <span data-ttu-id="9cab6-145">MPN-ID</span><span class="sxs-lookup"><span data-stu-id="9cab6-145">MPN ID</span></span> | <span data-ttu-id="9cab6-146">Beskrivning</span><span class="sxs-lookup"><span data-stu-id="9cab6-146">Description</span></span> |
| ------ | ----------- |
| <span data-ttu-id="9cab6-147">MPN-ID</span><span class="sxs-lookup"><span data-stu-id="9cab6-147">MPN ID</span></span> | <span data-ttu-id="9cab6-148">Microsoft Partner Network-ID (MPN) för Cloud Solution Provider (CSP)-partner (direkt eller indirekt).</span><span class="sxs-lookup"><span data-stu-id="9cab6-148">The Microsoft Partner Network (MPN) identifier of the Cloud Solution Provider (CSP) partner (direct or indirect).</span></span> |
| [<span data-ttu-id="9cab6-149">MPN-ID för åter försäljare</span><span class="sxs-lookup"><span data-stu-id="9cab6-149">Reseller MPN ID</span></span>](#reseller-mpn-id) | <span data-ttu-id="9cab6-150">[MPN identifierare för åter försäljaren av posten för prenumerationen](#reseller-mpn-id).</span><span class="sxs-lookup"><span data-stu-id="9cab6-150">The [MPN identifier of the reseller of record for the subscription](#reseller-mpn-id).</span></span> <span data-ttu-id="9cab6-151">Det här fältet motsvarar det åter försäljar-ID som anges för den aktuella prenumerationen i Partner Center.</span><span class="sxs-lookup"><span data-stu-id="9cab6-151">This field corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span> <span data-ttu-id="9cab6-152">Visas endast i avstämnings filer för partner i den indirekta modellen.</span><span class="sxs-lookup"><span data-stu-id="9cab6-152">Only appears on reconciliation files for partners in the indirect model.</span></span> |

### <a name="reseller-mpn-id"></a><span data-ttu-id="9cab6-153">MPN-ID för åter försäljare</span><span class="sxs-lookup"><span data-stu-id="9cab6-153">Reseller MPN ID</span></span>

<span data-ttu-id="9cab6-154">Om en CSP-partner sålde prenumerationen direkt till kunden visas deras **MPN-ID** två gånger, som både **MPN-ID** och **åter försäljarens MPN-ID**.</span><span class="sxs-lookup"><span data-stu-id="9cab6-154">If a CSP partner sold the subscription directly to the customer, their **MPN ID** is listed twice, as both the **MPN ID** and the **Reseller MPN ID**.</span></span>

<span data-ttu-id="9cab6-155">Om en CSP-partner har en åter försäljare utan **MPN-ID** är det här värdet inställt på partnerns **MPN-ID** i stället.</span><span class="sxs-lookup"><span data-stu-id="9cab6-155">If a CSP partner has a reseller with no **MPN ID** , this value is set to the partner's **MPN ID** instead.</span></span>

<span data-ttu-id="9cab6-156">Om CSP-partnern tar bort ett **MPN-ID för åter försäljaren** anges värdet *-1*.</span><span class="sxs-lookup"><span data-stu-id="9cab6-156">If the CSP partner removes a **Reseller MPN ID** , this value will be set to *-1*.</span></span>

<span data-ttu-id="9cab6-157">Visa eller uppdatera **MPN-ID: t för åter försäljaren** :</span><span class="sxs-lookup"><span data-stu-id="9cab6-157">To view or update the **Reseller MPN ID** :</span></span>

1. <span data-ttu-id="9cab6-158">Logga in på Partner Center.</span><span class="sxs-lookup"><span data-stu-id="9cab6-158">Sign in to Partner Center.</span></span>
2. <span data-ttu-id="9cab6-159">I menyn Partner Center väljer du **kunder**.</span><span class="sxs-lookup"><span data-stu-id="9cab6-159">In the Partner Center menu, select **Customers**.</span></span>
3. <span data-ttu-id="9cab6-160">Välj kund i listan.</span><span class="sxs-lookup"><span data-stu-id="9cab6-160">Choose the customer from the list.</span></span>
4. <span data-ttu-id="9cab6-161">I menyn kund väljer du **prenumerationer**.</span><span class="sxs-lookup"><span data-stu-id="9cab6-161">In the customer menu, select **Subscriptions**.</span></span>
5. <span data-ttu-id="9cab6-162">Välj prenumerationen i listan.</span><span class="sxs-lookup"><span data-stu-id="9cab6-162">Choose the subscription from the list.</span></span>
6. <span data-ttu-id="9cab6-163">Välj **Uppdatera** för att ändra **åter försäljaren (MPN-ID)**.</span><span class="sxs-lookup"><span data-stu-id="9cab6-163">Select **update** to change the **Reseller (MPN ID)**.</span></span>