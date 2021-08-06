---
title: Användningsbaserade avstämningsfiler
ms.topic: article
ms.date: 06/08/2020
description: Lär dig mer om alla objekt i din användningsbaserade avstämningsfil i Partnercenter. Innehåller några exempel.
author: sodeb
ms.service: partner-dashboard
ms.subservice: partnercenter-billing
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: f14b387649e6df8ded2e037858a7216eb361e848c8de6c8a71373d06ebe81d16
ms.sourcegitcommit: 121f1b9cbd88faeba60dc9b475f9c0647cdc933c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/06/2021
ms.locfileid: "115681220"
---
# <a name="understand-usage-based-reconciliation-files-and-their-specific-fields-in-partner-center"></a>Förstå användningsbaserade avstämningsfiler och deras specifika fält i Partnercenter

**Lämpliga roller:** Kontoadministratörsroller | Faktureringsadministratör

Om du vill stämma av dina avgifter mot en kunds användning jämför du **ResellerID**,  **ResellerName** och **ResellerBillableAccount** från avstämningsfilen med kundnamnet och prenumerations-ID:t från Partnercenter. 

## <a name="fields-in-usage-based-reconciliation-files"></a>Fält i användningsbaserade avstämningsfiler

I följande fält förklaras vilka tjänster som användes och priset.

