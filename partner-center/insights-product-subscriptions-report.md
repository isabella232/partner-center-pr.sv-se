---
title: Partnercenter Insights prenumerationsrapport
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-insights
description: Se vad du gör bra och var du kan förbättra dina kunders molnprenumerationer.
author: shthota77
ms.author: shthota
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: eefb4f4ee6657acf583ad0b5d4149e662c320184
ms.sourcegitcommit: 37eac16c4339cb97831eb2a86d156c45bdf6a531
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/13/2021
ms.locfileid: "126246811"
---
# <a name="product-subscriptions-report-available-from-the-partner-center-insights-dashboard"></a>Rapport för produktprenumerationer som är tillgänglig Insights Partnercenter

**Lämpliga roller:** Global | Administratörsagentens | Rapportvisningsprogram | Rapportvisningsprogram för chefer

Rapporten Produktprenumerationer visar analys av molnprenumerationer som du har sålt eller som du hanterar för dina kunder. Det här är en produktspecifik rapport som innehåller prestanda för prenumerationer som är associerade med molnprodukter som Office 365, Azure, Dynamics med flera.

Du kan visa följande avsnitt i rapporten Produktprenumerationer.

- Sammanfattning
- Geografisk spridning av prenumerationer
- Lägg till/omsättningstrend för prenumerationer
- Prenumerationsdistribution efter partnerplatser, försäljningskanal, SKU:er, partner bifoga typ, segment
- Trend efter prenumerations tillstånd
- Produkttrend

 > [!NOTE]
 > Den här rapporten är tillgänglig från Insights instrumentpanel. Om du vill visa den här rapporten måste du ha tilldelats en viss roll i Partnercenter, till exempel Global administratör, Kontoadministratör, Rapportvisningsprogram eller Visningsprogram för verkställande rapporter. Mer information finns i företagets globala administratör. Vissa typer av data i den här rapporten kan också vara tillgängliga endast för användare med privilegier för visningsprogrammet för chefsrapport.

## <a name="summary"></a>Sammanfattning

I sammanfattningsavsnittet visas en ögonblicksbild av KPI:er (Key Performance Indicators) relaterade till prenumerationer som säljs eller hanteras av dig för dina kunder.  

:::image type="content" source="images/insights/sub-report-summary.png" alt-text="prenumerationsrapportsammanfattning.":::

Mer information om varje avsnitt i sammanfattningen finns nedan:

- Prenumerationer:
  - Aktuellt antal molnproduktprenumerationer sålda eller hanterade av dig.
  - Procentuell ökning eller minskning av prenumerationer under det valda datumintervallet.
  - Micro-diagrammet visar en trend för antalet prenumerationer under månaden under det valda datumintervallet.

- Aktiva prenumerationer:
  - Aktuellt antal molnproduktprenumerationer med aktiv användning mätt baserat på produkttelemetri. Detta exkluderar alla utvärderingsprenumerationer för Azure-prenumerationer.
  - Procentuell ökning eller minskning av aktiva prenumerationer under den valda tidsperioden.
  - Micro-diagrammet visar en trend för aktiva prenumerationer månad för månad under det valda datumintervallet.

- Prenumerationer har lagts till:
  - Totalt antal kundprenumerationer som du har lagt till (sålt eller hanterat) under det valda datumintervallet. Nya prenumerationer med **tillståndet Aktiv** **eller Förnyad** räknas som Prenumerationer som läggs till.
  - Procentuell ökning eller minskning av prenumerationer som lagts till under den senaste fullständiga månaden jämfört med den första fullständiga månaden.
  - Micro-diagrammet visar en månatlig trend för prenumerationer som lagts till under det valda datumintervallet.

- Prenumerationer oms churned:
  - Totalt antal kundprenumerationer som omsnats under det valda datumintervallet. Prenumerationer med tillståndet **Avetablerade eller** **Inaktiverade** under den månaden räknas som en omsnavd prenumeration.  
  - Procentandel prenumerationer som omsnats under det valda datumintervallet.
  - Mikrodiagrammet visar en månatlig trend för prenumerationer som omsnats över det valda datumintervallet.

- Prenumerationer efter produkter: Uppdelning av det aktuella prenumerationsantalet efter molnprodukter.

## <a name="geographical-spread-of-subscriptions"></a>Geografisk spridning av prenumerationer

