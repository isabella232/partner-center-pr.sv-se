---
title: Partner Center Insights Microsoft Learn analys
ms.topic: article
ms.date: 08/13/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Spåra eleverna i ditt företag genom att utnyttja data om enskild utbildning, slutförda moduler, slutförda utbildningsvägar med mera.
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 132583352e1697a2f9dfa624eb9532692be6d734
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 05/19/2021
ms.locfileid: "110152638"
---
# <a name="the-microsoft-learn-analytics-report-shows-the-status-of-learners-in-your-company"></a>Rapporten Microsoft Learn analys visar status för elever i ditt företag

**Lämpliga roller:** Global | MPN-partneradministratör

Rapporten Microsoft Learn innehåller information om eleverna i företaget, inklusive de moduler som de har slutfört och de utbildningsvägar som de befinner sig på. Rapporten visar status för varje enskild användare. Den globala administratören och MPN-administratören för ditt företag kan visa data.

## <a name="how-to-read-the-report"></a>Läsa rapporten

### <a name="summary-charts"></a>Sammanfattningsdiagram

Dessa diagram sammanfattar antal och månatliga kumulativa trender för tränade individer, slutförda moduler och utbildningsvägar.


**Antal tränade** individer: Antalet distinkta elever som har slutfört minst en modul under det valda datumintervallet 

**Trendminidiagram för tränade** individer: Ackumulerat antal aktiva elever per månad 

**Antal slutförda moduler:** Antal slutförda moduler av eleverna i partnerns företag under det valda datumintervallet.
Om till exempel "Modul 1" slutförs av 15 individer och "Modul 2" har slutförts av samma 15 individer blir antalet slutförda moduler 30. Slutförandedatumet för modulen ska infalla i det valda datumintervallet.

**Trendminidiagram för slutförda moduler:** Ackumulerat antal slutförda moduler månad för månad 

**Antal slutförda** utbildningsväger: Antal slutförda utbildningsvägsslutningar av eleverna på partnerns företag under det valda datumintervallet.
Om utbildningsvägen "Path 1" till exempel har slutförts av 20 individer och utbildningsvägen "path 2" har slutförts av samma 20 individer, blir antalet slutförda utbildningsväg 40. Slutförandedatumet för utbildningsvägen ska vara inom det valda datumintervallet.

**Trendminidiagram för slutförande av utbildningsväg:** Kumulativt antal slutförda utbildningsvägen månad för månad 

### <a name="trained-individuals-monthly-trend"></a>Månatliga trender för tränade individer

Dessa data är trenden för företagets användare som har slutfört en modul för första gången under den månaden. 

**X-axeln** är månad för det valda tidsfiltret. 

**Y-axeln** är antalet aktiva elever som har registrerat sig (första gången en modul har slutförts) under den månaden. Detta är inte kumulativt.

### <a name="module-completions-monthly-trend"></a>Månadstrend för slutförda moduler

Dessa data är trenden för moduler som slutförts av alla företagets användare under den månaden. (inte kumulativt) 

**X-axeln** är månad för det valda tidsfiltret. 

**Y-axeln** är antalet slutförda moduler under den månaden. Detta är inte kumulativt.

### <a name="learning-path-completions-monthly-trend"></a>Månatlig trend för slutförande av utbildningsväg

Dessa data är trenden för utbildningsvägar som har slutförts av företagets användare under den månaden. (inte kumulativt) 

**X-axeln** är månad för det valda tidsfiltret. 

**Y-axeln** är antalet slutförda moduler under den månaden. Detta är inte kumulativt.

### <a name="learning-path-completion-tabs"></a>Flikar för slutförande av utbildningsväg 

**Fliken Modul**

Den här fliken innehåller en uppdelning av moduler som har slutförts i företaget efter de fem främsta modulnamnen. den produkt som modulen är associerad med; och användarrollen som är relevant för modulen.  

- Ringdiagram över slutförda moduler: uppdelning av modulens slutförande (antal som visas i sammanfattningsavsnittet) efter modulnamnen.

Tal som visas i mitten av diagrammet är det totala antalet slutförda moduler

