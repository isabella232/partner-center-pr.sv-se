---
title: Använda Partner Center Analytics för Power BI
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
description: Lär dig hur du visar dina affärsdata med hjälp av appen Partnercenteranalys för Power BI (för direkta partner i Molnlösningsleverantör(CSP)-programmet).
fwlink: https://go.microsoft.com/fwlink/?linkid=852581
author: v-sumukh
ms.author: v-sumukh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: eea221af22e9bd7aa684bc5120b0799f083f8663
ms.sourcegitcommit: ad1af627f5ee6b6e3a70655f90927e932cf4c985
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 07/29/2021
ms.locfileid: "114836108"
---
# <a name="view-your-business-data-with-the-partner-center-analytics-app-for-microsoft-power-bi"></a>Visa dina affärsdata med Partner Center Analytics-appen för Microsoft Power BI



**Lämpliga roller:** Global | Administratörsbehörighet för användarhantering | Försäljningsagentens | Administratörsagent

## <a name="view-your-business-data"></a>Visa dina affärsdata

Hämta en visuell representation av dina affärsdata med Partner Center Analytics-appen för Microsoft Power BI, inklusive:

- Tillväxt av kundbasen, prenumerationer och licenser

- Användning av Office 365, Microsoft Dynamics och Microsoft Azure produkter

- Dagliga förbrukningsenheter för varje förbrukningsresurs i varje Azure-prenumeration under de senaste 60 dagarna

- Uppskattad kostnad (baserat på det senaste priskortet)

- Möjlighet att exportera datauppsättningar och skapa anpassade rapporter, inklusive per kund.

### <a name="about-the-partner-center-analytics-app-preview-release"></a>Om förhandsversionen av Partner Center Analytics-appen

- Den här appen är endast för direkta partner i Molnlösningsleverantör-programmet (CSP). Andra partner i CSP (indirekta återförsäljare till exempel) kommer inte att kunna logga in.

- Uppskattade kostnader är fakturerings-/fakturadata före skatt och är inte juridiskt bindningsbaserade. Uppskattade kostnader är endast avsedda att användas för datainsikter.

- Kundinformation baseras på prenumerationer. Alla kunder som du nyligen har skapat konton för, men som ännu inte har prenumerationer, ingår inte i antalet.

- Den uppskattade kostnaden baseras på det senaste priskortet, som baseras på CSP-priser.

- Dagar är kalenderdagar.

### <a name="business-insights-report"></a>Rapport Insights företag

- **Kundklienter:** Antalet distinkta Azure Active Directory (Azure AD) för kunder som har köpt prenumerationer

- **Ny (senaste 30 dagarna):** Nya kunder har köpt minst en prenumeration under de senaste 30 dagarna

- **Omsättning (senaste 30 dagarna):** Kunder utan prenumerationer som är "aktiva", "i respit" eller "inaktiverade"

- **Ny (senaste 24 timmarna)**: Nya kunder har köpt minst en prenumeration under de senaste 24 timmarna

- **Uppskattad månadskostnad under de senaste 12** månaderna: Månad över månad-trend för beräknat belopp före skatt i dollar aggregerat månadsvis under de senaste 12 månaderna

- **Uppskattad kostnad per produkt under de senaste 12** månaderna: Produkter som sålts sorterade efter beräknat belopp före skatt som aggregerats under de senaste 12 månaderna. Den här statusen anger de främsta produkterna som ger mest intäkter.

- **Kunder under de senaste 12** månaderna: Trenden månad för månad för nya kunder och omsättningskunder aggregerats månadsvis under de senaste 12 månaderna

- **Uppskattad kostnad per kund under de senaste 12** månaderna: Kunder sorterade efter beräknat belopp före skatt som aggregerats under de senaste 12 månaderna. Den här statusen anger att de främsta kunderna har störst intäkter.

- **Antal kunder efter produkt:** Sålda produkter sorterade efter associerade kunder. Den här statusen anger de främsta produkter som sålts till de flesta kunder.

### <a name="subscription-insights-report"></a>Rapport Insights prenumerationsprenumeration

- **Prenumerationsstatus:**

- Aktiv: Prenumerationer som hör till antingen "aktiv" eller "i respittillstånd"

  - Inaktiverad: Prenumerationer som hör till tillståndet "inaktiverad"

  - Avetablerat: Prenumerationer som tillhör statusen "avetablerat" eller "upphört att gälla"

- **Förfallostatus:**

  - Har upphört att gälla: Prenumerationer som redan har upphört att gälla (där prenumerationens slutdatum har passerat)

  - Upphör att gälla efter 30 dagar: Prenumerationer som upphör att gälla efter 30 dagar (där prenumerationens slutdatum infaller efter de kommande 30 dagarna)

  - Upphör att gälla om 30 dagar: Prenumerationer som upphör att gälla inom de närmaste 30 dagarna (där slutdatumet för prenumerationen är mellan i dag och nästa 30 dagar)

- **Totalt antal** prenumerationer: Prenumerationer i statusen "aktiv", "i respit" eller "inaktiverad"

- **Nytt (senaste 30 dagarna): Nya** prenumerationer som köpts av kunder under de senaste 30 dagarna

