---
title: Registrera dina avtal
ms.topic: article
ms.date: 06/29/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: När du registrerar ett avtal som du har vunnit i Partnercenter hjälper det Microsoft att ge dig fler möjligheter i framtiden.
author: rajap-ms
ms.author: rajap
ms.localizationpriority: medium
ms.openlocfilehash: eaa9bb6f8e57033669ef584e7c52c0d050a532e0
ms.sourcegitcommit: 8235c89e789cdb5115fc1c19151fa8e97c743fe5
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/30/2021
ms.locfileid: "113080673"
---
# <a name="register-deals-youve-won-in-partner-center"></a>Registrera avtal som du har vunnit i Partnercenter

**Lämpliga roller:** Referensadministratör

Du kan registrera avtal som du har vunnit i Partnercenter genom att ange ytterligare information om kontraktet. Den här informationen hjälper oss att ge dig fler möjligheter i framtiden.

Det finns två vägar som leder till avtalsregistrering:

- Du har skapat ett nytt avtal i **avsnittet Möjligheter till säljförsäljning** och ditt avtal uppfyller villkoren för avtalsregistrering.
- Du vill rapportera ett stängt ISV Connect-avtal som inte samsåldes med Microsoft.

## <a name="register-a-deal-originating-from-a-co-sell-opportunity"></a>Registrera ett avtal som kommer från en möjlighet till säljförsäljning

Om du vill registrera ett avtal som kommer från en möjlighet till säljförsäljning måste ditt avtal uppfylla följande behörighetskrav:

- Avtalstypen är antingen samförsäljning eller partnerledd (du har valt att tillåta att Microsoft-säljare ser det här avtalet).
- Det finns minst en incitamentberättigad lösning i avtalet. En lösning är incitamentberättigad om den innehåller minst en av följande taggar:
  - Azure IP-sälj
  - Business Applications Premium
  - Business Applications Standard
- Statusen för avtalet är "Won".
- Om avtalstypen är säljinbjudan måste Microsoft antingen ha accepterat inbjudan eller markerat avtalet som vunnit. Du kan se Microsoft-statusen genom att titta på Microsoft-kortet under din avtalsinformation.

Om du har uppfyllt behörighetskraven uppmanas du automatiskt att registrera ditt avtal med knappen **Registrera nu** som visas i förloppsfältet för avtalet:

:::image type="content" source="images/register-deals.png" alt-text="Skärmbild som visar förloppsfältet för avtalet.":::

> [!NOTE]
> Om objektet **Avtalsregistrering** inte visas i förloppsfältet för avtalet uppfyller inte avtalet alla krav för avtalsregistrering.

När du **klickar på** Registrera dig nu omdirigeras du till sidan Avtalsregistrering och uppmanas att fylla i ett formulär med ifyllt information för din kund och lösning. Fyll i formuläret med hjälp av anvisningarna nedan och klicka på **Registrera**.

Vid registreringen skapas en eller två avtalsregistreringsposter beroende på lösningen.

- Om din lösning är berättigad till ISV Connect skapas en avtalsregistreringspost för ISV Connect. Den här avtalsregistreringsposten används för fakturering.
- Om din lösning är berättigad till IP-säljincitament skapas en registreringspost för IP-avtal för säljförsäljning. Den här avtalsregistreringsposten kommer att granskas och godkännas eller avvisas av granskningsteamet för säljavtal.

## <a name="report-a-closed-isv-connect-deal"></a>Rapportera ett stängt ISV Connect-avtal

Om du vill rapportera ett stängt ISV Connect-avtal går du till **fliken Avtalsregistrering** och klickar **på + Rapportera stängt ISV Connect-avtal.** Fyll i de obligatoriska fälten och klicka på **Registrera**. Den här avtalsregistreringsposten används för fakturering.

## <a name="fill-out-the-deal-registration-form"></a>Fyll i formuläret för avtalsregistrering

> [!NOTE]
> Du kan filtrera avtal efter kundnamn, status och avtalstyp. Det gör du genom att **klicka på** knappen Filter längst upp på sidan Avtalsregistrering.

