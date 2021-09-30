---
title: Nya handelskampanjer
ms.topic: article
ms.date: 09/29/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
description: Lär dig mer om nya handelsupplevelser för att upptäcka och köpa kampanjer.
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 45411827f200f205dc20b9a9c2d60519d4aba4eb
ms.sourcegitcommit: a59e1abb470f4847e8f8337ffa4ba705514a0424
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/29/2021
ms.locfileid: "129249318"
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

Partner kan operationalisera kampanjerna genom att implementera [getPromotions-API:et](/partner-center/develop/get-promotions). Detta API returnerar alla kampanjer som finns för en viss marknad (kundens land) och segment. API:et returnerar listan över kampanjer och viktig information som hjälper partnern att förstå vilka kampanjer som är tillgängliga för kunder i olika länder. 


API:et getPromotions innehåller följande data för en viss befordran:

- Befordrans varaktighet
- Procentrabatten för befordran
- De produkter och SKU:er som befordran är tillgänglig för

Kampanjer tillämpas av partnercentret när partnern köper produkt-SKU:n som befordran är tillgänglig för. Partnerkampanjer är tillgängliga i användargränssnittet för partnercenterkatalogen i produkt-SKU-informationen. De kan klicka på "Visa kampanjinformation" för att få mer information om befordran. Möjligheten att visa kampanjinformationen kan nås från SKU-informationen för katalogsidan, granskningssidan innan du skickar in köpet, bekräftelsen efter att ordern har skickats och sidan för orderhistorik. 

## <a name="verify-eligibility"></a>Verifiera berättigande ##

Partner kan se om ett kundköp är berättigat till en befordran genom att se informationen på granskningssidan i partnercenter innan de köper produkten. Partner kan också anropa API:et [verifyPromotionEligibility](/partner-center/develop/verify-promotion-eligibility)och skicka kundens klientorganisations-ID och uppflyttnings-ID. Anropet returnerar true om kunden är berättigad. Om kunden inte är berättigad returnerar API:et de villkor som inte uppfylldes för att befordran skulle vara tillämplig. 

Partner kan anropa verifiera berättigande och få tillbaka resultat. Berättigandefel kan baseras på antal platser, inkompatibla villkor eller gränser för hur många gånger en befordran kan tillämpas på en kunds produkt-SKU.

Viktiga ämnen för api:er för nya handelskampanjer:

- [GetPromotions-API](/partner-center/develop/get-promotions)
- [GetPromotionsById API](/partner-center/develop/get-promotion-by-id)
- [VerifyPromtionEligibilities](/partner-center/develop/verify-promotion-eligibility)
- [Kampanjresurser](/partner-center/develop/promotion-resources)

>[!IMPORTANT]
> Partner bör verifiera kampanjer innan de skickar en transaktion. Om en befordran *inte visas* på partnercentrets granskningssida tillämpas den inte på transaktionen. Partnern får priset för icke-befordran. Partner kan också titta på API:et för kundvagnsraden för att se om befordran finns innan en transaktion skickas. Partner kan anropa API:et för verifiering av kampanjer innan de skickar transaktioner för att verifiera att kombinationen av kundprodukt-SKU är berättigad för befordran och om inte, orsakerna till inkompatibiliteten.

Det finns tre orsaker till att en kund kanske inte är berättigad till en befordran. Dessa ej berättigade typer returneras i API:et för valideringsbefordran i fall där kunden inte är berättigad.

### <a name="seat-count"></a>Antal platser ###

