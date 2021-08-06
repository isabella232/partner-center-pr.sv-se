---
title: Så här läser du fakturan & rekognoseringsfilen
ms.topic: article
ms.date: 06/05/2020
description: Lär dig mer om dina & avstämningsfiler. Fakturan visar partnercenteravgifter för programmet, produkter och kunder för den månatliga perioden.
ms.service: partner-dashboard
ms.subservice: partnercenter-billing
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: bf75d847320e901638890bef8077a1656399d2ffc5aaaf984af329784d1de030
ms.sourcegitcommit: 121f1b9cbd88faeba60dc9b475f9c0647cdc933c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/06/2021
ms.locfileid: "115678245"
---
# <a name="understand-your-bill-and-reconciliation-file---learn-how-to-find-them-in-partner-center"></a>Förstå fakturan och avstämningsfilen – lär dig hur du hittar dem i Partnercenter


**Lämpliga roller:** Global | Faktureringsadministratörskonto | Administratörsagent


Fakturan **är** en **sammanfattning av alla dina partnercenteravgifter** (i programmet, alla produkter och alla kunder). 

## <a name="find-your-bill-and-reconciliation-file"></a>Hitta fakturan och avstämningsfilen 

Du hittar din faktura på sidan Fakturering på instrumentpanelen i Partnercenter. Du hittar även din faktureringshistorik, utgiftstrender och avstämningsfiler på den här sidan. 

1. Logga in på instrumentpanelen i [Partnercenter.](https://partner.microsoft.com/dashboard/home) 

2. I den vänstra menyn väljer du **Fakturering**. 

3. På sidan för faktureringsstatus väljer du en faktura eller avstämningsfil som du vill se mer detaljerad information för. 

Du hittar en länk till din senaste faktura längst upp på sidan under Kontosaldo från och med det senaste fakturadatumet. 

Du hittar tidigare fakturor i avsnittet Faktureringshistorik. Välj lämpligt år och välj sedan den nedrullningsna pilen bredvid lämplig faktureringsperiod. Välj länken bredvid Fakturor (.pdf) för att ladda ned periodens faktura. 

## <a name="invoice-types"></a>Fakturatyper

Microsoft utfärdar en faktura för alla licensbaserade avgifter (till exempel Office 365) och användningsbaserade avgifter (till exempel Azure) och en separat faktura för en gång-avgifter (till exempel Azure RI, Marketplace eller Azure-plan).

Exempel:  

**Scenario 1 [enkel valuta]**: Partnern har inköp för 145P-erbjudande Office 365 licenser,  

- Partnern får en PDF-faktura och två avstämningsfiler som täcker avgifterna för både Office 365 och Azure (145p).  

**Scenario 2 [enskild valuta]**: Partnern har inköp för Azure RI, Marketplace och/eller Azure-plan tillsammans med 145p-köp.

- Partnern får en PDF-faktura och en avstämningsfil som täcker avgifterna för Azure (145p). 

- Partnern får en annan FAKTURA-PDF och en avstämningsfil som täcker deras avgifter för reserverad Azure-instans (RI), Marketplace och Azure-plan. 

**Scenario 3 [Multi-Currency]**: Partnern har inköp för Azure RI i DK och Azure-planen i EUR tillsammans med 145p-köp i EUR.

- Partnern får en PDF-faktura och en avstämningsfil som täcker avgifterna för Azure RI i DK. 

- Partnern får en PDF-faktura och en avstämningsfil som täcker avgifterna för Azure-planen i EUR. 

- Partnern får en annan FAKTURA-PDF och en avstämningsfil som täcker deras avgifter för 145p-erbjudandet i EUR (eller partnerfaktureringsvaluta). 


## <a name="understanding-invoice-pdf"></a>Förstå PDF-faktura 

**Fakturor för användnings-** och licensbaserade avgifter: Fakturor för avgifter för tjänster som Office 365 och Azure är tillgängliga inom två (2) dagar från det valda faktureringsdatumet [UTC].  

**Fakturor för engångsavgifter och återkommande** avgifter: Fakturor för avgifter för tjänster som Azure RI, Azure-plan och Marketplace är tillgängliga senast den åttonde varje månad.  

Nedan visas några av nyckelfälten i PDF-fakturadokumentet –

**Fakturanummer:** Unik identifierare för fakturadokumentet som genererats för respektive faktureringsperiod. 

**Faktureringsperiod:** Det här är den period då du har användningar och licensbaserade tjänster. 

**Fakturadatum:** Faktureringsdatum eller årsdag då fakturan genereras varje månad. 

**Förfallodatum för betalning:** Det datum då betalningen måste tas emot. 

**Avgifter:** Det belopp som ska betalas i din faktureringsvaluta för respektive faktureringsperiod. 

**Krediter:** Krediter (till exempel serviceavtal (SLA) eller justeringar för ändringar som görs i prenumerationer (till exempel licensökningar eller minskningar). 

**Betalningsanvisningar:** Beskrivning av hur du betalar din faktura, baserat på din region. Se alltid till att inkludera ditt fakturanummer när du gör en betalning. 

En detaljerad beskrivning av alla fält i din fakturafil (inklusive fält för en gång-avgifter) finns i [Fälten för fakturafil](invoice-file.md). 

## <a name="understand-reconciliation-files"></a>Förstå avstämningsfiler

 Avstämningsfiler, som ger en detaljerad/detaljerad information om dina avgifter, är tillgängliga för nedladdning tillsammans med PDF-fakturan. Avstämningsfilerna innehåller kundidentifierare och prenumerationsidentifierare som du kan använda för att skapa kundfakturor. Mer information om avstämningsfiler finns i [Så här använder du avstämningsfilerna.](use-the-reconciliation-files.md) 

## <a name="next-steps"></a>Nästa steg

- [Så här använder du avstämningsfilerna](use-the-reconciliation-files.md)