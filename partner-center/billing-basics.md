---
title: Översikt över fakturering i Partner Center
ms.topic: article
ms.date: 01/28/2021
description: Lär dig mer om fakturerings-och faktura information för CSP-partner i Partner Center. Innehåller information om hur du fakturerar kunder och hur du hittar och läser din faktura.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 051d638024200fe58ca5e07f42b758b304b58219
ms.sourcegitcommit: 58432bbb7eb0aed123547da65642ca728cb9b32c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/07/2021
ms.locfileid: "106964383"
---
# <a name="billing-overview-for-csp-program-partners-working-in-partner-center"></a>Faktureringsöversikt för CSP-programpartner som arbetar i Partnercenter 

**Lämpliga roller**

- Administratörs agent
- Faktureringsadministratör
- Global administratör
- Support agent
- Försäljnings agent

Den här artikeln innehåller information om fakturering och faktura för CSP-partner i Partner Center, inklusive hur du fakturerar kunder och hur du hittar och läser din faktura.


## <a name="find-your-bill"></a>Hitta din faktura

Så här hittar du din faktura:

1. Logga in i Partnercenter och gå till [instrumentpanelen](https://partner.microsoft.com/dashboard/home).

2. Från menyn Partner Center väljer du **fakturering**.

3. På sidan **fakturering** kan du ladda ned din senaste faktura eller hämta tidigare fakturor i avsnittet **fakturerings historik** .

## <a name="bill-your-customers"></a>Debitera dina kunder

Microsoft har inga krav eller villkor för hur du hanterar din egen fakturering.

Se dina [avstämnings filer](#find-your-bill)för att fastställa en kunds användning. Använd kundens namn och andra relevanta fält för att fastställa användningen.

### <a name="billing-types"></a>Fakturerings typer

Fakturerings typer i Partner Center inkluderar **licensbaserade fakturerings-**, **användnings** fakturerings-och **engångs fakturering**. 

### <a name="billing-currency"></a>Fakturerings valuta

**Licens-och användnings fakturering**: du debiteras för produkt (er) i valutan för det land eller den region där du befinner dig. Du faktureras samma oavsett var kunden finns till vilken du sålde produkten/erna.

**Engångs fakturering**: från januari 28, 2021, partners i regionen EU/Efta och Storbritannien som har nya kunder och befintliga CSP-kunder som köper nya Commerce-erbjudanden för första gången vars innehavare skapades före 11 maj 2020, faktureras för dessa inköp i partner platsens valuta.  Partner som finns utanför EU/EFTA-och Storbritannien-regionen fortsätter att faktureras i partner platsens valuta. Läs mer om [Databasmigrering och återkommande](azure-plan-billing.md). 

## <a name="invoices"></a>Fakturor

Din faktura är en sammanfattning av alla avgifter för den aktuella fakturerings perioden. Detta omfattar kostnader i hela programmet, alla produkter och alla kunder. Exempel på månatliga och årliga fakturerings scenarier finns i [vanliga fakturerings scenarier](common-billing-scenarios.md)

För användnings- och licensbaserade faktureringar är din faktura tillgänglig inom två (2) dagar från det valda faktureringsdatumet i UTC-tid. Om du till exempel har ett 12 september-fakturerings datum påbörjas processen för att skapa fakturor vid 12:10:00 UTC på 13 och slutförs med 12:10:00 UTC på 14. 

Vid engångsfakturering och återkommande fakturering justeras faktureringsperioden till kalendermånad, och faktura-/avstämningsfilerna kommer att vara tillgängliga senast den 8:e varje månad. Mer information finns i [fakturering av Azure-plan](azure-plan-billing.md). 

## <a name="price-lists"></a>Pris listor

Pris listor uppdateras varje månad. För hands versionen av pris listor är tillgängliga en (1) månad i förväg.

Om du vill se de senaste programmen och erbjudandena från partner portalen går du till **försäljning > priser och erbjudanden**. Du hittar separata pris listor för de olika typerna av produkter som är tillgängliga. Följande pris listor finns på sidan **priser och erbjudanden** :

**Licensbaserade** priser garanteras för prenumerationens mandat period, vanligt vis 12 månader från inköps datumet. 

**Användnings priser** kan ändras varje månad.

**Priserna för produkter, tjänster och program varu prenumerationer** garanteras genom prenumerationens varaktighet. Priserna kan dock ändras när du förnyar.

Du ser justeringar och **krediter** i **efterhand** på nästa fakturerings faktura när krediten eller justeringen har tillämpats.

## <a name="payment-terms"></a>Betalningsvillkor

Betalnings villkoren är netto 60 dagar. Fakturor måste betalas efter fakturans förfallo datum (60 dagar efter fakturerings datumet), eller så kommer ditt konto att bli eftersatta, vilket kan påverka registreringen i CSP. 

Du kan få full funktionalitet för dina inaktiverade konton när du betalar den senaste förfallo mängden.

När den korrigerade fakturerings informationen har angetts visas din betalning på sidan för partner Center-fakturering inom 5 arbets dagar.

### <a name="taxes-and-vat"></a>Skatter och moms

Du beskattas utifrån dina uppgifter (inte dina kunders information) eftersom fakturerings förhållandet är mellan Microsoft och dig. Du kan skicka in ditt moms-ID under konto konfigurationen eller genom att köra en support förfrågan senare. Ändringarna visas på nästa fakturerings period.

För **käll-och moms befrielse** måste du lägga till skatte dokumentation via en support förfrågan. Du ser ändringarna och lämplig åter betalning på nästa fakturerings period. Få mer information om hur du [skickar käll skatt](withholding-tax-credit-form.md). 

För **mervärde skatte befrielse** måste du skicka in ditt moms-ID (validerat av Microsoft) via en tjänstbegäran.  Om moms-ID: t skickas efter konto konfigurationen (via en supportbegäran) får dina fakturor före denna begäran inte ett moms-ID som stämplas på faktura-PDF. Du ser ändringarna vid nästa fakturerings period.

Du hittar ytterligare skatte information från ditt lokala skatte kontor eller skatte rådgivare.

### <a name="adjustmentscreditscancellations"></a>Justeringar/krediter/uppsägningar

Annullerings krediter för licensierade tjänster är proportionellt för oanvända dagar för uppsägningar i medel hög grad (samt licens minskning enligt följande formel:

[Avrunda ((avrunda (enhets pris * antal/antal dagar i graderad månad, 2) * antal månads beräknade dagar)/kvantitet, 2) * antal] 

Microsoft debiterar inte avgifter för tidig uppsägning för annullering av licensbaserade tjänster.

### <a name="billing-rules"></a>Fakturerings regler

Det finns två typer av fakturerings frekvenser idag: årlig & varje månad.  
Avgiftsbelagda tjänste priser kan ändras inom faktura cykeln.

#### <a name="annual-billing-rules"></a>Årliga fakturerings regler 

- Prenumerationer är årliga och förnyas automatiskt.  

- Faktureringen sker i 12 månads betalningar eller en årlig betalning per årlig prenumeration. 

- Du faktureras i förväg för nästa fakturerings period för licensbaserade tjänster, baserat på antalet licenser i slutet av föregående fakturerings period. 

- Du faktureras/krediteras i efterhand för eventuella förändringar i antalet licenser (proportionell beräkning baseras på licens dagar). I en proportionell beräkning används följande formel: 

  - [Avrunda ((avrunda (enhets pris * antal/antal dagar i graderad månad, 2) * antal månads beräknade dagar)/kvantitet, 2) * antal] 

- Betalningar faktureras för sålda licenser, inte licenser etablerade 

#### <a name="monthly-billing-rules"></a>Månads fakturerings regler 

- Prenumerationer är månads-till-månad och förnyas automatiskt vid nya avgiftsbelagda tjänst avgifter. Du faktureras varje månad för föregående månads användning. 

- Avgiftsbelagda tjänste priser kan ändras inom faktura cykeln. 

- Fakturan du tar emot har bara de avgifter som debiteras för den månaden. 


### <a name="credit-notes"></a>Kredit kommentarer

Du kan behöva begära en kredit eller omstrukturering av följande orsaker:

- Du måste göra korrigeringar av adressen eller inköps ordern.
- En skatte åter betalning tillämpades när fakturan genererades. Du kan begära en kredit eller fakturera för att få moms åter betalningen tillbaka till den ursprungliga fakturan. Samma sak gäller även för åter betalningar. Du kan begära en kredit eller en omräkning av den ursprungliga fakturan och sedan hämta en åter betalning.

**För alla engångs-och återkommande transaktioner** kan Microsoft utfärda en kredit faktura när du begär en kredit eller fakturera. Fakturan annulleras när krediten utfärdas. 

## <a name="next-steps"></a>Nästa steg

- [Förstå din faktura-och avstämnings fil](read-your-bill.md)
- [Vanliga fakturerings scenarier för CSP-programpartner](common-billing-scenarios.md)
- [Ändra faktureringsfrekvens](common-billing-scenarios.md)
- [Kund order historik](csp-offers.md) 
- [Priser och erbjudanden](pricing-and-offers.md)