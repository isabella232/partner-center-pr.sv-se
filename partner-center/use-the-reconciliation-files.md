---
title: Använd dina avstämnings filer
ms.topic: article
ms.date: 03/26/2021
description: Lär dig mer om avstämnings filer i Partner Center och hur du tolkar de detaljerade vyerna för rad artikel med debiteringar för en fakturerings period.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 4a6a1455304f12e364d71e666cbd548821f8be55
ms.sourcegitcommit: a691d4cbe144a8fd71e344fd293cc658ac11d6f3
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/27/2021
ms.locfileid: "105633904"
---
# <a name="learn-how-to-read-the-line-items-in-your-partner-center-reconciliation-files"></a><span data-ttu-id="6593d-103">Lär dig hur du läser rad objekt i dina avstämnings filer för partner Center</span><span class="sxs-lookup"><span data-stu-id="6593d-103">Learn how to read the line items in your Partner Center reconciliation files</span></span>

<span data-ttu-id="6593d-104">**Lämpliga roller**</span><span class="sxs-lookup"><span data-stu-id="6593d-104">**Appropriate roles**</span></span>

- <span data-ttu-id="6593d-105">Faktureringsadministratör</span><span class="sxs-lookup"><span data-stu-id="6593d-105">Billing admin</span></span>
- <span data-ttu-id="6593d-106">Global administratör</span><span class="sxs-lookup"><span data-stu-id="6593d-106">Global admin</span></span>

<span data-ttu-id="6593d-107">Du kan ladda ned dina avstämnings filer från Partner Center för en detaljerad, rad objekt visning av varje debitering i en fakturerings period.</span><span class="sxs-lookup"><span data-stu-id="6593d-107">You can download your reconciliation files from Partner Center for a detailed, line-item view of each charge in a billing cycle.</span></span> <span data-ttu-id="6593d-108">Information om rad objekt inkluderar avgifter för varje kunds prenumerationer och detaljerade händelser (till exempel ett omslags kort tillägg av licenser till en prenumeration).</span><span class="sxs-lookup"><span data-stu-id="6593d-108">Line-item details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of licenses to a subscription).</span></span>

<span data-ttu-id="6593d-109">Information om hur du läser fakturan finns i [läsa din](read-your-bill.md) **faktura**.</span><span class="sxs-lookup"><span data-stu-id="6593d-109">For information on how to read your **invoice**, see [Read your bill](read-your-bill.md).</span></span>

## <a name="understand-reconciliation-file-fields"></a><span data-ttu-id="6593d-110">Förstå fält för avstämnings fil</span><span class="sxs-lookup"><span data-stu-id="6593d-110">Understand reconciliation file fields</span></span>

- [<span data-ttu-id="6593d-111">Fält för licensbaserad avstämningsfil</span><span class="sxs-lookup"><span data-stu-id="6593d-111">License-based reconciliation file fields</span></span>](license-based-recon-files.md)
- [<span data-ttu-id="6593d-112">Fält för användningsbaserad avstämningsfil</span><span class="sxs-lookup"><span data-stu-id="6593d-112">Usage-based reconciliation file fields</span></span>](usage-based-recon-files.md)
- [<span data-ttu-id="6593d-113">Fält i fil för dagligt beräknad användningsavstämning</span><span class="sxs-lookup"><span data-stu-id="6593d-113">Daily-rated usage reconciliation file fields</span></span>](daily-rated-usage-recon-files.md)
- [<span data-ttu-id="6593d-114">Fil fält för CSP-avstämning för inköp vid ett tillfälle</span><span class="sxs-lookup"><span data-stu-id="6593d-114">One-time purchase CSP reconciliation file fields</span></span>](modern-invoice-reconciliation-file.md)

## <a name="understand-charge-types-in-reconciliation-files"></a><span data-ttu-id="6593d-115">Förstå debiterings typer i avstämnings filer</span><span class="sxs-lookup"><span data-stu-id="6593d-115">Understand charge types in reconciliation files</span></span>

