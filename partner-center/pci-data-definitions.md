---
title: Datadefinitioner för insikter
ms.topic: article
ms.date: 12/14/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Dokumentet innehåller olika rapporter och deras datadefinitioner, som du kan ladda ned från sidan För nedladdning av insikter.
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 23ca20fbb2febfd4b1ea92f72fbfda5ac83d7eb6
ms.sourcegitcommit: 4118de5cf55d1bd618ecca13c1b2ec59d80f43db
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/24/2021
ms.locfileid: "112565516"
---
# <a name="export--data-definitions"></a>Export – Datadefinitioner 

**Lämpliga roller:** Rapportvisningsprogram | Rapportvisningsprogram för chefer

## <a name="introduction"></a>Introduktion 

Genom att använda hubben Ladda ned rapporter på instrumentpanelen Insights kan du exportera rådatauppsättningarna. 

De olika rapporterna, som du kan ladda ned tillsammans med deras datadefinitioner, visas i följande tabeller: 

### <a name="partner-profile-report"></a>**Partnerprofilrapport**

| Kolumnnamn | Databeskrivning | 
| :--------- | :--------- | 
| MPNId | Microsoft Partner Network (MPN) ID| 
| PartnerName | Partnerns namn | 
| PGA_MPNId | Identifierare för MPN för partnerns globala konto | 
| PGA_PartnerName | Partnerns globala kontonamn | 
| City | Partnerns ort | 
| Land | Partnerns land | 
| HierarchyLevel | Anger om det är ett globalt MPN-ID eller plats-MPN-ID | 

### <a name="customer-details-report"></a>**Kundinformationsrapport**

| Kolumnnamn | Databeskrivning | 
| :--------- | :--------- | 
| CustomerName | Kundens namn | 
| CustomerTenantId | Identifierare för kundens klientorganisation | 
| CustomerTpid | Identifierare för kundens överordnade överordnade | 
| CustomerSegment | Kundsegment | 
| CustomerMarket | Kundens geografiska marknad | 
| CustomerStatus | Kundstatus (aktiv eller inaktiv) | 
| Produkt | Produkten såldes till kunden via MPN: Office 365, Dynamics 365, Enterprise Mobility and Security, Power BI eller Microsoft Azure | 
| SKU | Produkt-SKU | 
| Månad | Månad då användning och intäkter rapporteras | 
| MPNId | Identifierare för Microsoft Partner Network | 
| PartnerName | Partnerns namn | 
| PartnerLocation | Partnerns geografiska plats | 
| PartnerAttributionType | Attributionstyp för partnern | 
| SalesChannel | Försäljningskanal | 
| AvailableSeats | Tillgängliga platser | 
| RevenueUSD | Intäkter i amerikanska dollar | 

### <a name="reseller-performance-report"></a>**Prestandarapport för återförsäljare**

> [!Note]
> Data om intäkter och Azure-förbrukade intäkter (ACR) är endast tillgängliga för användare som är rapportanvändare.

| Kolumnnamn | Databeskrivning | 
| :--------- | :--------- | 
| ResellerMPNid | Identifierare Microsoft Partner Network återförsäljare | 
| ResellerName | Återförsäljarens namn | 
| ResellerMarket | Återförsäljares land på marknaden | 
| IndirectProviderMPNId | Identifierare för den indirekta providern Microsoft Partner Network | 
| IndirectProviderName | Namn på indirekt leverantör | 
| Månad | Månad då användning och intäkter rapporteras | 
| Produkt | Produktnamn | 
| SubscriptionID | Identifierare för prenumerationen | 
| AvailableSeats | Antal tillgängliga platser | 
| AssignedSeats | Antal tilldelade platser | 
| BilledRevenueUSD | Fakturerade intäkter i amerikanska dollar | 
| CustomerName | Kundens namn | 
| CustomerTPid | Identifierare för kundens överordnade överordnade | 
| CustomerSegment | Kundsegment | 
| CustomerMarket | Kundens geografiska marknad | 
| ResellerStatus | Återförsäljarstatus | 

### <a name="subscription-details-report"></a>**Prenumerationsinformationsrapport**

>[!Note]
>Intäkter och ACR-data är endast tillgängliga för användare som är rapportanvändare.

| Kolumnnamn | Databeskrivning | 
| :--------- | :--------- | 
| SubscriptionId | GUID för prenumerationen | 
| SubscriptionStartDate | Startdatum för prenumerationen | 
| SubscriptionEndDate | Slutdatum för prenumerationen | 
| SubscriptionState | Status för prenumerationen (aktiv eller omsättning) | 
| Månad | Månad då användning och intäkter rapporteras | 
| IsAutoRenew | Anger om prenumerationen har förnyats automatiskt (Ja eller Nej) | 
| CustomerName | Kundens namn | 
| CustomerTenantId | GUID för kunden | 
| CustomerTpid | Kundens främsta överordnade identifierare | 
| CustomerSegment | Kundens marknadssegment | 
| CustomerMarket | Kundens geografiska marknad | 
| Produkt | Produkt som säljs till kunden av partnern | 
| SKU | Produktens SKU | 
| MPNId | Microsoft Partner Network ID för partnern | 
| PartnerName | Partnerns namn | 
| PartnerLocation | Partnerns geografiska plats | 
| PartnerAttributionType | Attributionstyp för prenumerationen | 
| SalesChannel | Kanal för försäljning – Direkt, Molnlösningsleverantör (CSP) och så vidare | 
| AvailableSeats | Aktuell tillgänglig plats | 
| RevenueUSD | Intäkter i amerikanska dollar | 
| Registrerings-ID | Registrerings-ID för prenumerationen | 

### <a name="azure-usage-report"></a>**Användningsrapport för Azure**

| Kolumnnamn | Databeskrivning | 
| :--------- | :--------- | 
| SubscriptionId | GUID för prenumerationen | 
| SubscriptionStartDate | Datumet för prenumerationens start | 
| SubscriptionEndDate | Datumet för prenumerationens slut | 
| SubscriptionState | Aktuellt tillstånd för prenumerationen (Öppen, Stängd, Aktiv eller Respitperiod) | 
| Månad | Datum aggregerat efter månad | 
| ServiceName | Namnet på Azure-tjänsten | 
| MeterCategory | Namnet på mätarkategorin | 
| UsageUnits | Antalet enheter som används under faktureringsperioden | 
| CustomerName | Kundens namn | 
| CustomerTenantId | Kundens klientorganisations-ID | 
| CustomerTpid | Kundens överordnade ID | 
| CustomerSegment | Kundens segment | 
| CustomerMarket | Kundens geografiska marknad | 
| MPNId | Microsoft Partner Network id för kunden | 
| PartnerName | Partnerns namn | 
| PartnerLocation | Partnerns geografiska land | 
| PartnerAttributionType | Attributionstyp för partnern | 
| SalesChannel | Kanal för försäljningen (Direct/CSP, Indirect/CSP, Direct och så vidare) | 
| ACR_USD | Azure-förbrukade intäkter (ACR) i amerikanska dollar | 
| Registrerings-ID | Registrerings-ID för Azure-prenumerationen | 

