---
title: Hämta insikter om hänvisningar
ms.topic: article
ms.date: 04/30/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-referrals
description: Granska dina hänvisningsinformationsdata regelbundet i Partnercenter för att se trender för att åtgärda eller förbättra områden som hjälper dig att nå dina affärsmål.
author: rajap-ms
ms.author: rajap
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 8886831228807c48bd3666daa485ac5357c8c6e2
ms.sourcegitcommit: 1161d5bcb345e368348c535a7211f0d353c5a471
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/09/2021
ms.locfileid: "123960716"
---
# <a name="get-referral-insights-in-partner-center-and-find-out-how-your-referrals-are-doing"></a>Få referensinsikter i Partnercenter och ta reda på hur dina hänvisningar fungerar

**Lämpliga roller:** Referensadministratör

På **sidan Möjligheter till säljförsäljning** under avsnittet **Analys** i Referenser kan du se hur dina hänvisningar fungerar. Granska dessa mått regelbundet för att identifiera trender eller områden som behöver åtgärder och börja arbeta mot dina affärsmål.

Om du vill se dina insikter om möjligheter till säljförsäljning går du till Referenser i Partnercenter **> Analytics > Möjligheter till säljförsäljning.**

> [!Important]
> Filtret för avtalstyp tillämpas i förväg med typen **Säljavtal** och **Partnerledd** vald för alla data. Ta bort filtret om du vill analysera data för alla eller specifika typer av avtal.

## <a name="apply-filters"></a>Använda filter

Längst upp på sidan **Medförsäljningsmöjligheter** kan du välja den tidsperiod som du vill visa data för. Standardvalet är **3 miljoner** (tre månader), men du kan välja att visa data i sex månader eller ett år i stället. Du kan också välja **Anpassad** om du vill visa data för alla hänvisningar under en viss tidsperiod.

Du kan välja **knappen Filter** för att öppna panelen där du kan filtrera alla data på den här sidan efter Kundnamn, Land, Avtalstyp, Avtalsriktning, Lösningsnamn och Status. Nedan visas information om dessa filter.

- **Kundnamn:** Standardvärdet är **Alla,** men du kan begränsa data till en eller flera kunder som du väljer.
- **Land:** Standardvärdet är **Alla,** men du kan begränsa data till ett eller flera länder av kunden som du väljer.
- **Avtalstyp:** Standardinställningen är **Samförsäljning** och **Partnerledd,** men du kan antingen välja Alla eller begränsa data till privata avtal eller partnerledda avtal baserat på ditt val.
- **Avtalsriktning** Standardvärdet är **Alla**, men du kan  välja att begränsa data till inkommande hänvisningar (sådana som du har fått) eller **utgående** hänvisningar (sådana som du har skickat).
- **Lösningsnamn:** Standardvärdet **är Alla**, men du kan välja att begränsa data till hänvisningar som innehåller en eller flera lösningar som du väljer.
- **Status:** Standardvärdet är **Alla**, men du kan välja att begränsa data till hänvisningar som innehåller en eller flera typer av hänvisningsstatus som skapas, godkänns, nekas, har upphört att gälla, förlorats och vunnits som du väljer.

Informationen i alla diagram som anges nedan återspeglar datumintervallet och eventuella filter som du har valt, förutom vad som anges nedan. I vissa avsnitt kan du också använda extra filter, till exempel filtrering för en specifik lösning.

## <a name="referrals-summary"></a>Sammanfattning av hänvisningar

Det här kortet visar en översikt över hur det går för dina möjligheter till säljförsäljning.

Diagrammet visar det totala antalet avtal, det antal som vanns, antalet som förlorades och den totala avtalsvolymen (i USD) för den valda tidsperioden.

