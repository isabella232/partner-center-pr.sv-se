---
title: Licensbaserade avstämningsfiler
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Lär dig mer om att läsa licensbaserade avstämnings filer i Partner Center. I den här artikeln beskrivs innebörden av varje fält i din licensbaserade rekognoseringar-fil.
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: bc97156d23fa4ea1082a0ad4a931ff36375897a7
ms.sourcegitcommit: 6498c57e75aa097861523b206dc142f789deeb36
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/02/2021
ms.locfileid: "106178926"
---
# <a name="understand-the-fields-in-partner-center-license-based-reconciliation-files"></a>Förstå fälten i licensbaserade, licensierade filer för partner Center

**Gäller för**

- Partner Center för Microsoft myndighets moln

**Lämpliga roller**

- Global administratör
- Administratör för användar hantering
- Faktureringsadministratör
- Administratörs agent

Om du vill stämma av dina ändringar mot en kunds order jämför du **Syndication_Partner_Subscription_Number** från avstämnings filen mot **prenumerations-ID: t** från Partner Center.

## <a name="fields-in-license-based-reconciliation-files"></a>Fält i licensbaserade avstämnings filer

| Kolumn | Beskrivning | Exempelvärde |
| ------ | ----------- | ------------ |
| Partner | Unikt ID i GUID-format för en angiven fakturerings enhet. Krävs inte för avstämning. Samma i alla rader. | *8ddd03642-test-test-test-test-46b58d356b4e* |
| CustomerId | Unikt Microsoft-ID för kunden i GUID-format. | *12ABCD34-001A-BCD2-987C-3210ABCD5678* |
| CustomerName | Kundens organisations namn, enligt rapporter i Partner Center. *Mycket viktigt fält för att stämma av fakturan med system information.* | *Testa kund A* |
| MpnId | MPN identifierare för CSP-partnern. Se [hur du specificerar en partner](use-the-reconciliation-files.md#itemize-reconciliation-files-by-partner). | *4390934* |
| ResellerMpnId | MPN identifierare för åter försäljaren av posten för prenumerationen.  |
| OrderId | Unik identifierare för en beställning i Microsofts fakturerings plattform. Kan vara användbart för att identifiera ordningen när du kontaktar supporten. Används inte för avstämning. | *566890604832738111* |
| SubscriptionId | Unikt ID för en prenumeration i Microsofts fakturerings plattform. Kan vara användbart för att identifiera prenumerationen när du kontaktar supporten. Används inte för avstämning. *Värdet är inte samma som **prenumerations-ID: t** i partner administratörs konsolen. Se **SyndicationPartnerSubscriptionNumber** i stället.* | *usCBMgAAAAAAAAIA* |
| SyndicationPartnerSubscriptionNumber | Unik identifierare för prenumerationer. En kund kan ha flera prenumerationer för samma plan. Den här kolumnen är viktig för analys av fil avstämning. Det här fältet mappar till **prenumerations-ID: t** i partner administratörs konsolen. | *fb977ab5-test-test-test-test-24c8d9591708* |
| OfferId | Unikt erbjudande-ID. Standard identifierare för erbjudande, enligt definitionen i pris listan. *Det här värdet matchar inte **erbjudande-ID** från pris listan. Se **DurableOfferID** i stället.* | *FE616D64-E9A8-40EF-843F-152E9BBEF3D1* |
| DurableOfferId | Unikt ID för beständiga erbjudanden, enligt definitionen i pris listan. *Det här värdet matchar **erbjudande-ID: t** från pris listan.* | *1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C* |
| OfferName | Namnet på det tjänst erbjudande som kunden har köpt, enligt definitionen i pris listan. | *Microsoft Office 365 (plan E3)* |
| SubscriptionStartDate | Prenumerationens start datum. Tiden är alltid början på dagen, 0:00. Det här fältet är inställt på dagen efter det att ordern skickades. Används tillsammans med **SubscriptionEndDate** för att fastställa: om kunden fortfarande är under det första året i prenumerationen eller om prenumerationen har förnyats under följande år. | *2/1/2019 0:00* |
| SubscriptionEndDate | Prenumerationens slutdatum. Tiden är alltid början på dagen, 0:00. *12 månader plus **x** dagar efter start datumet* för att justeras till partnerns fakturerings datum eller *12 månader från förnyelse datumet*. Vid förnyelsen uppdateras priserna till den aktuella pris listan. Kundens kommunikation kan krävas i förväg för automatisk förnyelse. | *2/1/2019 0:00* |
| ChargeStartDate | Start dag för avgifterna. Tiden är alltid början på dagen, 0:00. Används för att beräkna dagliga avgifter *(* proportionella avgifter) när en kund ändrar licens nummer. | *2/1/2019 0:00* |
| ChargeEndDate | Slutdatum för avgifterna. Tiden är alltid slutet på dagen, 23:59. Används för att beräkna dagliga avgifter *(* proportionella avgifter) när en kund ändrar licens nummer. | *2/28/2019 23:59* |
| ChargeType | [Typ av kostnad](recon-file-charge-types.md) eller justering. | Se [debiterings typer](recon-file-charge-types.md). |
| UnitPrice | Pris per licens, som publicerat i pris listan vid inköps tillfället. Se till att detta matchar informationen som lagras i fakturerings systemet under avstämning. | *6,82* |
| Kvantitet | Antal licenser. Se till att detta matchar informationen som lagras i fakturerings systemet under avstämning. | *2* |
| Amount | Total pris för kvantitet. Används för att kontrol lera om mängd beräkningen matchar hur du beräknar det här värdet för dina kunder. | *13,32* |
| TotalOtherDiscount | Rabatt belopp som tillämpas på dessa kostnader. Produkt licenser som ingår i en kompetens eller kartor, eller nya prenumerationer som är berättigade till ett incitament, kommer också att innehålla ett rabatt belopp i den här kolumnen. | *2,32* |
| Delsumma | Totalt före skatt. Kontrollerar om din delsumma motsvarar den förväntade summan, i händelse av en rabatt. | *11* |
| Skatt | Avgift för moms belopp. Baserat på marknadens skatte regler och särskilda omständigheter. | *0* |
| TotalForCustomer | Totalt efter skatt. Kontrollerar om du debiteras skatt på fakturan. | *11* |
| Valuta | Typ av valuta. Varje fakturerings enhet har bara en valuta. Kontrol lera om den matchar din första faktura. Kontrol lera igen efter eventuella större fakturerings plattforms uppdateringar. | *EUR* |
| DomainName | Kundens domän namn. Det här fältet kan vara tomt fram till den andra fakturerings perioden. *Använd inte det här fältet som en unik identifierare för kunden. Kunden/partnern kan uppdatera anpassad eller standard domänen via Office 365-portalen.* | *example.onmicrosoft.com* |
| SubscriptionName | Prenumerationens smek namn. Om inget smek namn anges använder Partner Center **OfferName**. | *PROJECT ONLINE* |
| SubscriptionDescription | Namnet på det tjänst erbjudande som kunden har köpt, enligt definitionen i pris listan. (Det här är ett identiskt fält för **OfferName**.) | *PROJECT ONLINE PREMIUM UTAN PROJECT-KLIENT* |
| BillingCycleType | Fakturerings frekvens vid en tidpunkt.| *Varje månad* |