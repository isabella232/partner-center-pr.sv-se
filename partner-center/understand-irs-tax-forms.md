---
title: Om IRS-skatteformulär som utfärdats av Microsoft
description: Lär dig mer om skatteformulär som utfärdats av Microsoft, inklusive vem som får dem och när de görs tillgängliga.
ms.topic: article
author: mingshen-ms
ms.author: mingshen
ms.service: partner-dashboard
ms.subservice: partnercenter-payouts
ms.localizationpriority: medium
ms.date: 09/30/2020
ms.openlocfilehash: 2e057219696de5eac300f9b6778489e047aceaad
ms.sourcegitcommit: d731813da1d31519dc2dc583d17899e5cf4ec1b2
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/27/2021
ms.locfileid: "129073328"
---
# <a name="understand-irs-tax-forms-issued-by-microsoft"></a>Om IRS-skatteformulär som utfärdats av Microsoft

**Lämpliga roller:** Global administratör

Du kan få ett eller flera skatteformulär från Microsoft varje år. Detta beror på din plats och hur mycket försäljning eller betalningar du får. Microsoft måste utfärda dessa formulär och arkivera dem med Internal Revenue Service (IRS).

Den här artikeln förklarar mer om dessa formulär, inklusive vem som får dem och när de görs tillgängliga.

## <a name="types-of-tax-forms"></a>Typer av skatteformulär

