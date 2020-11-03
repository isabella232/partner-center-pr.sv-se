---
title: Öka införandet och nöjdheten
ms.topic: how-to
ms.date: 07/21/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Lär dig hur du använder mått i Partner Center. Mått kan visa om din verksamhet växer, hur kunderna använder sina licenser och var de kan fokusera investeringen.
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: d995d72f6b5f9fb3beafff91eee7518ee999bf6c
ms.sourcegitcommit: 8dc139749916c822c5c438f54a03d2f147697dd5
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/04/2020
ms.locfileid: "92531189"
---
# <a name="use-metrics-in-partner-center-to-increase-adoption-and-satisfaction"></a>Använd mått i Partner Center för att öka implementeringen och nöjdheten

**Gäller för**

- Partnercenter
- Cloud Solution Provider-program

**Lämpliga roller**

- Global administratör
- Användaradministratör
- Administratörs agent
- Försäljnings agent

Våra partner använder många mått för att mäta om deras verksamhet växer och var investeringen ska riktas mot. Partner Center kan hjälpa till med att tillhandahålla data om och hur dina kunder använder de licenser som de har köpt. Den här informationen är tillgänglig för Office-produkter (inklusive OneDrive för företag, som räknas tillsammans med SharePoint).

Du kan se data för alla dina kunder via Cloud Solution Provider-programmet. Vissa kunder kan köpa licenser från andra partner eller direkt från Microsoft. I dessa situationer ser du de totala licenserna för alla partner. Om du bara vill se dina egna licenser går du till kundens prenumerationer i stället.

> [!NOTE]  
> För närvarande visar vi bara data för Office 365 och Dynamics 365. Vi kommer att aktivera data för ytterligare produkter i framtiden.

## <a name="find-license-and-user-data"></a>Hitta licens-och användar data

Du kan hitta licens-och användar data för en enskild kund eller över hela din portfölj.

### <a name="find-license-and-user-data-for-a-single-customer"></a>Hitta licens-och användar data för en enskild kund

1. Logga in på [instrument panelen](https://partner.microsoft.com/dashboard)för partner Center.

2. Välj **kunder** från **partner Center**

3. Välj en kund.

4. Välj **Customer Insights** .

### <a name="find-license-and-user-data-across-your-portfolio"></a>Hitta licens-och användar data i din portfölj

1. Logga in på [instrument panelen](https://partner.microsoft.com/dashboard)för partner Center.

2. Välj **analysera** och välj från något av analys alternativen på menyn.

3. Om du vill hämta distributions-och användnings data över hela kund uppsättningen väljer du alternativet **Exportera** (nedåtpil).

Terminologi:

- **Berättigande** = en licens som användaren har rätt att använda (den är inte inaktive rad för bedrägerier eller utebliven betalning, den har inte uppgraderats till en annan licens, den har inte avbrutits av användaren osv.)

- **Active** = om den prenumererade användaren har använt rättigheten för en aktivitet under de senaste 28 kalender dagarna.

- **Distribution%** = tilldelade licenser/sålda licenser

- **Användning%** = aktiva rättigheter/totala rättigheter

   Ibland är användningen% inplattad eller större än 100%. Detta kan bero på flera orsaker:

  - Om kunden hade omsättningen för den anställda och licensen överfördes till en ny användare.

  - Om kunden har två prenumerationer för en SKU, men en är i respitperiod, inaktive rad eller insamlad, kan rättigheter i båda prenumerationerna registrera aktiv användning under 28-dagars perioden, men endast en räknas i totalen.

  - Om kunden har en utvärderings prenumeration räknas aktiviteten men prenumerationen räknas inte in i det totala antalet rättigheter.

  - Om vissa kunder använder Yammer betydligt mer än vad de har rätt till av sin licens kan de skeva data dramatiskt.

## <a name="next-steps"></a>Nästa steg

Om du har ett fält med många hjälp-och instruktions frågor, är antagande numren på ditt konto lågt, eller så du är ute efter att sälja affärs möjligheter, kanske du vill överväga att erbjuda utbildning. Genom att lära kunderna hur man bättre använder moln lösnings program som de har köpt, är det mer troligt att du ser en ökning av produktiviteten och nöjdheten och en minskning av support behoven.

### <a name="considering-how-to-improve-customer-adoption-and-usage---a-couple-scenarios"></a>Fundera över hur du kan förbättra kundens antagande och användning – ett par scenarier

**Problem** : användar priset för införande är lågt och många licenser används inte.

**Vad du bör tänka** på: kunderna kanske inte förstår det värde som program varan kan tillhandahålla. De behöver hjälp med att skapa de sätt som de kan använda för att under lätta de uppgifter som de redan utför, eller för att aktivera nya typer av produktivitet.

**Vad du kan prova** : fallstudier, användar åsikter om vissa scenarier, själv studie Bloggar eller videor.

**Problem** : det finns en stor mängd support samtal för hjälp och instruktions frågor.

**Vad du bör tänka** på: kunder kan vara nya för program varan, produkt versionen eller uppgiften.

**Vad du kan prova** : du kan använda en dubbel strategi för att erbjuda utbildning (personligen eller online) för att öka kundernas övergripande expertis och samtidigt marknadsföra några av de självbetjänings alternativ som är tillgängliga för kunderna.

Du kanske vill designa om support webbplatsen för att även inkludera de självbetjänings alternativ som beskrivs i [Customer Self support](customer-self-support.md) förutom support kontakt information.

