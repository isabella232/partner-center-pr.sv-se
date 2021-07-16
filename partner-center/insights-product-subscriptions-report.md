---
title: Partnercenter – Insights prenumerationsrapport
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Se vad du gör bra och var du kan förbättra dina molnprenumerationer som du säljer eller hanterar för dina kunder.
author: shthota77
ms.author: shthota
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: a1ce0e75817376b5cf1996a56f416acc4bcbd0f3
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 07/16/2021
ms.locfileid: "114377026"
---
# <a name="product-subscriptions-report-available-from-the-partner-center-insights-dashboard"></a>Rapport för produktprenumerationer som är tillgänglig från Partnercenter Insights instrumentpanel

**Lämpliga roller:** Globala | Administratörsagent | Rapportvisningsprogram | Visningsprogram för exekutiv rapport

Rapporten Produktprenumerationer visar analys av molnprenumerationer som du har sålt eller som du hanterar för dina kunder. Det här är en produktspecifik rapport som innehåller prestanda för prenumerationer som är associerade med molnprodukter som Office 365, Azure, Dynamics med flera.

Du kan visa följande avsnitt i rapporten Produktprenumerationer.

- Sammanfattning
- Geografisk spridning av prenumerationer
- Lägg till/omsättningstrend för prenumerationer
- Prenumerationsdistribution efter partnerplatser, försäljningskanal, SKU:er, partner attach type, segment
- Trend efter prenumerations tillstånd
- Produkttrend

 > [!NOTE]
 > Den här rapporten är tillgänglig från Insights instrumentpanel. Om du vill visa den här rapporten måste du ha tilldelats en viss roll i Partnercenter, till exempel Global administratör, Kontoadministratör, Rapportvisare eller Visningsprogram för verkställande rapporter. Mer information finns i företagets globala administratör. Vissa typer av data i den här rapporten kan också vara tillgängliga endast för användare med behörighet som chefsrapportvisare.

## <a name="summary"></a>Sammanfattning

I sammanfattningsavsnittet visas en ögonblicksbild av KPI:er (Key Performance Indicators) relaterade till prenumerationer som säljs eller hanteras av dig för dina kunder.  

:::image type="content" source="images/insights/sub-report-summary.png" alt-text="rapportsammanfattning för prenumerationer.":::

Mer information om varje avsnitt i sammanfattningen finns nedan:

- Prenumerationer:
  - Aktuellt antal molnproduktprenumerationer som sålts eller hanteras av dig.
  - Procentuell ökning eller minskning av prenumerationer under det valda datumintervallet.
  - Micro-diagrammet visar en trend för antalet prenumerationer månad för månad under det valda datumintervallet.

- Aktiva prenumerationer:
  - Aktuellt antal molnproduktprenumerationer med aktiv användning mätt baserat på produkttelemetri. Detta exkluderar alla utvärderingsprenumerationer för Azure-prenumerationer.
  - Procentuell ökning eller minskning av aktiva prenumerationer under den valda tidsperioden.
  - Micro-diagrammet visar en månad över månad-trend för aktiva prenumerationer under det valda datumintervallet.

- Prenumerationer har lagts till:
  - Totalt antal kundprenumerationer som du har lagt till (sålt eller hanterat) under det valda datumintervallet. Nya prenumerationer med tillståndet **Aktiv** eller **Förnyad** räknas som prenumerationer som läggs till.
  - Procentuell ökning eller minskning av prenumerationer som lagts till under den senaste fullständiga månaden jämfört med den första fullständiga månaden.
  - Micro-diagrammet visar en månatlig trend för prenumerationer som lagts till under det valda datumintervallet.

- Omsade prenumerationer:
  - Totalt antal kundprenumerationer som omsörts under det valda datumintervallet. Prenumerationer med tillståndet **Avetablerade eller** **Pausade** under den månaden räknas som en omsedd prenumeration.  
  - Procentandel prenumerationer som omsörts under det valda datumintervallet.
  - Micro-diagrammet visar en månatlig trend för prenumerationer som omsörts under det valda datumintervallet.

- Prenumerationer efter produkter: Uppdelning av det aktuella prenumerationsantalet efter molnprodukter.

## <a name="geographical-spread-of-subscriptions"></a>Geografisk spridning av prenumerationer

