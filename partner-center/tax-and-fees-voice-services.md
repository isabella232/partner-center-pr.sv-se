---
title: Regionala tjänster och avgifter för PSTN-tjänster
description: Som en Office 365-partner som samverkar Microsoft 365 röst produkter kan du vara underkastad regionala skatter, avgifter eller myndighets krav för PSTN-tjänster.
ms.topic: article
ms.date: 09/10/2020
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 411932923e6bd35732e64521abe567f40f7499e9
ms.sourcegitcommit: 3c26a61982082787bbdaf5d1e92553b26f3a5076
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/06/2021
ms.locfileid: "106441497"
---
# <a name="regional-taxes-regulations-for-public-switched-telephone-network-ptsn-services"></a>Regionala skatter, bestämmelser för PTSN-tjänster (Public Switched Phone Network)

**Lämpliga roller**

- Global administratör
- Användaradministratör
- Administratörs agent

PSTN-tjänster (Public Switched Phone Network) i vissa jurisdiktioner kan omfattas av särskilda skatte-och reglerings krav som kan påverka partner order och fakturering. I USA, inklusive Puerto Rico, är PSTN-tjänster, som omfattar ljud konferens, samtals planer och kommunikations krediter, särskilda skatte-och reglerings krav. I USA och Puerto Rico är Microsofts priser PSTN-tjänster som skatt.  Unika PSTN-skatter och-föreskrifter påverkar Office 365-partner som agerar Microsoft 365 röst produkter.  Om en partner anger priset för en Microsoft PSTN-tjänst kan de vara ansvariga för att beräkna och remittera PSTN-skatter och-avgifter.

## <a name="partner-recommendations"></a>Partner rekommendationer

Engagera din skatte-och juridisk rådgivning för att förstå organisationens ansvar avseende PSTN-tjänsternas reglering, skatter och avgifter och andra potentiella skulder.

## <a name="invoice-presentation-and-partner-reconciliation-file"></a>Faktura presentation och partner avstämnings fil

CSP-fakturor och CSP-avstämnings filer i USA, Puerto Rico och Kanada, som inkluderar Skype för företag PSTN och Microsoft 365 röst tjänster, innehåller separata rad objekt för PSTN-och icke-PSTN-komponenterna.

Dessutom visas följande fotnot i CSP-fakturor:

* Priset som visas är en avgift för ljud konferenser och samtals plan tjänster.  Eventuella tillämpliga transaktions skatter debiteras exklusivt av den mängd som visas förutom försäljning som görs inom USA.  I USA är det pris som visas som avgift som omfattar en avgift för den anropande planen och ljud konferens tjänsterna och en avgift för de skatter och avgifter som vi måste debitera.  Ljud konferenser och samtals plan tjänster hanteras av de Microsoft-partners som har behörighet att tillhandahålla dem.  Mer information finns i [Microsoft-volymlicensiering](https://go.microsoft.com/fwlink/?LinkId=690247).

## <a name="reconciliation-file-example"></a>Exempel på avstämnings fil

Office 365 Enterprise E5 visar en avstämnings fil som två rad objekt med identiska namn och identiska ID: n, men varje rad objekt har ett unikt enhets pris (exempel: $28,40 och $2,00). Detta avgränsar komponenten Skype för företag, PSTN-konferens i Office 365-erbjudandet, så att du kan tillämpa skatter på rätt sätt.

**Exempel på partner avstämning #1 (Välj kolumner):**

|**Durable_offer_ID**|**Offer_Name**|**Subscription_Start_Date**|**Subscription_End_Date**|**Charge_Start_Date**|**Charge_End_Date**|**Charge_Type**|**Unit_Price**|
|:----:|:----:|:----:|:----:|:----:|:----:|:----:|:----:|
|a044b16a-1861-4308-8086-a3a3b506fac2   |Office 365 Enterprise E5   |8/10/2019 0:00   |8/11/2019 0:00   |8/11/2019 0:00|9/10/2019 0:00   |Cykel avgift   |28,40   |
|a044b16a-1861-4308-8086-a3a3b506fac2   |Office 365 Enterprise E5   |8/10/2019 0:00   |8/11/2019 0:00   |8/11/2019 0:00   |9/10/2019 0:00   |Cykel avgift   |2,00   |

**Exempel på partner avstämning #2**

Microsoft 365 Business röst som är tillgänglig i Kanada har ytterligare PSTN-beskattningsbara komponenter som konsol IDE ras på CSP-faktura (liknar Office 365 E5 visas två rad objekt, en för PSTN-komponenter och andra för icke-PSTN-komponenter).  I avstämnings filen för CSP för Microsoft 365 Business röst visas alla PSTN-beskattningsbara komponenter individuellt (enskilda PSTN-komponenter samlas inte in. CSV-eller API-verktyg).  Summan av order detaljer och fakturerade belopp för kunder som finns i avstämnings filen matchar CSP-fakturan.

## <a name="additional-resources"></a>Ytterligare resurser
Mer information finns på webbplatsen [för Microsoft 365 för partner](https://www.microsoft.com/microsoft-365/partners/) .

