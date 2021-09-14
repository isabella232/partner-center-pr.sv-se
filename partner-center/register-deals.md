---
title: Registrera dina avtal
ms.topic: article
ms.date: 09/08/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-referrals
description: När du registrerar ett avtal som du har vunnit i Partnercenter hjälper det Microsoft att ge dig fler möjligheter i framtiden.
author: rajap-ms
ms.author: rajap
ms.localizationpriority: medium
ms.openlocfilehash: 22dcf93c5028716fc3810c826abe1819459e58e1
ms.sourcegitcommit: 37eac16c4339cb97831eb2a86d156c45bdf6a531
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/13/2021
ms.locfileid: "126249091"
---
# <a name="register-deals-youve-won-in-partner-center"></a>Registrera avtal som du har vunnit i Partnercenter

**Lämpliga roller:** Referensadministratör

Du kan registrera avtal som du har vunnit i Partnercenter genom att ange ytterligare information om kontraktet. Den här informationen hjälper oss att ge dig fler möjligheter i framtiden.

Det finns två vägar som leder till avtalsregistrering:

- Du har skapat ett nytt avtal i **avsnittet Möjligheter till säljförsäljning** och ditt avtal uppfyller villkoren för avtalsregistrering.
- Du vill rapportera ett stängt ISV Anslut avtal som inte samsåldes med Microsoft.

> [!IMPORTANT]
> Om avtalet är berättigat till avtalsregistrering kontrollerar du att det finns en lucka på 72 timmar mellan att avtalet skapas och att avtalet markeras som vunnit. Om du stänger avtalet som tidigare har vunnits kan det leda till att avtalsregistreringar avvisas.

## <a name="register-a-deal-originating-from-a-co-sell-opportunity"></a>Registrera ett avtal som kommer från en möjlighet till säljförsäljning

Om du vill registrera ett avtal som kommer från en möjlighet till säljförsäljning måste ditt avtal uppfylla följande behörighetskrav:

