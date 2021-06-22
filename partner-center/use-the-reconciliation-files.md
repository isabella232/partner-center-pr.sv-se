---
title: Använda avstämningsfiler
ms.topic: article
ms.date: 03/26/2021
description: Lär dig mer om avstämningsfiler i Partnercenter och hur du tolkar detaljerade, radobjektsvyer av avgifter för en viss faktureringsperiod.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 1a7d5f3169c4b338a07475a7e246e87841b8dcfb
ms.sourcegitcommit: bce54ddb9fff7332a03d6aa228ba9414a87d76b7
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/22/2021
ms.locfileid: "112431561"
---
# <a name="learn-how-to-read-the-line-items-in-your-partner-center-reconciliation-files"></a><span data-ttu-id="4a0f9-103">Lär dig hur du läser radobjekten i avstämningsfilerna i Partnercenter</span><span class="sxs-lookup"><span data-stu-id="4a0f9-103">Learn how to read the line items in your Partner Center reconciliation files</span></span>

<span data-ttu-id="4a0f9-104">**Lämpliga roller:** Faktureringsadministratör | Global administratör</span><span class="sxs-lookup"><span data-stu-id="4a0f9-104">**Appropriate roles**: Billing admin | Global admin</span></span>

<span data-ttu-id="4a0f9-105">Du kan ladda ned avstämningsfilerna från Partnercenter för en detaljerad radobjektsvy för varje avgift i en faktureringsperiod.</span><span class="sxs-lookup"><span data-stu-id="4a0f9-105">You can download your reconciliation files from Partner Center for a detailed, line-item view of each charge in a billing cycle.</span></span> <span data-ttu-id="4a0f9-106">Information om radobjekt inkluderar avgifter för varje kunds prenumerationer och detaljerade händelser (till exempel ett halvtids tillägg av licenser i en prenumeration).</span><span class="sxs-lookup"><span data-stu-id="4a0f9-106">Line-item details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of licenses to a subscription).</span></span>

<span data-ttu-id="4a0f9-107">Information om hur du läser din **faktura finns** i Läsa [din faktura.](read-your-bill.md)</span><span class="sxs-lookup"><span data-stu-id="4a0f9-107">For information on how to read your **invoice**, see [Read your bill](read-your-bill.md).</span></span>

## <a name="understand-reconciliation-file-fields"></a><span data-ttu-id="4a0f9-108">Förstå avstämningsfilfält</span><span class="sxs-lookup"><span data-stu-id="4a0f9-108">Understand reconciliation file fields</span></span>

- [<span data-ttu-id="4a0f9-109">Fält för licensbaserad avstämningsfil</span><span class="sxs-lookup"><span data-stu-id="4a0f9-109">License-based reconciliation file fields</span></span>](license-based-recon-files.md)
- [<span data-ttu-id="4a0f9-110">Fält för användningsbaserad avstämningsfil</span><span class="sxs-lookup"><span data-stu-id="4a0f9-110">Usage-based reconciliation file fields</span></span>](usage-based-recon-files.md)
- [<span data-ttu-id="4a0f9-111">Fält i fil för dagligt beräknad användningsavstämning</span><span class="sxs-lookup"><span data-stu-id="4a0f9-111">Daily-rated usage reconciliation file fields</span></span>](daily-rated-usage-recon-files.md)
- [<span data-ttu-id="4a0f9-112">Fält för CSP-avstämningsfil vid ett köp</span><span class="sxs-lookup"><span data-stu-id="4a0f9-112">One-time purchase CSP reconciliation file fields</span></span>](modern-invoice-reconciliation-file.md)

## <a name="understand-charge-types-in-reconciliation-files"></a><span data-ttu-id="4a0f9-113">Förstå avgiftstyper i avstämningsfiler</span><span class="sxs-lookup"><span data-stu-id="4a0f9-113">Understand charge types in reconciliation files</span></span>

<span data-ttu-id="4a0f9-114">Information om vilka typer av avgifter som finns i avstämningsfiler **(kolumnen ChargeType)** finns i [Avgiftstyper för avstämningsfiler.](recon-file-charge-types.md)</span><span class="sxs-lookup"><span data-stu-id="4a0f9-114">To understand the types of charges in reconciliation files (the **ChargeType** column), see [Reconciliation file charge types](recon-file-charge-types.md).</span></span>

## <a name="fix-formatting-issues"></a><span data-ttu-id="4a0f9-115">Åtgärda formateringsproblem</span><span class="sxs-lookup"><span data-stu-id="4a0f9-115">Fix formatting issues</span></span>