- **Nytt (senaste 24 timmarna)**: Nya prenumerationer som köpts av kunder under de senaste 24 timmarna

- **Går ut om 30 dagar:** Prenumerationer som upphör att gälla inom 30 dagar

- **Omsättning (senaste 30 dagarna):** Prenumerationer som har avetablerades eller inaktiverats (inaktiverats) under de senaste 30 dagarna

- **Fördelning efter prenumerationstyper:**% fördelning av totalt antal prenumerationer efter licensbaserad och användningsbaserad prenumerationstyp

- **Antal aktiva prenumerationer efter produkt:** Sålda produkter sorterade efter antal aktiva prenumerationer

- **Prenumerationer under de senaste 12 månaderna:** Månad över månad-trenden för nya prenumerationer och omsättningsprenumerationer aggregerade månadsvis under de senaste 12 månaderna

- **Information om** kundprenumeration: Detaljerad vy över kunder, prenumerationer och erbjudanden

### <a name="license-insights-report"></a>Licensrapport Insights licens:

- **Totalt antal** licenser: Totalt antal licenser aggregerade för alla licensbaserade prenumerationer

- **Nytt (senaste 30 dagarna):** Licens utöver de senaste 30 dagarna

- **Omsättning (senaste 30 dagarna): Licensminskning** under de senaste 30 dagarna

- **Nytt (senaste 24 timmarna)**: Licens utöver de senaste 24 timmarna

- **Licenser under de senaste 90 dagarna:** Trenden månad för månad för licens tillägg och minskningar aggregeras månadsvis under de senaste 90 dagarna

- **Antal aktiva licenser efter produkt:** Sålda produkter sorterade efter antal aktiva licenser

- **Antal aktiva licenser per kund:** Kunder sorterade efter antal aktiva licenser

- **Information om kundlicenshändelser under de senaste 90** dagarna: Detaljerad vy över kunder, prenumerationer och prenumerationshändelser, inklusive händelsedatum, händelsenamn, kvantitet och ändring i kvantitet.

### <a name="licenses-usage-report"></a>Användningsrapport för licenser:

- **Licenser tilldelade efter produkt:** Sålda produkter sorterade efter antal licenstilldelningar

- **Licenser som används efter produkt:** Sålda produkter sorterade efter licensanvändningsantal

- **Kunddistribution av tilldelade licenser:**% fördelning av totalt antal kunder uppdelade i bucketar med 20 % intervall efter licenstilldelning %

- **Kunddistribution av licenser som används:**% fördelning av totalt antal kunder uppdelade i bucketar på 20 % intervall efter licensanvändning %

- **Licenser som tilldelats av kunden:** Detaljerad vy över sålda licenser och licenser som tilldelats av kunder och produkter

- **Licenser som används av kunden:** Detaljerad vy över sålda licenser och licenser som används av kunder och produkter

### <a name="azure-insights-report"></a>Azure Insights rapport:

- **Användningsbaserade kunder under** de senaste 12 månaderna: Trenden månad för månad för nya användningsbaserade kunder och omsättningsbaserade kunder aggregerade månadsvis under de senaste 12 månaderna

- **Användningsbaserade prenumerationer under de senaste 12** månaderna: Trenden månad för månad för nya användningsbaserade prenumerationer och omsade användningsbaserade prenumerationer aggregerade månadsvis under de senaste 12 månaderna

- Uppskattad kostnad för användning per kund under de **senaste 60** dagarna: Användningsbaserade kunder sorterade efter beräknat belopp före skatt i dollar aggregerat under de senaste 60 dagarna. Den här statusen anger de främsta användningsbaserade kunderna som har störst intäkter

- Uppskattad kostnad för användning efter kategori under de **senaste 60** dagarna: Mätarkategorier för användningsbaserade prenumerationer sorterade efter beräknat belopp före skatt som aggregerats under de senaste 60 dagarna.

- Uppskattad kostnad för användning per prenumeration under de **senaste 60** dagarna: Användningsbaserade prenumerationer efter beräknat belopp före skatt som aggregerats under de senaste 60 dagarna.

- **Kundens uppskattade användningskostnad efter utgiftsbudget:** Kunder sorterade efter procentandel av den aktuella användningsbudgeten överskrider tröskelvärdet (100 %).

### <a name="azure-resource-usage-report"></a>Rapport om Azure-resursanvändning:

- **Användning av Azure-resurser per dag** för den valda perioden: Dagliga förbrukningsenheter för varje förbrukningsresurs i varje användningsbaserad prenumeration under den valda perioden under de senaste 60 dagarna.

- **Uppskattad användningskostnad för Azure-resurser** för den valda perioden: Uppskattad kostnad baserat på det senaste priskortet för varje avgiftsbaserad resurs i varje användningsbaserad prenumeration för den valda perioden under de senaste 60 dagarna. 

## <a name="next-steps"></a>Nästa steg

- [Översikt över partnercenteranalys Power BI app](power-bi-app-for-direct-partners.md)

- [Installera och förhandsgranska partnercenteranalysappen för Microsoft Power BI](power-bi-app-for-direct-partners-install.md)
