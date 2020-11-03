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
ms.openlocfilehash: 98bfd9a9ce6f03ad62a830f05ba82f9b90268326
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/22/2020
ms.locfileid: "92531581"
---
# <a name="learn-how-to-read-the-line-items-in-your-partner-center-reconciliation-files"></a><span data-ttu-id="524b6-103">Lär dig hur du läser rad objekt i dina avstämnings filer för partner Center</span><span class="sxs-lookup"><span data-stu-id="524b6-103">Learn how to read the line items in your Partner Center reconciliation files</span></span>

<span data-ttu-id="524b6-104">Gäller för:</span><span class="sxs-lookup"><span data-stu-id="524b6-104">Applies to:</span></span>

- <span data-ttu-id="524b6-105">Partnercenter</span><span class="sxs-lookup"><span data-stu-id="524b6-105">Partner Center</span></span>
- <span data-ttu-id="524b6-106">Partner Center för Microsoft Cloud för amerikanska myndigheter</span><span class="sxs-lookup"><span data-stu-id="524b6-106">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="524b6-107">Du kan ladda ned dina avstämnings filer från Partner Center för en detaljerad, rad objekt visning av varje debitering i en fakturerings period.</span><span class="sxs-lookup"><span data-stu-id="524b6-107">You can download your reconciliation files from Partner Center for a detailed, line-item view of each charge in a billing cycle.</span></span> <span data-ttu-id="524b6-108">Information om rad objekt inkluderar avgifter för varje kunds prenumerationer och detaljerade händelser (till exempel ett omslags kort tillägg av licenser till en prenumeration).</span><span class="sxs-lookup"><span data-stu-id="524b6-108">Line-item details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of licenses to a subscription).</span></span>

<span data-ttu-id="524b6-109">Lämpliga roller:</span><span class="sxs-lookup"><span data-stu-id="524b6-109">Appropriate roles:</span></span>

- <span data-ttu-id="524b6-110">Faktureringsadministratör</span><span class="sxs-lookup"><span data-stu-id="524b6-110">Billing admin</span></span>
- <span data-ttu-id="524b6-111">Global administratör</span><span class="sxs-lookup"><span data-stu-id="524b6-111">Global admin</span></span>

<span data-ttu-id="524b6-112">Information om hur du läser fakturan finns i [läsa din](read-your-bill.md) **faktura** .</span><span class="sxs-lookup"><span data-stu-id="524b6-112">For information on how to read your **invoice** , see [Read your bill](read-your-bill.md).</span></span>

## <a name="understand-reconciliation-file-fields"></a><span data-ttu-id="524b6-113">Förstå fält för avstämnings fil</span><span class="sxs-lookup"><span data-stu-id="524b6-113">Understand reconciliation file fields</span></span>

- [<span data-ttu-id="524b6-114">Fil fält för licensbaserade avstämning</span><span class="sxs-lookup"><span data-stu-id="524b6-114">License-based reconciliation file fields</span></span>](license-based-recon-files.md)
- [<span data-ttu-id="524b6-115">Fil fält för användnings-baserad avstämning</span><span class="sxs-lookup"><span data-stu-id="524b6-115">Usage-based reconciliation file fields</span></span>](usage-based-recon-files.md)
- [<span data-ttu-id="524b6-116">Fil fält för dagligt Beräknad användnings avstämning</span><span class="sxs-lookup"><span data-stu-id="524b6-116">Daily-rated usage reconciliation file fields</span></span>](daily-rated-usage-recon-files.md)

## <a name="understand-charge-types-in-reconciliation-files"></a><span data-ttu-id="524b6-117">Förstå debiterings typer i avstämnings filer</span><span class="sxs-lookup"><span data-stu-id="524b6-117">Understand charge types in reconciliation files</span></span>

<span data-ttu-id="524b6-118">Information om vilka typer av kostnader som finns i avstämnings filer (kolumnen **ChargeType** ) finns i [fil avgifts typer för avstämning](recon-file-charge-types.md).</span><span class="sxs-lookup"><span data-stu-id="524b6-118">To understand the types of charges in reconciliation files (the **ChargeType** column), see [Reconciliation file charge types](recon-file-charge-types.md).</span></span>

## <a name="fix-formatting-issues"></a><span data-ttu-id="524b6-119">Åtgärda problem med formatering</span><span class="sxs-lookup"><span data-stu-id="524b6-119">Fix formatting issues</span></span>

<span data-ttu-id="524b6-120">Ibland kan en avstämnings fil innehålla formateringsfel.</span><span class="sxs-lookup"><span data-stu-id="524b6-120">Occasionally, a reconciliation file might contain formatting issues.</span></span> <span data-ttu-id="524b6-121">Det här problemet kan till exempel inträffa om en-US locale inte används.</span><span class="sxs-lookup"><span data-stu-id="524b6-121">For example, this issue might occur if the en-US locale is not used.</span></span>

<span data-ttu-id="524b6-122">Följ dessa steg för att åtgärda eventuella formateringsfel i dina avstämnings filer:</span><span class="sxs-lookup"><span data-stu-id="524b6-122">Follow these steps for fix any formatting issues in your reconciliation files:</span></span>

