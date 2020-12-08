---
title: Analysera dina leads
ms.topic: article
ms.date: 06/15/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Lär dig hur du använder sidan för leads-insikter för att se hur väl du fångar uppmärksamheten hos dina mål kunder och att skapa hänvisningar.
author: vikrambmsft
ms.author: vikramb
ms.localizationpriority: medium
ms.custom: SEOJUNE.20
ms.openlocfilehash: c3ca88d367ea9dea8df1bb2bb4945ecc7b900b26
ms.sourcegitcommit: 351c7ff4e6ebbb615a00190b2310156381f9cf03
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 12/07/2020
ms.locfileid: "96776859"
---
# <a name="analyze-your-leads---see-how-well-you-attract-target-customers-and-potential-referrals"></a>Analysera dina leads – se hur bra du får mål kunder och potentiella referenser
<!-- 
https://go.microsoft.com/fwlink/?linkid=849120
-->

**Lämpliga roller**

- Referens administratör

**Gäller för**

- Marketplace-leads
- Kvalificerade leads

På sidan **leads** i avsnittet **analys** i hänvisningar kan du se hur dina referenser fungerar. Granska dessa mått regelbundet för att identifiera trender eller områden som behöver åtgärdas och börja rikta mot dina affärs mål.

Om du vill se dina leads Insights-data går du till avsnittet Partner Center och går till **referenser > analysera > leads**.

## <a name="apply-filters"></a>Använda filter

Längst upp på sidan **leads** kan du välja den tids period som du vill visa data för. Standard valet är **3m** (tre månader), men du kan välja att visa data för en period på sex månader eller ett år i stället. Du kan också välja **anpassad** om du vill se data för alla referenser under en viss tids period.

Du kan klicka på knappen filter för att öppna panelen där du kan filtrera alla data på den här sidan med kund namn, land, avtals typ, avtals riktning, lösnings namn och status. Nedan visas information om dessa filter.

- **Kund namn**: standardvärdet är **alla**, men du kan begränsa data till en eller flera kunder som du väljer.
- **Land**: standardvärdet är **alla**, men du kan begränsa data till ett eller flera länder för kunden som du väljer.
- **Hänvisnings program**: standardvärdet är **alla**, men du kan begränsa data till ett angivet hänvisnings program. Det här filtret visas bara om din organisation är registrerad i referral program.
- **Status**: standardvärdet är **alla**, men du kan välja att begränsa data till referenser som innehåller en eller flera hänvisnings status typer som accepterade, nekade, förfallna, förlorade och uppnådda som du väljer.
- **Kvalificerings typ**: standardvärdet är **alla**, men du kan välja att begränsa data till referenser som antingen leder till marknads platser eller kvalificerade leads.

Informationen i alla diagram som visas nedan visar datum intervallet och eventuella filter som du har valt, förutom vad som anges nedan. I vissa avsnitt kan du också använda ytterligare filter, till exempel filtrera till en viss lösning.

## <a name="referrals-summary"></a>Sammanfattning av referenser

Det här kortet visar en översikt över hur dina leads presterar.

Diagrammet visar det totala antalet sid besök, antalet samtal till Åtgärds knappen (kontakt partner) klickar på, antalet leads som skapats efter att kunderna klickade på åtgärden för att utföra åtgärden och totalt antal vunna leads för den valda tids perioden.

Procent måtten för ändring (som visas i rött eller grönt, med en pil-indikator) visar skillnaden mellan den **senaste fullständiga månaden i det valda datum intervallet** och den **första fullständiga månaden i intervallet**. Anta till exempel att det aktuella datumet är 15 juni och att du har valt **3m** -filtret för att visa data för de senaste tre månaderna. I det här fallet skulle dessa mått Visa skillnaden mellan maj (den senaste fullständiga månaden för den valda tids perioden) och mars (den första fullständiga månaden för den valda tids perioden) det datum intervall som valts är sista **3m**, jämförelsen skulle vara mellan data för maj och data för mars.

:::image type="content" source="images/referrals/leadsanalyticssummary.png" alt-text="Bild som visar sammanfattnings kortet för leads Analytics.":::

## <a name="conversion-funnel"></a>Omvandlings tratt

Det här avsnittet visar en visuell indikator för hur dina avtal flyttas från ett tillstånd till ett annat via deras livs cykel. Du kan visa hela livs cykeln baserat på den avtalade volymen samt det avtalade värdet i USD baserat på det huvudsakliga Pivot-området för det här avsnittet. Det första avsnittet är märkt med typen av avtal för att ge dig en visuell indikator för volymen eller värdet efter typ. Det finns också ett avsnitt som förbrukas **tidigare**, som används för att ange vilka avtal som du har vidtagit för att acceptera/avböja dem eller markera dem som vunna/förlorade under den tids period som har valts för rapporten. Du kan använda filter för att visa förloppet för de olika stegen i deras livs cykel.

