---
title: Få betalt på den kommersiella marknadsplatsen
description: Lär dig mer om att få betalningar för intäkter på den kommersiella Marketplace – Azure Marketplace. Inkluderar utbetalnings princip, utbetalnings status och utbetalnings instruktioner.
ms.service: marketplace
ms.topic: conceptual
ms.date: 09/28/2020
author: eunjkim520
ms.author: eunjkim
ms.openlocfilehash: db347387df29dc36e256881546e632bd321dfde5
ms.sourcegitcommit: 3c45a181ef86b3a4866e97fb50efeae8714ab3f7
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 10/19/2020
ms.locfileid: "92532041"
---
# <a name="getting-paid-in-the-commercial-marketplace"></a>Få betalt på den kommersiella marknadsplatsen

Den här artikeln innehåller viktig information om att ta emot betalning för dina erbjudanden, tillägg och marknadsförings intäkter. Den sammanfattar en utbetalnings princip, steg som krävs innan du betalar och utbetalnings översikt.

## <a name="commercial-marketplace-payout-policies-and-agreements"></a>Principer och avtal för utbetalning av kommersiella marknads platser

För att få betalt måste du följa avtalen och utbetalnings principen.

- [Microsoft Azure Marketplace utgivar avtal](https://go.microsoft.com/fwlink/p/?LinkID=699560): innan du får betalt måste du godkänna det här utgivar avtalet. I det här avtalet förklaras förhållandet mellan dig och Microsoft som det gäller för säljar erbjudanden på den kommersiella marknaden, inklusive lagrings avgiften som Microsoft debiterar för varje försäljning.
- [Utbetalnings princip](payout-policy-details.md) visar betalnings principer för utbetalning, inklusive betalnings schema och betalnings metoder. Principen förklarar även processen för kunder som inte är betalningar.
- [Skatte information](tax-details-marketplace.md) förklarar skatte överväganden för pris val och skatte ansvar enligt Microsofts [utgivar avtal](https://go.microsoft.com/fwlink/p/?LinkID=699560).
- **Butiks avgifter** definieras officiellt i utgivar avtalet. Butiks avgiften tillämpas på alla försäljnings erbjudanden som samlas in av den kommersiella Marketplace, inklusive tillägg.
- **Betalningar** görs varje månad (förutsatt att betalnings tröskeln har uppfyllts). Vi skickar vanligt vis alla betalningar som förfaller under en månad med den 15: e dagen i den månaden. Betalningar tar vanligt vis 3 till 10 arbets dagar att uppnå ditt utbetalnings konto. Mer information finns i [betalnings trösklar, metoder och tids ramar](payment-thresholds-methods-timeframes.md).

## <a name="prerequisite-steps-before-getting-paid"></a>Nödvändiga steg innan du får betalt

Innan du börjar betala första gången måste du ställa in ditt utbetalnings konto och slutföra de nödvändiga bank-och skatte formulären. I bank-och skatte formulär får du dina prioriterade betalnings metoder och skatte former för käll skatt. Bank-och skatte formulär krävs innan vi kan betala. Mer information finns i [Konfigurera ditt konto för utbetalning och skatte former](set-up-your-payout-account.md).

### <a name="payout-hold-status"></a>Status för utbetalning

Som standard skickar vi betalningar varje månad enligt beskrivningen ovan. Du kan dock välja att ställa in dina utbetalningar för ett program som är parkerat och att Microsoft inte släpper ut dina betalningar på ditt konto. Om du väljer att spärra dina inbetalningar kommer vi att fortsätta att registrera intäkter på sidan **utbetalningar** . Vi kommer dock inte att skicka några betalningar till ditt konto förrän du tar bort spärren.

Om du vill spärra dina betalningar går du till **konto inställningar** . Under **utbetalning och skatt** , i avsnittet **utbetalning och skatte profil tilldelning** , letar du reda på det program som du vill ha betalningar för. Markera kryss rutan **Behåll min betalning** för att hålla betalningarna för det här programmet. Du kan ändra din utbetalnings status när som helst, men ditt beslut kommer att påverka nästa månads utbetalning. Om du till exempel vill ha en utbetalning av april, se till att ställa in din utbetalnings status **till före slutet** av mars.

När du har angett statusen för din utbetalnings spärr till **på** , är alla utbetalningar för det här programmet kvar tills du avmarkerar kryss **rutan.** När du gör det kommer du att inkluderas under nästa månads utbetalnings cykel (förutsatt att betalnings tröskeln har uppfyllts). Om du har haft dina inbetalningar spärrade, men vill ha en utbetalning som genererats i juni, avmarkerar du kryss **rutan för att ta bort den** före slutet av maj.

>[!Note]
> Din utbetalnings status gäller för varje program individuellt (Microsoft Store, annonsering, Azure Marketplace och så vidare). Om du vill lagra betalningar för alla dina program, ska du lagra det på varje program separat.

## <a name="payout-statements"></a>Utbetalningsinstruktioner

Utbetalnings instruktionen visar dina intäkter från försäljningen från dina erbjudanden och tillägg i transaktions historiken. Du kan också Visa betalnings information och hämta rapporter i TSV-eller CSV-format. Se [utbetalnings instruktioner](payout-statement.md) för att lära dig mer om hur du får åtkomst till utbetalnings instruktionen och information om transaktions historik och betalnings rapporter. Dessutom kan du använda [partnerns utbetalnings-API](https://apidocs.microsoft.com/services/partnerpayouts) för att systematiskt Hämta utbetalnings rapporterna.

## <a name="next-steps"></a>Nästa steg

- [Partner utbetalnings-API](https://apidocs.microsoft.com/services/partnerpayouts)
- [Vanliga frågor och svar om Marketplace](payout-faq.md)
