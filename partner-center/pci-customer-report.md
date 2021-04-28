---
title: Partner Center-insikter – kundrapport
ms.topic: article
ms.date: 06/16/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Upptäck sätt att förbättra din verksamhet. Se dina specifika kundtrender efter geografiskt område, efter produkt och andra attribut.
author: shthota77
ms.author: shthota
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 28343b5754546b653bd5a3e6b4a53a002b408668
ms.sourcegitcommit: 078eac1456f68585ff1003b21e5e1fe777af314b
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/28/2021
ms.locfileid: "108120842"
---
# <a name="customers-dashboard-reports-from-partner-center-insights"></a>Kunders instrumentpanelsrapporter från Partner Center Insights

**Lämpliga roller**

- Global administratör
- Administratörsagent
- Rapportvisningsprogram
- Rapportvisningsprogram för chefer

Instrumentpanelen Kunder visar data om dina kunder som antingen har köpt molnprodukter som Office, Azure, Dynamics osv. via dig eller använt dig för att distribuera och hantera dessa produkter i sina klienter. 
 
Instrumentpanelen Customers (Kunder) innehåller följande avsnitt: 

- Sammanfattning  
- Geografisk spridning för dina kunder 
- Kunder lägger till/omsättningstrender 
- Kundernas distribution efter partnerplatser, kundsegment, försäljningskanal, typ av partnerattribution 
- Kunddistribution efter produkt 
- Kundernas distributionstrender efter partnerplatser, kundsegment, prismodell, typ av partnerattribution 
- Trend för aktiva kunder 

## <a name="summary"></a>Sammanfattning

I sammanfattningsavsnittet visas en ögonblicksbild av olika KPI:er som är relaterade till dina kunder, till exempel kunder, aktiva kunder, prenumerationer, tillagda kunder, kunder som omsatts och kunder efter varje produkt. Sidnivåfilter gäller för varje avsnitt.

:::image type="content" source="images/pci/customerproduct.png" alt-text="Skärmbild av instrumentpanelen För kundsammanfattning som visar stapeldiagram och antalet kunder som är aktiva, nyligen tillagda, förlorade/omsatta eller efter specifik produkt.":::

### <a name="customers"></a>Kunder

- Det aktuella antalet kunder i din organisation är kopplat till olika attributionstyper för alla molnprodukter som Office, Azure och Dynamics. En kund räknas om de har minst en prenumeration med aktiv status.  
- Avböjning % av kunder under det valda datumintervallet 
- Mikrodiagram visar trenden månad för månad för antal kunder under det valda datumintervallet

### <a name="active-customers"></a>Aktiva kunder

- Aktuellt antal kunder med aktiv produktanvändning, till exempel aktiv användning på någon av molnprodukterna.
- Tillväxt eller minskning % av aktiva kunder under den valda tidsperioden
- Mikrodiagram visar en månad för månad-trend för antalet aktiva kunder under det valda datumintervallet.

### <a name="customers-added"></a>Kunder som har lagts till

- Antal kunder som lagts till under den valda tidsperioden.
- Tillväxt eller minskning % av kunder som lagts till under det valda sate-intervallet.
- Mikrodiagram visar trenden månad för månad för kunder som lagts till under det valda datumintervallet.

### <a name="customers-churned"></a>Kunder som har omsnat
- Antal kunder som omsörts varje månad under den valda tidsperioden. En kund anses vara förlorad om kunden inte har en enda prenumeration med aktiv status. 
- Procent av kunderna som omsattes under det valda datumintervallet 
- Mikrodiagram visar en månad för månad-trend för kunder som har omsörts under den valda tidsperioden 
 
### <a name="customers-by-products"></a>Kunder efter produkter

- Aktuellt antal kunder som distribuerats i olika molnprodukter som O365, Azure, Dynamics osv.  

## <a name="geographical-spread-of-your-customers"></a>Geografisk spridning för dina kunder

