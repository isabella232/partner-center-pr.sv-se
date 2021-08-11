---
title: Betalningsstatus för lösningsbedömning
ms.topic: how-to
ms.date: 11/09/2020
description: Använd CHIP (Channel Incentives Platform) för att hitta information om affärsmöjligheter för lösningsbedömning, deras beräkningar och deras betalningsstatus.
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
author: Karthic83
ms.author: kashanum
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 5443dedfcae17152b51df7aa021d900b2f61892509c85ba3c2ba99cb0b9b3a8d
ms.sourcegitcommit: 121f1b9cbd88faeba60dc9b475f9c0647cdc933c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/06/2021
ms.locfileid: "115692678"
---
# <a name="solution-assessment-payment-status-and-calculation-info"></a>Betalningsstatus och beräkningsinformation för Solution Assessment

**Lämpliga roller:** Primär kontakt eller programadministratör

Du kan granska betalningsstatusen för en affärsmöjlighetsstatus för solution assessment i CHIP.

## <a name="how-to-review-your-payment-status"></a>Så här granskar du din betalningsstatus

1. Öppna CHIP och logga in med ditt Microsoft-konto (tidigare live-ID).
2. I fältet **Affärsmöjlighets-ID** skriver eller klistrar du in ID-numret för affärsmöjligheten.
3. Klicka på **Sök**.
4. Välj affärsmöjlighetens namn för att visa information om affärsmöjligheten.
5. Kontrollera avsnittet **Betalningsbegäranden** för att se om en betalningsbegäran har skapats.
6. Granska affärsmöjlighetens status.

    - Om betalningsbegäran inte har skapats ser du till att affärsmöjligheten uppfyller behörighetskriterierna för att få incitamentet för lösningsutvärderingar. Du hittar mer information om att kontrollera behörighetskriterierna i [Solution Assessment.](chip-solution-assessment.md)
    - Om betalningsbegäran har skapats fortsätter du till steg 7.
7. Kontrollera status för betalningsbegäran.

    - Väntande betalningsgranskning: Kontakta Channel Incentives-teamet för vidare undersökning – kontaktuppgifter som anges nedan.
    - Godkänd betalning: Betalningen renderas av Microsoft inom 35 dagar från slutet av månaden efter EM-certifieringen av engagement-slutförande i CHIP där betalningsbegäran skapades
    -  Betalning skickat: Klicka på statuslänken för att visa betalningsinformation.
    - Betalningen avbröts: Klicka på statushyperlänken för att visa avvisningsorsaken. Kontakta Channel Incentives-teamet om du vill ha mer information.

## <a name="calculations-for-solutions-assessment"></a>Beräkningar för utvärdering av lösningar

Med hjälp av de definierade avgiftsschemana beräknar och bearbetar Microsofts regionala driftcentraler de associerade incitamentavgifterna, där betalningar utfärdas månadsvis.

Affärsmöjligheter måste ha alla följande attribut för att visas i den här rapporten för betalningsgodkännande:

1. Incitamentet för lösningsbedömning måste godkännas.

1. Lokalt attribut för lösningsutvärdering engagemangsnivå Frekvensnivå anges för engagemanget vid tidpunkten då incitamentet godkänns i MSX.
 
1. Kryssrutan "EM Review" måste vara markerad och skickad av EM i CHIP.

## <a name="next-steps"></a>Nästa steg

- [Problem med att komma åt CHIP](chip-access-trouble.md) 
