---
title: Utbetalningsinstruktioner
description: Lär dig mer om utbetalningsutdrag och sammanfattningar och hur du visar och exporterar dina betalningsdata från Microsoft Partner Center
ms.subservice: partnercenter-payouts
ms.service: partner-dashboard
ms.topic: article
author: eunjkim520
ms.author: eunjkim
ms.date: 09/27/2021
ms.openlocfilehash: fbc3b659bbb3dded386dfa970d815b27de48ebd5
ms.sourcegitcommit: cf8c78e0c8831371432007d5ab05f934f15a77b5
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 10/05/2021
ms.locfileid: "129525320"
---
# <a name="payout-statements"></a>Utbetalningsinstruktioner

**Lämpliga roller:** Kontoadministratörsroller | Global administratör

**Utbetalningsutdraget** ger en översikt över dina utbetalningserbjudanden från erbjudanden som säljs via den kommersiella marknadsplatsen. Den visar transaktionshistorik för dina intäkter, beräknar nästa betalning och visar betalningstrender. Du kan också ladda ned transaktionshistorik och betalningsutdrag. Den här artikeln förklarar hur du kommer åt ditt utbetalningsutdrag och de olika utbetalningssidorna och nedladdningarna som är tillgängliga för dig i Partnercenter.

> [!NOTE]
> Du ser bara data för MPN-ID:er och program som du är associerad med. Om du vill se ytterligare data kan du kontakta kontoadministratören för att få behörighet. 

## <a name="roles-and-permissions"></a>Roller och behörigheter

För att få åtkomst till ett utbetalningsutdrag måste du ha **tilldelats rollen Kontoägare** **eller Finansiell** deltagare.

| Rapporter/sidor | Kontoägare | Ansvarig | Utvecklare | Affärsdeltagare | Ekonomideltagare | Marknadsförare |
| --- | --- | --- | --- | --- | --- | --- |
| Förvärvsrapport (inklusive data i nära realtid) | Kan visa | Kan visa | Ingen åtkomst | Ingen åtkomst | Kan visa | Ingen åtkomst |
| Feedbackrapport/svar | Kan visa och skicka feedback | Kan visa och skicka feedback | Kan visa och skicka feedback | Ingen åtkomst | Ingen åtkomst | Kan visa och skicka feedback |
| Hälsorapport (inklusive data i nära realtid) | Kan visa | Kan visa | Kan visa | Kan visa | Ingen åtkomst | Ingen åtkomst |
| Användningsrapport | Kan visa | Kan visa | Kan visa | Kan visa | Ingen åtkomst | Ingen åtkomst |
| Utbetalningskonto | Kan uppdateras | Ingen åtkomst | Ingen åtkomst | Ingen åtkomst | Kan uppdateras | Ingen åtkomst |
| Skatteprofil | Kan uppdateras | Ingen åtkomst | Ingen åtkomst | Ingen åtkomst | Kan uppdateras | Ingen åtkomst |
| Utbetalningssammanfattning | Kan visa | Ingen åtkomst | Ingen åtkomst | Ingen åtkomst | Kan visa | Ingen åtkomst |
|

## <a name="access-your-payout-statement"></a>Få åtkomst till ditt utbetalningsutdrag

#### <a name="workspaces-view"></a>[Vyn Arbetsytor](#tab/workspaces-view)

