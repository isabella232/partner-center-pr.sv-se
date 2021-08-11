---
title: Licensbaserade avstämningsfiler
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-billing
description: Lär dig hur du läser licensbaserade avstämningsfiler i Partnercenter. Den här artikeln förklarar innebörden av varje fält i din licensbaserade rekognoseringsfil.
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 7bb6900ba34c99d497d8273e56e6385aa3bf55690c8729526a5e4c6a1e60ba28
ms.sourcegitcommit: 121f1b9cbd88faeba60dc9b475f9c0647cdc933c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/06/2021
ms.locfileid: "115694140"
---
# <a name="understand-the-fields-in-partner-center-license-based-reconciliation-files"></a>Förstå fälten i partnercenters licensbaserade avstämningsfiler

**Gäller för**: Partner Center-| Partnercenter för Microsoft Cloud for US Government

**Lämpliga roller:** Global | Administratörsbehörighet för användarhantering | Faktureringsadministratörskonto | Administratörsagent

Om du vill stämma av ändringarna mot en kunds beställningar jämför **du Syndication_Partner_Subscription_Number** från avstämningsfilen mot **prenumerations-ID:t** från Partnercenter.

## <a name="fields-in-license-based-reconciliation-files"></a>Fält i licensbaserade avstämningsfiler

| Kolumn | Beskrivning | Exempelvärde |
| ------ | ----------- | ------------ |
| PartnerId | Unik identifierare i GUID-format för en specifik faktureringsentitet. Krävs inte för avstämning. Samma i alla rader. | *8ddd03642-test-test-test-46b58d356b4e* |
| CustomerId | Unik Microsoft-identifierare för kunden i GUID-format. | *12ABCD34-001A-BCD2-987C-3210ABCD5678* |
| CustomerName | Kundens organisationsnamn, enligt vad som rapporteras i Partnercenter. *Mycket viktigt fält för att stämma av fakturan med systeminformationen.* | *Testa kund A* |
| MpnId | MPN-identifierare för CSP-partnern. Se [hur du specificerar efter partner](use-the-reconciliation-files.md#itemize-reconciliation-files-by-partner). | *4390934* |
| ResellerMpnId | MPN-identifierare för återförsäljaren av posten för prenumerationen.  |
| OrderId | Unik identifierare för en beställning på Microsofts faktureringsplattform. Kan vara användbart för att identifiera ordern när du kontaktar supporten. Används inte för avstämning. | *566890604832738111* |
| SubscriptionId | Unik identifierare för en prenumeration på Microsofts faktureringsplattform. Kan vara användbart för att identifiera prenumerationen när du kontaktar supporten. Används inte för avstämning. *Det här värdet är inte samma som **prenumerations-ID:t** i partneradministratörskonsolen. Se **SyndicationPartnerSubscriptionNumber i** stället.* | *usCBMgAAAAAAAIA* |
| SyndicationPartnerSubscriptionNumber | Unik identifierare för prenumerationer. En kund kan ha flera prenumerationer för samma plan. Den här kolumnen är viktig för avstämningsfilanalys. Det här fältet mappar till **prenumerations-ID:t** i partneradministratörskonsolen. | *fb977ab5-test-test-test-24c8d9591708* |
| OfferId | Unikt erbjudande-ID. Standarderbjudandeidentifierare enligt definitionen i prislistan. *Det här värdet matchar inte **erbjudande-ID** från prislistan. Se **DurableOfferID i** stället.* | *FE616D64-E9A8-40EF-843F-152E9BBEF3D1* |
| DurableOfferId | Unik identifierare för beständigt erbjudande enligt definitionen i prislistan. *Det här värdet matchar **erbjudande-ID** från prislistan.* | *1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C* |
| OfferName | Namnet på det tjänsterbjudande som köpts av kunden enligt definitionen i prislistan. | *Microsoft Office 365 (alternativ E3)* |
| SubscriptionStartDate | Prenumerationens startdatum i UTC. Tiden är alltid början på dagen, 0:00. Det här fältet anges till dagen efter att ordern skickades. Används med **SubscriptionEndDate** för att avgöra om kunden fortfarande är inom det första året i prenumerationen, eller om prenumerationen har förnyats för följande år. | *2/1/2019 0:00* |
| SubscriptionEndDate | Prenumerationens slutdatum i UTC. Tiden är alltid början på dagen, 0:00. Antingen *12 månader **plus x*** dagar efter startdatumet för att justera med partnerns faktureringsdatum eller *12 månader från förnyelsedatumet.* Vid förnyelse uppdateras priserna till den aktuella prislistan. Kundkommunikation kan krävas i förväg för automatisk förnyelse. | *2/1/2019 0:00* |
| ChargeStartDate | Startdag för avgifterna. Tiden är alltid början på dagen, 0:00. Används för att beräkna dagliga avgifter *(pro-avgifter)* när en kund ändrar licensnummer. | *2/1/2019 0:00* |
| ChargeEndDate | Slutdag för avgifterna. Tiden är alltid dagens slut, 23:59. Används för att beräkna dagliga avgifter *(pro-avgifter)* när en kund ändrar licensnummer. | *2/28/2019 23:59* |
| ChargeType | Typ [av avgift eller](recon-file-charge-types.md) justering. | Se [avgiftstyper.](recon-file-charge-types.md) |
| UnitPrice | Pris per licens, enligt vad som publicerades i prislistan vid tidpunkten för köpet. Se till att detta matchar informationen som lagras i faktureringssystemet under avstämningen. | *6.82* |
| Kvantitet | Antal licenser. Se till att detta matchar informationen som lagras i faktureringssystemet under avstämningen. | *2* |
| Amount | Totalt pris för kvantitet. Används för att kontrollera om beloppsberäkningen matchar hur du beräknar det här värdet för dina kunder. | *13.32* |
| TotalOtherDiscount | Rabattbelopp som tillämpas på dessa avgifter. Produktlicenser som ingår i en kompetens eller MAPS, eller nya prenumerationer som är berättigade till ett incitament, innehåller också ett rabattbelopp i den här kolumnen. | *2.32* |
| Delsumma | Totalsumma före skatt. Kontrollerar om din delsumma matchar din förväntade summa, om det finns en rabatt. | *11* |
| Skatt | Avgiftsbelopp för skatt. Baserat på din marknads skatteregler och specifika omständigheter. | *0* |
| TotalForCustomer | Totalsumma efter skatt. Kontrollerar om du debiteras skatt på fakturan. | *11* |
| Valuta | Valutatyp. Varje faktureringsentitet har bara en valuta. Kontrollera om den matchar din första faktura. Kontrollera igen efter eventuella större uppdateringar av faktureringsplattformen. | *EUR* |
| DomainName | Kundens domännamn. Det här fältet kan visas som tomt fram till den andra faktureringsperioden. *Använd inte det här fältet som en unik identifierare för kunden. Kunden/partnern kan uppdatera standarddomänen via Office 365 portalen.* | *example.onmicrosoft.com* |
| SubscriptionName | Smeknamn för prenumeration. Om inget smeknamn har angetts använder Partner Center **OfferName**. | *PROJECT ONLINE* |
| SubscriptionDescription | Namnet på det tjänsterbjudande som köpts av kunden enligt definitionen i prislistan. (Det här är ett identiskt fält **med OfferName**.) | *PROJECT ONLINE PREMIUM UTAN PROJEKTKLIENT* |
| BillingCycleType | Faktureringsfrekvens en gång.| *Varje månad* |
