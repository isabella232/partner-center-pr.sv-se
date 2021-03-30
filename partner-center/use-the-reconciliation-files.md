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
ms.openlocfilehash: aefd5258c778fd8a7b92bfe49f245bf818497fb8
ms.sourcegitcommit: dd51744a4af3797493a5ebbfc766dab86ff00477
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/29/2021
ms.locfileid: "105730099"
---
# <a name="learn-how-to-read-the-line-items-in-your-partner-center-reconciliation-files"></a><span data-ttu-id="54a86-103">Lär dig hur du läser rad objekt i dina avstämnings filer för partner Center</span><span class="sxs-lookup"><span data-stu-id="54a86-103">Learn how to read the line items in your Partner Center reconciliation files</span></span>

<span data-ttu-id="54a86-104">**Lämpliga roller**</span><span class="sxs-lookup"><span data-stu-id="54a86-104">**Appropriate roles**</span></span>

- <span data-ttu-id="54a86-105">Faktureringsadministratör</span><span class="sxs-lookup"><span data-stu-id="54a86-105">Billing admin</span></span>
- <span data-ttu-id="54a86-106">Global administratör</span><span class="sxs-lookup"><span data-stu-id="54a86-106">Global admin</span></span>

<span data-ttu-id="54a86-107">Du kan ladda ned dina avstämnings filer från Partner Center för en detaljerad, rad objekt visning av varje debitering i en fakturerings period.</span><span class="sxs-lookup"><span data-stu-id="54a86-107">You can download your reconciliation files from Partner Center for a detailed, line-item view of each charge in a billing cycle.</span></span> <span data-ttu-id="54a86-108">Information om rad objekt inkluderar avgifter för varje kunds prenumerationer och detaljerade händelser (till exempel ett omslags kort tillägg av licenser till en prenumeration).</span><span class="sxs-lookup"><span data-stu-id="54a86-108">Line-item details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of licenses to a subscription).</span></span>

<span data-ttu-id="54a86-109">Information om hur du läser fakturan finns i [läsa din](read-your-bill.md) **faktura**.</span><span class="sxs-lookup"><span data-stu-id="54a86-109">For information on how to read your **invoice**, see [Read your bill](read-your-bill.md).</span></span>

## <a name="understand-reconciliation-file-fields"></a><span data-ttu-id="54a86-110">Förstå fält för avstämnings fil</span><span class="sxs-lookup"><span data-stu-id="54a86-110">Understand reconciliation file fields</span></span>

- [<span data-ttu-id="54a86-111">Fält för licensbaserad avstämningsfil</span><span class="sxs-lookup"><span data-stu-id="54a86-111">License-based reconciliation file fields</span></span>](license-based-recon-files.md)
- [<span data-ttu-id="54a86-112">Fält för användningsbaserad avstämningsfil</span><span class="sxs-lookup"><span data-stu-id="54a86-112">Usage-based reconciliation file fields</span></span>](usage-based-recon-files.md)
- [<span data-ttu-id="54a86-113">Fält i fil för dagligt beräknad användningsavstämning</span><span class="sxs-lookup"><span data-stu-id="54a86-113">Daily-rated usage reconciliation file fields</span></span>](daily-rated-usage-recon-files.md)
- [<span data-ttu-id="54a86-114">Fil fält för CSP-avstämning för inköp vid ett tillfälle</span><span class="sxs-lookup"><span data-stu-id="54a86-114">One-time purchase CSP reconciliation file fields</span></span>](modern-invoice-reconciliation-file.md)

## <a name="understand-charge-types-in-reconciliation-files"></a><span data-ttu-id="54a86-115">Förstå debiterings typer i avstämnings filer</span><span class="sxs-lookup"><span data-stu-id="54a86-115">Understand charge types in reconciliation files</span></span>

<span data-ttu-id="54a86-116">Information om vilka typer av kostnader som finns i avstämnings filer (kolumnen **ChargeType** ) finns i [fil avgifts typer för avstämning](recon-file-charge-types.md).</span><span class="sxs-lookup"><span data-stu-id="54a86-116">To understand the types of charges in reconciliation files (the **ChargeType** column), see [Reconciliation file charge types](recon-file-charge-types.md).</span></span>

