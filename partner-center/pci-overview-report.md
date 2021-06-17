---
title: Översikt över Instrumentpanel för Partnercenter-insikter
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Se en ögonblicksbild av hur det går för dig med försäljning och distribution, kundtillväxt och intäktstillväxt med licenser, prenumerationer och Azure-förbrukning.
author: shthota77
ms.author: shthota
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: aea78f2a9b60f5d8adcc7962d15749479424c9f1
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/17/2021
ms.locfileid: "112277495"
---
# <a name="overview-dashboard-reports-available-in-partner-center-insights"></a>Översikt över instrumentpanelsrapporter som är tillgängliga i Partner Center Insights
 
**Lämpliga roller:** Globala | Administratörsagent | Rapportvisningsprogram | Visningsprogram för exekutiv rapport

Instrumentpanelen Insights Overview (Översikt över insikter) innehåller en ögonblicksbild av kpi:er som kunder, prenumerationer, Azure-förbrukningsintäkter och licenser. Du kan visualisera följande diagram i översiktsrapporten.

- Sammanfattning  
- Geografisk spridning av dina kunder, prenumerationer och licenser  
- Kundtillväxttrend 
- Trend för prenumerationstillväxt 
- Trend för tillväxt av förbrukade Azure-intäkter 
- Trend för licenstillväxt 

## <a name="summary"></a>Sammanfattning

Sammanfattningen innehåller information om kunder, Azure-intäktsförbrukning (ACR), sålda prenumerationer, aktiva prenumerationer och distribuerade licenser. 

:::image type="content" source="images/pci/summary.png" alt-text="Sammanfattningslicenser.":::

Mer information om varje avsnitt i sammanfattningen följer.

### <a name="customers"></a>Kunder

Området **Kunder** innehåller:

- Det aktuella antalet kunder med minst en aktiv prenumeration som är associerad med ditt företag via olika attributionstyper och för alla molnprodukter.
- Kundernas procentuella tillväxt under det valda datumintervallet.
- Mikrodiagrammet visar trenden månad för månad för antalet kunder inom det valda datumintervallet.

### <a name="azure-consumed-revenue-acr"></a>Azure-intäktsförbrukning (ACR)

Området **Azure-intäktsförbrukning (ACR)** i sammanfattningen innehåller:

- Det totala Azure-intäktsförbrukning (i USA $) som du har tilldelats under det valda datumintervallet.
- Den procentuella tillväxten eller minskningen i det tillskrivna ACR (i US $) under det valda datumintervallet.
- Mikrodiagrammet visar en månatlig trend för ACR US$ som tilldelats dig över det valda datumintervallet 

> [!NOTE]
> Azure-intäktsförbrukning (ACR)-data är tillgängliga för användare som har tilldelats rollen Som chef för rapportvisning 
 
### <a name="subscriptions-sold"></a>Sålda prenumerationer

Området **Sålda prenumerationer** i sammanfattningen innehåller:

- Det totala antalet molnproduktprenumerationer (aktiva och inaktiva) som sålts eller hanteras av dig.  
- Den procentuella tillväxten eller minskningen i prenumerationer under det valda datumintervallet.
- Mikrodiagrammet visar trenden månad för månad för totalt antal prenumerationer under det valda datumintervallet.

### <a name="active-subscriptions"></a>Aktiva prenumerationer

Området **Aktiva prenumerationer** i sammanfattningen innehåller:

- Det aktuella antalet molnproduktprenumerationer med aktiv användning mätt baserat på produkttelemetri. Detta exkluderar alla utvärderingsprenumerationer för Azure-prenumerationer.  
- Procentandelen ökning av aktiva prenumerationer under det valda datumintervallet.
- Mikrodiagrammet visar trenden månad för månad för aktiva prenumerationer under det valda datumintervallet.
 
### <a name="licenses-deployed"></a>Distribuerade licenser

Området **Licenser som distribueras** i sammanfattningen innehåller:
 
- Antalet molnproduktlicenser som distribuerats i dina kundprenumerationer under den valda tidsperioden. 
- Den procentuella tillväxten eller minskningen i dessa licenser under det valda datumintervallet. 
- Mikrodiagrammet visar trenden månad för månad för dessa tilldelade licenser under det valda datumintervallet.

## <a name="geographical-spread-of-your-customers-subscriptions-and-licenses"></a>Geografisk spridning av dina kunder, prenumerationer och licenser

Den här vyn är en geografisk fördelning av totalt antal kunder, prenumerationer och licenser per kundland. Välj de olika flikarna för att visa var och en av dessa insikter på kartan. Du kan söka efter och välja ett land i rutnätet för att zooma till platsen på kartan. Återgå till den ursprungliga vyn genom att trycka på knappen Start på kartan. Om du klickar på varje flik (till exempel Kunder, Prenumerationer) visas måttvärdet för varje land och procent av Total för landet.  

:::image type="content" source="images/pci/geosummary.png" alt-text="Geografisk sammanfattning.":::

## <a name="customers-growth-trend"></a>Kundtillväxttrend

Månatlig trend för totalt antal kunder för det valda datumintervallet. X-axeln representerar månader för det valda datumintervallet och Y-axeln representerar det totala kundantalet för den månaden. 

:::image type="content" source="images/pci/customergrowth.png" alt-text="kundtillväxttrend.":::

## <a name="subscriptions-growth-trend"></a>Trend för prenumerationstillväxt

Detta anger trenden för antalet kundprenumerationer för det valda datumintervallet. X-axeln representerar månader för det valda datumintervallet och Y-axeln representerar antalet prenumerationer för den produkt som har valts. Rulla igenom skjutreglaget överst i diagrammet för att zooma diagrammet till en viss tidsperiod. 

:::image type="content" source="images/pci/subscriptiongrowth.png" alt-text="Trend för prenumerationstillväxt.":::

## <a name="azure-consumed-revenue-growth-trend"></a>Azure-intäktsförbrukning tillväxttrend

Månadstrend för Azure-förbrukade intäkter US$ som har tilldelats dig under det valda datumintervallet. X-axeln representerar månader för det valda datumintervallet och Y-axeln representerar den totala Azure-förbrukade intäkten US$ som du har tilldelats under månaden.

> [!NOTE]
> Azure-intäktsförbrukning (ACR) är bara synligt för användare som har tilldelats rollen Visningsprogram för verkställande rapporter. 

:::image type="content" source="images/pci/azureconsumed.png" alt-text="Azure-förbrukning.":::

## <a name="licenses-growth-trend"></a>Trend för licenstillväxt
 
Trend för licenser som tilldelats av alla kunder under det valda datumintervallet. X-axeln representerar månader för det valda datumintervallet och Y-axeln representerar antalet licenser för den produkt som du har valt. Rulla igenom skjutreglaget överst i diagrammet för att zooma diagrammet till en viss tidsperiod.  

:::image type="content" source="images/pci/licensesgrowth.png" alt-text="Licenser.":::

## <a name="next-steps"></a>Nästa steg

Fler rapporter finns i [Partner Center Insights](partner-center-insights.md).
