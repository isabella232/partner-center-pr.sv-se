---
title: Förstå faktureringsfakturor i Partnercenter
ms.topic: article
ms.date: 05/18/2020
description: Förstå fälten i din fakturafil för Fakturering i Partnercenter. Fälten och definitionerna för alla fakturafält och entidsdefaktfält ingår.
author: sodeb
ms.service: partner-dashboard
ms.subservice: partnercenter-billing
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: c741caa6993a5da415d3a94d541bf10c21470889
ms.sourcegitcommit: 1161d5bcb345e368348c535a7211f0d353c5a471
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/09/2021
ms.locfileid: "123961056"
---
# <a name="understand-partner-center-billing-invoice-fields"></a>Förstå faktureringsfakturafält i Partnercenter

**Lämpliga roller:** Globala | Administratörsbehörighet för | Faktureringsadministratörskonto | Supportagent

Du kan använda följande tabeller för att förstå fälten i partnercentrets fakturafiler.

## <a name="invoice-file-fields"></a>Fält för fakturafil

Följande fält visas i dina fakturafiler.

| Field | Definition |
| ----- | ---------- |
| US FEIN | Ditt FEIN (Federal Employer Identification Number). Det här är USA nummer för federal skatteidentifierare. |
| Kundnummer | Ditt kundnummer. |
| Fakturera till | Adressen där vi skickar din faktura. Du kan ändra företagets namn och adress i faktureringsprofilen för Partnercenter. |
| Licensbaserade avgifter | De fasta månatliga eller årliga avgifterna för dina köpta användningsbaserade licenser som debiteras i förväg för tjänsten. Det här talet är summan av alla avgifter i **kolumnen Delsumma** (kolumn **T**) i din licensbaserade avstämningsfil. |
| Användningsbaserade avgifter | Din Azure-användning. Detta inkluderar nya tjänster eller program som är aktiverade och används under faktureringsperioden. Det här numret är summan av alla avgifter i **kolumnen PretaxCharges** (kolumn **Z)** i din användningsbaserade avstämningsfil. |
| Rabatter | Rabatten som kunden får från prenumerationens normala pris. Det här talet visas som ett *fast belopp*, inte som ett pris per enhet eller licens. |
| Krediter | Krediter eller justeringar för ändringar som görs i prenumerationer (till exempel licensökningar eller minskningar). |
| Delsumma | Totalsumma före skatter och skatte-exklusiva avgifter och krediter. |
| Skatt | Den totala momsen för dina aktuella avgifter, enligt summan i **avsnittet** Information som börjar på sidan 2 på fakturan. Det här numret är summan av alla avgifter i **Kolumnen TaxAmount** (kolumn **AA)** i din användningsbaserade avstämningsfil och kolumnen **Skatt** (kolumn **U)** i din licensbaserade avstämningsfil. |
| Andra krediter | Skatte- och exklusiv kredit. |
| Totalt antal aktuella avgifter | Det belopp som förfaller i faktureringsvalutan för faktureringsperioden. Dessa avgifter förfaller efter betalningens förfallodatum. |
| Betalningsanvisningar | Beskrivning av hur du betalar din faktura, baserat på din region. *Se alltid till att inkludera ditt fakturanummer när du gör en betalning.* |
| Fakturanr | Numret på din faktura. |
| Faktureringsperiod | Den månatliga perioden fram till fakturadatumet. Det här är den period då användningsbaserade tjänster förbrukas och licensbaserade tjänster stäms av för eventuella kreditjusteringar eller ändringar i licensantalet. |
| Fakturadatum | Faktureringsdatum eller årsdag då din faktura genereras varje månad. |
| Betalningsvillkor | Betalningsvillkoret. För ett köp är detta alltid 60 dagar. |
| Förfallodatum för betalning | Det datum då betalningen måste tas emot. |
| Kund-IO | Din inköpsorder. |
| Kundtjänst | Den webbplatsadress där du kan komma åt kundtjänst. |
| Tjänstmottagare | Adressen där tjänsten används. (Det här är den juridiska företagsadress som är associerad med företagets granskning.) |

## <a name="one-time-charges-fields"></a>Fält för one-time-avgifter

Följande fält gäller endast för **en-gång-avgifter** i Partnercenter:

| Field | Definition |
| ----- | ---------- |
| Datum | Inköpsdatum. |
| Description | Produktnamn. |
| Kvantitet | Antal produkter (till exempel reservationer) som köpts. |
| Enhetspris | Pris per produkt (till exempel en reservation). |
| Rabatter | Eventuella rabatter. |
| Belopp före skatt | Delsummor av inköp före skatter. |
| Moms | Skattebelopp. |
| Totalt | Totalt belopp som ska betalas. |
