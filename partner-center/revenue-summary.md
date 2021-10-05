---
title: Intäktssammanfattning på instrumentpanelen i Partnercenter
description: Du kan använda intäktssammanfattningen för att visa intäkter och intäkter och exportera data om eventuella icke-justerade transaktioner.
author: satinder37
ms.author: sabaja
ms.service: partner-dashboard
ms.topic: conceptual
ms.date: 10/04/2021
ms.custom: template-concept
customer intent: As an incentive user or incentive admin, I want to be able to read and export revenue data from Partner Center so I can see our earnings and learn why any transactions were reported ineligible.
ms.openlocfilehash: 9ec9d64127f537ac74615a8fbe17499ebb5872dd
ms.sourcegitcommit: cf8c78e0c8831371432007d5ab05f934f15a77b5
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 10/05/2021
ms.locfileid: "129528664"
---
# <a name="revenue-summary"></a>Intäktssammanfattning

Du kan använda intäktssammanfattningen för att förstå hur intäkter som genereras av kundförbrukning av Azure-tjänster bidrar till dina intäkter och varför vissa intäkter inte kan fastställas för intäkter.

:::image type="content" source="images/revenue-summary/revenue-reporting-diagram.png" alt-text="Diagram över hur intäkter utvärderas och rapporteras i Partnercenter":::

Intäktssammanfattningen uppdateras först efter att transaktioner har utvärderats, så Azure-förbrukning som sker i oktober visas inte i intäktssammanfattningen förrän i november, till exempel.

