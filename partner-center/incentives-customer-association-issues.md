---
title: Problem med incitament och kundassociationer
description: Lär dig hur du kan åtgärda problem som kommer upp när du arbetar med kundassociationer för apostpartner (CPOR).
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
author: Karthic83
ms.author: kashanum
ms.localizationpriority: medium
ms.date: 09/11/2020
ms.openlocfilehash: 8f1c087911e6dd7e58182c99e2b97b7a6b2246d8
ms.sourcegitcommit: 1161d5bcb345e368348c535a7211f0d353c5a471
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/09/2021
ms.locfileid: "123960533"
---
# <a name="issues-with-claimed-partner-of-record-cpor-customer-associations"></a>Problem med kundassociationer för Apostpartner (CPOR)

**Lämpliga roller:** Faktureringsadministratör | Globala | Incitamentsadministratör

Innehållet nedan hjälper dig att lösa problem som kan komma upp när du arbetar med kundassociationer.

## <a name="domain-tenant-mismatch"></a>Matchningsfel för domän-klient

I CPOR-associationsanspråksflödet (Akust Partner of Record) uppmanas du att ange kundens klientorganisations-ID och underdomän. Om du får ett felmeddelande om att de inte matchar kontaktar du kunden för att kontrollera att du har rätt information.

## <a name="subscription-errors-in-the-cpor-association-claim-flow"></a>Prenumerationsfel i CPOR-associationsanspråksflödet

I CPOR-associationsanspråksflödet kan du bli ombedd att ange en prenumeration på en produkt som du försöker göra anspråk på via Business Applications (Dynamics 365). Vi ber om prenumerationen eftersom vi kontrollerar dynamiskt att produkten och prenumerationen tillhör den klientorganisation som begärs. Vi kontrollerar också att prenumerationen har statusen aktiv/i respit.

Om du får felet kan det ha flera orsaker:

- Den valda produkten finns inte i kundens klientorganisation
- Den angivna prenumerationen är inte för Dynamics
- Den angivna prenumerationen är för CSP
- Kunden har ännu inte aktiverat/etablerat produkterna för den prenumerationen
- Prenumerationen har redan begärts
- Den angivna identifieraren är inte ett prenumerations-ID

Om du har en fråga om korrektheten i din prenumeration kan du kontakta kunden för att säkerställa att prenumerationen är korrekt och att du använder rätt klientorganisations-ID.

