---
title: Partnercenter Insights Azure-användningsrapport
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-insights
description: Se vad du gör bra och var du kan förbättra din användning av Azure-prenumerationer som du säljer eller hanterar för dina kunder.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 56e58ba6ace5a7c64ec4ddfd1e76d33deace87fc
ms.sourcegitcommit: d731813da1d31519dc2dc583d17899e5cf4ec1b2
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/27/2021
ms.locfileid: "129070244"
---
# <a name="azure-usage-report-available-from-the-partner-center-insights-dashboard"></a>Azure-användningsrapport som är tillgänglig från Partnercenter Insights instrumentpanel

**Lämpliga roller:** Global | Administratörsagentens | Rapportvisningsprogram | Rapportvisningsprogram för chefer

Azure-användningsrapporten visar mått som rör dina kunders Azure-prenumerationer. Den här rapporten innehåller azure-förbrukningsintäkter och -användning per mätarkategorier. Du kan visa följande avsnitt från Azure-användningsrapporten.

- Sammanfattning
- Azure-användning per geografiskt område
- Azure-användning

 > [!NOTE]
 > Den här rapporten är tillgänglig från Insights instrumentpanel. Om du vill visa den här rapporten måste du ha tilldelats en viss roll i Partnercenter, till exempel Global administratör, Kontoadministratör, Rapportvisningsprogram eller Visningsprogram för verkställande rapporter. Mer information finns i företagets globala administratör. Specifika typer av data i den här rapporten kan också vara tillgängliga endast för användare med privilegier i visningsprogrammet för verkställande rapporter.

## <a name="summary"></a>Sammanfattning

I sammanfattningsavsnittet visas en ögonblicksbild av KPI:er (Key Performance Indicators) relaterade till Azure-prenumerationer som säljs eller hanteras av dig för dina kunder.  

- Azure-prenumerationer: Det aktuella antalet Azure-kundprenumerationer som sålts eller hanteras av dig.
Procentuell tillväxt eller minskning av dessa Azure-prenumerationer under det valda datumintervallet.

Micro-diagrammet visar en trend för azure-prenumerationer per månad för det valda datumintervallet.
- Aktiva Azure-prenumerationer: Det aktuella antalet Sålda eller hanterade Azure-prenumerationer som har varit aktiva under de senaste 30 dagarna.
Procentuell tillväxt eller minskning av dessa prenumerationer under det valda datumintervallet.

Micro-diagrammet visar en trend för månad över månad för antalet aktiva Azure-prenumerationer under det valda datumintervallet.

- Azure-intäktsförbrukning (ACR): Totalt Azure-intäktsförbrukning (US$) som du har tilldelats under det valda datumintervallet.
Procentuell tillväxt eller minskning av det tillskrivna ACR US$ under det valda datumintervallet. 

Micro-diagrammet visar en månatlig trend för ACR US$ som tillskrivs dig under den valda tidsperioden


> [!NOTE]
 > Azure-intäktsförbrukning (ACR) är endast synligt för användare som har tilldelats rollen Som chef för rapportvisning.

:::image type="content" source="images/insights/azure-usage-summary.png" alt-text="Azure-användningssammanfattning.":::

## <a name="azure-usage-by-geography"></a>Azure-användning per geografiskt område

Vyn **Azure-användning per geografi** visar den geografiska fördelningen av Azure-förbrukningsintäkter (ACR US$) eller användningstimmar för alla eller valda Azure-tjänstnivå-/mätarkategorier. Ljusare färger på kartan representerar lägre värden, medan mörkare färger representerar högre värden. Du kan söka efter och välja ett land i rutnätet för att zooma till 

I **tabellen Antal länder/regioner** visas det totala antalet länder/regioner där Azure-användningshändelser genereras.

Du kan söka efter och välja ett land i rutnätet för att zooma till platsen på kartan. Välj alternativet **Start** på kartan för att återgå till den ursprungliga vyn.

:::image type="content" source="images/insights/azure-usage-by-geography.png" alt-text="Azure-användning per geografiskt område.":::

## <a name="azure-utilization"></a>Azure-användning

Den här vyn visar trender för Azure-förbrukningsintäkter eller användningstimmar per månad efter valda Azure-tjänstnivå-/mätarkategorier. 

Stapeldiagrammet visar trenden för månatliga intäkter/användningstimmar. Linjediagrammet visar tillväxttrenden jämfört med föregående månad för de valda Azure-kategorierna för servicenivå/mätare.

:::image type="content" source="images/insights/azure-usage-utilization.png" alt-text="Användning av Azure.":::

## <a name="next-steps"></a>Nästa steg

- Fler rapporter finns i [Partnercenter Insights](partner-center-insights.md).

>[!NOTE] 
> Du kan ladda ned rådata som driver den här rapporten från avsnittet Ladda ned rapporter i Insights instrumentpanel. [Läs mer](insights-download-reports.md) 
