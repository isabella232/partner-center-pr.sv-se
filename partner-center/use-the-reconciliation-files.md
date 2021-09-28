---
title: Använda avstämningsfiler
ms.topic: article
ms.date: 09/27/2021
description: Lär dig mer om avstämningsfiler i Partnercenter och hur du tolkar detaljerade radobjektsvyer av avgifter för en viss faktureringsperiod.
ms.service: partner-dashboard
ms.subservice: partnercenter-billing
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 15767f57131013b2087f76145851ce7d122548ff
ms.sourcegitcommit: e1da62b36420d78bf44e3962358d0af65ebc3402
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/27/2021
ms.locfileid: "129088458"
---
# <a name="learn-how-to-read-the-line-items-in-your-partner-center-reconciliation-files"></a>Lär dig hur du läser radobjekten i avstämningsfilerna i Partnercenter

**Lämpliga roller:** Faktureringsadministratörsroller | Global administratör

Du kan ladda ned dina avstämningsfiler från Partnercenter för en detaljerad radobjektsvy för varje avgift i en faktureringsperiod. Information om radobjekt omfattar avgifter för varje kunds prenumerationer och detaljerade händelser (till exempel ett halvtids tillägg av licenser i en prenumeration).

Information om hur du läser din **faktura finns** i [Läsa fakturan.](read-your-bill.md)

## <a name="understand-reconciliation-file-fields"></a>Förstå avstämningsfilfält

- [Fält för licensbaserad avstämningsfil](license-based-recon-files.md)
- [Fält för användningsbaserad avstämningsfil](usage-based-recon-files.md)
- [Fält i fil för dagligt beräknad användningsavstämning](daily-rated-usage-recon-files.md)
- [Fält för CSP-avstämningsfil vid köp en gång](modern-invoice-reconciliation-file.md)

## <a name="understand-charge-types-in-reconciliation-files"></a>Förstå avgiftstyper i avstämningsfiler

Information om vilka typer av avgifter som finns i avstämningsfiler **(kolumnen ChargeType)** finns i [Avgiftstyper för avstämningsfiler.](recon-file-charge-types.md)

## <a name="fix-formatting-issues"></a>Åtgärda formateringsproblem

Ibland kan en avstämningsfil innehålla formateringsproblem. Det här problemet kan till exempel inträffa om språken en-US inte används.

Följ de här stegen för att åtgärda eventuella formateringsproblem i avstämningsfilerna:

1. Öppna avstämningsfilen (i .csv format) i Microsoft Excel.
2. Välj den första kolumnen i filen.
3. Öppna guiden **Konvertera text till kolumner.** I menyfliksområdet väljer du **Data** och sedan **Text till Kolumner.**
4. I guiden väljer du **Avgränsad filtyp.** Välj **Nästa**.
5. I fältet **Avgränsare** väljer du **Kommatecken.** (Om **Tabb** redan är markerat kan du lämna det här alternativet markerat.) Välj sedan **Nästa.**
6. I fältet **Kolumndataformat** väljer du **Datum:MDY.** Välj **Nästa**.
7. I fältet **Kolumndataformat** väljer du **Text för** alla mängdkolumner. Välj sedan **Slutför**.

## <a name="download-reconciliation-files-programmatically"></a>Ladda ned avstämningsfiler programmatiskt

Avstämningsfiler kan vara mycket stora och ibland svåra att ladda ned. Information om hur du laddar ned avstämningsfiler programmatiskt [finns i Hämta fakturaradsobjekt.](/partner-center/develop/get-invoiceline-items)

## <a name="if-your-file-exceeds-the-row-limit-in-excel"></a>Om filen överskrider radgränsen i Excel

Om du kan ladda ned en avstämningsfil men inte öppna den i Microsoft Excel innebär det förmodligen att filen innehåller fler rader än vad Excel tillåter. Om detta inträffar kan du använda någon av procedurerna nedan för att öppna filen.

### <a name="open-a-recon-file-in-power-bi"></a>Öppna en rekognoseringsfil i Power BI

1. Ladda ned avstämningsfilen som vanligt.
2. Ladda ned, installera och öppna en instans av Microsoft Power BI.
3. På fliken Power BI **väljer** du **Hämta data.**
4. I listan över **vanliga datakällor väljer** du **Text/CSV.**
5. Öppna rekognoseringsfilen när du uppmanas till det.

