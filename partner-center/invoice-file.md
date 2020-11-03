---
title: Förstå fakturerings fakturor för partner Center
ms.topic: article
ms.date: 05/18/2020
description: Förstå fälten i faktura filen för fakturering i Partner Center. information omfattar fält och definitioner för alla faktura fält och en engångs avgift.
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 121b0bc756e715af358eda30eff92cba35e802ed
ms.sourcegitcommit: 22af0997d52a87417b62f44fb0a7d711bec77b35
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 10/19/2020
ms.locfileid: "92532113"
---
# <a name="understand-partner-center-billing-invoice-fields"></a>Förstå fakturerings faktura fält i Partner Center

**Lämpliga roller**

- Global administratör
- Användaradministratör
- Faktureringsadministratör
- Support agent

Du kan använda följande tabeller för att förstå fälten i filer för partner Center-fakturor.

## <a name="invoice-file-fields"></a>Fält för faktura fil

Följande fält visas på dina faktura filer.

| Field | Definition |
| ----- | ---------- |
| US FEIN | Ditt federala arbetsgivares identifierings nummer (FEIN). Detta är ditt USA Federal Tax Identifier-nummer. |
| Kund nummer | Ditt kund nummer. |
| Fakturera till | Adressen dit vi skickar din faktura. Du kan ändra företagets namn och/eller adress i din fakturerings profil för partner Center. |
| Licensbaserade avgifter | De fasta månatliga eller årliga avgifterna för dina köpta användnings licenser, faktureras i förväg för tjänsten. Det här talet är summan av alla kostnader i kolumnen **delsumma** (kolumn **T** ) i din licensbaserade avstämnings fil. |
| Användnings avgifter | Din Azure-användning. Detta omfattar nya tjänster eller program som är aktiverade och används under fakturerings perioden. Det här talet är summan av alla kostnader i kolumnen **PretaxCharges** (kolumn **Z** ) i din användnings-baserade avstämnings fil. |
| Rabatter | Den rabatt som kunden får från prenumerationens normala pris. Det här antalet visas som ett *fast belopp* , inte som ett pris per enhet eller licens. |
| Krediter | Krediter eller justeringar av ändringar som gjorts i prenumerationer (till exempel licens ökningar eller minskningar). |
| Delsumma | Totalt före skatt och skatte exklusiva kostnader och krediter. |
| Skatt | Den totala momsen för dina aktuella kostnader, totalt i avsnittet **information** som börjar på sidan 2 i din faktura. Det här talet är summan av alla kostnader i kolumnen **TaxAmount** (kolumn **AA** ) i din användnings-baserade avstämnings fil och kolumnen **skatt** (kolumn **U** ) i din licensbaserade avstämnings fil. |
| Andra krediter | Skatte exklusiva krediter. |
| Totalt antal aktuella avgifter | Det belopp som förfaller i fakturerings valutan för fakturerings perioden. Dessa avgifter förfaller efter förfallo datumet för betalning. |
| Betalningsanvisningar | Beskrivning av hur du betalar din faktura baserat på din region. *Var alltid noga med att inkludera ditt faktura nummer när du gör en betalning.* |
| Faktura nr | Numret på din faktura. |
| Faktureringsperiod | Månads perioden som leder fram till fakturerings datumet. Detta är den period under vilken användnings tjänster förbrukas och licensbaserade tjänster stäms av för eventuella kredit justeringar eller ändringar i licens antalet. |
| Fakturadatum | Det fakturerings datum eller den jubileums dag då din faktura genereras varje månad. |
| Betalningsvillkor | Betalnings villkoret. För en engångs inköp är detta alltid 60 dagar. |
| Förfallo datum för betalning | Datumet då din betalning måste tas emot. |
| Kund inköps order | Din inköps nummer ordning. |
| Kundtjänst | Webbplats adressen där du kan komma åt kund tjänsten. |
| Tjänst mottagare | Adressen där tjänsten används. (Detta är den juridiska företags adressen som är kopplad till företagets först konsumentsajter.) |

## <a name="one-time-charges-fields"></a>Fält för engångs kostnad

Följande fält gäller endast för **engångs kostnader** i Partner Center:

| Field | Definition |
| ----- | ---------- |
| Datum | Inköps datum. |
| Beskrivning | Produkt namn. |
| Kvantitet | Antalet produkter (till exempel reservationer) som köpts. |
| Enhetspris | Pris per produkt (till exempel en reservation). |
| Rabatter | Alla tillämpliga rabatter. |
| Belopp före skatt | Del summan av inköpen före skatt. |
| Moms | Skatte belopp. |
| Totalt | Totalt belopp som ska betalas. |
