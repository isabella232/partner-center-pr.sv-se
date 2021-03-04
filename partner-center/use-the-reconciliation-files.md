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
ms.openlocfilehash: d927b138c32b3e5f6f5d906db898e17f89a85aae
ms.sourcegitcommit: bff907bdbddc769716c7418a2b4a94ca37c2d590
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/03/2021
ms.locfileid: "101755770"
---
# <a name="learn-how-to-read-the-line-items-in-your-partner-center-reconciliation-files"></a>Lär dig hur du läser rad objekt i dina avstämnings filer för partner Center

Gäller för:

- Partnercenter
- Välkommen till Partnercenter för Microsoft Cloud for US Government

**Lämpliga roller**

- Faktureringsadministratör
- Global administratör

Du kan ladda ned dina avstämnings filer från Partner Center för en detaljerad, rad objekt visning av varje debitering i en fakturerings period. Information om rad objekt inkluderar avgifter för varje kunds prenumerationer och detaljerade händelser (till exempel ett omslags kort tillägg av licenser till en prenumeration).

Information om hur du läser fakturan finns i [läsa din](read-your-bill.md) **faktura**.

## <a name="understand-reconciliation-file-fields"></a>Förstå fält för avstämnings fil

- [Fält för licensbaserad avstämningsfil](license-based-recon-files.md)
- [Fält för användningsbaserad avstämningsfil](usage-based-recon-files.md)
- [Fält i fil för dagligt beräknad användningsavstämning](daily-rated-usage-recon-files.md)
- [Fil fält för CSP-avstämning för inköp vid ett tillfälle](modern-invoice-reconciliation-file.md)

## <a name="understand-charge-types-in-reconciliation-files"></a>Förstå debiterings typer i avstämnings filer

Information om vilka typer av kostnader som finns i avstämnings filer (kolumnen **ChargeType** ) finns i [fil avgifts typer för avstämning](recon-file-charge-types.md).

## <a name="fix-formatting-issues"></a>Åtgärda problem med formatering

Ibland kan en avstämnings fil innehålla formateringsfel. Det här problemet kan till exempel inträffa om en-US locale inte används.

Följ dessa steg för att åtgärda eventuella formateringsfel i dina avstämnings filer:

1. Öppna avstämnings filen (i CSV-format) i Microsoft Excel.
2. Markera den första kolumnen i filen.
3. Öppna **guiden Omvandla text till kolumner**. Välj **data** i menyfliksområdet och välj sedan **text till kolumner**.
4. Välj **avgränsad filtyp** i guiden. Välj **Nästa**.
5. I fältet **avgränsare** väljer du **kommatecken**. (Om **fliken** redan har valts kan du lämna det här alternativet markerat.) Välj sedan **Nästa**.
6. I fältet **kolumn data format** väljer du **datum: MDÅ**. Välj **Nästa**.
7. I fältet **kolumn data format** väljer du **text** för alla belopps kolumner. Välj sedan **Slutför**.

## <a name="download-reconciliation-files-programmatically"></a>Ladda ned filer för avstämning program mässigt

Avstämnings filer kan vara mycket stora och är ibland svåra att ladda ned. Information om hur du hämtar avstämnings filer program mässigt finns i [Hämta faktura rads objekt](/partner-center/develop/get-invoiceline-items).

## <a name="map-taxes-or-vat"></a>Mappa skatter eller moms

Så här mappar du skatter eller mervärdes skatt (moms) till din faktura:

- Summera **moms** kolumnen från den licensbaserade filen.
- Summera kolumnen **TaxAmount** från den Usage-baserade filen.

## <a name="itemize-reconciliation-files-by-partner"></a>Specificera avstämnings filer efter partner

Partner i den **indirekta modellen** kan använda dessa ytterligare fält i både licensbaserade och användnings bara avstämnings filer för att specificera filerna efter åter försäljare.

| MPN-ID | Beskrivning |
| ------ | ----------- |
| MPN-ID | Microsoft Partner Network-ID (MPN) för Cloud Solution Provider (CSP)-partner (direkt eller indirekt). |
| [MPN-ID för åter försäljare](#reseller-mpn-id) | [MPN identifierare för åter försäljaren av posten för prenumerationen](#reseller-mpn-id). Det här fältet motsvarar det åter försäljar-ID som anges för den aktuella prenumerationen i Partner Center. Visas endast i avstämnings filer för partner i den indirekta modellen. |

### <a name="reseller-mpn-id"></a>MPN-ID för åter försäljare

Om en CSP-partner sålde prenumerationen direkt till kunden visas deras **MPN-ID** två gånger, som både **MPN-ID** och **åter försäljarens MPN-ID**.

Om en CSP-partner har en åter försäljare utan **MPN-ID** är det här värdet inställt på partnerns **MPN-ID** i stället.

Om CSP-partnern tar bort ett **MPN-ID för åter försäljaren** anges värdet *-1*.

Visa eller uppdatera **MPN-ID: t för åter försäljaren**:

1. Logga in på Partner Center.
2. I menyn Partner Center väljer du **kunder**.
3. Välj kund i listan.
4. I menyn kund väljer du **prenumerationer**.
5. Välj prenumerationen i listan.
6. Välj **Uppdatera** för att ändra **åter försäljaren (MPN-ID)**.

## <a name="next-steps"></a>Nästa steg

- [Så här läser du rekognoseringar-filen för Bill &](read-your-bill.md) 