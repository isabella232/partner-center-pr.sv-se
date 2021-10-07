---
title: Intäktssammanfattning på instrumentpanelen i Partnercenter
description: Du kan använda intäktssammanfattningen för att förstå hur intäkter som genereras av kundförbrukning av Azure-tjänster bidrar till dina intäkter och varför vissa intäkter kan fastställas som ojusterade för intäkter.
author: satinder37
ms.author: sabaja
ms.service: partner-dashboard
ms.topic: conceptual
ms.date: 10/04/2021
ms.custom: template-concept
customer intent: As an incentive user or incentive admin, I want to be able to read and export revenue data from Partner Center so I can see our earnings and learn why any transactions were reported ineligible.
ms.openlocfilehash: 11e58324adf38e92fc892ec5dd62933e6372f2cb
ms.sourcegitcommit: 76a7dac540d129ae15cd4c251a4ff43d768370da
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 10/06/2021
ms.locfileid: "129593352"
---
# <a name="revenue-summary"></a>Intäktssammanfattning

Du kan använda intäktssammanfattningen för att förstå hur intäkter som genereras av kundförbrukning av Azure-tjänster bidrar till dina intäkter och varför vissa intäkter kan fastställas som ojusterade för intäkter.

:::image type="content" source="images/revenue-summary/revenue-reporting-diagram.png" alt-text="Diagram över hur intäkter utvärderas och rapporteras på Partnercenter":::

Intäktssammanfattningen uppdateras först efter att transaktioner har utvärderats, så Azure-förbrukning som äger rum i oktober visas inte i intäktssammanfattningen förrän i november, till exempel.