:::image type="content" source="images/referrals/leadsanalyticsfunnel.png" alt-text="Bild som visar omvandlings tratten för referenser.":::

## <a name="leads-by-geography"></a>Leads efter geografi

I det här avsnittet visas de länder/regioner där avtal kom från, tillsammans med information för varje land/region. Det finns en tabellvy över avtals detaljerna för varje land, tillsammans med en karta över alla länder. Du kan klicka på ett särskilt land i tabellen eller klicka på vyn karta för att zooma till ett särskilt land.

:::image type="content" source="images/referrals/leadsanalyticsgeodistribution.png" alt-text="Bild som visar geo-distributionen av hänvisningar.":::

## <a name="leads-by-program"></a>Leads efter program

Med den här kombinationen av tabell och diagram kan du se vilken av dina antecknings program som leads kör flest hänvisningar och det högsta värdet.
Tabellen har sammanlagt antal leads, leads som har accepterats med i SLA (24 timmar) i både procent och absoluta villkor, de leads som har upphört att gälla och de leads som gick i uppnådd status tillsammans med det totala värdet för leads som vunnits i USD-valutan. Det finns också ett trend diagram för leads till höger om tabellen som visar de totala antalet avtal och det avtalade värdet i USD-valutan baserat på det program som har valts. Standard valet är alla lösningar.

:::image type="content" source="images/referrals/leadsanalyticsreferralsprogram.png" alt-text="Bild som visar det kvalificerade programmet för hänvisnings program leder till prestanda.":::

## <a name="declined--lost-reasons"></a>Nekade & förlorade orsaker

Det här avsnittet hjälper dig att analysera orsakerna till att leads markeras som **avböjd** eller **förlorad** av ditt företag. Alternativen i dessa representationer är av samma skäl som att säljarna har valt när de stänger leadet som nekat eller förlorat.

:::image type="content" source="images/referrals/leadsanalyticsreasons.png" alt-text="Bild som visar de orsaker som valts av partnern när du avböjer eller gör ett lead som förlorat.":::

## <a name="comparison-charts"></a>Jämförelse diagram

Jämförelse avsnittet hjälper dig att jämföra data som är relaterade till leads baserat på flera dimensioner på volymen och värdet för leads vann i USD Pivot.
De tre dimensionerna som du kan välja för att jämföra data är

- Kvalificerings typ
- Marknaden
- Hänvisnings program

När du väljer kvalificerings typ har du möjlighet att jämföra hänvisnings prestandan för med avseende på Marketplace-leads och kvalificerade leads. För både marknader och referral program kan du hämta upp till tre olika alternativ för att jämföra deras prestanda. Det första diagrammet, som är ett stapeldiagram, kommer att ha data som visas i månaden på månads trend, baserat på huvud Pivot, som är volym eller uppnådda avtals värde. Det finns också ett cirkel diagram till höger om stapeldiagrammet, som visar fördelningen i procent för samma data.

:::image type="content" source="images/referrals/leadsanalyticscompare.png" alt-text="Bild som visar jämförelse avsnittet.":::

## <a name="raw-data-table"></a>Rå data tabell

Tabellen nedan med alla rå data som är relaterade till leads hjälper dig att snabbt **Exportera** data för en detaljerad eller anpassad analys som du vill utföra.

:::image type="content" source="images/referrals/leadsanalyticsrawdata.png" alt-text="Bild som visar rå data tabellen för leads.":::

## <a name="no-data"></a>Inga data

Det kan finnas flera orsaker till att du får ett tomt diagram som nedan när du öppnar leads Analytics enligt beskrivningen nedan.

- Det finns inga data för det här kontot. Försök att skapa avtal för att få den här rapporten ifylld.
- Det finns ett problem med nätverks anslutningen. Kontrol lera din Internet anslutning och försök igen.
- Det finns inga poster som matchar de filter som du har använt. Försök att återställa filtren.
- Det uppstår en fördröjning mellan ändringen av lead-tillstånd och för samma som ska uppdateras i analys rapporten. Kontrol lera rapporten efter 24 timmar.

:::image type="content" source="images/referrals/nodata.png" alt-text="Bild som visar inga data visualiseringar för leads.":::

> [!TIP]
> Om du vill se hur dina samförsäljnings möjligheter fungerar går du till [sidan för affärs möjligheter för samförsäljning](referral-insights.md).