| Kolumn | Beskrivning | Exempelvärden |
| ------ | ----------- | ------------ |
| PartnerId | Partneridentifierare i GUID-format. | *DA41BC5F-C52D-4464-8A8D-8C8DCC43503B* |
| PartnerName | Partnerns namn. | *Contoso, Ltd.* |
| PartnerBillableAccountId | Partnerkontoidentifierare. | *1010578050* |
| CustomerCompanyName | Kundens organisationsnamn, enligt vad som rapporteras i Partnercenter. *Detta är mycket viktigt för att stämma av fakturan med systeminformationen.* | *Testa kund* |
| MpnId | Microsoft Partner Network (MPN) för CSP-partnern (Molnlösningsleverantör). | *4390934* |
| ResellerMpnId | MPN-identifierare för återförsäljaren av posten för prenumerationen.  |
| InvoiceNumber | Fakturanummer där den angivna transaktionen visas. | *D020001IVK* |
| ChargeStartDate | Startdatum för faktureringsperioden, förutom när du presenterar datum för tidigare ej debiterade latent användningsdata (från föregående faktureringsperiod). Tiden är alltid början på dagen, 0:00. | *2/1/2019 0:00* |
| ChargeEndDate | Slutdatum för faktureringsperioden, förutom när du presenterar datum för tidigare ej debiterade latent användningsdata (från föregående faktureringsperiod). Tiden är alltid dagens slut, 23:59. | *2/28/2019 23:59* |
| SubscriptionId | Unik identifierare för en prenumeration på Microsofts faktureringsplattform. Kan vara användbart för att identifiera prenumerationen när du kontaktar supporten. Används inte för avstämning. *Detta är inte samma som **prenumerations-ID:t** i partneradministratörskonsolen.* | *usCBMgAAAAAAAIA* |
| SubscriptionName | Smeknamn för tjänsterbjudandet. | *Microsoft Azure* |
| SubscriptionDescription | Verksamhetsraden för tjänsteerbjudandet. | *Microsoft Azure* |
| OrderID | Unik identifierare för en beställning på Microsofts faktureringsplattform. Kan vara användbart för att identifiera prenumerationen när du kontaktar supporten. Används inte för avstämning. | *566890604832738111* |
| ServiceName | Namnet på den azure-tjänst som är i fråga. | *VIRTUELLA DATORER* |
| ServiceType | Den specifika typen av Azure-tjänst. | *Service Bus – individuell databas eller paketdatabas* *SQL Azure – Business eller Web Edition* |
| ResourceGuid | Specifik unik identifierare för alla tjänstdata och prisstrukturen. | *DA41BC5F-C52D-4464-8A8D-8C8DCC43503B* |
| ResourceName | Namnet på Azure-resursen. | *Dataöverföring i (GB)*, *dataöverföring ut (GB)* |
| Region | Den region som användningen gäller för. Används främst för att tilldela priser till dataöverföringar, eftersom priserna varierar beroende på region. | *Asien och stillahavsområdet*, *Europa,* *Latinamerika*, *Nordamerika* |
| Sku | Unik Microsoft-identifierare för ett erbjudande. | *7UD-00001* |
| DetailLineItemId | En identifierare och kvantitet för att specificera olika priser för en tjänst eller resurs under en viss faktureringsperiod. För nivåindelade Azure-priser kan det finnas ett pris för upp till en viss kvantitet fakturerbara enheter och sedan ett annat pris efter den kvantiteten. | *1* |
| ConsumedQuantity | Mängden tjänst som förbrukas (till exempel timmar eller GB) under rapporteringsperioden. Omfattar även eventuell ej fakturerad användning från tidigare rapporteringsperioder. | *11* |
| IncludedQuantity | Enheter som ingår i erbjudandet. Finns vanligtvis inte i CSP. | *0* |
| OverageQuantity | Enheter som inte ingår i erbjudandet. Dessa måste betalas av partnern. Lika med **ConsumedQuantity** minus **IncludedQuantity**. | *11* |
| ListPrice | Erbjudandets pris gäller vid prenumerationens startdatum. | *0,0808 USD* |
| PretaxCharges | Lika med **ListPrist multiplicerat** med **OverageQuantity**, avrundat till närmaste cent. | *0,085 USD* |
| TaxAmount | Debiterat skattebelopp. Baserat på din marknads skatteregler och specifika omständigheter. | *0,08 USD* |
| PostTaxTotal | Totalsumma efter skatt, när skatt är tillämplig. | *0,93 USD* |
| Valuta | Valutatyp. Varje faktureringsenhet har bara en valuta. Kontrollera att den matchar din första faktura och sedan efter eventuella större uppdateringar av faktureringsplattformen. | *EUR* |
| PretaxEffectiveRate | Pris före skatt per enhet. Lika med **PretaxCharges dividerat** med **OverageQuantity**, avrundat till närmaste cent. | *0,08 USD* |
| PostTaxEffectiveRate | Efter skatt per enhet. Lika med **PostTaxTotal dividerat** **med OverageQuantity**, avrundat till närmaste cent. Eller lika med **PretaxEffectiveRate** plus skattesatsen per enhetsbelopp, avrundat till närmaste cent. | *0,08 USD* |
| ChargeType | Typ [av avgift eller](recon-file-charge-types.md) justering. | Se [avgiftstyper](recon-file-charge-types.md). |
| CustomerId | Unik Microsoft-identifierare för kunden i GUID-format. | *ORDDC52E52FDEF405786F0642DD0108BE4* |
| DomainName | Kundens domännamn. Det här fältet kan visas tomt fram till den andra faktureringsperioden. | *example.onmicrosoft.com* |
| BillingCycleType | Tidsfaktureringsfrekvens.| **Varje månad**  |
| Enhet | Resursnamnets **enhet.** | *GB* eller *TIMMAR* |
| CustomerBillableAccount | Unikt konto-ID på Microsofts faktureringsplattform. | *1280018095* |
| UsageDate | Datum för tjänstdistribution. | *2/1/2019 0:00* |
| MeteredRegion | Identifierar platsen för ett datacenter i regionen (för tjänster där det här värdet är tillämpligt och ifylld). | *Asien, östra*, *Asien, sydöstra, Europa,* *norra,* *Europa, västra,* *USA, norra centrala,* *USA, södra centrala* |
| MeteredService | Identifierar den enskilda Azure-tjänstanvändningen när den inte har identifierats specifikt i **kolumnen ServiceName.** Dataöverföringar rapporteras till exempel som Microsoft Azure *– Alla tjänster* i kolumnen **ServiceName.** | *AccessControl*, *CDN*, *Compute*, *Database*, *ServiceBus*, *Storage* |
| MeteredServiceType | Bra att **veta mer om MeteredService-fältet** som förtydligar användningen av Azure-tjänster. | *Externa* |
| Project | Kunddefinierat namn för tjänstinstansen. | *ORDDC52E52FDEF405786F0642DD0108BE4* |
| ServiceInfo | Antalet Azure-Service Bus anslutningar som etablerades och används en viss dag. | *1.000000 anslutningar/30* dagar (om du hade en individuellt etablerad anslutning under en 30-dagars månad), *25 anslutningar/30 dagar – används: 1.000000* (om du hade ett 25 paket med Service Bus-anslutningar etablerade och du använde 1 under den dagen) |

## <a name="next-steps"></a>Nästa steg

- [Förstå fälten i licensbaserade avstämningsfiler i Partnercenter](license-based-recon-files.md)