I **vyn Prenumerationer efter geografisk** plats visas den geografiska fördelningen av det totala antalet prenumerationer efter kundmarknad. Det totala prenumerationsbeloppet omfattar både sålda prenumerationer och aktiva prenumerationer.

I **tabellen Antal länder/regioner** visas det totala antalet länder/regioner där du har prenumerationer och beloppet per land för totalt antal och aktiva prenumerationer.

Du kan söka efter och välja ett land i rutnätet för att zooma till platsen på kartan. Tryck på **alternativet** Start på kartan för att återgå till den ursprungliga vyn. Hovra över kartan för att visa alla prenumerationer och aktiva prenumerationer efter land. Båda fälten i rutnätet är sorterbara.

:::image type="content" source="images/insights/sub-report-sub-by-geography.png" alt-text="prenumerationer efter geografiskt område.":::

## <a name="subscription-addschurns"></a>Prenumerationen lägger till/omar

Den här vyn visar en trend för prenumerationer. Dessa är uppdelade i olika kategorier (Ny, Befintlig, Omsned) för det valda datumintervallet. X-axeln representerar månader för det valda datumintervallet. Y-axeln representerar antalet prenumerationer. Omomsättningsprenumerationer representeras på den negativa skalan för Y-axeln. 

Det staplade stapeldiagrammet visar en analys av nya, befintliga och omkastade prenumerationer för månaden. Du kan återskapa stapeldiagrammet, uppdelat med specifika stackobjekt. Det gör du genom att välja de specifika objekten i förklaringen. Du kan också använda skjutreglaget överst i diagrammet för att zooma in i en viss punkt.

:::image type="content" source="images/insights/sub-report-sub-adds-churns.png" alt-text="prenumeration lägger till och omsättningar.":::

## <a name="subscription-distribution"></a>Prenumerationsdistribution

I den här vyn visas en analys av dina aktuella prenumerationer efter dina Microsoft Partner Network-platser (MPN), kundsegment, försäljningskanal/Azure-prismodell och attributionstyp. Välj respektive flikar för att visa uppdelningen efter dessa kategorier. Om du vill skapa cirkeldiagrammet med en analys av specifika objektkategorier väljer du de objektkategorierna i förklaringen.

:::image type="content" source="images/insights/sub-report-distribution.png" alt-text="prenumerationsdistribution.":::

## <a name="subscription-state-distribution"></a>Distribution av prenumerationstillstånd

I den här vyn visas distributionen av dina aktuella kundprenumerationer efter prenumerationsstatus eller prenumerationsstatus. Detta inkluderar följande prenumerations tillstånd: **Active**, **Disabled**, **Deprovisioned**, **Open**, **InGracePeriod**, **Closed** och **Others**.

:::image type="content" source="images/insights/sub-report-sub-states.png" alt-text="distribution av prenumerationstillstånd.":::

## <a name="products-trend"></a>Produkttrend

I den här vyn visas ett stapeldiagram och två cirkeldiagram. Stapeldiagrammet visar en månatlig trend för prenumerationer uppdelade efter kommersiella produkter, till exempel Azure, Office och Dynamics.

De två cirkeldiagrammen visar en analys av dina aktuella kundprenumerationer. Det första cirkeldiagrammet delar upp prenumerationer efter produkter. Det andra cirkeldiagrammet delar upp prenumerationer efter SKU:er eller planer. När du väljer en  produkt i cirkeldiagrammet Detaljinformation efter Produkter visar det intilliggande cirkeldiagrammet en analys av den produktens prenumerationer efter SKU:er.

:::image type="content" source="images/insights/sub-report-prods-trend.png" alt-text="produkttrend.":::

> [!NOTE]
 > Antalet prenumerationer uppdelade efter SKU:er överensstämmer kanske inte alltid med det totala antalet prenumerationer för den produkten. Detta kan inträffa om en kund har köpt flera SKU:er under samma produktprenumeration.

## <a name="next-steps"></a>Nästa steg

- Fler rapporter finns i [Partnercenter Insights](partner-center-insights.md).

>[!NOTE] 
> Du kan ladda ned rådata som driver den här rapporten från avsnittet Ladda ned rapporter i Insights instrumentpanel. [Läs mer](insights-download-reports.md) 