## <a name="fix-formatting-issues"></a><span data-ttu-id="54a86-117">Åtgärda problem med formatering</span><span class="sxs-lookup"><span data-stu-id="54a86-117">Fix formatting issues</span></span>

<span data-ttu-id="54a86-118">Ibland kan en avstämnings fil innehålla formateringsfel.</span><span class="sxs-lookup"><span data-stu-id="54a86-118">Occasionally, a reconciliation file might contain formatting issues.</span></span> <span data-ttu-id="54a86-119">Det här problemet kan till exempel inträffa om en-US locale inte används.</span><span class="sxs-lookup"><span data-stu-id="54a86-119">For example, this issue might occur if the en-US locale is not used.</span></span>

<span data-ttu-id="54a86-120">Följ dessa steg för att åtgärda eventuella formateringsfel i dina avstämnings filer:</span><span class="sxs-lookup"><span data-stu-id="54a86-120">Follow these steps for fix any formatting issues in your reconciliation files:</span></span>

1. <span data-ttu-id="54a86-121">Öppna avstämnings filen (i CSV-format) i Microsoft Excel.</span><span class="sxs-lookup"><span data-stu-id="54a86-121">Open the reconciliation file (in .csv format) in Microsoft Excel.</span></span>
2. <span data-ttu-id="54a86-122">Markera den första kolumnen i filen.</span><span class="sxs-lookup"><span data-stu-id="54a86-122">Select the first column in the file.</span></span>
3. <span data-ttu-id="54a86-123">Öppna **guiden Omvandla text till kolumner**.</span><span class="sxs-lookup"><span data-stu-id="54a86-123">Open the **Convert Text to Columns Wizard**.</span></span> <span data-ttu-id="54a86-124">Välj **data** i menyfliksområdet och välj sedan **text till kolumner**.</span><span class="sxs-lookup"><span data-stu-id="54a86-124">On the ribbon, select **Data**, then select **Text to Columns**.</span></span>
4. <span data-ttu-id="54a86-125">Välj **avgränsad filtyp** i guiden.</span><span class="sxs-lookup"><span data-stu-id="54a86-125">In the wizard, select **Delimited file type**.</span></span> <span data-ttu-id="54a86-126">Välj **Nästa**.</span><span class="sxs-lookup"><span data-stu-id="54a86-126">Then, select **Next**.</span></span>
5. <span data-ttu-id="54a86-127">I fältet **avgränsare** väljer du **kommatecken**.</span><span class="sxs-lookup"><span data-stu-id="54a86-127">In the **Delimiters** field, select **Comma**.</span></span> <span data-ttu-id="54a86-128">(Om **fliken** redan har valts kan du lämna det här alternativet markerat.) Välj sedan **Nästa**.</span><span class="sxs-lookup"><span data-stu-id="54a86-128">(If **Tab** is already selected, you can leave this option selected.) Then, select **Next**.</span></span>
6. <span data-ttu-id="54a86-129">I fältet **kolumn data format** väljer du **datum: MDÅ**.</span><span class="sxs-lookup"><span data-stu-id="54a86-129">In the **Column data format** field, select **Date:MDY**.</span></span> <span data-ttu-id="54a86-130">Välj **Nästa**.</span><span class="sxs-lookup"><span data-stu-id="54a86-130">Then, select **Next**.</span></span>
7. <span data-ttu-id="54a86-131">I fältet **kolumn data format** väljer du **text** för alla belopps kolumner.</span><span class="sxs-lookup"><span data-stu-id="54a86-131">In the **Column data format** field, select **Text** for all amount columns.</span></span> <span data-ttu-id="54a86-132">Välj sedan **Slutför**.</span><span class="sxs-lookup"><span data-stu-id="54a86-132">Then, select **Finish**.</span></span>

## <a name="download-reconciliation-files-programmatically"></a><span data-ttu-id="54a86-133">Ladda ned filer för avstämning program mässigt</span><span class="sxs-lookup"><span data-stu-id="54a86-133">Download reconciliation files programmatically</span></span>

<span data-ttu-id="54a86-134">Avstämnings filer kan vara mycket stora och är ibland svåra att ladda ned.</span><span class="sxs-lookup"><span data-stu-id="54a86-134">Reconciliation files can be very large and are sometimes difficult to download.</span></span> <span data-ttu-id="54a86-135">Information om hur du hämtar avstämnings filer program mässigt finns i [Hämta faktura rads objekt](/partner-center/develop/get-invoiceline-items).</span><span class="sxs-lookup"><span data-stu-id="54a86-135">To download reconciliation files programmatically, see [Get invoice line items](/partner-center/develop/get-invoiceline-items).</span></span>

