---
title: Partner Center Insights – CloudAscent benägenhet-rapporter
description: Lär dig mer om CloudAscent benägenhet-rapporter i Partner Center. Innehåller information om en kunds benägenhet för att köpa Microsoft-produkter.
ms.topic: conceptual
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 09/18/2020
ms.openlocfilehash: 2cdb63c8f7e29fc8a56e920b587e47c382c6eacb
ms.sourcegitcommit: 10765386b2df0d4c2e8da9b302a692f452e1090d
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/31/2021
ms.locfileid: "106086965"
---
# <a name="cloudascent-propensity-reports-available-from-partner-center-dashboard"></a>CloudAscent benägenhet-rapporter som är tillgängliga från instrument panelen för partner Center

**Lämpliga roller**

- Rapport visnings program för chefer
- Rapport visnings program

Instrument panelen för partner Center innehåller nedladdnings bara benägenhet-data från CloudAscent-programmet. Data visar kundernas benägenhet för att köpa Microsoft-produkter.  Den här artikeln beskriver hur du analyserar data, hur du använder den och vad det innebär.

## <a name="summary-definitions"></a>Sammanfattnings definitioner

- **SMC-kunder**– detta är det totala antalet kunder i benägenhet nedladdning.  Kunderna identifieras av en partner av posten.
- **Avtalet upphör** att gälla – inom innevarande räkenskapsår tillhandahåller vi antalet avtals engångs avtal.
- **Förfallo datum för intäkter**– den intäkt som är kopplad till avtalets upphör Ande.
- **Öppna förfallo** datum för intäkt – intäkten som är kopplad till Open agreementd-avtal.

:::image type="content" source="images/pci/cust-oppor-1.png" alt-text="Skärm bild av instrument panelen Sammanfattning av kund möjligheter.":::

## <a name="cloudascent-smb-segmentation"></a>CloudAscent SMB-segmentering

Det lilla till mellanliggande segmentet (SMB) är indelat i tre distinkta del segment.

1. De mest **ohanterade** innehåller de största SMB-kunderna med flest möjligheter för Microsoft. Vanliga ohanterade kunder delar liknande egenskaper som hanterade konton, med ett stort antal anställda, stora IT-budgetar och utgifter och stora mängder potentiella intäkter för Microsoft.

   Vi definierar de vanligaste ohanterade två sätten:

   - **Topp ohanterad användare baserad**– inkluderar konton med 300 eller fler anställda. User-Based konton är bra mål för första inköpet, eller en utbyggnad av användarbaserade prenumerations produkter som Microsoft 365, Dynamics 365 eller Surface.
   - **Topp ohanterad beräkning baserad** – innehåller konton med Azure-potential som är större än $10 000. Compute-baserade konton inkluderar befintliga Azure. konton med betydande framtida års potential och konton som ännu inte har köpt Azure men som har potential för Azure större än $10 000.

2. **Medel stora företag** inkluderar befintliga kunder och kund konton med 25 till 300 anställda.

3. **Små företag** omfattar alla återstående företag med färre än 25 anställda.

:::image type="content" source="images/pci/cust-oppor-2.png" alt-text="Kund av SMC-typ.":::

**De främsta** del segmenten med ohanterade och **medel stora företag** representerar höga LTV-kunder (Life-Time-Time) för Microsoft och Microsoft-partner. Därför är de de ledande områdena i fokus för att öka tillväxten i det här segmentet. I de här två del segmenten har vi bättre möjligheter att förvärva socketen med Microsoft 365, köpa ytterligare med D365/Azure line of Business (LOB)-appar och inse en hög LTV för Microsoft.

Idag har vi två viktiga områden i affärs möjligheten – 1. vår kund ökar tillväxten; 11.2. Vi har också bra att köpa moln platser som leder till Microsoft 365, men vi har en stor möjlighet i D365 och Azure.

Följande skärm bild visar de tre SMB-undersegmenten och optimerade vägar till marknaden. CloudAscent prioriterar profileringen, poängsättningen och modelleringen av alla topp ohanterade och medel stora företags konton.

:::image type="content" source="images/pci/cust-oppor-3.png" alt-text="Skärm bild av SMB-undersegment.":::

## <a name="cloudascent-machine-learning"></a>CloudAscent Machine Learning

SMB använder maskin inlärnings teknik för att driva försäljnings-och marknadsförings kund förutsägelser inom de högsta ohanterade och medel stora affärs segmenten. Hur samlas signaler in och omvandlas till benägenhet-rekommendationer?

- **Data insamling**: webbcrawler genomsöker och samlar in miljarder kund signaler genom att skicka ping till företagets domäner och övervakning: blogg inlägg, pressmeddelanden, sociala data strömmar och tekniska forum.  Utöver de insamlade signalerna samlas firmographics information in från både interna och externa källor som D&B, Microsoft intern prenumeration och transaktions data.