1. Logga in på [instrumentpanelen i Partnercenter](https://partner.microsoft.com/dashboard) och välj **panelen** Utbetalning.

2. Välj en av de tillgängliga sammanfattningarna:

    - Betalningsöversikt
    - Transaktionshistorik
    - Exportera data

    :::image type="content" source="./images/payouts/payout-overview-workspaces.png" alt-text="Skärmbild som visar översikten över utbetalningsarbetsytan.":::

#### <a name="current-view"></a>[Aktuell vy](#tab/current-view)

Logga in på [Partnercenter](https://partner.microsoft.com/dashboard/home) och välj utbetalningsikonen i det övre högra hörnet på skärmen för att få åtkomst till dessa olika sammanfattningar:

- Transaktionshistorik
- Betalningar
- Exportera data

:::image type="content" source="images/payouts/payout-overview.png" alt-text="Skärmbild som visar utbetalningsikonen i det övre högra hörnet i Partnercenter-portalen.":::

* * *

Du kan också använda [partnerns utbetalnings-API för](/rest/api/partner-center/partner-payouts) att ansluta och hämta utbetalningstransaktions- och betalningsdata direkt. Läs mer i [Hantera utbetalningar med hjälp av API:et för utbetalningstjänsten](/partner-center/develop/manage-payouts).

## <a name="transaction-history"></a>Transaktionshistorik

Sidan **Transaktionshistorik** visar en sammanfattning av dina intäkter, beräknad nästa betalning samt din trend för intäkter och betalningar under de senaste 36 månaderna. Du kan också ladda ned transaktionsinformation från det här avsnittet.<br><br>Den här rapporten visar alla intäkter som är berättigade till utbetalning, inklusive betalningar som ännu inte har skickats. Intäkter är berättigade till utbetalning när en ISV har slutfört all bank- och skatteinformation i Partnercenter, har tjänade >50 USD, ISV-kontot är aktivt och kunden har fakturerats (för EA-transaktioner) eller om betalningen har tagits emot (för icke-EA-transaktioner).

- **Intäkter som skickats i** år – Totala intäkter och uppdelningar av intäkter som har betalats och kommer att betalas under den kommande månaden.
- **Uppskattad betalningsmånad** – Totala intäkter som förväntas under de kommande månaderna.
- **Intäkts- och betalningstrend** – Månatliga intjänings- och betalningsbelopp för de senaste 36 månaderna.
- **Ladda** ned – Ladda ned transaktionsinformation i .csv- eller .tsv-format.

Använd datumintervallmarkeringen i det övre högra hörnet på sidan för att filtrera utdata för sidan så att de senaste 3, 6, 12 eller 36 månaderna visas. Du kan också välja ett anpassat datumintervall på upp till 36 månader. Standardintervallet för datum är 12 månader. Du kan också filtrera efter Registrerings-ID, Program, Betalnings-ID, Intjäningstyp, Lever och Status. Data är tillgängliga för det aktuella räkenskapsåret (1 juli – 30 juni) och de föregående två räkenskapsåren.

Om du vill se mer information om en intjäning väljer du nedåtpilen till höger på sidan. Om du gör det visas reglaget, intäktsbeloppet, produkten och kunden. Om någon av dessa data av någon anledning inte är tillgänglig, men du behöver åtkomst till den, kontaktar du supporten. Om intjäning är resultatet av en justering och inte en transaktion visas inte fälten Produkt och Kund.

### <a name="transaction-history-summary"></a>Sammanfattning av transaktionshistorik

Den här vyn visar information om intjäning, inklusive ursprunget för intjäning från den sålda produkten, status och beräknad betalningsmånad.

:::image type="content" source="images/payouts/transaction-history.png" alt-text="Transaktionshistorik.":::

- **Intjänat** datum – inköpsdatum.
- **Typ av** intjäning – Typ av intjäning, till exempel Försäljning, Medarbetare eller Co-op.
- **Totalt belopp** – nettointäkterna. På den kommersiella marknadsplatsen innebär det att du har dra av standardavgiften för Marketplace.
- **Status** – Har tre alternativ:
    - **Kommande** – Intäkter är under en väntande kylningsperiod.
    - **Bearbetade** – intäkter förbereds för nästa betalning.
    - **Sent** – Intäkter har betalats.
- **Uppskattad betalningsmånad** – Den månad då intäkterna förväntas betalas. Mer information [finns i](#estimated-payment-month) nästa avsnitt.

Intäktstransaktioner visas när transaktionen uppfyller utbetalningsberättigandet. Information om varför du kan ha saknade eller oväntade intäkter finns i [Vanliga frågor om utbetalning på den kommersiella marknadsplatsen.](payout-faq.yml#why-are-my-earnings-missing-)

#### <a name="estimated-payment-month"></a>Uppskattad betalningsmånad

Sidan Transaktionshistorik innehåller nu en tabell som visar dina beräknade betalningsbelopp för de kommande månaderna. Du kan också visa och ladda ned den här informationen i exporterna av transaktionshistorik och sammanfattningsrapport. Den här informationen gör avstämningar och betalningsprognoser enklare.

Den uppskattade betalningsmånaden beräknas baserat på programmets konfigurationsregler och tidslinjer och bearbetas i nästa/kommande betalningscykel.

Beräknad betalningsmånad är för närvarande tillgänglig för alla intäktstyper utom co-op, som visas som **Ej tillämpligt.** För intäkter före 1 juli 2020 visas den uppskattade betalningsmånaden som **Ej tillgänglig.**

I följande tabell visas ett exempel på beräknad betalningsmånad.

| Månad | Amount |
| ------ | :-----------: |
|  Sep-2020 |  7 273,99 USD   |
|  Oktober 2020 | 8 692,30 USD  |
|  Nov-2020 | 107,89 USD  |

Det uppskattade beloppet kan variera från det faktiska beloppet av flera olika orsaker:

- Omräkning av intäkter: Om intäkterna beräknas om kommer det faktiska beloppet att vara annorlunda
- Justeringar: Det faktiska beloppet varierar beroende på vilka justeringar som har gjorts eller skickats.
- Ändring av regler: En ändring av regler kan återspegla omberäkning i det faktiska betalda beloppet
- Betalbar: Om betalningsfel inträffar kan det faktiska beloppet vara ett annat

Observera att din betalning endast släpps under den projicerade månaden om ditt programs tröskelvärde och regler för betalningsberättigande uppfylls. Dessa regler omfattar men är inte begränsade till listan nedan:

- Din skatteprofil måste vara uppdaterad
- Dina intäkter måste uppfylla eller överskrida den minsta intäktströskel som definierats i programguiden.
- Hållen utbetalning: Om du väljer alternativet "Håll min betalning" på profiltilldelningssidan.
- Utbetalningsinstrumentet är inte tillgängligt: Betalningen eller/och skatteprofilen har inte slutförts.

### <a name="transaction-history-download"></a>Nedladdning av transaktionshistorik

Om du vill se mer information om en intjäning väljer du **Ladda ned**. I följande tabell förklaras varje kolumn i rapporten.

| Kolumnnamn | Description | Tillämplighet för incitamentprogram/marknadsplatser |
| --- | --- | --- |
| agreementEndDate | Avtalets slutdatum | Incitament – endast vissa program |
| agreementNumber | Avtalsnummer | Incitament – endast vissa program |
| agreementStartDate | Avtalets startdatum | Incitament – endast vissa program |
| calculationDate | Datum då intjäning beräknades i systemet | Alla |
| claimId | Unik identifierare för anspråk | Incitament – endast vissa program |
| customerCountry | Kundens land/region | Marknadsplatser |
| customerEmail |  |  |
| customerName | Kan vara tomt | Endast incitamentprogram (undantag: OEM) och marknadsplatser. För CSP-transaktioner visar marknadsplatser namnet på CSP:en |
| customerTenantId |  |  |
| distributorId | Distributörsidentifierare | Incitament – endast vissa program |
| distributorName | Distributörsnamn | Incitament – endast vissa program |
| earningAmount | Intäktsbelopp i den ursprungliga transaktionsvalutan | Alla |
| earningAmountInLastPaymentCurrency | Intäktsbelopp i den senaste betalningsvalutan (fältet är tomt om inga tidigare betalningar har betalats) |  |
| earningAmountUSD | Intäktsbelopp i USD | Alla |
| earningDate | Datum för intjäning | Alla |
| earningExchangeRate | Exchange som används för att visa motsvarande USD-belopp | Alla |
| earningId | Unik identifierare för varje intjäning | Alla |
| earningRate | Incitamentsfrekvens som tillämpas på transaktionsbelopp för att generera intäkter | Alla |
| earningType | Anger om det är avgift, betalning, samarbete, försäljning och så vidare | Alla |
| exchangeRateDate | Exchange som används för att beräkna intjäningbelopp i USD | Alla |
| externalReferenceId | Unik identifierare för programmet | Direkt betalningsprogram (incitament och marknadsplatser) |
| externalReferenceIdLabel | Unik identifieraretikett | Direkt betalningsprogram (incitament och marknadsplatser) |
| instantRebateAmount |  |  |
| invoiceDate |  |  |
| invoiceNumber | Fakturanummer (gäller endast för företag) | Incitament och marknadsplatser – endast vissa program |
| lastPaymentCurrency | Senaste betalningsvaluta (fältet är tomt om ingen tidigare betalning har betalats) |  |
| Spaken | Anger affärsregel för intjäning | Alla |
| LicensingProgramName | Namn på licensprogrammet |  |
| LineItemId | Enskild rad i en kunds faktura |  |
| localProviderSeller | Lokal leverantör/säljare av post |  |
| Förfallomånad | Beräknad betalningsmånad | Alla |
| OrderId | Relaterar till en kunds faktura  | Marknadsplatser |
| parentProductId | Unik överordnad produktidentifierare. Om det inte finns någon överordnad produkt för transaktionen, så är överordnad produkt-ID = Produkt-ID. | Marknadsplatser |
| parentProductName | Namnet på den överordnade produkten. Om det inte finns någon överordnad produkt för transaktionen, så är överordnad produktnamn = produktnamn. | Marknadsplatser |
| participantId | Den primära identiteten för partnern som tjänar under programmet | Alla |
| participantIdType | Huvudsakligen program-ID för incitamentprogram och Seller IF för marknadsplatser | Alla |
| participantName | Namnet på intäktspartnern | Alla |
| partnerCountryCode | Plats/land/region för intäktspartnern | Alla |
| partNumber | Kommer alltid att vara tom | Vissa incitamentprogram och marknadsplatser |
| paymentId | Unik identifierare för att korrelera alla transaktioner i transaktionsrapporten med en specifik betalning i betalningsrapporten | Alla |
| paymentStatus | Betalningstatus | Alla |
| paymentStatusDescription | Användarvänlig beskrivning av betalningsstatus | Alla |
| productId | Unik produktidentifierare | Marknadsplatser |
| Productname | Produktnamn som är länkat till transaktionen | Alla |
| productType | Typ av produkt, till exempel app, tillägg eller spel | Marknadsplatser |
| Programkod | Sträng att mappa med programnamnet |  |
| programName | Namn på incitament/butiksprogram | Alla |
| purchaseOrderCoverageEndDate | Kommer alltid att vara tom | Incitamentprogram – CRI |
| purchaseOrderCoverageStartDate | Kommer alltid att vara tom | Incitamentprogram – CRI |
| purchaseOrderType | Kommer alltid att vara tom | Incitamentprogram – CRI |
| purchaseTypeCode | Kommer alltid att vara tom | Incitamentprogram – CRI |
| quantity | Varierar beroende på program. Anger fakturerad kvantitet för transaktionella program | Alla |
| reasonCode |  |  |
| resellerCountry |  |  |
| resellerId | Återförsäljares identifierare | Incitament – endast vissa program |
| resellerName | Återförsäljarens namn |  |
| SkuId | SKU-ID enligt definitionen under publiceringen. Ett erbjudande kan ha många SKU:er, men en SKU kan bara associeras med ett enda erbjudande. Incitament – endast vissa program |  |
| storeFee | Det belopp som Microsoft behåller som en avgift för att göra appen eller tillägget tillgängligt i Store | Marknadsplatser |
| subscriptionEndDate | Slutdatum för prenumeration | Incitament – endast vissa program |
| subscriptionId | Prenumerations-ID som är associerat med kunden | Incitament – endast vissa program |
| subscriptionStartDate | Startdatum för prenumeration | Incitament – endast vissa program |
| taxCity |  |  |
| taxCountry |  |  |
| taxRemitModel | Part som ansvarar för att överföra skatter (försäljning, användning eller moms/GST-skatter) | Marknadsplatser |
| taxRemitted | Belopp som har efterförts (försäljning, användning eller moms/GST-skatter) | Marknadsplatser |
| taxState | Kundens tillstånd |  |
| taxZipCode | Kundens postnummer |  |
| tpan | Anger ad-nätverket från tredje part | endast marketplaces-annonser |
| transactionAmount | Transaktionsbelopp i den ursprungliga transaktionsvalutan baserat på vilken intjäning som genereras | Alla |
| transactionAmountUSD | Transaktionsbelopp i USD | Alla |
| transactionCountryCode | Lands-/regionskod där transaktionen skedde |  |
| transactionCurrency | Valuta där den ursprungliga kundtransaktionen ägde rum (detta är inte partnerplatsens valuta) | Alla |
| transactionDate | Datum för transaktionen. Användbart för program där många transaktioner bidrar till en intjäning | Alla |
| transactionExchangeRate | Exchange som används för att visa motsvarande transaktionsbelopp i USD | Alla |
| transactionId | Unik identifierare för transaktionen | Alla |
| transactionPaymentMethod | Kundens betalningsmedel som används för transaktionen, till exempel kort, fakturering för mobiloperatör eller PayPal | Marknadsplatser |
| transactionType | Typ av transaktion, till exempel köp, återbetalning, återföring eller återbetalning | Marknadsplatser |
| workload | Arbetsbelastning | Incitament – endast vissa program |
|

### <a name="transaction-adjustment-codes"></a>Transaktionsjusteringskoder

I följande tabell visas orsakskoder för justeringar och deras beskrivningar.

| Orsakskod   | Description   |
|------------------|:-------------------------------------|
| AR-efterlevnad | Justering som minskar intäkterna när Microsoft-fakturor inte betalas i tid av partnern. |
| Co-op rollover | Justering som överför co-op-intäkter till en annan period eller konverterar co-op-intäkter till kunden. |
| Justering av operativa program | Justering som korrigerar microsofts systemberäkningsfel. |
| Felaktig beräkning för Ops-justering i Microsoft | Justering som korrigerar felberäkningar. |
| Ops Adjustment Microsoft incorrect enrollment | Justering för registreringsrelaterade felberäkningar. |
| Partnermappning (prenumeration) MCI/CSP | Justering som korrigerar prenumerationsfeljusteringen. |
| Principfel | Justering som åsidosätter en programregel.  |
| Intäkter från föregående period | Justering för intäkter utanför den aktuella intjäningsperioden. |

## <a name="payments"></a>Betalningar

Sidan **Betalningar** innehåller information om de pengar du har fått av Microsoft. Den visar även när och hur mycket du kommer att betalas.

> [!NOTE]
> För att vara berättigad till utbetalning måste dina intäkter nå [betalningströskeln](payment-thresholds-methods-timeframes.md) på 50 USD. Mer information finns i [Microsoft Publisher avtal](/legal/marketplace/msft-publisher-agreement).

- **Totalt antal som betalas** i år – summan som betalas ut till dig i år, i amerikanska dollar, för alla dina program.
- **Nästa beräknade betalning** – Den enda nästa betalningen kommer till dig (även om det kommer andra snart) i amerikanska dollar.
- **Senaste betalning** – Beloppet (i amerikanska dollar), programnamnet och programmet för din senaste betalning.
- **Betalning efter källa** – Betalningsbelopp (i amerikanska dollar) per program under de senaste 12 månaderna.

### <a name="payments-list"></a>Betalningslista

I **tabellen Lista över betalningar** visas betalda och väntande betalningar. Du kan ladda ned skatteinformation för tjänstavgifter i PDF-format och visa information om intjäning för en viss betalning.

:::image type="content" source="images/payouts/list-of-payments.png" alt-text="Exportera transaktionshistorik.":::

- **Betald** – Alla betalningar har skickats. Välj året i den nedrullningsna menyn för att filtrera fram de betalningar som gavs ut under det året.
- **Väntar –** kommande betalningar.
- **Skatt på tjänstavgifter (PDF-formulär)** – Tillgängligt för betalningar som har debiterats för serviceavgiftsskatt. Skatter på tjänstavgifter visas i **Andra skatter.**
- **Visa** – Omdirigerar till transaktionshistoriken med en lista över intäkter som ingår i betalningen.

Information om varför du kan ha saknade eller oväntade intäkter finns i [Vanliga frågor om utbetalning på den kommersiella marknadsplatsen.](payout-faq.yml#why-are-my-earnings-missing-)

### <a name="payment-status"></a>Betalningstatus

I följande tabell förklaras olika intäktsstatusar.

| Intäktsstatus | Anledning | Partneråtgärd krävs? |
| --- | --- | --- |
| Obearbetade | Intjäning är berättigad till betalning. Den förblir i det här tillståndet under en kylningsperiod enligt definitionen i programguiden för Incitamentsprogram. | No |
| Kommande | Betalningsordern genererade väntande interna granskningar innan betalningen bearbetas. | No |
| Väntande momsfaktura | Din momsfaktura är ofullständig eller ogiltig. | Du måste uppdatera din momsfaktura innan du kan betalas |
| Avvisades under granskning | Betalningen avvisades under granskningen. | Kontakta Microsofts support för mer information |
| Misslyckad | Betalningen misslyckades på grund av ett systemfel från Microsoft. | Kontakta Microsofts support för mer information |
| Pågår | Betalningen pågår. | No |
| Felaktig betalning | Betalningsrecouping pågår. | No |
| Skickat | Betalningen har skickats till din bank. | No |
| Upparbetning | Betalningen påträffade ett Microsoft-systemfel och bearbetas om. | No |
| Reversed | Betalningen har återförts av din bank och skickas igen i nästa betalningscykel. | No |
| Skattefakturan avvisades | Din skattefaktura avvisades under granskningen. Alla väntande betalningar är kvar tills granskningen av skattefakturan är klar. | Kontakta Microsofts support för mer information |
| Skattefaktura under granskning | Din momsfaktura granskas. Betalningen kommer att släppas när momsfakturan har godkänts. | No |
| Avslagen | Betalningen avvisades av din bank. | Kontakta din bank för mer information. |
|

### <a name="payments-download"></a>Nedladdning av betalningar

 I följande tabell förklaras varje kolumn i rapporten. Om du vill se mer information om dina betalningar **väljer du** Ladda ned överst på sidan Betalningar.

| Kolumnnamn | Description |
| --- | --- |
| deltagar-ID | Den primära identiteten för partnern som tjänar under programmet |
| participantIDType | Vanligtvis program-ID för incitamentsprogram och säljar-ID för butiksprogram |
| participantName | Namnet på den intjänande partnern |
| programName | Incitament/butiksprogramnamn |
| Tjänat | Belopp som intjänats i betala till-valutan för programmet/deltagar-ID:t |
| earnedUSD | Belopp som intjänats för program-/deltagar-ID i USD |
| withtax | Belopp skatt som medindets i betala till-valutan för programmet/deltagar-ID:t |
| salesTax | Totalt belopp för moms i betala till-valutan för program/deltagar-ID (gäller endast incitamentsprogram) |
| serviceFeeTax | Total mängd serviceFeeTax i betala till-valuta för program/deltagar-ID (gäller endast för butiksprogram Azure Marketplace) |
| totalbetalning | Total betalning i lokal valuta exklusive källskatten och inklusive momsen (om tillämpligt) för programmet/deltagar-ID:t |
| currencyCode | Valutakod för Betala till |
| paymentMethod | Den metod som används för att betala partnern, till exempel elektronisk banköverföring, kreditnota |
| paymentID | Unik identifierare för betalningen. Det här numret visas vanligtvis i ditt bankutdrag (gäller endast SAP-betalningar). |
| paymentStatus | Betalningstatus |
| paymentStatusDescription | Användarvänlig beskrivning av betalningsstatus |
| paymentDate | Datum då betalningen skickades från Microsoft |
|

## <a name="next-steps"></a>Nästa steg

- [Intäktssammanfattning](/partner-center/revenue-summary)
- [Ny exportsida för utbetalningsdata](/partner-center/payouts-enhanced-exports)
- [Partnerns utbetalnings-API](https://apidocs.microsoft.com/services/partnerpayouts)
- [Information om utbetalningsprincip](payout-policy-details.md)
- Om du behöver faktureringssupport kontaktar du supporten för [utgivare på den kommersiella marknadsplatsen.](https://partner.microsoft.com/support/v2/?stage=1)