<span data-ttu-id="6593d-116">Information om vilka typer av kostnader som finns i avstämnings filer (kolumnen **ChargeType** ) finns i [fil avgifts typer för avstämning](recon-file-charge-types.md).</span><span class="sxs-lookup"><span data-stu-id="6593d-116">To understand the types of charges in reconciliation files (the **ChargeType** column), see [Reconciliation file charge types](recon-file-charge-types.md).</span></span>

## <a name="fix-formatting-issues"></a><span data-ttu-id="6593d-117">Åtgärda problem med formatering</span><span class="sxs-lookup"><span data-stu-id="6593d-117">Fix formatting issues</span></span>

<span data-ttu-id="6593d-118">Ibland kan en avstämnings fil innehålla formateringsfel.</span><span class="sxs-lookup"><span data-stu-id="6593d-118">Occasionally, a reconciliation file might contain formatting issues.</span></span> <span data-ttu-id="6593d-119">Det här problemet kan till exempel inträffa om en-US locale inte används.</span><span class="sxs-lookup"><span data-stu-id="6593d-119">For example, this issue might occur if the en-US locale is not used.</span></span>

<span data-ttu-id="6593d-120">Följ dessa steg för att åtgärda eventuella formateringsfel i dina avstämnings filer:</span><span class="sxs-lookup"><span data-stu-id="6593d-120">Follow these steps for fix any formatting issues in your reconciliation files:</span></span>

1. <span data-ttu-id="6593d-121">Öppna avstämnings filen (i CSV-format) i Microsoft Excel.</span><span class="sxs-lookup"><span data-stu-id="6593d-121">Open the reconciliation file (in .csv format) in Microsoft Excel.</span></span>
2. <span data-ttu-id="6593d-122">Markera den första kolumnen i filen.</span><span class="sxs-lookup"><span data-stu-id="6593d-122">Select the first column in the file.</span></span>
3. <span data-ttu-id="6593d-123">Öppna **guiden Omvandla text till kolumner**.</span><span class="sxs-lookup"><span data-stu-id="6593d-123">Open the **Convert Text to Columns Wizard**.</span></span> <span data-ttu-id="6593d-124">Välj **data** i menyfliksområdet och välj sedan **text till kolumner**.</span><span class="sxs-lookup"><span data-stu-id="6593d-124">On the ribbon, select **Data**, then select **Text to Columns**.</span></span>
4. <span data-ttu-id="6593d-125">Välj **avgränsad filtyp** i guiden.</span><span class="sxs-lookup"><span data-stu-id="6593d-125">In the wizard, select **Delimited file type**.</span></span> <span data-ttu-id="6593d-126">Välj **Nästa**.</span><span class="sxs-lookup"><span data-stu-id="6593d-126">Then, select **Next**.</span></span>
5. <span data-ttu-id="6593d-127">I fältet **avgränsare** väljer du **kommatecken**.</span><span class="sxs-lookup"><span data-stu-id="6593d-127">In the **Delimiters** field, select **Comma**.</span></span> <span data-ttu-id="6593d-128">(Om **fliken** redan har valts kan du lämna det här alternativet markerat.) Välj sedan **Nästa**.</span><span class="sxs-lookup"><span data-stu-id="6593d-128">(If **Tab** is already selected, you can leave this option selected.) Then, select **Next**.</span></span>
6. <span data-ttu-id="6593d-129">I fältet **kolumn data format** väljer du **datum: MDÅ**.</span><span class="sxs-lookup"><span data-stu-id="6593d-129">In the **Column data format** field, select **Date:MDY**.</span></span> <span data-ttu-id="6593d-130">Välj **Nästa**.</span><span class="sxs-lookup"><span data-stu-id="6593d-130">Then, select **Next**.</span></span>
7. <span data-ttu-id="6593d-131">I fältet **kolumn data format** väljer du **text** för alla belopps kolumner.</span><span class="sxs-lookup"><span data-stu-id="6593d-131">In the **Column data format** field, select **Text** for all amount columns.</span></span> <span data-ttu-id="6593d-132">Välj sedan **Slutför**.</span><span class="sxs-lookup"><span data-stu-id="6593d-132">Then, select **Finish**.</span></span>

