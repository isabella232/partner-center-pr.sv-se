---
title: Prestanda instrument panel för partner Center Insights-insikter
ms.topic: article
ms.date: 09/01/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Instrument panelen för åter försäljaren i partners insikter ger en översikt över prestanda för olika indirekta åter försäljare av en indirekt CSP-Provider.
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 94cf24309486628d92878e0d8d5038b45c7b85df
ms.sourcegitcommit: eef446698ed4e21afee7fe091fe9c2664767755c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/01/2020
ms.locfileid: "92531328"
---
# <a name="reseller-performance-dashboard-in-partner-center-insights"></a>Åter försäljares prestanda instrument panel i Partner Center Insights

**Lämpliga roller**

- Global administratör
- Administratörs agent
- Rapport visnings program
- Rapport visnings program för chefer

Instrument panelen för åter försäljaren i partners insikter ger en översikt över prestanda för olika indirekta åter försäljare av en indirekt CSP-Provider. Instrument panelen tillhandahåller data på de åter försäljare som är aktiva, hur mycket som de genererar och vilka produkter som driver intäkterna. Indirekta leverantörer kommer att kunna söka efter en speciell åter försäljare efter namn och söka efter information om åter försäljaren i instrument panelen för åter försäljaren.

Du kan visa följande avsnitt från instrument panelen för åter försäljares prestanda.

- Sammanfattning
- Geografiskt spridning av åter försäljare
- Åter försäljare Lägg till/omsättning 
- Intäkts trend för åter försäljare 
- Åter försäljar prestanda efter produkter
- Aktiva åter försäljare efter partner platser
- Trend för intäkts geo-distribution
- Åter försäljarens prestanda per kund segment
- Försäljarens status för MPA-signering

 > [!NOTE]
 > Den här rapporten är tillgänglig från insikts instrument panelen. Om du vill visa den här rapporten måste du ha tilldelats en speciell roll i Partner Center, till exempel global administratör, konto administratör, rapport visnings program eller Executive Report Viewer. Mer information finns i företagets globala administratör. vissa typer av data i den här rapporten kan också endast vara tillgängliga för användare med behörigheten Executive Report Viewer.

## <a name="summary"></a>Sammanfattning

Avsnittet Sammanfattning visar en ögonblicks bild av KPI: erna (nyckeltal) som relaterar till den indirekta CSP-providern.

- Aktiva åter försäljare: antal åter försäljare som har minst en aktiv prenumeration under den månaden.

Micro-diagrammet presenterar den månads Visa månads trenden för distinkta åter försäljare som har varit aktiva under det valda datum intervallet.

- Att handla åter försäljare: antal åter försäljare som sålde minst en prenumeration under den månaden. 

Micro-diagrammet presenterar månads Visa trend för åter försäljare som registrerats för det valda datum intervallet.

- Nya åter försäljare: antal åter försäljare som började interagera med den indirekta providern under den månaden. 

Micro-diagrammet presenterar den månads Visa månads trenden för det totala antalet nya åter försäljare under det valda datum intervallet.

- Fakturerad intäkt USD: intäkter i USD som sköts av åter försäljarna under den månaden. 

Micro-diagrammet presenterar månads månads trenden för intäkter under det valda datum intervallet.

- I avsnittet fakturerad intäkt per produkt visas en månads analys av den fakturerade intäkten i USD, dela efter sålda produkter. 

:::image type="content" source="images/pci/pci-res-perf-summary-1.png" alt-text="prestanda Sammanfattning för åter försäljare":::

## <a name="geographical-spread-of-resellers"></a>Geografiskt spridning av åter försäljare

Vyn * * åter försäljare per geografi tillhandahåller den geografiska distributionen av åter försäljare. Med den här widgeten kan partners Visa totala **åter försäljare** , **nya åter försäljare** och **fakturerade intäkter (USD)** , delade efter olika geografiska områden.

Du kan söka efter och välja ett land i rutnätet för att zooma till platsen i kartan. Tryck på **Start** alternativet på kartan för att återgå till den ursprungliga vyn. Hovra över kartan för att visa den **fakturerade intäkten (USD)** efter land. Fältet fakturerad intäkt (USD) i rutnätet är sorterbart.

