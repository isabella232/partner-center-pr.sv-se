---
title: Datadefinitioner för insikter
ms.topic: article
ms.date: 12/14/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Dokumentet innehåller en lista över olika rapporter och deras data definitioner, som du kan hämta från sidan insikter Hämta rapport.
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 427ca3b60ec527a6a371a232538647448d03b084
ms.sourcegitcommit: 6632d7452be36010bfc8c6823efe5a5197377989
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 01/27/2021
ms.locfileid: "98861401"
---
# <a name="export--data-definitions"></a>Exportera – data definitioner 

 **Lämpliga roller** 

- Rapport visnings program 
- Rapport visnings program för chefer 

## <a name="introduction"></a>Introduktion 

Genom att använda hubben för att ladda ned rapporter på instrument panelen insikter kan du exportera rå data uppsättningar. 

De olika rapporterna, som du kan hämta tillsammans med deras data definitioner, visas i följande tabeller: 

### <a name="partner-profile-report"></a>**Rapporten partner profil**

| Kolumnnamn | Data Beskrivning | 
| :--------- | :--------- | 
| MPNId | Identifierare för Microsoft Partner Network (MPN) | 
| PartnerName | Partnerns namn | 
| PGA_MPNId | Identifierare för den globala partnerns konto MPN | 
| PGA_PartnerName | Globalt konto namn för partner | 
| City | Ortens plats för partnern | 
| Land | Partnerns land plats | 
| HierarchyLevel | Indikerar om det är ett globalt MPN-ID eller platsens MPN-ID | 

### <a name="customer-details-report"></a>**Rapporten kund information**

| Kolumnnamn | Data Beskrivning | 
| :--------- | :--------- | 
| CustomerName | Namnet på kunden | 
| CustomerTenantId | Identifierare för kund innehavaren | 
| CustomerTpid | Identifierare för överordnad kund | 
| CustomerSegment | Kund segment | 
| CustomerMarket | Den geografiska marknaden för kunden | 
| CustomerStatus | Kund status (aktiv eller inaktiv) | 
| Produkt | Produkten som säljs till kunden av MPN: O365, DYNAMICS 365, Enterprise Mobility + Security, Power BI eller Microsoft Azure | 
| SKU | Produkt-SKU | 
| Månad | Månad för vilken användning och intäkter rapporteras | 
| MPNId | Identifierare för Microsoft Partner Network | 
| PartnerName | Partnerns namn | 
| PartnerLocation | Partnerns geografiska plats | 
| PartnerAttributionType | Partnerns typ av behörighet | 
| SalesChannel | Försäljnings kanal | 
| AvailableSeats | Tillgängliga platser | 
| RevenueUSD | Intäkter i USD | 

### <a name="reseller-performance-report"></a>**Prestanda rapport för åter försäljare**

> [!Note]
> Intäkts-och ACR-data är bara tillgängliga för användare som är rapporter i Executive-rapporter.

| Kolumnnamn | Data Beskrivning | 
| :--------- | :--------- | 
| ResellerMPNid | Microsoft Partner Network identifierare för åter försäljare | 
| ResellerName | Återförsäljarens namn | 
| ResellerMarket | Åter försäljar land på marknaden | 
| IndirectProviderMPNId | Identifierare för den indirekta providern Microsoft Partner Network | 
| IndirectProviderName | Namn på indirekt Provider | 
| Månad | Månad för vilken användning och intäkt rapporteras | 
| Produkt | Produktnamn | 
| SubscriptionID | Identifierare för prenumerationen | 
| AvailableSeats | Antal tillgängliga platser | 
| AssignedSeats | Antal tilldelade platser | 
| BilledRevenueUSD | Fakturerad intäkt i USD | 
| CustomerName | Namnet på kunden | 
| CustomerTPid | Identifierare för överordnad kund | 
| CustomerSegment | Kund segment | 
| CustomerMarket | Den geografiska marknaden för kunden | 
| ResellerStatus | Status för åter försäljare | 

### <a name="subscription-details-report"></a>**Rapporten prenumerations information**

>[!Note]
>Intäkts-och ACR-data är bara tillgängliga för användare som är rapporter i Executive-rapporter.

| Kolumnnamn | Data Beskrivning | 
| :--------- | :--------- | 
| SubscriptionId | GUID för prenumerationen | 
| SubscriptionStartDate | Start datum för prenumerationen | 
| SubscriptionEndDate | Slutdatum för prenumerationen | 
| SubscriptionState | Status för prenumerationen (aktiv eller överomsättningen) | 
| Månad | Månad för vilken användning och intäkter rapporteras | 
| IsAutoRenew | Anger om prenumerationen är autoförnyelse (Ja eller Nej) | 
| CustomerName | Namnet på kunden | 
| CustomerTenantId | GUID för kunden | 
| CustomerTpid | Överordnad kund topp identifierare | 
| CustomerSegment | Marknads segment för kunden | 
| CustomerMarket | Den geografiska marknaden för kunden | 
| Produkt | Produkt som säljs till kunden av partnern | 
| SKU | Produkt-SKU för produkten | 
| MPNId | Partnerns Microsoft Partner Network-ID | 
| PartnerName | Partnerns namn | 
| PartnerLocation | Partnerns geografiska plats | 
| PartnerAttributionType | Tilldelnings typ för prenumerationen | 
| SalesChannel | Kanal för Sales – Direct, CSP (Cloud Solution Provider) och så vidare | 
| AvailableSeats | Aktuellt tillgängligt säte | 
| RevenueUSD | Intäkter i USD | 
| Registrerings-ID | Registrerings-ID för prenumerationen | 

### <a name="azure-usage-report"></a>**Användnings rapport för Azure**

| Kolumnnamn | Data Beskrivning | 
| :--------- | :--------- | 
| SubscriptionId | GUID för prenumerationen | 
| SubscriptionStartDate | Datumet då prenumerationen startades | 
| SubscriptionEndDate | Datum för prenumerationens slut | 
| SubscriptionState | Aktuell status för prenumerationen (öppen, stängd, aktiv eller i respitperiod) | 
| Månad | Datum sammanställt per månad | 
| ServiceName | Namnet på Azure-tjänsten | 
| MeterCategory | Namn på mätar kategorin | 
| UsageUnits | Antalet enheter som används under fakturerings perioden | 
| CustomerName | Namnet på kunden | 
| CustomerTenantId | Klient-ID för kunden | 
| CustomerTpid | Överordnad kund topp-ID | 
| CustomerSegment | Kunds segment | 
| CustomerMarket | Den geografiska marknaden för kunden | 
| MPNId | Microsoft Partner Network-ID för kunden | 
| PartnerName | Partnerns namn | 
| PartnerLocation | Den geografiska land platsen för partnern | 
| PartnerAttributionType | Partnerns typ av behörighet | 
| SalesChannel | Försäljnings kanal (direkt/CSP, indirekt/CSP, direkt och så vidare) | 
| ACR_USD | Azures förbrukade intäkter (ACR) i USD | 
| Registrerings-ID | Registrerings-ID för Azure-prenumerationen | 

