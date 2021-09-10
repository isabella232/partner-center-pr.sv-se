---
title: Regionala PSTN-tjänstskatter och -avgifter
description: Som Office 365 partner som Microsoft 365 Voice-produkter kan du omfattas av regionala skatter, avgifter eller regelkrav för PSTN-tjänster.
ms.topic: article
ms.date: 09/10/2020
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 85eefb49cf62c4bcfa5533683abd8ddb0e854463
ms.sourcegitcommit: 1161d5bcb345e368348c535a7211f0d353c5a471
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/09/2021
ms.locfileid: "123961514"
---
# <a name="regional-taxes-regulations-for-public-switched-telephone-network-ptsn-services"></a>Regionala skatter, föreskrifter för PTSN-tjänster (Public Switched Telephone Network)

**Lämpliga roller:** Global | Användaradministratörsbehörighet | Administratörsagent

PSTN-tjänster (Public Switched Telephone Network) i vissa jurisdiktioner kan omfattas av särskilda skatte- och regelkrav som kan påverka partnerorder och fakturering. I USA, inklusive PuertoJekt, PSTN-tjänster, som omfattar ljudkonferenser, samtalsplaner och kommunikationskrediter, omfattas av särskilda skatte- och regelkrav. Microsoft USA PSTN-tjänster som skatteomfattande i de här artiklarna USA Och Puerto Därför prissätter Microsoft PSTN-tjänster som moms.  Unika PSTN-skatter och -regler påverkar Office 365 partner som Microsoft 365 Voice-produkter.  Om en partner markerar priset för en Microsoft PSTN-tjänst kan de ansvara för att beräkna och överföra PSTN-skatter och -avgifter.

## <a name="partner-recommendations"></a>Partner Rekommendationer

Engagera din skatterådgivare och juridiska rådgivare för att förstå organisationens ansvar för PSTN-tjänsternas regler, skatter och avgifter och andra potentiella skulder.

## <a name="invoice-presentation-and-partner-reconciliation-file"></a>Fakturapresentation och partneravstämningsfil

Molnlösningsleverantör fakturor (CSP) och CSP-avstämningsfiler i USA, PuertoKommando och Kanada, som innehåller Skype för företag PSTN- och Microsoft 365 Voice-tjänster, tillhandahåller separata radobjekt för PSTN- och icke-PSTN-komponenterna.

Dessutom visar CSP-fakturor följande fotnot:

* Priset som visas är en avgift för ljudkonferenser och samtalsplantjänster.  Alla tillämpliga transaktionsskatter debiteras exklusivt för det belopp som visas förutom för försäljning som görs inom USA.  I USA är priset som visas inklusive skatt, eftersom det inkluderar en avgift för samtalsplanen och ljudkonferenstjänsterna och en avgift för de skatter och avgifter som vi måste debitera.  Ljudkonferens och samtalsplantjänster serdas av Microsofts dotterbolag som har behörighet att tillhandahålla dem.  Mer information finns i [Microsoft-volymlicensiering](https://go.microsoft.com/fwlink/?LinkId=690247).

## <a name="reconciliation-file-example"></a>Exempel på avstämningsfil

Office 365 Enterprise E5 visar i avstämningsfilen som två radobjekt med identiska namn och identiska ID:n, men varje radobjekt har ett unikt enhetspris (exempel: 28,40 USD och 2,00 USD). Detta separerar Skype för företag PSTN-konferenskomponenten i Office 365,så att du kan tillämpa skatter på rätt sätt.

**Exempel på partneravstämning #1 (välj kolumner):**

|**Durable_offer_ID**|**Offer_Name**|**Subscription_Start_Date**|**Subscription_End_Date**|**Charge_Start_Date**|**Charge_End_Date**|**Charge_Type**|**Unit_Price**|
|:----:|:----:|:----:|:----:|:----:|:----:|:----:|:----:|
|a044b16a-1861-4308-8086-a3a3b506fac2   |Office 365 Enterprise E5   |8/10/2019 0:00   |8/11/2019 0:00   |8/11/2019 0:00|9/10/2019 0:00   |Cykelavgift   |28,40   |
|a044b16a-1861-4308-8086-a3a3b506fac2   |Office 365 Enterprise E5   |8/10/2019 0:00   |8/11/2019 0:00   |8/11/2019 0:00   |9/10/2019 0:00   |Cykelavgift   |2,00   |

**Exempel på partneravstämning #2**

Microsoft 365 Business Voice som är tillgängliga i Kanada har ytterligare PSTN-momsbara komponenter som konsolideras på CSP-fakturan (liknar Office 365 E5 visas två radobjekt, en för PSTN-komponenter och den andra för icke-PSTN-komponenter).  CSP-avstämningsfilen för Microsoft 365 Business Voice visar alla PSTN-momsbara komponenter individuellt (enskilda PSTN-komponenter konsolideras inte i .CSV eller API-verktyget).  Sammanfattningen av orderinformationen och fakturerade belopp för kunder som finns i avstämningsfilen matchar CSP-fakturan.

## <a name="additional-resources"></a>Ytterligare resurser
Mer information finns på Microsoft 365 [för partner.](https://www.microsoft.com/microsoft-365/partners/)

