---
title: Rapporten Partner Center Insights-prenumerationer
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Se vad du gör bra och var du kan förbättra de moln prenumerationer du säljer eller hanterar för dina kunder.
author: shthota77
ms.author: shthota
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 019e489b4738515639bf181591dfbc671e1b795d
ms.sourcegitcommit: 10765386b2df0d4c2e8da9b302a692f452e1090d
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/31/2021
ms.locfileid: "106086200"
---
# <a name="product-subscriptions-report-available-from-the-partner-center-insights-dashboard"></a>Produkt prenumerations rapport som är tillgänglig från Partner Center Insights-instrumentpanelen

**Lämpliga roller**

- Global administratör
- Administratörs agent
- Rapport visnings program
- Rapport visnings program för chefer

Rapporten produkt prenumerationer visar analyser av moln prenumerationer som du har sålt eller som du hanterar för dina kunder. Det här är en produktspecifik rapport som innehåller prestanda för prenumerationer som är kopplade till moln produkter som Office 365, Azure, Dynamics och andra.

Du kan visa följande avsnitt från rapporten produkt prenumerationer.

- Sammanfattning
- Geografiskt spridning av prenumerationer
- Trend för prenumerations tillägg/omsättning
- Prenumerations distribution efter partner platser, försäljnings kanal, SKU: er, partner kopplings typ, segment
- Trend efter prenumerations tillstånd
- Produkter trend

 > [!NOTE]
 > Den här rapporten är tillgänglig från insikts instrument panelen. Om du vill visa den här rapporten måste du ha tilldelats en speciell roll i Partner Center, till exempel global administratör, konto administratör, rapport visnings program eller Executive Report Viewer. Mer information finns i företagets globala administratör. vissa typer av data i den här rapporten kan också endast vara tillgängliga för användare med behörigheten Executive Report Viewer.

## <a name="summary"></a>Sammanfattning

Avsnittet Sammanfattning visar en Snapshot-vy över KPI: er (nyckeltal) som rör prenumerationer som säljs eller hanteras av dig för dina kunder.  

:::image type="content" source="images/pci/pci-sub-report-summary-1.png" alt-text="rapport Sammanfattning för prenumerationer":::

Mer information om varje avsnitt i sammanfattningen finns nedan:

- Prenumerationer:
  - Aktuellt antal moln produkt prenumerationer som säljs eller hanteras av dig.
  - Procentuell tillväxt eller neka prenumerationer under det valda datum intervallet.
  - Micro-diagrammet presenterar en månads månads trend av prenumerations antalet under det valda datum intervallet.

- Aktiva prenumerationer:
  - Aktuellt antal moln produkt prenumerationer med aktiv användning mätt baserat på produkt telemetri. Detta utesluter alla utvärderings prenumerationer om Azure-prenumerationer.
  - Procentuell tillväxt eller avböja aktiva prenumerationer under den valda tids perioden.
  - Micro-diagrammet presenterar en månads månads trend för aktiva prenumerationer under det valda datum intervallet.

- Prenumerationer har lagts till:
  - Totalt antal kund prenumerationer som har lagts till (säljs eller hanteras) av dig under det valda datum intervallet. Nya prenumerationer med **aktiv** eller **förnyad** status räknas som prenumerationer som läggs till.
  - Procentuell tillväxt eller avböja prenumerationer som lagts till under den senaste fullständiga månaden jämfört med den första fullständiga månaden.
  - Micro-diagrammet presenterar en månatlig trend för prenumerationer som lagts till under det valda datum intervallet.

- Överomsättnings prenumerationer:
  - Totalt antal kund prenumerationer som har omsättningen under det valda datum intervallet. Prenumerationer med tillstånd **avetablerade** eller **inaktiverade** under den månaden räknas som en uppdelad prenumeration.  
  - Procent andel prenumerationer som har överomsättnings under det valda datum intervallet.
  - Micro-diagrammet presenterar en månatlig trend för prenumerationer som är uppdelade under det valda datum intervallet.

- Prenumerationer per produkter: analys av det aktuella antalet prenumerationer efter moln produkter.

## <a name="geographical-spread-of-subscriptions"></a>Geografiskt spridning av prenumerationer

