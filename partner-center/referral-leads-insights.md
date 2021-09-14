---
title: Analysera dina leads
ms.topic: article
ms.date: 06/15/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-referrals
description: Lär dig hur du använder sidan leadsinsikter för att se hur väl du fångar upp dina målkunders uppmärksamhet och genererar hänvisningar.
author: vikrambmsft
ms.author: vikramb
ms.localizationpriority: medium
ms.custom: SEOJUNE.20
ms.openlocfilehash: 55e502895b63e1c1a7e41f3d316355bedd7f7001
ms.sourcegitcommit: 37eac16c4339cb97831eb2a86d156c45bdf6a531
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/13/2021
ms.locfileid: "126249115"
---
# <a name="analyze-your-leads---see-how-well-you-attract-target-customers-and-potential-referrals"></a>Analysera dina leads – se hur bra du är på att locka kunder och potentiella referenser
<!-- 
https://go.microsoft.com/fwlink/?linkid=849120
-->

**Lämpliga roller:** Referensadministratör

På **sidan** Leads under **avsnittet Analys** i Referenser kan du se hur dina hänvisningar fungerar. Granska dessa mått regelbundet för att identifiera trender eller områden som behöver åtgärder och börja arbeta mot dina affärsmål.

Om du vill se dina insikter om leads går du till Menyn i Partnercenter **och går till Referenser > Analysera > Leads.**

## <a name="apply-filters"></a>Använda filter

Längst upp på sidan **Leads** kan du välja den tidsperiod som du vill visa data för. Standardvalet är **3 miljoner** (tre månader), men du kan välja att visa data under en period på sex månader eller ett år i stället. Du kan också välja **Anpassad** om du vill visa data för alla hänvisningar under en viss tidsperiod.

Du kan klicka på knappen Filter för att öppna panelen där du kan filtrera alla data på den här sidan efter Kundnamn, Land, Avtalstyp, Avtalsriktning, Lösningsnamn och Status. Nedan visas information om dessa filter.

- **Kundnamn:** Standardvärdet är **Alla,** men du kan begränsa data till en eller flera kunder som du väljer.
- **Land:** Standardvärdet är **Alla,** men du kan begränsa data till ett eller flera länder av kunden som du väljer.
- **Hänvisningsprogram:** Standardvärdet är **Alla,** men du kan begränsa data till ett specifikt hänvisningsprogram. Det här filtret visas bara om din organisation är registrerad i hänvisningsprogrammet.
- **Status:** Standardvärdet är **Alla**, men du kan välja att begränsa data till hänvisningar som innehåller en eller flera typer av hänvisningsstatus, t.ex. accepterade, avvisade, utgångna, förlorade och vann som du väljer.
- **Kvalificeringstyp:** Standardvärdet är **Alla**, men du kan välja att begränsa data till hänvisningar som antingen är marketplace-leads eller kvalificerade leads.

Informationen i alla diagram som anges nedan återspeglar datumintervallet och eventuella filter som du har valt, förutom vad som anges nedan. I vissa avsnitt kan du också använda ytterligare filter, till exempel filtrering för en specifik lösning.

## <a name="referrals-summary"></a>Sammanfattning av hänvisningar

Det här kortet visar en översikt över hur dina leads presterar.

Diagrammet visar det totala antalet sidbesök, antalet anrop till åtgärd-knappen (kontaktpartner), antalet leads som genererats efter att kunderna klickat på anropet till åtgärden och totalt antal leads som vunnits under den valda tidsperioden.

Måtten för procentuell ändring (visas i rött eller grönt med  en pilindikator) anger skillnaden mellan den senaste fullständiga månaden i det valda datumintervallet och den första fullständiga månaden i **intervallet**. Säg till exempel att det aktuella datumet är 15 juni och att du har valt **3M-filtret** för att visa data för de senaste tre månaderna. I det här fallet skulle de här måtten visa skillnaden mellan maj (den sista fullständiga månaden under den valda tidsperioden) och mars (den första fullständiga månaden under den valda tidsperioden) det valda datumintervallet är senaste **3** miljoner , jämförelsen skulle vara mellan data för maj och data för mars.

:::image type="content" source="images/referrals/leadsanalyticssummary.png" alt-text="Bild som visar sammanfattningskortet för leadsanalys.":::

## <a name="conversion-funnel"></a>Konverteringstratt

Det här avsnittet visar en visuell indikator på hur dina avtal flyttas från ett tillstånd till ett annat genom livscykeln. Du kan visa hela livscykeln baserat på avtalsvolymen samt avtalsvärdet i USD baserat på huvud pivoten för det här avsnittet. Det första avsnittet är märkt med typen av avtal så att du får en visuell indikator på volymen eller värdet efter typ. Det finns också ett avsnitt, **Leads** från tidigare , som används för att ange de avtal som du har vidtagit åtgärder för att antingen acceptera/avböja dem eller markera dem som won/lost under den tidsperiod som har valts för rapporten. Du kan använda filter för att visa förloppet för avtal i olika faser i livscykeln.

