---
title: Förstå faktureringsfakturor för Partnercenter
ms.topic: article
ms.date: 05/18/2020
description: Förstå fälten i din fakturafil för fakturering i Partnercenter. Här ingår fält och definitioner för alla fakturafält och avgiftsfält för en gång.
author: sodeb
ms.service: partner-dashboard
ms.subservice: partnercenter-billing
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: c741caa6993a5da415d3a94d541bf10c21470889
ms.sourcegitcommit: ad1af627f5ee6b6e3a70655f90927e932cf4c985
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 07/29/2021
ms.locfileid: "114840084"
---
# <a name="understand-partner-center-billing-invoice-fields"></a>Förstå faktureringsfakturafälten i Partnercenter

**Lämpliga roller:** Global | Administratörsbehörighet för användarhantering | Faktureringsadministratörskonto | Supportagent

Du kan använda följande tabeller för att förstå fälten i partnercentrets fakturafiler.

## <a name="invoice-file-fields"></a>Fält för fakturafil

Följande fält visas i dina fakturafiler.

| Field | Definition |
| ----- | ---------- |
| US FEIN | Ditt FEIN (Federal Employer Identification Number). Det här är USA skatteidentifierare. |
| Kundnummer | Ditt kundnummer. |
| Fakturera till | Adressen där vi skickar din faktura. Du kan ändra företagets namn och adress i faktureringsprofilen för Partnercenter. |
| Licensbaserade avgifter | De fasta månads- eller årsavgifterna för dina köpta användningsbaserade licenser debiteras i förväg för tjänsten. Det här numret är summan av alla avgifter i **kolumnen Delsumma** (kolumn **T**) i din licensbaserade avstämningsfil. |
| Användningsbaserade avgifter | Din Azure-användning. Detta inkluderar nya tjänster eller program som har aktiverats och används under faktureringsperioden. Det här numret är summan av alla avgifter i **kolumnen PretaxCharges** (kolumn **Z)** i din användningsbaserade avstämningsfil. |
| Rabatter | Rabatten som kunden får från prenumerationens normala pris. Det här numret visas som ett *fast belopp*, inte som ett pris per enhet eller licens. |
| Krediter | Krediter eller justeringar för ändringar som görs i prenumerationer (till exempel licensökningar eller minskningar). |
| Delsumma | Totalsumma före skatter och skatte-exklusiva avgifter och krediter. |
| Skatt | Den totala momsen för dina aktuella avgifter, enligt summan i avsnittet **Information** som börjar på sidan 2 på fakturan. Det här numret är summan av alla avgifter i **Kolumnen TaxAmount** (kolumn  **AA)** i din användningsbaserade avstämningsfil och kolumnen Skatt (kolumn **U)** i din licensbaserade avstämningsfil. |
| Andra krediter | Skatte exklusiv kredit. |
| Totalt antal aktuella avgifter | Det belopp som ska betalas i faktureringsvalutan för faktureringsperioden. Dessa avgifter förfaller efter betalningens förfallodatum. |
| Betalningsanvisningar | Beskrivning av hur du betalar din faktura, baserat på din region. *Se alltid till att inkludera ditt fakturanummer när du gör en betalning.* |
| Faktura nej | Numret på din faktura. |
| Faktureringsperiod | Den månadsperiod som leder fram till fakturadatumet. Det här är den period då användningsbaserade tjänster förbrukas och licensbaserade tjänster stäms av för eventuella kreditjusteringar eller ändringar i licensantalet. |
| Fakturadatum | Faktureringsdatum eller årsdag då fakturan genereras varje månad. |
| Betalningsvillkor | Betalningsvillkoret. För ett enda köp är detta alltid 60 dagar. |
| Förfallodatum för betalning | Det datum då betalningen måste tas emot. |
| Kund-IO | Din inköpsordernummer. |
| Kundtjänst | Den webbplatsadress där du kan komma åt kundtjänst. |
| Tjänstmottagare | Den adress där tjänsten används. (Det här är den juridiska företagsadress som är associerad med företagets granskning.) |

## <a name="one-time-charges-fields"></a>Fält för one-time-avgifter

Följande fält gäller endast för **one-time-avgifter** i Partnercenter:

| Field | Definition |
| ----- | ---------- |
| Datum | Inköpsdatum. |
| Beskrivning | Produktnamn. |
| Kvantitet | Antalet köpta produkter (till exempel reservationer). |
| Enhetspris | Pris per produkt (till exempel en reservation). |
| Rabatter | Alla tillämpliga rabatter. |
| Belopp före skatt | Delsummor för inköp före skatter. |
| Moms | Skattebelopp. |
| Totalt | Totalt belopp som ska betalas. |
