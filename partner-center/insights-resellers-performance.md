---
title: Partner Center Insights Resellers Performance-instrumentpanel
ms.topic: article
ms.date: 09/01/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Instrumentpanelen för återförsäljares prestanda i Partnercenter Insights ger en översikt över prestandan för olika indirekta återförsäljare av en indirekt leverantör Molnlösningsleverantör en leverantör av Molnlösningsleverantör (CSP).
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: c8fc28730fecdd97928159cef3f0c48a6eeda1f5
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 07/16/2021
ms.locfileid: "114376910"
---
# <a name="reseller-performance-dashboard-in-partner-center-insights"></a>Instrumentpanelen Reseller Performance i Partner Center Insights

**Lämpliga roller:** Globala | Administratörsagent | Rapportvisningsprogram | Visningsprogram för exekutiv rapport

Instrumentpanelen för återförsäljares prestanda i Partnercenter Insights ger en översikt över prestandan för olika indirekta återförsäljare av en indirekt leverantör Molnlösningsleverantör en leverantör av Molnlösningsleverantör (CSP). Instrumentpanelen innehåller data om återförsäljare som är aktiva, hur mycket intäkter de genererar och vilka produkter som ger intäkter. Indirekta leverantörer kommer att kunna söka efter en specifik återförsäljare efter namn och söka efter information för återförsäljaren på instrumentpanelen för återförsäljares prestanda.

Du kan visa följande avsnitt från instrumentpanelen Reseller Performance.

- Sammanfattning
- Geografisk spridning av återförsäljare
- Resellers add/churns 
- Intäktstrend för återförsäljare 
- Återförsäljares prestanda per produkt
- Aktiva återförsäljare efter partnerplatser
- Geofördelningstrend för intäkter
- Återförsäljares prestanda per kundsegment
- Signeringsstatus Microsoft-partneravtal Reseller Microsoft-partneravtal (MPA)

 > [!NOTE]
 > Den här rapporten är tillgänglig från Insights instrumentpanel. Om du vill visa den här rapporten måste du ha tilldelats en viss roll i Partnercenter, till exempel Global administratör, Kontoadministratör, Rapportvisare eller Visningsprogram för verkställande rapporter. Mer information finns i företagets globala administratör. Vissa typer av data i den här rapporten kan också vara tillgängliga endast för användare med behörighet som chefsrapportvisare.

## <a name="summary"></a>Sammanfattning

I sammanfattningsavsnittet visas en ögonblicksbild av KPI:er (Key Performance Indicators) som är relaterade till CSP Indirect Provider.

- Aktiva återförsäljare: Antal återförsäljare som har minst en aktiv prenumeration under den månaden.

Micro-diagrammet visar trenden månad för månad för olika återförsäljare som har varit aktiva under det valda datumintervallet.

- Transaktioner för återförsäljare: Antal återförsäljare som sålde minst en prenumeration under den månaden. 

Micro-diagrammet visar trenden månad för månad för återförsäljare som registrerats för det valda datumintervallet.

- Nya återförsäljare: Antal återförsäljare som började göra transaktioner med den indirekta leverantören under den månaden. 

Micro-diagrammet visar trenden månad för månad för det totala antalet nya återförsäljare under det valda datumintervallet.

- Fakturerade intäkter i USD: Intäkter i USD som drivs av återförsäljarna under den månaden. 

Micro-diagrammet visar intäktstrenden månad för månad under det valda datumintervallet.

- Avsnittet Fakturerade intäkter efter produkter innehåller en månadsuppdelning för fakturerade intäkter i USD, uppdelat efter sålda produkter. 

:::image type="content" source="images/insights/resellers-performance-summary.png" alt-text="prestandasammanfattning för återförsäljare.":::

## <a name="geographical-spread-of-resellers"></a>Geografisk spridning av återförsäljare

Vyn **Återförsäljare efter geografisk plats ger den geografiska fördelningen återförsäljare. Med den här widgeten kan partner visa totalt antal **återförsäljare,** nya återförsäljare och **fakturerade intäkter (USD)**, uppdelat efter olika geografiska områden.

Du kan söka efter och välja ett land i rutnätet för att zooma till platsen på kartan. Tryck på **alternativet** Start på kartan för att återgå till den ursprungliga vyn. Hovra över kartan för att visa **fakturerade intäkter (USD)** per land. Fältet Fakturerade intäkter (USD) i rutnätet är sorterbart.

