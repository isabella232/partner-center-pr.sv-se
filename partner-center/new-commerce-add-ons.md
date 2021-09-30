---
title: Tillägg för ny handel
ms.topic: article
ms.date: 09/29/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
description: Lär dig mer om nya köpupplevelser för köp av tillägg.
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 355c7ae3d4832764f6201613c040eebca998c3b6
ms.sourcegitcommit: a59e1abb470f4847e8f8337ffa4ba705514a0424
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/29/2021
ms.locfileid: "129249340"
---
# <a name="introduction-new-commerce-add-ons"></a>Introduktion: Tillägg för ny handel

**Lämpliga roller:** Administratörsagent | Försäljningsagent | Global administratör

> [!NOTE]
> Ändringarna i den nya handelsupplevelsen är för närvarande endast tillgängliga för partner som ingår i den tekniska förhandsversionen av Microsoft 365/Dynamics 365.

Partner kan köpa tillägg i ny handel för att aktivera andra tjänster som kompletterar en tidigare köpt produkt. Några exempel på tillägg är anropsplaner, mer diskutrymme eller andra funktioner som kan läggas till om kunden har bastjänsterna.

## <a name="add-ons-in-new-commerce"></a>Tillägg i ny handel

Nya tillägg för handel innehåller liknande begrepp som traditionella licensbaserade tillägg. Nya tillägg för handel, t.ex. traditionella licensbaserade, omfattar begreppet förutsättningar. Förutsättningar är produkt-SKU:er som kunden måste ha för att tillägget ska fungera korrekt. Kraven för ett tillägg finns i katalog-API:erna för en viss SKU och i användarupplevelsen i Partnercenter-katalogen. Köp av tillägg kräver att ett eller flera av förutsättningarna finns i kundens klientorganisation.

Den största skillnaden mellan traditionella och nya köp är hur **de** köps. Partner tillämpar tillägget till baserbjudandeprenumerationen i traditionella licensbaserade scenarier. Partner köper tillägg för ny handel från själva katalogen. Den här köpupplevelsen anpassar tilläggets identifiering till baserbjudandet, vilket gör det enklare att hitta och köpa tilläggen.

Många av begreppen om hur tillägg fungerar, ur ett tjänstperspektiv, förblir sanna inom traditionell och ny handel. Både traditionella och nya handelstransaktioner registrerar och etablerar tilläggstjänster. Etableringen sker på samma sätt i båda fallen. Dessutom kan ett enda tilläggstjänster komplettera fler än en basprodukt-SKU som tillägget är utformat för att fungera med.

## <a name="identifying-add-ons"></a>Identifiera tillägg

Partner kan identifiera tillägg och hämta listor med förutsättningar genom att granska SKU-informationen när de hämtar SKU:er via API:et. Tillägg identifieras också i den nya listan med licensbaserade priser för handel i kolumnen Taggar. Erbjudandematrisen innehåller en lista över krav för varje tilläggsprodukt-SKU.

## <a name="purchasing-add-ons"></a>Köpa tillägg

Tillägg finns för både traditionella licensbaserade och nya handelsupplevelser. Den viktigaste skillnaden är hur tilläggen identifieras. Nya köp-tillägg identifieras och köp från katalogen, på samma plats som baserbjudandena eller förutsättningarna hittas. Traditionella licensbaserade tillägg kan bara upptäckas och läggas till genom att gå till baserbjudandets prenumerationsinformationssida. 

Nya tillägg för köpupplevelsen identifieras och köps i själva katalogen. Partner kan filtrera efter tillägg för ny handel genom att välja listrutan produkttyp. Tilläggsprodukter identifieras med informationsikonen bredvid produktens SKU. Partner kan klicka på den här ikonen för att få mer information om förhandskrav för tillägget.

Partner kan få mer information om de produkter  som krävs för ett tillägg genom att klicka på Visa kompatibla basproduktprenumerationer för att visa en lista över produkt-SKU:er som måste finnas för att partnern ska kunna köpa ett visst tillägg.

## <a name="add-on-enforcement"></a>Tillämpning av tillägg

Partner ser användbar information om tillägg vid försök att köpa en ny tilläggsprodukt för handel när kunden inte har de förutsättningar som krävs. Partner kan kontrollera om förhandskrav för ett tillägg finns i Partnercenter-katalogen och granska sidupplevelser. Om tillägget inte har de nödvändiga kraven för stöd visar användargränssnittet meddelandet "The addon is not purchasable without a compatible base product" (Tillägget kan inte rensas utan en kompatibel basprodukt). Partner som använder CreateCart-API:et ser ett fel på kundvagnsraden om tillägget inte har nödvändiga produkt-SKU:er. Felkoden kommer att 400041 med beskrivningen "Tillägget kan inte rensas utan en kompatibel basprodukt".

## <a name="important-details-when-purchasing-add-ons"></a>Viktig information när du köper tillägg

Tillägg köps som distinkta produkt-SKU:er om kunden uppfyller kraven. Tilläggsprenumerationer har sin egen distinkta termjustering. Partner som köper tillägg kommer att märka att termen och det associerade slutdatumet kanske inte är samma som förutsättningarna. Så länge båda prenumerationerna förnyas automatiskt till nya villkor fortsätter kraven och tilläggen att fungera korrekt. Om partnern bestämmer sig för att avsluta den nödvändiga perioden genom att inte förnya automatiskt, bör tillägget också uppdateras så att det inte förnyas automatiskt i slutet av tilläggperioden om partnern drar slutsatsen att det inte längre behövs.  Partner konverterar en produkt-SKU till en högre SKU som redan har tilläggstjänster kan skicka en tjänstbegäran med stöd för att inaktivera ett tillägg.

Partner förväntas hantera termen slutdatum för tillägg som de får för att säkerställa att det finns en anpassning efter behov till baserbjudandena.