- Avtalstypen är antingen Samförsäljning eller partnerledd (du har valt att låta Microsoft-säljare visa det här avtalet).
- Avtalsvärdet är större än eller lika med 25 000 USD. Valutakonverteringen baseras på de månatliga [växelkurser som publiceras](https://www.reuters.com/markets/currencies) avByte.
- Det kundkonto som valts för avtalet hanteras av Microsoft. Det här är konton där Microsofts säljteam har en befintlig relation med företaget.
- Det finns minst en incitamentsberättigad lösning i avtalet. En lösning är berättigad till incitament om den innehåller minst en av följande taggar:
  - Azure IP Co-sell
  - Business Applications Premium
  - Business Applications Standard
- Avtalets status är **Won (Vunnit).**
- Om avtalstypen är Samförsäljning måste Microsoft antingen ha accepterat inbjudan eller markerat avtalet som vunnit. Du kan se Microsoft-statusen på Microsoft-kortet under din avtalsinformation.

> [!Important]
> Registrera avtalet endast om företagets namn och den berättigade lösningen för incitament i avtalet tydligt anges i avtalet med kunden.

Om du har uppfyllt behörighetskraven uppmanas du automatiskt att registrera ditt avtal med knappen **Registrera nu** som visas i förloppsfältet för avtalet:

:::image type="content" source="images/register-deals.png" alt-text="Skärmbild som visar förloppsfältet för avtalet.":::

> [!NOTE]
> Om **avtalsregistreringsobjektet** inte visas i avtalsförloppet för ditt avtal uppfyller inte avtalet alla krav för avtalsregistrering.

Du kan välja att registrera avtalet direkt efter att ha markera avtalet som won (vunnit) eller vid ett senare tillfälle via knappen Registrera nu för avtalslivscykeln. När avtalet har registrerats kan du visa förloppet för avtalsverifieringen från samma livscykel. Om det krävs någon åtgärd från ditt företag visas lämpliga fel i avtalslivscykelvyn. Avtalet förs i ett stängt tillstånd när avtalsverifieringen är klar.

### <a name="combinations"></a>Kombinationer

Tabellen nedan visar kombinationerna av vem som kan bjudas in i det här skedet av avtalet.

|**Ursprunglig avtalstyp**|**Vem kan bjudas in**|**Kommentarer**|
|-----|:-----|:-----|
|Privat|Microsoft och/eller andra partner|Avtalet uppgraderas till säljavtal om Microsoft bjuds in.|
|Privat|Microsofts säljteam för att visa avtal|Avtalet uppgraderas till partnerledd när Microsofts säljteam får insyn i avtalet.|
|Partnerledd|Microsoft och/eller andra partner|Avtalet uppgraderas till säljavtal om Microsoft bjuds in.|
|Säljförsäljning|Andra partner|Andra partner kan bara bjudas in om ditt företag har initierat avtalet. Partner kan inte bjudas in för avtal på fliken Inkommande.|
|Partner till partner utan Microsoft|Microsoft|Avtalet kommer att uppgraderas till ett säljavtal.|
|Partner till partner utan Microsoft|Andra partner||

När du **har klickat** på Registrera dig nu omdirigeras du till sidan Avtalsregistrering och uppmanas att fylla i ett formulär som innehåller i förväg ifylld information för din kund och lösning. Fyll i formuläret med hjälp av anvisningarna nedan och klicka på **Registrera**.

Vid registreringen skapas en eller två avtalsregistreringsposter beroende på lösningen.

- Om din lösning är berättigad till ISV Connect skapas en ISV Connect-avtalsregistreringspost. Den här avtalsregistreringsposten används för fakturering.
- Om din lösning är berättigad till IP-säljincitament skapas en registreringspost för IP-avtal för säljförsäljning. Den här avtalsregistreringsposten granskas och godkänns eller avvisas av granskningsteamet för säljavtal.

## <a name="report-a-closed-isv-connect-deal"></a>Rapportera ett stängt ISV-Anslut avtal

Om du vill rapportera ett stängt ISV Anslut-avtal går du till fliken Avtalsregistrering och klickar **på + Rapportera stängd ISV-Anslut avtal.**  Fyll i de obligatoriska fälten och klicka på **Registrera**. Den här avtalsregistreringsposten används för fakturering.

## <a name="fill-out-the-deal-registration-form"></a>Fyll i formuläret för avtalsregistrering

> [!NOTE]
> Du kan filtrera avtal efter kundnamn, status och avtalstyp. Det gör du genom att **klicka på knappen** Filter längst upp på sidan Avtalsregistrering.

Oavsett om du har kommit för att göra en avtalsregistrering från en möjlighet till säljförsäljning eller om du rapporterar ett stängt ISV Anslut-avtal, som inte samsåldes med Microsoft, uppmanas du att fylla i följande fält i formuläret för avtalsregistrering.

- **Kundinformation:** Ange **företagets namn** för kunden och välj **land/region.** Ange sedan **ort** och **delstat/provins.**
- **Lösning:** Välj den lösning som ska användas för avtalet. Kontakta supporten om du inte ser rätt lösning i listan.
- **Kontrakttyp:** Ange om det här avtalet är **ett nytt** kontrakt eller en **förnyelse** av ett tidigare kontrakt.
- **Totalt kontraktsvärde:** Det totala förväntade värdet för engagemanget. Det här värdet bör innehålla alla programvaru- och tjänstavgifter, men inte maskinvarukostnader. Se till att välja lämplig valuta.
- **Lösningsvärde:** Det totala värdet för den molnlösning som ska användas för avtalet. Se till att inkludera alla kostnader som är kopplade till programvara och underhållsavgifter, men inkludera inte återbetalningsbara objekt, icke-återkommande anpassningsavgifter eller direkt kopplade CSP-licensavgifter som betalas av Microsoft.
- **Kommer lösningen att distribueras i Azure? Om inte väljer du Annat:** Välj **antingen Azure** eller **Annat.**
- **Kommer förbrukningen av lösningen att köras på partnerklienten eller kundklientorganisationen?**: Välj antingen **kundklienten** eller **partnerklienten**.
- **Kontraktets startdatum:** Det datum då kontraktet börjar. För PAYG-avtal (Betala per användning) använder du datumet för den första fakturan. Partnercenter låter dig inte ange ett startdatum tidigare än kontraktstecknets datum. Detta kan påverka vissa avtal, till exempel IP-distributioner som startar före signeringsdatumet. För att kunna ingå dessa avtal använder du kontraktstecknets datum för **både** signeringsdatum och startdatumfält när du skickar in. (Kontraktet bör uttryckligen ange avtalets varaktighet så att ACV kan beräknas korrekt.)
- **Kontraktets slutdatum:** Om kontraktet slutar på ett visst datum väljer du **Har ett slutdatum och** anger det datumet. Om kontraktet inte har något specifikt slutdatum väljer du **Beständig**. För PAYG-avtal (betala per användning) använder du datumet för den senaste eller senaste fakturan.
- **Signerat kontraktsdatum:** Det datum då det slutliga kontraktet signerades av din organisation och av kunden. För PAYG-avtal (Betala per användning) använder du datumet för den första fakturan.
- **Registreringskontakt:** **Förnamn,** **Efternamn,** **Telefon nummer** och  E-postadress för en person i din organisation som vi kan kontakta om vi behöver mer information om informationen som anges här.

När du har slutfört alla avsnitt på sidan klickar du på **Registrera**.

- Om avtalet är ett isv-Anslut-avtal ser du att statusen för avtalet är **Skickat, Slutfört.** Det krävs ingen ytterligare åtgärd för den här avtalsregistreringsposten. Den här posten används för fakturering.
- Om avtalet är ett IP-säljavtal ser du att avtalets status är **Skickat.** Microsofts granskningsteam för säljavtal granskar den information som du angav i den här avtalsregistreringsposten. Granskningsteamet begär mer åtgärder från dig om det behövs, eller godkänner eller avvisar avtalet direkt.
- Om du registrerar ett avtal som kommer från en möjlighet till säljförsäljning och du ser att två avtalsregistreringsposter har skapats, innebär det att lösningen i ditt avtal är berättigad för både ISV Anslut och IP-sälj. ISV Anslut posten använder för fakturering. IP-säljeposten granskas av valideringsteamet för säljavtal.

## <a name="simplified-deal-registration-for-commercial-marketplace-transactions"></a>Förenklad avtalsregistrering för transaktioner på den kommersiella marknadsplatsen

Säljförsäljning vinner köp via den kommersiella marknadsplatsen [kommer](/azure/marketplace/) att dra nytta av betydande enkelhet i formuläret för avtalsregistrering.  Dessutom kräver avtal som har transaktioner via Commercial Marketplace inte ytterligare avtalsgranskningssamtal, vilket sparar drifttid och arbete.

Du behöver bara ange tre uppgifter:

1. Ange genom att markera kryssrutan om avtalet har handlats eller kommer att handla via den kommersiella marknadsplatsen.
2. Beräknat transaktionsdatum (i `mm-dd-yyyy` format).
3. Registrera partnerns kontaktuppgifter om det finns frågor om avtalet.