### <a name="office-365-license-usage-report"></a>**Licensanvändningsrapport för Office 365**

| Kolumnnamn | Databeskrivning | 
| :--------- | :--------- | 
| CustomerTenantId | Kundens klientorganisations-ID | 
| CustomerTpid | Kundens överordnade ID | 
| WorkloadName | Skype för företag, Teams, Exchange Online | 
| Månad | Månad då användning rapporteras | 
| PaidAvailableUnits | Antal betalda tillgängliga enheter | 
| MonthlyActiveUsers | Antal månatliga aktiva användare | 
| CustomerName | Kundens namn | 
| CustomerMarket | Geografiskt land för kundens marknad | 
| CustomerSegment | Kundsegment | 
| MPNId | Identifierare för Microsoft Partner Network | 
| PartnerName | Partnerns namn | 
| PartnerLocation | Partnerns geografiska plats | 
| PartnerAttributionType | Attributionstyp för partnern | 

### <a name="enterprise-mobility-license-usage-report"></a>**Användningsrapport för Enterprise Mobility-licens**

| Kolumnnamn | Databeskrivning | 
| :--------- | :--------- | 
| CustomerTenantId | Kundens klientorganisations-ID | 
| CustomerTpid | Kundens överordnade ID | 
| WorkloadName | Namnet på arbetsbelastningen Enterprise Mobility + Security (EMS) | 
| Månad | Månad då användning rapporteras | 
| PaidAvailableUnits | Antal betalda tillgängliga enheter | 
| MonthlyActiveUsers | Antal månatliga aktiva användare | 
| CustomerName | Kundens namn | 
| CustomerMarket | Geografiskt land för kundens marknad | 
| CustomerSegment | Kundsegment | 
| MPNId | Identifierare för Microsoft Partner Network | 
| PartnerName | Partnerns namn | 
| PartnerLocation | Partnerns geografiska plats | 
| PartnerAttributionType | Attributionstyp för partnern | 

### <a name="dynamics-365-license-usage-report"></a>**Licensanvändningsrapport för Dynamics 365**

| Kolumnnamn | Databeskrivning | 
| :--------- | :--------- | 
| SubscriptionId | GUID för prenumerationen | 
| SubscriptionStartDate | Startdatum för prenumerationen | 
| SubscriptionEndDate | Slutdatum för prenumerationen | 
| SubscriptionStatus | Status för prenumerationen | 
| Månad | Månad då användning rapporteras | 
| RevSumDivisionName | Namnet på rev-summadivisionen | 
| RevSumCategoryName | Namnet på rev-summakategorin | 
| SKU | Produktens SKU | 
| SKUId | SKU-ID för produkten | 
| FreeVs IASKU | Anger om det är en kostnadsfri eller betald SKU | 
| SalesModel | Försäljningskanal som används för att sälja prenumerationen | 
| DetailedSalesModel | Detaljerad försäljningsmodell för prenumerationen | 
| CustomerName | Kundens namn | 
| CustomerTenantId | GUID för kundens klientorganisation | 
| CustomerTpid | Kundens främsta överordnade identifierare | 
| CustomerSegment | Kundens marknadssegment | 
| CustomerMarket | Kundens geografiska marknad | 
| MPNId | Identifierare för Microsoft Partner Network | 
| PartnerName | Partnerns namn | 
| PartnerLocation | Partnerns geografiska land | 
| PartnerAttachType | Attributionstyp för prenumerationen | 
| AvailableSeats | Aktuell tillgänglig plats | 
| AssignedSeats | Aktuell tilldelad plats | 
| ActiveSeats | Aktuella aktiva platser | 
| DistributionOpportunity | Aktuell distributionsmöjlighet | 
| ActiveUsagePercent | Aktuell aktiv användning i procent | 

### <a name="power-bi-license-usage-report"></a>**Power BI licensanvändningsrapport**

| Kolumnnamn | Databeskrivning | 
| :--------- | :--------- | 
| SubscriptionId | GUID för prenumerationen | 
| SubscriptionStartDate | Startdatum för prenumerationen | 
| SubscriptionEndDate | Slutdatum för prenumerationen | 
| SubscriptionStatus | Status för prenumerationen (aktiv, inaktiv eller respitperiod) | 
| Månad | Datum aggregerat efter månad | 
| SKU | Produktens SKU | 
| SKUId | SKU-ID för produkten | 
| FreeVsAvsKU | Kostnadsfri eller betald SKU-differentiator | 
| SalesModel | Försäljningsmodell som används för att sälja prenumerationen | 
| DetailedSalesModel | Detaljerad försäljningsmodell för prenumerationen | 
| CustomerName | Kundens namn | 
| CustomerTenantId | GUID för kundklientorganisationen | 
| CustomerTpid | Identifierare för den överordnade kunden | 
| CustomerSegment | Kundens marknadssegment | 
| CustomerMarket | Kundens geografiska marknad | 
| MPNId | Identifierare för Microsoft Partner Network | 
| PartnerName | Namnet på partnern | 
| PartnerLocation | Partnerns geografiska land | 
| PartnerAttachType | Attributionstyp för prenumerationen | 
| AvailableSeats | Aktuella tillgängliga platser | 
| AssignedSeats | Aktuella tilldelade platser | 
| ActiveSeats | Aktuella aktiva platser | 
| DistributionOpportunity | Aktuell distribution möjlighet | 
| ActiveUsagePercent | Aktuell aktiv användning i procent | 

### <a name="teams-meetings-and-calls-report"></a>**Rapport för Teams-möten och -samtal**

