---
title: Microsoft Learn analys för partner Center Insights
ms.topic: article
ms.date: 08/13/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Spåra eleverna i företaget genom att använda data på individuell utbildning, färdiga moduler, slutförda utbildnings vägar och mycket annat.
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 5b9a0ea8c4eefee1a87b9ccd626b1f2864234521
ms.sourcegitcommit: f24089cd27b1de6ecf6ddbefb6cbb2d340e144de
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/01/2021
ms.locfileid: "106132323"
---
# <a name="the-microsoft-learn-analytics-report-shows-the-status-of-learners-in-your-company"></a>Rapporten Microsoft Learn Analytics visar status för elever i företaget

**Lämpliga roller**

- Global administratör
- MPN-partner administratör

Microsoft Learn rapporten innehåller information om de lärare i företaget, inklusive moduler som har slutförts och de inlärnings vägar som de är på. Rapporten visar status för varje enskild persons elev. Den globala administratören och MPN-administratören för ditt företag kan visa data.

## <a name="how-to-read-the-report"></a>Läsa rapporten

### <a name="summary-charts"></a>Sammanfattnings diagram

De här diagrammen sammanfattar antal och månatliga ackumulerade trender för inutbildade individer, komplettering av moduler och utbildnings vägar.


**Antal utbildade individer**: ett antal distinkta elever som har slutfört minst en modul under det valda datum intervallet 

**Utbildade Individer Trends mini-diagram**: månads Visa månad ackumulerat antal aktiva elever 

**Antal slutförda moduler**: antal moduler som slutförs av lärarna i partner företaget under det valda datum intervallet.
Om t. ex. "modul 1" har slutförts av 15 individer och "modul 2" har slutförts av samma 15 individer, är antalet slutförda moduler 30. Utgångs datumet för modulen ska ligga inom det valda datum intervallet.

**Modulen för att slutföra modulen trend diagrammet**: månads Visa månad ackumulerat antal slutförda moduler 

**Antal slutförda inlärnings Sök** vägar: antal inlärnings Sök vägar för utbildning i partner företaget under det valda datum intervallet.
Exempel: om utbildnings Sök vägen "sökväg 1" har slutförts av 20 individer och inlärnings Sök vägen "sökväg 2" har slutförts av samma 20 individer, är antalet slutförda utbildnings vägar 40. Utbildnings Sök vägens avslutnings datum ska ligga inom det valda datum intervallet.

**Trend linje för inlärnings Sök väg Trends mini-diagram**: månads Visa månad, totalt antal av utbildnings Sök vägens slut för ande 

### <a name="trained-individuals-monthly-trend"></a>Intränade individers månatliga trend

Dessa data är trenden för företagets användare som har slutfört en modul för första gången under den månaden. 

**X-axeln** är månad för det valda tids filtret. 

**Y-axeln** är antalet aktiva elever som har registrerat (första avslutnings tid för en modul) under den månaden. Detta är inte kumulativt.

### <a name="module-completions-monthly-trend"></a>Slutförd modul per månad

Dessa data är trenden för moduler som har slutförts av alla företagets användare under den månaden. (inte kumulativt) 

**X-axeln** är månad för det valda tids filtret. 

**Y-axeln** är antalet slutförda moduler under den månaden. Detta är inte kumulativt.

### <a name="learning-path-completions-monthly-trend"></a>Månads trend för utbildnings Sök väg

Dessa data är trenden för utbildnings vägar som slutförs av ditt företags användare under den månaden. (inte kumulativt) 

**X-axeln** är månad för det valda tids filtret. 

**Y-axeln** är antalet färdiga moduler i månaden. Detta är inte kumulativt.

### <a name="learning-path-completion-tabs"></a>Flikar för utbildnings Sök väg komplettering 

**Fliken modul**

På den här fliken finns en uppdelning av moduler som har slutförts i företaget med de fem främsta modulernas namn. produkten som modulen är associerad med. och användar rollen som är relevant för modulen.  

- Avslutnings diagram för modulen: nedbrytning av modulen slutförs (antal som visas i avsnittet Sammanfattning) av modulnamnet.

Talet som visas i diagrammets mitt är total summan av moduler som slutförts

