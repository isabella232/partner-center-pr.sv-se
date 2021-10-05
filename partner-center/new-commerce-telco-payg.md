---
title: Ny handel , telco – betala enligt din go-betalning
ms.topic: article
ms.date: 09/03/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
description: Lär dig mer om nya köperbjudanden för köp av erbjudanden där du betalar för över tid.
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 8265cb3ce77183c4919e9b8e4e028bb66e8cd2f7
ms.sourcegitcommit: 462d6026287b85c9feea602af5bcdf924f3e6976
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 10/05/2021
ms.locfileid: "129452505"
---
# <a name="introduction-new-commerce-overage-for-telco-pay-as-you-go"></a>Introduktion: Överkurs för ny handel för telco – betala enligt din go-betalning

**Lämpliga roller**

- Administratörsagent
- Försäljningsagent
- Global administratör

> [!NOTE]
> Ändringarna i den nya handelsupplevelsen är för närvarande endast tillgängliga för partner som ingår i den tekniska förhandsversionen av Microsoft 365/Dynamics 365.

Vissa licensbaserade produkter innehåller tjänster med allokerade anropsplaner som vanligtvis innehåller en allokering per licens för minuter per månad, vanligtvis 120 per licens. 

I traditionella licensbaserade partnerscenarier fanns det inget sätt att aktivera tjänstanvändning utöver de månatliga gränserna. Kunder som behöver mer än 120 minuter för att köpa kommunikationskrediter eller *själva kommunikationskrediten* direkt från Microsoft.  Dessa kommunikationskrediter erbjuds inte i Partnercenter.

## <a name="using-new-commerce-telco-pay-as-you-go"></a>Använda ny handel med telco – betala enligt användning

Den här begränsningen har åtgärdats i ny handel så att partnern kan aktivera överkapacitet för tjänster som tillåter det. Partner kan köpa erbjudanden som omfattar överkapacitet. Dessa erbjudanden identifieras i kolumnen taggar för prislistan som *IncludeOverage*. Katalog-SKU:n innehåller också en egenskap för att fastställa att SKU:n stöder överkapaciteten. Partner köper bara erbjudandena och systemet konfigurerar en överprenumeration som inte kostar något och endast ackumulerar fakturering när kundens användare överkommer de allokerade månatliga samtalsminuterna som följer med det köpta erbjudandet. 

Partner kan identifiera vilka produkt-SKU:er som omfattar överkapacitet genom att 

- Visa produkt-SKU:er för Partner Center-katalogen
- Filtrera den nya handelsprislistan efter **includesOverage** i taggkolumnen

Partner som köper produkter med överage aktiverar det genom att gå **till Hantera överköp** på sidan Hantera prenumerationer. Gränssnittet för hantering av överlagring gör det möjligt för partnern att aktivera och tilldela vilken Azure-prenumeration som överlagringsavgifterna flödar till. Partnern kan när som helst inaktivera överförbrukning genom att tilldela förbrukningsprenumerationen till *Ingen.* 

Partner tilldelar överage eller inaktiverar den *med hjälp av funktionen Hantera över* huvud i prenumerationslistan. Detta är endast tillgängligt om partnern har prenumerationer som aktiverar överåtkomlig. Månatliga överkostnader påförs den tilldelade prenumerationen och identifieras i partneravstämningsfilen. Partner kan spåra överförbrukningsanvändning genom att besöka Funktionerna för Azure-kostnadshantering i Azure Portal. 

Partner kan spåra överförbrukningsanvändning genom att gå till Azure Portal och använda kostnadshanteringsfunktioner. 

## <a name="important-details-about-overage"></a>Viktig information om överage

- Att köpa en licensbaserad produkt-SKU som innehåller överkapacitet köper endast den licensbaserade produkten. Partner måste vidta ytterligare ett steg efter inköp för att aktivera överhantering genom att gå till prenumerationshanteringssidan och klicka på **Hantera överhantering**
- Endast administratörsagenter för den hanterande partnern kan aktivera övergående efter det licensbaserade köpet. 
- Om du aktiverar överförbrukning skapas en Azure-plan utan kostnad och en associerad azure-standardprenumeration **prenumeration 1** specifikt för överförbrukning. Om Azure-planen redan finns skapar aktivering av överlagring den nya prenumerationen under den befintliga Azure-planen. Partner kan alltid visa eller omtilldela överning till andra prenumerationer i **Hantera överköp.** Kunder som ännu inte har en Azure-plan (äldre Azure) måste övergå till Azure-planen innan de kan aktivera övertid.

Övertilldelningen bestäms av den *första i* regeln. Om en partner köper E5 med anropsplaner för en ny kund tilldelas den här partnern överförbrukningsprenumeration. Om en andra partner köper en annan kopia av E5 med anropsplaner respekterar systemet den första partnerns köp och tilldelning. Partner kan alltid *hantera överagering* från prenumerationssidan för att inaktivera eller inaktivera den genom att tilldela överning till *Ingen.*

Överdatainställningar är per tjänst per kund. Endast en övertidsprenumeration kan tilldelas i taget. Om överbehovet måste ändras från en partner till en annan måste de tre berörda parterna först komma överens. När de är överens med den befintliga partnern kan du helt enkelt ange övereting till *Ingen,* vilket gör att den andra partnern kan ange överprenumeration till sin prenumeration.

## <a name="telco-pay-as-you-go-apis"></a>Telco-API:er där du betalar enligt din go-betalning

- [SKU-egenskaper](/partner-center/develop/product-resources#sku) innehåller en *consumptionType-egenskap* som hjälper partnern att identifiera om en SKU möjliggör överförbrukning
- [Få övereting](/partner-center/develop/get-subscription-overage) för att förstå om överdata har ställts in för kunden
- [Uppdatera överlagring](/partner-center/develop/update-subscription-overage) för att uppdatera kundens överlagring till en Azure-prenumeration eller ange den till *Ingen*