| Kolumnnamn | Databeskrivning | 
| :--------- | :--------- | 
| CustomerTenantId | Kundens klientorganisations-ID | 
| CustomerTpid | Identifierare för den överordnade kunden | 
| Månad | Månad då användning rapporteras | 
| Underarbetslast | Underbelastning som användning rapporteras för (möten, samtal eller telefonsystem) | 
| Antal möten | Antal möten | 
| Mötesvaraktighet | Total mötesvaraktighet i timmar | 

### <a name="teams-monthly-usage-report"></a>**Månatlig användningsrapport för Teams**

| Kolumnnamn | Databeskrivning | 
| :--------- | :--------- | 
| CustomerTenantId | Kundens klientorganisations-ID | 
| CustomerTpid | Identifierare för den överordnade kunden | 
| Månad | Månad då användning rapporteras | 
| Underarbetslast | Underbelastning som användning rapporteras för (möten, samtal eller telefonsystem) | 
| Desktop-användare | Antal användare som använder Teams på skrivbordet | 
| Mobila användare | Antal användare som använder Teams på mobila enheter | 
| Webbanvändare | Antal användare som använder Teams på webben | 
| AllUpParticipants | Antal unika Teams-användare för månaden | 

### <a name="teams-usage-3p-apps-report"></a>**Rapport för Teams-användning med 3P-appar**

| Kolumnnamn | Databeskrivning | 
| :--------- | :--------- | 
| CustomerTenantId | Kundens klientorganisations-ID | 
| CustomerTpid | Kundens överordnade ID | 
| Månad | Månad då användning rapporteras | 
| 3P-appnamn | Namnet på Teams-appen | 
| Antal användare | Antal användare för appen | 


### <a name="training-details-report"></a>**Rapport för träningsinformation**

| Kolumnnamn | Databeskrivning | 
| :--------- | :--------- | 
| TrainingActivityId | Identifierare för träningen | 
| TrainingTitle | Utbildningens titel | 
| TrainingType | Typ av utbildning (certifiering eller prov) | 
| IndividualFirstName | Kundens förnamn | 
| IndividualLastName | Kundens efternamn | 
| E-post | Kundens personliga e-post-ID | 
| CorpEmail | Kundens e-post-ID för Office | 
| TrainingCompletionDate | Slutförandedatum för träningen | 
| Månad | Månad då data rapporteras | 
| IcMCP | Anger om användaren är Microsoft Certified Professional (MCP) | 
| MCPID | MCP-ID för användaren | 
| MPNId | Identifierare för Microsoft Partner Network | 
| PartnerName | Namnet på partnern | 
| PartnerCityLocation | Partnerns geografiska plats | 
| PartnerCountryLocation | Partnerns geografiska land | 

### <a name="microsoft-learn-report"></a>**Microsoft Learn rapport**

| Kolumnnamn | Databeskrivning | 
| :--------- | :--------- | 
| Användarnamn | Användarens namn | 
| UserId | GUID för användaren | 
| TrainingName | Namnet på träningen | 
| TrainingType | Typ av utbildning (modul eller utbildningsväg) | 
| Produkter | Produkt som utbildningsmodulen gäller för | 
| Roller | Tillämpliga roller för träningen | 
| CompletionDate | Datum för slutförande av träningen | 
| MPNId | Identifierare för Microsoft Partner Network | 
| PartnerName | Namnet på partnern | 
| Land | Partnerns geografiska land | 

### <a name="competency-summary-and-history-report"></a>**Sammanfattning av kompetens och historikrapport**

| Kolumnnamn | Databeskrivning | 
| :--------- | :--------- | 
| CompetencyName | Namn på kompetensen | 
| CompetencyLevel | Kompetensnivå (guld eller silver) | 
| CompetencyStatus | Aktuell status för kompetensen (aktiv, inaktiv eller respitperiod) | 
| CompetencyStartDate | Startdatum för kompetensen | 
| CompetencyEndDate | Kompetensens slutdatum | 

### <a name="competency-performance-report"></a>**Prestandarapport för kompetens**

| Kolumnnamn | Databeskrivning | 
| :--------- | :--------- | 
| CompetencyName | Namn på kompetensen | 
| CompetencyAttainmentOptionName | Namn på kompetensalternativet | 
| Månad | Månad då måtten rapporteras | 
| MetricName | Namnet på det mått som är relevant för kompetensen | 
| MetricMonthlyContribution | Månatligt bidrag för måttet | 
| TTMAggregate | Aggregerat mått för de avslutande 12 månaderna | 
| AnniversaryYearAggregate | Aggregerat mått för det aktuella årsdagen | 
| GoldThreshold | Prestandakrav för att uppfylla guldkompetens | 
| SilverThreshold | Prestandakrav för att uppfylla Silver-kompetens | 

### <a name="cloud-ascent---microsoft-365-propensity-report"></a>**Cloud Ascent – Microsoft 365 rapport om skapacitet**

