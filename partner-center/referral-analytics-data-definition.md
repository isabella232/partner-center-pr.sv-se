---
title: Referensanalysdatadefinitioner
ms.topic: article
ms.date: 08/10/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-referrals
description: Dokumentet innehåller olika rapporter och deras datadefinitioner, som du kan ladda ned från referensanalyssidorna.
author: v-sausharma
ms.author: v-sausharma
ms.localizationpriority: medium
ms.openlocfilehash: e2409dcbfd2a9de677ef4ec79bf8749072859325
ms.sourcegitcommit: 37eac16c4339cb97831eb2a86d156c45bdf6a531
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/13/2021
ms.locfileid: "126246727"
---
# <a name="referral-analytics-export--data-definitions"></a>Export av hänvisningsanalys – datadefinitioner

**Lämpliga roller:** Referensadministratör

## <a name="introduction"></a>Introduktion

Genom att använda knappen Exportera på sidan Lead- och säljförsäljningsanalys kan du exportera rådatauppsättningarna.

De olika rapporterna, som du kan ladda ned tillsammans med deras datadefinitioner, visas i följande tabeller:

## <a name="leads-export"></a>Export av leads

|   Kolumnnamn |   Databeskrivning    |
|----|----|
|   Hänvisningskod |   Unikt ID för hänvisning  |
|   Kundland    |   Kundens land |
|   Kundnamn   |   Kundens namn    |
|   Skapandedatum för referens  |   Skapandedatum för hänvisning   |
|   Referenskälla |   Källa för hänvisningen: Kvalificerad, Marketplace  |
|   Referenstyp   |   Typ av lead    |
|   Leadriktning  |   Leadens riktning   |
|   Leadvaluta   |   Leadens valuta    |
|   Leadvärde  |   Beräknat leadvärde som tillhandahålls av partner    |
|   Leadvärde (USD)    |   Beräknat leadvärde som tillhandahålls av partner i USD |
|   Status      |   Senaste status för hänvisning   |
|   Statusorsak   |   Kommentarer eller orsak till statusen    |
|       |       |


## <a name="co-sell-export"></a>Export av säljförsäljning

|   Kolumnnamn |   Databeskrivning    |
|    ----    |    ----    |
|   Hänvisningskod |   Unikt ID för hänvisning  |
|   Kundland    |   Kundens land |
|   Kundstad   |   Kundens stad    |
|   Kundnamn   |   Kundens namn    |
|   Skapandedatum för referens  |   Skapandedatum för hänvisning   |
|   Avtalstyp   |   Typ av avtal: samförsäljning, partnerledd, privat |
|   Avtalsriktning  |   Avtalets riktning: Inkommande och utgående    |
|   Avtalsvaluta   |   Avtalets valuta    |
|   Beräknat avtalsvärde    |   Beräknat avtalsvärde som tillhandahålls av partner    |
|   Beräknat avtalsvärde (USD)  |   Beräknat avtalsvärde som tillhandahålls av partner i USD |
|   Lösnings-ID     |   Lista över lösnings-ID |
|   Namn på lösning   |   Lista över lösningsnamnen  |
|   MPN-ID  |   Microsoft-partnerns nätverks-ID för partnern |
|   Partnernamn    |   Partnerns namn |
|   Avtals-ID |   ID för avtalet  |
|   Engagemangs-ID   |   Unikt engagemangs-ID    |
|   Microsoft MSX-ID    |   MSX-ID för avtal  |
|   Skapandedatum för Microsoft-hänvisning    |   Skapandedatum för hänvisning från microsoft |
|   Förnamn för registrerad kontakt   |   Förnamnet på partnerkontakten som angavs under avtalsregistreringen |
|   Efternamn för registrerad kontakt    |   Efternamnet på partnerkontakten som angavs under avtalsregistreringen  |
|   E-postadress för registrerad kontakt    |   E-postadress för partnerkontakt som angavs under avtalsregistreringen  |
|   Registrerat kontakttelefonnummer |   Telefon antal partnerkontakter som angavs under avtalsregistreringen   |
|   Kontraktsvaluta   |   Kontraktsvalutan som angavs under avtalsregistreringen  |
|   Kontraktvärde  |   Totalt kontraktsvärde som angavs under avtalsregistreringen. Detta inkluderar programvaru- och tjänstavgifter men inte maskinvarukostnader  |
|   Kontraktvärde (USD)    |   Totalt kontraktsvärde i USD som angavs under avtalsregistreringen   |
|   Kontraktets startdatum |   Startdatumet för det kontrakt som angavs under avtalsregistreringen    |
|   Slutdatum för kontrakt   |   Slutdatum för det kontrakt som angavs under avtalsregistreringen  |
|   Datum för kontraktstecken  |   Signeringsdatum för det kontrakt som angavs under avtalsregistreringen |
|   Kontrakttyp   |   Typ av kontrakt    |
|   Id för registrerad avtalslösning |   ID för lösning för avtalsregistrering    |
|   Namn på registrerad avtalslösning   |   Namn på lösning för avtalsregistrering  |
|   Registrerad avtalslösningsvaluta   |   Valuta för lösningen som tillhandahålls under avtalsregistreringen |
|   Registrerat avtalslösningsvärde  |   Lösningsvärde som angavs under avtalsregistreringen. I allmänhet är detta det totala kontraktsvärdet minus eventuella icke-återkommande implementeringsavgifter.   |
|   Registrerat avtalslösningsvärde (USD)    |   Lösningsvärde i USD som angavs under avtalsregistreringen |
|   Distribuerad den |   Anger om lösningen har distribuerats i Azure eller andra    |
|   Primär distribution på   |   Anger om lösningen har distribuerats på kundens klientorganisation eller partnerklientorganisation  |
|   Skapandedatum för avtal  |   Skapandedatum för avtalsregistrering  |
|   Datum då avtalet skickades     |   Datum för avtalsregistrering skickades |
|   Avtalsgodkänd/avvisat datum     |   Avtalsgodkänd/avvisat datum. Detta mappas med statuskolumnen. |
|   Amerikanskt federalt avtal |   Anger om det är ett amerikanskt federalt avtal    |
|   Är Marketplace Transacted Deal  |   Anger om det är ett marketplace-avtal    |
|   Marketplace-transaktionsdatum    |   Marketplace-transaktionsdatum om avtalet har transaktionerats på Marketplace|
|   Status      |   Senaste status för hänvisning   |
|   Statusorsak   |   Kommentarer eller orsak till statusen    |
|       |       |