- Slutförda efter roll: uppdelning av modulen slutförs av modulens roll. Om en modul är associerad med flera roller läggs varje roll till i antalet slutförda moduler.

Talet som visas i diagrammets mitt är antalet distinkta roller för hur många moduler som ska slutföras. 

- Slut för ande efter produkt: nedbrytning av modulen slutförs av produkten som modulen är mappad till. Om en modul är associerad med flera produkter läggs varje produkt till i antalet slutförda moduler.    

Talet som visas i diagrammets mitt är antalet distinkta produkter för att slutföra modulen.  

**Fliken utbildnings Sök väg**   

På den här fliken finns en uppdelning av utbildnings vägar som har slutförts i företaget med de fem främsta modulnamnna. produkten som utbildnings vägen är mappad till; och rollen som är relevant för den här utbildnings vägen.  

- Slut för ande av utbildnings vägar ring diagram: nedbrytning av utbildnings Sök vägens slut för ande (antal som visas i avsnittet Sammanfattning) efter namn.

- Slut för ande av roll *: analys av inlärnings Sök vägarnas slut för ande av rollen. Om en modul är associerad med flera roller läggs varje roll till i antalet slutförda moduler.

- Slut för ande efter produkt: nedbrytning av de utbildnings vägar som slutförs av produkten som utbildnings vägen mappas till. Om en modul är associerad med flera produkter läggs varje produkt till i antalet slutförda moduler.

### <a name="completions-by-learning-individuals"></a>Slut för ande genom att lära sig personer

Här visas de tränade användarna i företaget och information om deras slutförda moduler och utbildnings vägar.

Microsoft Learn identifierar läraare med ett användar objekt-ID. På **fliken moduler** sorteras alla lärare efter att modulerna har slutförts. De visas med sina Microsoft Learn användar namn, objekt-ID och moduler antal. Du kan söka med användar namn. 

På **fliken inlärnings Sök vägar** , visas alla inlärningar sorterade efter inlärnings Sök vägar som har slutförts, med elevens visnings namn, objekt-ID och antal moduler.

Så här hämtar du en elevs information med hjälp av användar objektets ID: 

1. Logga in i [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer ). (Du måste vara den globala administratören för ditt företags Azure AD-klient.)

2. Kopiera användar objekt-ID: t till det område som är [markerat](https://graph.microsoft.com/v1.0/users/a9633ad7-c8dc-4587-b119-0bc286b0711f) i Graph Explorer. 

## <a name="faq"></a>Vanliga frågor

1. Jag kan inte se min företags utbildnings information.

Den här rapporten är tillgänglig för partner som har ett konto i Partner Center. Om du fortfarande befinner dig i partner medlemskaps Center kan du inte se den här rapporten.

2.  Vem i företaget kan visa den här rapporten? 

Den globala administratören och MPN-administratören kan visa rapporten.

3. Hur kan jag se till att alla våra användare associerar sina Microsoft Learn-konton med sitt Partner Center-konto?

När den globala administratören lägger till en ny användare måste användaren gå till **min profil** för att associera sitt Microsoft Learn-konto.

- Välj **din konto** -ikon i det högra hörnet på instrument panelen och välj **min profil**. 

-  Under **din utbildning** kommer användaren att kunna associera sitt Microsoft Learning-konto och ansluta sina Microsoft-konto till partner University.

3. Kan jag se alla företagets användare som loggar in på Microsoft Learn med ett MSA-konto i den här rapporten?

För närvarande är det bästa sättet att göra detta är att lägga till dessa användare i Azure AD-klienten och sedan lägga till dem i Partner Center så att de kan associera sina Microsoft Learn-konton via **min profil** i Partner Center. 

För användare som bara använder sitt MSA-konto för utbildning, kommer Microsoft Learns teamet att göra det möjligt för dem att associera sitt arbets-e-postmeddelande till sin Microsoft Learn-profil. 

## <a name="next-steps"></a>Nästa steg

Mer information finns i [partner Center Insights](partner-center-insights.md).

>[!NOTE] 
> Du kan ladda ned rå data från den här rapporten från avsnittet hämta rapporter på instrument panelen insikter. [Läs mer](pci-download-reports.md) 