## <a name="download-reconciliation-files-programmatically"></a><span data-ttu-id="6593d-133">Ladda ned filer för avstämning program mässigt</span><span class="sxs-lookup"><span data-stu-id="6593d-133">Download reconciliation files programmatically</span></span>

<span data-ttu-id="6593d-134">Avstämnings filer kan vara mycket stora och är ibland svåra att ladda ned.</span><span class="sxs-lookup"><span data-stu-id="6593d-134">Reconciliation files can be very large and are sometimes difficult to download.</span></span> <span data-ttu-id="6593d-135">Information om hur du hämtar avstämnings filer program mässigt finns i [Hämta faktura rads objekt](/partner-center/develop/get-invoiceline-items).</span><span class="sxs-lookup"><span data-stu-id="6593d-135">To download reconciliation files programmatically, see [Get invoice line items](/partner-center/develop/get-invoiceline-items).</span></span>

## <a name="if-your-file-exceeds-the-row-limit-in-excel"></a><span data-ttu-id="6593d-136">Om filen överskrider rad gränsen i Excel</span><span class="sxs-lookup"><span data-stu-id="6593d-136">If your file exceeds the row limit in Excel</span></span>

<span data-ttu-id="6593d-137">Om du kan ladda ned en avstämnings fil men inte öppna den i Microsoft Excel, betyder det förmodligen att filen innehåller fler rader än vad Excel tillåter.</span><span class="sxs-lookup"><span data-stu-id="6593d-137">If you’re able to download a reconciliation file but not open it in Microsoft Excel, it probably means the file contains more rows than Excel will allow.</span></span> <span data-ttu-id="6593d-138">I så fall kan du använda någon av stegen nedan för att öppna filen.</span><span class="sxs-lookup"><span data-stu-id="6593d-138">If this happens, you can use either of the procedures below to open the file.</span></span>

### <a name="open-a-recon-file-in-power-bi"></a><span data-ttu-id="6593d-139">Öppna en rekognoseringar-fil i Power BI</span><span class="sxs-lookup"><span data-stu-id="6593d-139">Open a recon file in Power BI</span></span>

1. <span data-ttu-id="6593d-140">Ladda ned avstämnings filen precis som vanligt.</span><span class="sxs-lookup"><span data-stu-id="6593d-140">Download the reconciliation file as you normally would.</span></span>
2. <span data-ttu-id="6593d-141">Ladda ned, installera och öppna en instans av Power BI.</span><span class="sxs-lookup"><span data-stu-id="6593d-141">Download, install, and open an instance of Power BI.</span></span>
3. <span data-ttu-id="6593d-142">På fliken Power BI **Start** väljer du **Hämta data**.</span><span class="sxs-lookup"><span data-stu-id="6593d-142">On the Power BI **Home** tab, select **Get data**.</span></span>
4. <span data-ttu-id="6593d-143">I listan med **vanliga data källor** väljer du **text/CSV**.</span><span class="sxs-lookup"><span data-stu-id="6593d-143">In the list of **Common data sources**, select **Text/CSV**.</span></span>
5. <span data-ttu-id="6593d-144">Öppna din rekognoseringar-fil när du uppmanas till det.</span><span class="sxs-lookup"><span data-stu-id="6593d-144">When prompted, open your recon file.</span></span>

### <a name="open-a-recon-file-in-an-excel-pivot-table"></a><span data-ttu-id="6593d-145">Öppna en rekognoseringar-fil i en pivottabell i Excel</span><span class="sxs-lookup"><span data-stu-id="6593d-145">Open a recon file in an Excel pivot table</span></span>

