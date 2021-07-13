---
title: Få betalt i Partnercenter
description: Lär dig mer om att ta emot betalningar för intäkter som en Microsoft-partner, till exempel via erbjudanden på den kommersiella marknadsplatsen, incitamentprogram och Molnlösningsleverantör-programmet. Innehåller utbetalningsprincip, utbetalningsstatus och utbetalningsutdrag.
ms.service: marketplace
ms.subservice: partnercenter-marketplace-publisher
ms.topic: conceptual
ms.date: 11/25/2020
author: eunjkim520
ms.author: eunjkim
ms.openlocfilehash: cc01a1aada6c6665d3fd8f6efc6e5ef873736bdc
ms.sourcegitcommit: a09a5f893e876de23a8aa5c0d637e50c5be84941
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 07/13/2021
ms.locfileid: "113684397"
---
# <a name="getting-paid-in-partner-center"></a>Få betalt i Partnercenter

**Lämpliga roller:** Kontoadministratörsroller | Global administratör

Den här artikeln innehåller viktig information om hur du tar emot betalning för dina erbjudanden, tillägg och reklamintäkter. Den sammanfattar utbetalningsprincipen, de steg som krävs innan du betalar och översikten över utbetalningsutdrag.

## <a name="payout-policies-and-agreements"></a>Utbetalningsprinciper och avtal

För att få betalt måste du följa avtalen och utbetalningsprincipen.

- [Microsoft Azure Marketplace Publisher:](/legal/marketplace/msft-publisher-agreement)Innan du får betalt måste du godkänna det här utgivaravtalet. Det här avtalet beskriver relationen mellan dig och Microsoft vad gäller säljarerbjudanden på den kommersiella marknadsplatsen, inklusive butiksavgiften som Microsoft debiterar för varje försäljning som görs.
- [Utbetalningspolicyn](payout-policy-details.md) visar utbetalningsbetalningsprinciperna, inklusive betalningsschema och betalningsmetoder. Principen förklarar också processen för icke-betalningar från kunder.
- [Skatteinformation](tax-details-marketplace.md) förklarar skatteuppskattningen vid val av pris och skatteansvar enligt [Microsofts Publisher avtal.](/legal/marketplace/msft-publisher-agreement)
- **Butiksavgifter** definieras officiellt i Publisher avtalet. Butiksavgiften tillämpas på alla erbjudanden som samlas in av den kommersiella marknadsplatsen, inklusive tillägg.
- **Betalningar** görs månadsvis (förutsatt att betalningströskeln har uppnåtts). Vi skickar vanligtvis alla betalningar som förfaller under en viss månad den 15:e dagen i den månaden. Betalningar tar vanligtvis 3 till 10 ytterligare arbetsdagar för att nå ditt utbetalningskonto. Mer information finns i [Betalningströsklar, metoder och tidsramar.](payment-thresholds-methods-timeframes.md)

## <a name="prerequisite-steps-before-getting-paid"></a>Nödvändiga steg innan du betalar

Innan du får betalt första gången måste du konfigurera ditt utbetalningskonto och fylla i nödvändiga bank- och skatteformulär. I bank- och skatteformulär anger du dina önskade betalningsmetoder och skatteformulär för källskatt. Bank- och skatteformulär krävs innan vi kan betala dig. Mer information finns i [Konfigurera ditt utbetalningskonto och skatteformulär.](set-up-your-payout-account.md)

### <a name="payout-hold-status"></a>Status för utbetalnings hold

Som standard skickar vi betalningar per månad enligt beskrivningen ovan. Du kan dock lägga ut dina betalningar för ett program som är i spel och Microsoft kommer inte att släppa dina betalningar till ditt konto. Om du väljer att vänta med dina utbetalningsbetalningar fortsätter vi att registrera eventuella intäkter på **sidan Utbetalningar.** Vi skickar dock inga betalningar till ditt konto förrän du tar bort stödet.

Om du vill hålla dina betalningar väljer du **Inställningar** kugghjulsikonen längst upp till höger och sedan **Kontoinställningar**. Välj **Utbetalning och skatt** på den  vänstra menyn. I avsnittet Utbetalnings- och skatteprofiltilldelning letar du upp programmet som du vill att betalningarna ska hållas för. Markera kryssrutan **Håll min betalning för** att hålla betalningar för det här programmet. Du kan ändra statusen för utbetalnings hold när som helst, men ditt beslut påverkar nästa månadsutbetalning. Om du till exempel vill hålla kvar aprils utbetalning ska du se till att ställa in statusen för utbetalnings hold till **På** innan slutet av mars.

När du har ställt in din utbetalningsstatus på **På** är alla utbetalningar för det här programmet kvar tills du avmarkerar kryssrutan till **Av**. När du gör det inkluderas du under nästa månatliga utbetalningscykel (förutsatt att betalningströskeln har uppnåtts). Om du har fått vänta på dina utbetalningsbetalningar, men vill generera en utbetalning i juni, avmarkerar du kryssrutan till **Av** innan slutet av maj.

>[!Note]
> Din utbetalningsstatus gäller för varje program individuellt (Microsoft Store, reklam, Azure Marketplace och så vidare). Om du vill hålla betalningar för alla dina program kan du hålla betalningen på varje program individuellt.

## <a name="payout-statements"></a>Utbetalningsinstruktioner

Utbetalningsutdrag visar dina intäkter från försäljningen från dina erbjudanden och tillägg i transaktionshistoriken. Du kan också visa betalningsinformation och ladda ned rapporter i tsv- eller csv-format. Se [Utbetalningsutdrag](payout-statement.md) för att lära dig mer om hur du kommer åt utbetalningsutdrag och information om transaktionshistorik och betalningsrapporter. Dessutom kan du använda API:et [partnerutbetalningar för](https://apidocs.microsoft.com/services/partnerpayouts) att systematiskt hämta utbetalningsrapporterna.

## <a name="next-steps"></a>Nästa steg

- [PARTNER utbetalnings-API](https://apidocs.microsoft.com/services/partnerpayouts)
- [Vanliga frågor och svar om utbetalning](payout-faq.yml)