Oavsett om du har kommit till avtalsregistreringen från en möjlighet till säljförsäljning eller om du rapporterar ett stängt ISV Connect-avtal som inte har samförsäljningsförsäljning med Microsoft, uppmanas du att fylla i följande fält i formuläret för avtalsregistrering.

- **Kundinformation:** Ange **företagets namn** för kunden och välj **land/region.** Ange sedan **ort och** **delstat/provins.**
- **Lösning:** Välj den lösning som ska användas för avtalet. Kontakta supporten om du inte ser rätt lösning i listan.
- **Kontrakttyp:** Ange om det här avtalet är **ett nytt** kontrakt eller **en förnyelse** av ett tidigare kontrakt.
- **Totalt kontraktsvärde:** Det totala förväntade värdet för engagemanget. Det här värdet ska innehålla alla programvaru- och tjänstavgifter, men inte maskinvarukostnader. Se till att välja lämplig valuta.
- **Lösningsvärde:** Det totala värdet för den molnlösning som ska användas för avtalet. Se till att inkludera alla kostnader som är kopplade till programvaru- och underhållsavgifter, men inkludera inte återbetalningsbara objekt, icke-återkommande anpassningsavgifter eller direkt kopplade CSP-licensavgifter som betalas av Microsoft.
- **Kommer lösningen att distribueras i Azure? Om inte väljer du Annat:** Välj **antingen Azure** eller **Annat.**
- **Kommer förbrukningen av lösningen att köras på partnerklientorganisationen eller kundklientorganisationen?**: Välj antingen **kundklientorganisationen** eller **partnerklientorganisationen**.
- **Kontraktets startdatum:** Det datum då kontraktet börjar. För pay-as-you-go-avtal (PAYG) använder du datumet för den första fakturan. Partnercenter låter dig inte ange ett startdatum tidigare än avtalstecknets datum. Detta kan påverka vissa avtal, till exempel IP-distributioner som börjar före signeringsdatumet. För att kunna genomföra dessa avtal använder du avtalstecknets datum **för både** signeringsdatum och startdatumfält när du skickar in. (Kontraktet bör uttryckligen ange avtalets varaktighet så att ACV kan beräknas korrekt.)
- **Slutdatum för kontraktet:** Om kontraktet slutar på ett visst datum väljer du **Har ett slutdatum** och anger det datumet. Om kontraktet inte har något specifikt slutdatum väljer du **Beständiga**. För pay-as-you-go-avtal (PAYG) använder du datumet för den senaste eller senaste fakturan.
- **Signerat kontraktsdatum:** Det datum då det slutliga kontraktet signerades av din organisation och av kunden. För pay-as-you-go-avtal (PAYG) använder du datumet för den första fakturan.
- **Registreringskontakt:** **Förnamn,** **Efternamn,** Telefonnummer och  E-postadress för en person i din organisation som vi kan kontakta om vi behöver mer information om informationen som anges här. 

När du har slutfört alla avsnitt på sidan klickar du på **Registrera**.

- Om avtalet är ett ISV Connect-avtal ser du att statusen för avtalet är "Submitted, Completed" (Skickat, Slutfört). Ingen ytterligare åtgärd krävs för den här avtalsregistreringsposten. Den här posten används för fakturering.
- Om avtalet är ett IP-säljavtal ser du att statusen för avtalet är "Skickat". Microsofts granskningsteam för säljavtal granskar den information som du angav i den här avtalsregistreringsposten. Granskningsteamet begär mer åtgärder från dig om det behövs eller godkänner/avvisar avtalet direkt.
- Om du registrerar ett avtal som kommer från en möjlighet till säljförsäljning och du ser att två avtalsregistreringsposter har skapats, innebär det att lösningen i ditt avtal är berättigad för både ISV Connect och IP-sälj. ISV Connect-posten använder för fakturering. IP-säljeposten granskas av valideringsteamet för säljavtal.

