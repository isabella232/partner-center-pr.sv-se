---
title: Tillägg för ny handel
ms.topic: article
ms.date: 09/03/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
description: Lär dig mer om nya köpupplevelser för köp av tillägg.
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 01644e5d2dd2fe2057d223b62f1f4e9d6f9cd101
ms.sourcegitcommit: 847ad384d44a5a673791cb2950af02225d8174c9
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/16/2021
ms.locfileid: "127876959"
---
# <a name="introduction-new-commerce-add-ons"></a>Introduktion: Tillägg för ny handel

**Lämpliga roller**

- Administratörsagent
- Försäljningsagent
- Global administratör

> [!Note] 
> Ändringarna i den nya handelsupplevelsen är för närvarande endast tillgängliga för partner som ingår i den tekniska förhandsversionen av Microsoft 365/Dynamics 365.

Partner kan köpa tillägg i ny handel för att aktivera andra tjänster som kompletterar en tidigare köpt produkt. Några exempel på detta är anropsplaner, mer diskutrymme eller andra funktioner som kan läggas till om kunden har bastjänsterna.



## <a name="add-ons-in-new-commerce"></a>Tillägg i ny handel ## 

Nya tillägg för handel innehåller liknande begrepp som traditionella licensbaserade tillägg. Nya tillägg för handel, till exempel traditionella licensbaserade, omfattar begreppet förutsättningar. Det här är produkt-SKU:er som kunden måste ha för att tillägget ska fungera korrekt. Kraven för ett tillägg finns i katalog-API:er för en viss SKU och i användarupplevelsen i Partner Center-katalogen. Köp av tillägg kräver att ett eller flera av förutsättningarna finns i kundens klientorganisation.
 
Den största skillnaden vid köp av tillägg mellan traditionell licensbaserad och ny handel är hur *de* köps. I traditionell licensbaserad tillämpar partnern tillägget på en befintlig baserbjudandeprenumeration. I ny handel köper partner tilläggen från själva katalogen, de har inte längre en dubbelköpt köpupplevelse för baserbjudanden och tillägg, allt finns i katalogen i den nya näthandelen.

Många av begreppen om hur tillägg fungerar, ur ett tjänstperspektiv, förblir sanna inom traditionell och ny handel. Både registrera och etablera tilläggstjänster, det finns inget annorlunda med hur etableringen sker. Dessutom kan ett enda tilläggstjänster komplettera fler än en basprodukt-SKU som tillägget är utformat för att fungera med.

## <a name="identifying-add-ons"></a>Identifiera tillägg ##

Partner kan identifiera tillägg och hämta listor med förutsättningar genom att granska SKU-informationen när de hämtar SKU:er via API:et. Tillägg identifieras också i den nya listan med licensbaserade priser för handel i kolumnen Taggar. Erbjudandematrisen innehåller en lista över krav för varje tilläggsprodukt-SKU.

## <a name="purchasing-add-ons"></a>Köpa tillägg ##

Tillägg finns för både traditionella licensbaserade och nya handelsupplevelser. Den största skillnaden är att ny handel möjliggör identifiering och inköp från katalogen, på samma plats som baserbjudandena eller förutsättningarna hittas. Traditionella licensbaserade tillägg kan bara upptäckas och köpas genom att gå till baserbjudandets prenumerationsinformationssida. När ett tillägg visas där tillämpar partnern önskat tillägg.


Nya tillägg för köpupplevelsen identifieras och köps i själva katalogen. Partner kan filtrera efter tillägg för ny handel genom att välja listrutan produkttyp. Tilläggsprodukter är också enkla att se eftersom de har en informationsikon bredvid sig, vilket förklarar deras tilläggsstatus och innebörd.


Partner kan få mer information om de produkter  som krävs för ett tillägg genom att klicka på Visa kompatibla basproduktprenumerationer för att visa en lista över produkt-SKU:er som måste finnas för att partnern ska kunna köpa ett visst tillägg.


## <a name="add-on-enforcement"></a>Tillämpning av tillägg ##

Partner får felmeddelanden när de försöker köpa en ny tilläggsprodukt för handel där kunden inte har något av kraven. Partner kan verifiera att en kund uppfyller kraven genom att anropa API:et validateAddon i Partnercenter.

## <a name="important-details-when-purchasing-add-ons"></a>Viktig information när du köper tillägg ##

Tillägg köps som distinkta produkt-SKU:er om kunden uppfyller kraven. Tilläggsprenumerationer har sin egen distinkta termjustering. Partner som köper tillägg kommer att märka att termen och det associerade slutdatumet kanske inte är samma som förutsättningarna. Så länge båda prenumerationerna förnyas automatiskt till nya villkor fungerar kraven och tilläggen utmärkt. Om partnern bestämmer sig för att avsluta den nödvändiga perioden genom att inte förnya automatiskt, bör tillägget också uppdateras till att inte förnyas automatiskt i slutet av tilläggperioden om partnern drar slutsatsen att det inte längre behövs.  Partner konverterar en produkt-SKU till en högre SKU som redan har tilläggstjänster kan skicka en tjänstbegäran med stöd för att inaktivera ett tillägg.

Partner förväntas hantera termen slutdatum för tillägg som de får för att säkerställa att det finns en anpassning efter behov till baserbjudandena.

