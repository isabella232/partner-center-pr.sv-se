---
title: Instrumentpanel för Insights partnercenter
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-insights
description: Se en ögonblicksbild av hur det går med försäljning och distribution, kundtillväxt och intäktstillväxt med licenser, prenumerationer och Azure-förbrukning.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 439d49a7286ae9a2a1d61a088d86ec32b3f8fcb5
ms.sourcegitcommit: d731813da1d31519dc2dc583d17899e5cf4ec1b2
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/27/2021
ms.locfileid: "129071879"
---
# <a name="overview-dashboard-reports-available-in-partner-center-insights"></a>Översikt över instrumentpanelsrapporter som är tillgängliga i Partnercenter Insights
 
**Lämpliga roller:** Global | Administratörsagentens | Rapportvisningsprogram | Rapportvisningsprogram för chefer

Instrumentpanelen Insights Översikt innehåller en ögonblicksbild av KPI:er (Key Performance Indicators), till exempel kunder, prenumerationer, Azure-förbrukningsintäkter och licenser. Du kan visualisera följande diagram i översiktsrapporten.

- Sammanfattning  
- Geografisk spridning av dina kunder, prenumerationer och licenser  
- Kunders tillväxttrend 
- Trend för prenumerationstillväxt 
- Trend för intäktstillväxt i Azure 
- Trend för licenstillväxt 

## <a name="summary"></a>Sammanfattning

Sammanfattningen innehåller information om kunder, Azure-intäktsförbrukning (ACR), sålda prenumerationer, aktiva prenumerationer och distribuerade licenser. 

:::image type="content" source="images/insights/summary.png" alt-text="Sammanfattningslicenser.":::

Mer information om varje avsnitt i sammanfattningen följer.

### <a name="customers"></a>Kunder

Området **Kunder** innehåller:

- Det aktuella antalet kunder med minst en aktiv prenumeration som är associerad med ditt företag via olika attributionstyper och över alla molnprodukter.
- Kundernas procentuella tillväxt under det valda datumintervallet.
- Mikrodiagrammet visar trenden för antalet kunder under månaden inom det valda datumintervallet.

### <a name="azure-consumed-revenue-acr"></a>Azure-intäktsförbrukning (ACR)

Området **Azure-intäktsförbrukning (ACR)** i sammanfattningen innehåller:

- Det totala ACR (i amerikanska dollar) som du har tilldelats under det valda datumintervallet.
- Den procentuella tillväxten eller minskningen i ACR (i amerikanska dollar) under det valda datumintervallet.
- Mikrodiagrammet visar en månatlig trend för ACR i amerikanska dollar som har tilldelats dig under det valda datumintervallet 

> [!NOTE]
> ACR-data är tillgängliga för användare som har tilldelats rollen Som chef för rapportvisning.
 
### <a name="subscriptions-sold"></a>Sålda prenumerationer

Området **Prenumerationer sålda** i sammanfattningen innehåller:

- Det totala antalet molnproduktprenumerationer (aktiva och inaktiva) som sålts eller hanteras av dig.  
- Den procentuella tillväxten eller minskningen i prenumerationer under det valda datumintervallet.
- Mikrodiagrammet visar trenden månad för månad för totalt antal prenumerationer under det valda datumintervallet.

### <a name="active-subscriptions"></a>Aktiva prenumerationer

Området **Aktiva prenumerationer** i sammanfattningen innehåller:

- Det aktuella antalet molnproduktprenumerationer med aktiv användning mätt baserat på produkttelemetri. Detta exkluderar alla Azure-utvärderingsprenumerationer.  
- Procentandelen ökning av aktiva prenumerationer under det valda datumintervallet.
- Mikrodiagrammet visar trenden för aktiva prenumerationer under månaden över det valda datumintervallet.
 
### <a name="licenses-deployed"></a>Distribuerade licenser

Området **Licenser som distribueras** i sammanfattningen innehåller:
 
- Antalet molnproduktlicenser som distribuerats i dina kundprenumerationer under den valda tidsperioden. 
- Den procentuella tillväxten eller minskningen i dessa licenser under det valda datumintervallet. 
- Mikrodiagrammet visar trenden månad för månad för dessa tilldelade licenser under det valda datumintervallet.

## <a name="geographical-spread-of-your-customers-subscriptions-and-licenses"></a>Geografisk spridning av dina kunder, prenumerationer och licenser

Den här vyn är en geografisk distribution av totalt antal kunder, prenumerationer och licenser efter kundland. Välj de olika flikarna för att visa var och en av dessa insikter på kartan. Du kan söka efter och välja ett land i rutnätet för att zooma till platsen på kartan. Återgå till den ursprungliga vyn genom att trycka på knappen Start på kartan. Om du klickar på varje flik (till exempel Kunder, Prenumerationer) visas måttvärdet för varje land och procent av Total för landet.  

:::image type="content" source="images/insights/geosummary.png" alt-text="Geografisk sammanfattning.":::

## <a name="customers-growth-trend"></a>Kunders tillväxttrend

Månatlig trend för totalt antal kunder för det valda datumintervallet. X-axeln representerar månader för det valda datumintervallet och Y-axeln representerar det totala kundantalet för den månaden. 

:::image type="content" source="images/insights/customer-growth.png" alt-text="kunders tillväxttrend.":::

## <a name="subscriptions-growth-trend"></a>Trend för prenumerationstillväxt

Detta anger trenden för antalet kundprenumerationer för det valda datumintervallet. X-axeln representerar månader för det valda datumintervallet och Y-axeln representerar antalet prenumerationer för den produkt som har valts. Bläddra igenom skjutreglaget överst i diagrammet för att zooma diagrammet till en viss tidsperiod. 

:::image type="content" source="images/insights/subscription-growth.png" alt-text="Trend för prenumerationstillväxt.":::

## <a name="azure-consumed-revenue-growth-trend"></a>Azure-intäktsförbrukning tillväxttrend

Månatlig trend för Azure-förbrukade intäkter i amerikanska dollar som tillskrivs dig under det valda datumintervallet. X-axeln representerar månader för det valda datumintervallet och Y-axeln representerar de totala Azure-förbrukade intäkterna i amerikanska dollar som du har tilldelats under månaden.

> [!NOTE]
> ACR är endast synligt för användare som har tilldelats rollen som visningsprogram för chefsrapport. 

:::image type="content" source="images/insights/azure-consumed.png" alt-text="Azure-förbrukning.":::

## <a name="licenses-growth-trend"></a>Trend för licenstillväxt
 
Trend för licenser som tilldelats av alla kunder under det valda datumintervallet. X-axeln representerar månader för det valda datumintervallet och Y-axeln representerar antalet licenser för den produkt som du har valt. Bläddra igenom skjutreglaget överst i diagrammet för att zooma diagrammet till en viss tidsperiod.  

:::image type="content" source="images/insights/licenses-growth.png" alt-text="Licenser.":::

## <a name="next-steps"></a>Nästa steg

Fler rapporter finns i [Partnercenter Insights](partner-center-insights.md).