| Kolumnnamn | Databeskrivning | 
| :--------- | :--------- | 
| MPN-ID | Microsoft Partner Network-ID | 
| Partnernamn | Namnet på partnern | 
| Kund-ID | Kundens identifierarnummer | 
| DUNS-nummer | Dun & Bradstreet (D&B) för den kund som poängas för berättigande | 
| Account Name | Namn på kontot | 
| Domain | Domänen för kontot | 
| Organisationsstorlek | Organisationens storlek | 
| Industri | Bransch som organisationen tillhör | 
| Lodrät | Vertikalen hos den kund som poängas för benägenhet enligt Microsoft, D&B och andra branschstandarder | 
| Område | Geografiskt område för platsen | 
| Dotterbolag | Dotterbolaget till den kund som poängas för benägenhet | 
| Säljområde | Försäljningsområde för den kund som poängsattes för benägenhet | 
| City | Organisationens geografiska plats | 
| Tillstånd | Organisationens geografiska plats | 
| Postnummer | Organisationens postnummer | 
| Land | Organisationens geografiska land | 
| Segment | Marknadssegment | 
| Undersegment | Undersegment för marknad | 
| Sammanfattning av SMC-typ | SMC-typ | 
| Översta ohanterade – beräkningsbas | De främsta ohanterade kunderna – beräkning | 
| Översta ohanterade – användarbas | De mest ohanterade kunderna – användare | 
| IsNonProfit | Anger om organisationen är ideell (Ja eller Nej) | 
| Aktivera fjärrarbete – Exchange Online som mål | Kunder som har en aktiv Exchange Online-prenumeration, merförsäljning till Microsoft 365 | 
| Aktivera fjärrarbete – lokalt förvärv (aktuell version) med Cloud Ascent-benägenhet – +10 licenser | Kund som har en aktuell lokal Office- eller Windows-klient. Klientversionen är alltså senare än en EOL-version (End of Life). Kunden har 10 eller fler licenser. Kund som har en benägenhetspoäng. Partnern bör rikta in sig på konvertering till Microsoft 365. | 
| Aktivera fjärrarbete – lokalt förvärv (aktuell version) med Cloud Ascent-benägenhet – <10 licenser | Kund som har en aktuell lokal Office- eller Windows-klient (det vill säga en senare version än EOL). Kunden har färre än 10 licenser. Kund som har en benägenhetspoäng. Partnern bör rikta in sig på konvertering till Microsoft 365. | 
| Aktivera fjärrarbete – lokalt förvärv (aktuell version) utan Cloud Ascent-benägenhet – +10 licenser | Kund som har en aktuell lokal Office- eller Windows-klient (det vill säga en senare version än EOL). Kunden har 10 eller fler licenser. Kunden har ingen benägenhetspoäng. Partnern bör rikta in sig på konvertering till Microsoft 365. | 
| Aktivera fjärrarbete – lokalt förvärv (aktuell version) utan Cloud Ascent-benägenhet – <10 licenser | Kund som har en aktuell lokal Office- eller Windows-klient (det vill säga en senare version än EOL). Kunden har färre än 10 licenser. Kunden har ingen benägenhetspoäng. Partnern bör rikta in sig på konvertering till Microsoft 365. | 
| Aktivera fjärrarbete – lokalt förvärv (EOL-version) med Cloud Ascent-benägenhet – +10 licenser | Kund som har en lokal Office- eller Windows-klient för EOL (det vill säga en EOL-version eller tidigare). Kunden har 10 eller fler licenser. Kunden har en benägenhetspoäng. Partnern bör rikta in sig på konvertering till Microsoft 365. | 
| Aktivera fjärrarbete – lokalt förvärv (EOL-version) med Cloud Ascent-benägenhet – <10 licenser | Kund som har en lokal Office- eller Windows-klient för EOL (det vill säga en EOL-version eller tidigare). Kunden har färre än 10 licenser. Kunden har en benägenhetspoäng. Partnern bör rikta in sig på konvertering till Microsoft 365. | 
| Aktivera fjärrarbete – lokalt förvärv (EOL-version) utan Cloud Ascent-benägenhet – +10 licenser | Kund som har en aktuell lokal Office- eller Windows-klient (det vill säga en EOL-version eller tidigare). Kunden har 10 eller fler licenser. Kunden har ingen benägenhetspoäng. Partnern bör rikta in sig på konvertering till Microsoft 365. | 
| Aktivera fjärrarbete – lokalt förvärv (EOL-version) utan Cloud Ascent-benägenhet – <10 licenser | Kund som har en aktuell lokal Office- eller Windows-klient (det vill säga en EOL-version eller tidigare). Kunden har färre än 10 licenser. Kunden har ingen benägenhetspoäng. Partnern bör rikta in sig på konvertering till Microsoft 365. | 
| Enable Remote Work - high-propensity prospect for Microsoft 365 (Act NowithEvaluate) | Potentiell kund med hög benägenhet för Microsoft 365 | 
| Aktivera fjärrarbete – konkurrera (Zooma) med Microsoft 365 | Kund med Zoom och Microsoft 365, mål för konvertering till Teams | 
| Aktivera fjärrarbete – konkurrera (Zooma) utan Microsoft 365 | Kund med Zoom, mål för konvertering till Teams | 
| Minska kostnader och hantera – Microsoft 365 E3 riktad mot Microsoft 365 E5 | Befintlig kund med Microsoft 365 E3, mål för Microsoft 365 E5 | 
| Minska kostnader och hantera – Microsoft 365 Business Basic- och Business Standard-kunder som är Microsoft 365 Business Premium | Befintliga Microsoft 365 Business Basic- och Business Standard-kunder, mål för Microsoft 365 Business Premium | 
| Transformera organisationsproduktivitet – surface-benägenhet | Kunden visar en benägenhet för Surface | 
| M365Cluster | Identifierar en kunds benägenhet att köpa Microsoft 365. Target Act Now och Evaluate clusters eftersom de ger högre avkastning. Rikta in sig på att utveckla och utbilda kunder endast om det fortfarande finns kapacitet efter att kunderna Act Now (Agera nu) och Evaluate (Utvärdera) har mål. | 
| M365Fit | Interna och externa datapunkter som definierar företagsgrafiska data. Fit scoring använder en lookalike-modell för våra bästa små eller medelstora företag (SBS) för att jämföra kunder och se om de är lämpliga för Microsofts molnprodukter. Bedömning av passning uppdateras kvartalsvis. | 
| M365Intent | Signaler som rör sociala medier och en kunds onlinebeteende definierar Intent. Avsiktsbedömningen överlagras i Anpassa för att definiera klustren. Avsiktsbedömningen uppdateras varje månad. | 
| SurfaceCluster | Identifierar en kunds återgivning av Surface genom att konsolidera rekommendationerna anpassa och avsikter i ett kluster. Target Act Now och Evaluate clusters eftersom de ger högre avkastning. Målrikta och utbilda kunder endast om det fortfarande finns kapacitet efter att kunderna Act Now (Agera nu) och Evaluate (Utvärdera) har mål. | 
| SurfaceFit | Interna och externa datapunkter som definierar företagsgrafiska data. Fit scoring använder en lookalike-modell till våra bästa SMI:er för att jämföra kunder och se om de är lämpliga för Microsofts molnprodukter. Bedömning av passning uppdateras kvartalsvis. | 
| SurfaceIntent | Signaler som rör sociala medier och en kunds onlinebeteende definierar Avsikt. Avsiktsbedömningen överlagras i Anpassa för att definiera klustren. Avsiktsbedömningen uppdateras varje månad. | 
| O365Cluster | Identifierar kundens ighet att köpa Office 365. Target Act Now och Evaluate clusters eftersom de ger högre avkastning. Målrikta och utbilda kunder endast om det fortfarande finns kapacitet efter att kunderna Act Now (Agera nu) och Evaluate (Utvärdera) har mål. | 
| O365Fit | Interna och externa datapunkter som definierar företagsgrafiska data. Fit scoring använder en lookalike-modell till våra bästa SMI:er för att jämföra kunder och se om de är lämpliga för Microsofts molnprodukter. Bedömning av passning uppdateras kvartalsvis. | 
| O365Intent | Signaler som rör sociala medier och en kunds onlinebeteende definierar Avsikt. Avsiktsbedömningen överlagras i Anpassa för att definiera klustren. Avsiktsbedömningen uppdateras varje månad. | 
| M365UpsellCustomer | Identifierar om kunden visar säljförsäljningsrekvisitet för Microsoft 365 | 
| Har Google | Identifierar om kunden visar konkurrenssignaler för att äga Google-produkter | 
| Har AWS | Identifierar om kunden visar konkurrenssignaler för att äga Amazon Web Services (AWS)-produkter | 
| Har EA | Anger om en förnyelse är ett Enterprise-avtal (EA) eller en EA-prenumeration | 
| Har öppen | Anger om en förnyelse är ett open- eller open value-avtal | 