:::image type="content" source="images/insights/resellers-performance-by-geo.png" alt-text="Återförsäljare efter geografiskt område.":::

## <a name="resellers-addchurns"></a>Resellers add/churns

Den här vyn visar en månadsdelning av antalet **nya** återförsäljare, **omdubbade** återförsäljare och **befintliga återförsäljare.** 

- Nya återförsäljare: Antal återförsäljare som nyligen registrerades hos den indirekta leverantören under det valda datumintervallet.
- Omsättningsåterförsäljare: Antal återförsäljare som inte har någon transaktion under de senaste sex månaderna exklusive den aktuella månaden.
- Befintliga återförsäljare: Antal återförsäljare som gjorde transaktioner under föregående månad.

:::image type="content" source="images/insights/resellers-performance-add-churn.png" alt-text="Återförsäljare lägger till/omar.":::

## <a name="resellers-revenue-trend"></a>Intäktstrend för återförsäljare 

Den här vyn visar en månatlig trend för fakturerade intäkter (USD) uppdelade efter produkter, nämligen Office 365, Dynamics 365, Enterprise Mobility and Security (EMS), Microsoft Power BI och Azure. De övergripande måtten aggregeras över de olika produkterna för varje månad. Partnern kan söka efter en specifik återförsäljare efter namn och söka efter data för den specifika återförsäljaren. Fältet Fakturerade intäkter (USD) i rutnätet är sorterbart.

:::image type="content" source="images/insights/resellers-performance-revenue-trend.png" alt-text="Intäktstrend för återförsäljare.":::

## <a name="reseller-performance-by-products"></a>Återförsäljares prestanda per produkt

Den här vyn innehåller en uppdelning av viktiga mått som Fakturerade intäkter, antal prenumerationer och antal licenser per olika produkter per månad. Cirkeldiagrammet till höger visar den övergripande uppdelningen av måtten efter olika produkter, så att partnern får en snabb inblick i uppdelningen av olika produkter som återförsäljaren säljer.

:::image type="content" source="images/insights/resellers-performance-product.png" alt-text="Återförsäljares prestanda efter produkter.":::

## <a name="active-resellers-by-partner-locations"></a>Aktiva återförsäljare efter partnerplatser

Den här vyn ger en uppdelning av aktiva återförsäljare efter partnergeografiska områden. De översta fem geografiska områden visas i förklaringen och återstående kategoriseras som "Övriga".

:::image type="content" source="images/insights/resellers-performance-location.png" alt-text="Aktiva återförsäljare efter partnerplatser.":::

## <a name="revenue-geo-distribution-trend"></a>Geofördelningstrend för intäkter

Den här vyn visar månadstrenden för fakturerade intäkter (USD) uppdelat efter de fem viktigaste geografiska områden.  Resten av intäkterna kategoriseras som "Andra".

:::image type="content" source="images/insights/resellers-performance-revenue-geo-trend.png" alt-text="Trend för geofördelning av intäkter.":::

## <a name="reseller-performance-by-customer-segment"></a>Återförsäljares prestanda per kundsegment

Med den här vyn kan en partner förstå månatliga trender för intäkter i USD, antal prenumerationer och licenser, uppdelat efter olika kundsegment. De fem viktigaste kundsegmenten visas i diagrammet och de återstående kategoriseras som "Övriga".

:::image type="content" source="images/insights/resellers-performance-customer-segment.png" alt-text="Återförsäljares prestanda per kundsegment.":::

## <a name="reseller-mpa-signing-status"></a>Signeringsstatus för återförsäljares MPA

Den här vyn visar MPA-signeringsstatus för återförsäljare tillsammans med ytterligare metadata, till exempel Microsoft Partner Network (MPN), kontrollera status och Partner Membership Center (PMC) till Partner Center-migreringsstatus.

:::image type="content" source="images/insights/resellers-performance-mpa-status.png" alt-text="Signeringsstatus för återförsäljares MPA.":::

## <a name="next-steps"></a>Nästa steg

- Fler rapporter finns i [Partnercenter Insights](partner-center-insights.md).

>[!NOTE] 
> Du kan ladda ned rådata som driver den här rapporten från avsnittet Ladda ned rapporter i Insights instrumentpanel. [Läs mer](insights-download-reports.md) 
