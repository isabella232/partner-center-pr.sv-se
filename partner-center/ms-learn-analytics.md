---
title: Partnercenter för Insights Microsoft Learn analys
ms.topic: article
ms.date: 08/13/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-insights
description: Spåra eleverna i ditt företag genom att utnyttja data om enskild utbildning, slutförda moduler, slutförda utbildningsvägar med mera.
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: e56ba633df6980605361fb5dabde185bda5baa663581e5ef47d4da4fda924a04
ms.sourcegitcommit: 121f1b9cbd88faeba60dc9b475f9c0647cdc933c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/06/2021
ms.locfileid: "115694548"
---
# <a name="use-microsoft-learn-analytics-reports"></a>Använda Microsoft Learn analysrapporter

**Lämpliga roller:** Global | MPN-partneradministratör

Rapporten [Microsoft Learn](/learn/) innehåller information om eleverna i företaget, inklusive de moduler som de har slutfört och de utbildningsvägar som de befinner sig på. Rapporten visar status för varje enskild användare. Globala administratörer och MPN-administratörer för ett företag kan visa data.

## <a name="how-to-read-the-report"></a>Läsa rapporten

### <a name="summary-charts"></a>Sammanfattningsdiagram

Dessa diagram sammanfattar antal och månatliga kumulativa trender för tränade individer, slutförda moduler och utbildningsvägar.

**Antal tränade** individer: Antalet distinkta elever som har slutfört minst en modul under det valda datumintervallet 

**Trendminidiagram för tränade** individer: Ackumulerat antal aktiva elever per månad 

**Antal slutförda moduler:** Antal slutförda moduler av eleverna i partnerns företag under det valda datumintervallet.
Om till exempel "Modul 1" slutförs av 15 individer och "Modul 2" har slutförts av samma 15 individer blir antalet slutförda moduler 30. Slutförandedatumet för modulen ska infalla i det valda datumintervallet.

**Trendminidiagram för slutförda moduler:** Ackumulerat antal slutförda moduler månad för månad 

**Learning** antal slutförda sökvägar: Antal Learning slutförda sökvägar av eleverna i partnerns företag under det valda datumintervallet.
Om till exempel Learning sökvägen "Sökväg 1" har slutförts av 20 individer och Learning-sökvägen "sökväg 2" har slutförts av samma 20 individer, blir antalet slutförda Learning-sökvägar 40. Slutförandedatumet Learning sökvägen ska vara inom det valda datumintervallet.

**Learning för slutförande av utbildningsvägens trendminidiagram:** Kumulativt antal utbildningsvägsslutningar för månad över månad 

### <a name="trained-individuals-monthly-trend"></a>Tränade individers månatliga trend

Dessa data är trenden för företagets användare som har slutfört en modul för första gången under den månaden. 

**X-axeln** är månad för det valda tidsfiltret. 

**Y-axeln** är antalet aktiva elever som har registrerat sig (första gången en modul slutförs) under den månaden. Detta är inte kumulativt.

### <a name="module-completions-monthly-trend"></a>Månadstrend för slutförande av moduler

Dessa data är trenden för moduler som slutförts av alla företagets användare under den månaden. (inte kumulativt) 

**X-axeln** är månad för det valda tidsfiltret. 

**Y-axeln** är antalet slutförda moduler under den månaden. Detta är inte kumulativt.

### <a name="learning-path-completions-monthly-trend"></a>Learning slutförande av sökvägar månadsvis trend

Dessa data är trenden för utbildningsvägar som slutfördes av företagets användare under den månaden. (inte kumulativt) 

**X-axeln** är månad för det valda tidsfiltret. 

**Y-axeln** är antalet slutförda moduler den månaden. Detta är inte kumulativt.

### <a name="learning-path-completion-tabs"></a>Learning sökvägsflikar

#### <a name="module-tab"></a>Fliken Modul

Den här fliken innehåller en uppdelning av moduler som har slutförts i företaget efter de fem främsta modulnamnen. den produkt som modulen är associerad med; och användarrollen som är relevant för modulen.  

- Ringdiagram över slutförda moduler: uppdelning av modulens slutförande (antal som visas i sammanfattningsavsnittet) efter modulnamnen.

Tal som visas i mitten av diagrammet är det totala antalet slutförda moduler

- Slutförande per roll: uppdelning av modulsluten efter modulens roll. Om en modul är associerad med flera roller läggs var och en av rollerna till i antalet slutförda moduler.