<span data-ttu-id="4a0f9-116">Ibland kan en avstämningsfil innehålla formateringsproblem.</span><span class="sxs-lookup"><span data-stu-id="4a0f9-116">Occasionally, a reconciliation file might contain formatting issues.</span></span> <span data-ttu-id="4a0f9-117">Det här problemet kan till exempel inträffa om språken en-US inte används.</span><span class="sxs-lookup"><span data-stu-id="4a0f9-117">For example, this issue might occur if the en-US locale is not used.</span></span>

<span data-ttu-id="4a0f9-118">Följ de här stegen för att åtgärda eventuella formateringsproblem i avstämningsfilerna:</span><span class="sxs-lookup"><span data-stu-id="4a0f9-118">Follow these steps for fix any formatting issues in your reconciliation files:</span></span>

1. <span data-ttu-id="4a0f9-119">Öppna avstämningsfilen (i .csv format) i Microsoft Excel.</span><span class="sxs-lookup"><span data-stu-id="4a0f9-119">Open the reconciliation file (in .csv format) in Microsoft Excel.</span></span>
2. <span data-ttu-id="4a0f9-120">Välj den första kolumnen i filen.</span><span class="sxs-lookup"><span data-stu-id="4a0f9-120">Select the first column in the file.</span></span>
3. <span data-ttu-id="4a0f9-121">Öppna guiden **Konvertera text till kolumner.**</span><span class="sxs-lookup"><span data-stu-id="4a0f9-121">Open the **Convert Text to Columns Wizard**.</span></span> <span data-ttu-id="4a0f9-122">I menyfliksområdet väljer du **Data** och sedan **Text till kolumner.**</span><span class="sxs-lookup"><span data-stu-id="4a0f9-122">On the ribbon, select **Data**, then select **Text to Columns**.</span></span>
4. <span data-ttu-id="4a0f9-123">I guiden väljer du **Avgränsad filtyp.**</span><span class="sxs-lookup"><span data-stu-id="4a0f9-123">In the wizard, select **Delimited file type**.</span></span> <span data-ttu-id="4a0f9-124">Välj **Nästa**.</span><span class="sxs-lookup"><span data-stu-id="4a0f9-124">Then, select **Next**.</span></span>
5. <span data-ttu-id="4a0f9-125">I **fältet Avgränsare** väljer du **kommatecken**.</span><span class="sxs-lookup"><span data-stu-id="4a0f9-125">In the **Delimiters** field, select **Comma**.</span></span> <span data-ttu-id="4a0f9-126">(Om **Tabb** redan är markerat kan du lämna det här alternativet markerat.) Välj sedan **Nästa.**</span><span class="sxs-lookup"><span data-stu-id="4a0f9-126">(If **Tab** is already selected, you can leave this option selected.) Then, select **Next**.</span></span>
6. <span data-ttu-id="4a0f9-127">I fältet **Kolumndataformat** väljer du **Datum:MDY.**</span><span class="sxs-lookup"><span data-stu-id="4a0f9-127">In the **Column data format** field, select **Date:MDY**.</span></span> <span data-ttu-id="4a0f9-128">Välj **Nästa**.</span><span class="sxs-lookup"><span data-stu-id="4a0f9-128">Then, select **Next**.</span></span>
7. <span data-ttu-id="4a0f9-129">I fältet **Kolumndataformat** väljer du **Text för** alla mängdkolumner.</span><span class="sxs-lookup"><span data-stu-id="4a0f9-129">In the **Column data format** field, select **Text** for all amount columns.</span></span> <span data-ttu-id="4a0f9-130">Välj sedan **Slutför**.</span><span class="sxs-lookup"><span data-stu-id="4a0f9-130">Then, select **Finish**.</span></span>

## <a name="download-reconciliation-files-programmatically"></a><span data-ttu-id="4a0f9-131">Ladda ned avstämningsfiler programmatiskt</span><span class="sxs-lookup"><span data-stu-id="4a0f9-131">Download reconciliation files programmatically</span></span>

<span data-ttu-id="4a0f9-132">Avstämningsfiler kan vara mycket stora och ibland svåra att ladda ned.</span><span class="sxs-lookup"><span data-stu-id="4a0f9-132">Reconciliation files can be very large and are sometimes difficult to download.</span></span> <span data-ttu-id="4a0f9-133">Information om hur du laddar ned avstämningsfiler programmatiskt [finns i Hämta fakturaradsobjekt.](/partner-center/develop/get-invoiceline-items)</span><span class="sxs-lookup"><span data-stu-id="4a0f9-133">To download reconciliation files programmatically, see [Get invoice line items](/partner-center/develop/get-invoiceline-items).</span></span>