Måtten för procentuell ändring (visas i rött eller grönt med  en pilindikator) anger skillnaden mellan den senaste fullständiga månaden i det valda datumintervallet och den första fullständiga månaden i **intervallet**. Säg till exempel att det aktuella datumet är 15 juni och att du har valt **3M-filtret** för att visa data för de senaste tre månaderna. I det här fallet skulle de här måtten visa skillnaden mellan maj (den sista fullständiga månaden under den valda tidsperioden) och mars (den första fullständiga månaden under den valda tidsperioden) det valda datumintervallet är senaste **3** miljoner , jämförelsen skulle vara mellan data för maj och data för mars.

:::image type="content" source="images/referrals/cosellanalyticssummary.png" alt-text="Bild som visar sammanfattningskortet för analys av möjligheter till säljförsäljning.":::

## <a name="conversion-funnel"></a>Konverteringstratt

Det här avsnittet visar en visuell indikator på hur dina avtal flyttas från ett tillstånd till ett annat genom livscykeln. Du kan visa hela livscykeln baserat på avtalsvolymen och avtalsvärdet i USD baserat på huvud pivoten för det här avsnittet. Det första avsnittet är märkt både med tillståndet och typen av avtal för att ge dig en visuell indikator för volymen eller värdet efter typ. Det finns också ett **avsnitt,** Referenser från tidigare , som används för att ange de avtal som du har vidtagit åtgärder för att antingen acceptera/avböja dem eller markera dem som förlorade/förlorade under den tidsperiod som har valts för rapporten. Du kan använda filter för att visa förloppet för avtal i olika faser i livscykeln.

Inkommande avtal för sälj samförsäljning kan sammanfogas med antingen Accepterade, Avvisade eller Utgångna som partner måste antingen godkänna eller neka inkommande samförsäljningserbjudanden.

:::image type="content" source="images/referrals/inbound.png" alt-text="Bild som visar tillstånd för inkommande hänvisningar.":::

Partnerledda, privata och utgående avtal för samförsäljning sammanslås till Skapad eftersom dessa typer av avtal skapas av partner.

:::image type="content" source="images/referrals/outbound.png" alt-text="Bild som visar tillstånd för utgående hänvisningar.":::

:::image type="content" source="images/referrals/cosell-analytics-funnel-v2.png" alt-text="Bild som visar konverteringstratten för hänvisningar.":::

## <a name="deals-by-geography"></a>Avtal efter geografiskt område

Det här avsnittet visar de länder/regioner där avtal kom från, tillsammans med information om varje land/region. Det finns en tabellvy över avtalsinformationen för varje land tillsammans med en kartvy över alla länder. Du kan välja ett visst land i tabellen eller välja kartvyn för att zooma till ett visst land.

:::image type="content" source="images/referrals/cosell-analytics-geo-distribution-v2.png" alt-text="Bild som visar geofördelningen av hänvisningar.":::

## <a name="deals-by-solutions"></a>Avtal efter lösningar

I det här diagrammet kan du se vilka av dina lösningar som ger flest hänvisningar och det högsta avtalsvärdet. Tabellen har tre pivoter – Säljpartner, Partnerledd och Privat.
Baserat på ditt pivotval kan du se resultatet för de avtal som sammanställs av lösningen.

> [!NOTE]
> Om flera lösningar ingår i ett avtal visar tabellen samma avtal som räknas mot alla dessa lösningar. Du bör inte addera värdena som är relaterade till lösningar och jämföra dem med andra referensvolymmått. Den här vyn är avsedd att hjälpa dig att förstå avtalsprestanda med lösnings pivot.

Tabellen har totalt antal avtal som innehåller lösningen och motsvarande delstater som avtal som vunnits, förlorade avtal, avtal har upphört att gälla tillsammans med det totala avtalsvärdet som vunnits och förlorats i USD-valuta. Det finns också ett avtalstrenddiagram till höger om tabellen som visar det totala antalet avtal och det avtalsvärde som vunnits i USD-valutan baserat på den lösning som valts. Standardvalet är alla lösningar.

:::image type="content" source="images/referrals/cosell-analytics-solutions-v2.png" alt-text="Bild som visar lösningars prestanda.":::