### <a name="cloud-ascent---dynamics-365-propensity-report"></a>**Cloud Ascent – 365-gångarrapport för Dynamics**

| Kolumnnamn | Databeskrivning | 
| :--------- | :--------- | 
| MPN-ID | MICROSOFT PARTNER NETWORK-ID (MPN) | 
| Partnernamn | Namnet på partnern | 
| Kund-ID | Kundidentifierarnummer | 
| DUNS-nummer | Dun & Ett Bradstreet-nummer för den kund som poängsätts för berättigande | 
| Account Name | Namn på kontot | 
| Domain | Domänen för kontot | 
| Organisationsstorlek | Organisationens storlek | 
| Industri | Bransch som organisationen tillhör | 
| Lodrät | Den lodräta kunden som får ett lägespoäng enligt Microsofts, D&B:s och andra branschstandarder
| Område | Geografiskt område för platsen | 
| Dotterbolag | Dotterbolaget till kunden som poängas för öjlighet | 
| Säljområde | Försäljningsområde för den kund som poängsattes för gångar | 
| City | Geografisk ort | 
| Tillstånd | Geografisk plats | 
| Postnummer | Organisationens postnummer | 
| Land | Geografiskt land | 
| Segment | Marknadssegment | 
| Undersegment | Undersegment för marknad | 
| Sammanfattning av SMC-typ | Kategorisering av en kund: De främsta ohanterade användarbaserna är kunder med över 300 anställda, de främsta ohanterade beräkningsbaserna är kunder med tre års potential i Azure med 10 000 USD, medelstora företag är kunder med 25 anställda eller större och små företag är kunder med färre än 25 anställda. | 
| Främsta ohanterade – beräkningsbas | De mest ohanterade kunderna – beräkning | 
| Översta ohanterade – användarbas | De mest ohanterade kunderna – användare | 
| IsNonProfit | Anger om organisationen är ideell (Ja eller Nej) | 
| Activate Digital Selling - Microsoft 365 - seat size >= 25 seats (SalesPro propensity model) | Kund utan Dynamics 365. Platsstorlek: 25+. Partnern bör rikta sig mot korsförsäljning av Dynamics 365 SalesPro. | 
| Aktivera digital försäljning – Dynamics 365 SalesPro-ighet (agera nu eller utvärdera) | Hög ighetskunder utan Dynamics 365. Partnern bör vara mål för Dynamics 365 SalesPro. | 
| Hantera ekonomiska risker & bedrägeri – Lokal Dynamics-installationsbas – Navision (Business Central-fundamentsmodell) | Befintlig kund med lokal Navision. Partnern bör vara mål för Dynamics 365 Business Central. | 
| Hantera finansiella & bedrägerier – Dynamics on-premises install base – Dynamics AX (Dynamics 365 Finance + Operations propensity model) | Befintlig kund med lokal AX. Partnern bör vara mål för Dynamics 365 Finance + Operations. | 
| Hantera finansiella risker & bedrägeri – Lokal Dynamics-installationsbas – Great Plains (Business Central-fundamentsmodell) | Befintlig kund med lokala Great Plains. Partnern bör vara mål för Dynamics 365 Business Central. | 
| Hantera finansiella risker & bedrägeri – Dynamics on-premises install base – Installeringsbas – Installeringsmodell (Business Central) | Befintlig kund med lokal Vara. Partnern bör vara mål för Dynamics 365 Business Central. | 
| Hantera finansiella risker & bedrägeri – Lokal Dynamics-installationsbas – Andra (Business Central-förfalskningsmodell) | Befintlig kund med andra lokala lösningar som inte tidigare listats. Partnern bör vara mål för Dynamics 365 Business Central. | 
| Skapa agila affärsprocesser – Lokal Dynamics-installationsbas – AX/GP/SL/NAV/Övrigt (365-gångarsmodell för Dynamics) | Skapa agila affärsprocesser – Lokal Dynamics-installationsbas – AX/GP/SL/NAV/Övrigt (365-gångarsmodell för Dynamics) | 
| Skapa agila affärsprocesser – Dynamics konkurrerar bas – Mendix/OutSystems/Salesforce (gångarmodell för Dynamics 365) | Skapa agila affärsprocesser – Dynamics konkurrerar bas – Mendix/OutSystems/Salesforce (365-gångarsmodell för Dynamics) | 
| Skapa agila affärsprocesser – Installationsbas för Dynamics 365 Finance + Operations | Befintliga Dynamics 365 Finance + Operations-kunder. Partner till Power Apps. | 
| Skapa agila affärsprocesser – Installationsbas för Dynamics 365 Business Central | Befintliga Dynamics 365 Business Central-kunder. Partner till Power Apps. | 
| Skapa agila affärsprocesser – Installationsbas för Dynamics 365 för kundengagemang | Befintliga Dynamics 365 Customer Engagement-kunder. Partner till Power Apps. | 
| Skapa en motståndskraftig leveranskedja – Windows och aktivera den första Dynamics 365-arbetsbelastningen som Dynamics 365 Supply Chain Management med kunder som inte använder Oracle eller SAP ERP (resursplanering för företag) | Målkunder för Dynamics 365 Supply Chain Management | 
| Skapa en motståndskraftig leveranskedja – korsförsäljning av Dynamics 365 Supply Chain Management och/eller detaljhandel eller handel till befintliga Dynamics 365 Customer Engagement-kunder | Befintliga Dynamics 365 Customer Engagement-kunder som mål för korsförsäljning av Dynamics 365 Supply Chain Management. | 
| Skapa en motståndskraftig leveranskedja – korsförsäljning av Dynamics 365 Supply Chain Management och/eller detaljhandel eller handel till Dynamics 365 Customer Engagement och Oracle eller SAP | Befintliga Dynamics 365 Customer Engagement-kunder med Oracle eller SAP som mål för Dynamics 365 Supply Chain Management | 
| D365BCCluster | Identifierar kundens ighet att köpa Dynamics 365 Business Central. Kunder som har en ighet för Business Central finns i kategorierna Medel och Liten. Target Act Now och Evaluate clusters, eftersom de ger högre avkastning. Rikta in dig på att utbilda kunder om det fortfarande finns kapacitet efter att du riktar in dig på Agera nu och Utvärdera kunder. | 
| D365BCFit | Interna och externa datapunkter som definierar företagsgrafiska data. Fit scoring använder en lookalike-modell till vår bästa SMB för att jämföra kunder och se om de är lämpliga för Microsofts molnprodukter. Bedömning av passning uppdateras kvartalsvis. | 
| D365BCIntent | Signaler som rör sociala medier och en kunds onlinebeteende definierar Avsikt. Avsiktsbedömningen överlagras i Anpassa för att definiera klustren. Avsiktsbedömningen uppdateras varje månad. | 
| D365FOCluster | Identifierar kundens ighet att köpa Dynamics 365 Finance and Operations. Kunder som har en ighet för Finance + Operations finns i de främsta ohanterade kategorierna. Target Act Now och Evaluate clusters, eftersom de ger högre avkastning. Rikta in dig på att utbilda kunder om det fortfarande finns kapacitet efter att du riktar in dig på Agera nu och Utvärdera kunder. | 
| D365FOFit | Interna och externa datapunkter som definierar företagsgrafiska data. Fit scoring använder en lookalike-modell till vår bästa SMB för att jämföra kunder och se om de är lämpliga för Microsofts molnprodukter. Bedömning av passning uppdateras kvartalsvis. | 
| D365FOIntent | Signaler som rör sociala medier och en kunds onlinebeteende definierar Avsikt. Avsiktsbedömningen överlagras i Anpassa för att definiera klustren. Avsiktsbedömningen uppdateras varje månad. | 
| D365CECluster | Identifierar kundens ighet att köpa Dynamics 365 Customer Engagement. Kunder som har en öjlighet för Customer Engagement finns i kategorierna Medel och Liten. Target Act Now och Evaluate clusters, eftersom de ger högre avkastning. Rikta in dig på att utbilda kunder om det fortfarande finns kapacitet efter att du riktar in dig på Agera nu och Utvärdera kunder. | 
| D365CEFit | Anger Anpassa för Dynamics 365 Customer Engagement | 
| D365CEIntent | Anger avsikt för Dynamics 365 Customer Engagement | 
| DynamicsOnPremAXorCRM_HasOpenRenewal | Anger om kunden har en öppen förnyelse för Dynamics on-premises AX eller CRM | 
| M365UpsellCustomer | Identifierar om kunden visar säljförsäljningsrekvisitet för Microsoft 365 | 
| Har Google | Identifierar om kunden visar konkurrenssignaler för att äga Google-produkter | 
| Har AWS | Identifierar om kunden visar konkurrenssignaler för att äga AWS-produkter | 
| Har EA | Anger om en förnyelse är en EA- eller EA-prenumeration | 
| Har öppen | Anger om en förnyelse är ett open- eller open value-avtal | 