## <a name="if-your-file-exceeds-the-row-limit-in-excel"></a><span data-ttu-id="4a0f9-134">Om filen överskrider radgränsen i Excel</span><span class="sxs-lookup"><span data-stu-id="4a0f9-134">If your file exceeds the row limit in Excel</span></span>

<span data-ttu-id="4a0f9-135">Om du kan ladda ned en avstämningsfil men inte öppna den i Microsoft Excel, innebär det förmodligen att filen innehåller fler rader än Vad som tillåts i Excel.</span><span class="sxs-lookup"><span data-stu-id="4a0f9-135">If you’re able to download a reconciliation file but not open it in Microsoft Excel, it probably means the file contains more rows than Excel will allow.</span></span> <span data-ttu-id="4a0f9-136">Om detta inträffar kan du använda någon av procedurerna nedan för att öppna filen.</span><span class="sxs-lookup"><span data-stu-id="4a0f9-136">If this happens, you can use either of the procedures below to open the file.</span></span>

### <a name="open-a-recon-file-in-power-bi"></a><span data-ttu-id="4a0f9-137">Öppna en rekognoseringsfil i Power BI</span><span class="sxs-lookup"><span data-stu-id="4a0f9-137">Open a recon file in Power BI</span></span>

1. <span data-ttu-id="4a0f9-138">Ladda ned avstämningsfilen som vanligt.</span><span class="sxs-lookup"><span data-stu-id="4a0f9-138">Download the reconciliation file as you normally would.</span></span>
2. <span data-ttu-id="4a0f9-139">Ladda ned, installera och öppna en instans av Microsoft Power BI.</span><span class="sxs-lookup"><span data-stu-id="4a0f9-139">Download, install, and open an instance of Microsoft Power BI.</span></span>
3. <span data-ttu-id="4a0f9-140">På Power BI **Start** väljer du **Hämta data.**</span><span class="sxs-lookup"><span data-stu-id="4a0f9-140">On the Power BI **Home** tab, select **Get data**.</span></span>
4. <span data-ttu-id="4a0f9-141">I listan över **vanliga datakällor väljer** du **Text/CSV.**</span><span class="sxs-lookup"><span data-stu-id="4a0f9-141">In the list of **Common data sources**, select **Text/CSV**.</span></span>
5. <span data-ttu-id="4a0f9-142">Öppna rekognoseringsfilen när du uppmanas till det.</span><span class="sxs-lookup"><span data-stu-id="4a0f9-142">When prompted, open your recon file.</span></span>

### <a name="open-a-recon-file-in-an-excel-pivot-table"></a><span data-ttu-id="4a0f9-143">Öppna en rekognoseringsfil i en Excel-pivottabell</span><span class="sxs-lookup"><span data-stu-id="4a0f9-143">Open a recon file in an Excel pivot table</span></span>

1. <span data-ttu-id="4a0f9-144">Ladda ned avstämningsfilen som vanligt.</span><span class="sxs-lookup"><span data-stu-id="4a0f9-144">Download the reconciliation file as you normally would.</span></span>
2. <span data-ttu-id="4a0f9-145">Öppna en ny fil i Microsoft Excel.</span><span class="sxs-lookup"><span data-stu-id="4a0f9-145">Open a new file in Microsoft Excel.</span></span>
3. <span data-ttu-id="4a0f9-146">På fliken **Data** väljer du **Hämta data,** väljer **Från fil** och sedan **Text/CSV.**</span><span class="sxs-lookup"><span data-stu-id="4a0f9-146">On the **Data** tab, select **Get data**, select **From file**, and then select **Text/CSV**.</span></span>
4. <span data-ttu-id="4a0f9-147">Öppna rekognoseringsfilen när du uppmanas till det.</span><span class="sxs-lookup"><span data-stu-id="4a0f9-147">When prompted, open your recon file.</span></span> <span data-ttu-id="4a0f9-148">Dina data visas.</span><span class="sxs-lookup"><span data-stu-id="4a0f9-148">Your data will appear.</span></span>
5. <span data-ttu-id="4a0f9-149">I **listrutan** Läs in väljer du **Läs in till** och sedan **OK.**</span><span class="sxs-lookup"><span data-stu-id="4a0f9-149">In the **Load** dropdown menu, select **Load to**, and then select **OK**.</span></span>
6. <span data-ttu-id="4a0f9-150">I dialogrutan **Importera data** väljer du **Pivottabellrapport för** att öppna filen.</span><span class="sxs-lookup"><span data-stu-id="4a0f9-150">In the **Import Data** dialog box, select **PivotTable Report** to open your file.</span></span>