I **vyn Prenumerationer per geografisk** plats visas den geografiska fördelningen av de totala prenumerationerna efter kundmarknad. Det totala prenumerationsbeloppet omfattar både sålda prenumerationer och aktiva prenumerationer.

I **tabellen Antal länder/regioner** visas det totala antalet länder/regioner där du har prenumerationer och beloppet per land för totalt antal och aktiva prenumerationer.

Du kan söka efter och välja ett land i rutnätet för att zooma till platsen på kartan. Tryck på **alternativet** Start på kartan för att återgå till den ursprungliga vyn. Hovra över kartan för att visa alla prenumerationer och aktiva prenumerationer efter land. Båda fälten i rutnätet är sorterbara.

:::image type="content" source="images/insights/sub-report-sub-by-geography.png" alt-text="prenumerationer efter geografiskt område.":::

## <a name="subscription-addschurns"></a>Prenumeration lägger till/omsättningar

Den här vyn visar en trend för prenumerationer. Dessa är uppdelade i olika kategorier (Ny, Befintlig, Omsättning) för det valda datumintervallet. X-axeln representerar månader för det valda datumintervallet. Y-axeln representerar antalet prenumerationer. Omkastade prenumerationer representeras på den negativa skalan för Y-axeln. 

Det staplade stapeldiagrammet visar en analys av nya, befintliga och omkastade prenumerationer för månaden. Du kan återskapa stapeldiagrammet, uppdelat med specifika stackobjekt. Det gör du genom att välja de specifika objekten i förklaringen. Du kan också använda skjutreglaget överst i diagrammet för att zooma in en viss punkt.

:::image type="content" source="images/insights/sub-report-sub-adds-churns.png" alt-text="prenumeration lägger till och omsättningar.":::

## <a name="subscription-distribution"></a>Prenumerationsdistribution

I den här vyn visas en analys av dina aktuella prenumerationer efter dina Microsoft Partner Network-platser (MPN), kundsegment, försäljningskanal/Azure-prismodell och attributionstyp. Välj respektive flikar för att visa uppdelningen efter dessa kategorier. Om du vill skapa cirkeldiagrammet med en analys av specifika objektkategorier väljer du de objektkategorierna i förklaringen.

:::image type="content" source="images/insights/sub-report-distribution.png" alt-text="prenumerationsdistribution.":::

## <a name="subscription-state-distribution"></a>Distribution av prenumerationstillstånd

I den här vyn visas distributionen av dina aktuella kundprenumerationer efter prenumerationsstatus eller prenumerationsstatus. Detta inkluderar följande prenumerations tillstånd: **Aktiv**, **Inaktiverad**, **Avetablerade**, **Öppna,** **InGracePeriod,** **Stängd** och **andra**.

:::image type="content" source="images/insights/sub-report-sub-states.png" alt-text="distribution av prenumerationstillstånd.":::

## <a name="products-trend"></a>Produkttrend

Den här vyn visar ett stapeldiagram och två cirkeldiagram. Stapeldiagrammet visar en månatlig trend för prenumerationer uppdelade efter kommersiella produkter, till exempel Azure, Office och Dynamics.

De två cirkeldiagrammen visar en analys av dina aktuella kundprenumerationer. Det första cirkeldiagrammet delar upp prenumerationer efter produkter. Det andra cirkeldiagrammet delar upp prenumerationer efter SKU:er eller planer. När du väljer en  produkt i detalj efter cirkeldiagrammet Produkter visar det intilliggande cirkeldiagrammet en uppdelning av produktens prenumerationer efter SKU:er.

:::image type="content" source="images/insights/sub-report-prods-trend.png" alt-text="produkttrend.":::

> [!NOTE]
 > Antalet prenumerationer uppdelade efter SKU:er kanske inte alltid matchar det totala prenumerationsantalet för den produkten. Detta kan inträffa om en kund har köpt flera SKU:er under samma produktprenumeration.

## <a name="next-steps"></a>Nästa steg

- Fler rapporter finns i [Partnercenter Insights](partner-center-insights.md).

>[!NOTE] 
> Du kan ladda ned rådata som driver den här rapporten från avsnittet Ladda ned rapporter i Insights instrumentpanel. [Läs mer](insights-download-reports.md) 
