---
title: Ny handel telco betala allt eftersom
ms.topic: article
ms.date: 09/03/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
description: Lär dig mer om nya handelsupplevelser för köperbjudanden som möjliggör betalning när du överköper.
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: b7f3fa6ce3b92e7b182192290f5ebb4ee167ff7a
ms.sourcegitcommit: 986573bc4382b803bf4d641df6dd1e37c3af1955
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/16/2021
ms.locfileid: "127872194"
---
# <a name="introduction-new-commerce-overage-for-telco-pay-as-you-go"></a>Introduktion: Överkurs i ny handel för telco-betalning allt eftersom

**Lämpliga roller**

- Administratörsagent
- Försäljningsagent
- Global administratör

> [!NOTE]
> De nya ändringarna i handelsupplevelsen är för närvarande endast tillgängliga för partner som ingår i den nya tekniska förhandsversionen av Microsoft 365/Dynamics 365.

Vissa licensbaserade produkter innehåller tjänster med allokerade anropsplaner. Dessa anropsplaner har vanligtvis en allokering per licens för minuter per månad, vanligtvis 120 per licens.

I traditionella licensbaserade partnerscenarier fanns det inget sätt att aktivera tjänstanvändning utöver de månatliga gränserna. Kunder som behöver mer än 120 minuter för att köpa kommunikationskrediter eller *själva kommunikationskrediten* direkt från Microsoft.  Dessa kommunikationskrediter erbjuds inte i Partnercenter.

## <a name="using-new-commerce-telco-pay-as-you-go"></a>Använda telco pay as you go med hjälp av ny handel ##

Den här begränsningen har åtgärdats i ny handel, vilket gör det möjligt för partnern att aktivera överkapacitet för tjänster som tillåter det. Partner kan köpa erbjudanden som innehåller överkapacitet. Dessa erbjudanden identifieras i kolumnen taggar för prislistan som *includeOverage*. Katalog-SKU:n innehåller också en egenskap för att fastställa att SKU:n stöder överkapaciteten. Partner köper bara erbjudandena och systemet konfigurerar och överutnyttjar prenumerationen, vilket inte kostar något och endast ackumulerar fakturering när kundens användare överser de allokerade månatliga samtalsminuterna som följer med det köpta erbjudandet.

Partner kan spåra överförbrukningsanvändning genom att gå till Azure Portal och använda kostnadshanteringsfunktioner. Partner har också möjlighet att när som helst ange övertiden till *Ingen* om de vill inaktivera eller inaktivera övertid när som helst.

Partner kan identifiera vilka produkter som innehåller överkapacitet genom att visa produkt-SKU:er för Partnercenter-katalogen. 

Partner som köper produkter med överagering aktiverar över tiden genom att gå till *hantera över- och över- eller* över- eller över-hantering på sidan Hantera prenumerationer. Detta gör att partnern kan aktivera överförbrukning och tilldela önskad förbrukningsprenumeration som överförbrukningsavgifterna flödar till. Partnern kan när som helst inaktivera överförbrukning genom att tilldela förbrukningsprenumerationen till *Ingen.*

Partner tilldelar överage eller inaktiverar det *med hjälp av funktionen Hantera över* funktion i prenumerationslistan. Detta är endast tillgängligt om partnern har prenumerationer som möjliggör överåtkomlig. Månatliga överavgifter påförs den tilldelade prenumerationen och identifieras i partneravstämningsfilen. Partner kan spåra överförbrukningsanvändning genom att besöka funktionerna för Azure-kostnadshantering i Azure Portal. 

## <a name="important-details-about-overage"></a>Viktig information om överage ##

Om du köper en produkt-SKU som möjliggör överströmning ser du automatiskt till att partnerns kund har ställts in för att överflödet ska flöda. Detta omfattar att skapa en Azure-plan utan kostnad, en associerad Azure-standardprenumeration och en prenumeration som är specifikt för överförbrukning. Partner kan se och tilldela den prenumeration de vill att överprenumerationen ska ackumuleras till i Hantera överage.

Övertilldelningen bestäms av den *första i* regeln. Om en partner köper E5 med anropsplaner för en ny kund kommer den här partnern att ha överförbrukning tilldelad till sin förbrukningsprenumeration. Om en andra partner köper en annan kopia av E5 med anropsplaner respekterar systemet den första partnerns köp och tilldelning. Partner kan alltid *hantera överning från* prenumerationssidan för att inaktivera eller inaktivera den genom att tilldela överning till *Ingen.*

Inställningarna för övernivå är per tjänst och kund. Om en kund har samma övertidstjänster från olika partner kan endast en övertidsprenumeration tilldelas i taget. Om överbehovet måste ändras från en partner till en annan måste de tre berörda parterna först komma överens. När de är överens kan den befintliga partnern helt enkelt ange överprenumeration till *Ingen,* vilket gör att den andra partnern kan ange överprenumeration till sin prenumeration.

API-stöd för funktioner för telco pay as you go är:

- SKU-egenskaper som hjälper partnern att identifiera om en SKU möjliggör över-
- Ett nytt API för att tilldela överning till en befintlig prenumeration eller för att ange över- och för lite till *Ingen*
