---
title: Översikt över fakturering i Partnercenter
ms.topic: article
ms.date: 01/28/2021
description: Lär dig grundläggande fakturerings- och fakturainformation för CSP-partner i Partnercenter. Innehåller information om hur du fakturerar kunder och hur du hittar och läser din faktura.
ms.service: partner-dashboard
ms.subservice: partnercenter-billing
author: sodeb
ms.author: sodeb
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: f594b7d39234080e2c3f99c05a2e64fdaa18f0dd
ms.sourcegitcommit: 1161d5bcb345e368348c535a7211f0d353c5a471
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/09/2021
ms.locfileid: "123960053"
---
# <a name="billing-overview-for-csp-program-partners-working-in-partner-center"></a>Faktureringsöversikt för CSP-programpartner som arbetar i Partnercenter 

**Lämpliga roller:** Administratörsagent | Faktureringsadministratörskonto | Global | Supportagent | Försäljningsagent

Den här artikeln innehåller grundläggande fakturerings- och fakturainformation för CSP-partner i Partnercenter, inklusive hur du fakturerar kunder och hur du hittar och läser din faktura.


## <a name="find-your-bill"></a>Hitta din faktura

Så här hittar du din faktura:

1. Logga in i Partnercenter och gå till [instrumentpanelen](https://partner.microsoft.com/dashboard/home).

2. I menyn i Partnercenter väljer du **Fakturering.**

3. På sidan **Fakturering** kan du ladda ned din senaste faktura eller ladda ned tidigare fakturor i **avsnittet Faktureringshistorik.**

## <a name="bill-your-customers"></a>Fakturera dina kunder

Microsoft har inga krav eller villkor för hur du hanterar din egen fakturering.

Information om hur du fastställer en kunds användning finns i dina [avstämningsfiler.](#find-your-bill) Använd kundens namn och andra relevanta fält för att fastställa användningen.

### <a name="billing-types"></a>Faktureringstyper

Faktureringstyper i Partnercenter **omfattar licensbaserad fakturering,** **användningsbaserad** fakturering och **en-gång-fakturering.** 

### <a name="billing-currency"></a>Faktureringsvaluta

**Licensbaserad och användningsbaserad** fakturering: Du debiteras för produkter i valutan för det land eller den region där du befinner dig. Du debiteras på samma sätt oavsett var kunden som du sålde produkten till finns.

**En-gång-fakturering:** Från och med augusti 2021 debiteras alla partner i partnerns valuta oavsett var kunden som du sålde produkterna finns. Läs mer om [engångs- och återkommande](azure-plan-billing.md). 

## <a name="invoices"></a>Fakturor

Din faktura är en sammanfattning av alla avgifter för den aktuella faktureringsperioden. Detta inkluderar avgifter för programmet, alla produkter och alla kunder. Exempel på månatliga och årliga faktureringsscenarier finns i [vanliga faktureringsscenarier](common-billing-scenarios.md)

För användnings- och licensbaserade faktureringar är din faktura tillgänglig inom två (2) dagar från det valda faktureringsdatumet i UTC-tid. Om du till exempel har faktureringsdatum 12 september börjar fakturagenereringen kl. 12:00 UTC den 13 september och slutförs 12:00 UTC den 14:e. 

Vid engångsfakturering och återkommande fakturering justeras faktureringsperioden till kalendermånad, och faktura-/avstämningsfilerna kommer att vara tillgängliga senast den 8:e varje månad. Mer information finns i [Fakturering för Azure-plan.](azure-plan-billing.md) 

## <a name="price-lists"></a>Prislistor

Prislistor uppdateras varje månad. Förhandsgranskningsprislistor är tillgängliga en (1) månad i förväg.

Om du vill se Molnlösningsleverantör senaste program och erbjudanden går du till Sell > Pricing and Offers (Sälja > och erbjudanden) på **instrumentpanelen i Partnerportal.** Du hittar separata prislistor för de olika typer av produkter som är tillgängliga. Följande prislistor finns på sidan **Priser och** erbjudanden:

**Licensbaserade** priser garanteras för prenumerationens period, vanligtvis 12 månader från inköpsdatum. 

**Användningsbaserade priser** kan ändras månadsvis.

**Priserna för produkter, tjänster och programvaruprenumerationer** garanteras genom prenumerationens varaktighet. Priserna kan dock ändras när du förnyar.

Du ser justeringar **och krediter** **i efterskott** på nästa faktureringsfaktura när krediten eller justeringen har tillämpats.

## <a name="payment-terms"></a>Betalningsvillkor

Betalningsvillkoren är netto 60 dagar. Fakturor måste betalas enligt fakturans förfallodatum (60 dagar efter faktureringsdatumet), annars kommer ditt konto att vara inaktuellt, vilket kan påverka registreringen i CSP. 

Du kan återfå alla funktioner för dina inaktiverade konton när du betalar det förfallna beloppet.

När den korrigerade faktureringsinformationen har angetts visas betalningen på faktureringssidan för Partnercenter inom 5 arbetsdagar.

### <a name="taxes-and-vat"></a>Skatter och moms

Du debiteras baserat på din information (inte dina kunders information) eftersom faktureringsrelationen är mellan Microsoft och dig. Du kan skicka din skatteidentifierare under kontokonfigurationen eller via en supportbegäran senare. Ändringarna visas i nästa faktureringsperiod.

För **källskatt och momsbefrielse måste** du skicka in skattedokumentation via en supportbegäran. Du ser ändringarna och lämpliga återbetalningar för nästa faktureringsperiod. Läs mer om att [skicka källskatt.](withholding-tax-credit-form.md) 

För **momsbefrielse måste du skicka** ditt momsregistreringsnummer (verifierat av Microsoft) via en tjänstbegäran.  Om momsregistrerings-ID:t skickas efter kontokonfigurationen (via en supportbegäran) kommer dina fakturor före denna begäran inte att ha ett momsregistreringsnummer stämplat på PDF-fakturan. Du ser ändringarna i nästa faktureringsperiod.

Du hittar ytterligare skatteinformation från ditt lokala skattekontor eller skatterådgivare.

### <a name="adjustmentscreditscancellations"></a>Justeringar/krediter/annulleringar

Annulleringskrediter för licensierade tjänster klassificeras i enlighet med den här formeln för oanvända dagar vid uppsägningar mitt i cykeln (samt licensminskningar enligt följande formel:

[ROUND(ROUND(Unit Price * Quantity/Number of days in pro-rated Month, 2) * Number of pro-rated days) /Quantity, 2) * Quantity] 

Microsoft debiterar inte avgifter för tidig uppsägning för annullering av licensbaserade tjänster.

### <a name="billing-rules"></a>Faktureringsregler

Det finns två typer av faktureringsfrekvenser idag: årlig & varje månad.  
Mätarpriser för tjänster kan ändras inom fakturacykeln.

#### <a name="annual-billing-rules"></a>Årliga faktureringsregler 

- Prenumerationer förnyas år och förnyas automatiskt.  

- Faktureringen sker i 12 månadsbetalningar eller en årlig betalning per årsprenumeration. 

- Du debiteras i förväg för nästa faktureringsperiod för licensbaserade tjänster, baserat på antalet licenser i slutet av den föregående faktureringsperioden. 

- Du debiteras/krediteras i efterskott för eventuella ändringar i antalet licenser (pro-area-beräkning baserat på licensdagar). Pro beräkning använder följande formel: 

  - [ROUND(ROUND(Unit Price * Quantity/Number of days in pro-rated Month, 2) * Number of pro-rated days) /Quantity, 2) * Quantity] 

- Betalningar debiteras för sålda licenser, inte etablerade licenser 

#### <a name="monthly-billing-rules"></a>Månatliga faktureringsregler 

- Prenumerationer är månad för månad och förnyas automatiskt enligt de nya priserna för tjänster som mäts. Du debiteras varje månad för föregående månads användning. 

- Mätarpriser för tjänster kan ändras inom fakturacykeln. 

- Fakturan du får har bara de avgifter som ackumuleras för den månaden. 


### <a name="credit-notes"></a>Kreditanteckningar

Du kan behöva begära en kredit eller fakturera på nytt av följande skäl:

- Du måste göra adress- eller inköpsorderkorrigeringar.
- En skatteåterbetalning tillämpades efter att fakturan genererades. Du kan begära en kredit eller en omfakturering för att få tillbaka skatteåterbetalningen till den ursprungliga fakturan. Samma sak gäller för återbetalningar. Du kan begära en kredit eller fakturera om den ursprungliga fakturan och sedan hämta en återbetalning.

**För alla engångstransaktioner och återkommande transaktioner kan** Microsoft utfärda en kreditfaktura när du begär en kredit eller fakturerar på nytt. Fakturan avbryts när krediten utfärdas. 

## <a name="next-steps"></a>Nästa steg

- [Förstå fakturan och avstämningsfilen](read-your-bill.md)
- [Vanliga faktureringsscenarier för CSP-programpartner](common-billing-scenarios.md)
- [Ändra faktureringsfrekvens](common-billing-scenarios.md)
- [Kundorderhistorik](csp-offers.md) 
- [Priser och erbjudanden](pricing-and-offers.md)
