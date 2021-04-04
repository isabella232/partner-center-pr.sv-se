---
title: Problem med incitament och kundassociationer
description: Lär dig hur du löser problem som uppstår när du arbetar med CPOR-kundkopplingar (påstått partner of Record).
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
author: Karthic83
ms.author: kashanum
ms.localizationpriority: medium
ms.date: 09/11/2020
ms.openlocfilehash: 30639725c0a852046251e83c3791f56d788931c1
ms.sourcegitcommit: 6498c57e75aa097861523b206dc142f789deeb36
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/02/2021
ms.locfileid: "106179222"
---
# <a name="issues-with-claimed-partner-of-record-cpor-customer-associations"></a>Problem med CPOR-kundkopplingar (påstått partner of Record)

**Lämpliga roller**

- Faktureringsadministratör
- Global administratör
- Incitaments administratör

Innehållet nedan hjälper dig att lösa problem som kan uppstå när du arbetar med kund kopplingar.

## <a name="domain-tenant-mismatch"></a>Domän-klient matchnings fel

I anspråks partnern för anspråks partner (CPOR) uppmanas du att ange kundens klient-ID och under domän. Om du får ett fel meddelande om att de inte matchar kan du kontakta kunden och se till att du har rätt information.

## <a name="subscription-errors-in-the-cpor-association-claim-flow"></a>Prenumerations fel i CPOR Associations anspråks flödet

I CPOR Associations anspråks flödet kan du bli ombedd att ange en prenumeration för en produkt som du försöker att begära via Business Applications (Dynamics 365). Vi ber om prenumerationen eftersom vi dynamiskt kontrollerar att produkten och prenumerationen tillhör innehavaren som begärs. Vi kontrollerar också att prenumerationen befinner sig i aktiv/i Grace-status.

Om du får ett fel meddelande kan det bero på flera orsaker:

- Den valda produkten finns inte i kundens klientorganisation
- Den tillhandahållna prenumerationen är inte för Dynamics
- Den angivna prenumerationen är för CSP
- Kunden har ännu inte Aktiver ATS/etablerat produkter för den prenumerationen
- Prenumerationen har redan begärts
- Den angivna identifieraren är inget prenumerations-ID

Om du har frågor om din prenumerations precision kan du arbeta med kunden för att se till att prenumerationen är korrekt och att du använder rätt klient-ID.

Kontakta [supporten](https://partner.microsoft.com/dashboard/support/incentives/servicerequests?category=incentives)om den här vägen inte har löst problemet.

## <a name="when-subscriptions-will-be-available-to-claim"></a>När prenumerationer kommer att vara tillgängliga för anspråk

När du begär en prenumeration får du ett fel meddelande om prenumerationen ännu inte har etablerats. Det finns flera steg som kunden måste vidta för att prenumerationen ska bli tillgänglig för CPOR-plattformen för att kunna välja den och göra den tillgänglig för anspråk. Om du får ett fel meddelande när du försöker att begära en prenumeration kan du kontakta kunden för att kontrol lera att den har etablerats och att den prenumeration du ansöker är korrekt. Kontakta [supporten](https://partner.microsoft.com/dashboard/support/incentives/servicerequests?category=incentives)om du redan har tagit den här vägen.

## <a name="which-activity-do-i-choose"></a>Vilken aktivitet väljer jag?

CPOR-anspråks plattformen gör det möjligt för CPOR Associations anspråk relaterade till Business Applications och Microsoft 365 lösnings områden. De aktiviteter som gäller för varje lösnings områden nedan. Välj rätt aktivitet baserat på beskrivningarna för att undvika att behöva frigöra i framtiden. Anspråk på en felaktig aktivitet kan resultera i utebliven berättigande och incitaments vinster.


| Lösningsområde | Aktivitet | Tillämpligt för |
| ------ | ----------- | ----------- |
| Affärs program      | Före försäljning   | Välj om du har påverkat inköp av en berättigad produkt och vill ansöka om förskotts incitament. Det här alternativet kan bara användas om kunden har köpt dessa produkter via volym licens avtal eller webb-direkt. |
|    |  Användning  | Välj om du vill att deras antagande och användning av en berättigad arbets belastning ska användas och om du vill använda för användnings incitament. Det här alternativet kan bara användas om kunden har köpt dessa produkter via volym licens avtal eller webb-direkt. |
|    | Intäkts koppling   | Välj om du har påverkat valet av en berättigad produkt som en verksamhets påverkan. Det här alternativet gäller endast för intäkts associationer, inte för incitaments betalningar. Det här alternativet kan bara användas om kunden har köpt dessa produkter via volym licens avtal eller webb-direkt.   |
| Microsoft 365   | Användning   | Välj om du vill att deras antagande och användning av en berättigad arbets belastning ska användas och om du vill använda för användnings incitament. |

## <a name="which-mpn-do-i-choose"></a>Vilken MPN väljer jag?

I CPOR Associations anspråks flödet uppmanas du att välja ett företags-MPN som ska kopplas till det arbete som du anspråkerar för slutanvändaren. Ditt företag kan ha många MPNs, varav vissa kan vara registrerade i incitaments program och andra som är associerade med en partner typ, till exempel FRP FastTrack. CPOR Associations anspråks flödet identifierar vilka MPNs som är registrerade i ett incitaments program, men det kommer inte att meddela dig om det är en speciell partner typ MPN. Det är viktigt att välja rätt MPN för att undvika att behöva göra anspråk i framtiden. Anspråk på en felaktig MPN kan resultera i utebliven berättigande och incitament.

Om du inte vet vilken MPN du ska använda kontaktar du din globala administratör.

Om den MPN som du vill använda inte är registrerad kan du hantera den på [fliken incitament översikt](https://partner.microsoft.com/dashboard/incentives/enrollment/summary) (inloggning krävs).

## <a name="choosing-a-product-vs-entering-a-subscription"></a>Välja en produkt kontra att ange en prenumeration

När en Dynamics-produkt begärs och godkänns, kan partnern Visa prenumerations-ID: t i själva CPOR-Associerings anspråket. När den här prenumerationen har begärts, är den aktiv eller i Grace-status, men det kan finnas en tid när prenumerationen upphör och nya prenumerationer måste begäras i ett separat CPOR Associations anspråk.

## <a name="competing-claims"></a>Konkurrerande anspråk

Om du skapar ett CPOR Associations anspråk för en kund och deras produkt som redan är kopplad till en annan partner, kommer ditt anspråk att gå igenom medlingen:

1. När du har skapat en ny kundassociation kommer Microsoft att kontrollera informationen om associationen och PoE (Proof of Execution) för att bekräfta att de stämmer.

2. Om du och en annan partner ansöker samma kund och produkt/arbets belastning, kommer Microsoft att granska varje partners bevis på körnings dokumentation för att avgöra vilken partner som ska godkännas.

3. Ytterligare information kan begäras från båda partnerna, vilket kan orsaka fördröjningar vid bearbetning av din associerings förfrågan.

4. Ditt CPOR-associerings anspråk kommer fortfarande att granskas inom fem arbets dagar, även om dess status kan stanna som _under granskning under_ en längre tids period. Det här scenariot kan inträffa när Microsoft arbetar med den partner som för närvarande äger produkten/arbets belastningen. Du kommer att meddelas i avsnittet kommentarer i ditt anspråk om så är fallet. 

>[!IMPORTANT]
>Om vi behöver ytterligare information för att verifiera din CPOR-CPOR (PoE) kommer vi att kontakta dig via avsnittet om kommentarer för Association med.

## <a name="next-steps"></a>Nästa steg

- [Komma igång med incitament](incentives-get-started-intro.md)
