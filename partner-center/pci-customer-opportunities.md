---
title: Partner Center-insikter – Rapporter om molnocent- sida
description: Lär dig mer om cloudAscent Propensity-rapporter i Partnercenter. Innehåller information om en kunds ighet att köpa Microsoft-produkter.
ms.topic: conceptual
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 04/27/2021
ms.openlocfilehash: 430aea81964d1b75514b6e1377bd2ba1af41b538
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 05/19/2021
ms.locfileid: "110153046"
---
# <a name="cloudascent-propensity-reports-available-from-partner-center-dashboard"></a>CloudAscent Propensity-rapporter som är tillgängliga från instrumentpanelen i Partnercenter

**Lämpliga roller:** Användare av | Rapportvisningsprogram

Instrumentpanelen i Partnercenter innehåller nedladdningsbara beständiga data från CloudAscent-programmet. Data visar kundernas sannolikhet att köpa Microsoft-produkter.  I den här artikeln beskrivs analys av dessa data, hur bedömning används och vad det innebär.

## <a name="summary-definitions"></a>Sammanfattningsdefinitioner

- **SMC-kunder**– Det här är det totala antalet kunder som har ighetsnedladdningar.  Kunder identifieras av en postpartner.
- **Upphör att** gälla – Under det aktuella räkenskapsåret tillhandahåller vi antalet utgångna avtal.
- **Öppna Förfallande intäkter**– De intäkter som är associerade med de öppna utgångna avtalen.

:::image type="content" source="images/pci/cust-oppor-11.png" alt-text="Skärmbild av instrumentpanelen Sammanfattning av kundmöjligheter.":::

## <a name="cloudascent-smb-segmentation"></a>CloudAscent SMB-segmentering

SMB-segmentet (small to medium business) är indelat i tre distinkta delsegment.

1. **De största ohanterade innehåller** de största SMB-kunderna med flest möjligheter för Microsoft. Vanliga kunder som inte är mest ohanterade har liknande egenskaper som hanterade konton, med ett stort antal anställda, stora IT-budgetar och -utgifter samt stora mängder potentiella intäkter för Microsoft.

   Vi definierar Top Unmanaged på två sätt:

   - **Top Unmanaged User Based**– innehåller konton med 300 eller fler anställda. User-Based-konton är bra mål för första gången köp eller expansion av användarbaserade prenumerationsprodukter som Microsoft 365, Dynamics 365 eller Surface.
   - **Top Unmanaged Compute Based –** innehåller konton med azure-potential som är större än 10 000 USD. Beräkningsbaserade konton omfattar befintliga Azure. konton med betydande framtida års potential och konton som ännu inte har köpt Azure men som har potential för Azure som är större än 10 000 USD.

2. **Medium Business** innehåller befintliga kunder och konton för potentiella kunder med 25 till 300 anställda.

3. **Små företag** omfattar företag med 10–25 anställda.

4. **I Very Small Business** finns företag med 1–9 anställda.

:::image type="content" source="images/pci/cust-oppor-2.png" alt-text="Kund efter SMC-typ.":::

**De främsta delsegmenten för** ohanterade och medelstora företag representerar LTV-kunder (High Life-Time Value) för Microsoft och Microsoft-partner.  Därför är de de viktiga fokusområdena för att öka tillväxten i det här segmentet. I dessa två undersegment är vi bättre positionerade för att skaffa socketen med Microsoft 365, tjäna pengar ytterligare med D365-/LOB-appar (LOB) för Azure och realisera en hög LTV för Microsoft.

Idag har vi två viktiga affärsmöjlighetsområden – 1. vår kund ökar tillväxten; 2. Även om det går bra att skaffa molnsocketar som leder Microsoft 365, har vi stora möjligheter i Dynamics 365 och Azure.

Följande skärmbild representerar de fyra SMB-undersegmenten. CloudAscent prioriterar profilering, bedömning och modellering av alla konton i de främsta ohanterade och medelstora företagarna.

:::image type="content" source="images/pci/cust-oppor-32.png" alt-text="Skärmbild av SMB-undersegment.":::

## <a name="cloudascent-machine-learning"></a>CloudAscent Machine Learning

SMB använder maskininlärningsteknik för att driva kundförutsägelser för försäljning och marknadsföring inom de viktigaste segmenten ohanterade och medelstora företag. Hur samlas signaler in och omvandlas till rekommendationer om benägenhet?

- **Datainsamling:** Webbrobotar söker igenom och samlar in miljarder kundsignaler genom att pinga företagsdomänerna och övervaka blogginlägg, pressutgåor, sociala strömmar och tekniska forum.  Förutom insamlade signaler samlas företagsinformation in från både interna och externa källor som D&B, Microsoft Internal-prenumeration och transaktionsdata.

