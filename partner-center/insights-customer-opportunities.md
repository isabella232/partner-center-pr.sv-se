---
title: Partnercenter Insights – CloudAscent Propensity-rapporter
description: Lär dig mer om cloudAscent Propensity-rapporter i Partnercenter. Innehåller information om en kunds ighet att köpa Microsoft-produkter.
ms.topic: conceptual
ms.service: partner-dashboard
ms.subservice: partnercenter-insights
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 04/27/2021
ms.openlocfilehash: 4248c3d72512073ba361bf1e0ee276a766b04176
ms.sourcegitcommit: 1161d5bcb345e368348c535a7211f0d353c5a471
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/09/2021
ms.locfileid: "123960806"
---
# <a name="cloudascent-propensity-reports-available-from-partner-center-dashboard"></a>CloudAscent Propensity-rapporter som är tillgängliga från instrumentpanelen i Partnercenter

**Lämpliga roller:** Visningsprogram för | Rapportvisningsprogram

Instrumentpanelen i Partnercenter innehåller nedladdningsbara beständiga data från CloudAscent-programmet. Data visar kundernas sannolikhet att köpa Microsoft-produkter.  I den här artikeln beskrivs uppdelningen av dessa data, hur bedömning används och vad det innebär.

## <a name="summary-definitions"></a>Sammanfattningsdefinitioner

- **SMC-kunder**– Det här är det totala antalet kunder som har ighetsnedladdningar.  Kunder identifieras av en postpartner.
- **Upphör att** gälla – Under det aktuella räkenskapsåret tillhandahåller vi antalet utgångna avtal.
- **Öppna Förfallande intäkter**– De intäkter som är associerade med de öppna utgångna avtalen.

:::image type="content" source="images/insights/customer-opportunity-1.png" alt-text="Skärmbild av instrumentpanelen Sammanfattning av kundmöjligheter.":::

## <a name="cloudascent-smb-segmentation"></a>CloudAscent SMB-segmentering

SMB-segmentet (small to medium business) är indelat i tre distinkta delsegment.

1. **De mest ohanterade** innehåller de största SMB-kunderna med flest möjligheter för Microsoft. Vanliga kunder som inte är mest ohanterade har liknande egenskaper som hanterade konton, med ett stort antal anställda, stora IT-budgetar och -utgifter samt stora mängder potentiella intäkter för Microsoft.

   Vi definierar Top Unmanaged på två sätt:

   - **Top Unmanaged User Based**– innehåller konton med 300 eller fler anställda. User-Based-konton är bra mål för första köp eller expansion av användarbaserade prenumerationsprodukter som Microsoft 365, Dynamics 365 eller Surface.
   - **Högsta ohanterade beräkningsbaserad –** innehåller konton med en potentiell Azure-användning som är större än 10 000 USD. Beräkningsbaserade konton omfattar befintliga Azure. konton med betydande framtida års potential och konton som ännu inte har köpt Azure men som har potential för Azure som är större än 10 000 USD.

2. **Medium Business** innehåller befintliga kunder och potentiella konton med 25 till 300 anställda.

3. **Små företag** omfattar företag med 10–25 anställda.

4. **I Very Small Business** finns företag med 1–9 anställda.

:::image type="content" source="images/insights/customer-opportunity-2.png" alt-text="Kund efter SMC-typ.":::

**De främsta undersegmenten** **för** ohanterade och medelstora företag representerar LTV-kunder (High Life-Time Value) för Microsoft och Microsoft-partner. Därför är de huvudfokusområden för att driva tillväxt i det här segmentet. I dessa två undersegment är vi bättre positionerade för att skaffa socketen med Microsoft 365, tjäna pengar ytterligare med D365-/Azure LOB-appar och få en hög LTV för Microsoft.

Idag har vi två viktiga affärsmöjlighetsområden – 1. vår kund ökar tillväxten; 2. Även om vi har ett bra sätt att skaffa molnsocketar som leder Microsoft 365, har vi en stor möjlighet i Dynamics 365 och Azure.

Följande skärmbild representerar de fyra SMB-undersegmenten. CloudAscent prioriterar profilering, bedömning och modellering av alla konton i de främsta ohanterade och medelstora verksamhetskontona.

:::image type="content" source="images/insights/customer-opportunity-3.png" alt-text="Skärmbild av SMB-undersegment.":::

## <a name="cloudascent-machine-learning"></a>CloudAscent Machine Learning

SMB använder maskininlärningsteknik för att driva kundförutsägelser för försäljning och marknadsföring i de viktigaste segmenten för ohanterade och medelstora företag. Hur samlas signaler in och omvandlas till rekommendationer om rekommendationer för rekommendationer?

- **Datainsamling:** Webb crawlers söker igenom och samlar in miljarder kundsignaler genom att pinga företagsdomänerna och övervaka blogginlägg, pressutgåor, sociala strömmar och tekniska forum.  Förutom insamlade signaler samlas företagsinformation in från både interna och externa källor, till exempel D&B, Microsoft Internal-prenumeration och transaktionsdata.