:::image type="content" source="images/pci/pci-res-perf-resel-by-geo-1.png" alt-text="prestanda Sammanfattning för åter försäljare":::

## <a name="resellers-addchurns"></a>Åter försäljare Lägg till/omsättning

I den här vyn visas månads fördelningen av antalet **nya åter försäljare** , uppdelade **åter försäljare** och **befintliga åter försäljare** . 

- Nya åter försäljare: antal åter försäljare som nyligen har registrerats med den indirekta providern under det valda datum intervallet.
- Omsättnings bara åter försäljare: antal åter försäljare som inte hade någon transaktion under de senaste sex månaderna exklusive den aktuella månaden.
- Befintliga åter försäljare: antal åter försäljare som var i föregående månad.

:::image type="content" source="images/pci/pci-res-perf-resel-add-churn-1.png" alt-text="prestanda Sammanfattning för åter försäljare":::

## <a name="resellers-revenue-trend"></a>Intäkts trend för åter försäljare 

Den här vyn ger en månatlig trend för de fakturerade intäkterna (USD) som delas av produkter, nämligen O365, D365, EMS, Power BI och Azure. De allmänna måtten sammanställs i de olika produkterna för varje månad. Partnern kan söka efter en speciell åter försäljare efter namn och söka efter data för den aktuella åter försäljaren. Fältet fakturerad intäkt (USD) i rutnätet är sorterbart.

:::image type="content" source="images/pci/pci-res-perf-resel-rev-trend-1.png" alt-text="prestanda Sammanfattning för åter försäljare":::

## <a name="reseller-performance-by-products"></a>Åter försäljar prestanda efter produkter

Den här vyn ger en uppdelning av viktiga mått som fakturerad intäkt, antalet prenumerationer och antalet licenser av olika produkter per månad månads vis. Cirkel diagrammet till höger visar den övergripande delningen av dessa mått av olika produkter, så att partnern får en snabb översikt över bruten av olika produkter som åter försäljaren säljer.

:::image type="content" source="images/pci/pci-res-perf-resel-perf-product-1.png" alt-text="prestanda Sammanfattning för åter försäljare":::

## <a name="active-resellers-by-partner-locations"></a>Aktiva åter försäljare efter partner platser

Den här vyn ger en uppdelning av aktiva åter försäljare efter partner geografiska områden. De fem främsta diagrammen visas i förklaringen och de återstående kategoriseras som "andra".

:::image type="content" source="images/pci/pci-res-perf-part-loc-1.png" alt-text="prestanda Sammanfattning för åter försäljare":::

## <a name="revenue-geo-distribution-trend"></a>Trend för intäkts geo-distribution

I den här vyn visas månads trenden för den fakturerade intäkten (USD) som delas av de fem främsta diagrammen.  Resten av intäkterna kategoriseras som "andra".

:::image type="content" source="images/pci/pci-res-perf-rev-geo-trend-1.png" alt-text="prestanda Sammanfattning för åter försäljare":::

## <a name="reseller-performance-by-customer-segment"></a>Åter försäljarens prestanda per kund segment

I den här vyn kan en partner förstå månads trenden för intäkter per månad, antal prenumerationer och licenser, delas av olika kund segment. De fem främsta kund segmenten visas i diagrammet och de återstående kategoriseras som "andra".

:::image type="content" source="images/pci/pci-res-perf-resel-cust-seg-1.png" alt-text="prestanda Sammanfattning för åter försäljare":::

## <a name="reseller-mpa-signing-status"></a>Försäljarens status för MPA-signering

Den här vyn visar status för MPA-signering för åter försäljare tillsammans med ytterligare metadata, till exempel MPN först konsumentsajter status, PMC till PC migration status osv.

:::image type="content" source="images/pci/pci-res-perf-mpa-stat-1.png" alt-text="prestanda Sammanfattning för åter försäljare":::

## <a name="next-steps"></a>Nästa steg

- Mer information finns i [partner Center Insights](partner-center-insights.md).

>[!NOTE] 
> Du kan ladda ned rå data från den här rapporten från avsnittet hämta rapporter på instrument panelen insikter. [Läs mer](pci-download-reports.md) 