### <a name="office-365-license-usage-report"></a>**Licens användnings rapport för Office 365**

| Kolumnnamn | Data Beskrivning | 
| :--------- | :--------- | 
| CustomerTenantId | Klient-ID för kunden | 
| CustomerTpid | Överordnad kund topp-ID | 
| WorkloadName | Skype för företag, team, Exchange Online | 
| Månad | Månad för vilken användning rapporteras | 
| PaidAvailableUnits | Antal betalda tillgängliga enheter | 
| MonthlyActiveUsers | Antal aktiva användare per månad | 
| CustomerName | Namnet på kunden | 
| CustomerMarket | Geografisk plats för kundens marknad | 
| CustomerSegment | Kund segment | 
| MPNId | Identifierare för Microsoft Partner Network | 
| PartnerName | Partnerns namn | 
| PartnerLocation | Partnerns geografiska plats | 
| PartnerAttributionType | Partnerns typ av behörighet | 

### <a name="enterprise-mobility-license-usage-report"></a>**Användnings rapport över Enterprise Mobility Licensing**

| Kolumnnamn | Data Beskrivning | 
| :--------- | :--------- | 
| CustomerTenantId | Klient-ID för kunden | 
| CustomerTpid | Överordnad kund topp-ID | 
| WorkloadName | Namnet på Enterprise Mobility + Security (EMS) arbets belastningen | 
| Månad | Månad för vilken användning rapporteras | 
| PaidAvailableUnits | Antal betalda tillgängliga enheter | 
| MonthlyActiveUsers | Antal aktiva användare per månad | 
| CustomerName | Namnet på kunden | 
| CustomerMarket | Geografisk plats för kundens marknad | 
| CustomerSegment | Kund segment | 
| MPNId | Identifierare för Microsoft Partner Network | 
| PartnerName | Partnerns namn | 
| PartnerLocation | Partnerns geografiska plats | 
| PartnerAttributionType | Partnerns typ av behörighet | 

### <a name="dynamics-365-license-usage-report"></a>**Licens användnings rapport för Dynamics 365**

| Kolumnnamn | Data Beskrivning | 
| :--------- | :--------- | 
| SubscriptionId | GUID för prenumerationen | 
| SubscriptionStartDate | Start datum för prenumerationen | 
| SubscriptionEndDate | Slutdatum för prenumerationen | 
| SubscriptionStatus | Status för prenumerationen | 
| Månad | Månad för vilken användning rapporteras | 
| RevSumDivisionName | Namn på rev sum-divisionen | 
| RevSumCategoryName | Namnet på rev sum-kategorin | 
| SKU | Produkt-SKU för produkten | 
| SKUId | SKU-ID för produkten | 
| FreeVsPaidSKU | Anger om det är en kostnads fri eller betald SKU | 
| SalesModel | Försäljnings kanal som används för att sälja prenumerationen | 
| DetailedSalesModel | Detaljerad försäljnings modell för prenumerationen | 
| CustomerName | Namnet på kunden | 
| CustomerTenantId | GUID för kund innehavaren | 
| CustomerTpid | Överordnad kund topp identifierare | 
| CustomerSegment | Marknads segment för kunden | 
| CustomerMarket | Den geografiska marknaden för kunden | 
| MPNId | Identifierare för Microsoft Partner Network | 
| PartnerName | Partnerns namn | 
| PartnerLocation | Den geografiska land platsen för partnern | 
| PartnerAttachType | Tilldelnings typ för prenumerationen | 
| AvailableSeats | Aktuellt tillgängligt säte | 
| AssignedSeats | Aktuellt tilldelat säte | 
| ActiveSeats | Aktuella aktiva platser | 
| DeploymentOpportunity | Aktuell distributions möjlighet | 
| ActiveUsagePercent | Aktuell aktiv användning i procent | 

### <a name="power-bi-license-usage-report"></a>**Power BI licens användnings rapport**

| Kolumnnamn | Data Beskrivning | 
| :--------- | :--------- | 
| SubscriptionId | GUID för prenumerationen | 
| SubscriptionStartDate | Start datum för prenumerationen | 
| SubscriptionEndDate | Slutdatum för prenumerationen | 
| SubscriptionStatus | Status för prenumerationen (aktiv, inaktiv eller i respitperiod) | 
| Månad | Datum sammanställt per månad | 
| SKU | Produkt-SKU för produkten | 
| SKUId | SKU-ID för produkten | 
| FreeVsPaidSKU | Kostnads fri eller betald SKU-differentiering | 
| SalesModel | Försäljnings modell som används för att sälja prenumerationen | 
| DetailedSalesModel | Detaljerad försäljnings modell för prenumerationen | 
| CustomerName | Namnet på kunden | 
| CustomerTenantId | GUID för kund innehavaren | 
| CustomerTpid | Identifierare för överordnad kund | 
| CustomerSegment | Marknads segment för kunden | 
| CustomerMarket | Den geografiska marknaden för kunden | 
| MPNId | Identifierare för Microsoft Partner Network | 
| PartnerName | Partnerns namn | 
| PartnerLocation | Den geografiska land platsen för partnern | 
| PartnerAttachType | Tilldelnings typ för prenumerationen | 
| AvailableSeats | Aktuella tillgängliga platser | 
| AssignedSeats | Aktuella tilldelade platser | 
| ActiveSeats | Aktuella aktiva platser | 
| DeploymentOpportunity | Aktuell distributions möjlighet | 
| ActiveUsagePercent | Aktuell aktiv användning i procent | 

### <a name="teams-meetings-and-calls-report"></a>**Rapport över team möten och samtal**