Kontakta supporten om den här vägen inte har löst [problemet.](https://partner.microsoft.com/dashboard/support/incentives/servicerequests?category=incentives)

## <a name="when-subscriptions-will-be-available-to-claim"></a>När prenumerationer kommer att vara tillgängliga för anspråk

När du begär en prenumeration får du ett felmeddelande om prenumerationen inte har etablerats ännu. Det finns flera steg som kunden måste vidta för att prenumerationen ska bli tillgänglig för CPOR-plattformen för att hämta upp den och göra den tillgänglig för anspråk. Om du får ett felmeddelande när du försöker göra anspråk på en prenumeration kontaktar du kunden för att kontrollera att den har etablerats och att prenumerationen som du gör anspråk på är korrekt. Kontakta supporten om du redan har gått den [här vägen.](https://partner.microsoft.com/dashboard/support/incentives/servicerequests?category=incentives)

## <a name="which-activity-do-i-choose"></a>Vilken aktivitet väljer jag?

CPOR-anspråksplattformen möjliggör CPOR-associationsanspråk relaterade Business Applications och Microsoft 365 lösningsområden. De aktiviteter som gäller för varje lösningsområde finns nedan. Välj rätt aktivitet baserat på beskrivningarna för att undvika att behöva återta i framtiden. Anspråk med en felaktig aktivitet kan resultera i uteblivna berättigande- och incitamentintäkter.


| Lösningsområde | Aktivitet | Gäller för |
| ------ | ----------- | ----------- |
| Företagsprogram      | Förförsäljning   | Välj om du har påverkat deras köp av en berättigad produkt och vill ansöka om incitament före försäljning. Det här alternativet gäller endast om kunden har köpt dessa produkter via volymlicensavtal eller Web-Direct. |
|    |  Användning  | Välj om du driver implementeringen och användningen av en berättigad arbetsbelastning och vill ansöka om användningsincitament. Det här alternativet gäller endast om kunden har köpt dessa produkter via volymlicensavtal eller Web-Direct. |
|    | Intäktsassociaty   | Välj om du har påverkat deras val av en berättigad produkt som affärsinfluerare. Det här alternativet är endast för intäktsassociaty, inte för incitamentbetalningar. Det här alternativet gäller endast om kunden har köpt dessa produkter via volymlicensavtal eller Web-Direct.   |
| Microsoft 365   | Användning   | Välj om du driver implementeringen och användningen av en berättigad arbetsbelastning och vill ansöka om användningsincitament. |

## <a name="which-mpn-do-i-choose"></a>Vilket MPN väljer jag?

I CPOR-associationsanspråksflödet uppmanas du att välja ett företags-MPN som ska associeras med det arbete som du begär på slutanvändaren. Ditt företag kan ha många MPN, varav vissa kan registreras i incitamentprogram och andra som är associerade med en partnertyp, till exempel FRP-FastTrack. CPOR-associationsanspråksflödet identifierar vilka MPN som har registrerats i ett incitamentprogram, men det visar inte om det är en specifik partnertyp MPN. Det är viktigt att välja rätt MPN för att undvika att behöva frigöra i framtiden. Anspråk med ett felaktigt MPN kan resultera i uteblivna intäkter för berättigande och incitament.

Kontakta din globala administratör om du inte vet vilket MPN du ska använda.

Om det MPN som du vill använda inte har registrerats kan du hantera det på fliken [Incitamentsöversikt](https://partner.microsoft.com/dashboard/incentives/enrollment/summary) (inloggning krävs).

## <a name="choosing-a-product-vs-entering-a-subscription"></a>Välja en produkt jämfört med att ange en prenumeration

När en Dynamics-produkt begärs och godkänns kan partnern visa prenumerations-ID:t i själva CPOR-associationsanspråket. När den här prenumerationen begärs har den aktiv eller respitstatus, men det kan finnas en tid när prenumerationen upphör och de nya prenumerationerna måste begäras i ett separat CPOR-associationsanspråk.

## <a name="competing-claims"></a>Konkurrerande anspråk

Om du skapar ett CPOR-associationsanspråk för en kund och deras produkter som redan är associerade med en annan partner, kommer ditt anspråk att gå igenom ett skiljeavtal:

1. När du har skapat en ny kundassociation kommer Microsoft att kontrollera informationen om associationen och PoE (Proof of Execution) för att bekräfta att de stämmer.

2. Om du och en annan partner begär samma kund och produkt/arbetsbelastning granskar Microsoft varje partners bevis på utförandedokumentationen för att avgöra vilken partner som ska godkännas.

3. Ytterligare information kan begäras från båda partnerna, vilket kan orsaka fördröjningar i bearbetningen av din associationsbegäran.

4. Ditt CPOR-associationsanspråk kommer fortfarande att granskas inom fem arbetsdagar, även om dess status kan vara _Under_ Granskning under en längre tidsperiod. Det här scenariot kan inträffa när Microsoft arbetar med den partner som för närvarande äger produkten/arbetsbelastningen. Du meddelas i kommentarsavsnittet i anspråket om så är fallet. 

>[!IMPORTANT]
>Om vi behöver ytterligare information för att verifiera ditt CPOR-associationsbevis (PoE) kontaktar vi dig via avsnittet CPOR-associationsanspråkskommentarer.

## <a name="next-steps"></a>Nästa steg

- [Komma igång med incitament](incentives-get-started-intro.md)