- **Machine Learning**: signalerna matas in i Machine Learning-modellen som ger en strukturerad data uppsättning av försäljnings-och marknadsförings förutsägelser för varje kund enligt moln produkt och-kluster.  Varje kund betygs ätter en valfri modell till Microsofts främsta SMB som fastställer kundens anpassnings-och Machine Learning-algoritmer som integrerar kundens beteende för online-beteendet. Poängen slås samman i kluster som visar en kunds benägenhet att köpa Microsoft Cloud produkter.

- **Optimering**: Machine Learning systemet optimerar modellerna genom att förbruka transaktions data varje månad och prenumerations data kvartals vis.  Med hjälp av vinst-/förlust data justerar Machine Learning algoritmerna och validerar att modellerna fungerar som förväntat genom att jämföra kluster rekommendationer med affärs möjligheter som har bearbetats i MSX.

:::image type="content" source="images/pci/cust-oppor-4.png" alt-text="Skärm bild av SMB Machine Learning.":::

## <a name="cloudascent-propensity"></a>CloudAscent benägenhet

Hur skapas benägenhet-rekommendationer?

Genom att använda signaler som samlats in via webbcrawler och data från olika källor konsoliderar vi firmographics-data och kundens sociala medie signaler.  Poängen använder dessa signaler och data i jämförelse modeller för anpassningar och bedömnings modeller för avsikten.

1. Kund konto passning

   - Interna och externa data punkter som definierar firmographics.

   - Anpassnings bedömnings använder en modell som liknar vår bästa SMB för att jämföra kunder och se om de är en potentiell anpassning för Microsoft Cloud produkter.

   - Anpassnings resultat uppdateras varje kvartal

2. Avsikt för kund konto

   - Signaler som rör sociala medier och en kunds beteende för online-beteende definierar avsikt.

   - Poängen för avsikten är överordnad för att definiera klustren.

   - Avsikts poängen uppdateras varje månad.

   :::image type="content" source="images/pci/cust-oppor-5.png" alt-text="CloudAscent SMB förutsägande modeller.":::

3. Klustring

   Signalerna för passa och avsikten samlas in i ett kluster poäng. CloudAscent har fyra kluster:

      - Handla nu – försäljnings klara kunder
      - Utvärdera – marknadsförings klara kunder
      - Nurture – disk medvetenhets kampanjer
      - Utbilda – utbilda och övervaka för avsikt

   Med klustringen kan användarna rikta in sig på specifika kunder för försäljnings-och marknadsförings initiativ baserat på segment faktorer, till exempel: produkt, geo, bransch och vertikal.

   Fliken **benägenhet modell** i arbets böckerna CloudAscent delar benägenhet och den beräknade intäkten på tomt utrymme. Vi går igenom följande steg för att definiera klustring av anpassning och avsikt:

      1. Med hjälp av ML-modeller beräknar vi först kund anpassnings poängen och avsikts poängen på en skala på 100.  Exakta resultat varierar beroende på ML-modeller.  Exempel resultat nedan:

         |**Klassificering**|**Resultat**|
         |---------|:---------|
         |Högt|75 – 100|
         |Medel|55 – 74|
         |Låg|30 - 54|
         |Mycket låg|0 - 29|

      2. Med regeln ovan klassificerar vi företag som hög, medel, låg och mycket låg i både kund anpassningar och avsikts signaler.

      3. Vi åker kundernas passnings-och avsikts signaler på en 2D-matris med varje skärnings punkt som representerar benägenhet. Till exempel hög passning + hög avsikt = a1 som representerar den högsta benägenhet.

      4. Slutligen är segment gruppen till att bilda kluster.  Till exempel a1, a2, A3, A4 form fungerar nu-klustret.

         :::image type="content" source="images/pci/cust-oppor-6.png" alt-text="CloudAscent-modeller.":::

   För dessa kunder rekommenderar vi att du riktar in dig på målet och utvärderar kunderna.

## <a name="cloudascent-products--models"></a>CloudAscent-produkter & modeller

Följande bild visar en vy över varje benägenhet-modell i CloudAscent:

:::image type="content" source="images/pci/cust-oppor-7.png" alt-text="CloudAscent benägenhet-modell.":::

Blank stegs modeller består av förutsägelser för befintliga Microsoft-kunder där de inte har en produkt och/eller är kunder med nya kunder.

Merförsäljning-modeller använder transaktions data för att förutsäga potentialen för merförsäljning i Azure och Microsoft 365 SKU: er.

EOS delar tjänst kundernas slut för Windows 7, Office 2010, SQL Server och Windows Server. EOS-data hämtas från MS Sales och överlappar med CloudAscent benägenhet-modellen där det är möjligt. EOS data liv i det moderna arbetet och Azure Sales spelar.