### <a name="cloud-ascent---azure-propensity-report"></a>**Cloud Ascent – Azure-ighetsrapport**

| Kolumnnamn | Databeskrivning | 
| :--------- | :--------- | 
| MPN-ID | MICROSOFT PARTNER NETWORK-ID (MPN) | 
| Partnernamn | Namnet på partnern | 
| Kund-ID | Kundidentifierarnummer | 
| DUNS-nummer | Dun & Ett Bradstreet-nummer för den kund som poängsätts för berättigande | 
| Account Name | Namn på kontot | 
| Domain | Domänen för kontot | 
| Organisationsstorlek | Organisationens storlek | 
| Industri | Industri | 
| Lodrät | Den lodräta kunden som får ett lägespoäng enligt Microsofts, D&B:s och andra branschstandarder | 
| Område | Geografiskt område för platsen | 
| Dotterbolag | Dotterbolaget till kunden som poängas för öjlighet | 
| Säljområde | Försäljningsområde för den kund som poängsattes för gångar | 
| City | Geografisk ort | 
| Tillstånd | Geografisk plats | 
| Postnummer | Organisationens postnummer | 
| Land | Geografiskt land | 
| Segment | Marknadssegment | 
| Undersegment | Undersegment för marknad | 
| Sammanfattning av SMC-typ | SMC-typ | 
| Översta ohanterade – beräkningsbas | De främsta ohanterade kunderna – beräkning | 
| Översta ohanterade – användarbas | De mest ohanterade kunderna – användare | 
| IsNonProfit | Anger om organisationen är ideell (Ja eller Nej) | 
| Migrera – EOL Windows Server – EOL Windows Server IB med Cloud Ascent-benägenhet – fler än 5 licenser | Kund som har en lokal EOL Windows Server (det vill säga en EOL-version eller tidigare). Kunden har 5 eller fler licenser. Kund som har en benägenhetspoäng. Partnern bör rikta in sig på den här kunden för migrering till Azure. | 
| Migrera – EOL Windows Server – EOL Windows Server IB med Cloud Ascent-benägenhet – <5 licenser | Kund som har en lokal EOL Windows Server (det vill säga en EOL-version eller tidigare). Kunden har färre än 5 licenser. Kund som har en benägenhetspoäng. Partnern bör rikta in sig på den här kunden för migrering till Azure. | 
| Migrera – EOL Windows Server – EOL Windows Server IB utan Cloud Ascent-benägenhet – fler än 5 licenser | Kund som har en lokal EOL Windows Server (det vill säga en EOL-version eller tidigare). Kunden har fler än 5 licenser. Kunden har ingen benägenhetspoäng. Partnern bör rikta in sig på den här kunden för migrering till Azure. | 
| Migrera – EOL Windows Server – EOL Windows Server IB utan Cloud Ascent-benägenhet – <5 licenser | Kund som har en lokal EOL Windows Server (det vill säga en EOL-version eller tidigare). Har färre än 5 licenser. Kunden har ingen benägenhetspoäng. Partnern bör rikta in sig på den här kunden för migrering till Azure. | 
| Migrera – EOL SQL – EOL SQL Server IB med Cloud Ascent-benägenhet – fler än 5 licenser | Kund som har en lokal EOL-SQL Server (det vill säga en EOL-version eller tidigare). Kunden har fler än 5 licenser. Kunden har en benägenhetspoäng. Partnern bör rikta in sig på den här kunden för migrering till Azure. | 
| Migrera – EOL SQL – EOL SQL Server IB med Cloud Ascent-benägenhet – <5 licenser | Kund som har en lokal EOL-SQL Server (det vill säga en EOL-version eller tidigare). Har färre än 5 licenser. Kund som har en benägenhetspoäng. Partnern bör rikta in sig på den här kunden för migrering till Azure. | 
| Migrera – EOL SQL – EOL SQL Server IB utan Cloud Ascent-benägenhet – fler än 5 licenser | Kund som har en lokal EOL-SQL Server (det vill säga en EOL-version eller tidigare). Kunden har 5 eller fler licenser. Kunden har ingen benägenhetspoäng. Partnern bör rikta in sig på den här kunden för migrering till Azure. | 
| Migrera – EOL SQL – EOL SQL Server IB utan Cloud Ascent-benägenhet – <5 licenser | Kund som har en lokal EOL-SQL Server (det vill säga en EOL-version eller tidigare). Kunden har färre än 5 licenser. Kunden har ingen benägenhetspoäng. Partnern bör rikta in sig på den här kunden för migrering till Azure. | 
| Migrera – Migrera lokal Windows Server – aktuell Windows Server IB med Cloud Ascent-benägenhet – fler än 5 licenser | Kund som har en aktuell lokal Windows Server (det vill säga en senare version än EOL). Kunden har fler än 5 licenser. Kunden har en benägenhetspoäng. Partnern bör rikta in sig på den här kunden för migrering till Azure. | 
| Migrera – Migrera lokal Windows Server – aktuell Windows Server IB med Cloud Ascent-benägenhet – <5 licenser | Kund som har en aktuell lokal Windows Server (det vill säga en senare version än EOL). Kunden har färre än 5 licenser. Kunden har en benägenhetspoäng för Azure. Partnern bör rikta in sig på den här kunden för migrering till Azure. | 
| Migrera – Migrera lokal Windows Server – aktuell Windows Server IB utan Cloud Ascent-benägenhet – fler än 5 licenser | Kund som har en aktuell lokal Windows Server (det vill säga en senare version än EOL). Kunden har fler än 5 licenser. Kunden har ingen benägenhetspoäng. Partnern bör rikta in sig på den här kunden för migrering till Azure. | 
| Migrera – Migrera lokal Windows Server – aktuell Windows Server IB utan Cloud Ascent-benägenhet – <5 licenser | Kund som har en aktuell lokal Windows Server (det vill säga en senare version än EOL). Kunden har färre än 5 licenser. Kunden har ingen benägenhetspoäng. Partnern bör rikta in sig på den här kunden för migrering till Azure. | 
| Migrera – Migrera till Azure SQL eller virtuella SQL-datorer (VM) – aktuell SQL Server IB med Cloud Ascent-benägenhet – 5+ licenser | Kund som har en aktuell lokal SQL Server (det vill säga en senare version än EOL). Kunden har fler än 5 licenser. Kunden har en benägenhetspoäng. Partnern bör rikta in sig på den här kunden för migrering till Azure. | 
| Migrera – Migrera till Azure SQL eller VIRTUELLA SQL-datorer – aktuell SQL Server IB med Cloud Ascent-benägenhet – <5 licenser | Kund som har en aktuell lokal SQL Server (det vill säga en senare version än EOL). Kunden har färre än 5 licenser. Kunden har en benägenhetspoäng. Partnern bör rikta in sig på den här kunden för migrering till Azure. | 
| Migrera – Migrera till Azure SQL eller virtuella SQL-datorer – SQL Server IB utan Cloud Ascent-benägenhet – fler än 5 licenser | Kund som har en aktuell lokal SQL Server (det vill säga en senare version än EOL). Kunden har fler än 5 licenser. Kunden har ingen benägenhetspoäng. Partnern bör rikta in sig på den här kunden för migrering till Azure. | 
| Migrera – Migrera till Azure SQL eller VIRTUELLA SQL-datorer – aktuell SQL Server IB utan Cloud Ascent-benägenhet – <5 licenser | Kund som har en aktuell lokal SQL Server (det vill säga en senare version än EOL). Kunden har färre än 5 licenser. Kunden har ingen benägenhetspoäng. Partnern bör rikta in sig på den här kunden för migrering till Azure. | 
| Migrera – OSS – Migrera till DATABAS med öppen källkod ( OSS) | Befintlig kund med någon av följande konkurrerande produkter: PostgreSQL, MySQL, MariaDB. Partnern bör rikta in sig på den här kunden för migrering till Azure. | 
| Migrera – OSS – Linux på Azure | Befintlig kund med Linux. Partnern bör rikta in sig på den här kunden för migrering till Azure. | 
| Migrera – SAP – SAP på Azure | Befintlig kund med SAP. Partnern bör rikta in sig på den här kunden för migrering till Azure. | 
| Migrera – Windows Virtual Desktop – Fjärrskrivbordstjänster IB | Identifierar kunder med aktiva Windows-Fjärrskrivbordstjänster. Partnern bör rikta in sig på den här kunden för migrering till Azure. | 
| Migrera – Windows Virtual Desktop – Cross Sell Modern Work till Azure/WVD | Identifierar kunder med Microsoft 365 och inte har Azure. Partnern bör rikta in sig på den här kunden för migrering till Azure. | 
| Migrera – VMware IB | Befintlig kund med produkten: VMware. Partnern bör rikta in sig på den här kunden för migrering till Azure. | 
| Migrera – Citrix IB | Befintlig kund med produkten: Citrix Systems. Partnern bör rikta in sig på den här kunden för migrering till Azure. | 
| Innovation – Analytics – Power BI IB med hög benägenhet i Azure | Kunder med och Active Power BI-prenumeration inklusive: Power BI – Fristående Pro, Power BI – Azure-paket, Power BI – Office-paket, Power BI-paket – Microsoft 365 | 
| Aktivera – DevOps med GitHub – Visual Studio/MSDN IB | Identifierar kunder med aktiva Visual Studio versioner | 
| Windows Server Standard-version | Visar versionen av Windows Server Standard-köp av kunden | 
| Windows Server Standard-licens | Visar licenstypen för Windows Server Standard-köp av kunden | 
| Windows Server Data Center-version | Visar versionen av Windows Data Center-köp av kunden | 
| Licens för Windows Server Data Center | Visar licenstypen för Windows Data Center-köp av kunden | 
| AzureFit | Interna och externa datapunkter som definierar företagsgrafiska data. Fit scoring använder en lookalike-modell till vår bästa SMB för att jämföra kunder och se om de är lämpliga för Microsofts molnprodukter. Bedömning av passning uppdateras kvartalsvis. | 
| AzureIntent | Signaler som rör sociala medier och en kunds onlinebeteende definierar Intent. Avsiktsbedömningen överlagras i Anpassa för att definiera klustren. Avsiktsbedömningen uppdateras varje månad. | 
| AzureCluster | Identifierar kundens benägenhet att köpa Azure genom att konsolidera rekommendationerna anpassa och avsikter i ett kluster. Target Act Now och Evaluate clusters, eftersom de ger högre avkastning. Rikta in dig på att utveckla och utbilda kunder om det fortfarande finns kapacitet efter att du riktar in dig på Agera nu och Utvärdera kunder. | 
| WindowsServerDataCenter_HasOpenRenewal | Anger om kunden har en öppen förnyelse för Windows Server Datacenter | 
| WindowsServerStandard_HasOpenRenewal | Anger om kunden har en öppen förnyelse för Windows Server Standard | 
| AzureUpsellCustomer | Identifierar om kunden visar säljförseningar för Azure | 
| Har Google | Identifierar om kunden visar konkurrenssignaler för att äga Google-produkter | 
| Har AWS | Identifierar om kunden visar konkurrenssignaler för att äga AWS-produkter | 
| Har EA | Anger om en förnyelse är en EA- eller EA-prenumeration | 
| Har öppen | Anger om en förnyelse är ett Open- eller Open Value-avtal | 

