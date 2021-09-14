---
title: Hantera Azure-reservationer för kunder
description: Lär dig hur du hanterar Azure-reservationer för en kund, inklusive hur du avbryter en reservation, byter ut en reservation eller begär en återbetalning.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-customers
author: amitravat
ms.author: amrava
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 08/06/2020
ms.openlocfilehash: 627c6f8d09a904e7d988c4229ec10eeac38dc2e9
ms.sourcegitcommit: 37eac16c4339cb97831eb2a86d156c45bdf6a531
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/13/2021
ms.locfileid: "126246361"
---
# <a name="manage-cancel-exchange-or-refund-microsoft-azure-reservations-for-customers"></a>Hantera, avbryta, byta eller återbetala Microsoft Azure reservationer för kunder

**Lämpliga roller:** Administratörsagent | Global | Supportagent | Försäljningsagent | Administratör för användarhantering

Den här artikeln beskriver hur du hanterar Azure-reservationer för en kund, inklusive hur du avbryter en reservation, byter ut en reservation eller begär en återbetalning.

> [!NOTE]
> Den här artikeln gäller endast för partner i programmet Molnlösningsleverantör (CSP). Kunder som använder andra typer av prenumerationer (till exempel betala enligt användning, enskilda prenumerationer, Microsoft-kundavtal eller företagsavtal-prenumerationer) bör i stället läsa dokumentationen om [Azure-reservationer.](/azure/cost-management-billing/reservations)

Om du vill hantera dina kunders Azure-reservationer efter köpet väljer du den kund och reservation som du vill hantera i Partnercenter och gör sedan ändringar i reservationen i Azure Portal.

1. Kom igång genom att **välja Kunder** på menyn i Partnercenter och sedan välja den kund vars reservationer du vill hantera. 

2. På kundens informationssida väljer du **Azure-reservationer** och sedan den specifika reservation som du vill hantera.  

3. Under **Åtgärder** väljer du **Hantera** för att gå till kundens reservationspost i Azure Portal. På sidan med reservationsinformation följer du stegen nedan för att slutföra uppgifter.  

    | **Välj**   | **Till**    |
    |:-----------------------------|:-----------------|
    | **Översikt**   | Visa information om en kunds reservation, inklusive förfallodatum, omfång och användningsdata. **OBS!** Välj **Återbetalning** för att skapa en supportbegäran för en prode beräknad återbetalning. Välj **Exchange skapa** en supportbegäran för att byta ut den oanvända delen av reservationen.  
    | **Access Control (IAM)**   | Hantera åtkomst till kundens reservationsinformation.|
    | **Konfiguration**   | Ändra reservationens omfång och/eller den Azure-prenumeration som reservationen är associerad med.    |
    | **Egenskaper**   | Visa reservationens egenskaper och kopiera reservations-ID och reservationsbeställnings-ID till Urklipp. **OBS!** Supporten kan be dig om reservations-ID och reservationsbeställnings-ID när du begär support för en kunds räkning.    |
    | **Ny supportbegäran**    | Be om hjälp från Microsoft Support.   |
 
## <a name="cancel-or-exchange-a-reservation"></a>Avbryta eller byta en reservation

Om en kunds affärsbehov ändras kan de vilja avbryta en reservation och få en återbetalning eller byta ut en reservations propåförda återbetalningsbelopp som ska användas mot priset för en ny reservation.

I båda dessa scenarier återbetalar Microsoft beloppet till dig så att du sedan kan hantera de resulterande ekonomiska transaktionerna med dina kunder. Microsoft kontaktar inte kunderna direkt om fakturering, annulleringar eller återbetalningar.

### <a name="how-cancellations-work"></a>Så här fungerar annulleringar

Kunder kan begära att avbryta en reservation när som helst (återbetalningsbeloppet är begränsat till 50 000 USD per år). Om du avbryter en reservation kan kunden returnera beloppet för de återstående månaderna i en Azure-reservation mot en avgift för tidig uppsägning. Det återstående prorrerade saldot, minus avgiften för tidig uppsägning, återbetalas till ditt konto så att du kan återbetala kundens konto. 