## <a name="negative-amount-displayed"></a><span data-ttu-id="4a0f9-151">Negativt belopp visas</span><span class="sxs-lookup"><span data-stu-id="4a0f9-151">Negative amount displayed</span></span>

<span data-ttu-id="4a0f9-152">Du kan se ett negativt belopp i avstämningsfilen.</span><span class="sxs-lookup"><span data-stu-id="4a0f9-152">You may see a negative amount in your reconciliation file.</span></span> <span data-ttu-id="4a0f9-153">Detta beror troligtvis på något av följande:</span><span class="sxs-lookup"><span data-stu-id="4a0f9-153">This is probably caused by one of the following things:</span></span>

- <span data-ttu-id="4a0f9-154">Du har nyligen avbrutit eller minskat antalet licenser</span><span class="sxs-lookup"><span data-stu-id="4a0f9-154">You recently canceled or reduced your number of licenses</span></span>
- <span data-ttu-id="4a0f9-155">Du har fått kredit för antingen ett servicelicensavtal (SLA) eller för Azure-förbrukning</span><span class="sxs-lookup"><span data-stu-id="4a0f9-155">You received credit for either a service license agreement (SLA) or for Azure consumption</span></span>

<span data-ttu-id="4a0f9-156">Om du vill få mer information om den här transaktionen granskar du dess attribut av avgiftstyp i avstämningsfilen.</span><span class="sxs-lookup"><span data-stu-id="4a0f9-156">To get more information about this transaction, review its charge type attribute in your reconciliation file.</span></span>

## <a name="map-taxes-or-vat"></a><span data-ttu-id="4a0f9-157">Mappa skatter eller moms</span><span class="sxs-lookup"><span data-stu-id="4a0f9-157">Map taxes or VAT</span></span>

<span data-ttu-id="4a0f9-158">Så här mappar du Skatter eller moms till din faktura:</span><span class="sxs-lookup"><span data-stu-id="4a0f9-158">To map Taxes or value-added tax (VAT) to your invoice:</span></span>

- <span data-ttu-id="4a0f9-159">Summera **kolumnen** Skatt från den licensbaserade filen.</span><span class="sxs-lookup"><span data-stu-id="4a0f9-159">Sum the **Tax** column from the license-based file.</span></span>
- <span data-ttu-id="4a0f9-160">Summera **kolumnen TaxAmount** från den användningsbaserade filen.</span><span class="sxs-lookup"><span data-stu-id="4a0f9-160">Sum the **TaxAmount** column from the usage-based file.</span></span>

## <a name="itemize-reconciliation-files-by-partner"></a><span data-ttu-id="4a0f9-161">Specificera avstämningsfiler efter partner</span><span class="sxs-lookup"><span data-stu-id="4a0f9-161">Itemize reconciliation files by partner</span></span>

<span data-ttu-id="4a0f9-162">Partner i den **indirekta modellen** kan använda dessa ytterligare fält i både licensbaserade och användningsbaserade avstämningsfiler för att specificera filerna efter återförsäljare.</span><span class="sxs-lookup"><span data-stu-id="4a0f9-162">Partners in the **indirect model** can use these additional fields in both license-based and usage-based reconciliation files to itemize the files by reseller.</span></span>

