---
title: Incitament för kundassociationer
description: Förstå viktiga processer och tidslinjer för att hantera CPOR-kundassociationer (Claimed Partner of Record).
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
ms.topic: how-to
author: Karthic83
ms.author: kashanum
ms.localizationpriority: medium
ms.date: 09/11/2020
ms.openlocfilehash: d99de8ed53ae6ed7fa094f6da7a8947c1bcfccb9
ms.sourcegitcommit: ad1af627f5ee6b6e3a70655f90927e932cf4c985
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 07/29/2021
ms.locfileid: "114836514"
---
# <a name="manage-incentives-customer-associations"></a>Hantera incitament för kundassociationer

**Lämpliga roller:** Faktureringsadministratör | Globala | Incitamentsadministratör

CPOR-plattformen (Claimed Partner of Record) används för partner för att associera sig med slutanvändare som de påverkar användning eller inköp av Microsoft-produkter för. För närvarande stöder CPOR-plattformen Business Applications och Microsoft 365 produkter. Partner använder den här associationsmetoden för att få insyn i kundernas prestanda, få incitamentsbetalningar via OSU- och OSA-programmen och få intäktsassociata som affärsinfluerare.  

## <a name="how-your-cpor-association-claim-relates-to-incentives"></a>Hur ditt CPOR-associationsanspråk relaterar till incitament

Om du har gjort ett CPOR-associationsanspråk och det har godkänts är du nu associerad med kunden. Det innebär inte att anspråket godkänns för incitamentintäkter eller utbetalning. Din guide för incitamentprogram beskriver behörighetskraven för incitament som ska betalas ut baserat på godkända anspråk.