Se nedan för information om annullering och avgifter.


|**Annulleringsdatum**<br> (dagar)   |**Användning**    |**Kredit**  |**Tidig avslutning**<br> Avgift    |**Tak för återbetalning** | 
|:----------------------------------|:------------|:-----------|:--------------------------------|:--------------|
|5 eller färre                         | No          | 100 %       | No                              | 50 000 USD   |
|5 eller färre                         | Yes         | Pro betygsatt  | No                              | 50 000 USD   |
|Mer än 5                        | No          | Pro betygsatt  | 12 %                             | 50 000 USD   |
|Mer än 5                        | Yes         | Pro betygsatt  | 12 %                             | 50 000 USD   |

### <a name="how-exchanges-work"></a>Så här fungerar utbyten 

Om en kund vill köpa en annan reservation än den som kunden ursprungligen köpte från dig kan de begära ett byte. Att byta en reservation kan vara ett attraktivt alternativ till att avbryta en reservation eftersom det gör att kunden kan använda det jämförda återbetalningsbeloppet mot priset för den nya reservationen. 

Det prorrerade återbetalningsbeloppet krediteras till ditt konto så att du kan erbjuda kunden ett byte.

## <a name="request-a-refund-or-exchange-on-behalf-of-a-customer"></a>Begära en återbetalning eller byta för en kunds räkning

Om du vill skicka en supportbegäran om återbetalning eller utbyte för dina kunders räkning väljer du kunden och reservationen i Partnercenter och skapar sedan supportbegäran i Azure Portal. 

>[!NOTE]
>Microsoft Support kan be dig att ange reservations-ID och reservationsbeställnings-ID. Du hittar den här informationen på sidan Egenskaper **för** reservationen i Azure Portal.

1. Kom igång genom att välja **Kunder** på menyn i Partnercenter och sedan välja den kund som vill få en återbetalning. 

2. På kundens informationssida väljer du **Azure-reservationer och** sedan den specifika reservation som kunden vill få återbetalning för.  

3. Under **Åtgärder** väljer du **Återbetalning** för att gå till kundens reservationspost i Azure Portal och initiera en supportbegäran.  

4. På sidan **Ny supportbegäran** följer du stegen nedan för att begära en återbetalning. Välj **Nästa** efter varje steg. 

   |**Steg**                    |**Val**    |
   |:---------------------------|:-----------------|
   |**1 Grunderna**                |Typ av problem: Fakturering.  |
   |**2 Problem**               |Problemtyp: Reservationshantering. Kategori: Utbyten och återbetalningar. |
   |**3 Kontaktinformation**   |Välj dina inställningar och ange den information som krävs. 

5. Välj **Skapa när** du är klar.

## <a name="azure-reservations-resources"></a>Resurser för Azure-reservationer

|**För information om**   |**Läs detta**    |
|:-----------------------------|:-----------------|
|Översikt över Azure-reservationer i CSP  | [Sälja Microsoft Azure reserverade instanser](azure-reservations.md) |
|Köpa Azure-reservationer för dina kunder i Partnercenter   | [Köpa Azure-reservationer](azure-reservations-buying.md) |
|Fastställ rätt VM-storlek och verifiera kundens VM-användning   | [VM-storlek för maximal användning av Azure-reservationer](azure-usage.md)   |
|Köpa Azure-reservationer med partnercenter-API:et | [Köp Azure Reserved VM Instances](/partner-center/develop/purchase-azure-reservations) i utvecklardokumentationen för Partnercenter   |
|Ge kunderna tillstånd att köpa sina egna Azure-reservationer från en prenumeration som du har köpt åt dem. | [Ge kunderna behörighet att köpa sina egna Azure-reservationer](give-customers-permission.md)   |