Intäktssammanfattningen finns på arbetsytan Utbetalningar, tillsammans med sidan [Transaktionshistorik](https://partner.microsoft.com/dashboard/payouts/reports/transactionhistory) [och Betalningar.](https://partner.microsoft.com/dashboard/payouts/reports/incentivepayments)

## <a name="using-the-revenue-summary"></a>Använda intäktssammanfattningen

Med hjälp av intäktssammanfattningen kan du:

- Leta upp berättigade intäkter och mängden resulterande intäkter per kund eller prenumeration.
- Komplettera det du lär dig i [transaktionshistoriken med](https://partner.microsoft.com/dashboard/payouts/reports/transactionhistory)  insikter om underliggande intäktsbelopp.
- Leta upp eventuella icke-justerade intäkter och ta reda på orsaken till att dessa intäkter klassificerades som icke-justerade.
- Exportera data om icke-justerade [](#ineligibility-reasons) transaktioner, inklusive orsaker och attribut som inte är justerade, [](#exported-data-attributes)vilket hjälper dig att förstå varför dessa transaktioner inte gav incitament.

## <a name="access-roles-and-permissions"></a>Åtkomstroller och behörigheter

Incitamentanvändare och incitamentsadministratörer har åtkomst till intäktssammanfattningen.
Informationen som är tillgänglig i sammanfattningen beror på vilka kombinationer av program och Microsoft Partner Network (MPN) som dessa användare och administratörer har åtkomst till (precis som med transaktionshistorik och betalningssidor). (Se [Tilldela roller och behörigheter för](permissions-overview.md) att lära dig mer om att konfigurera användare med roller och lösenord.)

## <a name="when-data-is-available"></a>När data är tillgängliga

Azure-förbrukningsdata utvärderas vanligtvis flera veckor efter den månad då transaktionerna sker. Sammanfattningsinformation om intäkter uppdateras bara när utvärderingen är klar. Detta resulterar i en fördröjning mellan när transaktioner inträffar och när de rapporteras, så att du inte kan se förbrukningen för den aktuella månaden i intäktssammanfattningen. Till exempel skulle data för mars vanligtvis utvärderas ungefär den tredje veckan i april, och information om intäktssammanfattningen skulle vanligtvis uppdateras strax därefter.

## <a name="customer-summary-view"></a>Sammanfattningsvy för kund

Vyn Kundsammanfattning visar aggregerade intäkter efter kundnamn och program/engagemang.

Insikter om kundsammanfattning är:

- **De 10 främsta efter berättigade intäkter** visar att de 10 främsta kunderna bidrar till de högsta berättigade intäkterna.
- **De 10 främsta efter intäkter som inte** är justerade visar att de 10 främsta kunderna bidrar till de högsta intäkterna som inte är justerade.
- **De 10 främsta efter intäkter** visar de 10 främsta kunderna som bidrar till maximala intäkter.

Du kan söka efter information om alla kunder i kundsammanfattningen, inte bara de 10 främsta.

## <a name="eligible-transactions"></a>Berättigade transaktioner

*Berättigade transaktioner är* transaktioner som ger intäkter som är berättigade till intäkter.

Du kan söka efter information om berättigade transaktioner efter kund-ID eller prenumerations-ID. Du kan dock inte exportera data om berättigade transaktioner.

## <a name="ineligible-transactions"></a>Icke-justerade transaktioner

*Icke-justerade transaktioner* är transaktioner som inte är justerade för intäktsbetalningar.

- Orsakerna till varför transaktioner anses vara ojusterade för intäkter anges i avsnittet [Orsaker till ineligibilitet](#ineligibility-reasons) i den här artikeln.
- Du kan söka efter och  [exportera data](#exporting-data) om eventuella icke-justerade transaktioner för att ta reda på varför du kanske inte har fått MCI-incitament.
- Intäktssammanfattningen visar alltid den senaste intäktsklassificeringen (så du kan inte se hur en transaktion klassificerades en månad tidigare). En transaktion som är markerad som icke-berättigad en månad kan markeras som berättigad nästa månad.

Icke-liga transaktioner som anges i intäktssammanfattningen har attribut som omfattar:

- produkt
- Intäkter som inte är justerade
- [orsak till ineligibility](#ineligibility-reasons)
- subscription ID
- kundnamn (vanligtvis tillgängligt när en prenumeration har fakturerats för första gången)

Du kan söka efter icke-giltigt transaktioner efter kundnamn och prenumerations-ID. (Antalet poster som visas är begränsat till 10.) Om informationen du hittar inte besvarar dina frågor kan du kontakta supporten för hjälp.

## <a name="ineligibility-reasons"></a>Orsaker till ineligibility

*Orsaker till ineligibilitet* i de tabeller som följer visar varför intäkterna klassificerades som ojusterade för intäkter. Varje rad i tabellerna har också en förklaring om huruvida och hur en partner med oberättigande intäkter kan bli berättigad till intäkter igen.

Vissa orsaker till ineligibility i dessa tabeller kanske inte är tillämpliga för ett visst engagemang.

Det finns tre kategorier av inkompatibilitet:

- [Kund som inte kan berättigas](#ineligible-customer)
- [Icke-justerad partner](#ineligible-partner)
- [Icke-justerad transaktion](#ineligible-transaction)

### <a name="ineligible-customer"></a>Kund som inte kan berättigas

|Orsak till ineligibility|Partneråtgärd krävs?|Så här blir du berättigad igen|
|---------|---------|---------|
|Kunden är offentlig sektor|Ja, om kunden finns i USA, Puerto Puerto eller Indien|Om du har svarat på en POE-begäran (Proof of Execution) och den avvisades kan du inte bli berättigad igen. (När ett POE avvisas skickas ett e-postmeddelande som förklarar varför.)<br><br>Du kan begära en annan POE inom 90 dagar från transaktions-/intäktsdatumet. (Se till att bekräfta att du har fått POE-e-postmeddelandet när det tas emot.) Du kan också bestrida ineligibility inom 90 dagar genom att kontakta supporten med orsaken till ineligibility, prenumerations- och kundinformation och orsaken till en konflikt.|
|Kinaintäkter bör inte tillhöra partner som inte tillhör Kina|No|Partnern kan inte bli berättigad igen av en princip.|

### <a name="ineligible-partner"></a>Icke-justerad partner

|Orsak till ineligibility|Partneråtgärd krävs|Så här blir du berättigad igen|
|---------|---------|---------|
|Avancerat specialiseringskrav uppfylls inte|Yes|[Lär dig mer om avancerade specialiseringar](advanced-specializations.md)|
|Kompetensstatusen uppfylls inte eller har upphört att gälla|Yes|Visa kompetensstatusen på [Kompetenser.](https://partner.microsoft.com/pcv/partnership/competencies) Visa nödvändiga kompetenser för ditt engagemang på [Incentives Engagements](https://partner.microsoft.com/dashboard/incentives/engagements/ux)|
|MPA-avtalet har upphört att gälla eller har inte signerats|Yes|Verifiera och signera MPA-avtal enligt vägledning om [Microsoft-partneravtal för CSP-programpartner](microsoft-partner-agreement.md)|
|Berättigande till säljmedförsäljning har upphört att gälla eller har inte upprättats|Yes|Mer [information finns i Översikt över säljteam och partners i Microsoft](/azure/marketplace/co-sell-overview)|
|Partnerplats är inte berättigad till incitament|No|Partnern kan inte bli berättigad igen av en princip|
|MPN-ID:t är inte berättigat att delta i engagemanget|No|Partnern kan inte bli berättigad igen av en princip|

### <a name="ineligible-transaction"></a>Icke-justerad transaktion

|Orsak till ineligibility|Partneråtgärd krävs?|Så här blir du berättigad igen|
|---------|---------|---------|
|Körningsbeviset godkänns inte|Ja, om du inte har svarat på ett E-postmeddelande med DPOR (Digital Partner of Record) som krävs (POE) från Microsoft|Bevis på körningsbegäran gäller endast för offentlig sektor eller DPOR. Från och med den 1 oktober 2021 är DPOR inte längre incentiviserat för Azure, så POE-begäranden skickas inte.<br><br>Om du har svarat på ett e-postmeddelande med ämnet "Proof of execution required" (Bevis på körning krävs) och svaret avvisades kan du inte bli berättigad igen.|

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
- På sidan [Utbetalningsutdrag](payout-statement.md) kan du få en översikt över dina utbetalningserbjudanden från erbjudanden som säljs via den kommersiella marknadsplatsen.
