---
title: Utbetalnings instruktion för den kommersiella marknads platsen i Partner Center
description: Lär dig mer om utbetalnings instruktioner och sammanfattningar och hur du visar och exporterar dina betalnings data för den kommersiella Marketplace
ms.subservice: partnercenter-marketplace-publisher
ms.service: marketplace
ms.topic: article
author: mingshen-ms
ms.author: mingshen
ms.date: 09/23/2020
ms.openlocfilehash: 460a7b1992d7db40e0f45d3aeb7e2236e9495e07
ms.sourcegitcommit: a84812b650ec8b6d0513c46c04840e4bbb0c8460
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/25/2020
ms.locfileid: "92531772"
---
# <a name="payout-statements"></a>Utbetalningsinstruktioner

**Utbetalnings instruktionen** visar en översikt över dina utbetalningar från erbjudanden som säljs via den kommersiella marknads platsen. Den visar transaktions historik för dina intäkter, uppskattar nästa betalning och visar betalnings trender. Du kan också hämta transaktions historik och betalnings uttryck. Den här artikeln förklarar hur du får åtkomst till din utbetalnings instruktion och de olika utbetalnings sidorna och nedladdningarna som är tillgängliga för dig i Partner Center.

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

:::image type="content" source="images/payouts/transaction-overview.png" alt-text="Visar utbetalnings ikonen i det övre högra hörnet på Partner Center-portalen":::

- **Intäkter som skickats detta år** – totala intäkter och nedbrytning av intäkter som har betalats och som kommer att betalas under den kommande månaden.
- **Beräknad betalnings månad** – totala förväntade intäkter under kommande månader.
- **Vinst-och betalnings trend** – månatliga och betalnings belopp för de senaste 36 månaderna.
- **Hämta** – Hämta transaktions information i CSV-eller TSV-format.

Använd datum intervall markeringen i det övre högra hörnet på sidan för att filtrera utdata från sidan för att visa de senaste 3, 6, 12 eller 36 månaderna. Eller Välj ett anpassat datum intervall upp till 36 månader. Standard datum intervallet är 12 månader.

:::image type="content" source="images/payouts/search-filter.png" alt-text="Visar utbetalnings ikonen i det övre högra hörnet på Partner Center-portalen":::

### <a name="transaction-history-summary"></a>Sammanfattning av transaktions historik

Detta visar information, inklusive ursprunget för att betala från produktens sålda datum, status och beräknad betalnings månad.

:::image type="content" source="images/payouts/transaction-history.png" alt-text="Visar utbetalnings ikonen i det övre högra hörnet på Partner Center-portalen":::

- **Upparbetat datum** – datum för köpet.
- **Typ** av erbjudande – typ av erbjudande, till exempel Sälj, rabatt eller co-op.
- **Total belopp** – netto beloppet. På den kommersiella marknads platsen innebär det att du har dragit av standard Marketplace-avgiften.
- **Status** – har tre alternativ:
    - **Kommande** – intäkter är i väntande kylnings period.
    - **Bearbetad** – intäkter förbereds för nästa betalning.
    - **Skickat** – intäkterna har betalats.
- **Beräknad betalnings månad** – månaden då intäkterna förväntas betalas.

