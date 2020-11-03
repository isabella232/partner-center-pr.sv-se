---
title: Översikts instrument panel för partner Center Insights
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Se en ögonblicks bild av hur du gör med försäljning och distribution, kund tillväxt och inkomst tillväxt med licenser, prenumerationer och Azure-förbrukning.
author: shthota77
ms.author: shthota
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 91075e8aab1759904a1549dd38bee6fb886c1c65
ms.sourcegitcommit: 5f31146f50e01dc4c1922e0a5bc369f0a3cd8162
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/01/2020
ms.locfileid: "92531305"
---
# <a name="overview-dashboard-reports-available-in-partner-center-insights"></a>Översikt över instrument panels rapporter i Partner Center Insights
 
Instrument panelen översikt över insikter innehåller en Snapshot-vy över nyckeltal för nyckeltal, till exempel kunder, prenumerationer, Azures förbruknings intäkter, licenser osv. Du kan visualisera följande diagram i översikts rapporten.

- Sammanfattning  
- Geografisk spridning av kunder, prenumerationer och licenser  
- Tillväxt trend för kunder 
- Trend för prenumerations tillväxt 
- Tillväxt trend för förbrukade Azure-intäkter 
- Tillväxt trend för licenser 

## <a name="summary"></a>Sammanfattning

Sammanfattningen innehåller information om kunder, förbrukade intäkter i Azure (ACR), prenumerationer som säljs, aktiva prenumerationer och distribuerade licenser. 

:::image type="content" source="images/pci/summary.png" alt-text="Sammanfattnings licenser":::

Se nedan för mer information om varje del av sammanfattningen.

### <a name="customers"></a>Kunder

I avsnittet **kunder** finns:

- Aktuellt antal kunder med minst en aktiv prenumeration som är kopplad till ditt företag via olika typer av behörighet och alla moln produkter.
- Kundernas procentuella tillväxt under det valda datum intervallet.
- Micro-diagrammet presenterar månads månaders trenden för kund antalet inom det valda datum intervallet.

### <a name="azure-consumed-revenue-acr"></a>Förbrukade intäkter i Azure (ACR)

I **ACR-ytan (Azure förbrukade intäkter)** i sammanfattningen ingår:

- Den totala förbrukade omsättningen i Azure (i USA $) till dig under det valda datum intervallet.
- Procentuell tillväxt eller neka i attributed ACR (i USA $) under det valda datum intervallet.
- Micro-diagrammet presenterar en månatlig trend för ACR US $ som är tilldelad dig över det valda datum intervallet 

> [!NOTE]
> ACR-data (Azure förbrukade intäkter) är tillgängliga för användare som har tilldelats rollen Executive Report Viewer 
 
### <a name="subscriptions-sold"></a>Sålda prenumerationer

I avsnittet **prenumerationer som säljs** i sammanfattningen ingår:

- Det totala aktuella antalet moln produkt prenumerationer (aktiva och inaktiva) som säljs eller hanteras av dig.  
- Procent andelen växer eller nekas i prenumerationer under det valda datum intervallet.
- Micro-diagrammet presenterar den månads Visa månads trenden för totala prenumerationer under det valda datum intervallet.

### <a name="active-subscriptions"></a>Aktiva prenumerationer

Det **aktiva prenumerations** avsnittet i sammanfattningen innehåller:

- Aktuellt antal moln produkt prenumerationer med aktiv användning mätt baserat på produkt telemetri. Detta utesluter alla utvärderings prenumerationer om Azure-prenumerationer.  
- Procentuell ökning av aktiva prenumerationer under det valda datum intervallet.
- Micro-diagrammet presenterar den månads Visa månads trend för aktiva prenumerationer under det valda datum intervallet.
 
### <a name="licenses-deployed"></a>Distribuerade licenser

I avsnittet **licenser som distribueras** i sammanfattningen ingår:
 
- Antalet moln produkt licenser som har distribuerats i dina kund prenumerationer under den valda tids perioden. 
- Procent andelen tillväxt eller neka i de här licenserna under det valda datum intervallet. 
- Micro-diagrammet visar månads trenden för de tilldelade licenserna över det valda datum intervallet.

## <a name="geographical-spread-of-your-customers-subscriptions-and-licenses"></a>Geografisk spridning av kunder, prenumerationer och licenser

Den här vyn är en geografisk fördelning av totala kunder, prenumerationer och licenser per kund land. Klicka på de olika flikarna om du vill visa var och en av dessa insikter på kartan. Du kan söka efter och välja ett land i rutnätet för att zooma till platsen i kartan. Återgå till den ursprungliga vyn genom att trycka på knappen Start på kartan. Om du klickar på varje flik (t. ex. kunder, prenumerationer) visas värdet för måttet för varje land samt% av summan för landet.  

:::image type="content" source="images/pci/geosummary.png" alt-text="Sammanfattnings licenser":::

## <a name="customers-growth-trend"></a>Tillväxt trend för kunder

Månatlig trend per månad av totalt antal kunder för det valda datum intervallet. X-axeln representerar månader i det valda datum intervallet och Y-axeln representerar det totala antalet kunder för den månaden. 

:::image type="content" source="images/pci/customergrowth.png" alt-text="Sammanfattnings licenser":::

## <a name="subscriptions-growth-trend"></a>Trend för prenumerations tillväxt

Detta anger trenden för antalet kund prenumerationer för det valda datum intervallet. X-axeln representerar månader i det valda datum intervallet och Y-axeln representerar antalet prenumerationer för produkten som har valts. Rulla genom skjutreglaget ovanpå diagrammet för att zooma diagrammet till en viss tids period. 

:::image type="content" source="images/pci/subscriptiongrowth.png" alt-text="Sammanfattnings licenser":::

## <a name="azure-consumed-revenue-growth-trend"></a>Tillväxt trend för förbrukade Azure-intäkter

Månatlig trend för förbrukade intäkter från Azure till dig under det valda datum intervallet. X-axeln representerar månader i det valda datum intervallet och Y-axeln visar den totala förbrukade intäkterna från Azure till dig under månaden.

> [!NOTE]
> Azures förbrukade intäkter (ACR) visas bara för användare som har tilldelats rollen Executive Report Viewer. 

:::image type="content" source="images/pci/azureconsumed.png" alt-text="Sammanfattnings licenser":::

## <a name="licenses-growth-trend"></a>Tillväxt trend för licenser
 
Trenden för licenser som har tilldelats av alla kunder under det valda datum intervallet. X-axeln representerar månader i det valda datum intervallet och Y-axeln representerar antalet licenser för den produkt som du har valt. Rulla genom skjutreglaget ovanpå diagrammet för att zooma diagrammet till en viss tids period.  

:::image type="content" source="images/pci/licensesgrowth.png" alt-text="Sammanfattnings licenser":::

## <a name="next-steps"></a>Nästa steg

Mer information finns i [partner Center Insights](partner-center-insights.md).
