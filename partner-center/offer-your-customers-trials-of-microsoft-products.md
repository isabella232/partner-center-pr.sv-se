---
title: Erbjuda kunderna utvärderingsversioner av Microsoft-produkter
ms.topic: article
ms.date: 08/22/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
description: Låt kunderna prova microsoftprenumerationsprodukter. Registrera dig för dessa kostnadsfria utvärderingsversioner i katalogen precis som många andra onlinetjänster.
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 48f4c81f217e68836dd755d1d4342d240276ea79
ms.sourcegitcommit: 1e616b52d55eff41d67a081ba3f4a8370a49e027
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/29/2021
ms.locfileid: "129191506"
---
# <a name="give-customers-free-trials-of-microsoft-products"></a>Ge kunderna kostnadsfria utvärderingsversioner av Microsoft-produkter

**Lämpliga roller:** Global | Administratörsbehörighet för användarhantering | Försäljningsagent

Ett bra sätt att introducera kunder till nya Microsoft-produkter är att erbjuda 30 dagars kostnadsfria utvärderingsversioner. Du kan registrera dig för utvärderingsversioner i katalogen precis som många andra onlinetjänster. Alla partner kan delta.

## <a name="available-trial-offers"></a>Tillgängliga utvärderingserbjudanden

Du hittar alla dina utestående utvärderingserbjudanden på **sidan** Kund. På den här sidan visas alla prenumerationer, inklusive kostnadsfria utvärderingsversioner och betalda prenumerationer. (Den här funktionen är för närvarande inte tillgänglig i Kina.)

Varje kund har rätt till en kostnadsfri utvärderingsversion för varje tillgängligt erbjudande. De kan till exempel få en kostnadsfri utvärderingsversion Microsoft 365 Business Standard en kostnadsfri utvärderingsversion för Office 365 E3. Men om kunden redan äger erbjudandet kan kunden inte använda en kostnadsfri utvärderingsversion av erbjudandet.

### <a name="available-products"></a>Tillgängliga produkter

Kostnadsfria utvärderingsversioner är tillgängliga för de mest omfattande och populära erbjudandena. Nya utvärderingserbjudanden kan introduceras månadsvis.

Partner hittar utvärderingsversioner i den månatliga prislistan på **sidan med priser och** erbjudanden i Partnercenter. Utvärderingserbjudandena visas med "UTVÄRDERINGSVERSION" i kolumnen **Sekundär licenstyp** i prislistan.

För närvarande finns det **inga kostnadsfria utvärderingsversioner** för myndighetserbjudanden, utbildningserbjudanden eller tilläggserbjudanden.

## <a name="licenses-for-free-trial-offers"></a>Licenser för kostnadsfria utvärderingserbjudanden

Alla kostnadsfria utvärderingsversioner har 25 licenser. Du kan inte ändra det här antalet under utvärderingsperioden. Du kan inte lägga till eller ta bort licenser i den kostnadsfria utvärderingsversionen. När utvärderingsversionen har konverterats till en betald prenumeration kan du lägga till fler licenser i prenumerationen.

Utvärderingslicenser ska tilldelas till användare på samma sätt som licensen för betaltjänster tilldelas.

## <a name="sign-customers-up-for-trials"></a>Registrera kunder för utvärderingsversioner

Skaffa en utvärderingsversion för din kund i Partnercenter:

1. Från **Sälj** på Partnercenter går du till **Katalog.** 
2. I katalogen går du till **Faktureringsfrekvens och** väljer **Utvärderingserbjudande.** Detta gör att endast kostnadsfria utvärderingsversioner visas och inaktiverar andra erbjudanden som inte är kostnadsfria. Utvärderingsversioner visas på **fliken Utvärderingsversioner** i katalogen.
3. Välj den kostnadsfria utvärderingsversion som du vill erbjuda och välj sedan **Skicka**. Alla utvärderingsversioner gäller i 30 dagar då du inte debiteras. Du kan också konvertera den till en betald prenumeration när som helst under utvärderingsperioden.

## <a name="converting-trials-to-paid-subscriptions"></a>Konvertera utvärderingsversioner till betalda prenumerationer

