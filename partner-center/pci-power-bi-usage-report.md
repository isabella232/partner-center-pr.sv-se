---
title: Power BI användnings rapport för partner Center Insights
ms.topic: article
ms.date: 01/11/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Se vad du gör bra och var du kan förbättra användningen av Power BI prenumerationer som du säljer eller hanterar för dina kunder.
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.openlocfilehash: e05ea33665ded2e52eae2ef8f096b30d3bfe9ee5
ms.sourcegitcommit: 10765386b2df0d4c2e8da9b302a692f452e1090d
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/31/2021
ms.locfileid: "106086302"
---
# <a name="power-bi-usage-report-available-from-the-partner-center-insights-dashboard"></a>Power BI användnings rapport som är tillgänglig från Partner Center Insights-instrumentpanelen

**Lämpliga roller**

- Global administratör
- Administratörs agent
- Rapport visnings program
- Rapport visnings program för chefer

Power BI användnings rapporten innehåller användnings data för de Power BI prenumerationer som du sålde eller hanterar för dina kunder. Du kan visa följande avsnitt från rapporten Power BI användning.

- Sammanfattning
- Power BI användning efter geografi
- Power BI användning per SKU
- Prenumerations prestanda
- Power BI användnings distribution

 > [!NOTE]
 > Den här rapporten är tillgänglig från insikts instrument panelen. Om du vill visa den här rapporten måste du ha tilldelats en speciell roll i Partner Center, till exempel global administratör, konto administratör, rapport visnings program eller Executive Report Viewer. Mer information finns i företagets globala administratör. vissa typer av data i den här rapporten kan också endast vara tillgängliga för användare med behörigheten Executive Report Viewer.

## <a name="summary"></a>Sammanfattning

Avsnittet Sammanfattning visar en ögonblicks bild av de viktigaste indikatorerna för Power BI användnings prenumerationer som du har sålt eller hanterat för dina kunder. 

- Tillgängliga platser: totalt antal sålda licenser under den valda tids perioden.

   Micro-diagrammet presenterar en månads månads trend för tillgängliga antal platser för det valda datum intervallet.

- Tilldelade platser: totalt antal licenser som tilldelats under den valda tids perioden.

   Micro-diagrammet presenterar en månads månads trend för tilldelade platser under det valda datum intervallet.

- Aktiva platser: totalt antal licenser som hade användning under den valda tids perioden. 

   Micro-diagrammet presenterar en månatlig trend för månatliga aktiva platser under den valda tids perioden.

- Aktiv användning%: totalt antal aktiva platser som uttryckts som en procent andel tillgängliga platser för den valda tids perioden. 

   Micro-diagrammet presenterar en månatlig trend för aktiv användnings procent under den valda tids perioden.

:::image type="content" source="images/pci/pci-pbi-usage-summary.png" alt-text="Sammanfattning av Power BI användning":::

## <a name="power-bi-usage-by-geography"></a>Power BI användning efter geografi

**Power BI användning per geografi** visar distributionen av tillgängliga platser och aktiva platser efter kund land. Ljusare färger på kartan representerar lägre värden, medan mörkare färger representerar högre värden. Du kan söka efter och välja ett land i rutnätet för att zooma till.

Tabellen **land/region** visar det totala antalet länder/regioner där Azures användnings händelser genereras.

Du kan söka efter och välja ett land i rutnätet för att zooma till platsen i kartan. Välj alternativet **Start** på kartan för att återgå till den ursprungliga vyn.

:::image type="content" source="images/pci/pci-pbi-usage-geography.png" alt-text="Power BI användning efter geografi":::

## <a name="power-bi-usage-by-sku"></a>Power BI användning per SKU

Power BI användning per SKU visar månads trenden för tillgängliga platser, aktiva platser och tilldelade platser med SKU: er.

:::image type="content" source="images/pci/pci-pbi-usage-sku.png" alt-text="Power BI användning per SKU":::

## <a name="subscriptions-performance"></a>Prenumerations prestanda

Prenumerations prestandan visar månads trenden för aktiv användning per kund prenumeration. Data för de främsta 100 kunderna med fakturerad intäkt visas i tabellen och du kan söka efter en kund eller ladda ned rå data för att visa information om alla prenumerationer.

:::image type="content" source="images/pci/pci-pbi-usage-subscription.png" alt-text="Power BI prenumerations prestanda":::

## <a name="power-bi-usage-distribution"></a>Power BI användnings distribution

Den Power BI användnings fördelningen illustrerar fördelningen av tillgängliga platser, aktiva platser och tilldelade platser med SKU: er.

:::image type="content" source="images/pci/pci-pbi-usage-distribution.png" alt-text="Power BI användnings distribution":::

## <a name="next-steps"></a>Nästa steg

- Mer information finns i [partner Center Insights](partner-center-insights.md).

- Du kan ladda ned rå data från den här rapporten från avsnittet hämta rapporter på instrument panelen insikter. [Läs mer](pci-download-reports.md) 
