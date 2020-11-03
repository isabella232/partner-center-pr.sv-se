---
title: Användning-baserade avstämnings filer
ms.topic: article
ms.date: 06/08/2020
description: Lär dig mer om alla objekt i din användnings-baserade avstämnings fil i Partner Center. Innehåller några exempel.
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 04ad6a0c2c7a6330d2e1230f046ee78b2a7405c8
ms.sourcegitcommit: 36a60f672c1c3d6b63fd225d04c5ffa917694ae0
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 07/03/2020
ms.locfileid: "92529198"
---
# <a name="understand-usage-based-reconciliation-files-and-their-specific-fields-in-partner-center"></a>Förstå användnings avstämnings filer och deras respektive fält i Partner Center

Gäller för:

- Partnercenter
- Partner Center för Microsoft Cloud för amerikanska myndigheter

För att stämma av dina avgifter mot kundens användning, jämför **ResellerID** , **ResellerName** och **ResellerBillableAccount** från avstämnings filen med **kund namnet** och **prenumerations-ID: t** från Partner Center.

## <a name="fields-in-usage-based-reconciliation-files"></a>Fält i användnings avstämnings filer

I följande fält förklaras vilka tjänster som användes och priset.

| Kolumn | Beskrivning | Exempel värde (n) |
| ------ | ----------- | ------------ |
| Partner | Partner-ID i GUID-format. | *DA41BC5F-C52D-4464-8A8D-8C8DCC43503B* |
| PartnerName | Partnerns namn. | *Contoso, Ltd.* |
| PartnerBillableAccountId | Partner konto identifierare. | *1010578050* |
| CustomerCompanyName | Kundens organisations namn, enligt rapporter i Partner Center. *Mycket viktigt för att stämma av fakturan med din system information.* | *Testa kund* |
| MpnId | MPN identifierare för CSP-partnern. | *4390934* |
| ResellerMpnId | MPN identifierare för åter försäljaren av posten för prenumerationen.  |
| InvoiceNumber | Faktura nummer där den angivna transaktionen visas. | *D020001IVK* |
| ChargeStartDate | Start datum för fakturerings perioden, förutom vid presentation av datum för tidigare avlastade latens användnings data (från föregående fakturerings cykel). Tiden är alltid början på dagen, 0:00. | *2/1/2019 0:00* |
| ChargeEndDate | Slutdatum för fakturerings perioden, förutom vid presentation av datum för tidigare avlastade latens användnings data (från föregående fakturerings cykel). Tiden är alltid slutet på dagen, 23:59. | *2/28/2019 23:59* |
| SubscriptionId | Unikt ID för en prenumeration i Microsofts fakturerings plattform. Kan vara användbart för att identifiera prenumerationen när du kontaktar supporten. Används inte för avstämning. *Detta är inte samma som **prenumerations-ID: t** i partner administratörs konsolen.* | *usCBMgAAAAAAAAIA* |
| SubscriptionName | Smek namn för tjänst erbjudandet. | *Microsoft Azure* |
| SubscriptionDescription | Tjänste utbudets verksamhets nivå. | *Microsoft Azure* |
| OrderID | Unik identifierare för en beställning i Microsofts fakturerings plattform. Kan vara användbart för att identifiera prenumerationen när du kontaktar supporten. Används inte för avstämning. | *566890604832738111* |
| ServiceName | Namnet på den aktuella Azure-tjänsten. | *VIRTUELLA DATORER* |
| ServiceType | Den speciella typen av Azure-tjänst. | *Service Bus – individ eller Pack* , *SQL Azure Database – Business eller Web Edition* |
| ResourceGuid | Specifika unika identifierare för alla tjänst data och pris strukturen. | *DA41BC5F-C52D-4464-8A8D-8C8DCC43503B* |
| ResourceName | Namnet på Azure-resursen. | *Dataöverföring i (GB)* *utgående dataöverföring (GB)* |
| Region | Den region som användningen gäller. Används främst för att tilldela priser till data överföringar, eftersom priserna varierar mellan olika regioner. | *Asien och Stillahavsområdet* , *Europa* , *Latinamerika* , *Nordamerika* |
| Sku | Unikt Microsoft-ID för ett erbjudande. | *7UD – 00001* |
| DetailLineItemId | En identifierare och kvantitet för att specificera olika taxa för en tjänst eller resurs under en viss fakturerings period. För priser på Azure-nivå, kan det finnas en avgift för upp till en viss kvantitet fakturerbara enheter, sedan en annan kostnad efter den kvantiteten. | *1* |
| ConsumedQuantity | Mängden förbrukad tjänst (till exempel timmar eller GB) under rapporterings perioden. Inkluderar även eventuell ej fakturerad användning från föregående rapporterings perioder. | *11* |
| IncludedQuantity | Enheter som ingår som en del av erbjudandet. Förekommer vanligt vis inte i CSP. | *0* |
| OverageQuantity | Enheter som inte ingår som en del av erbjudandet. Dessa måste betalas av partnern. Lika med **ConsumedQuantity** minus **IncludedQuantity** . | *11* |
| ListPrice | Erbjudande priset som påverkas av prenumerationens start datum. | *$0,0808* |
| PretaxCharges | Lika med **ListPrist** multiplicerat med **OverageQuantity** , avrundat till närmaste cent. | *$0,085* |
| TaxAmount | Debiteras skatte belopp. Baserat på marknadens skatte regler och särskilda omständigheter. | *$0,08* |
| PostTaxTotal | Totalt efter skatt, när skatt är tillämpligt. | *$0,93* |
| Valuta | Typ av valuta. Varje fakturerings enhet har bara en valuta. Kontrol lera att den matchar din första faktura och sedan efter eventuella större fakturerings plattforms uppdateringar. | *EUR* |
| PretaxEffectiveRate | Pretax pris per enhet. Lika med **PretaxCharges** dividerat med **OverageQuantity** , avrundat till närmaste cent. | *$0,08* |
| PostTaxEffectiveRate | Bokför skatt pris per enhet. Lika med **PostTaxTotal** dividerat med **OverageQuantity** , avrundat till närmaste cent. Eller, lika med **PretaxEffectiveRate** plus skatte satsen per enhets belopp, avrundat till närmaste procent. | *$0,08* |
| ChargeType | [Typ av kostnad](recon-file-charge-types.md) eller justering. | Se [debiterings typer](recon-file-charge-types.md). |
| CustomerId | Unikt Microsoft-ID för kunden i GUID-format. | *ORDDC52E52FDEF405786F0642DD0108BE4* |
| DomainName | Kundens domän namn. Det här fältet kan vara tomt fram till den andra fakturerings perioden. | *example.onmicrosoft.com* |
| BillingCycleType | Tids fakturerings frekvens.| **Varje månad**  |
| Enhet | Enhet för resurs **namnet** . | *GB* eller *timmar* |
| CustomerBillableAccount | Unikt konto-ID på Microsofts fakturerings plattform. | *1280018095* |
| UsageDate | Datum för tjänst distribution. | *2/1/2019 0:00* |
| MeteredRegion | Identifierar platsen för ett Data Center i regionen (för tjänster där det här värdet är tillämpligt och ifyllt). | *Asien, östra* , *Asien, sydöstra* , *Nord Europa* , *Västeuropa,* *norra centrala USA* , *södra centrala USA* |
| MeteredService | Identifierar den enskilda användningen av Azure-tjänsten när den inte identifieras särskilt i kolumnen **ServiceName** . Data överföringar rapporteras till exempel som *Microsoft Azure – alla tjänster* i kolumnen **ServiceName** . | *AccessControl* , *CDN* , *Compute* , *databas* , *Service Bus* , *Storage* |
| MeteredServiceType | Under rubrik för **MeteredService** -fältet som ger ytterligare klargörande av användning av Azure-tjänster. | *5,25* |
| Project | Kunddefinierat namn för tjänst instansen. | *ORDDC52E52FDEF405786F0642DD0108BE4* |
| ServiceInfo | Antalet Azure Service Bus anslutningar som etablerades och utnyttjas på en bestämd dag. | *1,000000 anslutningar/30 dagar* (om du hade en individuellt etablerad anslutning under en 30-dagars månad), *25 anslutningar/30 dagar – använt: 1,000000* (om du har ett 25-paket med Service Bus anslutningar etablerade och du använder 1 under den dagen) |
