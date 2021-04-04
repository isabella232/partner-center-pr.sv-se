---
title: Azures användnings rapport för partner Center Insights
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Se vad du gör bra och var du kan förbättra din användning av Azure-prenumerationer som du säljer eller hanterar för dina kunder.
author: shthota77
ms.author: shthota
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: ef72aa2e44797c906cdd0a216cf2d8355668c0a9
ms.sourcegitcommit: 10765386b2df0d4c2e8da9b302a692f452e1090d
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/31/2021
ms.locfileid: "106086217"
---
# <a name="azure-usage-report-available-from-the-partner-center-insights-dashboard"></a>Azures användnings rapport som är tillgänglig från Partner Center Insights-instrumentpanelen

**Lämpliga roller**

- Global administratör
- Administratörs agent
- Rapport visnings program
- Rapport visnings program för chefer

I rapporten Azure Usage visas mått som är relaterade till dina kunders Azure-prenumerationer. Den här rapporten inkluderar Azures förbruknings intäkter och användning efter mätnings kategorier. Du kan visa följande avsnitt från rapporten Azure Usage.

- Sammanfattning
- Användning av geografi i Azure
- Azure-användning

 > [!NOTE]
 > Den här rapporten är tillgänglig från insikts instrument panelen. Om du vill visa den här rapporten måste du ha tilldelats en speciell roll i Partner Center, till exempel global administratör, konto administratör, rapport visnings program eller Executive Report Viewer. Mer information finns i företagets globala administratör. vissa typer av data i den här rapporten kan också endast vara tillgängliga för användare med behörigheten Executive Report Viewer.

## <a name="summary"></a>Sammanfattning

Avsnittet Sammanfattning visar en ögonblicks bild av KPI: er (nyckeltal) som relaterar till Azure-prenumerationer som säljs eller hanteras av dig för dina kunder.  

- Azure-prenumerationer: Aktuellt antal Azure kund prenumerationer som säljs eller hanteras av dig.
Procentuell tillväxt eller avböja de här Azure-prenumerationerna under det valda datum intervallet.

Micro-diagrammet presenterar en månads månads trend för antalet Azure-prenumerationer för det valda datum intervallet.
- Aktiva Azure-prenumerationer: Aktuellt antal Azure-prenumerationer som har sålts eller hanteras av dig som haft aktiv användning under de senaste 30 dagarna.
Procentuell tillväxt eller avböja de här prenumerationerna under det valda datum intervallet.

Micro-diagrammet presenterar en månads månads trend för antalet Azure Active-prenumerationer under det valda datum intervallet.

- Förbrukade intäkter i Azure (ACR): total förbrukad Azure-intäkt (US $) som är tilldelad till dig under det valda datum intervallet.
Procentuell tillväxt eller avböja av attributet ACR US $ under det valda datum intervallet. 

Micro-diagrammet presenterar en månatlig trend för ACR US $ som är tilldelad till dig under den valda tids perioden


> [!NOTE]
 > Azures förbrukade intäkter (ACR) visas bara för användare som har tilldelats rollen Executive Report Viewer.

:::image type="content" source="images/pci/pci-azure-usage-summary-1.png" alt-text="Översikt över Azure-användning":::

## <a name="azure-usage-by-geography"></a>Användning av geografi i Azure

Vyn **för Azure-användning per geografi** visar den geografiska distributionen av Azures förbruknings intäkter (ACR US $) eller användnings timmar för alla eller valda Azure Service nivå/meter-kategorier. Ljusare färger på kartan representerar lägre värden, medan mörkare färger representerar högre värden. Du kan söka efter och välja ett land i rutnätet för att zooma till 

Tabellen **land/region** visar det totala antalet länder/regioner där Azures användnings händelser genereras.

Du kan söka efter och välja ett land i rutnätet för att zooma till platsen i kartan. Välj alternativet **Start** på kartan för att återgå till den ursprungliga vyn.

:::image type="content" source="images/pci/pci-azure-usage-by-geography-2.png" alt-text="Användning av geografi i Azure":::

## <a name="azure-utilization"></a>Azure-användning

I den här vyn visas trender per månads användning av Azure-förbrukning eller användnings timmar för de valda kategorierna för Azure Service nivå/meter. 

I stapeldiagrammet visas en trend för månads intäkterna/förbrukning per timme. Linje diagrammet presenterar tillväxt trenden jämfört med föregående månad för de valda kategorierna för Azure Service nivå/meter.

:::image type="content" source="images/pci/pci-azure-usage-utilization-3.png" alt-text="Användnings användning i Azure":::

## <a name="next-steps"></a>Nästa steg

- Mer information finns i [partner Center Insights](partner-center-insights.md).

>[!NOTE] 
> Du kan ladda ned rå data från den här rapporten från avsnittet hämta rapporter på instrument panelen insikter. [Läs mer](pci-download-reports.md) 