| Kolumnnamn | Data Beskrivning | 
| :--------- | :--------- | 
| CustomerTenantId | Klient-ID för kunden | 
| CustomerTpid | Identifierare för överordnad kund | 
| Månad | Månad för vilken användning rapporteras | 
| Under arbets belastning | Under arbets belastning för vilken användning rapporteras (möten, samtal eller telefon system) | 
| Antal möten | Antal möten | 
| Mötets varaktighet | Total Mötes varaktighet i timmar | 

### <a name="teams-monthly-usage-report"></a>**Rapport över månatliga användnings grupper**

| Kolumnnamn | Data Beskrivning | 
| :--------- | :--------- | 
| CustomerTenantId | Klient-ID för kunden | 
| CustomerTpid | Identifierare för överordnad kund | 
| Månad | Månad för vilken användning rapporteras | 
| Under arbets belastning | Under arbets belastning för vilken användning rapporteras (möten, samtal eller telefon system) | 
| Skriv bords användare | Antal användare som använder team på Skriv bordet | 
| Mobila användare | Antal användare som använder team på mobilen | 
| Webb användare | Antal användare som använder team på webben | 
| AllUpParticipants | Antal unika team användare för månaden | 

### <a name="teams-usage-3p-apps-report"></a>**Rapport över team användning 3P-appar**

| Kolumnnamn | Data Beskrivning | 
| :--------- | :--------- | 
| CustomerTenantId | Klient-ID för kunden | 
| CustomerTpid | Överordnad kund topp-ID | 
| Månad | Månad för vilken användning rapporteras | 
| Namn på 3P-app | Namn på Team-appen | 
| Antal användare | Antal användare för appen | 


### <a name="training-details-report"></a>**Kurs informations rapport**

| Kolumnnamn | Data Beskrivning | 
| :--------- | :--------- | 
| TrainingActivityId | ID för utbildningen | 
| TrainingTitle | Rubrik på utbildningen | 
| TrainingType | Typ av utbildning (certifiering eller tentamen) | 
| IndividualFirstName | Förnamn för kunden | 
| IndividualLastName | Kundens efter namn | 
| E-post | Personligt e-post-ID för kunden | 
| CorpEmail | Office-e-post-ID för kunden | 
| TrainingCompletionDate | Slut för ande datum för utbildningen | 
| Månad | Månad för vilken data rapporteras | 
| IcMCP | Anger om användaren är Microsoft Certified Professional (MCP) | 
| MCPID | MCP-ID för användaren | 
| MPNId | Identifierare för Microsoft Partner Network | 
| PartnerName | Partnerns namn | 
| PartnerCityLocation | Partnerns geografiska ort plats | 
| PartnerCountryLocation | Den geografiska land platsen för partnern | 

### <a name="microsoft-learn-report"></a>**Microsoft Learn rapport**

| Kolumnnamn | Data Beskrivning | 
| :--------- | :--------- | 
| Användarnamn | Användarens namn | 
| UserId | Användarens GUID | 
| TrainingName | Utbildnings namn | 
| TrainingType | Typ av utbildning (modul eller utbildnings väg) | 
| Produkter | Produkt för vilken inlärnings modulen gäller | 
| Roller | Relevanta roller för utbildningen | 
| CompletionDate | Datum för slutförd träning | 
| MPNId | Identifierare för Microsoft Partner Network | 
| PartnerName | Partnerns namn | 
| Land | Den geografiska land platsen för partnern | 

### <a name="competency-summary-and-history-report"></a>**Rapport om kompetens Sammanfattning och historik**

| Kolumnnamn | Data Beskrivning | 
| :--------- | :--------- | 
| CompetencyName | Kompetensens namn | 
| CompetencyLevel | Kompetens nivå (guld eller silver) | 
| CompetencyStatus | Aktuell status för kompetensen (aktiv, inaktiv eller i respitperiod) | 
| CompetencyStartDate | Start datum för kompetensen | 
| CompetencyEndDate | Slutdatum för kompetensen | 

### <a name="competency-performance-report"></a>**Prestanda rapport för kompetens**

| Kolumnnamn | Data Beskrivning | 
| :--------- | :--------- | 
| CompetencyName | Kompetensens namn | 
| CompetencyAttainmentOptionName | Namn på alternativet för att erhålla kompetens | 
| Månad | Månad för vilken måtten rapporteras | 
| MetricName | Namnet på det mått som är relevant för kompetensen | 
| MetricMonthlyContribution | Månatligt bidrag för måttet | 
| TTMAggregate | Aggregerade mått för de efterföljande 12 månaderna | 
| AnniversaryYearAggregate | Aggregerad mått för innevarande jubileums år | 
| GoldThreshold | Prestanda krav för att uppfylla guld kompetensen | 
| SilverThreshold | Prestanda krav för att uppfylla silver kompetensen | 

### <a name="cloud-ascent---microsoft-365-propensity-report"></a>**Molnbaserad stigning – Microsoft 365 benägenhet-rapport**

