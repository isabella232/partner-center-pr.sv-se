---
title: Hantera Azure-reservationer för kunder
description: Lär dig hur du hanterar Azure-reservationer för en kund, inklusive hur du avbryter en reservation, utbyter en reservation eller ber om en åter betalning.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: amitravat
ms.author: amrava
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 08/06/2020
ms.openlocfilehash: 937a7268caa5ae7872f8a3ec6dcb05f56dd9fbe5
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/22/2020
ms.locfileid: "92531632"
---
# <a name="manage-cancel-exchange-or-refund-microsoft-azure-reservations-for-customers"></a>Hantera, avbryta, byta ut eller återbetala Microsoft Azure reservationer för kunder

**Gäller för**

- Partnercenter
- Microsoft Azure-portalen 
- Partner i CSP

**Lämpliga roller**

- Administratörs agent
- Global administratör
- Support agent
- Försäljnings agent
- Administratör för användar hantering

> [!NOTE]
> Den här artikeln gäller endast partner i Cloud Solution Provider (CSP)-programmet. Kunder som använder andra typer av prenumerationer (t. ex. betala per användning, enskilda, Microsoft-kundavtal eller Enterprise-avtal prenumerationer) bör i stället läsa [denna dokumentation om Azure-reservationer](/azure/cost-management-billing/reservations).

Om du vill hantera dina kunders Azure-reservationer efter köp väljer du den kund och reservation som du vill hantera i Partner Center och gör sedan ändringar i reservationen i Azure Portal.

1. Kom igång genom att välja **kunder** från menyn Partner Center och sedan välja den kund vars reservationer du vill hantera. 

2. På kundens informations sida-meny väljer du **Azure-reservationer** och väljer sedan den specifika reservation som du vill hantera.  

3. Under **åtgärder** väljer du **Hantera** för att gå till kundens reservations post i Azure Portal. På sidan reservations information följer du stegen nedan för att slutföra aktiviteterna.  

    | **Välj**   | **Om du vill**    |
    |:-----------------------------|:-----------------|
    | **Översikt**   | Visa information om en kunds reservation, inklusive förfallo datum, omfattning och användnings data. **Obs!** Välj **åter betalning** för att skapa en supportbegäran för en proportionell åter betalning. Välj **Exchange** om du vill skapa en supportbegäran för att utbyta den oanvända delen av din reservations term.  
    | **Access Control (IAM)**   | Hantera åtkomst till kundens reservations information.|
    | **Konfiguration**   | Ändra reservationens omfång och/eller den Azure-prenumeration som reservationen är kopplad till.    |
    | **Egenskaper**   | Visa reservationens egenskaper och kopiera till Urklipp reservations-ID och ID för reservations order. **Obs!** Support kan be dig om reservations-ID och ID för reservations ordning när du begär support för en kunds räkning.    |
    | **Ny supportbegäran**    | Be om hjälp från Microsoft Support.   |
 
## <a name="cancel-or-exchange-a-reservation"></a>Avbryta eller byta ut en reservation

Om en kunds affärs behov förändras, kan det vara bra att avbryta en reservation och få en åter betalning eller byta ut en reservations proportionellt belopp som ska användas mot priset för en ny reservation.

I båda dessa scenarier har Microsoft pengarna pengarna till dig så att du sedan kan hantera de resulterande ekonomiska transaktionerna med dina kunder. Microsoft kontaktar inte kunder direkt om fakturering, uppsägningar eller åter betalningar.

### <a name="how-cancellations-work"></a>Så här fungerar annulleringar

Kunderna kan när som helst beställa en reservation (bidrags belopp på $50 000 per år). Om du avbryter en reservation kan kunden returnera de återstående månaderna av en Azure-reservation för en tidig uppsägnings avgift. Det återstående proportionella saldot minus den tidigaste uppsägnings avgiften återbetalas till ditt konto så att du kan återbetala kundens konto. 

Se nedan för att avbryta information och avgifter.


|**Datum för annullering**<br> antalet   |**Användning**    |**Kredit**  |**Tidig uppsägning**<br> betalning    |**Bidrags Kap** | 
|:----------------------------------|:------------|:-----------|:--------------------------------|:--------------|
|5 eller färre                         | No          | 100 %       | No                              | $50 000 USD   |
|5 eller färre                         | Yes         | Proportionellt beräknad  | No                              | $50 000 USD   |
|Mer än 5                        | No          | Proportionellt beräknad  | 12 %                             | $50 000 USD   |
|Mer än 5                        | Yes         | Proportionellt beräknad  | 12 %                             | $50 000 USD   |

### <a name="how-exchanges-work"></a>Hur utbyte fungerar 

Om en kund vill köpa en annan reservation än den som ursprungligen köptes från dig kan de begära ett utbyte. Att utväxla en reservation kan vara ett attraktivt alternativ för att avbryta en reservation eftersom kunden kan använda det proportionellt beräknade bidrags beloppet mot priset för den nya reservationen. 

Den proportionella åter betalnings summan krediteras ditt konto så att du kan erbjuda kunden ett utbyte.

## <a name="request-a-refund-or-exchange-on-behalf-of-a-customer"></a>Begär åter betalning eller Exchange för en kunds räkning

Om du vill skicka en support förfrågan om åter betalning eller Exchange åt dina kunder väljer du kunden och reservationen i Partner Center och skapar sedan support förfrågan i Azure Portal. 

>[!NOTE]
>Microsoft Support agenter kan be dig att ange reservations-ID och ID för reservations ordning. Du hittar den här informationen på sidan med reservationens **Egenskaper** i Azure Portal.

1. Kom igång genom att välja **kunder** från menyn Partner Center och sedan välja den kund som vill ha en åter betalning. 

2. På kundens informations sida väljer du **Azure-reservationer** och väljer sedan den specifika reservation som kunden vill betala om.  

3. Under **åtgärder** väljer du **åter betalning** för att gå till kundens reservations post i Azure Portal och initiera en support förfrågan.  

4. På sidan **ny supportbegäran** följer du stegen nedan för att begära en åter betalning. Välj **Nästa** efter varje steg. 

   |**Steg**                    |**Markerat**    |
   |:---------------------------|:-----------------|
   |**1 grunder**                |Typ av problem: fakturering.  |
   |**2 problem**               |Problem typ: reservations hantering. Kategori: utbyten och åter betalningar. |
   |**3 kontakt uppgifter**   |Välj dina inställningar och ange den information som krävs. 

5. Välj **skapa** när du är färdig.

## <a name="azure-reservations-resources"></a>Resurser för Azure-reservationer

|**För information om**   |**Läs detta**    |
|:-----------------------------|:-----------------|
|Översikt över Azure-reservationer i CSP  | [Sälj Microsoft Azure reserverade instanser](azure-reservations.md) |
|Köpa Azure-reservationer för dina kunder i Partner Center   | [Köp Azure-reservationer](azure-reservations-buying.md) |
|Fastställ rätt storlek på virtuell dator och kontrol lera användningen av kund-VM   | [Storlek på virtuell dator för maximal användning av Azure-reservationer](azure-usage.md)   |
|Köpa Azure-reservationer med partner Center API | [Köp Azure Reserved VM instances](/partner-center/develop/purchase-azure-reservations) i dokumentationen för partner Center-utvecklare   |
|Ge kunderna tillstånd att köpa sina egna Azure-reservationer från en prenumeration som du har köpt för dem. | [Ge kunderna tillstånd att köpa sina egna Azure-reservationer](give-customers-permission.md)   |