Antalet aktuella kunder, aktiva kunder och kunder som nyligen lagts till under det valda datumintervallet geo-mappas med hjälp av kundens land. Procentandelarna som visas under måttet visar det procentuella bidraget för det landet av totalsumman för måttet. Du kan hovra över kartan om du vill visa totalt antal aktiva, nya kunder för det landet. Du kan söka efter och välja ett land i rutnätet för att zooma till platsen på kartan. Återgå till den ursprungliga vyn genom att **välja** knappen Start på kartan. Alla kolumner i rutnätet är sorterbara.  

:::image type="content" source="images/pci/customersgeo.png" alt-text="Skärmbild av partnercenterinsikter, kundrapport efter geografiskt område, som visar världskarta och lista över totalt antal, tillagda och nya kunder efter region.":::

## <a name="customer-adds-and-churns"></a>Kunden lägger till och omsättningar

Trend för kunder med uppdelning i nya, befintliga och omsade för det valda datumintervallet. X-axeln representerar månader för det valda datumintervallet och Y-axeln representerar antalet kunder. Omsättningskunder representeras på negativ skala av Y-axeln. I ett staplat stapeldiagram visas en uppbrytning av nya, befintliga och kundomsättningar för månaden. Du kan återskapa stapeldiagrammet med specifika stackobjekt genom att välja dem i förklaringen. Du kan använda skjutreglaget överst i diagrammet för att zooma in till en viss punkt. 

:::image type="content" source="images/pci/customerslost.png" alt-text="Skärmbild av partnercenterinsiktskundrapporten med ett stapeldiagram som visar antalet kunder som har lagts till och förlorats eller omsatts under en viss tidsperiod.":::

## <a name="customer-distribution"></a>Kunddistribution

Uppdelning av dina aktuella kunder efter MPN-platser, kundsegment, försäljningskanal/Azure-prismodell och attributionstyp (till exempel DPOR, DAP). Välj respektive flikar ovanför diagrammet för att visa uppdelningen efter dessa kategorier. Du kan återskapa diagrammet genom att markera/avmarkera vissa dimensioner genom att välja förklaringsobjekten. 

## <a name="customers-by-products"></a>Kunder efter produkter

Uppdelning av antalet aktuella kunder efter produkter och SKU:er/planer. Välj en produkt i cirkeldiagrammet för produktbrytning för att visa uppbrytningen efter SKU:er/planer i diagrammet bredvid den.

:::image type="content" source="images/pci/customerbyprod.png" alt-text="Skärmbild av kunder efter produktrapport som visar två radiella diagram – ett med kunduppdelning efter produkt, det andra med kunduppdelning efter SKU.":::

## <a name="customer-distribution-trend"></a>Trend för kunddistribution 

Månatlig trend för kundernas fördelning under det valda datumintervallet efter marknader, segment, mpn-platser och produkter som de har köpt. Välj respektive flikar i diagrammet för att visa trenden efter dessa kategorier. X-axeln representerar månaderna för det datumintervall som du har valt och Y-axeln har antalet kunder för den valda kategorin (flikval). Du kan hovra över diagramkolumnerna för att visa värdena för varje stack. Du kan använda skjutreglaget överst i diagrammet för att zooma in på en viss punkt.   

:::image type="content" source="images/pci/customerdistri.png" alt-text="Skärmbild av rapporten Customer distribution trend (Trendrapport för kunddistribution) som visar stapeldiagram som du kan visa efter marknad, segment, partnerplats eller produkter.":::

## <a name="active-customers"></a>Aktiva kunder

Månatligt trenddiagram som jämför aktiva och totala kunder för det valda datumintervallet. Kolumner representerar aktiva kundantal varje månad och raden representerar det totala antalet kunder varje månad. 

:::image type="content" source="images/pci/activecustomer.png" alt-text="Skärmbild av partnercenterinsikter Aktiva kunders rapport som visar stapeldiagram över tid för aktiva kunder.":::

## <a name="next-steps"></a>Nästa steg

Fler rapporter finns i [Partner Center Insights](partner-center-insights.md).

>[!NOTE]
> Du kan ladda ned rådata som driver den här rapporten från avsnittet Ladda ned rapporter på Insights-instrumentpanelen. [Läs mer](pci-download-reports.md) 