| Skatteformulär för IRS | Description | Tillgänglighet |
|--------------|-------------|--------------|
|1099-MISC, 1099-K | Relaterat till säljaktivitet och/eller betalningar som görs till dig för deltagande på Microsofts marknadsplatser | Utskrivna formulär postmarkeras den **31** januari eller .pdf tillgängliga i partnercentrets utbetalnings- och [skatteprofiler.](https://partner.microsoft.com/dashboard/payee/profiles/partner/manage) |
|1042-S | Relaterade till betalningar som görs till dig och som USA källskatten | Utskrivna formulär publiceras den **15** mars eller tidigare, och .pdf-kopior blir tillgängliga i Partnercenter (i **PartnerCenter Developer Inställningar** under Utbetalnings- och skatteprofiler **för >** Utbetalning och skatt ) samtidigt  |

> [!NOTE]
> Den adress som vi använder på IRS-skatteformulär kommer från adressen i skatteprofilen när du ställer in [ditt utbetalningskonto och skatteformulär](set-up-your-payout-account.md). Om din adress har ändrats ser du till att uppdatera adressen i **skatteprofilen**.

Skatteformulären skickas till dig från följande adresser:

**Amerikanska medborgare:**

| Affärsgrupp         | Juridisk enhet          | Adress                                          |
|------------------------|-----------------------|--------------------------------------------------|
| Windows, Office, Azure | Microsoft Corporation | One Microsoft Way<br>Redmond, WA 98052 USA       |
| Annonsering            | Microsoft Online Inc. | 6880 Sierra Center Parkway<br>Reno, NV 98511 USA |

**Icke-amerikanska medborgare:**

| Affärsgrupp         | Juridisk enhet          | Adress                                          |
|------------------------|-----------------------|--------------------------------------------------|
| Windows, Office, Azure | Microsoft Ireland Operations Limited (betalning görs av Microsoft Corporation via Microsoft Ireland som en kvalificerad mellanhand för Microsoft Corporation) | One Microsoft Place<br>South County Business Park<br>Öje, Dublin 18, D18 P521, Irland|
| Annonsering          | Microsoft Ireland Operations Limited (betalningen görs av Microsoft Online Inc. via Microsoft Ireland och fungerar som utbetalningsagent för Microsoft Online Inc.) | One Microsoft Place<br>South County& Business Park<br>Öje, Dublin 18, D18 P521, Irland |
| Annonsering            | Microsoft Online Inc. | 6880 Sierra Center Parkway<br>Reno, NV 98511 USA |

>[!NOTE]
> \* Medborgare i följande länder som tjänar reklamintäkter kommer att betalas via Microsoft Ireland Operations Limited: Schweiz, Schweiz,Arbet,Arbet, Hälsa, Tjeckiska, Fall, Härska, Frankrike, Tyskland, Nederländska, Nederländska, Irland, Isle of Man, Italien, Let, Eta, 1, 10, 15, 14, 75, 10, 200 000, 200 000

## <a name="for-developers-located-in-the-united-states"></a>För utvecklare som finns i USA

| Om jag är en USA som säljer betalappar och...   | Jag bör få det här formuläret: |
|------------------------|-----------------------|
| Jag hade mer än **200 appförsäljningar** med ett totalt inköpsbelopp för dessa försäljningar som var större än **20 000 USD** under det tillämpliga skatteåret **(räkna** inte försäljningen som gjorts i Brasilien och Kina via Microsoft Store på Windows 10.)| **1099 K:**<br/>Filer: Microsoft Corporation<br/>HAR: \* \* \* \* \* 4442<br/><br/>**Viktigt:** Formulär 1099 K innehåller **bruttoköpsbelopp,** inte betalningar som görs till dig.| 
| Jag har **fått minst 10** USD i betalningar för (i) appförsäljning som gjorts i Brasilien och Kina via Microsoft Store på Windows 10 eller (ii) försäljning på Minecraft Marketplace.<br/><br/>**OR**<br/><br/>Jag fick minst 600 USD i betalningar som inte rör appförsäljning från Microsoft under det tillämpliga skatteåret (till exempel incitamentbetalningar eller betalningar från en deltagare eller befordran)| **1099-MISC:**<br/>Betalare: Microsoft Corporation<br/>HAR: \* \* \* \* \* 4442<br/><br/>**Viktigt:** Vissa affärsenheter får inte formulären 1099-MISC oavsett vilka betalningsbelopp som tas emot från Microsoft.  Kontakta skatteproffset om du vill ha mer information.| 
| Inget av ovanstående gäller.| Ingen |
| <br/><br/>**Om jag är en USA som säljer annonser i appar och...** |<br/><br/>**Jag bör få det här formuläret:** |
|Jag har **fått minst 600 USD i betalningar** från annonser i appar under det tillämpliga skatteåret. | **1099-MISC:**<br/>Betalare: Microsoft Online Inc<br/>HAR: \* \* \* \* \* 0505<br/><br/>**Viktigt:** Vissa affärsenheter får inte formulären 1099-MISC oavsett vilka betalningsbelopp som tas emot från Microsoft.  Kontakta din skatteproffs för mer information. |
| Jag fick **mindre än 600 USD i betalningar** från annonser i appar under det tillämpliga skatteåret. | Ingen |


## <a name="for-developers-located-outside-of-the-united-states"></a>För utvecklare utanför USA


| **Fråga** | **Svar** |
|---|---|
| **Jag har fått ett formulär 1042-S från Microsoft. Vad är det till för?** | Microsoft har försedt dig med ett formulär eller formulär för 1042-S eftersom vi har betalat dig intäkter som anses vara rapportbara för USA-skatteverket och var föremål för källskatt.  Formulär 1042-S används för det här rapporteringskravet. | 
| **Vad ska jag göra med formulären?** | I allmänhet krävs ingen specifik åtgärd från din sida. Formuläret 1042-S kan vara användbart för dig om du vill ansöka om någon form av skattekredit hos dina lokala skattedeklarationer.  Kontakta dina egna skatterådgivare för att få mer information om det här ämnet. | 
| **Varför gjordes skatt på mina betalningar när jag slutförde ett W8-formulär?** | Skatter förser om antingen:<br/><br/>1. Du slutförde inte skatteavsnittet i W8 korrekt, eller <br/>2. Du är hemmahörande i ett land som inte har skatteavtal med USA.<br/><br/>Du kan när som helst besöka Partnercenter för att skicka ett uppdaterat W8-formulär.<br/><br/> **Obs!** Det är inte alla intäkter som omfattas av källskatt. | 
| **Jag skickade ett uppdaterat W8-formulär med giltig information. Kan Microsoft återbetala mig den skatt som förbarbar sig?** | När skatt har tagits med kan den inte återbetalas. Kontakta skatteråden för att diskutera om du kan begära en lokal kredit för dessa skatter eller om du kan begära återbetalning från IRS. | 
| **Vilken försäljning rapporteras i formuläret 1042-S?** | Endast försäljning som gjorts till säljare som finns USA som klassificerats som föremål för **källskatt** kan rapporteras.  All annan försäljning betraktas inte som rapportbar. | 
| **Varför fick jag tre kopior av samma formulär 1042-S i ett kuvert?** | IRS-regler kräver att tre kopior av formuläret tillhandahålls:<br/><br/>– En för mottagarens poster<br/>– En för att skicka in med USA federal skattedeklaration (om tillämpligt)<br/>– En för att skicka USA skattedeklaration (om tillämpligt) |

> [!NOTE]
> Om du har ytterligare frågor eller problem som rör **skatteformulär för IRS** går du till [Hjälp + support på](https://partner.microsoft.com/dashboard/support/) instrumentpanelen i Partnercenter. Microsoft kan inte besvara frågor som rör dina specifika skatteförhållanden; För dessa frågor kan du få råd från din skatteproffs.

## <a name="next-steps"></a>Nästa steg

- [Få betalt på den kommersiella marknadsplatsen](marketplace-get-paid.md)