### <a name="open-a-recon-file-in-an-excel-pivot-table"></a>Öppna en rekognoseringsfil Excel en pivottabell

1. Ladda ned avstämningsfilen som vanligt.
2. Öppna en ny fil i Microsoft Excel.
3. På fliken **Data** väljer du **Hämta data,** väljer **Från fil** och sedan **Text/CSV.**
4. Öppna rekognoseringsfilen när du uppmanas till det. Dina data visas.
5. I **listrutan Läs** in väljer du **Läs in till** och sedan **OK.**
6. I dialogrutan **Importera data** väljer du **Pivottabellrapport för** att öppna filen.

## <a name="negative-amount-displayed"></a>Negativt belopp visas

Du kan se ett negativt belopp i avstämningsfilen. Detta beror troligtvis på något av följande:

- Du har nyligen avbrutit eller minskat antalet licenser
- Du har fått kredit för antingen ett servicelicensavtal (SLA) eller för Azure-förbrukning

Om du vill få mer information om den här transaktionen granskar du dess attribut av avgiftstyp i avstämningsfilen.

## <a name="map-taxes-or-vat"></a>Mappa skatter eller moms

Så här mappar du skatter eller moms till din faktura:

- Summera **kolumnen** Skatt från den licensbaserade filen.
- Summera **kolumnen TaxAmount** från den användningsbaserade filen.

## <a name="itemize-reconciliation-files-by-partner"></a>Specificera avstämningsfiler efter partner

Partner i den **indirekta modellen** kan använda dessa ytterligare fält i både licensbaserade och användningsbaserade avstämningsfiler för att specificera filerna efter återförsäljare.

| MPN-ID | Description |
| ------ | ----------- |
| MPN-ID | Mpn Microsoft Partner Network(Mpn)-id för Molnlösningsleverantör (CSP)-partner (direkt eller indirekt). |
| [MPN-ID för återförsäljare](#reseller-mpn-id) | [MPN-identifieraren för återförsäljaren av posten för prenumerationen](#reseller-mpn-id). Det här fältet motsvarar det återförsäljar-ID som anges för den specifika prenumerationen i Partnercenter. Visas endast i avstämningsfiler för partner i den indirekta modellen. |

### <a name="reseller-mpn-id"></a>MPN-ID för återförsäljare

Om en CSP-partner sålde prenumerationen direkt till kunden visas deras **MPN-ID** två gånger, både som **MPN-ID** och **ÅTERFÖRSÄLJAREns MPN-ID.**

Om en CSP-partner har en återförsäljare utan **MPN-ID** anges det här värdet till partnerns **MPN-ID i** stället.

Om CSP-partnern tar bort ett **MPN-ID** för återförsäljare anges det här värdet till *-1*.

Så här visar eller uppdaterar du **MPN-ID:t för återförsäljare:**

> [!NOTE]
> Mer information om gränssnittet för arbetsytor finns i [Getting around Partner Center (Ta sig runt i Partnercenter).](get-around-partner-center.md#turn-workspaces-on-and-off)

#### <a name="workspaces-view"></a>[Vy över arbetsytor](#tab/workspaces-view)

1. Logga in på [instrumentpanelen i Partnercenter](https://partner.microsoft.com/dashboard).

2. Välj **panelen** Kunder och välj sedan kunden i listan.

3. I kundmenyn väljer du **Prenumerationer.**

4. Välj prenumerationen i listan.

5. Välj **Uppdatera** för att ändra återförsäljarens (MPN-ID).

#### <a name="current-view"></a>[Aktuell vy](#tab/current-view)

1. Logga in på [instrumentpanelen i Partnercenter](https://partner.microsoft.com/dashboard).

2. I menyn i Partnercenter väljer du **Kunder.**

3. Välj kunden i listan.

4. I kundmenyn väljer du **Prenumerationer.**

5. Välj prenumerationen i listan.

6. Välj **Uppdatera** för att ändra återförsäljarens (MPN-ID).

* * *

## <a name="next-steps"></a>Nästa steg

- [Så här läser du fakturan & rekognoseringsfilen](read-your-bill.md)