| Kolumnnamn | Data Beskrivning | 
| :--------- | :--------- | 
| MPN-ID | Microsoft Partner Network-ID | 
| Partner namn | Partnerns namn | 
| Kund-ID | ID-nummer för kunden | 
| DUNS-nummer | Dun & Bradstreet-numret (D&B) för kunden som poängs ätter för benägenhet | 
| Kontonamn | Namn på kontot | 
| Domain | Kontots domän | 
| Organisations storlek | Organisationens storlek | 
| Industri | Bransch som organisationen tillhör | 
| Lodrät | Den lodräta för kunden som poängs ätter för benägenhet, som identifieras av Microsoft, D&B och andra bransch standarder | 
| Område | Geografiskt område på platsen | 
| Dotterbolag | Dotter bolag till kunden som har Poäng för benägenhet | 
| Säljområde | Försäljnings området för kunden som poängs ätter för benägenhet | 
| City | Organisationens geografiska ort | 
| Stat | Organisationens geografiska tillstånds plats | 
| Postnummer | Post nummer för organisationen | 
| Land | Organisationens geografiska landskod | 
| Segment | Marknads segment | 
| Del segment | Marknads del segment | 
| Översikt över SMC-typ | SMC-typ | 
| Topp ohanterad – beräknings bas | Främsta ohanterade kunder – beräkning | 
| Topp ohanterad-användar bas | Vanligaste ohanterade kunder – användare | 
| IsNonProfit | Anger om organisationen är ideell (Ja eller Nej) | 
| Aktivera fjärran sluten arbete – rikta Exchange Online | Kunder som har en aktiv prenumeration på Exchange Online, merförsäljning till Microsoft 365 | 
| Aktivera fjärran sluten arbete – lokal förvärv (aktuell version) med benägenhet i moln stigning – + 10 licenser | Kund som har en aktuell lokal Office-eller Windows-klient. Det vill säga klient versionen är senare än en EOL-version (End of Life). Kunden har 10 eller fler licenser. Kund som har en benägenhet poäng. Partner ska vara mål för konvertering till Microsoft 365. | 
| Aktivera fjärran sluten arbete – lokal hämtning (aktuell version) med <benägenhet 10 licenser för moln stigning | Kund som har en aktuell lokal Office-eller Windows-klient (det vill säga en senare version än EOL). Kunden har färre än 10 licenser. Kund som har en benägenhet poäng. Partner ska vara mål för konvertering till Microsoft 365. | 
| Aktivera fjärran sluten arbete – lokal förvärv (aktuell version) utan uppstigning benägenhet-+ 10 licenser | Kund som har en aktuell lokal Office-eller Windows-klient (det vill säga en senare version än EOL). Kunden har 10 eller fler licenser. Kunden har inget benägenhet poäng. Partner ska vara mål för konvertering till Microsoft 365. | 
| Aktivera fjärran sluten arbete – lokal förvärv (aktuell version) utan <benägenhet 10 licenser för moln stigning | Kund som har en aktuell lokal Office-eller Windows-klient (det vill säga en senare version än EOL). Kunden har färre än 10 licenser. Kunden har inget benägenhet poäng. Partner ska vara mål för konvertering till Microsoft 365. | 
| Aktivera fjärran sluten arbete – lokal hämtning (EOL-version) med benägenhet för moln stigning – + 10 licenser | Kund som har en EOL lokal Office-eller Windows-klient (dvs. en EOL-version eller tidigare). Kunden har 10 eller fler licenser. Kunden har en benägenhet poäng. Partner ska vara mål för konvertering till Microsoft 365. | 
| Aktivera fjärran sluten arbete – lokal hämtning (EOL-version) med benägenhet i molnet-<10 licenser | Kund som har en EOL lokal Office-eller Windows-klient (dvs. en EOL-version eller tidigare). Kunden har färre än 10 licenser. Kunden har en benägenhet poäng. Partner ska vara mål för konvertering till Microsoft 365. | 
| Aktivera fjärran sluten arbete – lokal hämtning (EOL-version) utan benägenhet-+ 10-licenser för molnet | Kund som har en aktuell lokal Office-eller Windows-klient (dvs. en EOL-version eller tidigare). Kunden har 10 eller fler licenser. Kunden har inget benägenhet poäng. Partner ska vara mål för konvertering till Microsoft 365. | 
| Aktivera fjärran sluten arbete – lokal hämtning (EOL-version) utan benägenhet-<10 licenser | Kund som har en aktuell lokal Office-eller Windows-klient (dvs. en EOL-version eller tidigare). Kunden har färre än 10 licenser. Kunden har inget benägenhet poäng. Partner ska vara mål för konvertering till Microsoft 365. | 
| Aktivera fjärrarbete – hög benägenhet potentiell kund för Microsoft 365 (Act-NowithEvaluate) | Kund kunder med hög benägenhet för Microsoft 365 | 
| Aktivera fjärran slutet arbete – konkurrerande (zoom) med Microsoft 365 | Kunden med zoomnings-och Microsoft 365 mål för konvertering till team | 
| Aktivera fjärran slutet arbete (zoom) utan Microsoft 365 | Kunden med zoom, mål för konvertering till Teams | 
| Minska kostnaderna och hantera Microsoft 365 E3 riktade mot Microsoft 365 E5 | Befintlig kund med Microsoft 365 E3, mål för Microsoft 365 E5 | 
| Minska kostnaderna och hantera Microsoft 365 Business Basic-och Business Standard-kunder som är riktade till Microsoft 365 Business Premium | Befintliga Microsoft 365 Business Basic-och Business Standard-kunder, mål för Microsoft 365 Business Premium | 
| Transformera organisationens produktivitet – benägenhet | Kunden visar en benägenhet för Surface | 
| M365Cluster | Identifierar en kunds benägenhet att köpa Microsoft 365. Mål Act och utvärderar kluster eftersom det ger högre avkastning. Rikta in dig på Nurture och utbilda kunder endast om det fortfarande finns kapacitet efter att ha agerat och utvärdera kunderna. | 
| M365Fit | Interna och externa data punkter som definierar firmographics. Anpassnings bedömnings använder en lookalike modell för våra bästa små eller medel stora företag (SMB) för att jämföra kunder och se om de är en potentiell anpassning för Microsofts moln produkter. Anpassnings resultat uppdateras kvartals vis. | 
| M365Intent | Signaler som rör sociala medier och en kunds beteende för online-beteende definierar avsikt. Poängen för avsikt är att anpassas till att definiera klustren. Avsikts poängen uppdateras varje månad. | 
| SurfaceCluster | Identifierar en kunds benägenhet till köp-ytan genom att konsolidera anpassnings-och avsikts rekommendationerna i ett kluster. Mål Act och utvärderar kluster eftersom det ger högre avkastning. Rikta in dig på Nurture och utbilda kunder endast om det fortfarande finns kapacitet efter att ha agerat och utvärdera kunderna. | 
| SurfaceFit | Interna och externa data punkter som definierar firmographics. Anpassnings bedömnings använder en lookalike modell till våra bästa SMB: er för att jämföra kunder och se om de är en potentiell anpassning för Microsofts moln produkter. Anpassnings resultat uppdateras kvartals vis. | 
| SurfaceIntent | Signaler som rör sociala medier och en kunds beteende för online-beteende definierar avsikt. Poängen för avsikt är att anpassas till att definiera klustren. Avsikts poängen uppdateras varje månad. | 
| O365Cluster | Identifierar kundens benägenhet för att köpa Office 365. Mål Act och utvärderar kluster eftersom det ger högre avkastning. Rikta in dig på Nurture och utbilda kunder endast om det fortfarande finns kapacitet efter att ha agerat och utvärdera kunderna. | 
| O365Fit | Interna och externa data punkter som definierar firmographics. Anpassnings bedömnings använder en lookalike modell till våra bästa SMB: er för att jämföra kunder och se om de är en potentiell anpassning för Microsofts moln produkter. Anpassnings resultat uppdateras kvartals vis. | 
| O365Intent | Signaler som rör sociala medier och en kunds beteende för online-beteende definierar avsikt. Poängen för avsikt är att anpassas till att definiera klustren. Avsikts poängen uppdateras varje månad. | 
| M365UpsellCustomer | Identifierar om kunden visar merförsäljning-benägenhet för Microsoft 365 | 
| Har Google | Identifierar om kunden visar konkurrerande signaler för att äga Google-produkter | 
| Har AWS | Identifierar om kunden visar konkurrerande signaler för ägande Amazon Web Services-produkter (AWS) | 
| Har EA | Identifierar om en förnyelse är ett Enterprise-avtal (EA) eller en EA-prenumeration | 
| Har öppen | Identifierar om en förnyelse är ett avtal med öppen eller öppen värde | 