## <a name="if-your-file-exceeds-the-row-limit-in-excel"></a><span data-ttu-id="54a86-136">Om filen överskrider rad gränsen i Excel</span><span class="sxs-lookup"><span data-stu-id="54a86-136">If your file exceeds the row limit in Excel</span></span>

<span data-ttu-id="54a86-137">Om du kan ladda ned en avstämnings fil men inte öppna den i Microsoft Excel, betyder det förmodligen att filen innehåller fler rader än vad Excel tillåter.</span><span class="sxs-lookup"><span data-stu-id="54a86-137">If you’re able to download a reconciliation file but not open it in Microsoft Excel, it probably means the file contains more rows than Excel will allow.</span></span> <span data-ttu-id="54a86-138">I så fall kan du använda någon av stegen nedan för att öppna filen.</span><span class="sxs-lookup"><span data-stu-id="54a86-138">If this happens, you can use either of the procedures below to open the file.</span></span>

### <a name="open-a-recon-file-in-power-bi"></a><span data-ttu-id="54a86-139">Öppna en rekognoseringar-fil i Power BI</span><span class="sxs-lookup"><span data-stu-id="54a86-139">Open a recon file in Power BI</span></span>

1. <span data-ttu-id="54a86-140">Ladda ned avstämnings filen precis som vanligt.</span><span class="sxs-lookup"><span data-stu-id="54a86-140">Download the reconciliation file as you normally would.</span></span>
2. <span data-ttu-id="54a86-141">Ladda ned, installera och öppna en instans av Power BI.</span><span class="sxs-lookup"><span data-stu-id="54a86-141">Download, install, and open an instance of Power BI.</span></span>
3. <span data-ttu-id="54a86-142">På fliken Power BI **Start** väljer du **Hämta data**.</span><span class="sxs-lookup"><span data-stu-id="54a86-142">On the Power BI **Home** tab, select **Get data**.</span></span>
4. <span data-ttu-id="54a86-143">I listan med **vanliga data källor** väljer du **text/CSV**.</span><span class="sxs-lookup"><span data-stu-id="54a86-143">In the list of **Common data sources**, select **Text/CSV**.</span></span>
5. <span data-ttu-id="54a86-144">Öppna din rekognoseringar-fil när du uppmanas till det.</span><span class="sxs-lookup"><span data-stu-id="54a86-144">When prompted, open your recon file.</span></span>

### <a name="open-a-recon-file-in-an-excel-pivot-table"></a><span data-ttu-id="54a86-145">Öppna en rekognoseringar-fil i en pivottabell i Excel</span><span class="sxs-lookup"><span data-stu-id="54a86-145">Open a recon file in an Excel pivot table</span></span>

1. <span data-ttu-id="54a86-146">Ladda ned avstämnings filen precis som vanligt.</span><span class="sxs-lookup"><span data-stu-id="54a86-146">Download the reconciliation file as you normally would.</span></span>
2. <span data-ttu-id="54a86-147">Öppna en ny fil i Microsoft Excel.</span><span class="sxs-lookup"><span data-stu-id="54a86-147">Open a new file in Microsoft Excel.</span></span>
3. <span data-ttu-id="54a86-148">På fliken **data** väljer du **Hämta data**, Välj **från fil** och välj sedan **text/CSV**.</span><span class="sxs-lookup"><span data-stu-id="54a86-148">On the **Data** tab, select **Get data**, select **From file**, and then select **Text/CSV**.</span></span>
4. <span data-ttu-id="54a86-149">Öppna din rekognoseringar-fil när du uppmanas till det.</span><span class="sxs-lookup"><span data-stu-id="54a86-149">When prompted, open your recon file.</span></span> <span data-ttu-id="54a86-150">Dina data kommer att visas.</span><span class="sxs-lookup"><span data-stu-id="54a86-150">Your data will appear.</span></span>
5. <span data-ttu-id="54a86-151">I list **Rute** menyn väljer **du Läs in till** och sedan **OK**.</span><span class="sxs-lookup"><span data-stu-id="54a86-151">In the **Load** dropdown menu, select **Load to**, and then **OK**.</span></span>
6. <span data-ttu-id="54a86-152">I dialog rutan **Importera data** väljer du **Pivot** -registerrapport för att öppna filen.</span><span class="sxs-lookup"><span data-stu-id="54a86-152">In the **Import Data** dialog box, select **PivotTable Report** to open your file.</span></span>