Vyn **prenumerationer per geografi** visar den geografiska fördelningen av de totala prenumerationerna av kund marknader. Det totala prenumerations beloppet omfattar både sålda prenumerationer och aktiva prenumerationer.

Tabellen **land/region** visar det totala antalet länder/regioner där du har prenumerationer och belopp per land för totalt antal och aktiva prenumerationer.

Du kan söka efter och välja ett land i rutnätet för att zooma till platsen i kartan. Tryck på **Start** alternativet på kartan för att återgå till den ursprungliga vyn. Hovra över kartan för att visa alla prenumerationer och aktiva prenumerationer efter land. Båda fälten i rutnätet kan sorteras.

:::image type="content" source="images/pci/pci-sub-report-sub-by-geography-2.png" alt-text="prenumerationer per geografi":::

## <a name="subscription-addschurns"></a>Prenumerations tillägg/omsättning

I den här vyn presenteras en trend för prenumerationer. Dessa delas upp i olika kategorier (nya, befintliga, uppdelade) för det valda datum intervallet. X-axeln representerar månader i det valda datum intervallet. Y-axeln representerar antalet prenumerationer. Omsättnings bara prenumerationer representeras på den negativa skalan på Y-axeln. 

Det liggande stapeldiagrammet visar en uppdelning av nya, befintliga och brutna prenumerationer för månaden. Du kan återskapa stapeldiagrammet, uppdelat med specifika stack-objekt. Det gör du genom att markera de aktuella objekten i förklaringen. Du kan också använda skjutreglaget ovanpå diagrammet för att zooma in i en viss period.

:::image type="content" source="images/pci/pci-sub-report-sub-adds-churns-3.png" alt-text="prenumerations tillägg och omsättning":::

## <a name="subscription-distribution"></a>Prenumerations distribution

I den här vyn presenteras en uppdelning av dina aktuella prenumerationer av dina MPN-platser, kund segment, försäljnings kanaler/Azures pris modell och behörighets typ (till exempel DPOR, DAP och andra). Välj respektive flikar för att Visa uppdelningen efter dessa kategorier. Om du vill bygga cirkel diagrammet med en uppdelning av specifika objekt kategorier väljer du dessa objekt kategorier i förklaringen.

:::image type="content" source="images/pci/pci-sub-report-distribution-4.png" alt-text="prenumerations distribution":::

## <a name="subscription-state-distribution"></a>Distribution av prenumerations tillstånd

Den här vyn visar distributionen av dina aktuella kund prenumerationer efter prenumerations status eller status. Detta omfattar följande prenumerations tillstånd: **aktiva**, **inaktiverade**, **avetablerade**, **Öppna**, **statusen ingraceperiod**, **stängda** och **andra**.

:::image type="content" source="images/pci/pci-sub-report-sub-states-5.png" alt-text="distribution av prenumerations tillstånd":::

## <a name="products-trend"></a>Produkter trend

I den här vyn visas ett liggande stapeldiagram och två cirkel diagram. Stapeldiagrammet visar en månatlig trend för prenumerationer som delas upp av kommersiella produkter, till exempel Azure, Office, Dynamics osv.

De två cirkel diagrammen visar en uppdelning av dina aktuella kund prenumerationer. Det första cirkel diagrammet delar upp prenumerationer efter produkter. Det andra cirkel diagrammet delar upp prenumerationer efter SKU: er eller planer. När du väljer en produkt i cirkel diagrammet dela **efter produkter** visar det intilliggande cirkel diagrammet en uppdelning av produktens prenumerationer efter SKU: er.

:::image type="content" source="images/pci/pci-sub-report-prods-trend-6.png" alt-text="produkter trend":::

> [!NOTE]
 > Antalet prenumerationer som delas upp av SKU: er kanske inte alltid matchar det totala antalet prenumerationer för produkten. Detta kan inträffa om en kund har köpt flera SKU: er under samma produkt prenumeration.

## <a name="next-steps"></a>Nästa steg

- Mer information finns i [partner Center Insights](partner-center-insights.md).

>[!NOTE] 
> Du kan ladda ned rå data från den här rapporten från avsnittet hämta rapporter på instrument panelen insikter. [Läs mer](pci-download-reports.md) 