1. <span data-ttu-id="6593d-146">Ladda ned avstämnings filen precis som vanligt.</span><span class="sxs-lookup"><span data-stu-id="6593d-146">Download the reconciliation file as you normally would.</span></span>
2. <span data-ttu-id="6593d-147">Öppna en ny fil i Microsoft Excel.</span><span class="sxs-lookup"><span data-stu-id="6593d-147">Open a new file in Microsoft Excel.</span></span>
3. <span data-ttu-id="6593d-148">På fliken **data** väljer du **Hämta data**, Välj **från fil** och välj sedan **text/CSV**.</span><span class="sxs-lookup"><span data-stu-id="6593d-148">On the **Data** tab, select **Get data**, select **From file**, and then select **Text/CSV**.</span></span>
4. <span data-ttu-id="6593d-149">Öppna din rekognoseringar-fil när du uppmanas till det.</span><span class="sxs-lookup"><span data-stu-id="6593d-149">When prompted, open your recon file.</span></span> <span data-ttu-id="6593d-150">Dina data kommer att visas.</span><span class="sxs-lookup"><span data-stu-id="6593d-150">Your data will appear.</span></span>
5. <span data-ttu-id="6593d-151">I list **Rute** menyn väljer **du Läs in till** och sedan **OK**.</span><span class="sxs-lookup"><span data-stu-id="6593d-151">In the **Load** dropdown menu, select **Load to**, and then **OK**.</span></span>
6. <span data-ttu-id="6593d-152">I dialog rutan **Importera data** väljer du **Pivot** -registerrapport för att öppna filen.</span><span class="sxs-lookup"><span data-stu-id="6593d-152">In the **Import Data** dialog box, select **PivotTable Report** to open your file.</span></span>

## <a name="map-taxes-or-vat"></a><span data-ttu-id="6593d-153">Mappa skatter eller moms</span><span class="sxs-lookup"><span data-stu-id="6593d-153">Map taxes or VAT</span></span>

<span data-ttu-id="6593d-154">Så här mappar du skatter eller mervärdes skatt (moms) till din faktura:</span><span class="sxs-lookup"><span data-stu-id="6593d-154">To map Taxes or value-added tax (VAT) to your invoice:</span></span>

- <span data-ttu-id="6593d-155">Summera **moms** kolumnen från den licensbaserade filen.</span><span class="sxs-lookup"><span data-stu-id="6593d-155">Sum the **Tax** column from the license-based file.</span></span>
- <span data-ttu-id="6593d-156">Summera kolumnen **TaxAmount** från den Usage-baserade filen.</span><span class="sxs-lookup"><span data-stu-id="6593d-156">Sum the **TaxAmount** column from the usage-based file.</span></span>

## <a name="itemize-reconciliation-files-by-partner"></a><span data-ttu-id="6593d-157">Specificera avstämnings filer efter partner</span><span class="sxs-lookup"><span data-stu-id="6593d-157">Itemize reconciliation files by partner</span></span>

<span data-ttu-id="6593d-158">Partner i den **indirekta modellen** kan använda dessa ytterligare fält i både licensbaserade och användnings bara avstämnings filer för att specificera filerna efter åter försäljare.</span><span class="sxs-lookup"><span data-stu-id="6593d-158">Partners in the **indirect model** can use these additional fields in both license-based and usage-based reconciliation files to itemize the files by reseller.</span></span>