## <a name="negative-amount-displayed"></a><span data-ttu-id="54a86-153">Negativt belopp visas</span><span class="sxs-lookup"><span data-stu-id="54a86-153">Negative amount displayed</span></span>

<span data-ttu-id="54a86-154">Du kan se ett negativt belopp i avstämnings filen.</span><span class="sxs-lookup"><span data-stu-id="54a86-154">You may see a negative amount in your reconciliation file.</span></span> <span data-ttu-id="54a86-155">Detta beror troligen på någon av följande saker:</span><span class="sxs-lookup"><span data-stu-id="54a86-155">This is probably caused by one of the following things:</span></span>

- <span data-ttu-id="54a86-156">Du har nyligen avbrutit eller minskat antalet licenser</span><span class="sxs-lookup"><span data-stu-id="54a86-156">You recently canceled or reduced your number of licenses</span></span>
- <span data-ttu-id="54a86-157">Du har fått kredit för antingen ett service licens avtal (SLA) eller för Azure-förbrukning</span><span class="sxs-lookup"><span data-stu-id="54a86-157">You received credit for either a service license agreement (SLA) or for Azure consumption</span></span>

<span data-ttu-id="54a86-158">Om du vill ha mer information om den här transaktionen granskar du ett attribut för debiterings typ i avstämnings filen.</span><span class="sxs-lookup"><span data-stu-id="54a86-158">To get more information about this transaction, review its charge type attribute in your reconciliation file.</span></span>

## <a name="map-taxes-or-vat"></a><span data-ttu-id="54a86-159">Mappa skatter eller moms</span><span class="sxs-lookup"><span data-stu-id="54a86-159">Map taxes or VAT</span></span>

<span data-ttu-id="54a86-160">Så här mappar du skatter eller mervärdes skatt (moms) till din faktura:</span><span class="sxs-lookup"><span data-stu-id="54a86-160">To map Taxes or value-added tax (VAT) to your invoice:</span></span>

- <span data-ttu-id="54a86-161">Summera **moms** kolumnen från den licensbaserade filen.</span><span class="sxs-lookup"><span data-stu-id="54a86-161">Sum the **Tax** column from the license-based file.</span></span>
- <span data-ttu-id="54a86-162">Summera kolumnen **TaxAmount** från den Usage-baserade filen.</span><span class="sxs-lookup"><span data-stu-id="54a86-162">Sum the **TaxAmount** column from the usage-based file.</span></span>

## <a name="itemize-reconciliation-files-by-partner"></a><span data-ttu-id="54a86-163">Specificera avstämnings filer efter partner</span><span class="sxs-lookup"><span data-stu-id="54a86-163">Itemize reconciliation files by partner</span></span>

<span data-ttu-id="54a86-164">Partner i den **indirekta modellen** kan använda dessa ytterligare fält i både licensbaserade och användnings bara avstämnings filer för att specificera filerna efter åter försäljare.</span><span class="sxs-lookup"><span data-stu-id="54a86-164">Partners in the **indirect model** can use these additional fields in both license-based and usage-based reconciliation files to itemize the files by reseller.</span></span>

