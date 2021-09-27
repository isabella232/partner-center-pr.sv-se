---
title: Ny handel , telco betala allt eftersom
ms.topic: article
ms.date: 09/03/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
description: Lär dig mer om nya handelsupplevelser för köperbjudanden som möjliggör betalning när du går över.
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: e6ca40f44b97a9b60b48ccedbed7a3df7baad465
ms.sourcegitcommit: d731813da1d31519dc2dc583d17899e5cf4ec1b2
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/27/2021
ms.locfileid: "129070236"
---
# <a name="introduction-new-commerce-overage-for-telco-pay-as-you-go"></a>Introduktion: Överkurs för ny handel för telco – betala enligt din go-betalning

**Lämpliga roller**

- Administratörsagent
- Försäljningsagent
- Global administratör

> [!NOTE]
> Ändringarna i den nya handelsupplevelsen är för närvarande endast tillgängliga för partner som ingår i den tekniska förhandsversionen av Microsoft 365/Dynamics 365.

Vissa licensbaserade produkter innehåller tjänster med allokerade anropsplaner. Dessa anropsplaner har vanligtvis en allokering per licens för minuter per månad, vanligtvis 120 per licens. 

I traditionella licensbaserade partnerscenarier fanns det inget sätt att aktivera tjänstanvändning utöver de månatliga gränserna. Kunder som behöver mer än 120 minuter för att köpa kommunikationskrediter eller *själva kommunikationskrediten* direkt från Microsoft.  Dessa kommunikationskrediter erbjuds inte i Partnercenter.

## <a name="using-new-commerce-telco-pay-as-you-go"></a>Använda telco pay för ny handel

Den här begränsningen har åtgärdats i ny handel så att partnern kan aktivera överkapacitet för tjänster som tillåter det. Partner kan köpa erbjudanden som omfattar överkapacitet. Dessa erbjudanden identifieras i kolumnen taggar för prislistan som *IncludeOverage*. Katalog-SKU:n innehåller också en egenskap för att fastställa att SKU:n stöder överkapaciteten. Partner köper bara erbjudandena och systemet konfigurerar och överprenumeration som inte är någon kostnad och endast ackumulerar fakturering när kundens användare överkommer de allokerade månatliga samtalsminuterna som följer med det köpta erbjudandet. 

Partner kan spåra överförbrukningsanvändning genom att gå till Azure Portal och använda funktioner och funktioner för kostnadshantering. Partner har också möjlighet att när som helst ange övertiden till *Ingen* om de vill inaktivera eller inaktivera övertid när som helst.

Partner kan identifiera vilka produkter som innehåller överkapacitet genom att visa produkt-SKU:er för Partner Center-katalogen. 

Partner som köper produkter med överköp möjliggör över- och överning genom att gå *till Hantera överköp* på sidan Hantera prenumerationer. Detta gör att partnern kan aktivera överförbrukning och tilldela önskad förbrukningsprenumeration som överförbrukningsavgifterna flödar till. Partnern kan när som helst inaktivera överförbrukning genom att tilldela förbrukningsprenumerationen till *Ingen.* 

Partner tilldelar överage eller inaktiverar den *med hjälp av funktionen Hantera över* huvud i prenumerationslistan. Detta är endast tillgängligt om partnern har prenumerationer som aktiverar överåtkomlig. Månatliga överkostnader påförs den tilldelade prenumerationen och identifieras i partneravstämningsfilen. Partner kan spåra överförbrukningsanvändning genom att besöka Funktionerna för Azure-kostnadshantering i Azure Portal. 

## <a name="important-details-about-overage"></a>Viktig information om överage

Om du köper en produkt-SKU som möjliggör överflöde ser du automatiskt till att partnerns kund har ställts in för att överflödet ska gå över. Detta omfattar att skapa en Azure-plan utan kostnad, en associerad Azure-standardprenumeration och en prenumeration som är specifikt för överförbrukning. Partner kan se och tilldela den prenumeration som de vill att över- och överningen ska ackumuleras till i Hantera överage.

Övertilldelningen bestäms av den *första i* regeln. Om en partner köper E5 med anropsplaner för en ny kund tilldelas den här partnern överförbrukningsprenumeration. Om en andra partner köper en annan kopia av E5 med anropsplaner respekterar systemet den första partnerns köp och tilldelning. Partner kan alltid *hantera överagering* från prenumerationssidan för att inaktivera eller inaktivera den genom att tilldela överning till *Ingen.*

Överdatainställningar är per tjänst per kund. Om en kund har samma övertidstjänster från olika partner kan endast en övertidsprenumeration tilldelas i taget. Om överbehovet måste ändras från en partner till en annan måste de tre berörda parterna först komma överens. När de är överens med den befintliga partnern kan du helt enkelt ange övereting till *Ingen,* vilket gör att den andra partnern kan ange överprenumeration till sin prenumeration.

API-stöd för telco betala allt eftersom funktioner är:

- SKU-egenskaper som hjälper partnern att identifiera om en SKU möjliggör över-
- Ett nytt API för att tilldela överbegäran till en befintlig prenumeration eller för att ange över- till *Ingen*
