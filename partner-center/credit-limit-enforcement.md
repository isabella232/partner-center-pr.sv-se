---
title: Tvingande kreditgräns
ms.topic: how-to
ms.date: 05/11/2021
description: Lär dig mer om din kreditgräns och hur den beräknas. Innehåller vanliga frågor och svar.
ms.service: partner-dashboard
ms.subservice: partnercenter-billing
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 32dc94a4bd85160a02a4be880469f713d98449ba
ms.sourcegitcommit: ad1af627f5ee6b6e3a70655f90927e932cf4c985
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 07/29/2021
ms.locfileid: "114837976"
---
# <a name="credit-limit-enforcement-cle"></a>Tvingande kreditgräns (CLE)

**Lämpliga roller:** Faktureringsadministratör

## <a name="your-credit-limit-and-how-it-works"></a>Din kreditgräns och hur den fungerar

Din kreditgräns är det maximala belopp (i amerikanska dollar) som du som partner kan spendera för att köpa produkter eller prenumerationer i Partnercenter. Om du överskrider kreditgränsen kan du inte göra nya köp förrän tillräckligt med betalning har gjorts. Dina befintliga prenumerationer fortsätter att avbrytas.

Kreditgränser gäller för erbjudanden i Azure-plan, Azure-reservationer, programvara, Marketplace, Azure 145 P, Office och Dynamics-produkter. Kreditgränser gäller inte för förnyelser och löpande förbrukning.

Vi tilldelar din kreditgräns på klientorganisationsnivå under registreringsperioden. Vi baserar den på dina prognostiserade intäkter, inköp och betalningshistorik. Sedan använder vi följande formel för att beräkna ditt tillgängliga saldo:

**[Kreditgräns – (inkommande köp + utestående obetalta fakturor + ej fakturerade avgifter – överskottsbetalning)]**

## <a name="frequently-asked-questions"></a>Vanliga frågor och svar

### <a name="is-my-credit-limit-set-at-the-tenant-or-global-level"></a>Har min kreditgräns angetts på klientorganisationsnivå eller global nivå?

Klientorganisationsnivå. Anta till exempel att du arbetar från USA, Kanada och Japan. Om den amerikanska klientorganisationen når sin kreditgräns får den klientorganisationen ett meddelande när de försöker göra ett köp i Partnercenter. De andra klienterna påverkas inte. 

### <a name="if-i-exceed-my-credit-limit-can-i-continue-servicing-existing-customers-and-subscriptions-with-full-access"></a>Kan jag fortsätta att betjäna befintliga kunder och prenumerationer med fullständig åtkomst om jag överskrider min kreditgräns?

Ja. Dina kunders befintliga prenumerationer fortsätter utan avbrott. Du kan dock inte köpa nya prenumerationer för dina kunder.

### <a name="does-cle-apply-to-both-direct-bill-partners-and-indirect-providers"></a>Gäller CLE både direkta faktureringspartner och indirekta leverantörer?

Ja, det gäller för båda.

### <a name="after-i-submit-my-payment-to-reinstate-my-account-when-can-i-purchase-more-subscriptions"></a>När jag har skickat min betalning för att återställa mitt konto, när kan jag köpa fler prenumerationer? 

Du bör kunna återuppta köpet inom 24 timmar från betalningen, förutsatt att Microsoft har fått alla krav för att fortsätta med kreditkontrollprocessen.

### <a name="how-can-i-check-my-credit-limit"></a>Hur kan jag kontrollera min kreditgräns?

Kontakta [ucmwrcsp@microsoft.com](mailto:ucmwrcsp@microsoft.com) om du vill se din kreditgräns och få information om de senaste köpen.

### <a name="do-invoices-that-are-in-dispute-count-against-the-credit-limit"></a>Räknas fakturor som är i konflikt med kreditgränsen?

Ja. Du kan dock kontakta Microsoft på [ucmwrcsp@microsoft.com](mailto:ucmwrcsp@microsoft.com) för att lösa problemet.

### <a name="how-soon-will-i-hear-back-if-i-write-to-ucmwrcspmicrosoftcom"></a>Hur snart kommer jag att höra tillbaka om jag skriver till ucmwrcsp@microsoft.com ?

Du bör ha ett svar på mindre än 24 timmar. 

### <a name="what-criteria-does-microsoft-use-for-setting-a-partners-credit-limit"></a>Vilka kriterier använder Microsoft för att ange en partners kreditgräns?

Vi fastställer din kreditgräns baserat på dina prognostiserade intäkter, köpprowes och betalningshistorik.

### <a name="is-the-credit-limit-currently-enforced-on-the-new-commerce-experience"></a>Tillämpas kreditgränsen för den nya handelsupplevelsen för närvarande?

Ja. Kreditgränser gäller för alla CSP-program och produkter i Partnercenter.

### <a name="who-will-receive-the-notification-when-my-organization-is-nearing-its-credit-limit"></a>Vem får meddelandet när min organisation närmar sig sin kreditgräns?

Din organisations ekonomikontoreskontrakontakt bör få meddelandet.

## <a name="next-steps"></a>Nästa steg

[Grundläggande information om fakturering](./billing-basics.md)
