---
title: Data definitioner för insikter
ms.topic: article
ms.date: 12/14/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Dokumentet innehåller en lista över olika rapporter och data definitioner för varje rapport, som kan hämtas från rapport sidan för insikter.
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: d4a805957fac7c7cff373d807347b7c6d0b13d6f
ms.sourcegitcommit: 4e36d1a4ca2f074b55f9b9a08e300734eae1f06d
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 12/15/2020
ms.locfileid: "97502133"
---
# <a name="export--data-definitions"></a>Exportera – data definitioner 

 **Lämpliga roller** 

- Rapport visnings program 
- Rapport visnings program för chefer 

## <a name="introduction"></a>Introduktion 

Med hubben för att ladda ned rapporter i insikts instrument panelen kan du exportera rå data uppsättningar.  

De olika rapporterna, som kan hämtas tillsammans med data definitionen, är följande: 

**Partner profil**: data definitionerna för de olika fälten i profil rapporten är: 


| **Kolumn namn** | **Data Beskrivning** |
|---------|:---------|
|MPNId|Microsoft Partner Network-ID|
|PartnerName|Partnerns namn |
|PGA_MPNId|Partner globalt konto MPN-ID|
|PGA_PartnerName|Globalt konto namn för partner|
|City|Ortens plats för partner |
|Land|Partnerns land plats |
|HierarchyLevel|Anger om det är ett globalt MPN-ID eller platsens MPN-ID|

**Kund information**: data definitionerna för de olika fälten i rapporten kund information är:

| **Kolumn namn** | **Data Beskrivning** |
|---------|:---------|
|CustomerName|Namnet på kunden |
|CustomerTenantId|Kundens klientorganisations-ID |
|CustomerTpid|Överordnad kund topp identifierare |
|CustomerSegment|Kund segment |
|CustomerMarket|Den geografiska marknaden för kunden  |
|CustomerStatus|Kund status (aktiv/inactive) |
|Produkt|Produkten som säljs till kunden av MPN. Det här är en av O365, D365, Enterprise Mobility, Power BI Microsoft Azure.|
|SKU|   Produkt-SKU|
|Månad| Månad för vilken användning och intäkt rapporteras|
|MPNId| Microsoft Partner Network-ID|
|PartnerName|   Partnerns namn|
|PartnerLocation|   Partnerns geografiska plats|
|PartnerAttributionType|    Tilldelnings typ för partner|
|SalesChannel|  Försäljnings kanal|
|AvailableSeats|    Tillgängliga platser| 
|RevenueUSD|    Intäkter i USD|

**Åter försäljarens prestanda**: data definitionerna för de olika fälten i prestanda rapporterna för åter försäljare är:

> [!Note]
> Intäkts-och ACR-data är bara tillgängliga för användare som har rapport visnings program för chefer.

| **Kolumn namn** | **Data Beskrivning** |
|---------|:---------|
|ResellerMpnid|Microsoft Partner Network identifierare för åter försäljare| 
|ResellerName|Åter försäljarens namn|
|ResellerMarket|Åter försäljar land på marknaden| 
|IndirectProviderMPNId|ID för indirekt Provider Microsoft Partner Network|
|IndirectProviderName|Namn på indirekt Provider|
|Månad|Månad för vilken användning och intäkt rapporteras|
|Produkt|Produktnamn|
|SubscriptionID|Prenumerations-ID|
|AvailableSeats|Antal tillgängliga platser|
|AssignedSeats|Antal tilldelade platser|
|BilledRevenueUSD|Fakturerad intäkt (i kr)|
|CustomerName|Namnet på kunden| 
|CustomerTPid|Överordnad kund topp identifierare| 
|CustomerSegment|Kund segment |
|CustomerMarket|Den geografiska marknaden för kunden |
|ResellerStatus|Status för åter försäljare| 

**Prenumerations information**: data definitionerna för de olika fälten i prenumerations informations rapporten är:

>[!Note]
>Intäkts-och ACR-data är bara tillgängliga för användare som arbetar med rapport visnings program för chefer

| **Kolumn namn** | **Data Beskrivning** |
|---------|:---------|
|SubscriptionId|    GUID för prenumerationen|
|SubscriptionStartDate| Start datum för prenumerationen|
|SubscriptionEndDate|   Slutdatum för prenumerationen|
|SubscriptionState| Status för prenumerationen (aktiv eller överomsättningen)|
|Månad| Månad för vilken användning och intäkt rapporteras|
|IsAutoRenew|   Anger om prenumerationen är automatisk förnyelse eller inte (j/N)|
|CustomerName|  Kundnamn| 
|CustomerTenantId|  Kund-GUID|
|CustomerTpid|  Överordnad kund topp identifierare| 
|CustomerSegment|   Marknads segment för kunden| 
|CustomerMarket|    Den geografiska marknaden för kunden|
|Produkt|   Produkt som säljs till kunden av partnern| 
|SKU|   Produkt-SKU för produkten |
|MPNId| Partnerns Microsoft Partner Network-ID |
|PartnerName|   Partnerns namn |
|PartnerLocation|   Partnerns geografiska plats |
|PartnerAttributionType|    Tilldelnings typ för prenumerationen|
|SalesChannel|  Försäljnings kanal (direkt/CSP osv.) |
|AvailableSeats|    Aktuellt tillgängligt säte|
|RevenueUSD|    Intäkter i USD|
|Registrerings-ID| Registrerings-ID för prenumerationen|

**Azure-användning**: data definitionerna för de olika fälten i Azure-användnings rapporten är:

| **Kolumn namn** | **Data Beskrivning** |
|---------|:---------|
|SubscriptionId|    GUID för prenumerationen|
|SubscriptionStartDate| Datumet då prenumerationen startades.|
|SubscriptionEndDate|   Det datum då prenumerationen slutar.|
|SubscriptionState| Aktuellt tillstånd för prenumerationen (öppen/stängd/aktiv/inrespitperiod)|
|Månad| Datum sammanställt per månad |
|ServiceName|   Namnet på Azure-tjänsten|
|MeterCategory| Namn på mätar kategorin|
|UsageUnits|    Antalet enheter som används under fakturerings perioden |
|CustomerName|  Namnet på kunden |
|CustomerTenantId|  Klient-ID för kund |
|CustomerTpid|  Överordnad kund topp-ID |
|CustomerSegment|   Kunds segment |
|CustomerMarket|    Den geografiska marknaden för kunden |
|MPNId  |Microsoft Partner Network-ID för kunden |
|PartnerName|   Partnerns namn |
|PartnerLocation    |Den geografiska land platsen för partnern |
|PartnerAttributionType |Tilldelnings typ för partner|
|SalesChannel|  Försäljnings kanal (direkt/CSP indirekt/CSP Direct osv.) |
|ACR_USD|   Förbrukade Azure-intäkter i USD|
|Registrerings-ID| Registrerings-ID för Azure-prenumerationen|