### <a name="cloud-ascent---dynamics-365-propensity-report"></a>**Molnbaserad stigning – Dynamics 365 benägenhet-rapport**

| Kolumnnamn | Data Beskrivning | 
| :--------- | :--------- | 
| MPN-ID | Microsoft Partner Network-ID | 
| Partner namn | Partnerns namn | 
| Kund-ID | Kund-ID-nummer | 
| DUNS-nummer | Dun & Bradstreet-numret för kunden som poängs ätter för benägenhet | 
| Kontonamn | Namn på kontot | 
| Domain | Kontots domän | 
| Organisations storlek | Organisationens storlek | 
| Industri | Bransch som organisationen tillhör | 
| Lodrät | Den lodräta för kunden som poängs ätter för benägenhet, som identifieras av Microsoft, D&B och andra bransch standarder
| Område | Geografiskt område på platsen | 
| Dotterbolag | Dotter bolag till kunden som har Poäng för benägenhet | 
| Säljområde | Försäljnings området för kunden som poängs ätter för benägenhet | 
| City | Geografisk ort plats | 
| Stat | Geografisk tillstånds plats | 
| Postnummer | Post nummer för organisationen | 
| Land | Plats för geografiskt land | 
| Segment | Marknads segment | 
| Del segment | Marknads del segment | 
| Översikt över SMC-typ | Kategoriseringen av en kund: främsta ohanterade användar baser är kunder med 300 och anställda, topp ohanterade beräknings baser är kunder med USD10, 000 i Azure tre års potential, medel stora företag är kunder med 25 anställda eller större och små företag är kunder med färre än 25 anställda. | 
| Topp ohanterad – beräknings bas | Främsta ohanterade kunder – beräkning | 
| Topp ohanterad-användar bas | Vanligaste ohanterade kunder – användare | 
| IsNonProfit | Anger om organisationen är ideell (Ja eller Nej) | 
| Aktivera digital försäljning – Microsoft 365-plats storlek >= 25 platser (SalesPro benägenhet Model) | Kunden utan Dynamics 365. Plats storlek: 25 +. Partner ska vara mål för över-försäljning av Dynamics 365-SalesPro. | 
| Aktivera digital försäljning – Dynamics 365 SalesPro benägenhet (agera nu eller utvärdera) | Kunder med höga benägenhet utan Dynamics 365. Partner ska vara mål för Dynamics 365-SalesPro. | 
| Hantering av ekonomisk risk & bedrägeri-Dynamics lokal installation bas – Navision (företags Central benägenhet-modell) | Befintlig kund med lokalt Navision. Partner ska vara mål för Dynamics 365 Business Central. | 
| Hantering av ekonomisk risk & bedrägerier – Dynamics lokal installation Base-Dynamics AX (Dynamics 365 finans + Operations benägenhet Model) | Befintlig kund med lokal AX. Partner ska vara mål för Dynamics 365 finans + Operations. | 
| Hantering av ekonomisk risk & bedrägeri-Dynamics lokala installations Base – Great Plains (företags Central benägenhet modell) | Befintlig kund med lokala fantastiska Plains-enheter. Partner ska vara mål för Dynamics 365 Business Central. | 
| Hantering av ekonomisk risk & bedrägerier – Dynamics lokal installation Base-Salomonöarna (företags Central benägenhet-modell) | Befintlig kund med lokal Salomonöarna. Partner ska vara mål för Dynamics 365 Business Central. | 
| Hantering av ekonomisk risk & bedrägeri-Dynamics lokala installations Base – andra (företags Central benägenhet-modell) | Befintlig kund med andra lokala lösningar som inte tidigare har listats. Partner ska vara mål för Dynamics 365 Business Central. | 
| Bygg flexibla affärs processer – Dynamics lokal installation Base-AX/GP/SL/NAV/övrigt (Dynamics 365 benägenhet-modell) | Bygg flexibla affärs processer – Dynamics lokal installation Base-AX/GP/SL/NAV/övrigt (Dynamics 365 benägenhet-modell) | 
| Bygg Agile-affärsprocesser – Dynamics-konkurrens för grund-Mendix/-system/Salesforce (Dynamics 365 benägenhet Model) | Bygg Agile-affärsprocesser – Dynamics-konkurrens för grund-Mendix/-system/Salesforce (Dynamics 365 benägenhet Model) | 
| Bygg flexibla affärs processer – Dynamics 365 finans + Operations install Base | Befintliga Dynamics 365-finans + drifts kunder. Partner för att rikta in Power Apps. | 
| Bygg flexibla affärs processer – Dynamics 365 Business Central install Base | Befintliga Dynamics 365 Business Central-kunder. Partner för att rikta in Power Apps. | 
| Bygg Agile-affärsprocesser – Dynamics 365-installations bas för kund engagemang | Befintliga Dynamics 365-kunder för kund engagemang. Partner för att rikta in Power Apps. | 
| Bygg en elastisk försörjnings kedja – Windows och aktivera första Dynamics 365-arbetsbelastningen som Dynamics 365-hantering av leverans kedjan med icke-Oracle-eller SAP ERP-kunder (Enterprise Resource Planning) | Mål kunder för Dynamics 365-hantering av leverans kedjan | 
| Bygg en elastisk försörjnings kedja – en över gång till Dynamics 365-hantering av leverans kedjan och/eller detalj handel eller Commerce till befintliga kunder med kund engagemang i Dynamics 365 | Befintliga Dynamics 365 kund engagemang-kunder för att rikta in sig på en försäljnings kedja i Dynamics 365. | 
| Bygg en elastisk försörjnings kedja – en över gång till Dynamics 365-hantering av leverans kedjan och/eller detalj handel eller Commerce till Dynamics 365 kund engagemang och Oracle eller SAP | Befintliga Dynamics 365 kund engagemang kunder med Oracle eller SAP för att rikta in sig på Dynamics 365-hantering av leverans kedjan | 
| D365BCCluster | Identifierar kundens benägenhet för att köpa Dynamics 365 Business Central. Kunder som visar en benägenhet for Business Central kommer att ingå i kategorierna medel och liten. Mål Act nu och utvärderar kluster, eftersom de kommer att producera högre avkastning. Rikta in dig på Nurture och utbilda kunder enbart om det fortfarande finns kapacitet efter att du har riktat in dig på att utvärdera kunderna. | 
| D365BCFit | Interna och externa data punkter som definierar firmographics. Anpassnings bedömnings använder en lookalike modell till vårt bästa SMB för att jämföra kunder och se om de är en potentiell anpassning för Microsofts moln produkter. Anpassnings resultat uppdateras kvartals vis. | 
| D365BCIntent | Signaler som rör sociala medier och en kunds beteende för online-beteende definierar avsikt. Poängen för avsikt är att anpassas till att definiera klustren. Avsikts poängen uppdateras varje månad. | 
| D365FOCluster | Identifierar kundens benägenhet för att köpa Dynamics 365-ekonomi och-åtgärder. Kunder som visar en benägenhet för finans + Operations visas i de översta ohanterade kategorierna. Mål Act nu och utvärderar kluster, eftersom de kommer att producera högre avkastning. Rikta in dig på Nurture och utbilda kunder enbart om det fortfarande finns kapacitet efter att du har riktat in dig på att utvärdera kunderna. | 
| D365FOFit | Interna och externa data punkter som definierar firmographics. Anpassnings bedömnings använder en lookalike modell till vårt bästa SMB för att jämföra kunder och se om de är en potentiell anpassning för Microsofts moln produkter. Anpassnings resultat uppdateras kvartals vis. | 
| D365FOIntent | Signaler som rör sociala medier och en kunds beteende för online-beteende definierar avsikt. Poängen för avsikt är att anpassas till att definiera klustren. Avsikts poängen uppdateras varje månad. | 
| D365CECluster | Identifierar kundens benägenhet för att köpa Dynamics 365 kund engagemang. Kunder som visar en benägenhet för kund engagemang kommer att ingå i kategorierna medel och liten. Mål Act nu och utvärderar kluster, eftersom de kommer att producera högre avkastning. Rikta in dig på Nurture och utbilda kunder enbart om det fortfarande finns kapacitet efter att du har riktat in dig på att utvärdera kunderna. | 
| D365CEFit | Anger anpassning för Dynamics 365 kund engagemang | 
| D365CEIntent | Anger avsikt för kund engagemang i Dynamics 365 | 
| DynamicsOnPremAXorCRM_HasOpenRenewal | Identifierar om kunden har en öppen förnyelse för Dynamics lokal AX eller CRM | 
| M365UpsellCustomer | Identifierar om kunden visar merförsäljning-benägenhet för Microsoft 365 | 
| Har Google | Identifierar om kunden visar konkurrerande signaler för att äga Google-produkter | 
| Har AWS | Identifierar om kunden visar konkurrens bara signaler för ägande AWS-produkter | 
| Har EA | Identifierar om en förnyelse är en EA-eller EA-prenumeration | 
| Har öppen | Identifierar om en förnyelse är ett avtal med öppen eller öppen värde | 

