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
ms.openlocfilehash: cd302a7b4839b98cdd96fda38b381d9282b00620
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/17/2021
ms.locfileid: "112275999"
---
# <a name="azure-usage-report-available-from-the-partner-center-insights-dashboard"></a>Azure-användningsrapport som är tillgänglig från instrumentpanelen i PartnerCenter Insights

**Lämpliga roller:** Global | Administratörsagent | Rapportvisningsprogram | Rapportvisningsprogram för chefer

Azure-användningsrapporten visar mått som är relaterade till dina kunders Azure-prenumerationer. Den här rapporten innehåller azure-förbrukningsintäkter och -användning per mätarkategorier. Du kan visa följande avsnitt från Azure-användningsrapporten.

- Sammanfattning
- Azure-användning per geografiskt område
- Azure-användning

 > [!NOTE]
 > Den här rapporten är tillgänglig från instrumentpanelen Insights. Om du vill visa den här rapporten måste du ha tilldelats en viss roll i Partnercenter, till exempel Global administratör, Kontoadministratör, Rapportvisningsprogram eller Visningsprogram för verkställande rapporter. Mer information finns i företagets globala administratör. Specifika typer av data i den här rapporten kan också vara tillgängliga endast för användare med privilegier i visningsprogrammet för verkställande rapporter.

## <a name="summary"></a>Sammanfattning

I sammanfattningsavsnittet visas en ögonblicksbild av KPI:er (Key Performance Indicators) relaterade till Azure-prenumerationer som säljs eller hanteras av dig för dina kunder.  

- Azure-prenumerationer: Det aktuella antalet Azure-kundprenumerationer som sålts eller hanteras av dig.
Procentuell tillväxt eller minskning av dessa Azure-prenumerationer under det valda datumintervallet.

Micro-diagrammet visar en trend för månad för månad för antal Azure-prenumerationer för det valda datumintervallet.
- Aktiva Azure-prenumerationer: Det aktuella antalet Sålda eller hanterade Azure-prenumerationer som har varit aktiva under de senaste 30 dagarna.
Procentuell tillväxt eller minskning av dessa prenumerationer under det valda datumintervallet.

Micro-diagrammet visar en trend för månad över månad för antalet aktiva Azure-prenumerationer under det valda datumintervallet.

- Azure-intäktsförbrukning (ACR): Totalt Azure-intäktsförbrukning (US$) som du har tilldelats under det valda datumintervallet.
Procentuell tillväxt eller minskning av det tillskrivna ACR US$ under det valda datumintervallet. 

Micro-diagrammet visar en månatlig trend för ACR US$ som du har tilldelats under den valda tidsperioden


> [!NOTE]
 > Azure-intäktsförbrukning (ACR) är bara synligt för användare som har tilldelats rollen som visningsprogram för chefsrapport.

:::image type="content" source="images/pci/pci-azure-usage-summary-1.png" alt-text="Azure-användningssammanfattning.":::

## <a name="azure-usage-by-geography"></a>Azure-användning per geografiskt område

Vyn **Azure-användning per geografi** visar den geografiska fördelningen av Azure-förbrukningsintäkter (ACR US$) eller användningstimmar för alla eller valda Azure-tjänstnivå-/mätarkategorier. Ljusare färger på kartan representerar lägre värden, medan mörkare färger representerar högre värden. Du kan söka efter och välja ett land i rutnätet för att zooma till 

I **tabellen Antal länder/regioner** visas det totala antalet länder/regioner där Azure-användningshändelser genereras.

Du kan söka efter och välja ett land i rutnätet för att zooma till platsen på kartan. Välj alternativet **Start** på kartan för att återgå till den ursprungliga vyn.

:::image type="content" source="images/pci/pci-azure-usage-by-geography-2.png" alt-text="Azure-användning per geografiskt område.":::

## <a name="azure-utilization"></a>Azure-användning

Den här vyn visar trender för Azure-förbrukningsintäkter eller användningstimmar per månad efter valda Azure-tjänstnivå-/mätarkategorier. 

Stapeldiagrammet visar trenden för månatliga intäkter/användningstimmar. Linjediagrammet visar tillväxttrenden jämfört med föregående månad för de valda Azure-kategorierna för servicenivå/mätare.

:::image type="content" source="images/pci/pci-azure-usage-utilization-3.png" alt-text="Användning av Azure.":::

## <a name="next-steps"></a>Nästa steg

- Fler rapporter finns i [Partner Center Insights.](partner-center-insights.md)

>[!NOTE] 
> Du kan ladda ned rådata som driver den här rapporten från avsnittet Ladda ned rapporter på instrumentpanelen Insights. [Läs mer](pci-download-reports.md) 