Intäktssammanfattningen finns på arbetsytan Utbetalningar, tillsammans med sidan [Transaktionshistorik](https://partner.microsoft.com/dashboard/payouts/reports/transactionhistory) [och Betalningar.](https://partner.microsoft.com/dashboard/payouts/reports/incentivepayments)

## <a name="using-the-revenue-summary"></a>Använda intäktssammanfattningen

Med hjälp av intäktssammanfattningen kan du:

- Leta upp berättigade intäkter och mängden resulterande intäkter per kund eller prenumeration.
- Komplettera det du lär dig i [transaktionshistoriken med](https://partner.microsoft.com/dashboard/payouts/reports/transactionhistory)  insikter om underliggande intäktsbelopp.
- Leta upp eventuella icke-justerade intäkter och ta reda på varför dessa intäkter klassificerades som icke-ligaliga.
- Exportera data om icke-justerade [](#ineligibility-reasons) transaktioner, inklusive orsaker och attribut som inte är liga, [](#exported-data-attributes)vilket hjälper dig att förstå varför dessa transaktioner inte gav incitament.

## <a name="access-roles-and-permissions"></a>Åtkomstroller och behörigheter

Incitamentanvändare och incitamentsadministratörer har åtkomst till intäktssammanfattningen.
Informationen som är tillgänglig i sammanfattningen beror på vilka kombinationer av program och Microsoft Partner Network (MPN) som dessa användare och administratörer har åtkomst till (precis som med transaktionshistorik och betalningssidor). (Se [Tilldela roller och behörigheter för](permissions-overview.md) att lära dig mer om att konfigurera användare med roller och lösenord.)

## <a name="when-data-is-available"></a>När data är tillgängliga

Azure-förbrukningsdata utvärderas vanligtvis flera veckor efter den månad då transaktionerna sker. Information om intäktssammanfattning uppdateras bara när utvärderingen är klar. Detta resulterar i en fördröjning mellan när transaktioner inträffar och när de rapporteras, så att du inte kan se förbrukningen för den aktuella månaden i sammanfattningen intäkter. Till exempel skulle data för mars vanligtvis utvärderas ungefär den tredje veckan i april, och information om intäktssammanfattningen skulle vanligtvis uppdateras strax därefter.

## <a name="customer-summary-view"></a>Sammanfattningsvy för kund

I vyn Kundsammanfattning visas aggregerade intäkter efter kundnamn och program/engagemang.

Här är några exempel på insikter från kundsammanfattningen:

- **De 10 främsta efter berättigade intäkter** visar att de 10 främsta kunderna bidrar till de högsta berättigade intäkterna.
- **De 10 främsta efter ojusterade intäkter** visar att de 10 främsta kunderna bidrar till de högsta intäkterna som inte är liga.
- **De 10 främsta efter intäkter** visar att de 10 främsta kunderna bidrar till maximala intäkter.

Du kan söka efter information om alla kunder i kundsammanfattningen, inte bara de 10 främsta.

## <a name="eligible-transactions"></a>Berättigade transaktioner

*Berättigade transaktioner är* transaktioner som producerar intäkter som är berättigade till intäkter.

Du kan söka efter information om berättigade transaktioner efter kund-ID eller prenumerations-ID. Du kan dock inte exportera data om berättigade transaktioner.

## <a name="ineligible-transactions"></a>Icke-justerade transaktioner

*Icke-liga transaktioner* är transaktioner som inte är justerade för intäkter.

- Orsakerna till varför transaktioner betraktas som ojusterade för intäkter anges i avsnittet [Ineligibility reasons i](#ineligibility-reasons) den här artikeln.
- Du kan söka efter och  [exportera data](#exporting-data) om icke-liga transaktioner för att få hjälp med att ta reda på varför du kanske inte har fått MCI-incitament.
- I intäktssammanfattningen visas alltid den senaste intäktsklassificeringen (så du kan inte se hur en transaktion klassificerades en månad tidigare). En transaktion som är markerad som icke-berättigad en månad kan markeras som berättigad nästa månad.

Icke-liga transaktioner som anges i intäktssammanfattningen har attribut som omfattar:

- produkt
- intäkter som inte är liga
- [orsak till ineligibility](#ineligibility-reasons)
- subscription ID
- kundnamn (vanligtvis tillgängligt när en prenumeration har fakturerats för första gången)

Du kan söka efter icke-giltigt transaktioner efter kundnamn och prenumerations-ID. (Antalet poster som visas är begränsat till 10.) Om informationen du hittar inte besvarar dina frågor kan du kontakta supporten för att få hjälp.

## <a name="ineligibility-reasons"></a>Orsaker till ineligibility

*Ineligibility reasons* in the tables that follow indicate why revenue was classified ineligible for earnings. Varje rad i tabellerna har också en förklaring om huruvida och hur en partner med oberättigande intäkter kan bli berättigad till intäkter igen.

Vissa orsaker till ineligibility i dessa tabeller kanske inte gäller för ett visst engagemang.

Det finns tre kategorier av inkompatibilitet:

- [Kund som inte är tillgänglig](#ineligible-customer)
- [Icke-liglig partner](#ineligible-partner)
- [Icke-liglig transaktion](#ineligible-transaction)

### <a name="ineligible-customer"></a>Kund som inte är tillgänglig

|Orsak till ineligibility|Partneråtgärd krävs?|Så här blir du berättigad igen|
|---------|---------|---------|
|Kunden är offentlig sektor|Ja, om kunden är i USA, Gör det eller Indien|Om du svarade på en POE-begäran (Proof of Execution) och den avvisades kan du inte bli berättigad igen. (När en POE avvisas skickas ett e-postmeddelande som förklarar varför.)<br><br>Du kan begära en annan POE inom 90 dagar efter transaktionens/intäktsdatumet. (Se till att bekräfta att poE-e-postmeddelandet har mottagits när det tas emot.) Du kan också bestrida ineligibility inom 90 dagar genom att kontakta supporten med orsaken till ineligibility, prenumerations- och kundinformation och orsaken till en konflikt.|
|Intäkter från Kina bör inte tillhöra partner som inte tillhör Kina|No|Partnern kan inte bli berättigad igen av en princip.|

### <a name="ineligible-partner"></a>Icke-liglig partner

|Orsak till ineligibility|Partneråtgärd krävs|Så här blir du berättigad igen|
|---------|---------|---------|
|Avancerat specialiseringskrav har inte uppfyllts|Yes|[Lär dig mer om avancerade specialiseringar](advanced-specializations.md)|
|Kompetensstatusen uppfylls inte eller har upphört att gälla|Yes|Visa kompetensstatusen i [Kompetenser.](https://partner.microsoft.com/pcv/partnership/competencies) Visa de kompetenser som krävs för ditt engagemang [på Incentives Engagements](https://partner.microsoft.com/dashboard/incentives/engagements/ux)|
|MPA-avtalet har upphört att gälla eller är inte signerat|Yes|Verifiera och signera MPA-avtalet genom vägledning om [Microsoft-partneravtal för CSP-programpartner](microsoft-partner-agreement.md)|
|Berättigandet till säljförsäljning har upphört att gälla eller har inte upprättats|Yes|Mer [information finns i Översikt över säljteam och partner i Microsofts säljteam](/azure/marketplace/co-sell-overview)|
|Partnerplats är inte berättigad till incitament|No|Partnern kan inte bli berättigad igen av en princip|
|MPN-ID som inte är berättigat till att delta i engagemang|No|Partnern kan inte bli berättigad igen av en princip|

### <a name="ineligible-transaction"></a>Icke-liglig transaktion

|Orsak till ineligibility|Partneråtgärd krävs?|Så här blir du berättigad igen|
|---------|---------|---------|
|Bevis på körning godkänns inte|Ja, om du inte har svarat på ett DPOR-bevis (Digital Partner of Record) som krävs (POE) via e-post från Microsoft|Bevis på körningsbegäran gäller endast för offentlig sektor eller DPOR. Från och med den 1 oktober 2021 är DPOR inte längre incentivt för Azure, så POE-begäranden skickas inte.<br><br>Om du har svarat på ett e-postmeddelande med ämnet "Proof of execution required" (Bevis på utförande krävs) och svaret avvisades kan du inte bli berättigad igen.|

## <a name="exporting-data"></a>Exportera data

Du kan ladda ned information om ej berättigade transaktioner (men inte berättigade transaktioner) i intäktssammanfattningen.

:::image type="content" source="images/revenue-summary/export-data-page.png" alt-text="Skärmbild av sidan Exportera data i Partnercenter":::

### <a name="exported-data-attributes"></a>Exporterade dataattribut

Attribut för icke-liga transaktioner är:

|Attributnamn  |Description  |
|---------|---------|
|agreementNumber|Avtalsnummer (endast tillgängligt som tillämpligt)|
|customerId|Identitet för den kund som är associerad med en prenumeration/resurs. (För Azure-förbrukning är den här informationen inte tillgänglig för de första 30 till 45 dagarna i en ny prenumeration såvida inte den första fakturan har skapats.)|
|customerIdType|TPID- eller MCAPI-ID|
|customerName|Namn på kund|
|invoiceNumber|Fakturanummer (endast tillgängligt för partnerledda, fältledda och kundledda)|
|partnerCountryCode|Registrerad MPN-plats|
|partnerId|MPN-ID för den registrerade partnern|
|partnerName|Namnet på partnern|
|productId|Produktnamn för handel|
|productFamily|Produktfamilj|
|orsak|Orsak till ineligibility|
|subscriptionId|Prenumerations-ID:t|
|transactionAmountUSD|Förbrukningsbelopp i amerikanska dollar|
|transactionDate|Datum för förbrukning eller fakturering
|unearnedId|Unik identifierare som kan hjälpa dig att skapa en supportförfrågan|
|workload|Namn på tjänst eller arbetsbelastning|

## <a name="next-steps"></a>Nästa steg

Mer information om transaktioner, intäkter, intäkter och betalningar finns i följande artiklar.

- Visa sidan [Transaktionshistorik](https://partner.microsoft.com/dashboard/payouts/reports/transactionhistory) om du vill visa intäkter och tillhörande transaktionsinformation för alla dina program med motsvarande betalningsstatus.
- Visa sidan [Betalningar för](https://partner.microsoft.com/dashboard/payouts/reports/incentivepayments) att visa slutförda och väntande betalningar för alla dina program.
- Visa sidan [Utbetalningsutdrag](payout-statement.md) för att få en översikt över dina utbetalningserbjudanden från erbjudanden som säljs via den kommersiella marknadsplatsen.