| <span data-ttu-id="4a0f9-163">MPN-ID</span><span class="sxs-lookup"><span data-stu-id="4a0f9-163">MPN ID</span></span> | <span data-ttu-id="4a0f9-164">Beskrivning</span><span class="sxs-lookup"><span data-stu-id="4a0f9-164">Description</span></span> |
| ------ | ----------- |
| <span data-ttu-id="4a0f9-165">MPN-ID</span><span class="sxs-lookup"><span data-stu-id="4a0f9-165">MPN ID</span></span> | <span data-ttu-id="4a0f9-166">Den Microsoft Partner Network (MPN) identifierare för Molnlösningsleverantör (CSP)-partner (direkt eller indirekt).</span><span class="sxs-lookup"><span data-stu-id="4a0f9-166">The Microsoft Partner Network (MPN) identifier of the Cloud Solution Provider (CSP) partner (direct or indirect).</span></span> |
| [<span data-ttu-id="4a0f9-167">MPN-ID för återförsäljare</span><span class="sxs-lookup"><span data-stu-id="4a0f9-167">Reseller MPN ID</span></span>](#reseller-mpn-id) | <span data-ttu-id="4a0f9-168">[MPN-identifieraren för återförsäljaren av posten för prenumerationen](#reseller-mpn-id).</span><span class="sxs-lookup"><span data-stu-id="4a0f9-168">The [MPN identifier of the reseller of record for the subscription](#reseller-mpn-id).</span></span> <span data-ttu-id="4a0f9-169">Det här fältet motsvarar det återförsäljar-ID som anges för den specifika prenumerationen i Partnercenter.</span><span class="sxs-lookup"><span data-stu-id="4a0f9-169">This field corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span> <span data-ttu-id="4a0f9-170">Visas endast i avstämningsfiler för partner i den indirekta modellen.</span><span class="sxs-lookup"><span data-stu-id="4a0f9-170">Only appears on reconciliation files for partners in the indirect model.</span></span> |

### <a name="reseller-mpn-id"></a><span data-ttu-id="4a0f9-171">MPN-ID för återförsäljare</span><span class="sxs-lookup"><span data-stu-id="4a0f9-171">Reseller MPN ID</span></span>

<span data-ttu-id="4a0f9-172">Om en CSP-partner sålde prenumerationen direkt till kunden visas deras **MPN-ID** två gånger, både som **MPN-ID** och **ÅTERFÖRSÄLJAREns MPN-ID.**</span><span class="sxs-lookup"><span data-stu-id="4a0f9-172">If a CSP partner sold the subscription directly to the customer, their **MPN ID** is listed twice, as both the **MPN ID** and the **Reseller MPN ID**.</span></span>

<span data-ttu-id="4a0f9-173">Om en CSP-partner har en återförsäljare utan **MPN-ID** anges det här värdet till partnerns **MPN-ID i** stället.</span><span class="sxs-lookup"><span data-stu-id="4a0f9-173">If a CSP partner has a reseller with no **MPN ID**, this value is set to the partner's **MPN ID** instead.</span></span>

<span data-ttu-id="4a0f9-174">Om CSP-partnern tar bort **ett MPN-ID** för återförsäljare anges det här värdet till *-1.*</span><span class="sxs-lookup"><span data-stu-id="4a0f9-174">If the CSP partner removes a **Reseller MPN ID**, this value will be set to *-1*.</span></span>

<span data-ttu-id="4a0f9-175">Så här visar eller uppdaterar du **MPN-ID:t för återförsäljare:**</span><span class="sxs-lookup"><span data-stu-id="4a0f9-175">To view or update the **Reseller MPN ID**:</span></span>

1. <span data-ttu-id="4a0f9-176">Logga in på Partner Center.</span><span class="sxs-lookup"><span data-stu-id="4a0f9-176">Sign in to Partner Center.</span></span>
2. <span data-ttu-id="4a0f9-177">I menyn i Partnercenter väljer du **Kunder.**</span><span class="sxs-lookup"><span data-stu-id="4a0f9-177">In the Partner Center menu, select **Customers**.</span></span>
3. <span data-ttu-id="4a0f9-178">Välj kunden i listan.</span><span class="sxs-lookup"><span data-stu-id="4a0f9-178">Choose the customer from the list.</span></span>
4. <span data-ttu-id="4a0f9-179">I kundmenyn väljer du **Prenumerationer.**</span><span class="sxs-lookup"><span data-stu-id="4a0f9-179">In the customer menu, select **Subscriptions**.</span></span>
5. <span data-ttu-id="4a0f9-180">Välj prenumerationen i listan.</span><span class="sxs-lookup"><span data-stu-id="4a0f9-180">Choose the subscription from the list.</span></span>
6. <span data-ttu-id="4a0f9-181">Välj **uppdatera** för att ändra **Reseller (MPN ID)**.</span><span class="sxs-lookup"><span data-stu-id="4a0f9-181">Select **update** to change the **Reseller (MPN ID)**.</span></span>

## <a name="next-steps"></a><span data-ttu-id="4a0f9-182">Nästa steg</span><span class="sxs-lookup"><span data-stu-id="4a0f9-182">Next steps</span></span>

- [<span data-ttu-id="4a0f9-183">Så här läser du fakturan & rekognoseringsfilen</span><span class="sxs-lookup"><span data-stu-id="4a0f9-183">How to read your bill & recon file</span></span>](read-your-bill.md) 