| <span data-ttu-id="54a86-165">MPN-ID</span><span class="sxs-lookup"><span data-stu-id="54a86-165">MPN ID</span></span> | <span data-ttu-id="54a86-166">Beskrivning</span><span class="sxs-lookup"><span data-stu-id="54a86-166">Description</span></span> |
| ------ | ----------- |
| <span data-ttu-id="54a86-167">MPN-ID</span><span class="sxs-lookup"><span data-stu-id="54a86-167">MPN ID</span></span> | <span data-ttu-id="54a86-168">Microsoft Partner Network-ID (MPN) för Cloud Solution Provider (CSP)-partner (direkt eller indirekt).</span><span class="sxs-lookup"><span data-stu-id="54a86-168">The Microsoft Partner Network (MPN) identifier of the Cloud Solution Provider (CSP) partner (direct or indirect).</span></span> |
| [<span data-ttu-id="54a86-169">MPN-ID för åter försäljare</span><span class="sxs-lookup"><span data-stu-id="54a86-169">Reseller MPN ID</span></span>](#reseller-mpn-id) | <span data-ttu-id="54a86-170">[MPN identifierare för åter försäljaren av posten för prenumerationen](#reseller-mpn-id).</span><span class="sxs-lookup"><span data-stu-id="54a86-170">The [MPN identifier of the reseller of record for the subscription](#reseller-mpn-id).</span></span> <span data-ttu-id="54a86-171">Det här fältet motsvarar det åter försäljar-ID som anges för den aktuella prenumerationen i Partner Center.</span><span class="sxs-lookup"><span data-stu-id="54a86-171">This field corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span> <span data-ttu-id="54a86-172">Visas endast i avstämnings filer för partner i den indirekta modellen.</span><span class="sxs-lookup"><span data-stu-id="54a86-172">Only appears on reconciliation files for partners in the indirect model.</span></span> |

### <a name="reseller-mpn-id"></a><span data-ttu-id="54a86-173">MPN-ID för åter försäljare</span><span class="sxs-lookup"><span data-stu-id="54a86-173">Reseller MPN ID</span></span>

<span data-ttu-id="54a86-174">Om en CSP-partner sålde prenumerationen direkt till kunden visas deras **MPN-ID** två gånger, som både **MPN-ID** och **åter försäljarens MPN-ID**.</span><span class="sxs-lookup"><span data-stu-id="54a86-174">If a CSP partner sold the subscription directly to the customer, their **MPN ID** is listed twice, as both the **MPN ID** and the **Reseller MPN ID**.</span></span>

<span data-ttu-id="54a86-175">Om en CSP-partner har en åter försäljare utan **MPN-ID** är det här värdet inställt på partnerns **MPN-ID** i stället.</span><span class="sxs-lookup"><span data-stu-id="54a86-175">If a CSP partner has a reseller with no **MPN ID**, this value is set to the partner's **MPN ID** instead.</span></span>

<span data-ttu-id="54a86-176">Om CSP-partnern tar bort ett **MPN-ID för åter försäljaren** anges värdet *-1*.</span><span class="sxs-lookup"><span data-stu-id="54a86-176">If the CSP partner removes a **Reseller MPN ID**, this value will be set to *-1*.</span></span>

<span data-ttu-id="54a86-177">Visa eller uppdatera **MPN-ID: t för åter försäljaren**:</span><span class="sxs-lookup"><span data-stu-id="54a86-177">To view or update the **Reseller MPN ID**:</span></span>

1. <span data-ttu-id="54a86-178">Logga in på Partner Center.</span><span class="sxs-lookup"><span data-stu-id="54a86-178">Sign in to Partner Center.</span></span>
2. <span data-ttu-id="54a86-179">I menyn Partner Center väljer du **kunder**.</span><span class="sxs-lookup"><span data-stu-id="54a86-179">In the Partner Center menu, select **Customers**.</span></span>
3. <span data-ttu-id="54a86-180">Välj kund i listan.</span><span class="sxs-lookup"><span data-stu-id="54a86-180">Choose the customer from the list.</span></span>
4. <span data-ttu-id="54a86-181">I menyn kund väljer du **prenumerationer**.</span><span class="sxs-lookup"><span data-stu-id="54a86-181">In the customer menu, select **Subscriptions**.</span></span>
5. <span data-ttu-id="54a86-182">Välj prenumerationen i listan.</span><span class="sxs-lookup"><span data-stu-id="54a86-182">Choose the subscription from the list.</span></span>
6. <span data-ttu-id="54a86-183">Välj **Uppdatera** för att ändra **åter försäljaren (MPN-ID)**.</span><span class="sxs-lookup"><span data-stu-id="54a86-183">Select **update** to change the **Reseller (MPN ID)**.</span></span>

## <a name="next-steps"></a><span data-ttu-id="54a86-184">Nästa steg</span><span class="sxs-lookup"><span data-stu-id="54a86-184">Next steps</span></span>

- [<span data-ttu-id="54a86-185">Så här läser du rekognoseringar-filen för Bill &</span><span class="sxs-lookup"><span data-stu-id="54a86-185">How to read your bill & recon file</span></span>](read-your-bill.md) 