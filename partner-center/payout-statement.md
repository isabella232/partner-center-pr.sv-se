---
title: Utbetalningsinstruktioner
description: Lär dig mer om utbetalnings instruktioner och sammanfattningar och hur du visar och exporterar dina betalnings data från Microsoft Partner Center
ms.subservice: partnercenter-marketplace-publisher
ms.service: marketplace
ms.topic: article
author: eunjkim520
ms.author: eunjkim
ms.date: 10/29/2020
ms.openlocfilehash: 4a511dc026e3c71f05c5b18ca6d8915bd2654826
ms.sourcegitcommit: bff907bdbddc769716c7418a2b4a94ca37c2d590
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/03/2021
ms.locfileid: "101756174"
---
# <a name="payout-statements"></a>Utbetalningsinstruktioner

**Lämpliga roller:**

- Kontoadministratör
- Global administratör

**Utbetalnings instruktionen** visar en översikt över dina utbetalningar från erbjudanden som säljs via den kommersiella marknads platsen. Den visar transaktions historik för dina intäkter, uppskattar nästa betalning och visar betalnings trender. Du kan också hämta transaktions historik och betalnings uttryck. Den här artikeln förklarar hur du får åtkomst till din utbetalnings instruktion och de olika utbetalnings sidorna och nedladdningarna som är tillgängliga för dig i Partner Center.

>[!NOTE]
>Du ser bara data för MPN-ID: n och program som du är associerad med. Om du vill visa ytterligare data kan du arbeta med konto administratören för behörigheter. 

## <a name="roles-and-permissions"></a>Roller och behörigheter

För att få åtkomst till en utbetalnings instruktion måste du tilldelas rollen **konto ägare** eller **finansiell deltagare** .

| Rapporter/sidor | Kontoägare | Ansvarig | Utvecklare | Företags deltagare | Ekonomi deltagare | Rika marknads föraren |
| --- | --- | --- | --- | --- | --- | --- |
| Anskaffnings rapport (inklusive data i nära real tid) | Kan visa | Kan visa | Ingen åtkomst | Ingen åtkomst | Kan visa | Ingen åtkomst |
| Feedback-rapport/svar | Kan visa och skicka feedback | Kan visa och skicka feedback | Kan visa och skicka feedback | Ingen åtkomst | Ingen åtkomst | Kan visa och skicka feedback |
| Hälso rapport (inklusive data i nära real tid) | Kan visa | Kan visa | Kan visa | Kan visa | Ingen åtkomst | Ingen åtkomst |
| Användnings rapport | Kan visa | Kan visa | Kan visa | Kan visa | Ingen åtkomst | Ingen åtkomst |
| Konto utbetalning | Kan uppdatera | Ingen åtkomst | Ingen åtkomst | Ingen åtkomst | Kan uppdatera | Ingen åtkomst |
| Skatte profil | Kan uppdatera | Ingen åtkomst | Ingen åtkomst | Ingen åtkomst | Kan uppdatera | Ingen åtkomst |
| Utbetalningssammanfattning | Kan visa | Ingen åtkomst | Ingen åtkomst | Ingen åtkomst | Kan visa | Ingen åtkomst |
|

## <a name="access-your-payout-statement"></a>Få åtkomst till din utbetalnings instruktion