### <a name="cloud-ascent---agreement-renewal-propensity-report"></a>**Cloud Ascent – rapport om avtalsförnyelseförnyelse**

| Kolumnnamn | Databeskrivning | 
| :--------- | :--------- | 
| MPN-ID | Microsoft Partner Network-ID | 
| Partnernamn | Partnerns namn | 
| Kund-ID | Kundidentifierarnummer | 
| DUNS-nummer | Dun & Bradstreet-numret för den kund som poängsätts för berättigande | 
| Account Name | Namn på kontot | 
| Domain | Domänen för kontot | 
| Organisationsstorlek | Organisationens storlek | 
| Industri | Industri | 
| Lodrät | Vertikalen hos den kund som poängas för benägenhet enligt Microsoft, D&B och andra branschstandarder | 
| Område | Geografiskt område för platsen | 
| Dotterbolag | Dotterbolaget till den kund som poängas för benägenhet | 
| Säljområde | Försäljningsområde för den kund som poängsattes för benägenhet | 
| City | Geografisk ort | 
| Tillstånd | Geografisk plats | 
| Postnummer | Organisationens postnummer | 
| Land | Geografiskt land | 
| Segment | Marknadssegment | 
| Undersegment | Undersegment för marknad | 
| Sammanfattning av SMC-typ | SMC-typ | 
| Översta ohanterade – beräkningsbas | De främsta ohanterade kunderna – beräkning | 
| Översta ohanterade – användarbas | De mest ohanterade kunderna – användare | 
| IsNonProfit | Anger om organisationen är ideell (Ja eller Nej) | 
| Har Google | Identifierar om kunden visar konkurrenssignaler för att äga AWS-produkter | 
| Har AWS | Identifierar om kunden visar konkurrenssignaler för att äga AWS-produkter | 
| Azure-kluster | Identifierar kundens ighet att köpa Azure. Target Act Now och Evaluate clusters, eftersom de ger högre avkastning. Rikta in dig på att utbilda kunder om det fortfarande finns kapacitet efter att du riktar in dig på Agera nu och Utvärdera kunder. | 
| D365 Finance + Operations-kluster | Identifierar kundens ighet att köpa Dynamics 365 Finance and Operations. Kunder som har en ighet för Finance + Operations finns i de främsta ohanterade kategorierna. Target Act Now och Evaluate clusters, eftersom de ger högre avkastning. Rikta in dig på att utbilda kunder om det fortfarande finns kapacitet efter att du riktar in dig på Agera nu och Utvärdera kunder. | 
| D365 CE-kluster | Identifierar kundens ighet att köpa Dynamics 365 Customer Engagement. Kunder som har en öjlighet för Customer Engagement finns i kategorierna Medel och Liten. Target Act Now och Evaluate clusters, eftersom de ger högre avkastning. Rikta in dig på att utbilda kunder om det fortfarande finns kapacitet efter att du riktar in dig på Agera nu och Utvärdera kunder. | 
| D365 BC-kluster | Identifierar kundens ighet att köpa Dynamics 365 Business Central. Kunder som har en ighet för Business Central finns i kategorierna Medel och Liten. Target Act Now och Evaluate clusters, eftersom de ger högre avkastning. Rikta in dig på att utbilda kunder om det fortfarande finns kapacitet efter att du riktar in dig på Agera nu och Utvärdera kunder. | 
| Microsoft 365 kluster | Identifierar kundens ighet att köpa Microsoft 365. Target Act Now och Evaluate clusters, eftersom de ger högre avkastning. Rikta in dig på att utbilda kunder om det fortfarande finns kapacitet efter att du riktar in dig på Agera nu och Utvärdera kunder. | 
| Licensprogram | Identifierar typ av licensprogram för förnyelsen | 
| Avtals-ID | Identifierare för avtalet | 
| Avtalets slutdatum | Avtalets slutdatum | 
| Förfallotyp | Typ av förfallotid | 
| Intäkter som upphör att gälla | Intäkter som är associerade med utgående prenumerationer | 
| Har EA | Anger om en förnyelse är en EA- eller EA-prenumeration | 
| Har öppen | Anger om en förnyelse är ett open- eller open value-avtal | 
| Azure Upsell-kund | Identifierar om kunden visar säljrekvisitet för Azure | 
| Microsoft 365 uppförsäljningskund | Anger om kunden visar huruvida säljförsäljningen är Microsoft 365 | 
| RevSumDivisionName | Identifierar den produkt som är upp för förnyelse | 

## <a name="next-steps"></a>Nästa steg

Mer information finns i Ladda [ned rapporter.](pci-download-reports.md)
