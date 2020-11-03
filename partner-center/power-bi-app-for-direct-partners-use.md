---
title: Använd partner Center Analytics för Power BI
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Lär dig hur du visar dina affärs data med hjälp av Partner Center Analytics-appen för Power BI (för direkta partner i CSP).
fwlink: https://go.microsoft.com/fwlink/?linkid=852581
author: v-sumukh
ms.author: v-sumukh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 248527fdbc536c552f7b2d00f208838b4ef19085
ms.sourcegitcommit: 0a6b1e6d845391539f54213efff00af4d23f028c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 07/14/2020
ms.locfileid: "92529209"
---
# <a name="view-your-business-data-with-the-partner-center-analytics-app-for-microsoft-power-bi"></a>Visa dina affärs data med partner Center Analytics-appen för Microsoft Power BI

**Gäller för**

- Partnercenter

**Lämpliga roller**

- Global administratör
- Användaradministratör
- Försäljnings agent
- Administratörs agent

## <a name="view-your-business-data"></a>Visa dina affärs data

Få en visuell representation av dina affärs data med partner Center Analytics-appen för Power BI, inklusive:

- Tillväxt av kund basen, prenumerationer och licenser

- Användning av Office 365, Microsoft Dynamics och Microsoft Azure produkter

- Dagliga förbruknings enheter för varje avgiftsbelagd resurs i varje Azure-prenumeration under de senaste 60 dagarna

- Beräknad kostnad (baserat på senaste pris kortet)

- Möjlighet att exportera data uppsättningar och skapa anpassade rapporter, inklusive per kund.

### <a name="about-the-partner-center-analytics-app-preview-release"></a>Om för hands versionen av Partner Center Analytics-appen

- Den här appen är endast för direkta partner i Cloud Solution Provider-programmet. Andra partner i CSP (indirekt åter försäljare, till exempel) kan inte logga in.

- Eventuella beräknade kostnader är fakturerings-och faktura data för moms, och är inte juridiskt bindande. Uppskattade kostnader är avsedda att användas enbart för data insikter.

- Kund information baseras på prenumerationer. Alla kunder som du nyligen har skapat konton för, men som ännu inte har några prenumerationer, ingår inte i antal.

- Den uppskattade kostnaden baseras på det senaste avgifts kortet, som baseras på CSP-priset.

- Dagar är kalender dagar.

### <a name="business-insights-report"></a>Rapporten affärs insikter

- **Kund klienter** : antal olika Azure AD-klienter med kunder som har köpt prenumerationer

- **Nytt (senaste 30 dagarna)** : nya kunder som köper minst en prenumeration under de senaste 30 dagarna

- **Omsättning (senaste 30 dagarna)** : kunder utan några "aktiva", "i respittiden" eller "inaktiverade" prenumerationer

- **Nytt (senaste 24 timmarna)** : nya kunder som köper minst en prenumeration under de senaste 24 timmarna

- **Beräknad månads kostnad under de senaste 12 månaderna** : månads Visa månads trend för uppskattat belopp för förskotts betalning per månad under perioden de senaste 12 månaderna

- **Uppskattad kostnad per produkt under de senaste 12 månaderna** : produkter som säljs sorterade efter uppskattat belopp för moms belopp som sammanställs under perioden de senaste 12 månaderna. Den här statusen anger de främsta produkterna som visar de flesta intäkter.

- **Kunder under de senaste 12 månaderna** : månads Visa månads trend för nya kunder och omsättnings kunder sammanlagt månads vis under perioden de senaste 12 månaderna

- **Uppskattad kostnad per kund under de senaste 12 månaderna** : kunder sorteras efter uppskattat belopp för moms belopp som sammanställs under perioden de senaste 12 månaderna. Den här statusen anger de främsta kunderna som har störst intäkt.

- **Kund antal per produkt** : produkter som säljs sorterade efter associerade kunder. Denna status anger de produkter som säljs till de flesta kunder.

### <a name="subscription-insights-report"></a>Rapport om prenumerations Insights

- **Prenumerations status** :

- Aktiv: prenumerationer som tillhör status "aktiv" eller "i respittid"

  - Pausad: prenumerationer som tillhör tillståndet "inaktiverat"

  - Insamlad: prenumerationer som hör till statusen företablerad eller upphört att gälla

- **Förfallo status** :

  - Utgånget: prenumerationer som redan har upphört att gälla (där prenumerationens slutdatum har passerat)

  - Upphör att gälla efter 30 dagar: prenumerationer som upphör att gälla efter 30 dagar (där prenumerationens slutdatum är efter nästa 30 dagar)

  - Går ut om 30 dagar: prenumerationer som upphör att gälla inom de närmaste 30 dagarna (där prenumerationens slutdatum infaller mellan idag och de närmaste 30 dagarna)

- **Totalt antal prenumerationer** : prenumerationer i "aktiv", "i respittiden" eller "inaktive rad" status

- **Nytt (senaste 30 dagarna)** : nya prenumerationer som har köpts av kunder under de senaste 30 dagarna