Tal som visas i mitten av diagrammet är antalet distinkta roller för modulens slutförande. 

- Slutförande per produkt: uppdelning av modulens slutförande per produkt som modulen mappas till. Om en modul är associerad med flera produkter läggs var och en av produkterna till i antalet slutförda moduler.    

Tal som visas i mitten av diagrammet är antalet distinkta produkter för modulens slutförande.  

#### <a name="learning-path-tab"></a>Learning sökvägsflik

Den här fliken innehåller en analys av utbildningsvägar som har slutförts i företaget efter de fem främsta modulnamnen. den produkt som utbildningsvägen är mappad till; och den roll som är relevant för den här utbildningsvägen.  

- Learning diagram över slutförda sökvägar: uppdelning av Learning sökvägsslutningar (antal som visas i sammanfattningsavsnittet) efter namn.

- Slutförande per roll: uppdelning av slutförda utbildningsvägar efter roll. Om en modul är associerad med flera roller läggs var och en av rollerna till i antalet slutförda moduler.

- Slutförande per produkt: uppdelning av de slutförda utbildningsvägarna efter den Produkt som utbildningsvägen är mappad till. Om en modul är associerad med flera produkter läggs var och en av produkterna till i antalet slutförda moduler.

### <a name="completions-by-learning-individuals"></a>Slutförande av inlärning av individer

Här visas en lista över tränade användare i företaget och information om deras färdiga moduler och utbildningsvägar.

Microsoft Learn identifierar användare med ett användarobjekt-ID. På fliken **Moduler sorteras** alla elever efter de moduler som har slutförts. De visas med deras Microsoft Learn, objekt-ID och antal moduler. Du kan söka med användarnamn. 

På fliken **Learning sökvägar** visas alla elever som sorterats efter slutförda utbildningsvägar med elevens visningsnamn, objekt-ID och modulantal.

Så här hämtar du information om en användare med hjälp av användarobjekt-ID:t: 

1. Logga in på [Graph Explorer.](https://developer.microsoft.com/graph/graph-explorer ) (Du måste vara global administratör för företagets Azure AD-klientorganisation.)

2. Kopiera användarobjektets ID till det [område som är markerat](https://graph.microsoft.com/v1.0/users/a9633ad7-c8dc-4587-b119-0bc286b0711f) i Graph Explorer. 

## <a name="frequently-asked-questions-faq"></a>Vanliga frågor och svar (FAQ)

1. Jag kan inte se mitt företags Learn-information.

   Den här rapporten är tillgänglig för partner som har ett konto i Partnercenter. Om du fortfarande Partner Membership Center kan du inte se den här rapporten.

2. Vem på mitt företag kan visa den här rapporten? 

   Den globala administratören och MPN-administratören kan visa rapporten.

3. Hur ser jag till att alla våra användare associerar sina Microsoft Learn med sitt Partnercenter-konto?

   *När den globala administratören* lägger till en ny användare måste användaren gå till [Microsoft Learn](/learn/) för att länka sitt Azure Active Directory(AD) företagskonto eller arbetskonto med sitt Learn-konto. Detta säkerställer Insights Learning fliken visar rätt kurser och färdigheter.
   
   Användaren måste:
   
   1. Logga in [Microsoft Learn](/learn/).
   2. Välj profilbilden och välj sedan **Min profil**.
   3. Välj **inställningar**.
   4. Under **Kontohantering lägger** du till arbetskontot under **Länkade konton**.

4. Kan jag se alla företagets användare som loggar in på Microsoft Learn med ett MSA-konto i den här rapporten?

   Det bästa sättet att göra detta är för närvarande att lägga till dessa användare i din Azure AD-klientorganisation och sedan lägga till dem i Partnercenter så att de kan associera sina Microsoft Learn-konton **via Min profil** i Partnercenter. 

   För användare som bara använder sitt MSA-konto för utbildning kommer Microsoft Learn-teamet inom en snar framtid att kunna koppla sin e-post till sin Microsoft Learn profil. 

## <a name="next-steps"></a>Nästa steg

Fler rapporter finns i [Partnercenter Insights](partner-center-insights.md).

>[!NOTE] 
> Du kan ladda ned rådata som driver den här rapporten från avsnittet Ladda ned rapporter i Insights instrumentpanel. [Läs mer](insights-download-reports.md) 