- **Machine Learning:** Signalerna matas in i maskininlärningsmodellen som matar ut en strukturerad datauppsättning med försäljnings- och marknadsföringsförutsägelser för varje kund efter molnprodukt och kluster.  Varje kund poängsätts med hjälp av en modell av samma utseende som Microsofts främsta SMB som avgör kundens anpassa, och maskininlärningsalgoritmer som integrerar kundens onlinebeteende definieras som avsikt. Poängen slås samman i kluster som visar en kunds ighet att köpa Microsoft Cloud Products.

- **Optimering:** Machine Learning optimerar modellerna genom att använda transaktionsdata månadsvis och prenumerationsdata kvartalsvis.  Med hjälp av win/loss-data justerar Machine Learning algoritmerna och verifierar att modellerna fungerar som förväntat genom att jämföra klusterrekommendationer med affärsmöjligheter som åtgärdats i MSX.

:::image type="content" source="images/insights/customer-opportunity-4.png" alt-text="Skärmbild av SMB-maskininlärning.":::

## <a name="cloudascent-propensity"></a>CloudAscent-propensitet

Hur skapas rekommendationer för rekommendationer om rekommendationer för rekommendationer?

Med hjälp av signaler som samlas in via webb crawlers och data från olika källor konsoliderar vi företagets data och kundens sociala mediesignaler.  Poängsättningen använder dessa signaler och data i jämförelsemodeller för anpassa och bedömningsmodeller för avsikt.

1. Anpassa kundkonto

   - Interna och externa datapunkter som definierar företagsgrafiska data.

   - Bedömning av passningar använder en modell som ser likadan ut för vår bästa SMB för att jämföra kunder och se om de är lämpliga för Microsoft Cloud Products.

   - Bedömning av passning uppdateras kvartalsvis

2. Avsikt för kundkonto

   - Signaler som rör sociala medier och en kunds onlinebeteende definierar Intent.

   - Avsiktsbedömningen överlagras ovanpå passning för att definiera klustren.

   - Avsiktsbedömningen uppdateras varje månad.

   :::image type="content" source="images/insights/customer-opportunity-5.png" alt-text="CloudAscent SMB-förutsägelsemodeller.":::

3. Klustring

   Signalerna för passning och avsikt konsolideras till en klustringspoäng. CloudAscent har fyra kluster:

      - Agera nu – kunder som är redo för försäljning
      - Utvärdera – marknadsföringsklara kunder
      - Vård – främja medvetenhetskampanjer
      - Utbilda – utbilda och övervaka avsikter

   Klustringen gör att användare kan rikta in sig på specifika kunder för sälj- och marknadsföringsinitiativ baserat på segmentfaktorer, till exempel produkt, geo, bransch och vertikal.

   Fliken **Propensity model (Propensity Model)** i CloudAscent-arbetsböcker delar heten och de beräknade utrymmesintäkterna. För att definiera klustringen av Anpassa och Avsikt går vi igenom följande steg:

      1. Med ML-modeller beräknar vi först kundpoäng och avsiktspoäng på en skala på 100.  Exakta poäng varierar beroende på ML modeller.  Exempelresultat nedan:

         |**Klassificering**|**Poäng**|
         |---------|:---------|
         |Högt|75 - 100|
         |Medel|55 - 74|
         |Låg|30 - 54|
         |Mycket låg|0 - 29|

      2. Med hjälp av regeln ovan klassificerar vi företag som Hög, Medel, Låg och Mycket låg för både Customer Fit och Intent Signals.

      3. Vi ritar kundpassnings- och avsiktssignaler på en 2D-matris där varje skärningspunkt representerar återgivningen. Till exempel hög passning + hög avsikt = A1, som representerar den högsta återgivningen.

      4. Slutligen grupperar dessa segment för att bilda kluster.  Till exempel, A1, A2, A3 och A4 utgör act now-klustret.

         :::image type="content" source="images/insights/customer-opportunity-6.png" alt-text="CloudAscent-modeller.":::

   För dessa kunder rekommenderar vi att du riktar in dig på Agera nu och Utvärdera kunder.

## <a name="cloudascent-products--models"></a>CloudAscent Products & Models

Följande bild visar en vy över varje stående modell i CloudAscent:

:::image type="content" source="images/insights/customer-opportunity-7.png" alt-text="CloudAscent-ighetsmodell.":::

Tomt utrymmesmodeller består av förutsägelser för befintliga Microsoft-kunder där de inte har en produkt och/eller är netto nya kunder.

Modeller för merförsäljning använder transaktionsdata för att förutsäga potentialen för merförsäljning i Azure och Microsoft 365 SKU:er.

Dessa kunder kommer redan att ha både Azure Microsoft 365 och modellen för merförsäljning visar att de sannolikt kommer att köpa mer av sin befintliga SKU.

EOS delar EOS-kunder (end of service) för Win 7, Office 2010, SQL Server och Windows Server. EOS-data hämtas från MS Sales och överlagras med CloudAscent propensity modeling där det är tillgängligt. EOS-data finns i Modern Work och Azure Sales spelar.
