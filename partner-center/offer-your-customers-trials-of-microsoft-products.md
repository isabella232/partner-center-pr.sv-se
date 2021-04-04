---
title: Erbjud kunderna utvärderings versioner av Microsofts produkter
ms.topic: article
ms.date: 05/04/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Låt kunderna testa prenumerations produkter från Microsoft i 30 dagar. Registrera dig för de här kostnads fria utvärderingarna i katalogen precis som många andra onlinetjänster.
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 53f4a16ac5d0f33fd534d7fd9a13eaf5a25cf3ea
ms.sourcegitcommit: f24089cd27b1de6ecf6ddbefb6cbb2d340e144de
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/01/2021
ms.locfileid: "106132340"
---
# <a name="give-customers-30-day-free-trials-of-microsoft-products"></a>Ge kunderna 30 dagars kostnads fria utvärderings versioner av Microsofts produkter

**Lämpliga roller**

- Global administratör
- Administratör för användar hantering
- Försäljnings agent

Ett bra sätt att lansera kunder på nya Microsoft-produkter är att erbjuda 30 dagars kostnads fria utvärderings versioner. Du kan registrera dig för test versioner i katalogen precis som många andra onlinetjänster. Alla partner kan delta.

## <a name="available-trial-offers"></a>Tillgängliga utvärderings erbjudanden

Du hittar alla dina utestående utvärderings erbjudanden på **kund** sidan. Den här sidan listar alla prenumerationer, inklusive kostnads fria utvärderingar och betalda prenumerationer. (Den här funktionen är för närvarande inte tillgänglig i Kina.)

Varje kund har rätt till en kostnads fri utvärderings version för varje tillgängligt erbjudande. De kan till exempel få en kostnads fri utvärderings version av Microsoft 365 Business Standard och en kostnads fri utvärderings version för Office 365 E3. Men om kunden redan äger erbjudandet kan de inte använda en kostnads fri utvärderings version för det erbjudandet.

### <a name="available-products"></a>Tillgängliga produkter

Kostnads fria utvärderings versioner är tillgängliga för de mest omfattande och populära licesen-baserade erbjudandena. Nya utvärderings erbjudanden kan införas varje månad.

Partners kan hitta utvärderings versioner i månads pris listan på sidan **priser och erbjudanden** i Partner Center. Utvärderings versionen har "utvärdering" som visas i kolumnen pris lista för **sekundär licens typ** .

För närvarande finns det **inga kostnads fria utvärderingar** för myndighets erbjudanden, utbildnings erbjudanden eller erbjudanden om tillägg.

## <a name="licenses-for-free-trial-offers"></a>Licenser för kostnads fria utvärderings erbjudanden

Alla kostnads fria utvärderings versioner tillhandahåller 25 licenser. Du kan inte ändra det här numret under utvärderings perioden. Du kan inte lägga till eller ta bort licenser i den kostnads fria utvärderings versionen. När utvärderings versionen har konverterats till en betald prenumeration kan du lägga till fler licenser i prenumerationen.

Utvärderings licenser ska tilldelas till användare på samma sätt som betalda tjänster licens tilldelas.

## <a name="sign-customers-up-for-trials"></a>Registrera kunder för utvärderings versioner

Få en utvärderings version av din kund i Partner Center:

1. Gå till **katalogen** från **Sälj** Partner Center. 
2. I katalogen, från **fakturerings frekvens**, väljer du **utvärderings erbjudande**. Detta gör att endast kostnads fria utvärderings versioner visas och inaktiverar andra erbjudanden som inte är kostnads fria. Test versioner visas på fliken **försök** i katalogen.
3. Välj den kostnads fria utvärderings version som du vill erbjuda och välj sedan **Skicka**. Alla utvärderingar är i 30 dagar under vilka du inte debiteras. Du kan också konvertera den till en betald prenumeration när som helst under utvärderings perioden.

## <a name="converting-trials-to-paid-subscriptions"></a>Konvertera utvärderingar till betalda prenumerationer