Logga in på [partner Center](https://partner.microsoft.com/dashboard/home) och välj utbetalnings ikonen i det övre högra hörnet på skärmen för att få åtkomst till dessa olika sammanfattningar:

- Transaktions historik
- Betalningar
- Exportera data

:::image type="content" source="images/payouts/payout-overview.png" alt-text="Visar utbetalnings ikonen i det övre högra hörnet på Partner Center-portalen":::

Du kan också använda [API: et för partner utbetalning](https://apidocs.microsoft.com/services/partnerpayouts) för att ansluta och hämta utbetalnings transaktion och betalnings data direkt.


## <a name="transaction-history"></a>Transaktions historik

På sidan **transaktions historik** visas en översikt över dina intäkter, uppskattad nästa betalning och din prenumeration på intäkter och betalningar under de senaste 36 månaderna. Du kan också hämta transaktions information från det här avsnittet.


:::image type="content" source="images/payouts/transaction-overview.png" alt-text="Transaktions översikt.":::

- **Intäkter som skickats detta år** – totala intäkter och nedbrytning av intäkter som har betalats och som kommer att betalas under den kommande månaden.
- **Beräknad betalnings månad** – totala förväntade intäkter under kommande månader.
- **Vinst-och betalnings trend** – månatliga och betalnings belopp för de senaste 36 månaderna.
- **Hämta** – Hämta transaktions information i CSV-eller TSV-format.

Använd datum intervall markeringen i det övre högra hörnet på sidan för att filtrera utdata från sidan för att visa de senaste 3, 6, 12 eller 36 månaderna. Eller Välj ett anpassat datum intervall upp till 36 månader. Standard datum intervallet är 12 månader. Du kan också filtrera efter registrerings-ID, program, betalnings-ID, typ, spaken och status. Data är tillgängliga för innevarande räkenskapsår (1 juli 30 juni) och de föregående två räkenskapsåren.

:::image type="content" source="images/payouts/search-filter.png" alt-text="Sök filtret längst upp till höger på sidan.":::

Om du vill se mer information om ett som du väljer väljer du nedåtpilen till höger på sidan. På så sätt visas spaken, intäkts belopp, produkter och kund. Om någon av dessa data inte är tillgänglig, men du behöver åtkomst till den, kan du kontakta supporten. Om resultatet är resultatet av en justering, och inte en transaktion, kommer fälten produkt och kund inte att visas.

### <a name="transaction-history-summary"></a>Sammanfattning av transaktions historik

Detta visar information, inklusive ursprunget för att betala från produktens sålda datum, status och beräknad betalnings månad.

:::image type="content" source="images/payouts/transaction-history.png" alt-text="Transaktions historik.":::

- **Upparbetat datum** – datum för köpet.
- **Typ** av erbjudande – typ av erbjudande, till exempel Sälj, rabatt eller co-op.
- **Total belopp** – netto beloppet. På den kommersiella marknads platsen innebär det att du har dragit av standard Marketplace-avgiften.
- **Status** – har tre alternativ:
    - **Kommande** – intäkter är i väntande kylnings period.
    - **Bearbetad** – intäkter förbereds för nästa betalning.
    - **Skickat** – intäkterna har betalats.
- **Beräknad betalnings månad** – månaden då intäkterna förväntas betalas. Mer information finns i [Nästa avsnitt](#estimated-payment-month) .

Tjänande transaktioner visas när transaktionen uppfyller utbetalnings berättigande. För att förstå varför du kan sakna eller oväntade intäkter, se [vanliga frågor om utbetalningar på kommersiella platser](payout-faq.md#why-are-my-earnings-missing).

#### <a name="estimated-payment-month"></a>Beräknad betalnings månad

Sidan transaktions historik innehåller nu en tabell som visar de uppskattade betalnings beloppen för de kommande månaderna. Du kan också visa och hämta informationen i exporten av transaktions historik och sammanfattnings rapporter. Den här informationen gör avstämningar och betalnings projekt enklare.

Den uppskattade betalnings månaden beräknas utifrån program konfigurations regler och tids linjer och bearbetas i nästa/kommande betalnings cykel.

Den uppskattade betalnings månaden är för närvarande tillgänglig för alla typer av typer förutom samop, som visas som **ej tillämpligt**. Den uppskattade betalnings månaden visas som **ej tillgänglig** för intäkter före den 1 juli 2020.

I följande tabell visas ett exempel på en uppskattad betalnings månad.

| Månad | Amount |
| ------ | :-----------: |
|  Sep-2020 |  $7 273,99   |
|  Okt-2020 | $8 692,30  |
|  Nov-2020 | $107,89  |

Det beräknade beloppet kan variera från den faktiska mängden av olika orsaker:

- Tilldelad omberäkning: om intäkter beräknas om, kommer den faktiska mängden att vara olika
- Justeringar: den faktiska mängden varierar beroende på justeringar som har inträffat eller skickats.
- Regel ändring: en ändring i reglerna kan återspegla omberäkningen av faktiskt betalt belopp
- Debiterad: om betalnings fel inträffar kan den faktiska mängden vara olika

Observera att din betalning endast lanseras under den beräknade månaden om programmets tröskel och regler för betalnings kvalifikationer är uppfyllda. Dessa regler inkluderar, men är inte begränsade till listan nedan:

- Din skatte profil måste vara aktuell
- Dina intäkter måste uppfylla eller överskrida det lägsta gräns värde som definierats i din program guide.
- Utbetalning väntar: om du väljer alternativet "Behåll min betalning" på sidan profil tilldelning.
- Utbetalnings instrument inte tillgängligt: betalnings-eller/och skatte profil har inte slutförts.

### <a name="transaction-history-download"></a>Hämtning av transaktions historik

Om du vill se mer information om ett sådant väljer du **Ladda ned** överst på sidan. I följande tabell beskrivs varje kolumn i rapporten.

>[!NOTE]
>Exporten av transaktions historiken har två nya fält från augusti 2020:
>
>- **lastPaymentCurrency**  Den valuta i vilken den senaste betalningen togs emot, över alla MPNs som partnern som för tillfället är inloggad med har åtkomst. Om ingen betalning tas emot kommer den sista betalnings valutan att vara US-dollar.
>- **earningAmountInLastPaymentCurrency**  Det totala antalet i den senaste betalnings valutan.

| Kolumnnamn | Description | Tillämplighet för stimulans program/marknads platser |
| --- | --- | --- |
| agreementEndDate | Datum för avtals slutdatum | Incitament – endast vissa program |
| agreementNumber | Avtals nummer | Incitament – endast vissa program |
| agreementStartDate | Avtalets start datum | Incitament – endast vissa program |
| calculationDate | Datum då intjänaren beräknades i systemet | Alla |
| claimId | Unikt ID för anspråk | Incitament – endast vissa program |
| customerCountry | Kund land/-region | marknads platser |
| customerEmail |  |  |
| customerName | Kan vara tomt | Incitaments program (undantag: OEM) och marknads platser. För CSP-transaktioner visar Marketplace namnet på KRYPTOGRAFIPROVIDERn |
| customerTenantId |  |  |
| distributorId | Distributions-ID | Incitament – endast vissa program |
| distributorName | Namn på distributör | Incitament – endast vissa program |
| earningAmount | Tjänande belopp i den ursprungliga transaktions valutan | Alla |
| earningAmountInLastPaymentCurrency | Detta belopp i den senaste betalnings valutan (fältet är tomt om inga tidigare betalningar har betalats) |  |
| earningAmountUSD | Tjäna belopp i USD | Alla |
| earningDate | Datum för den tjänande | Alla |
| earningExchangeRate | Växelkurs som används för att visa motsvarande USD-belopp | Alla |
| earningId | Unikt ID för varje tilltjänande | Alla |
| earningRate | Incitaments satser som tillämpas på transaktions belopp för att generera en tjänande | Alla |
| earningType | Anger om det är avgift, rabatt, samop, Sälj, och så vidare | Alla |
| exchangeRateDate | Valutakurs datum som används för att beräkna EarningAmount USD | Alla |
| externalReferenceId | Unikt ID för programmet | Direkta löne program (incitament och marknads platser) |
| externalReferenceIdLabel | Etikett för unikt ID | Direkta löne program (incitament och marknads platser) |
| instantRebateAmount |  |  |
| invoiceDate |  |  |
| invoiceNumber | Faktura nummer (gäller endast för företag) | Incitament och marknads platser – vissa program är bara |
| lastPaymentCurrency | Senaste betalnings valuta (fältet är tomt om ingen tidigare betalning har betalats) |  |
| handtag | Indikerar affärs regel för att tjäna | Alla |
| LicensingProgramName | Namn på licensierings programmet |  |
| LineItemId | Enskild rad i en kunds faktura |  |
| localProviderSeller | Lokal leverantör/säljare i post |  |
| Förfallo månad | Beräknad betalnings månad | Alla |
| OrderId | Avser en kund faktura  | marknads platser |
| parentProductId | Unikt ID för överordnad produkt. Om det inte finns någon överordnad produkt för transaktionen, så överordnad produkt-ID = produkt-ID. | marknads platser |
| parentProductName | Namnet på den överordnade produkten. Om det inte finns någon överordnad produkt för transaktionen får du ett överordnat produkt namn = produkt namn. | marknads platser |
| participantId | Den primära identiteten för partnern enligt programmet | Alla |
| participantIdType | De flesta program-ID: n för stimulans program och näringsidkare om för marknads platser | Alla |
| participantName | Partnerns namn | Alla |
| partnerCountryCode | Plats/land/region för partnern | Alla |
| partNumber | Är alltid tomt | Vissa stimulans program och marknads platser |
| paymentId | Unikt ID för betalningen. Det här numret visas vanligt vis i ditt konto utdrag | Endast SAP-betalningar |
| paymentStatus | Betalningstatus | Alla |
| paymentStatusDescription | Egen beskrivning av betalnings status | Alla |
| productId | Unikt produkt-ID | marknads platser |
| Namn | Produkt namn som är kopplat till transaktionen | Alla |
| productType | Typ av produkt, till exempel app, tillägg eller spel | marknads platser |
| Program kod | Sträng som ska mappas med program namnet |  |
| programName | Namn på incitament/Store-program | Alla |
| purchaseOrderCoverageEndDate | Är alltid tomt | Incitaments program – CRI |
| purchaseOrderCoverageStartDate | Är alltid tomt | Incitaments program – CRI |
| purchaseOrderType | Är alltid tomt | Incitaments program – CRI |
| purchaseTypeCode | Är alltid tomt | Incitaments program – CRI |
| quantity | Varierar beroende på program. Anger Fakturerat antal för transaktions program | Alla |
| reasonCode |  |  |
| resellerCountry |  |  |
| resellerId | Åter försäljarens ID | Incitament – endast vissa program |
| resellerName | Återförsäljarens namn |  |
| SkuId | SKU-ID som definieras under publiceringen. Ett erbjudande kan ha många SKU: er, men en SKU kan bara associeras med ett enda erbjudande. Incitament – endast vissa program |  |
| storeFee | Det belopp som Microsoft har bevarat som en avgift för att göra appen eller tillägget tillgängligt i butiken | marknads platser |
| subscriptionEndDate | Slutdatum för prenumeration | Incitament – endast vissa program |
| subscriptionId | Prenumerations-ID som är associerad med kunden | Incitament – endast vissa program |
| subscriptionStartDate | Start datum för prenumeration | Incitament – endast vissa program |
| taxCity |  |  |
| taxCountry |  |  |
| taxRemitModel | Part som ansvarar för att remittera skatter (försäljning, användning eller moms/GST-skatter) | marknads platser |
| taxRemitted | Moms omremitterad (försäljning, användning eller moms/GST-moms) | marknads platser |
| taxState | Kundens tillstånd |  |
| taxZipCode | Kundens post nummer |  |
| tpan | Anger AD-nätverk från tredje part | endast Marketplace-annonser |
| transactionAmount | Transaktions belopp i den ursprungliga transaktions valutan baserat på vilken du genererar | Alla |
| transactionAmountUSD | Transaktions belopp i USD | Alla |
| transactionCountryCode | Lands nummer/region kod som transaktionen skedde i |  |
| transactionCurrency | Valutan i vilken den ursprungliga kund transaktionen inträffade (detta är inte en partner plats valuta) | Alla |
| transactionDate | Datum för transaktionen. Användbart för program där många transaktioner bidrar till en | Alla |
| transactionExchangeRate | Valutakurs datum som används för att visa motsvarande transaktions USD-belopp | Alla |
| transactionId | Unikt ID för transaktionen | Alla |
| transactionPaymentMethod | Kund betalnings instrument som används för transaktionen, till exempel kort, fakturering av mobil företag eller PayPal | marknads platser |
| transactionType | Transaktions typ, till exempel köp, åter betalning, återföring eller åter betalning | marknads platser |
| workload | Arbetsbelastning | Incitament – endast vissa program |
|

### <a name="transaction-adjustment-codes"></a>Transaktions justerings koder

I följande tabell visas orsaks koder för justeringar och deras beskrivningar.

|**Orsaks kod**   |**Beskrivning**   |
|------------------|:-------------------------------------|
| Efterlevnad av P.A. | Justering som minskar intäkterna när Microsoft-fakturor inte betalas i tid av partnern. |
| Ko-förnyelse | Justering som överför samförsäljnings intäkter till en annan period eller omvandlar samsiga intäkter till rabatter. |
| OPS-justering | Justering som korrigerar Microsofts system beräknings fel. |
| OPS-justering Microsoft felaktig calc | Justering som korrigerar fel beräkningar. |
| OPS-justering Microsoft felaktig registrering | Justering för registrering av relaterade felberäkningar. |
| Partner mappning (prenumeration) MCI/CSP | Justering som korrigerar felaktig justering av prenumeration. |
| Princip undantag | Justering som åsidosätter en program regel.  |
| Föregående period vinst | Justering för intäkter utanför den aktuella perioden. |

## <a name="payments"></a>Betalningar

På sidan **betalningar** finns information om de pengar du har fått med Microsoft. Det visar även när och hur mycket du kommer att betala.

>[!Note]
> För att bli berättigad till utbetalning måste du ha uppnått [betalnings tröskeln](payment-thresholds-methods-timeframes.md) på $50. Mer information finns i [Microsoft Publisher-avtalet](https://go.microsoft.com/fwlink/?LinkID=699560).

:::image type="content" source="images/payouts/payments-overview.png" alt-text="Översikt över betalningar.":::

- **Totalt betalat det här året** – den sammanlagda summan betalas ut till dig detta år, i amerikanska dollar, för alla dina program.
- **Nästa beräknade betalning** – den enda nästa betalning som kommer till dig (även om andra kommer snart) i amerikanska dollar.
- **Senaste betalning** – summan (i USD), program namn och program för din senaste betalning.
- **Betalning per källa – betalnings** belopp (i USD), per program, under de senaste 12 månaderna.

### <a name="payments-list"></a>Betalnings lista

**Listan över betalnings** tabeller visar betalda och väntande betalningar. Du kan hämta skatte information om service avgiften i PDF-format och Visa mer information om en specifik betalning.

:::image type="content" source="images/payouts/list-of-payments.png" alt-text="Exportera transaktions historik":::

- **Betald** – alla betalningar har skickats. Välj året i den nedrullningsbara menyn för att filtrera fram de betalningar som publicerats under det året.
- **Väntande** – kommande betalningar.
- **Service avgifts skatt (PDF-formulär)** – tillgängligt för betalningar som omfattas av service avgifts skatt. Avgifter för service avgift visas i **andra skatter**.
- **Visa** – omdirigerar till transaktions historiken med en lista över intäkter som ingår i betalningen.

För att förstå varför du kan sakna eller oväntade intäkter, se [vanliga frågor om utbetalningar på kommersiella platser](payout-faq.md#why-are-my-earnings-missing).

### <a name="payment-status"></a>Betalningstatus

I följande tabell förklaras de olika ställnings statusarna.

| Status för att tjäna | Anledning | Krävs partner åtgärd? |
| --- | --- | --- |
| Obearbetade | Betalningen är berättigad till betalning. Den förblir i det här läget för en kylnings period som definieras i program guiden för stimulans programmet. | Inga |
| Planer | Betalnings order som genererats som väntande interna granskningar innan betalningen bearbetas. | Inga |
| Väntande moms faktura | Din moms faktura är ofullständig eller ogiltig. | Du måste uppdatera din moms faktura innan du kan betala |
| Avvisad under granskning | Betalningen avvisades under granskningen. | Kontakta Microsoft support om du vill ha mer information |
| Misslyckad | Betalningen misslyckades på grund av ett fel i Microsoft-systemet. | Kontakta Microsoft support om du vill ha mer information |
| Pågår | Betalningen pågår. | Inga |
| Felaktig betalning | Betalnings återkoppling pågår. | Inga |
| Skickat | Betalningen har skickats till din bank. | Inga |
| Ombearbetning | Ett Microsoft-systemfel påträffades under betalningen och ombearbetas. | Inga |
| Reversed | Betalningen återfördes av banken och skickas igen vid nästa betalnings cykel. | Inga |
| Avvisad moms faktura | Din moms faktura avvisades under granskningen. Alla väntande betalningar stoppas tills moms granskningen är klar. | Kontakta Microsoft support om du vill ha mer information |
| Moms faktura under granskning | Din moms faktura granskas. Din betalning frigörs när moms fakturan har godkänts. | Inga |
| Avslagen | Betalningen avvisades av din bank. | Kontakta din bank om du vill ha mer information. |
|

### <a name="payments-download"></a>Hämtning av betalningar

 I följande tabell beskrivs varje kolumn i rapporten. Om du vill se mer information om dina betalningar väljer du **Hämta** överst på sidan betalningar.

| Kolumnnamn | Description |
| --- | --- |
| participantID | Den primära identiteten för partnern enligt programmet |
| participantIDType | Normalt program-ID för stimulans program och säljar-ID för Store-program |
| participantName | Partnerns namn |
| programName | Namn på incitament/Store-program |
| tjänade | Belopp som erhållits i betala till valuta för programmet/participantID |
| earnedUSD | Belopp som erhållits för program-/deltagar-ID i USD |
| withheldTax | Skatte belopp i betalningen till valuta för programmet/participantID |
| Moms | Total moms belopp i fältet betala till valuta för programmet/participantID (gäller endast incitaments program) |
| serviceFeeTax | Total mängd serviceFeeTax i betalning till valuta för programmet/participantID (gäller endast för Store-program och Azure Marketplace) |
| totalPayment | Total betalning i lokal valuta exklusive käll skatt och inklusive moms (om tillämpligt) för programmet/participantID |
| currencyCode | Betala till valuta kod |
| paymentMethod | Den metod som används för att betala partnern, till exempel elektronisk bank överföring, kredit anteckning |
| paymentID | Unikt ID för betalningen. Det här numret visas vanligt vis i ditt konto utdrag (gäller endast för SAP-betalningar). |
| paymentStatus | Betalningstatus |
| paymentStatusDescription | Egen beskrivning av betalnings status |
| paymentDate | Datum betalning skickades från Microsoft |
|

## <a name="export-data"></a>Exportera data

Sidan **Exportera data** uppdateras inte på egen hand. Du kan behöva uppdatera sidan manuellt för att se de senaste data. Välj från de tre flikarna för att exportera antingen **transaktions historik**, **betalningar**, **transaktions Sammanfattning** eller **historisk instruktion**.

Filtret kan resultera i att det **inte finns några tillgängliga data** fel. Detta kan inträffa om du har lämnat standard tids perioden som valts vid tre månader och sedan valt ett betalnings-ID från ett som ligger utanför den perioden. Om detta inträffar expanderar du din tids period och försöker igen.

Här är ett exempel på betalnings export:

:::image type="content" source="images/payouts/pc-export-payments.png" alt-text="Exportera betalnings rapport.":::

### <a name="historical-statements"></a>Historiska instruktioner

Sammanfattningen av **export data** ger även åtkomst till historiska instruktioner.

> [!NOTE]
> En historisk instruktion är en ögonblicks bild och uppdateras inte. Kontakta [supporten](https://partner.microsoft.com/support/v2/?stage=1) och begär den senaste informationen om det behövs.

:::image type="content" source="images/payouts/pc-export-statements.png" alt-text="Exportera historiska instruktioner.":::

- Transaktions historik från före den 1 juli 2019 hanteras separat och använder olika fält från senare historik rapporter.
- Tidigare transaktions historik har en kolumn med namnet "reserverad" som motsvarar kolumnen "intäkter" i den moderna historiken, förutom att den utesluter alla intäkter med status lika med "betalning har skickats".
- Filter som 3M, 6 M eller 12M kommer inte att gälla för avsnittet historiska instruktioner.

### <a name="historical-statement-downloads"></a>Hämtning av historiska instruktioner

I följande tabell beskrivs varje kolumn i en historisk instruktion.

| Fältnamn | Beskrivning |
| --- | --- |
| Intäkts källa | Källan till intäkterna baserat på var transaktionen ägde rum, till exempel Microsoft Store, Windows Phone butik, Windows Store 8 eller annonsering |
| Order-ID | Unikt order-ID. Med det här ID: t kan du identifiera inköps transaktioner med deras respektive icke-inköps transaktioner, till exempel åter betalningar eller åter betalningar. Båda kommer att ha samma order-ID. Om det finns en aktie avgift där flera betalnings metoder användes för ett enda köp kan du länka inköps transaktionerna. |
| Transaktions-ID | Unikt transaktions-ID. |
| Transaktions datum tid | Datum och tid då transaktionen inträffade (UTC). |
| ID för överordnad produkt | Unikt ID för överordnad produkt. Om det inte finns någon överordnad produkt för transaktionen, så överordnad produkt-ID = produkt-ID. |
| Produkt-ID | Unikt produkt-ID. |
| Namn på överordnad produkt | Namnet på den överordnade produkten. Om det inte finns någon överordnad produkt för transaktionen får du ett överordnat produkt namn = produkt namn. |
| Produktnamn | Produktens namn |
| Produkttyp | Typ av produkt, till exempel app, tillägg eller spel |
| Kvantitet | När intäkts källan är Microsoft Store för företag, representerar kvantiteten antalet licenser som har köpts. För alla andra intäkts källor är antalet alltid 1. Även om en enskild transaktion delas upp i två rad objekt eftersom två olika betalnings metoder användes, visar varje rad objekt en kvantitet på 1. |
| Transaktionstyp | Transaktions typ, till exempel köp, åter betalning, återföring eller åter betalning |
| Betalnings metod | Kund betalnings instrument som används för transaktionen, till exempel kort, fakturering av mobil företag eller PayPal |
| Land/region | Land/region där transaktionen ägde rum |
| Lokal leverantör/säljare | Lokal leverantör/säljare i post |
| Transaktions valuta | Transaktions valuta |
| Transaktions belopp | Transaktions belopp |
| Skatte mottagare | Moms omremitterad (försäljning, användning eller moms/GST-moms) |
| Netto kvitton | Transaktions belopp exklusive skatte mottagare |
| Butiks avgift | Procent andelen av netto inleveranser som har behållits av Microsoft som en avgift för att göra appen eller tillägget tillgängligt i butiken |
| Appen fortsätter | Netto inleveranser minus butiks avgiften |
| Kvarhållna skatter | **Förbehållen** inkomst skatt (del ingår i den reserverade CSV-filen) |
| Payment | Appen fortsätter minus eventuell tillämplig inkomst skatts katt (belopp som visas i transaktions valutan). Ingår inte i **reserverad** CSV-fil. |
| FX-pris | Utländsk växelkurs som används för att omvandla transaktions valutan till betalnings valutan |
| Betalningsvaluta | Valutan som din betalning görs i |
| Konverterad betalning | Betalnings belopp konverterat till betalnings valuta med hjälp av FX-pris |
| Moms remitterad modell | Part som ansvarar för att remittera skatter (försäljning, användning eller moms/GST-skatter) |
| Datum och tid för berättigande | Datum och tid när transaktions fortsätter blir berättigade till utbetalning (UTC). När en utbetalning skapas, inkluderar den transaktions Fortsätt med en giltighets tid innan datumet för utbetalning skapas (endast inkluderad i den **reserverade** CSV-filen). |
| Avgifter | Visar en analys av all avgifts information som sammanställs i kolumnen transaktions belopp (ingår endast för Azure Marketplace, ingår inte i den **reserverade** CSV-filen). |
|||

## <a name="next-steps"></a>Nästa steg

- [Partnerns utbetalnings-API](https://apidocs.microsoft.com/services/partnerpayouts)
- [Information om utbetalningsprincip](payout-policy-details.md)
- Kontakta [supporten för stöd för Microsoft](https://partner.microsoft.com/support/v2/?stage=1)Marketplace för fakturerings support.