### <a name="cloud-ascent---azure-propensity-report"></a>**Moln stigning – Azure benägenhet-rapport**

| Kolumnnamn | Data Beskrivning | 
| :--------- | :--------- | 
| MPN-ID | Microsoft Partner Network-ID | 
| Partner namn | Partnerns namn | 
| Kund-ID | Kund-ID-nummer | 
| DUNS-nummer | Dun & Bradstreet-numret för kunden som poängs ätter för benägenhet | 
| Kontonamn | Namn på kontot | 
| Domain | Kontots domän | 
| Organisations storlek | Organisationens storlek | 
| Industri | Industri | 
| Lodrät | Den lodräta för kunden som poängs ätter för benägenhet, som identifieras av Microsoft, D&B och andra bransch standarder | 
| Område | Geografiskt område på platsen | 
| Dotterbolag | Dotter bolag till kunden som har Poäng för benägenhet | 
| Säljområde | Försäljnings området för kunden som poängs ätter för benägenhet | 
| City | Geografisk ort plats | 
| Stat | Geografisk tillstånds plats | 
| Postnummer | Post nummer för organisationen | 
| Land | Plats för geografiskt land | 
| Segment | Marknads segment | 
| Del segment | Marknads del segment | 
| Översikt över SMC-typ | SMC-typ | 
| Topp ohanterad – beräknings bas | Främsta ohanterade kunder – beräkning | 
| Topp ohanterad-användar bas | Vanligaste ohanterade kunder – användare | 
| IsNonProfit | Anger om organisationen är ideell (Ja eller Nej) | 
| Migrate-EOL Windows Server-EOL Windows Server IB med Cloud-stigning benägenhet-5 + licenser | Kund som har en EOL lokal Windows Server (dvs. en EOL-version eller tidigare). Kunden har 5 eller fler licenser. Kund som har en benägenhet poäng. Partner ska rikta in sig på den här kunden för migrering till Azure. | 
| Migrate-EOL Windows Server-EOL Windows Server IB med Cloud stigning benägenhet-<5 licenser | Kund som har en EOL lokal Windows Server (dvs. en EOL-version eller tidigare). Kunden har färre än 5 licenser. Kund som har en benägenhet poäng. Partner ska rikta in sig på den här kunden för migrering till Azure. | 
| Migrate-EOL Windows Server-EOL Windows Server IB utan att du behöver använda en moln nedstapel benägenhet-5 + licenser | Kund som har en EOL lokal Windows Server (dvs. en EOL-version eller tidigare). Kunden har fler än 5 licenser. Kunden har inget benägenhet poäng. Partner ska rikta in sig på den här kunden för migrering till Azure. | 
| Migrate-EOL Windows Server-EOL Windows Server IB utan moln nedstigning benägenhet-<5 licenser | Kund som har en EOL lokal Windows Server (dvs. en EOL-version eller tidigare). Har färre än 5 licenser. Kunden har inget benägenhet poäng. Partner ska rikta in sig på den här kunden för migrering till Azure. | 
| Migrera-EOL SQL-EOL SQL Server IB med molnets stigning benägenhet-5 + licenser | Kund som har en EOL lokal SQL Server (det vill säga en EOL-version eller tidigare). Kunden har 5 licenser. Kunden har en benägenhet poäng. Partner ska rikta in sig på den här kunden för migrering till Azure. | 
| Migrera-EOL SQL-EOL SQL Server IB med benägenhet-<5-licenser | Kund som har en EOL lokal SQL Server (det vill säga en EOL-version eller tidigare). Har färre än 5 licenser. Kund som har en benägenhet poäng. Partner ska rikta in sig på den här kunden för migrering till Azure. | 
| Migrera-EOL SQL-EOL SQL Server IB utan att du behöver ha en benägenhet på 5 + licenser | Kund som har en EOL lokal SQL Server (det vill säga en EOL-version eller tidigare). Kunden har 5 eller fler licenser. Kunden har inget benägenhet poäng. Partner ska rikta in sig på den här kunden för migrering till Azure. | 
| Migrera-EOL SQL-EOL SQL Server IB utan 5 <-licenser för moln stigning | Kund som har en EOL lokal SQL Server (det vill säga en EOL-version eller tidigare). Kunden har färre än 5 licenser. Kunden har inget benägenhet poäng. Partner ska rikta in sig på den här kunden för migrering till Azure. | 
| Migrera – migrera lokalt Windows Server – aktuell Windows Server IB med molnbaserad benägenhet – 5 + licenser | Kunden som har en aktuell lokal Windows Server (dvs. en senare version än EOL). Kunden har 5 licenser. Kunden har en benägenhet poäng. Partner ska rikta in sig på den här kunden för migrering till Azure. | 
| Migrera – migrera lokalt Windows Server – aktuell Windows Server IB med molnbaserad benägenhet-<5-licenser | Kunden som har en aktuell lokal Windows Server (dvs. en senare version än EOL). Kunden har färre än 5 licenser. Kunden har en benägenhet poäng för Azure. Partner ska rikta in sig på den här kunden för migrering till Azure. | 
| Migrera – migrera lokalt Windows Server – aktuell Windows Server IB utan benägenhet – 5 + licenser | Kunden som har en aktuell lokal Windows Server (dvs. en senare version än EOL). Kunden har 5 licenser. Kunden har inget benägenhet poäng. Partner ska rikta in sig på den här kunden för migrering till Azure. | 
| Migrera – migrera lokalt Windows Server – aktuell Windows Server IB utan benägenhet 5 <-licenser för moln stigning | Kunden som har en aktuell lokal Windows Server (dvs. en senare version än EOL). Kunden har färre än 5 licenser. Kunden har inget benägenhet poäng. Partner ska rikta in sig på den här kunden för migrering till Azure. | 
| Migrera – migrera till Azure SQL eller SQL Virtual Machines (VM) – aktuellt SQL Server IB med benägenhet i molnet, 5 + licenser | Kunden som har en aktuell lokal SQL Server (det vill säga en senare version än EOL). Kunden har 5 licenser. Kunden har en benägenhet poäng. Partner ska rikta in sig på den här kunden för migrering till Azure. | 
| Migrera – migrera till Azure SQL-eller SQL-VM – aktuell SQL Server IB med benägenhet i molnet, <5 licenser | Kunden som har en aktuell lokal SQL Server (det vill säga en senare version än EOL). Kunden har färre än 5 licenser. Kunden har en benägenhet poäng. Partner ska rikta in sig på den här kunden för migrering till Azure. | 
| Migrera – migrera till Azure SQL eller SQL VM-Current SQL Server IB utan benägenhet-5 + licenser | Kunden som har en aktuell lokal SQL Server (det vill säga en senare version än EOL). Kunden har 5 licenser. Kunden har inget benägenhet poäng. Partner ska rikta in sig på den här kunden för migrering till Azure. | 
| Migrera – migrera till Azure SQL-eller SQL-VM – aktuell SQL Server IB utan benägenhet-<5-licenser | Kunden som har en aktuell lokal SQL Server (det vill säga en senare version än EOL). Kunden har färre än 5 licenser. Kunden har inget benägenhet poäng. Partner ska rikta in sig på den här kunden för migrering till Azure. | 
| Migrera – OSS – migrera till Open Source Shakespeare (OSS) DB | Befintlig kund med någon av följande konkurrerande produkter: PostgreSQL, MySQL, MariaDB. Partner ska rikta in sig på den här kunden för migrering till Azure. | 
| Migrera – OSS – Linux på Azure | Befintlig kund med Linux. Partner ska rikta in sig på den här kunden för migrering till Azure. | 
| Migrera – SAP – SAP på Azure | Befintlig kund med SAP. Partner ska rikta in sig på den här kunden för migrering till Azure. | 
| Migrera – Windows Virtual Desktop – Fjärrskrivbordstjänster IB | Identifierar kunder med aktiva Windows-Fjärrskrivbordstjänster. Partner ska rikta in sig på den här kunden för migrering till Azure. | 
| Migrera – Windows Virtual Desktop – mellan Sälj modern arbete i Azure/WVD | Identifierar kunder med Microsoft 365 och har inte Azure. Partner ska rikta in sig på den här kunden för migrering till Azure. | 
| Migrera – VMware IB | Befintlig kund med produkten: VMware. Partner ska rikta in sig på den här kunden för migrering till Azure. | 
| Migrera – Citrix IB | Befintlig kund med produkten: Citrix Systems. Partner ska rikta in sig på den här kunden för migrering till Azure. | 
| Förnya-Analytics-Power BI IB med hög Azure-benägenhet | Kunder med och aktiva Power BI prenumeration, inklusive: Power BI fristående Pro, Power BI – Azure-paket, Power BI-Office-paket, Power BI Suites – Microsoft 365 | 
| Enable-DevOps med GitHub-Visual Studio/MSDN IB | Identifierar kunder med aktiva Visual Studio-versioner | 
| Windows Server Standard-version | Visar versionen av Windows Server standard-inköp från kunden | 
| Windows Server standard-licens | Visar licens typen för Windows Server standard-inköp av kunden | 
| Windows Server Data Center-version | Visar versionen av Windows Data Center-köp av kunden | 
| Windows Server Data Center-licens | Visar licens typen för Windows Data Center-köp av kunden | 
| AzureFit | Interna och externa data punkter som definierar firmographics. Anpassnings bedömnings använder en lookalike modell till vårt bästa SMB för att jämföra kunder och se om de är en potentiell anpassning för Microsofts moln produkter. Anpassnings resultat uppdateras kvartals vis. | 
| AzureIntent | Signaler som rör sociala medier och en kunds beteende för online-beteende definierar avsikt. Poängen för avsikt är att anpassas till att definiera klustren. Avsikts poängen uppdateras varje månad. | 
| AzureCluster | Identifierar kundens benägenhet för att köpa Azure genom att konsolidera anpassnings-och avsikts rekommendationerna i ett kluster. Mål Act nu och utvärderar kluster, eftersom de kommer att producera högre avkastning. Rikta in dig på Nurture och utbilda kunder enbart om det fortfarande finns kapacitet efter att du har riktat in dig på att utvärdera kunderna. | 
| WindowsServerDataCenter_HasOpenRenewal | Identifierar om kunden har en öppen förnyelse för Windows Server Data Center | 
| WindowsServerStandard_HasOpenRenewal | Identifierar om kunden har en öppen förnyelse för Windows Server standard | 
| AzureUpsellCustomer | Identifierar om kunden visar merförsäljning-benägenhet för Azure | 
| Har Google | Identifierar om kunden visar konkurrerande signaler för att äga Google-produkter | 
| Har AWS | Identifierar om kunden visar konkurrens bara signaler för ägande AWS-produkter | 
| Har EA | Identifierar om en förnyelse är en EA-eller EA-prenumeration | 
| Har öppen | Identifierar om en förnyelse är ett avtal med öppen eller öppen värde | 