En kostnadsfri utvärderingsversion konverteras inte automatiskt till en betald prenumeration. Efter 30 dagar måste en kostnadsfri utvärderingsversion konverteras till en betald prenumeration, annars upphör den att [gälla.](#expiring-offers) Kostnadsfria utvärderingsversioner kan inte utökas.

Du måste konvertera utvärderingsversionen till en betald prenumeration själv. Du kan göra detta [med hjälp av Partnercenter eller](#convert-trials-using-partner-center) via Partner [Center-API:erna](#convert-trials-using-apis).

> [!NOTE]
> Kundfria utvärderingsversioner av Molnlösningsleverantör-programmet (CSP) kan inte konverteras till en annan programklientorganisation (till exempel EA, Open eller MOSP).

### <a name="convert-trials-using-partner-center"></a>Konvertera utvärderingsversioner med Partnercenter

Du kan konvertera utvärderingsversioner till betalda prenumerationer med partnercenter:

1. Gå till kundens prenumerationssida och välj den kostnadsfria utvärderingsversionen.
2. Välj **Konvertera utvärderingsversion till betald prenumeration.**
3. Ange önskad licenskvantitet och faktureringsfrekvens och välj **Tillämpa**.
4. Faktureringen för den betalda prenumerationen börjar på konverteringsdatumet och prenumerationen förnyas automatiskt 12 månader från konverteringsdatumet. 

### <a name="convert-trials-using-apis"></a>Konvertera utvärderingsversioner med API:er

Du kan behöva ändra dina API:er för att anpassa konverteringen av en kostnadsfri utvärderingsversion till en betald prenumeration. Mer information finns i följande utvecklardokumentation:

- [Konvertera en utvärderingsprenumeration till betald](/partner-center/develop/convert-a-trial-subscription-to-paid)
- [Hämta en lista över erbjudanden för utvärderingskonvertering](/partner-center/develop/get-a-list-of-trial-conversion-offers)

### <a name="trials-without-conversions"></a>Utvärderingsversioner utan konverteringar

Det är inte alla utvärderingsversioner som kan konverteras till betalda prenumerationer. Partner kan använda en utvärderingsversion som inte har några konverteringar förrän förfallodatumet. Partner kan köpa kompatibla erbjudanden som stöder samma tjänster som utvärderingserbjudandet.  Detta bör göras innan utvärderingsversionen upphör att gälla för att säkerställa att de nyligen köpta erbjudandena överensstämmer med utvärderingsversionens tjänster. 

|**Utvärdering**   |**Kompatibla erbjudanden för små företag**   |**Kompatibla Enterprise-erbjudanden**   |
|----------------------------|:---------------------------------|:------------------------------------------|
|Microsoft Teams Utvärderingsversion av commercial cloud (användarinitierad)   |Microsoft 365 Business Basic, Microsoft 365 Business Standard, Microsoft 365 Business Premium   | F3 (tidigare F1), Office 365 for Enterprise (E1, E3 och E5), Microsoft 365 F1/F3, Microsoft 365 Enterprise (E3)   |

> [!NOTE]
> Erbjudandena ovan har liknande tjänstplaner med liknande funktioner, men det kan finnas vissa skillnader mellan erbjudandena.

### <a name="expiring-offers"></a>Erbjudanden som upphör att gälla

Du kommer inte att meddelas om att erbjudanden upphör att gälla. Du kan spåra kommande förfallodatum med hjälp av kundvyn i Partnercenter eller genom att fråga API:et. Det är en bra idé att övervaka dessa datum ofta så att du kan vidta lämpliga uppföljningsåtgärder med kunderna när de närmar sig en beslutspunkt.

När en utvärderingsversion har gått ut visas ett meddelande om att en kund försöker logga in på den utvärderingsversionen. Data lagras dock i enlighet med datalagringsstandarder. När du har köpt en ny prenumeration med samma tjänstplaner kan du komma åt kundens information igen från den nyligen aktiverade prenumerationen.

## <a name="converting-new-commerce-trials-to-paid-subscriptions"></a>Konvertera nya utvärderingsversioner av handel till betalda prenumerationer

> [!NOTE]
> Nya handelsändringar är för närvarande endast tillgängliga för partner som ingår i den tekniska förhandsversionen av den nya handelsupplevelsen M365/D365.

Efter 30 dagar förnyas den kostnadsfria utvärderingsversionen automatiskt till en betald prenumeration. Du kan konvertera din utvärderingsversion före den automatiska förnyelsen genom att följa stegen nedan. 

Du kan konvertera utvärderingsversionen till en betald prenumeration själv. Du kan göra detta med hjälp av Partnercenter eller via Partner Center-API:erna. 

> [!NOTE]
> Kundfria utvärderingsversioner av Molnlösningsleverantör-programmet (CSP) kan inte konverteras till en annan programklientorganisation (till exempel EA, Open eller MOSP).

### <a name="convert-new-commerce-trials-using-partner-center"></a>Konvertera nya handelsversioner med Partnercenter

> [!NOTE]
> Nya handelsändringar är för närvarande endast tillgängliga för partner som ingår i den tekniska förhandsversionen av den nya handelsupplevelsen M365/D365.

Du kan konvertera nya utvärderingsversioner av handel till betalda prenumerationer med partnercenter:

1. Gå till kundens prenumerationssida och välj den kostnadsfria utvärderingsversionen.
2. Välj **Konvertera utvärderingsversion till betald prenumeration.**
3. Välj den betalda motsvarigheten och välj sedan **Skicka**.
4. Faktureringen för den betalda prenumerationen börjar på konverteringsdatumet och prenumerationen förnyas automatiskt tolv månader från konverteringsdatumet.

## <a name="billing"></a>Fakturering

Årlig fakturering och kostnadsfria utvärderingsversioner är desamma i nationella moln och det offentliga molnet. Den enda skillnaden är de utvärderings-SKU:er som är tillgängliga vid tidpunkten för start.

## <a name="billing-for-free-trials"></a>Fakturering för kostnadsfria utvärderingsversioner

Kostnadsfria utvärderingsversioner kan användas för både månatliga och årliga fakturerade prenumerationer. Du kan välja faktureringsfrekvens när du konverterar utvärderingsversionen till en betald prenumeration.

Startdatumet för prenumerationen baseras på konverteringsdatumet. Om den kostnadsfria utvärderingsversionen konverteras till ett betalt erbjudande med årlig fakturering är förnyelsedatumet för prenumerationen 12 månader från konverteringsdatumet. Om den kostnadsfria utvärderingsversionen konverteras till ett betalt erbjudande med månatlig fakturering är förnyelsedatumet för prenumerationen tolv månader från faktureringsdatumet efter konverteringsdatumet.

### <a name="invoices"></a>Fakturor

Kostnadsfria utvärderingsversioner visas inte i din faktura eller licensbaserade avstämningsfil. Kostnadsfria utvärderingsversioner visas bara på din faktura och licensbaserade avstämningsfil när du har konverterat en kostnadsfri utvärderingsversion till en betald prenumeration. Den konverterade prenumerationen visas på samma sätt som alla nya prenumerationer.

### <a name="incentives"></a>Incitament

Kostnadsfria utvärderingsversioner påverkar inte incitamenten.

## <a name="support"></a>Support

Om du vill ha support för kostnadsfria utvärderingsversioner skickar du en tjänstbegäran via Partnercenter.