- Slutförande per roll: uppdelning av modulsluten efter modulens roll. Om en modul är associerad med flera roller läggs var och en av rollerna till i antalet slutförda moduler.

Tal som visas i mitten av diagrammet är antalet distinkta roller för modulens slutförande. 

- Slutförande per produkt: uppdelning av modulens slutförande per produkt som modulen mappas till. Om en modul är associerad med flera produkter läggs var och en av produkterna till i antalet slutförda moduler.    

Tal som visas i mitten av diagrammet är antalet distinkta produkter för modulens slutförande.  

**Fliken Utbildningsväg**   

Den här fliken innehåller en analys av utbildningsvägar som har slutförts i företaget efter de fem främsta modulnamnen. den produkt som utbildningsvägen är mappad till; och den roll som är relevant för den här utbildningsvägen.  

- Ringdiagram över slutförda utbildningsvägar: uppdelning av slutförda utbildningsvägar (antal som visas i sammanfattningsavsnittet) efter namn.

- Slutförande efter roll*: uppdelning av slutförda utbildningsvägar efter roll. Om en modul är associerad med flera roller läggs var och en av rollerna till i antalet slutförda moduler.

- Slutförande per produkt: uppdelning av de slutförda utbildningsvägarna efter den Produkt som utbildningsvägen är mappad till. Om en modul är associerad med flera produkter läggs var och en av produkterna till i antalet slutförda moduler.

### <a name="completions-by-learning-individuals"></a>Slutförande av inlärning av individer

Här visas en lista över tränade användare i företaget och information om deras färdiga moduler och utbildningsvägar.

Microsoft Learn identifierar användare med ett användarobjekt-ID. På fliken **Moduler sorteras** alla elever efter de moduler som har slutförts. De visas med sina Microsoft Learn, objekt-ID och moduler. Du kan söka med användarnamn. 

På fliken **Utbildningsvägar visas** alla elever som sorterats efter slutförda utbildningsvägar med elevens visningsnamn, objekt-ID och modulantal.

Så här hämtar du information om en användare med hjälp av användarobjekt-ID:t: 

1. Logga in på [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer ). (Du måste vara global administratör för ditt företags Azure AD-klientorganisation.)

2. Kopiera användarobjektets ID till det [område som är markerat](https://graph.microsoft.com/v1.0/users/a9633ad7-c8dc-4587-b119-0bc286b0711f) i Graph Explorer. 

## <a name="faq"></a>Vanliga frågor

1. Jag kan inte se mitt företags utbildningsdetaljer.

Den här rapporten är tillgänglig för partner som har ett konto i Partnercenter. Om du fortfarande Partner Membership Center kan du inte se den här rapporten.

2.  Vem i vårt företag kan visa den här rapporten? 

Den globala administratören och MPN-administratören kan visa rapporten.

3. Hur ser jag till att alla våra användare associerar sina Microsoft Learn med sina Partnercenter-konton?

När den globala administratören lägger till en ny användare måste användaren gå till användarens **Min profil** associera sitt Microsoft Learn konto.

- Välj ikonen **Ditt** konto i det högra hörnet på instrumentpanelen och välj sedan **Min profil**. 

-  Under **Din utbildning** kommer en användare att kunna associera sitt Microsoft Learning konto och ansluta sina Microsoft-konto till Partner University.

3. Kan jag se alla företagsanvändare som loggar in på Microsoft Learn ett MSA-konto i den här rapporten?

Det bästa sättet att göra detta är för närvarande att lägga till dessa användare i din Azure AD-klientorganisation och sedan lägga till dem i Partnercenter så att de kan associera sina Microsoft Learn-konton **via Min profil** i Partnercenter. 

För användare som bara använder sitt MSA-konto för utbildning kommer Microsoft Learn-teamet inom en snar framtid att kunna koppla sin arbets-e-post till sin Microsoft Learn profil. 

## <a name="next-steps"></a>Nästa steg

Fler rapporter finns i [Partner Center Insights](partner-center-insights.md).

>[!NOTE] 
> Du kan ladda ned rådata som driver den här rapporten från avsnittet Ladda ned rapporter på instrumentpanelen Insights. [Läs mer](pci-download-reports.md) 