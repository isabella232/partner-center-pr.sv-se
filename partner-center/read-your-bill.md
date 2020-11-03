---
title: Så här läser du rekognoseringar-filen för Bill &
ms.topic: article
ms.date: 06/05/2020
description: Läs om din faktura & avstämnings filer. Din faktura visar kostnader för partner Center i alla program, produkter och kunder för den månads perioden.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: edb2d25b49bd5c40dfd30e9f21d2d8537a5669c4
ms.sourcegitcommit: e1c8bea4aaf807aebe99c125cb1fb6dc8fdfa210
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 07/30/2020
ms.locfileid: "92531105"
---
# <a name="understand-your-bill-and-reconciliation-file---learn-how-to-find-them-in-partner-center"></a>Förstå din faktura-och avstämnings fil – lär dig hur du hittar dem i Partner Center

**Gäller för**

- Partnercenter
- Partner Center för Microsoft Cloud för amerikanska myndigheter

**Lämpliga roller**

- Global administratör
- Faktureringsadministratör
- Administratörs agent


Din **faktura** är en **Sammanfattning av alla dina partner Center-avgifter** (över hela programmet, alla produkter och alla kunder). 

## <a name="invoice-types"></a>Faktura typer

Microsoft utfärdar en faktura för alla licensbaserade avgifter (till exempel Office 365) och användnings avgifter (till exempel Azure) och en separat faktura för engångs kostnader (till exempel Azure RI, Marketplace eller Azure-abonnemang).

Exempel:  

**Scenario 1 [enskild valuta]** : partnern har köp för 145P-erbjudande och O365-licenser,  

- Partner får en faktura PDF-och 2-avstämnings fil som täcker avgifterna för både O365 och Azure (145p).  

**Scenario 2 [enskild valuta]** : partnern har köp för Azure RI-, Marketplace-och/eller Azure-plan tillsammans med 145p köp.

- Partner får en faktura-PDF och en avstämnings fil som täcker kostnaderna för Azure (145p). 

- Partner får en annan faktura PDF och en avstämnings fil som täcker deras kostnader för Azure RI, Marketplace, Azure-abonnemang. 

**Scenario 3 [Multi-Currency]** : partnern har inköp för Azure RI i DKK och Azure-abonnemang i EUR tillsammans med 145p inköp i EUR.

- Partner får en faktura-PDF och en avstämnings fil som täcker avgifterna för Azure RI i SEK. 

- Partner får en faktura-PDF och en avstämnings fil som täcker avgifterna för Azure-abonnemang i EUR. 

- Partner får en annan faktura PDF och en avstämnings fil som täcker sina avgifter för 145p-erbjudandet i EUR (eller partner fakturerings valuta). 

## <a name="find-your-bill"></a>Hitta din faktura 

Du kan hitta din faktura på sidan fakturering på instrument panelen i Partner Center. Du kan också hitta fakturerings historik, utgifts trender och avstämnings filer på den här sidan. 

1. Logga in på Partner Center- [instrumentpanelen](https://partner.microsoft.com/dashboard/home). 

2. Välj **fakturering** på menyn till vänster. 

3. På sidan fakturering väljer du den faktura som du vill ladda ned. 

Du kan hitta en länk till den senaste fakturan högst upp på sidan under kontosaldo per senaste faktura datum. 

Du kan hitta tidigare fakturor i avsnittet fakturerings historik. Välj lämpligt år och välj sedan listpilen bredvid lämplig fakturerings period. Välj länken bredvid fakturor (. pdf) för att hämta periodens faktura. 

## <a name="understanding-invoice-pdf"></a>Förstå faktura-PDF 

**Fakturor för användnings-och licensbaserade avgifter** : fakturor för avgifter för tjänster som Office 365 och Azure kommer att vara tillgängliga inom två (2) dagar från det valda fakturerings DATUMET [UTC].  

**Fakturor för databasmigrering och återkommande avgifter** : fakturor för avgifter för tjänster som Azure-RI, Azure-plan, Marketplace kommer att vara tillgängliga senast den 8: a varje månad.  

Nedan visas några av nyckel fälten i PDF-dokumentet för fakturor –

**Faktura nummer** : unik identifierare för det faktura dokument som genererats för respektive fakturerings period. 

**Fakturerings period** : det här är den period under vilken du har användnings-och licensbaserade tjänster. 

**Faktura datum** : fakturerings datumet eller jubileums datumet som fakturan genereras för varje månad. 

**Förfallo datum för betalning** : det datum då din betalning måste tas emot. 

**Avgifter** : det belopp som förfaller i din fakturerings valuta för respektive fakturerings period. 

**Krediter** : krediter (till exempel SLA) eller justeringar för ändringar av prenumerationer (till exempel licens ökningar eller minskningar). 

**Betalnings anvisningar** : en beskrivning av hur du betalar din faktura baserat på din region. Var alltid noga med att inkludera ditt faktura nummer när du gör en betalning. 

En detaljerad beskrivning av alla fält i din faktura fil (inklusive fält för engångs kostnader) finns i [fält för faktura fil](invoice-file.md). 

## <a name="understand-reconciliation-files"></a>Förstå avstämnings filer

 Avstämnings filer, som ger en detalj nivå ned/specificerad information om dina avgifter, är tillgängliga för hämtning tillsammans med fakturan PDF. I avstämnings filerna ingår kund identifierare och prenumerations-ID: n som du kan använda för att skapa kund fakturor. Se  [hur du använder avstämnings filerna](use-the-reconciliation-files.md) för att få mer information om rekognoseringar-filerna. 