### <a name="cloud-ascent---agreement-renewal-propensity-report"></a>**Cloud-stigning – avtals förnyelse benägenhet rapport**

| Kolumnnamn | Data Beskrivning | 
| :--------- | :--------- | 
| MPN-ID | Microsoft Partner Network-ID | 
| Partner namn | Partnerns namn | 
| Kund-ID | Kund-ID-nummer | 
| DUNS-nummer | Dun & Bradstreet-numret för kunden som poängs ätter för benägenhet | 
| Kontonamn | Namn på kontot | 
| Domain | Kontots domän | 
| Organisations storlek | Organisationens storlek | 
| Industri | Industri | 
| Lodrät | Den lodräta för kunden som poängs ätter för benägenhet, som identifieras av Microsoft, D&B och andra bransch standarder | 
| Område | Geografiskt område på platsen | 
| Dotterbolag | Dotter bolag till kunden som har Poäng för benägenhet | 
| Säljområde | Försäljnings området för kunden som poängs ätter för benägenhet | 
| City | Geografisk ort plats | 
| Stat | Geografisk tillstånds plats | 
| Postnummer | Post nummer för organisationen | 
| Land | Plats för geografiskt land | 
| Segment | Marknads segment | 
| Del segment | Marknads del segment | 
| Översikt över SMC-typ | SMC-typ | 
| Topp ohanterad – beräknings bas | Främsta ohanterade kunder – beräkning | 
| Topp ohanterad-användar bas | Vanligaste ohanterade kunder – användare | 
| IsNonProfit | Anger om organisationen är ideell (Ja eller Nej) | 
| Har Google | Identifierar om kunden visar konkurrens bara signaler för ägande AWS-produkter | 
| Har AWS | Identifierar om kunden visar konkurrens bara signaler för ägande AWS-produkter | 
| Azure-kluster | Identifierar kundens benägenhet för att köpa Azure. Mål Act nu och utvärderar kluster, eftersom de kommer att producera högre avkastning. Rikta in dig på Nurture och utbilda kunder enbart om det fortfarande finns kapacitet efter att du har riktat in dig på att utvärdera kunderna. | 
| D365 finans + drift kluster | Identifierar kundens benägenhet för att köpa Dynamics 365-ekonomi och-åtgärder. Kunder som visar en benägenhet för finans + Operations visas i de översta ohanterade kategorierna. Mål Act nu och utvärderar kluster, eftersom de kommer att producera högre avkastning. Rikta in dig på Nurture och utbilda kunder enbart om det fortfarande finns kapacitet efter att du har riktat in dig på att utvärdera kunderna. | 
| D365 CE-kluster | Identifierar kundens benägenhet för att köpa Dynamics 365 kund engagemang. Kunder som visar en benägenhet för kund engagemang kommer att ingå i kategorierna medel och liten. Mål Act nu och utvärderar kluster, eftersom de kommer att producera högre avkastning. Rikta in dig på Nurture och utbilda kunder enbart om det fortfarande finns kapacitet efter att du har riktat in dig på att utvärdera kunderna. | 
| D365 BC-kluster | Identifierar kundens benägenhet för att köpa Dynamics 365 Business Central. Kunder som visar en benägenhet for Business Central kommer att ingå i kategorierna medel och liten. Mål Act nu och utvärderar kluster, eftersom de kommer att producera högre avkastning. Rikta in dig på Nurture och utbilda kunder enbart om det fortfarande finns kapacitet efter att du har riktat in dig på att utvärdera kunderna. | 
| Microsoft 365 kluster | Identifierar kundens benägenhet för inköp Microsoft 365. Mål Act nu och utvärderar kluster, eftersom de kommer att producera högre avkastning. Rikta in dig på Nurture och utbilda kunder enbart om det fortfarande finns kapacitet efter att du har riktat in dig på att utvärdera kunderna. | 
| Licens program | Identifierar licens programmets typ för förnyelsen | 
| Avtals-ID | Identifierare för avtalet | 
| Datum för avtals slutdatum | Avtalets slutdatum | 
| Förfallo typ | Typ av förfallo datum | 
| Förfallo datum för intäkter | Intäkter som associeras med prenumerationer som upphör att gälla | 
| Har EA | Identifierar om en förnyelse är en EA-eller EA-prenumeration | 
| Har öppen | Identifierar om en förnyelse är ett avtal med öppen eller öppen värde | 
| Azure merförsäljning-kund | Identifierar om kunden visar merförsäljning-benägenhet för Azure | 
| Microsoft 365 merförsäljning-kund | Identifierar om kunden visar merförsäljning-benägenhet för Microsoft 365 | 
| RevSumDivisionName | Identifierar produkten som ska förnyas | 

## <a name="next-steps"></a>Nästa steg

Mer information finns i [Hämta rapporter](pci-download-reports.md).
