---
title: Hämta insikter om hänvisningar
ms.topic: article
ms.date: 02/26/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Granska dina referral Insights-data regelbundet i Partner Center för att se trender för att hjälpa dig att uppnå dina affärs mål.
author: rajap-ms
ms.author: rajap
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: f58a7cc34b5b5b5755f652faf220d290ec2a355d
ms.sourcegitcommit: 700150044ea4f1a0b96cb4caeb97d7197da29ef6
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/25/2021
ms.locfileid: "105549268"
---
# <a name="get-referral-insights-in-partner-center-and-find-out-how-your-referrals-are-doing"></a>Få referensinformation om Partner Center och ta reda på hur dina hänvisningar fungerar

På sidan för **samförsäljnings möjligheter** under avsnittet **analys** i hänvisningar kan du se hur dina hänvisningar fungerar. Granska dessa mått regelbundet för att identifiera trender eller områden som behöver åtgärdas och börja rikta mot dina affärs mål.

Om du vill se dina samordnade affärs möjligheter insikter från menyn Partner Center går du till **rekommendationer > Analytics > samförsäljnings möjligheter**.

> [!Important]
> Filtret för avtals typ tillämpas i förväg med den typ av **Co-försäljning** som har valts för alla data. Ta bort filtret om du vill anlayze data som rör privata erbjudanden.

## <a name="apply-filters"></a>Använda filter

Längst upp på sidan **samförsäljnings möjligheter** kan du välja den tids period som du vill visa data för. Standard valet är **3m** (tre månader), men du kan välja att visa data i sex månader eller ett år i stället. Du kan också välja **anpassad** om du vill se data för alla referenser under en viss tids period.

Du kan välja knappen **filter** för att öppna panelen där du kan filtrera alla data på den här sidan med kund namn, land, avtals typ, avtals riktning, lösnings namn och status. Nedan visas information om dessa filter.

- **Kund namn**: standardvärdet är **alla**, men du kan begränsa data till en eller flera kunder som du väljer.
- **Land**: standardvärdet är **alla**, men du kan begränsa data till ett eller flera länder för kunden som du väljer.
- **Avtals typ**: standardvärdet är **alla**, men du kan begränsa data till antingen samförsäljnings möjligheter eller privata avtal baserat på ditt val.
- **Avtals riktning** Standardvärdet är **alla**, men du kan välja att begränsa data till antingen **inkommande** referenser (som du har tagit emot) eller **utgående** referenser (som du har skickat).
- **Lösnings namn**: standardvärdet är **alla**, men du kan välja att begränsa data till referenser som innehåller en eller flera lösningar som du väljer.
- **Status**: standardvärdet är **alla**, men du kan välja att begränsa data till referenser som innehåller en eller flera hänvisnings status typer som accepterade, nekade, förfallna, förlorade och uppnådda som du väljer.

Informationen i alla diagram som visas nedan visar datum intervallet och eventuella filter som du har valt, förutom vad som anges nedan. I vissa avsnitt kan du också använda extra filter, till exempel filtrera till en viss lösning.

## <a name="referrals-summary"></a>Sammanfattning av referenser

Det här kortet visar en översikt över hur dina samförsäljnings möjligheter fungerar.

Diagrammet visar det totala antalet avtal, det antal som vanns, antalet förlorade och den totala avtals volymen (i USD) för den valda tids perioden.

Procent måtten för ändring (som visas i rött eller grönt, med en pil-indikator) visar skillnaden mellan den **senaste fullständiga månaden i det valda datum intervallet** och den **första fullständiga månaden i intervallet**. Anta till exempel att det aktuella datumet är 15 juni och att du har valt **3m** -filtret för att visa data för de senaste tre månaderna. I det här fallet skulle dessa mått Visa skillnaden mellan maj (den senaste fullständiga månaden för den valda tids perioden) och mars (den första fullständiga månaden för den valda tids perioden) det datum intervall som valts är sista **3m**, jämförelsen skulle vara mellan data för maj och data för mars.

:::image type="content" source="images/referrals/cosellanalyticssummary.png" alt-text="Bild som visar sammanfattnings kortet för samförsäljning av affärs möjligheter analyser.":::

## <a name="conversion-funnel"></a>Omvandlings tratt

Det här avsnittet visar en visuell indikator för hur dina avtal flyttas från ett tillstånd till ett annat via deras livs cykel. Du kan visa hela livs cykeln baserat på den avtalade volymen samt det avtalade värdet i USD baserat på det huvudsakliga Pivot-området för det här avsnittet. Det första avsnittet är märkt både med tillstånd och typ av affären för att ge dig en visuell indikator för volymen eller värdet efter typ. Det finns också ett avsnitt som **redan har inträffat**, som används för att ange vilka avtal som du har vidtagit för att antingen acceptera/avböja dem eller markera dem som vunna/förlorade under den tids period som har valts för rapporten. Du kan använda filter för att visa förloppet för de olika stegen i deras livs cykel.

:::image type="content" source="images/referrals/cosellanalyticsfunnel.png" alt-text="Bild som visar omvandlings tratten för referenser.":::