1. <span data-ttu-id="524b6-123">Öppna avstämnings filen (i CSV-format) i Microsoft Excel.</span><span class="sxs-lookup"><span data-stu-id="524b6-123">Open the reconciliation file (in .csv format) in Microsoft Excel.</span></span>
2. <span data-ttu-id="524b6-124">Markera den första kolumnen i filen.</span><span class="sxs-lookup"><span data-stu-id="524b6-124">Select the first column in the file.</span></span>
3. <span data-ttu-id="524b6-125">Öppna **guiden Omvandla text till kolumner** .</span><span class="sxs-lookup"><span data-stu-id="524b6-125">Open the **Convert Text to Columns Wizard** .</span></span> <span data-ttu-id="524b6-126">Välj **data** i menyfliksområdet och välj sedan **text till kolumner** .</span><span class="sxs-lookup"><span data-stu-id="524b6-126">On the ribbon, select **Data** , then select **Text to Columns** .</span></span>
4. <span data-ttu-id="524b6-127">Välj **avgränsad filtyp** i guiden.</span><span class="sxs-lookup"><span data-stu-id="524b6-127">In the wizard, select **Delimited file type** .</span></span> <span data-ttu-id="524b6-128">Välj **Nästa** .</span><span class="sxs-lookup"><span data-stu-id="524b6-128">Then, select **Next** .</span></span>
5. <span data-ttu-id="524b6-129">I fältet **avgränsare** väljer du **kommatecken** .</span><span class="sxs-lookup"><span data-stu-id="524b6-129">In the **Delimiters** field, select **Comma** .</span></span> <span data-ttu-id="524b6-130">(Om **fliken** redan har valts kan du lämna det här alternativet markerat.) Välj sedan **Nästa** .</span><span class="sxs-lookup"><span data-stu-id="524b6-130">(If **Tab** is already selected, you can leave this option selected.) Then, select **Next** .</span></span>
6. <span data-ttu-id="524b6-131">I fältet **kolumn data format** väljer du **datum: MDÅ** .</span><span class="sxs-lookup"><span data-stu-id="524b6-131">In the **Column data format** field, select **Date:MDY** .</span></span> <span data-ttu-id="524b6-132">Välj **Nästa** .</span><span class="sxs-lookup"><span data-stu-id="524b6-132">Then, select **Next** .</span></span>
7. <span data-ttu-id="524b6-133">I fältet **kolumn data format** väljer du **text** för alla belopps kolumner.</span><span class="sxs-lookup"><span data-stu-id="524b6-133">In the **Column data format** field, select **Text** for all amount columns.</span></span> <span data-ttu-id="524b6-134">Välj sedan **Slutför** .</span><span class="sxs-lookup"><span data-stu-id="524b6-134">Then, select **Finish** .</span></span>

## <a name="download-reconciliation-files-programmatically"></a><span data-ttu-id="524b6-135">Ladda ned filer för avstämning program mässigt</span><span class="sxs-lookup"><span data-stu-id="524b6-135">Download reconciliation files programmatically</span></span>

<span data-ttu-id="524b6-136">Avstämnings filer kan vara mycket stora och är ibland svåra att ladda ned.</span><span class="sxs-lookup"><span data-stu-id="524b6-136">Reconciliation files can be very large and are sometimes difficult to download.</span></span> <span data-ttu-id="524b6-137">Information om hur du hämtar avstämnings filer program mässigt finns i [Hämta faktura rads objekt](/partner-center/develop/get-invoiceline-items).</span><span class="sxs-lookup"><span data-stu-id="524b6-137">To download reconciliation files programmatically, see [Get invoice line items](/partner-center/develop/get-invoiceline-items).</span></span>

## <a name="map-taxes-or-vat"></a><span data-ttu-id="524b6-138">Mappa skatter eller moms</span><span class="sxs-lookup"><span data-stu-id="524b6-138">Map taxes or VAT</span></span>

<span data-ttu-id="524b6-139">Så här mappar du skatter eller mervärdes skatt (moms) till din faktura:</span><span class="sxs-lookup"><span data-stu-id="524b6-139">To map Taxes or value-added tax (VAT) to your invoice:</span></span>

- <span data-ttu-id="524b6-140">Summera **moms** kolumnen från den licensbaserade filen.</span><span class="sxs-lookup"><span data-stu-id="524b6-140">Sum the **Tax** column from the license-based file.</span></span>
- <span data-ttu-id="524b6-141">Summera kolumnen **TaxAmount** från den Usage-baserade filen.</span><span class="sxs-lookup"><span data-stu-id="524b6-141">Sum the **TaxAmount** column from the usage-based file.</span></span>

## <a name="itemize-reconciliation-files-by-partner"></a><span data-ttu-id="524b6-142">Specificera avstämnings filer efter partner</span><span class="sxs-lookup"><span data-stu-id="524b6-142">Itemize reconciliation files by partner</span></span>