## <a name="declined--lost-reasons"></a>Nekade & förlorade orsaker

Det här avsnittet hjälper dig att analysera orsakerna till att avtal markeras som **nekade** **eller förlorade** av ditt företag. Alternativen i dessa representationer är samma skäl som dina säljare har valt när de stänger avtalet som nekat eller förlorat.

:::image type="content" source="images/referrals/cosellanalyticsreasons.png" alt-text="Bild som visar orsakerna som valts av en partner när de avböjer eller gör ett avtal som förlorat.":::

## <a name="comparison-charts"></a>Jämförelsediagram

Jämförelseavsnittet hjälper dig att jämföra data relaterade till hänvisningar baserat på flera dimensioner både på volymen och det avtalsvärde som vunnits i USD-pivot. De tre dimensioner som du kan välja för att jämföra data är:

- Avtalstyp
- Marknader
- Lösningar

När avtalstyp har valts kan du jämföra referensprestanda med avseende på möjligheter till säljförsäljning, partnerledda och privata avtal. För både marknader och lösningar kan du välja mellan tre olika alternativ för att jämföra deras prestanda. Det första diagrammet, som är ett stapeldiagram, har data som visas med en månadstrend baserat på huvud pivoten, som är volym eller det avtalsvärde som vunnits. Det finns också ett cirkeldiagram till höger om stapeldiagrammet, som visar fördelningen efter procentandel för samma data.

:::image type="content" source="images/referrals/cosell-analytics-compare-v2.png" alt-text="Bild som visar jämförelseavsnittet.":::

## <a name="export"></a>Exportera

Du kan exportera registreringsdata för hänvisningar och avtal. Följande information beskriver exportfunktionen.

- Du kan exportera högst **5 000 poster genom** att klicka på **exportknappen.** Posterna sorteras i fallande ordning baserat på datumet då hänvisningen skapades.
- Exportfunktionen tar hänsyn till tidslinjen och de filter som har tillämpats.
- Partnern kan välja att ladda ned rapporten i csv-format (kommaavgränsat värde) eller TSV-format (tabbavgränsat värde).
- Det kan ta några minuter att ladda ned posterna.
- Du måste vänta tills nedladdningen är klar. Om du navigerar bort avbryts exporten.

## <a name="no-data"></a>Inga data

Det kan finnas flera orsaker till varför du får ett tomt diagram som nedan när du använder co-sell-analys enligt beskrivningen nedan.

- Det finns inga data för det här kontot. Prova att skapa avtal för att få rapporten ifylld.
- Det finns ett problem med nätverksanslutningen. Kontrollera internetanslutningen och försök igen.
- Sidan läses in med standardfiltret för säljavtal. Om du bara har privata avtal återställer du filtret för avtalstyp.
- Det finns inga poster som matchar de filter som du har tillämpat. Försök att återställa filtren.
- Det finns en fördröjning mellan ändringen av affärsmöjlighetstillståndet och för att det ska uppdateras i analysrapporten. Kontrollera rapporten efter 24 timmar.

:::image type="content" source="images/referrals/nodata.png" alt-text="Bild som visar ingen datavisualisering för hänvisningar.":::

> [!NOTE]
> Sidan **Hänvisningsinsikter** visar bara data för hänvisningar som skapats i Partnercenter. Den visar inte data för hänvisningar som genereras via [Partner Sales Anslut](psc-to-pc.md) andra mekanismer.

> [!TIP]
> Om du vill se hur din företagsprofil presterar i find a solution provider experience (Hitta en [lösningsleverantör)](https://www.microsoft.com/solution-providers/home) kan du gå till [sidan Leads insights (Leadsinsikter).](referral-leads-insights.md)

## <a name="next-steps"></a>Nästa steg

- [Utveckla din verksamhet med Microsoft-hänvisningar](referrals.md)
- [Analysera dina leads](referral-leads-insights.md)