---
title: Partner Center Insights Azure-användningsrapport
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Se vad du gör bra och var du kan förbättra din användning av Azure-prenumerationer som du säljer eller hanterar för dina kunder.
author: shthota77
ms.author: shthota
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 0d9224e9d86c540cc463538acc435f682cdc2d58
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 05/19/2021
ms.locfileid: "110146858"
---
# <a name="azure-usage-report-available-from-the-partner-center-insights-dashboard"></a>Azure-användningsrapport som är tillgänglig från instrumentpanelen i Partnercenter Insights

**Lämpliga roller:** Globala | Administratörsagent | Rapportvisningsprogram | Visningsprogram för exekutiv rapport

Azure-användningsrapporten visar mått som rör dina kunders Azure-prenumerationer. Den här rapporten innehåller Azure-förbrukningsintäkter och -användning efter mätarkategorier. Du kan visa följande avsnitt från Azure-användningsrapporten.

- Sammanfattning
- Azure-användning efter geografiskt område
- Azure-användning

 > [!NOTE]
 > Den här rapporten är tillgänglig från Insights-instrumentpanelen. Om du vill visa den här rapporten måste du ha tilldelats en viss roll i Partnercenter, till exempel Global administratör, Kontoadministratör, Rapportvisare eller Rapportvisningsprogram. Mer information finns i företagets globala administratör. Specifika typer av data i den här rapporten kan också vara tillgängliga endast för användare med privilegier för visningsprogrammet för verkställande rapporter.

## <a name="summary"></a>Sammanfattning

I sammanfattningsavsnittet visas en ögonblicksbild av KPI:er (Key Performance Indicators) relaterade till Azure-prenumerationer som säljs eller hanteras av dig för dina kunder.  

- Azure-prenumerationer: Aktuellt antal Azure-kundprenumerationer som säljs eller hanteras av dig.
Procentuell tillväxt eller minskning av dessa Azure-prenumerationer under det valda datumintervallet.

Micro-diagrammet visar en månad för månad-trend för Antal Azure-prenumerationer för det valda datumintervallet.
- Aktiva Azure-prenumerationer: Det aktuella antalet Sålda eller hanterade Azure-prenumerationer som har haft aktiv användning under de senaste 30 dagarna.
Procentuell tillväxt eller minskning av dessa prenumerationer under det valda datumintervallet.

Micro-diagrammet visar en månad för månad-trend för antalet aktiva Azure-prenumerationer under det valda datumintervallet.

- Azure-intäktsförbrukning (ACR): Totalt Azure-intäktsförbrukning (US$) som du har tilldelats under det valda datumintervallet.
Procentuell tillväxt eller minskning av det tillskrivna ACR US$ under det valda datumintervallet. 

Micro-diagrammet visar en månatlig trend för ACR US$ som du har tilldelats under den valda tidsperioden


> [!NOTE]
 > Azure-intäktsförbrukning (ACR) är bara synligt för användare som har tilldelats rollen som visningsprogram för chefsrapport.

:::image type="content" source="images/pci/pci-azure-usage-summary-1.png" alt-text="Sammanfattning av Azure-användning":::

## <a name="azure-usage-by-geography"></a>Azure-användning per geografiskt område

Vyn **Azure-användning per geografi** visar den geografiska fördelningen av Azure-förbrukningsintäkter (ACR US$) eller användningstimmar för alla eller valda Azure-tjänstnivå-/mätarkategorier. Ljusare färger på kartan representerar lägre värden, medan mörkare färger representerar högre värden. Du kan söka efter och välja ett land i rutnätet för att zooma till 

I **tabellen Antal länder/regioner** visas det totala antalet länder/regioner där Azure-användningshändelser genereras.

Du kan söka efter och välja ett land i rutnätet för att zooma till platsen på kartan. Välj alternativet **Start** på kartan för att återgå till den ursprungliga vyn.

:::image type="content" source="images/pci/pci-azure-usage-by-geography-2.png" alt-text="Azure-användning per geografiskt område":::

## <a name="azure-utilization"></a>Azure-användning

Den här vyn visar trender för Azure-förbrukningsintäkter eller användningstimmar per månad efter valda Azure-tjänstnivå-/mätarkategorier. 

Stapeldiagrammet visar trenden för månatliga intäkter/användningstimmar. Linjediagrammet visar tillväxttrenden jämfört med föregående månad för de valda Azure-kategorierna för servicenivå/mätare.

:::image type="content" source="images/pci/pci-azure-usage-utilization-3.png" alt-text="Användning av Azure":::

## <a name="next-steps"></a>Nästa steg

- Fler rapporter finns i [Partner Center Insights](partner-center-insights.md).

>[!NOTE] 
> Du kan ladda ned rådata som driver den här rapporten från avsnittet Ladda ned rapporter på instrumentpanelen Insights. [Läs mer](pci-download-reports.md) 