- **Machine Learning:** Signalerna matas in i maskininlärningsmodellen som matar ut en strukturerad datauppsättning med försäljnings- och marknadsföringsförutsägelser för varje kund efter molnprodukt och kluster.  Varje kund poängeras med en modell av samma utseende som Microsofts främsta SMB som avgör kundens Anpassa, och maskininlärningsalgoritmer som integrerar kundens onlinebeteende definieras som Avsikt. Poängen sammanfogas i kluster som visar en kunds önskemål om att köpa Microsoft Cloud Products.

- **Optimering:** Machine Learning optimerar modellerna genom att använda transaktionsdata varje månad och prenumerationsdata kvartalsvis.  Med hjälp av win/loss-data justerar Machine Learning algoritmerna och verifierar att modellerna fungerar som förväntat genom att jämföra klusterrekommendationerna med affärsmöjligheter som åtgärdas i MSX.

:::image type="content" source="images/pci/cust-oppor-4.png" alt-text="Skärmbild av SMB-maskininlärning.":::

## <a name="cloudascent-propensity"></a>CloudAscent-ständiga

Hur skapas rekommendationer för rekommendationer om rekommendationer för rekommendationer?

Med hjälp av signaler som samlas in via webb crawlers och data från olika källor konsoliderar vi företagets data och kundens signaler på sociala medier.  Poängen använder dessa signaler och data i jämförelsemodeller för anpassa och bedömningsmodeller för avsikt.

1. Anpassa kundkonto

   - Interna och externa datapunkter som definierar företagsgrafiska data.

   - Fit scoring använder en modell av samma utseende som vår bästa SMB för att jämföra kunder och se om de är lämpliga för Microsoft Cloud Products.

   - Bedömning av passning uppdateras kvartalsvis

2. Avsikt för kundkonto

   - Signaler relaterade till sociala medier och en kunds onlinebeteende definierar Intent.

   - Avsiktsbedömningen överlagras ovanpå passning för att definiera klustren.

   - Avsiktsbedömningen uppdateras varje månad.

   :::image type="content" source="images/pci/cust-oppor-5.png" alt-text="CloudAscent SMB-förutsägelsemodeller.":::

3. Klustring

   Signalerna för passning och avsikt konsolideras till en klustringspoäng. CloudAscent har fyra kluster:

      - Agera nu – kunder som är redo för försäljning
      - Utvärdera – marknadsföringsklara kunder
      - Vård – främja medvetenhetskampanjer
      - Utbilda – utbilda och övervaka avsikter

   Klustringen gör att användare kan rikta in sig på specifika kunder för sälj- och marknadsföringsinitiativ baserat på segmentfaktorer, till exempel produkt, geo, bransch och vertikal.

   Fliken **Propensity model (Propensity Model)** i CloudAscent-arbetsböcker delar heten och de beräknade utrymmesintäkterna. För att definiera klustringen av Anpassa och Avsikt går vi igenom följande steg:

      1. Med hjälp av ML-modeller beräknar vi först kundpoäng och avsiktspoäng på en skala på 100.  Exakta poäng varierar beroende på ML-modeller.  Exempelresultat nedan:

         |**Klassificering**|**Poäng**|
         |---------|:---------|
         |Högt|75 - 100|
         |Medel|55 - 74|
         |Låg|30 - 54|
         |Mycket låg|0 - 29|

      2. Med hjälp av regeln ovan klassificerar vi företag som Hög, Medel, Låg och Mycket låg för både Customer Fit och Intent Signals.

      3. Vi ritar kundens passnings- och avsiktssignaler på en 2D-matris där varje skärningspunkt representerar återgivningen. Till exempel hög passning + hög avsikt = A1, som representerar den högsta återgivningen.

      4. Slutligen grupperar dessa segment för att bilda kluster.  A1, A2, A3 och A4 utgör till exempel Act Now-klustret.

         :::image type="content" source="images/pci/cust-oppor-6.png" alt-text="CloudAscent-modeller.":::

   För dessa kunder rekommenderar vi att du riktar in dig på Agera nu och Utvärdera kunder.

## <a name="cloudascent-products--models"></a>CloudAscent Products & Models

Följande bild visar en vy över varje benägenhetsmodell i CloudAscent:

:::image type="content" source="images/pci/cust-oppor-7.png" alt-text="CloudAscent-benägenhetsmodell.":::

Blankstegsmodeller består av förutsägelser för befintliga Microsoft-kunder där de inte har någon produkt och/eller är netto nya kunder.

Modeller för merförsäljning använder transaktionsdata för att förutsäga potentialen för merförsäljning i Azure och Microsoft 365 SKU:er.

Dessa kunder kommer redan att ha både Azure Microsoft 365 och uppförsäljningsmodellen visar att de sannolikt kommer att köpa mer av sin befintliga SKU.

EOS delar EOS-kunder (End of Service) för Win 7, Office 2010, SQL Server och Windows Server. EOS-data hämtas från MS Sales och överlagras med CloudAscent-modellering där det är tillgängligt. EOS-data finns i Modern Work och Azure Sales spelar.