Många kampanjer har en plats som maximalt kan vara 2 400 platser. I dessa fall skickas en transaktion med fler än 2 400 till priserna för icke-befordran. Det här antalet platser tillämpas också när du lägger till platser i en uppflyttningsprenumeration med dessa gränser. Partner får ett felmeddelande om de försöker öka en prenumeration som är aktiverad för befordran utöver gränserna. Platsbegränsningarna från kampanjer tillämpas mellan partner, så om en partner köper en befordran på 2 300 platser med en gräns för uppflyttningsplatser får en andra partner som köper 200 platser prenumerationspriset till priset för icke-befordran. Befordran tillämpas på den produkt-SKU-nivå som partnern gör, så en partner kan få kampanjpriser för 2 400 platser med Microsoft 365 E3 och även för en annan produkt-SKU Microsoft 365 E5. Partner kan anropa [API:et subscribedSKUs](/partner-center/develop/get-a-list-of-available-licenses) för att se hur många licenser en kund har för en viss etablerat SKU.

Om en partner vill ha fler licenser än de 2 400 platserna och de vill ha befordran, kan partnern helt enkelt köpa en prenumeration upp till gränsen på 2 400 till kampanjpriset och en andra prenumeration till priset för icke-befordran.

### <a name="term"></a>Period ###

Villkorsbegränsningar definierar vilka produkt-SKU-termer som passar för en viss befordran. Många kampanjer har olika rabatter som definierats baserat på termen. Om en partner skickar en transaktion och termen inte överensstämmer med befordran förväntar de sig att transaktionen kommer att ha det pris för icke-befordran som de förväntar sig. Exempel på villkor är *årlig eller* *månatlig*.

### <a name="first-purchase"></a>Första köpet ###

Vissa kampanjer framtvingas endast en gång. En partner ser behörigheten false med *hjälp av* API:et för validering av berättigande med feltypen *FirstPurchase*. En partner kan fortfarande köpa den angivna produkt-SKU:n, men prenumerationen kommer att ha priset för icke-befordran. Den här begränsningen gäller per kund, inte per partner. När en kund har en befordran med den här regeln kan de inte få en andra instans av befordran tillämpad av en andra partner.

## <a name="promotions-and-renewals"></a>Kampanjer och förnyelser ##

Kampanjrabatter som tillämpas gäller för inköpperioden. Prenumerationer med tillämpade kampanjer behåller kampanjpriset om förnyelsedatumet är inom datumintervallet för befordrans varaktighet. Förnyelser utanför datumintervallet för befordran förnyas till priset för icke-befordran (från prislistan). Partner kan spåra förnyelsestatusen till prispunkterna på sidan med prenumerationsinformation och i instruktionerna för att förnya getSubscription-data.

## <a name="promotions-and-upgrades"></a>Kampanjer och uppgraderingar ##
Partner som uppgraderar från en prenumeration till en annan SKU lämnar kampanjpriset kvar. Den här åtgärden beror på att befordran har konfigurerats för den SKU som de lämnar när de uppgraderar till en annan SKU. Partner som uppgraderar till en SKU som kan ha en befordran får inte automatiskt kampanjpriset. Om de behöver eller vill ha kampanjpriset för den SKU som de vill flytta till måste de köpa den nya SKU:n manuellt som en ny prenumeration. För närvarande tillämpas kampanjer endast på nya prenumerationsköp och förnyelser.

## <a name="promotions-and-migrations"></a>Kampanjer och migreringar ##
Partner kan migrera sina kunders prenumerationer från traditionella Microsoft 365/Dynamics 365 till nya handelsversioner av sina prenumerationer. Migreringarna är tillgängliga både från Partner Center-användargränssnittet eller från att anropa migrerings-API:erna. Partner som migrerar från en traditionell prenumeration till ny handel får befordran när de migrerar så länge produkt-SKU:n de flyttar till överensstämmer med befordransdefinitionen. Partner bör anropa API:et för verifiering av berättigande för att säkerställa att målproduktens SKU tillämpar kampanjpriset före migreringen.

## <a name="cross-channel-considerations"></a>Överväganden för flera kanaler ##
Molnlösningsleverantör (CSP) begränsningar och begränsningar tillämpas inte i kanaler, till exempel Enterprise-avtal (EA). En CSP-partner kan erhålla en befordran med en begränsning på 2 400 befordran även om kunden kan ha 3 000 platser från EA.  