| <span data-ttu-id="6593d-159">MPN-ID</span><span class="sxs-lookup"><span data-stu-id="6593d-159">MPN ID</span></span> | <span data-ttu-id="6593d-160">Description</span><span class="sxs-lookup"><span data-stu-id="6593d-160">Description</span></span> |
| ------ | ----------- |
| <span data-ttu-id="6593d-161">MPN-ID</span><span class="sxs-lookup"><span data-stu-id="6593d-161">MPN ID</span></span> | <span data-ttu-id="6593d-162">Microsoft Partner Network-ID (MPN) för Cloud Solution Provider (CSP)-partner (direkt eller indirekt).</span><span class="sxs-lookup"><span data-stu-id="6593d-162">The Microsoft Partner Network (MPN) identifier of the Cloud Solution Provider (CSP) partner (direct or indirect).</span></span> |
| [<span data-ttu-id="6593d-163">MPN-ID för åter försäljare</span><span class="sxs-lookup"><span data-stu-id="6593d-163">Reseller MPN ID</span></span>](#reseller-mpn-id) | <span data-ttu-id="6593d-164">[MPN identifierare för åter försäljaren av posten för prenumerationen](#reseller-mpn-id).</span><span class="sxs-lookup"><span data-stu-id="6593d-164">The [MPN identifier of the reseller of record for the subscription](#reseller-mpn-id).</span></span> <span data-ttu-id="6593d-165">Det här fältet motsvarar det åter försäljar-ID som anges för den aktuella prenumerationen i Partner Center.</span><span class="sxs-lookup"><span data-stu-id="6593d-165">This field corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span> <span data-ttu-id="6593d-166">Visas endast i avstämnings filer för partner i den indirekta modellen.</span><span class="sxs-lookup"><span data-stu-id="6593d-166">Only appears on reconciliation files for partners in the indirect model.</span></span> |

### <a name="reseller-mpn-id"></a><span data-ttu-id="6593d-167">MPN-ID för åter försäljare</span><span class="sxs-lookup"><span data-stu-id="6593d-167">Reseller MPN ID</span></span>

<span data-ttu-id="6593d-168">Om en CSP-partner sålde prenumerationen direkt till kunden visas deras **MPN-ID** två gånger, som både **MPN-ID** och **åter försäljarens MPN-ID**.</span><span class="sxs-lookup"><span data-stu-id="6593d-168">If a CSP partner sold the subscription directly to the customer, their **MPN ID** is listed twice, as both the **MPN ID** and the **Reseller MPN ID**.</span></span>

<span data-ttu-id="6593d-169">Om en CSP-partner har en åter försäljare utan **MPN-ID** är det här värdet inställt på partnerns **MPN-ID** i stället.</span><span class="sxs-lookup"><span data-stu-id="6593d-169">If a CSP partner has a reseller with no **MPN ID**, this value is set to the partner's **MPN ID** instead.</span></span>

<span data-ttu-id="6593d-170">Om CSP-partnern tar bort ett **MPN-ID för åter försäljaren** anges värdet *-1*.</span><span class="sxs-lookup"><span data-stu-id="6593d-170">If the CSP partner removes a **Reseller MPN ID**, this value will be set to *-1*.</span></span>

<span data-ttu-id="6593d-171">Visa eller uppdatera **MPN-ID: t för åter försäljaren**:</span><span class="sxs-lookup"><span data-stu-id="6593d-171">To view or update the **Reseller MPN ID**:</span></span>

1. <span data-ttu-id="6593d-172">Logga in på Partner Center.</span><span class="sxs-lookup"><span data-stu-id="6593d-172">Sign in to Partner Center.</span></span>
2. <span data-ttu-id="6593d-173">I menyn Partner Center väljer du **kunder**.</span><span class="sxs-lookup"><span data-stu-id="6593d-173">In the Partner Center menu, select **Customers**.</span></span>
3. <span data-ttu-id="6593d-174">Välj kund i listan.</span><span class="sxs-lookup"><span data-stu-id="6593d-174">Choose the customer from the list.</span></span>
4. <span data-ttu-id="6593d-175">I menyn kund väljer du **prenumerationer**.</span><span class="sxs-lookup"><span data-stu-id="6593d-175">In the customer menu, select **Subscriptions**.</span></span>
5. <span data-ttu-id="6593d-176">Välj prenumerationen i listan.</span><span class="sxs-lookup"><span data-stu-id="6593d-176">Choose the subscription from the list.</span></span>
6. <span data-ttu-id="6593d-177">Välj **Uppdatera** för att ändra **åter försäljaren (MPN-ID)**.</span><span class="sxs-lookup"><span data-stu-id="6593d-177">Select **update** to change the **Reseller (MPN ID)**.</span></span>

## <a name="next-steps"></a><span data-ttu-id="6593d-178">Nästa steg</span><span class="sxs-lookup"><span data-stu-id="6593d-178">Next steps</span></span>

- [<span data-ttu-id="6593d-179">Så här läser du rekognoseringar-filen för Bill &</span><span class="sxs-lookup"><span data-stu-id="6593d-179">How to read your bill & recon file</span></span>](read-your-bill.md) 