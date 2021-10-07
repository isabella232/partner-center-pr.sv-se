---
title: Ny handel , telco – betala enligt din go-betalning
ms.topic: article
ms.date: 09/03/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
description: Lär dig mer om nya handelsupplevelser för köperbjudanden som möjliggör betala vid överköp.
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: a6abf0a837758819fba8c3a584ba68216657a2b9
ms.sourcegitcommit: 76a7dac540d129ae15cd4c251a4ff43d768370da
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 10/06/2021
ms.locfileid: "129593250"
---
# <a name="introduction-new-commerce-overage-for-telco-pay-as-you-go"></a>Introduktion: Överkurs i ny handel för telco betala enligt din go-betalning

**Lämpliga roller**

- Administratörsagent
- Försäljningsagent
- Global administratör

> [!NOTE]
> De nya ändringarna i handelsupplevelsen är för närvarande endast tillgängliga för partner som ingår i den nya tekniska förhandsversionen av Microsoft 365/Dynamics 365.

Vissa licensbaserade produkter innehåller tjänster med allokerade anropsplaner som vanligtvis inkluderar en allokering per licens för minuter per månad, vanligtvis 120 per licens. 

I traditionella licensbaserade partnerscenarier fanns det inget sätt att aktivera tjänstanvändning utöver de månatliga gränserna. Kunder som behöver mer än 120 minuter för att köpa kommunikationskrediter eller *själva kommunikationskrediten* direkt från Microsoft.  Dessa kommunikationskrediter erbjuds inte i Partnercenter.

## <a name="using-new-commerce-telco-pay-as-you-go"></a>Använda ny handel med Telco – betala enligt användning

Den här begränsningen har åtgärdats i ny handel, vilket gör det möjligt för partnern att aktivera överkapacitet för tjänster som tillåter det. Partner kan köpa erbjudanden som innehåller överkapacitet. Dessa erbjudanden identifieras i kolumnen taggar för prislistan som *includeOverage*. Katalog-SKU:n innehåller också en egenskap för att fastställa att SKU:n stöder överkapaciteten. Partner köper bara erbjudandena och systemet konfigurerar en överprenumeration som inte är någon kostnad och endast ackumulerar fakturering när kundens användare överser de allokerade månatliga samtalsminuterna som följer med det köpta erbjudandet. 

Partner kan identifiera vilka produkt-SKU:er som innehåller överkapacitet genom att 

- Visa produkt-SKU:er för Partner center-katalogen
- Filtrera den nya handelsprislistan efter **includesOverage** i taggkolumnen

Partner som köper produkter med överagering aktiverar det genom att **gå till hantera överköp** på sidan Hantera prenumerationer. Gränssnittet för hantering av överlagring gör att partnern kan aktivera och tilldela vilken Azure-prenumeration överlagringsavgifterna ska flöda till. Partnern kan när som helst inaktivera överförbrukning genom att tilldela förbrukningsprenumerationen till *Ingen.* 

> [!NOTE]
> Hantera överlagring kräver möjligheten att skapa en Azure-plan. Som standard kan partner inte etablera Azure-planer med sina sandbox-konton. Partner som behöver göra det med sitt sandbox-konto måste ansöka om åtkomst. Mer infromation finns i sandbox-dokumentationen för [Azure-plan.](/partner-center/develop/test-and-debug#azure-plan)

Partner tilldelar överage eller inaktiverar det *med hjälp av funktionen Hantera över* funktion i prenumerationslistan. Detta är endast tillgängligt om partnern har prenumerationer som möjliggör överåtkomlig. Månatliga överavgifter påförs den tilldelade prenumerationen och identifieras i partneravstämningsfilen. Partner kan spåra överförbrukningsanvändning genom att besöka funktionerna för Azure-kostnadshantering i Azure Portal. 

Partner kan spåra överförbrukningsanvändning genom att gå till Azure Portal och använda funktioner för kostnadshantering. 

## <a name="important-details-about-overage"></a>Viktig information om överage

- Om du köper en licensbaserad produkt-SKU som innehåller överkapacitet köps endast den licensbaserade produkten. Partner måste vidta ytterligare ett steg efter inköp för att aktivera överhantering genom att gå till prenumerationshanteringssidan och klicka på **Hantera överhantering**
- Endast administratörsagenter för den transacting-partnern kan aktivera övergående efter det licensbaserade köpet. 
- Om du aktiverar överförbrukning skapas en Azure-plan utan kostnad och en associerad azure-standardprenumeration **1** specifikt för överförbrukning. Om Azure-planen redan finns skapar aktivering av överlagring den nya prenumerationen under den befintliga Azure-planen. Partner kan alltid visa eller omtilldela överning till andra prenumerationer i **Hantera överage.** Kunder som ännu inte har en Azure-plan (äldre Azure) måste övergå till En Azure-plan innan de kan aktivera överlagring.

Övertilldelningen bestäms av den *första i* regeln. Om en partner köper E5 med anropsplaner för en ny kund kommer den här partnern att ha överförbrukning tilldelad till sin förbrukningsprenumeration. Om en andra partner köper en annan kopia av E5 med anropsplaner respekterar systemet den första partnerns köp och tilldelning. Partner kan alltid *hantera överning från* prenumerationssidan för att inaktivera eller inaktivera den genom att tilldela överning till *Ingen.*

Inställningarna för övernivå är per tjänst och kund. Endast en övertidsprenumeration kan tilldelas i taget. Om överbehovet måste ändras från en partner till en annan måste de tre berörda parterna först komma överens. När de är överens kan den befintliga partnern helt enkelt ange överprenumeration till *Ingen,* vilket gör att den andra partnern kan ange överprenumeration till sin prenumeration.

## <a name="telco-pay-as-you-go-apis"></a>Telco-API:er med betala/du-betalning

- [SKU-egenskaper](/partner-center/develop/product-resources#sku) innehåller en *consumptionType-egenskap* som hjälper partnern att identifiera om en SKU möjliggör överförbrukning
- [Få överning](/partner-center/develop/get-subscription-overage) för att förstå om någon överning har ställts in för din kund
- [Uppdatera överlagring](/partner-center/develop/update-subscription-overage) för att uppdatera kundens överlagring till en Azure-prenumeration eller ange den till *Ingen*
