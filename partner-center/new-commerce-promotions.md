---
title: Nya handelskampanjer
ms.topic: article
ms.date: 09/03/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
description: Lär dig mer om nya handelsupplevelser för att upptäcka och köpa kampanjer.
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: dc2d52dd444168b32f0cadaeccec1e6d906348d1
ms.sourcegitcommit: 847ad384d44a5a673791cb2950af02225d8174c9
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/17/2021
ms.locfileid: "127906340"
---
# <a name="introduction-new-commerce-promotions"></a>Introduktion: Nya handelskampanjer

**Lämpliga roller**

- Administratörsagent
- Försäljningsagent
- Global administratör

> [!Note] 
> Ändringarna i den nya handelsupplevelsen är för närvarande endast tillgängliga för partner som ingår i den tekniska förhandsversionen av Microsoft 365/Dynamics 365.

Microsoft kommer att stödja kampanjer inom ny handel. Dessa kampanjer har olika rabattbelopp och varaktigheter. 

## <a name="discovering-promotions"></a>Upptäcka kampanjer ##

Partner kan identifiera kampanjer genom att besöka sökningsloggarna eller genom att anropa API:et getPromotions. Listan över listan över lista över kampanjer som våra partner behöver känna till. Listan underhålls och uppdateras varje månad. 


## <a name="operationalize-promotions"></a>Operationalisera kampanjer ##

Partner kan operationalisera kampanjerna genom att implementera getPromotions-API:et. Detta API returnerar alla kampanjer som finns för en viss marknad (kundens land) och segment. API:et returnerar listan över kampanjer och viktig information som hjälper partnern att förstå vilka kampanjer som är tillgängliga för kunder i olika länder. 


API:et getPromotions innehåller följande data för en viss befordran:

- Befordrans varaktighet
- Procentrabatten för befordran
- De produkter och SKU:er som befordran är tillgänglig för

Kampanjer tillämpas av partnercentret när partnern köper produkt-SKU:n som befordran är tillgänglig för. Partnerkampanjer är tillgängliga i användargränssnittet för Partner Center-katalogen i produkt-SKU-informationen. De kan klicka på "Visa kampanjinformation" för att få mer information om befordran. Möjligheten att visa kampanjinformationen kan nås från SKU-informationen för katalogsidan, granskningssidan innan du skickar in köpet, bekräftelsen efter att ordern har skickats och sidan för orderhistorik. 


## <a name="verify-eligibility"></a>Verifiera berättigande ##

Partner kan se om ett kundköp är berättigat till en befordran genom att se informationen på granskningssidan i partnercenter innan de köper produkten. Partner kan också anropa API:et verifyPromotionEligibility och skicka kundens klientorganisations-ID och uppflyttnings-ID. Anropet returnerar true om kunden är berättigad. Om kunden inte är berättigad returnerar API:et de villkor som inte uppfylldes för att befordran skulle vara tillämplig. 



## <a name="promotions-and-renewals"></a>Kampanjer och förnyelser ##

Kampanjrabatter som tillämpas gäller för inköpperioden. Prenumerationer med tillämpade kampanjer behåller kampanjpriset om förnyelsedatumet är inom datumintervallet för befordrans varaktighet. Förnyelser utanför datumintervallet för befordran förnyas till priset för icke-befordran (från prislistan). Partner kan spåra förnyelsestatusen till prispunkterna på sidan med prenumerationsinformation och i instruktionerna för att förnya getSubscription-data.


## <a name="promotions-and-upgrades"></a>Kampanjer och uppgraderingar ##
Partner som uppgraderar från en prenumeration till en annan SKU lämnar kampanjpriset kvar. Den här åtgärden beror på att befordran har konfigurerats för den SKU som de lämnar när de uppgraderar till en annan SKU. Partner som uppgraderar till en SKU som kan ha en befordran får inte automatiskt kampanjpriset. Om de behöver eller vill ha kampanjpriset för den SKU som de vill flytta till måste de köpa den nya SKU:n manuellt som en ny prenumeration. För närvarande tillämpas kampanjer endast på nya prenumerationsköp och förnyelser.