Tjänande transaktioner visas när transaktionen uppfyller utbetalnings berättigande. För att förstå varför du kan sakna eller oväntade intäkter, se [vanliga frågor om utbetalningar på kommersiella platser](payout-faq.md#why-are-my-earnings-missing).

### <a name="transaction-history-download"></a>Hämtning av transaktions historik

Om du vill se mer information om ett sådant väljer du **Ladda ned** överst på sidan. I följande tabell beskrivs varje kolumn i rapporten.

| Kolumnnamn | Description | Tillämplighet för stimulans program/marknads platser |
| --- | --- | --- |
| agreementEndDate | Datum för avtals slutdatum | Incitament – endast vissa program |
| agreementNumber | Avtals nummer | Incitament – endast vissa program |
| agreementStartDate | Avtalets start datum | Incitament – endast vissa program |
| calculationDate | Datum då intjänaren beräknades i systemet | Alla |
| claimId | Unikt ID för anspråk | Incitament – endast vissa program |
| customerCountry | Kund land/-region | marknads platser |
| customerEmail |  |  |
| customerName | Är alltid tomt | Incitaments program (undantag: OEM) och marknads platser |
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

## <a name="payments"></a>Betalningar

På sidan **betalningar** finns information om de pengar du har fått med Microsoft. Det visar även när och hur mycket du kommer att betala.

>[!Note]
> För att bli berättigad till utbetalning måste du ha uppnått [betalnings tröskeln](payment-thresholds-methods-timeframes.md) på $50. Mer information finns i [Microsoft Publisher-avtalet](https://go.microsoft.com/fwlink/?LinkID=699560).

:::image type="content" source="images/payouts/payments-overview.png" alt-text="Visar utbetalnings ikonen i det övre högra hörnet på Partner Center-portalen":::

- **Totalt betalat det här året** – den sammanlagda summan betalas ut till dig detta år, i amerikanska dollar, för alla dina program.
- **Nästa beräknade betalning** – den enda nästa betalning som kommer till dig (även om andra kommer snart) i amerikanska dollar.
- **Senaste betalning** – summan (i USD), program namn och program för din senaste betalning.
- **Betalning per källa – betalnings** belopp (i USD), per program, under de senaste 12 månaderna.

### <a name="payments-list"></a>Betalnings lista

**Listan över betalnings** tabeller visar betalda och väntande betalningar. Du kan hämta skatte information om service avgiften i PDF-format och Visa mer information om en specifik betalning.

:::image type="content" source="images/payouts/list-of-payments.png" alt-text="Visar utbetalnings ikonen i det övre högra hörnet på Partner Center-portalen":::

- **Betald** – alla betalningar har skickats. Välj året i den nedrullningsbara menyn för att filtrera fram de betalningar som publicerats under det året.
- **Väntande** – kommande betalningar.
- **Service avgifts skatt (PDF-formulär)** – tillgängligt för betalningar som omfattas av service avgifts skatt. Avgifter för service avgift visas i **andra skatter** .
- **Visa** – omdirigerar till transaktions historiken med en lista över intäkter som ingår i betalningen.

För att förstå varför du kan sakna eller oväntade intäkter, se [vanliga frågor om utbetalningar på kommersiella platser](payout-faq.md#why-are-my-earnings-missing).

### <a name="payment-status"></a>Betalningstatus

I följande tabell förklaras de olika ställnings statusarna.

| Status för att tjäna | Orsak | Krävs partner åtgärd? |
| --- | --- | --- |
| Obearbetade | Betalningen är berättigad till betalning. Den förblir i det här läget för en kylnings period som definieras i program guiden för stimulans programmet. | No |
| Planer | Betalnings order som genererats som väntande interna granskningar innan betalningen bearbetas. | No |
| Väntande moms faktura | Din moms faktura är ofullständig eller ogiltig. | Du måste uppdatera din moms faktura innan du kan betala |
| Avvisad under granskning | Betalningen avvisades under granskningen. | Kontakta Microsoft support om du vill ha mer information |
| Misslyckades | Betalningen misslyckades på grund av ett fel i Microsoft-systemet. | Kontakta Microsoft support om du vill ha mer information |
| Pågår | Betalningen pågår. | No |
| Felaktig betalning | Betalnings återkoppling pågår. | No |
| Skickat | Betalningen har skickats till din bank. | No |
| Ombearbetning | Ett Microsoft-systemfel påträffades under betalningen och ombearbetas. | No |
| Reversed | Betalningen återfördes av banken och skickas igen vid nästa betalnings cykel. | No |
| Avvisad moms faktura | Din moms faktura avvisades under granskningen. Alla väntande betalningar stoppas tills moms granskningen är klar. | Kontakta Microsoft support om du vill ha mer information |
| Moms faktura under granskning | Din moms faktura granskas. Din betalning frigörs när moms fakturan har godkänts. | No |
| Avslagen | Betalningen avvisades av din bank. | Kontakta din bank om du vill ha mer information. |
|

### <a name="payments-download"></a>Hämtning av betalningar

Om du vill se mer information om dina betalningar väljer du **Hämta** överst på sidan. I följande tabell beskrivs varje kolumn i rapporten.

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

Sidan **Exportera data** uppdateras inte på egen hand. Du kan behöva uppdatera sidan manuellt för att se de senaste data. Välj från de tre flikarna för att exportera antingen **transaktions historik** , **betalningar** , **transaktions Sammanfattning** eller **historisk instruktion** .

Filtret kan resultera i att det **inte finns några tillgängliga data** fel. Detta kan inträffa om du har lämnat standard tids perioden som valts vid tre månader och sedan valt ett betalnings-ID från ett som ligger utanför den perioden. Om detta inträffar expanderar du din tids period och försöker igen.

Här är ett exempel på betalnings export:

:::image type="content" source="images/payouts/pc-export-payments.png" alt-text="Visar utbetalnings ikonen i det övre högra hörnet på Partner Center-portalen":::

### <a name="historical-statements"></a>Historiska instruktioner

Sammanfattningen av **export data** ger även åtkomst till historiska instruktioner.

> [!NOTE]
> En historisk instruktion är en ögonblicks bild och uppdateras inte. Kontakta [supporten](https://partner.microsoft.com/support/v2/?stage=1) och begär den senaste informationen om det behövs.

:::image type="content" source="images/payouts/pc-export-statements.png" alt-text="Visar utbetalnings ikonen i det övre högra hörnet på Partner Center-portalen" i den moderna historiken, förutom att den utesluter alla intäkter med status lika med "betalning har skickats".
- Filter som 3M, 6 M eller 12M kommer inte att gälla för avsnittet historiska instruktioner.

### <a name="historical-statement-downloads"></a>Hämtning av historiska instruktioner

I följande tabell beskrivs varje kolumn i en historisk instruktion.

| Fältnamn | Description |
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