En kostnads fri utvärderings version konverteras inte automatiskt till en betald prenumeration. Efter 30 dagar måste en kostnads fri utvärderings version konverteras till en betald prenumeration eller [upphör att gälla](#expiring-offers). Det går inte att utöka kostnads fria utvärderings versioner.

Du måste konvertera utvärderings versionen till en betald prenumeration själv. Du kan göra detta [med hjälp av Partner Center](#convert-trials-using-partner-center) eller [via API: er för partner Center](#convert-trials-using-apis).

> [!NOTE]
> Kundens kostnads fria utvärderings version för Cloud Solution Provider (CSP)-programmet kan inte konverteras till en annan program klient (till exempel EA, Open eller MOSP).

### <a name="convert-trials-using-partner-center"></a>Konvertera försök med hjälp av Partner Center

Du kan konvertera utvärderingar till betalda prenumerationer med hjälp av Partner Center:

1. Gå till sidan för kundens prenumeration och välj den kostnads fria utvärderings versionen.
2. Välj **konvertera utvärderings version till betald prenumeration**.
3. Ange önskad licens antal och fakturerings frekvens och välj **Använd**.
4. Faktureringen för den betalda prenumerationen börjar på konverterings datumet och prenumerationen förnyas automatiskt 12 månader från konverterings datumet. 

### <a name="convert-trials-using-apis"></a>Konvertera försök med API: er

Du kan behöva ändra dina API: er för att passa konverteringen av en kostnads fri utvärderings version till en betald prenumeration. Mer information finns i följande dokumentation om utvecklare:

- [Konvertera en utvärderingsprenumeration till betald](/partner-center/develop/convert-a-trial-subscription-to-paid)
- [Hämta en lista över erbjudanden för utvärderingskonvertering](/partner-center/develop/get-a-list-of-trial-conversion-offers)

### <a name="trials-without-conversions"></a>Försök utan konverteringar

Alla utvärderings versioner kan inte konverteras till betalda prenumerationer. Partner kan använda en utvärderings version som inte har några konverteringar förrän förfallo datumet. Partner kan köpa kompatibla erbjudanden som stöder samma tjänster som utvärderings erbjudandet.  Detta bör göras innan utvärderings versionen upphör att gälla för de nyligen köpta erbjudandena-tjänsterna med utvärderings tjänsterna. 

|**Utvärdering**   |**Kompatibla små företags erbjudanden**   |**Kompatibla företags erbjudanden**   |
|----------------------------|:---------------------------------|:------------------------------------------|
|Utvärderings version av Microsoft Teams kommersiella moln (användaren har initierats)   |Microsoft 365 Business Basic, Microsoft 365 Business Standard, Microsoft 365 Business Premium   | F3 (tidigare F1), Office 365 för Enterprise (E1, E3 och E5), Microsoft 365 F1/F3, Microsoft 365 Enterprise (E3)   |

>[!NOTE]
>Erbjudandena ovan har liknande Service planer med liknande funktioner, men det kan finnas vissa skillnader mellan erbjudandena.

### <a name="expiring-offers"></a>Erbjudanden som upphör att gälla

Du kommer inte att meddelas om erbjudanden som upphör att gälla. Du kan spåra kommande förfallo datum med vyn kund i Partner Center eller genom att fråga API: et. Det är en bra idé att övervaka dessa datum ofta så att du kan vidta lämpliga uppföljnings åtgärder med kunder när de närmar sig ett besluts punkt.

När en utvärderings version har upphört att gälla kan en kund som försöker logga in på den här utvärderings versionen se ett förfallo meddelande. Data lagras dock i linje med data lagrings standarder. När du har köpt en ny prenumeration med samma service planer kan du komma åt kundens information igen från den nyligen aktiverade prenumerationen.

## <a name="billing"></a>Fakturering

Årliga fakturerings-och kostnads fria utvärderings versioner är desamma i suveräna moln och det offentliga molnet. Den enda skillnaden är utvärderings SKU: er som är tillgängliga vid tidpunkten för lanseringen.

## <a name="billing-for-free-trials"></a>Fakturering för kostnads fria utvärderings versioner

Kostnads fria utvärderings versioner kan användas för både månatliga och årligen fakturerade prenumerationer. Du kan välja fakturerings frekvensen när du konverterar utvärderings versionen till en betald prenumeration.

Prenumerationens start datum baseras på konverterings datumet. Om den kostnads fria utvärderings versionen konverteras till ett betalt erbjudande med årlig fakturering, blir prenumerationens förnyelse datum 12 månader från konverterings datumet. Om den kostnads fria utvärderings versionen konverteras till ett betalt erbjudande med månatlig fakturering, kommer prenumerationens förnyelse datum att vara tolv månader från fakturerings datumet efter konverterings datumet.

### <a name="invoices"></a>Fakturor

Inga kostnads fria utvärderings versioner visas i din faktura eller licensbaserade avstämnings fil. Kostnads fria utvärderings versioner visas bara på din faktura och licensbaserade avstämnings fil när du har konverterat en kostnads fri utvärderings version till en betald prenumeration. Den konverterade prenumerationen kommer att visas på samma sätt som en ny prenumeration.

### <a name="incentives"></a>Incitament

Kostnads fria utvärderings versioner har ingen påverkan på incitament.

## <a name="support"></a>Support

För support vid kostnads fria utvärderingar skickar du en tjänstbegäran via partner Center.