:::image type="content" source="images/referrals/leadsanalyticsfunnel.png" alt-text="Bild som visar konverteringstratten för hänvisningar.":::

## <a name="leads-by-geography"></a>Leads efter geografiskt område

Det här avsnittet visar de länder/regioner där avtal kom från, tillsammans med information om varje land/region. Det finns en tabellvy över avtalsinformationen för varje land tillsammans med en kartvy över alla länder. Du kan klicka på ett visst land i tabellen eller klicka på kartvyn för att zooma till ett visst land.

:::image type="content" source="images/referrals/leadsanalyticsgeodistribution.png" alt-text="Bild som visar geofördelningen av hänvisningar.":::

## <a name="leads-by-program"></a>Leads efter program

Med den här kombinationen av tabeller och diagram kan du se vilka av dina hänvisningsprograms leads som driver flest hänvisningar och det högsta avtalsvärdet.
Tabellen innehåller totalt antal leads, de leads som har accepterats med i serviceavtalet (24 timmar) i både procent och absoluta termer, de leads som har upphört att gälla och de leads som gick in i ett won-tillstånd tillsammans med det totala antalet leads som vunnits i USD-valuta. Det finns också ett trenddiagram för leads till höger om tabellen som visar det totala antalet avtal och det avtalsvärde som vunnits i USD-valutan baserat på det program som valts. Standardvalet är alla lösningar.

:::image type="content" source="images/referrals/leadsanalyticsreferralsprogram.png" alt-text="Bild som visar prestanda för kvalificerade hänvisningsprograms leads.":::

## <a name="declined--lost-reasons"></a>Nekade & förlorade orsaker

Det här avsnittet hjälper dig att analysera orsakerna till varför leads markeras som **nekade** **eller förlorade** av ditt företag. Alternativen i dessa representationer är samma orsaker som säljarna har valt när de stänger leaden som nekad eller förlorad.

:::image type="content" source="images/referrals/leadsanalyticsreasons.png" alt-text="Bild som visar orsakerna som valts av partnern vid avböjning eller tagande av ett lead som förlorat.":::

## <a name="comparison-charts"></a>Jämförelsediagram

Jämförelseavsnittet hjälper dig att jämföra data relaterade till leads baserat på flera dimensioner både på volymen och det leads som vann värdet i USD-pivot.
De tre dimensioner som du kan välja för att jämföra data är

- Kvalificeringstyp
- Marknader
- Hänvisningsprogram

När kvalificeringstyp har valts kan du jämföra referensprestandan för med avseende på marketplace-leads och kvalificerade leads. För både marknader och hänvisningsprogram kan du välja mellan tre olika alternativ för att jämföra deras prestanda. Det första diagrammet, som är ett stapeldiagram, har data som visas med en månadstrend baserat på huvud pivoten, som är volym eller det avtalsvärde som vunnits. Det finns också ett cirkeldiagram till höger om stapeldiagrammet, som visar fördelningen efter procentandel för samma data.

:::image type="content" source="images/referrals/leadsanalyticscompare.png" alt-text="Bild som visar jämförelseavsnittet.":::

## <a name="raw-data-table"></a>Rådatatabell

Tabellen nedan med alla rådata som är relaterade  till leads hjälper dig att snabbt exportera data för alla detaljerade eller anpassade analyser som du vill utföra.

:::image type="content" source="images/referrals/leadsanalyticsrawdata.png" alt-text="Bild som visar rådatatabellen för leads.":::

## <a name="no-data"></a>Inga data

Det kan finnas flera orsaker till varför du får ett tomt diagram som nedan när du använder leadsanalysen enligt beskrivningen nedan.

- Det finns inga data för det här kontot. Prova att skapa avtal för att få rapporten ifylld.
- Det finns ett problem med nätverksanslutningen. Kontrollera internetanslutningen och försök igen.
- Det finns inga poster som matchar de filter som du har tillämpat. Försök att återställa filtren.
- Det finns en fördröjning mellan ändringen av leadtillståndet och för att det ska uppdateras i analysrapporten. Kontrollera rapporten efter 24 timmar.

:::image type="content" source="images/referrals/nodata.png" alt-text="Bild som visar ingen datavisualisering för leads.":::

> [!TIP]
> Om du vill se hur dina möjligheter till säljförsäljning fungerar kan du gå till sidan insikter [om möjligheter till säljförsäljning.](referral-insights.md)

## <a name="next-steps"></a>Nästa steg

- [Hantera leads](manage-leads.md)