Du hittar dina incitamentprogramguider på [Microsoft Partner Network](https://aka.ms/partnerincentives).

Om ditt CPOR-associationsanspråk godkänns och är berättigat till incitament kan du verifiera prenumerationen eller klientorganisations-ID:t i intäkts- och utbetalningsrapporteringen. 

## <a name="cpor-association-claims-timeline"></a>Tidslinje för CPOR-associationsanspråk

- Skickat: Det skickas i upp till fem arbetsdagar tills Microsoft startar godkännandeprocessen.
- Under Granska: Microsoft har fem arbetsdagar på sig att fatta ett beslut baserat på det utförandebevis som du anger.
- Partneråtgärd krävs: Om en granskare skickar kommentarer till dig och en begäran om ytterligare information har du fem arbetsdagar på dig att svara. Ett beslut bör fattas om ditt CPOR-associationsanspråk inom 10 dagar baserat på granskarens serviceavtal, plus hur lång tid det tar att tillhandahålla poE-granskare (proof of execution) med ytterligare information.
- Godkänd: Ditt CPOR-associationsanspråk har godkänts. När din association har godkänts skickas ett meddelande till kunden som ger dem möjlighet att neka din association. Kunden har sedan sju dagar på sig att avanmäla sig. När medgivandeperioden har passerat skickas anspråket för att utvärdera berättigandet för incitamentprogram.

## <a name="view-the-status-of-your-cpor-association-claim"></a>Visa status för ditt CPOR-associationsanspråk

Du kan när som helst kontrollera statusen för ditt CPOR-associationsanspråk med hjälp av [instrumentpanelen för](https://partner.microsoft.com/dashboard/incentives/claims/associations) kundassociationer (inloggning krävs).

Här är statusen och deras innebörd:

| Anspråksstatus | Visas när |
| ------ | ----------- | 
|  Redigering  | Ditt CPOR-associationsanspråk har skapats. Den förblir i det här tillståndet tills du laddar upp beviset för körningsdokumentet och skickar anspråket för godkännande.   |
|  Skickad  | Partnern har skickat sitt CPOR-associationsanspråk men Microsoft har ännu inte startat granskningsprocessen.   |
|  Under granskning  | Microsoft har börjat verifiera PoE-dokumentationen. Vi kan kontakta dig om du vill ha mer information. Granskningsprocessens serviceavtal är fem arbetsdagar.  |
|  Avslagen  | PoE var otillräckligt, eller så svarade du inte inom fem arbetsdagar enligt PoE-granskningsriktlinjerna och anspråket har nekats.   |
|  Godkända  | Anspråket har godkänts. Efter Microsofts godkännande har kunden gett möjlighet att neka din association. Kunden har sju dagar på sig att avanmäla sig efter Microsofts godkännande. Även om ditt anspråk visas som godkänt skickas det endast för incitamentutvärdering efter medgivandeperioden har passerat.   |
|  Partneråtgärd krävs  | Microsoft har granskat PoE för ditt CPOR-associationsanspråk och behöver mer information om din PoE för de produkter/arbetsbelastningar som du har begärt. Du har fem arbetsdagar på dig att ange den begärda informationen och skicka in anspråket på nytt, annars avvisas det. Nedan är potentiella orsaker till varför ytterligare kan behövas:

- Missing All PoE (PoE saknas) – PoE saknas på grund av att felaktig fil har laddats upp eller gäller inte för CPOR-associationsanspråket

- Kundsignaturen för kundbekräftelse saknas inte i PoE

- Missing or Old Dates (Saknade eller gamla datum) – Datum på PoE saknas eller är gamla i förhållande till anspråket

- Missing Partner Solution/Service (Partnerlösning/-tjänst saknas) – Beskrivningen av arbete du har slutfört är otillräckligt i dokumentet

- Missing Products (Produkter saknas) – PoE innehåller inte en produkt eller arbetsbelastning som anspråket gäller 

## <a name="dispute-the-status-of-a-cpor-association-claim"></a>Bestrida status för ett CPOR-associationsanspråk

Om ditt CPOR-associationsanspråk avvisas har du 30 dagar på dig att bestrida avvisningen. I e-postmeddelandet du får om avvisningen anges också var du kan se orsaken till avvisningen och hur du bestrider den.  

Om 30 dagar har passerat och du fortfarande vill bestrida ett avvisat anspråk måste du skicka en ny koppling med ditt uppdaterade PoE (Proof of Execution). 

### <a name="to-dispute-a-rejected-claim"></a>Så här bestrider du ett avvisat anspråk

1. Logga in på [instrumentpanelen i Partnercenter](https://partner.microsoft.com/dashboard/).
2. Öppna det anspråk som du vill bestrida.
3. På anspråkssidan väljer du **Bestrid**.
4. Ange en affärs motivering och/eller en uppdaterad PoE som förklarar varför avvisningen bör övervägas.
5. När du är klar med att lägga till information väljer du **Dispute** (Bestrid). Våra granskare bör kontakta dig med resultat inom fem arbetsdagar.

## <a name="reasons-a-cpor-association-claim-is-rejected"></a>Orsaker till att ett CPOR-associationsanspråk avvisas

Det finns tre huvudsakliga orsaker till att ett CPOR-associationsanspråk avvisas.

**Partnerbegäran:** Partner kan begära att deras association avvisas. Den här logiken används främst när partnern har skapat ett CPOR-associationsanspråk av misstag med hjälp av ett felaktigt MPN, valt en felaktig aktivitet (till exempel om du har valt Intäktsassociating i stället för Förförsäljning) eller inte arbetar med kunden längre.

**Kundminskning:** När CPOR-associationsanspråket har gått igenom PoE-godkännandeprocessen ändras dess status till Godkänd medan kunden ges möjlighet att neka medgivande för associationen. Om kunden nekar till medgivande avvisas associationen.

**Otillräckligt bevis för körning:** Proof of Execution krävs för varje CPOR-association. När ditt CPOR-associationsanspråk har skickats tar det upp till fem dagar för Microsofts granskare att granska din PoE och be om ytterligare information som behövs med hjälp av kommentarsavsnittet i ditt anspråk. Om informationen inte är tillräcklig avvisas ditt CPOR-associationsanspråk.

Andra möjliga orsaker till avvisandet:

- Kundmedgivande saknas i PoE
- Produkter som saknas
- Inget partnersvar
- PoE är inte tillgängligt

## <a name="edit-your-cpor-association-claim"></a>Redigera ditt CPOR-associationsanspråk

Du har möjlighet att redigera vissa fält i CPOR-associationsanspråket. Du kan bli ombedd att ta bort produkt(er)/arbetsbelastning(ar) om granskarna meddelar att PoE som skickats är otillräckligt. För att kunna redigera måste ditt CPOR-associationsanspråk vara i tillstånden Submitted (Skickat) eller Partner Action Required (Partneråtgärd krävs).

Fält som du kan redigera:

- MPN
- Produkter
- Kontaktinformation för kund och partner
- Lägga till ytterligare PoE och kommentarer

## <a name="customer-consent-notification"></a>Meddelande om kundmedgivande

När ditt CPOR-associationsanspråk har godkänts skickas ett meddelande till kunden som ger dem möjlighet att neka din association. Kunden har sedan sju dagar på sig att avanmäla sig. Din status under den här perioden visas som Godkänd. Om kunden nekar till medgivande avvisas associationen. När medgivandeperioden har passerat och kunden inte har nekat medgivande skickas anspråket för att utvärdera berättigandet för incitamentprogram.

## <a name="how-to-communicate-with-poe-reviewers"></a>Så här kommunicerar du med PoE-granskare

När granskarna har gått igenom PoE kan de komma fram till att ytterligare information behövs. I så fall kontaktar de dig via avsnittet Kommentarer i anspråket. Du kan även svara på dem i avsnittet Kommentarer.

## <a name="view-claim-history"></a>Visa anspråkshistorik

Längst upp till höger i CPOR-associationsanspråk  finns knappen Historik som gör att du kan se alla ändringar, kommentarer och åtgärder som vidtas på det här anspråket från en partners och granskares perspektiv.

## <a name="next-steps"></a>Nästa steg

- [Komma igång med incitament](incentives-get-started-intro.md)