## <a name="deals-by-geography"></a>Avtal per geografi

I det här avsnittet visas de länder/regioner där avtal kom från, tillsammans med information för varje land/region. Det finns en tabellvy över avtals detaljerna för varje land, tillsammans med en karta över alla länder. Du kan välja ett särskilt land i tabellen eller välja vyn mappa för att zooma till ett särskilt land.

:::image type="content" source="images/referrals/cosellanalyticsgeodistribution.png" alt-text="Bild som visar geo-distributionen av hänvisningar.":::

## <a name="deals-by-solutions"></a>Avtal utifrån lösningar

I det här diagrammet kan du se vilka av dina lösningar som kör flest hänvisningar och det högsta värdet. Tabellen har två Pivot-förs-och privat-produkter.
Baserat på ditt val av ditt val kan du se prestandan för de avtal som sammanställs av lösningen.

> [!NOTE]
> Om flera lösningar ingår i ett avtal visar tabellen samma avtal för alla dessa lösningar. Du bör inte lägga till värden som är relaterade till lösningar och jämföra dem med andra referens volym mått. Den här vyn är avsedd att hjälpa dig att förstå avtals prestandan med lösningen Pivot.

Tabellen har total avtal som innehåller lösningen som ingår i dem och motsvarande tillstånd, t. ex. vunna avtal, förlorade avtal, avtal upphör att gälla tillsammans med det totala värdet för avtals vinst och förlust i KRONORnas valuta. Det finns också ett trend diagram för avtal till höger om tabellen som visar de totala antalet avtal och det avtalade värdet i USD-valutan baserat på den valda lösningen. Standard valet är alla lösningar.

:::image type="content" source="images/referrals/cosellanalyticssolutions.png" alt-text="Bild som visar lösningens prestanda.":::

## <a name="declined--lost-reasons"></a>Nekade & förlorade orsaker

I det här avsnittet får du hjälp att analysera **orsakerna till att** avtalen markeras som avvisade eller **förlorade** av ditt företag. Alternativen i dessa representationer är samma orsaker som säljarna har valt när de stänger affären som nekad eller förlorad.

:::image type="content" source="images/referrals/cosellanalyticsreasons.png" alt-text="Bild som visar de orsaker som valts av partnern när de avböjer eller gör en affär som förlorad.":::

## <a name="comparison-charts"></a>Jämförelse diagram

Jämförelse avsnittet hjälper dig att jämföra data som rör hänvisningar baserat på flera dimensioner både på volymen och de avtals värden som vunnits i USD-Pivot.
De tre dimensionerna som du kan välja för att jämföra data är

- Avtals typ
- Marknaden
- Lösningar

När du väljer avtals typ kan du jämföra hänvisnings prestandan för med avseende på samförsäljnings möjligheter och privata avtal. För både marknader och lösningar kan du hämta upp till tre olika alternativ för att jämföra deras prestanda. Det första diagrammet, som är ett stapeldiagram, kommer att ha data som visas i månaden på månads trend, baserat på huvud Pivot, som är volym eller uppnådda avtals värde. Det finns också ett cirkel diagram till höger om stapeldiagrammet, som visar fördelningen i procent för samma data.

:::image type="content" source="images/referrals/cosellanalyticscompare.png" alt-text="Bild som visar jämförelse avsnittet.":::

## <a name="raw-data-table"></a>Rå data tabell

I tabellen nedan med alla rå data som är relaterade till samförsäljnings möjligheterna kan du snabbt **Exportera** data för alla detaljerade eller anpassade analyser som du vill utföra.

:::image type="content" source="images/referrals/cosellanalyticsrawdata.png" alt-text="Bild som visar rå data tabell för hänvisningar.":::

## <a name="no-data"></a>Inga data

Det kan finnas flera orsaker till att du får ett tomt diagram, till exempel nedan, när du får åtkomst till co-försäljnings analys enligt beskrivningen nedan.

- Det finns inga data för det här kontot. Försök att skapa avtal för att få den här rapporten ifylld.
- Det finns ett problem med nätverks anslutningen. Kontrol lera din Internet anslutning och försök igen.
- Sidan hämtas med standard filtret för samförsäljnings avtal. Om du bara har privata erbjudanden återställer du filtret för avtals typ.
- Det finns inga poster som matchar de filter som du har använt. Försök att återställa filtren.
- Det finns en fördröjning mellan ändring av affärs möjlighets tillstånd och för samma som ska uppdateras i analys rapporten. Kontrol lera rapporten efter 24 timmar.

:::image type="content" source="images/referrals/nodata.png" alt-text="Bild som visar inga data visualiseringar för referenser.":::

> [!NOTE]
> Sidan **Hänvisningsinsikter** visar bara data för hänvisningar som skapats i Partnercenter. Den visar inte data för hänvisningar som skapats via [partner Sales Connect](psc-to-pc.md) eller andra mekanismer.

> [!TIP]
> Om du vill se hur din företags profil presterar i [lösningen hitta en lösnings leverantör](https://www.microsoft.com/solution-providers/home) kan du läsa mer i [sidan affärs profil insikter](analyze-your-marketing-profile.md).