**Office 365 – licens användning**: data definitionerna för de olika fälten i rapporten Office 365 – licens användning är:

| **Kolumn namn** | **Data Beskrivning** |
|---------|:---------|
|CustomerTenantId|  Klient-ID för kund| 
|CustomerTpid|  Överordnad kund topp-ID |
|WorkloadName|  SFB, teams, EXO |
|Månad| Månad för vilken användning rapporteras|
|PaidAvailableUnits|    Antal betalda tillgängliga enheter|
|MonthlyActiveUsers|    Antal aktiva användare per månad|
|CustomerName|  Namnet på kunden|
|CustomerMarket|    Geografisk marknads plats för kunden |
|CustomerSegment|   Kund segment |
|MPNId| Microsoft Partner Network-ID|
|PartnerName|   Partnerns namn|
|PartnerLocation|   Partnerns geografiska plats|
|PartnerAttributionType|    Tilldelnings typ för partner|

**Enterprise Mobility – licens användning**: data definitionen för de olika fälten i EMS – licens användnings rapporten är:

| **Kolumn namn** | **Data Beskrivning** |
|---------|:---------|
|CustomerTenantId|  Klient-ID för kund| 
|CustomerTpid|  Överordnad kund topp-ID |
|WorkloadName|  Namnet på EMS-arbetsbelastningen |
|Månad| Månad för vilken användning rapporteras|
|PaidAvailableUnits|    Antal betalda tillgängliga enheter|
|MonthlyActiveUsers|    Antal aktiva användare per månad|
|CustomerName|  Namnet på kunden|
|CustomerMarket|Geografisk marknads plats för kunden |
|CustomerSegment|   Kund segment |
|MPNId| Microsoft Partner Network-ID|
|PartnerName|   Partnerns namn|
|PartnerLocation|   Partnerns geografiska plats|
|PartnerAttributionType|    Tilldelnings typ för partner|

**Dynamics 365 – licens användning**: data definitionen för de olika fälten i Dynamics 365 – licens användnings rapporten är:

| **Kolumn namn** | **Data Beskrivning** |
|---------|:---------|
|SubscriptionId|GUID för prenumerationen|
|SubscriptionStartDate| Start datum för prenumerationen|
|SubscriptionEndDate|   Slutdatum för prenumerationen|
|SubscriptionStatus|    Status för prenumerationen |
|Månad| Månad för vilken användning rapporteras|
|RevSumDivisionName|    Namn på rev sum-divisionen|
|RevSumCategoryName|    Namnet på rev sum-kategorin|
|SKU|   Produkt-SKU för produkten |
|SKUId| SKU-ID för produkten |
|FreeVsPaidSKU| Anger om det är en kostnads fri eller betald SKU |
|SalesModel|    Försäljnings kanal som används för att sälja prenumerationen|
|DetailedSalesModel|    Detaljerad försäljnings modell för prenumerationen|
|CustomerName|  Kundnamn |
|CustomerTenantId|  GUID för kund klient organisation |
|CustomerTpid|  Överordnad kund topp identifierare |
|CustomerSegment|   Marknads segment för kunden |
|CustomerMarket|    Den geografiska marknaden för kunden |
|MPNId| Microsoft partner nätverks-ID |
|PartnerName|   Partnerns namn |
|PartnerLocation|   Den geografiska land platsen för partnern |
|PartnerAttachType| Tilldelnings typ för prenumerationen|
|AvailableSeats|    Aktuellt tillgängligt säte|
|AssignedSeats| Aktuellt tilldelat säte |
|ActiveSeats|   Aktuella aktiva platser |
|DeploymentOpportunity| Aktuell distributions möjlighet|
|ActiveUsagePercent|    Aktuell aktiv användning i procent|
 
**Power BI licens användning**: data definitionen för de olika fälten i Power BI – licens användnings rapporten är:

| **Kolumn namn** | **Data Beskrivning** |
|---------|:---------|
|SubscriptionId|    GUID för prenumerationen|
|SubscriptionStartDate| Start datum för prenumerationen|
|SubscriptionEndDate|   Slutdatum för prenumerationen|
|SubscriptionStatus|    Status för prenumerationen (aktiv eller In-Active eller under Grace-period)|
|Månad| Datum sammanställt per månad |
|SKU|   Produkt-SKU för produkten |
|SKUId| SKU-ID för produkten |
|FreeVsPaidSKU| Kostnads fri eller betald SKU-differentiering |
|SalesModel|    Försäljnings modell som används för att sälja prenumerationen|
|DetailedSalesModel|    Detaljerad försäljnings modell för prenumerationen|
|CustomerName|  Kundnamn |
|CustomerTenantId|  GUID för kund klient organisation |
|CustomerTpid|  Överordnad kund topp identifierare| 
|CustomerSegment|   Marknads segment för kunden |
|CustomerMarket|    Den geografiska marknaden för kunden |
|MPNId| Microsoft Partner Network-ID |
|PartnerName|   Partnerns namn |
|PartnerLocation|   Den geografiska land platsen för partnern |
|PartnerAttachType| Tilldelnings typ för prenumerationen|
|AvailableSeats|    Aktuella tillgängliga platser|
|AssignedSeats| Aktuella tilldelade platser|
|ActiveSeats|   Aktuella aktiva platser|
|DeploymentOpportunity| Aktuell distributions möjlighet|
|ActiveUsagePercent|    Aktuell aktiv användning i procent|

**Team användning – möten och samtal**: data definitionerna för de olika fälten är:

| **Kolumn namn** | **Data Beskrivning** |
|---------|:---------|
|CustomerTenantId|  Klient-ID för kund |
|CustomerTpid|  Överordnad kund topp-ID |
|Månad| Månad för vilken användning rapporteras|
|Under arbets belastning|   Under arbets belastning för vilken användning rapporteras (möten, samtal, telefon system)|
|Antal möten| Antal möten|
|Mötets varaktighet|  Total Mötes varaktighet i timmar|

**Team-månatlig användnings information**: data definitioner för de olika fälten är:

| **Kolumn namn** | **Data Beskrivning** |
|---------|:---------|
|CustomerTenantId|  Klient-ID för kund |
|CustomerTpid|  Överordnad kund topp-ID |
|Månad| Månad för vilken användning rapporteras|
|Under arbets belastning|   Under arbets belastning för vilken användning rapporteras (möten, samtal, telefon system)|
|Skriv bords användare| Antal användare som använder team på Skriv bordet|
|Mobila användare|  Antal användare som använder team på mobilen|
|Webb användare| Antal användare som använder team på webben|
|AllUpParticipants| Antal distinkta team användare för månaden|

**Team användning – 3P appar**: data definitionerna för de olika fälten är:

| **Kolumn namn** | **Data Beskrivning** |
|---------|:---------|
|CustomerTenantId|  Klient-ID för kund| 
|CustomerTpid|  Överordnad kund topp-ID |
|Månad| Månad för vilken användning rapporteras|
|Namn på 3P-app|   Namn på Team-appen|
|Antal användare|    Antal användare för appen|


**Tränings information**: data definitionerna för de olika fälten i kurs informations rapporten är:

| **Kolumn namn** | **Data Beskrivning** |
|---------|:---------|
|TrainingActivityId|    ID för utbildningen |
|TrainingTitle| Rubrik på utbildningen |
|TrainingType|  Typ av utbildning (certifiering/tentamen)|
|IndividualFirstName|   Förnamn för kunden| 
|IndividualLastName|    Kundens efter namn| 
|E-post| Personligt e-post-ID för kunden|
|CorpEmail| Office-e-post-ID för kund|
|TrainingCompletionDate|    Slut för ande datum för utbildningen |
|Månad| Månad för vilken data rapporteras|
|IcMCP| Anger om användaren är Microsoft Certified Professional|
|MCPID| MCP-ID för användaren|
|MPNId| Microsoft Partner Network-ID |
|PartnerName|   Partnerns namn |
|PartnerCityLocation|   Partnerns geografiska ort plats |
|PartnerCountryLocation|    Den geografiska land platsen för partnern |

**Microsoft Learn**: data definitionerna för de olika fälten i Microsoft Learn rapporten är:

| **Kolumn namn** | **Data Beskrivning** |
|---------|:---------|
|Användarnamn|Användarens namn| 
|UserId|Användar-GUID |
|TrainingName|Utbildnings namn |
|TrainingType|Typ av utbildning (modul/Learning sökväg)|
|Produkter|Produkt för vilken inlärnings modulen gäller|
|Roller|Relevanta roller för utbildningen |
|CompletionDate|Datum för slutförd utbildning |
|MPNId|Microsoft Partner Network-ID |
|PartnerName|Partnerns namn |
|Land|Den geografiska land platsen för partnern |

**Översikt över kompetens och historik**: data definitionen för de olika fälten i kompetens sammanfattningen och historik rapporten är:

| **Kolumn namn** | **Data Beskrivning** |
|---------|:---------|
|CompetencyName|Kompetensens namn |
|CompetencyLevel|Kompetens nivå (Gold/Silver)|
|CompetencyStatus|Aktuell status för kompetens (aktiv/inaktiv/i respitperiod)|
|CompetencyStartDate|Start datum för den aktuella kompetensen| 
|CompetencyEndDate|Slutdatum för den aktuella kompetensen |

**Kompetens prestanda**: data definitionerna för de olika fälten i kompetens prestanda rapporten är:

| **Kolumn namn** | **Data Beskrivning** |
|---------|:---------|
|CompetencyName|    Kompetensens namn |
|CompetencyAttainmentOptionName|    Namn på alternativet för att erhålla kompetens|
|Månad| Månad för vilken måtten rapporteras|
|MetricName|    Namnet på det mått som är relevant för kompetensen|
|MetricMonthlyContribution| Månatligt bidrag för måttet|
|TTMAggregate|  Aggregerade mått för de efterföljande 12 månaderna|
|AnniversaryYearAggregate|  Aggregerad mått för innevarande jubileums år|
|GoldThreshold| Prestanda krav för att uppfylla guld kompetensen|
|SilverThreshold|   Prestanda krav för att uppfylla silver kompetensen|

**Molnbaserad stigning – M365 benägenhet**: data definitionerna för de olika fälten i Cloud stigning-M365 benägenhet-rapporten är:

| **Kolumn namn** | **Data Beskrivning** |
|---------|:---------|
|MPN-ID|    Microsoft Partner Network-ID|
|Partner namn|  Partnerns namn|
|Kund-ID|   Kund-ID-nummer |
|DUNS-nummer|   Dun & Bradstreet nummer för den kund som poängs ätter för benägenhet|
|Account Name|  Kontots namn |
|Domain|    Kontots domän|
|Organisations storlek|  Organisationens storlek|
|Industri|  Industri  |
|Lodrät|  Den lodräta av kunden som betecknas för benägenhet, som identifieras av Microsoft och andra bransch standarder (D&B)|
|Område|  Geografiskt område på platsen|
|Dotterbolag|    Dotter bolag till kunden som poängs ätter för benägenhet|
|Säljområde|   Försäljnings området för kunden som poängs ätter för benägenhet|
|City|  Geografisk ort plats |
|Stat| Geografisk tillstånds plats|
|Postnummer|   Postnummer|
|Land|   Plats för geografiskt land |
|Segment|   Marknads segment |
|Del segment|   Marknads del segment |
|Översikt över SMC-typ|  SMC-typ |
|Topp ohanterad – beräknings bas|  Främsta ohanterade kunder – beräkning|
|Topp ohanterad-användar bas| Vanligaste ohanterade kunder – användare|
|IsNonProfit|   Om icke-vinst eller vinst (Ja/Nej)|
|Aktivera fjärran sluten arbete – rikta Exchange Online|   Kunder som har en aktiv Exchange Online-prenumeration, merförsäljning till M365|
|Aktivera fjärran sluten arbete – lokal förvärv (aktuell version) med CLAS benägenhet-+ 10 licenser|Kunden som har aktuellt lokal-kontor eller Win-klient (versioner som är efter EOS-produkter). Kunden har 10 eller fler licenser. Kund som har en benägenhet poäng. Partner ska vara mål för omvandling till M365.|
|Aktivera fjärran sluten arbete – lokal förvärv (aktuell version) med CLAS benägenhet-<10 licenser|Kunden som har aktuellt lokal-kontor eller Win-klient (versioner som är efter EOS-produkter). Kunden har färre än 10 licenser. Kund som har en benägenhet poäng. Partner ska vara mål för omvandling till M365.|
|Aktivera fjärran sluten arbete – lokal förvärv (aktuell version) utan CLAS benägenhet-+ 10 licenser| Kunden som har aktuellt lokal-kontor eller Win-klient (versioner som är efter EOS-produkter). Kunden har 10 eller fler licenser. Kunden har ingen benägenhet poäng. Partner ska vara mål för omvandling till M365.|
|Aktivera fjärran sluten arbete – lokal förvärv (aktuell version) utan CLAS benägenhet-<10 licenser| Kunden som har aktuellt lokal-kontor eller Win-klient (versioner som är efter EOS-produkter). Kunden har färre än 10 licenser. Kunden har ingen benägenhet poäng. Partner ska vara mål för omvandling till M365.|
|Aktivera fjärran sluten lokal förvärv (EOS) med CLAS benägenhet-+ 10 licenser|Kunden som har EOS on-lokal Office eller Win client (det vill säga versioner som är tidigare än och inklusive EOS-produkter. Kunden har 10 eller fler licenser. Kunden har en benägenhet poäng. Partner ska vara mål för omvandling till M365.|
|Aktivera fjärran sluten lokal förvärv (EOS) med CLAS-benägenhet – <10 licenser|Kunden som har EOS on-lokal Office eller Win client (det vill säga versioner som är tidigare än och inklusive EOS-produkter. Kunden har färre än 10 licenser. Kunden har en benägenhet poäng. Partner ska vara mål för omvandling till M365.|
|Aktivera fjärran sluten lokal förvärv (EOS) utan CLAS benägenhet-+ 10 licenser| Kunden som har aktuellt lokal-kontor eller Win-klient (det vill säga versioner som är tidigare än och inklusive EOS-produkter). Kunden har 10 eller fler licenser. Kunden har ingen benägenhet poäng. Partner ska vara mål för omvandling till M365.|
|Aktivera fjärran sluten arbete – lokal förvärv (EOS) utan CLAS-benägenhet – <10 licenser| Kunden som har aktuellt lokal-kontor eller Win-klient (det vill säga versioner som är tidigare än och inklusive EOS-produkter). Kunden har färre än 10 licenser. Kunden har ingen benägenhet poäng. Partner ska vara mål för omvandling till M365.|
|Aktivera fjärrarbete – hög benägenhet-potentiell kund för M365 (agera nu/utvärdera)| Kunder med höga benägenhet för M365.|
|Aktivera fjärran slutet arbete – tävlar (zoom) med M365| Kunder med zoomnings-och M365, mål för konvertering till team|
|Aktivera fjärran slutet arbete (zoom) utan M365|  Kunder med zoom, mål för konvertering till team|
|Minska kostnaderna och hantera M365 E3 riktade mot M365 E5| Befintlig kund med M365 E3, mål för M365 E5|
|Minska kostnaderna och hantera-M365 BB-och BS-kunder riktade mot M365 BP|    Befintliga M365 BB-och BS-kunder är riktade mot M365 BP|
|Transformera organisationens produktivitet – benägenhet|    Kunden visar benägenhet för ytan.|
|M365Cluster|Identifierar kundens benägenhet för att köpa M365.  Kluster fungerar nu och utvärderas bör vara riktade eftersom de kommer att producera högre avkastning.  Nurture och utbilda kunder bör bara vara riktade om det fortfarande finns kapacitet efter det att mål har åtgärdas och utvärderas för kunderna.|
|M365Fit|   Interna och externa data punkter som definierar firmographics. Anpassnings bedömnings använder en modell som liknar vår bästa SMB för att jämföra kunder och se om de är en potentiell anpassning för Microsoft Cloud produkter. Anpassnings resultat uppdateras kvartals vis.|
|M365Intent|    Signaler som rör sociala medier och en kunds beteende för online-beteende definierar avsikt. Poängen för avsikten är överordnad för att definiera klustren. Avsikts poängen uppdateras varje månad.|
|SurfaceCluster|    Detta identifierar kundens benägenhet till köp-ytan genom att konsolidera anpassnings-och avsikts rekommendationerna i ett kluster.  Kluster fungerar nu och utvärderas bör vara riktade eftersom de kommer att producera högre avkastning.  Nurture och utbilda kunder bör bara vara riktade om det fortfarande finns kapacitet efter det att mål har åtgärdas och utvärderas för kunderna.|
|SurfaceFit|    Interna och externa data punkter som definierar firmographics. Anpassnings bedömnings använder en modell som liknar vår bästa SMB för att jämföra kunder och se om de är en potentiell anpassning för Microsoft Cloud produkter. Anpassnings resultat uppdateras kvartals vis.|
|SurfaceIntent| Signaler som rör sociala medier och en kunds beteende för online-beteende definierar avsikt. Poängen för avsikten är överordnad för att definiera klustren. Avsikts poängen uppdateras varje månad.|
|O365Cluster|   Detta identifierar kundens benägenhet för att köpa O365.  Kluster fungerar nu och utvärderas bör vara riktade eftersom de kommer att producera högre avkastning.  Nurture och utbilda kunder bör bara vara riktade om det fortfarande finns kapacitet efter det att mål har åtgärdas och utvärderas för kunderna.|
|O365Fit|   Interna och externa data punkter som definierar firmographics. Anpassnings bedömnings använder en modell som liknar vår bästa SMB för att jämföra kunder och se om de är en potentiell anpassning för Microsoft Cloud produkter. Anpassnings resultat uppdateras kvartals vis.|
|O365Intent|    Signaler som rör sociala medier och en kunds beteende för online-beteende definierar avsikt. Poängen för avsikten är överordnad för att definiera klustren. Avsikts poängen uppdateras varje månad.|
|M365UpsellCustomer|    Detta anger om kunden visar merförsäljning-benägenhet för M365|
|Har Google|    Den här flaggan identifierar om en kund visar konkurrerande signaler för att äga Google-produkter|
|Har AWS|   Den här flaggan identifierar om en kund visar konkurrens bara signaler för ägande AWS-produkter|
|Har EA|    Detta anger om en förnyelse är ett Enterprise-avtal (EA) eller en EA-prenumeration|
|Har öppen|  Detta anger om en förnyelse är ett avtal med öppen eller öppen värde|

**Molnbaserad stigning – D365 benägenhet**: data definitionerna för de olika fälten i Cloud stigning-D365 benägenhet-rapporten är:

| **Kolumn namn** | **Data Beskrivning** |
|---------|:---------|
|MPN-ID|    Microsoft Partner Network-ID|
|Partner namn|  Partnerns namn|
|Kund-ID|   Kund-ID-nummer |
|DUNS-nummer|   Dun & Bradstreet nummer för den kund som poängs ätter för benägenhet|
|Account Name|  Kontots namn |
|Domain|    Kontots domän|
|Organisations storlek|  Organisationens storlek|
|Industri|  Industri  |
|Lodrät|  Den lodräta av kunden som betecknas för benägenhet, som identifieras av Microsoft och andra bransch standarder (D&B)
|Område|  Geografiskt område på platsen|
|Dotterbolag|    Dotter bolag till kunden som poängs ätter för benägenhet|
|Säljområde|   Säljområde|
|City|  Geografisk ort plats |
|Stat| Geografisk tillstånds plats|
|Postnummer|   Postnummer|
|Land|   Plats för geografiskt land |
|Segment|   Marknads segment |
|Del segment|   Marknads del segment |
|Översikt över SMC-typ|  Kategoriseringen av en kund: främsta ohanterade användar baser är kunder med 300 + anställda, topp ohanterad beräknings bas är kunder med en inverkan på 10 år på Azure 3 år, medel stora företag är kunder med 25 anställda eller större, små företag är kunder med färre än 25 anställda|
|Topp ohanterad – beräknings bas   |Främsta ohanterade kunder – beräkning|
|Topp ohanterad-användar bas| Vanligaste ohanterade kunder – användare|
|IsNonProfit|   Om icke-vinst eller vinst (Ja/Nej)|
|Aktivera digital försäljning – M365-plats storlek >= 25 platser (SalesPro benägenhet Model)|   Kunden utan D365. Plats storlek: 25 +. Partner bör vara mål för D365 Salespro|
|Aktivera Digital säljning – D365 SalesPro benägenhet (agera nu/utvärdera) |Höga benägenhet-kunder utan D365.  Partner bör vara mål för D365-SalesPro.|
|Hantering av ekonomisk risk & bedrägeri-Dynamics lokal install Base – Navision (BC benägenhet Model)|Befintlig kund med OnPrem Navision.  Partner ska vara mål för D365 BC|
|Hantering av ekonomisk risk & bedrägeri-Dynamics lokal install Base-AX (F&O benägenhet modell)    |Befintlig kund med OnPrem AX.  Partner ska vara mål för D365 F&O|
|Hantering av ekonomisk risk & bedrägerier-Dynamics lokal install Base – Great Plains (BC benägenhet Model)|  Befintlig kund med OnPrem Great Plains.  Partner ska vara mål för D365 BC|
|Hantering av ekonomisk risk & bedrägeri-Dynamics lokal install Base-Salomonöarna (BC benägenhet Model)|Befintlig kund med OnPrem Salomonöarna  Partner ska vara mål för D365 BC|
|Hantering av ekonomisk risk & bedrägeri-Dynamics lokal installation Base – andra (BC benägenhet Model) |Befintlig kund med andra OnPrem-lösningar som inte listas ovan.  Partner ska vara mål för D365 BC|
|Bygg Agile-affärsprocesser – Dynamics lokal install Base-AX/GP/SL/NAV/övrigt (D365 benägenhet Model)|   Bygg Agile-affärsprocesser – Dynamics lokal install Base-AX/GP/SL/NAV/övrigt (D365 benägenhet Model)|
|Bygg Agile-affärsprocesser – Dynamics-konkurrens för grund-Mendix/-system/Salesforce (D365 benägenhet Model)| Bygg Agile-affärsprocesser – Dynamics-konkurrens för grund-Mendix/-system/Salesforce (D365 benägenhet Model)|
|Bygg Agile-affärsprocesser – D365 F&O install Base |Befintliga D365 F&O-kunder.  Partner för att rikta in Power Apps.|
|Bygg flexibla affärs processer – D365 BC-installations Base| Befintliga D365 BC-kunder. Partner för att rikta in Power Apps.|
|Bygg flexibla affärs processer – D365 CE install Base| Befintliga D365 CE-kunder. Partner för att rikta in Power Apps.|
|Bygg en elastisk leverans kedja – Win och aktivera den första D365 arbets belastningen som D365 med icke-Oracle/SAP ERP-kunder|  Rikta in dig på kunder för D365-försörjnings kedja.|
|Bygg en elastisk leverans kedja – en D365 leverans kedja och/eller detalj handel/handel till befintliga D365 CE-kunder |Befintliga D365 CE-kunder för att rikta in sig på D365 leverans kedja|
|Bygg en elastisk leverans kedja – D365-SUP mellan försäljning. Kedja och/eller detalj handel/handel med D365 CE och (Oracle eller SAP)| Befintliga D365 CE-kunder med Oracle eller SAP som mål för D365-försörjnings kedjan|
|D365BCCluster| Detta identifierar kundens benägenhet att köpa D365 Business Central.  Kunder som visar benägenhet för BC är i kategorierna medel och liten.  Kluster fungerar nu och utvärderas bör vara riktade eftersom de kommer att producera högre avkastning.  Nurture och utbilda kunder bör bara vara riktade om det fortfarande finns kapacitet efter det att mål har åtgärdas och utvärderas för kunderna.|
|D365BCFit| Interna och externa data punkter som definierar firmographics. Anpassnings bedömnings använder en modell som liknar vår bästa SMB för att jämföra kunder och se om de är en potentiell anpassning för Microsoft Cloud produkter. Anpassnings resultat uppdateras kvartals vis.|
|D365BCIntent|  Signaler som rör sociala medier och en kunds beteende för online-beteende definierar avsikt. Poängen för avsikten är överordnad för att definiera klustren. Avsikts poängen uppdateras varje månad.|
|D365FOCluster| Detta identifierar kundens benägenhet för att köpa D365 ekonomi och åtgärder.  Kunder som visar benägenhet för F&O visas i de översta ohanterade kategorierna. Kluster fungerar nu och utvärderas bör vara riktade eftersom de kommer att producera högre avkastning.  Nurture och utbilda kunder bör bara vara riktade om det fortfarande finns kapacitet efter det att mål har åtgärdas och utvärderas för kunderna.|
|D365FOFit| Interna och externa data punkter som definierar firmographics. Anpassnings bedömnings använder en modell som liknar vår bästa SMB för att jämföra kunder och se om de är en potentiell anpassning för Microsoft Cloud produkter. Anpassnings resultat uppdateras kvartals vis.|
|D365FOIntent|  Signaler som rör sociala medier och en kunds beteende för online-beteende definierar avsikt. Poängen för avsikten är överordnad för att definiera klustren. Avsikts poängen uppdateras varje månad.|
|D365CECluster| Detta identifierar kundens benägenhet att köpa D365 kund engagemang.  Kunder som visar benägenhet för CE visas i kategorierna medel och liten.  Kluster fungerar nu och utvärderas bör vara riktade eftersom de kommer att producera högre avkastning.  Nurture och utbilda kunder bör bara vara riktade om det fortfarande finns kapacitet efter det att mål har åtgärdas och utvärderas för kunderna.|
|D365CEFit| Anpassa för D365 CE|
|D365CEIntent|  Avsikt för D365 CE|
|DynamicsOnPremAXorCRM_HasOpenRenewal|  Detta identifierar om en kund har en öppen förnyelse för Dynamics lokal AX eller CRM.|
|M365UpsellCustomer|    Detta anger om kunden visar merförsäljning-benägenhet för M365|
|Har Google|    Den här flaggan identifierar om en kund visar konkurrerande signaler för att äga Google-produkter|
|Har AWS|   Den här flaggan identifierar om en kund visar konkurrens bara signaler för ägande AWS-produkter|
|Har EA |Detta anger om en förnyelse är ett Enterprise-avtal (EA) eller en EA-prenumeration|
|Har öppen|  Detta anger om en förnyelse är ett avtal med öppen eller öppen värde|

**Cloud Ascent-Azure benägenhet**: data definitionerna för de olika fälten i Cloud Ascent-Azure benägenhet-rapporten är:

|**Kolumn namn** |**Data Beskrivning** |
|---------|:---------|
|MPN-ID|    Microsoft Partner Network-ID|
|Partner namn|  Partnerns namn|
|Kund-ID|   Kund-ID-nummer |
|DUNS-nummer|   Dun & Bradstreet nummer för den kund som poängs ätter för benägenhet|
|Account Name|  Kontots namn |
|Domain|    Kontots domän|
|Organisations storlek|  Organisationens storlek|
|Industri|  Industri  |
|Lodrät|  Den lodräta av kunden som betecknas för benägenhet, som identifieras av Microsoft och andra bransch standarder (D&B)|
|Område|  Geografiskt område på platsen|
|Dotterbolag|    Dotter bolag till kunden som poängs ätter för benägenhet|
|Säljområde|   Säljområde|
|City|  Geografisk ort plats |
|Stat| Geografisk tillstånds plats|
|Postnummer|   Postnummer|
|Land|   Plats för geografiskt land |
|Segment|   Marknads segment |
|Del segment|   Marknads del segment |
|Översikt över SMC-typ|  SMC-typ |
|Topp ohanterad – beräknings bas|  Främsta ohanterade kunder – beräkning|
|Topp ohanterad-användar bas| Vanligaste ohanterade kunder – användare|
|IsNonProfit|   Om icke-vinst eller vinst (Ja/Nej)|
|Migrera-EOS Win Server-EOS Windows Server IB med CLAS benägenhet-5 + licenser|   Kunder som har EOS on-lokal Win Server (det vill säga versioner som är tidigare än och inklusive EOS-produkter). Kunden har 5 eller fler licenser. Kund som har en benägenhet poäng.  Partner bör rikta in sig på dessa kunder för migrering till Azure.|
|Migrera-EOS Win Server-EOS Windows Server IB med CLAS benägenhet-<5 licenser|   Kunden som har EOS (End of Service) lokal Win Server (det vill säga versioner som är tidigare än och inklusive EOS-produkter). Kunden har färre än 5 licenser. Kund som har en benägenhet poäng.  Partner bör rikta in sig på dessa kunder för migrering till Azure.|
|Migrera-EOS Win Server-EOS Windows Server IB utan CLAS benägenhet-5 + licenser |Kunder som har EOS on-lokal Win Server (det vill säga versioner som är tidigare än och inklusive EOS-produkter). Kunden har fler än 5 licenser. Kunden har ingen benägenhet poäng. Partner bör rikta in sig på dessa kunder för migrering till Azure.|
|Migrera-EOS Win Server-EOS Windows Server IB utan CLAS benägenhet-<5 licenser|    Kunder som har EOS on-lokal Win Server (det vill säga versioner som är tidigare än och inklusive EOS-produkter). Har färre än 5 licenser. Kunden har ingen benägenhet poäng. Partner bör rikta in sig på dessa kunder för migrering till Azure.|
|Migrera-EOS SQL-EOS SQL Server IB med CLAS benägenhet-5 + licenser|  Kunden som har EOS lokal SQL Server (det vill säga versioner som är tidigare än och inklusive EOS-produkter). Kunden har 5 licenser. Kunden har en benägenhet poäng.  Partner bör rikta in sig på dessa kunder för migrering till Azure.|
|Migrera-EOS SQL-EOS SQL Server IB med CLAS benägenhet-<5-licenser|  Kunden som har EOS lokal SQL Server (det vill säga versioner som är tidigare än och inklusive EOS-produkter). Har färre än 5 licenser. Kund som har en benägenhet poäng. Partner bör rikta in sig på dessa kunder för migrering till Azure.|
|Migrera-EOS SQL-EOS SQL Server IB utan CLAS benägenhet-5 + licenser|   Kunden som har EOS lokal SQL Server (det vill säga versioner som är tidigare än och inklusive EOS-produkter). Kunden har 5 eller fler licenser. Kunden har ingen benägenhet poäng. Partner bör rikta in sig på dessa kunder för migrering till Azure.|
|Migrera-EOS SQL-EOS SQL Server IB utan CLAS benägenhet-<5 licenser|   Kunden som har EOS lokal SQL Server (det vill säga versioner som är tidigare än och inklusive EOS-produkter). Kunden har färre än 5 licenser. Kunden har ingen benägenhet poäng. Partner bör rikta in sig på dessa kunder för migrering till Azure.|
|Migrera – migrera lokal Win Server-Current Windows Server IB med CLAS benägenhet-5 + licenser|   Kunden som har aktuell lokal Win-Server (dvs versioner som är efter EOS-produkter). Kunden har 5 licenser. Kunden har en benägenhet poäng. Partner bör rikta in sig på dessa kunder för migrering till Azure.|
|Migrera – migrera på lokal Win Server – aktuell Windows Server IB med CLAS benägenhet-<5-licenser|   Kunden som har aktuell lokal Win-Server (dvs versioner som är efter EOS-produkter). Kunden har färre än 5 licenser. Kunden har en benägenhet poäng för Azure. Partner bör rikta in sig på dessa kunder för migrering till Azure.|
|Migrera – migrera lokal Win Server-Current Windows Server IB utan CLAS benägenhet-5 + licenser|    Kunden som har aktuell lokal Win-Server (dvs versioner som är efter EOS-produkter). Kunden har 5 licenser. Kunden har ingen benägenhet poäng. Partner bör rikta in sig på dessa kunder för migrering till Azure.|
|Migrera – migrera lokal Win Server-Current Windows Server IB utan CLAS benägenhet-<5-licenser |Kunden som har aktuell lokal Win-Server (dvs versioner som är efter EOS-produkter). Kunden har färre än 5 licenser. Kunden har ingen benägenhet poäng. Partner bör rikta in sig på dessa kunder för migrering till Azure.|
|Migrera – migrera till Azure SQL eller SQL VM-Current SQL Server IB med CLAS benägenhet-5 + licenser|  Kunden som har aktuell lokal SQL Server (det vill säga versioner som är efter EOS-produkter). Kunden har 5 licenser. Kunden har en benägenhet poäng. Partner bör rikta in sig på dessa kunder för migrering till Azure.|
|Migrera – migrera till Azure SQL-eller SQL-VM – aktuellt SQL Server IB med CLAS benägenhet-<5-licenser|  Kunden som har aktuell lokal SQL Server (det vill säga versioner som är efter EOS-produkter). Kunden har färre än 5 licenser. Kunden har en benägenhet poäng. Partner bör rikta in sig på dessa kunder för migrering till Azure.|
|Migrera – migrera till Azure SQL eller SQL VM-Current SQL Server IB utan CLAS benägenhet-5 + licenser|   Kunden som har aktuell lokal SQL Server (det vill säga versioner som är efter EOS-produkter). Kunden har 5 licenser. Kunden har ingen benägenhet poäng. Partner bör rikta in sig på dessa kunder för migrering till Azure.|
|Migrera – migrera till Azure SQL eller SQL VM-Current SQL Server IB utan CLAS benägenhet-<5-licenser|   Kunden som har aktuell lokal SQL Server (det vill säga versioner som är efter EOS-produkter). Kunden har färre än 5 licenser. Kunden har ingen benägenhet poäng. Partner bör rikta in sig på dessa kunder för migrering till Azure.|
|Migrera – OSS – migrera till OSS DB| Befintlig kund med någon av följande konkurrerande produkter: PostgreSQL, MySQL, MariaDB. Partner bör rikta in sig på dessa kunder för migrering till Azure.|
|Migrera – OSS – Linux på Azure |Befintlig kund med produkten: Linux. Partner bör rikta in sig på dessa kunder för migrering till Azure.|
|Migrera – SAP – SAP på Azure|  Befintlig kund med produkten: SAP. Partner bör rikta in sig på dessa kunder för migrering till Azure.|
|Migrera-WVD-RDS IB |Identifierar kunder med aktiva Windows-Fjärrskrivbordstjänster. Partner bör rikta in sig på dessa kunder för migrering till Azure.|
|Migrera-WVD – Cross Sälj modern work to Azure/WVD|   Identifierar kunder med M365 och inte har Azure. Partner bör rikta in sig på dessa kunder för migrering till Azure.|
|Migrera – VMware IB|   Befintlig kund med produkten: VMware. Partner bör rikta in sig på dessa kunder för migrering till Azure.|
|Migrera – Citrix IB|   Befintlig kund med produkten: Citrix Systems. Partner bör rikta in sig på dessa kunder för migrering till Azure.|
|Innovation-Analytics – Power BI IB med hög Azure-benägenhet|   Kunder med och aktiva Power BI prenumeration, inklusive: Power BI fristående Pro, Power BI – Azure-paket, Power BI-Office-paket, Power BI Suites – M365|
|Enable-DevOps med GitHub-VisualStudio/MSDN IB|    Identifierade kunder med aktiva visuella Studios|
|Win Server Standard-version|   Detta visar versionen av Windows Server standard-inköp från kunden|
|Win Server standard-licens|   Detta visar licens typen för Windows Server standard-köp av kunden|
|Data Center version för Win Server|    Detta visar versionen av Windows Data Center-köp av kunden|
|Licens för Win Server Data Center| Detta visar licens typen för köp av Windows Data Center från kunden|
|AzureFit|  Interna och externa data punkter som definierar firmographics. Anpassnings bedömnings använder en modell som liknar vår bästa SMB för att jämföra kunder och se om de är en potentiell anpassning för Microsoft Cloud produkter. Anpassnings resultat uppdateras kvartals vis.|
|AzureIntent|   Signaler som rör sociala medier och en kunds beteende för online-beteende definierar avsikt. Poängen för avsikten är överordnad för att definiera klustren. Avsikts poängen uppdateras varje månad.|
|AzureCluster|  Detta identifierar kundens benägenhet att köpa Azure genom att konsolidera anpassnings-och avsikts rekommendationerna i ett kluster.  Kluster fungerar nu och utvärderas bör vara riktade eftersom de kommer att producera högre avkastning.  Nurture och utbilda kunder bör bara vara riktade om det fortfarande finns kapacitet efter det att mål har åtgärdas och utvärderas för kunderna.|
|WindowsServerDataCenter_HasOpenRenewal|    Detta identifierar om en kund har en öppen förnyelse för ett Windows Server-datacenter|
|WindowsServerStandard_HasOpenRenewal|  Detta identifierar om en kund har en öppen förnyelse för en Windows Server standard|
|AzureUpsellCustomer|   Detta anger om kunden visar merförsäljning-benägenhet för Azure|
|Har Google|    Den här flaggan identifierar om en kund visar konkurrerande signaler för att äga Google-produkter|
|Har AWS|   Den här flaggan identifierar om en kund visar konkurrens bara signaler för ägande AWS-produkter|
|Har EA |Detta anger om en förnyelse är ett Enterprise-avtal (EA) eller en EA-prenumeration|
|Har öppen|  Detta anger om en förnyelse är ett avtal med öppen eller öppen värde|

**Cloud Ascent-Agreement-förnyelser benägenhet**: data definitionerna för de olika fälten i Cloud stigning-avtalet förnyelser benägenhet rapporten är:

|**Kolumn namn** |**Data Beskrivning** |
|---------|:---------|
|MPN-ID|    Microsoft Partner Network-ID|
|Partner namn|  Partnerns namn|
|Kund-ID|   Kund-ID-nummer |
|DUNS-nummer|   Dun & Bradstreet nummer för den kund som poängs ätter för benägenhet|
|Account Name|  Kontots namn |
|Domain|    Kontots domän|
|Organisations storlek|  Organisationens storlek|
|Industri|  Industri  |
|Lodrät|  Den lodräta av kunden som betecknas för benägenhet, som identifieras av Microsoft och andra bransch standarder (D&B)|
|Område|  Geografiskt område på platsen|
|Dotterbolag|    Dotter bolag till kunden som poängs ätter för benägenhet|
|Säljområde|   Säljområde|
|City|  Geografisk ort plats |
|Stat| Geografisk tillstånds plats|
|Postnummer|   Postnummer|
|Land|   Plats för geografiskt land |
|Segment|   Marknads segment |
|Del segment|   Marknads del segment |
|Översikt över SMC-typ|  SMC-typ |
|Topp ohanterad – beräknings bas|  Främsta ohanterade kunder – beräkning|
|Topp ohanterad-användar bas| Vanligaste ohanterade kunder – användare|
|IsNonProfit|Om icke-vinst eller vinst (Ja/Nej)|
|Har Google|Den här flaggan identifierar om en kund visar konkurrens bara signaler för ägande AWS-produkter|
|Har AWS|Den här flaggan identifierar om en kund visar konkurrens bara signaler för ägande AWS-produkter|
|Azure-kluster|Detta identifierar kundens benägenhet för att köpa Azure.  Kluster fungerar nu och utvärderas bör vara riktade eftersom de kommer att producera högre avkastning.  Nurture och utbilda kunder bör bara vara riktade om det fortfarande finns kapacitet efter det att mål har åtgärdas och utvärderas för kunderna.|
|D365 F&O-kluster|  Detta identifierar kundens benägenhet för att köpa D365 ekonomi och åtgärder.  Kunder som visar benägenhet för F&O visas i de översta ohanterade kategorierna.  Kluster fungerar nu och utvärderas bör vara riktade eftersom de kommer att producera högre avkastning.  Nurture och utbilda kunder bör bara vara riktade om det fortfarande finns kapacitet efter det att mål har åtgärdas och utvärderas för kunderna.|
|D365 CE-kluster|   Detta identifierar kundens benägenhet att köpa D365 kund engagemang.  Kunder som visar benägenhet för CE visas i kategorierna medel och liten.  Kluster fungerar nu och utvärderas bör vara riktade eftersom de kommer att producera högre avkastning.  Nurture och utbilda kunder bör bara vara riktade om det fortfarande finns kapacitet efter det att mål har åtgärdas och utvärderas för kunderna.|
|D365 BC-kluster|   Detta identifierar kundens benägenhet att köpa D365 Business Central.  Kunder som visar benägenhet för BC är i kategorierna medel och liten.  Kluster fungerar nu och utvärderas bör vara riktade eftersom de kommer att producera högre avkastning.  Nurture och utbilda kunder bör bara vara riktade om det fortfarande finns kapacitet efter det att mål har åtgärdas och utvärderas för kunderna.|
|M365-kluster|  Detta identifierar kundens benägenhet att köpa M365.  Kluster fungerar nu och utvärderas bör vara riktade eftersom de kommer att producera högre avkastning.  Nurture och utbilda kunder bör bara vara riktade om det fortfarande finns kapacitet efter det att mål har åtgärdas och utvärderas för kunderna.|
|Licens program|   Detta identifierar licens programmets typ för förnyelsen|
|Avtals-ID|  Avtals identifierare|
|Datum för avtals slutdatum|    Datum för avtals slutdatum |
|Förfallo typ|   Typ av förfallo datum|
|Förfallo datum för intäkter|  Intäkter som associeras med prenumerationer som upphör att gälla|
|Har EA|    Detta anger om en förnyelse är ett Enterprise-avtal (EA) eller en EA-prenumeration|
|Har öppen|  Detta anger om en förnyelse är ett avtal med öppen eller öppen värde|
|Azure merförsäljning-kund| Detta anger om kunden visar merförsäljning-benägenhet för Azure|
|M365 merförsäljning-kund|  Detta anger om kunden visar merförsäljning-benägenhet för M365|
|RevSumDivisionName|    Detta identifierar produkten som är igång för förnyelsen|

## <a name="next-steps"></a>Nästa steg

Information om rapporter finns i [Hämta rapporter](pci-download-reports.md).