<span data-ttu-id="524b6-143">Partner i den **indirekta modellen** kan använda dessa ytterligare fält i både licensbaserade och användnings bara avstämnings filer för att specificera filerna efter åter försäljare.</span><span class="sxs-lookup"><span data-stu-id="524b6-143">Partners in the **indirect model** can use these additional fields in both license-based and usage-based reconciliation files to itemize the files by reseller.</span></span>

| <span data-ttu-id="524b6-144">MPN-ID</span><span class="sxs-lookup"><span data-stu-id="524b6-144">MPN ID</span></span> | <span data-ttu-id="524b6-145">Beskrivning</span><span class="sxs-lookup"><span data-stu-id="524b6-145">Description</span></span> |
| ------ | ----------- |
| <span data-ttu-id="524b6-146">MPN-ID</span><span class="sxs-lookup"><span data-stu-id="524b6-146">MPN ID</span></span> | <span data-ttu-id="524b6-147">Microsoft Partner Network-ID (MPN) för Cloud Solution Provider (CSP)-partner (direkt eller indirekt).</span><span class="sxs-lookup"><span data-stu-id="524b6-147">The Microsoft Partner Network (MPN) identifier of the Cloud Solution Provider (CSP) partner (direct or indirect).</span></span> |
| [<span data-ttu-id="524b6-148">MPN-ID för åter försäljare</span><span class="sxs-lookup"><span data-stu-id="524b6-148">Reseller MPN ID</span></span>](#reseller-mpn-id) | <span data-ttu-id="524b6-149">[MPN identifierare för åter försäljaren av posten för prenumerationen](#reseller-mpn-id).</span><span class="sxs-lookup"><span data-stu-id="524b6-149">The [MPN identifier of the reseller of record for the subscription](#reseller-mpn-id).</span></span> <span data-ttu-id="524b6-150">Det här fältet motsvarar det åter försäljar-ID som anges för den aktuella prenumerationen i Partner Center.</span><span class="sxs-lookup"><span data-stu-id="524b6-150">This field corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span> <span data-ttu-id="524b6-151">Visas endast i avstämnings filer för partner i den indirekta modellen.</span><span class="sxs-lookup"><span data-stu-id="524b6-151">Only appears on reconciliation files for partners in the indirect model.</span></span> |

### <a name="reseller-mpn-id"></a><span data-ttu-id="524b6-152">MPN-ID för åter försäljare</span><span class="sxs-lookup"><span data-stu-id="524b6-152">Reseller MPN ID</span></span>

<span data-ttu-id="524b6-153">Om en CSP-partner sålde prenumerationen direkt till kunden visas deras **MPN-ID** två gånger, som både **MPN-ID** och **åter försäljarens MPN-ID** .</span><span class="sxs-lookup"><span data-stu-id="524b6-153">If a CSP partner sold the subscription directly to the customer, their **MPN ID** is listed twice, as both the **MPN ID** and the **Reseller MPN ID** .</span></span>

<span data-ttu-id="524b6-154">Om en CSP-partner har en åter försäljare utan **MPN-ID** är det här värdet inställt på partnerns **MPN-ID** i stället.</span><span class="sxs-lookup"><span data-stu-id="524b6-154">If a CSP partner has a reseller with no **MPN ID** , this value is set to the partner's **MPN ID** instead.</span></span>

<span data-ttu-id="524b6-155">Om CSP-partnern tar bort ett **MPN-ID för åter försäljaren** anges värdet *-1* .</span><span class="sxs-lookup"><span data-stu-id="524b6-155">If the CSP partner removes a **Reseller MPN ID** , this value will be set to *-1* .</span></span>

<span data-ttu-id="524b6-156">Visa eller uppdatera **MPN-ID: t för åter försäljaren** :</span><span class="sxs-lookup"><span data-stu-id="524b6-156">To view or update the **Reseller MPN ID** :</span></span>

1. <span data-ttu-id="524b6-157">Logga in på Partner Center.</span><span class="sxs-lookup"><span data-stu-id="524b6-157">Sign in to Partner Center.</span></span>
2. <span data-ttu-id="524b6-158">I menyn Partner Center väljer du **kunder** .</span><span class="sxs-lookup"><span data-stu-id="524b6-158">In the Partner Center menu, select **Customers** .</span></span>
3. <span data-ttu-id="524b6-159">Välj kund i listan.</span><span class="sxs-lookup"><span data-stu-id="524b6-159">Choose the customer from the list.</span></span>
4. <span data-ttu-id="524b6-160">I menyn kund väljer du **prenumerationer** .</span><span class="sxs-lookup"><span data-stu-id="524b6-160">In the customer menu, select **Subscriptions** .</span></span>
5. <span data-ttu-id="524b6-161">Välj prenumerationen i listan.</span><span class="sxs-lookup"><span data-stu-id="524b6-161">Choose the subscription from the list.</span></span>
6. <span data-ttu-id="524b6-162">Välj **Uppdatera** för att ändra **åter försäljaren (MPN-ID)** .</span><span class="sxs-lookup"><span data-stu-id="524b6-162">Select **update** to change the **Reseller (MPN ID)** .</span></span>