- **Nytt (senaste 24 timmarna)** : nya prenumerationer som har köpts av kunder inom de senaste 24 timmarna

- **Upphör att gälla om 30 dagar** : prenumerationer som upphör att gälla inom de närmaste 30 dagarna

- **Omsättning (senaste 30 dagarna)** : prenumerationer som har avbrutits eller skjutits upp (inaktiverade) inom de senaste 30 dagarna

- **Distribution efter prenumerations typer** :% distribution av totala prenumerationer efter licens typ och användnings beroende prenumerations typ

- **Antal aktiva prenumerationer per produkt** : produkter som säljs sorterade efter antal aktiva prenumerationer

- **Prenumerationer under de senaste 12 månaderna** : månads Visa månads trend för nya prenumerationer och omsättnings prenumerationer sammanlagt månads vis under perioden de senaste 12 månaderna

- **Kund prenumerations information** : detaljerad vy över kunder, prenumerationer och erbjudanden

### <a name="license-insights-report"></a>Licens insikts rapport:

- **Totalt antal licenser** : totalt antal licenser som sammanställts i alla licensbaserade prenumerationer

- **Ny (senaste 30 dagarna)** : licens tillägget inom de senaste 30 dagarna

- **Omsättning (senaste 30 dagarna)** : licens minskning inom de senaste 30 dagarna

- **Nytt (senaste 24 timmarna)** : licens tillägget inom de senaste 24 timmarna

- **Licenser under de senaste 90 dagarna** : månads Visa månads trend för licens tillägg och minskning sammanlagt månads vis under perioden de senaste 90 dagarna

- **Antal aktiva licenser per produkt** : produkter som säljs sorterade efter aktiva licens antal

- **Antal aktiva licenser per kund** : kunder sorterade efter aktiva licens antal

- **Information om kund licens händelser under de senaste 90 dagarna** : detaljerad vy över kunder, prenumerationer och prenumerations händelser, inklusive händelse datum, händelse namn, kvantitet och ändring av kvantitet.

### <a name="licenses-usage-report"></a>Licens användnings rapport:

- **Licenser som tilldelas av produkten** : produkter som säljs sorterade efter licens tilldelnings antal

- **Licenser som används av produkten** : produkter som säljs sorterade efter licens användning

- **Kund distribution av tilldelade licenser** :% distribution av totalt antal kunder som brutits i Bucket med 20% intervall av licens tilldelningen%

- **Kund distribution av licenser som används** :% distribution av totalt antal kunder som är brutna i Bucket med 20% intervall med licens användning%

- **Licenser tilldelade av kunden** : detaljerad vy över licenser som har sålts och licenser tilldelade av kunder och produkter

- **Licenser som används av kunden** : detaljerad vy över licenser som har sålts och licenser som används av kunder och produkter

### <a name="azure-insights-report"></a>Azure Insights-rapport:

- **Användnings kunder under de senaste 12 månaderna** : månads Visa månads trend för nya användnings kunder och omsättnings bara användnings kunder sammanställda månads vis under perioden de senaste 12 månaderna

- **Användnings prenumerationer under de senaste 12 månaderna** : månads Visa månads trend för nya användnings prenumerationer och indelade användnings prenumerationer sammanställda månads vis under perioden de senaste 12 månaderna

- **Uppskattad kostnad för användning av kunden under de senaste 60 dagarna** : användnings kunder sorteras efter uppskattat belopp belopp för förskotts betalning som sammanställs under perioden senaste 60 dagar. Denna status anger de mest använda användnings kunderna som tar de flesta intäkter

- **Uppskattad kostnad för användning per kategori över de senaste 60 dagarna** : mätar kategorier med användnings prenumerationer sorterade efter uppskattat belopp för förskotts betalning som sammanställs under perioden senaste 60 dagar.

- **Uppskattad kostnad för användning av prenumeration under de senaste 60 dagarna** : användnings prenumerationer efter uppskattat belopp belopp för förskotts betalning som sammanställts under perioden senaste 60 dagar.

- **Kund Beräknad användnings kostnad per utgifts budget** : kunderna sorteras efter procent andel av den aktuella förbruknings utgifts budgeten som överskrider tröskelvärdet (100%).

### <a name="azure-resource-usage-report"></a>Azure-resurs användnings rapport:

- **Användning av Azure-resurser per dag för vald period** : dagliga förbruknings enheter för varje mätnings resurs i varje Använd prenumeration för vald period under de senaste 60 dagarna.

- **Uppskattad användnings kostnad för Azure-resurser för vald period** : uppskattad kostnad baserat på det senaste kortet för varje mätnings resurs i varje Använd prenumeration för den valda perioden under de senaste 60 dagarna. 

## <a name="next-steps"></a>Nästa steg

- [Översikt över partner Center-analys för Power BI app](power-bi-app-for-direct-partners.md)

- [Installera och förhandsgranska partnercenteranalysappen för Microsoft Power BI](power-bi-app-for-direct-partners-install.md)
