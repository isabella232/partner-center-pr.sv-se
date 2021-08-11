---
title: Datadefinitioner för insikter
ms.topic: article
ms.date: 12/14/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-insights
description: Dokumentet innehåller olika rapporter och deras datadefinitioner, som du kan ladda ned från Insights Ladda ned rapportsidan.
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: d210e067790980d377812f1200b20e470f2f52b51ccd3dcb1bab4d04a49b76b4
ms.sourcegitcommit: 121f1b9cbd88faeba60dc9b475f9c0647cdc933c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/06/2021
ms.locfileid: "115694905"
---
# <a name="export--data-definitions"></a>Export – Datadefinitioner 

**Lämpliga roller:** Rapportvisningsprogram | Rapportvisningsprogram för chefer

## <a name="introduction"></a>Introduktion 

Genom att använda hubben Ladda ned rapporter Insights instrumentpanelen kan du exportera rådatauppsättningarna. 

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
| PGAMpnId| Identifierare för MPN för partnerns globala konto|
| CustomerName| Kundens namn|
| CustomerTenantId| Identifierare för kundens klientorganisation|
| CustomerTpid| Identifierare för kundens överordnade överordnade|
| DUNSNumber|   Global Data Universal Number System Identifier för kund|
| CustomerSegment | Kundsegment|
| TopSegment    | Segmentklassificering på högre nivå för kunden|
| CustomerMarket|   Kundens geografiska marknad|  
| CustomerStatus    | Kundstatus (aktiv eller inaktiv)| 
| CustomerTenantName|   Namnet på kundens klientorganisation|
| CustomerTenantCountry|    Land för kundklientorganisation|
| TenantDomainName| Domännamn för kundklientorganisation|
| Produkt|  Produkten såldes till kunden via MPN: O365, Dynamics 365, Enterprise Mobility + Security, Power BI eller Microsoft Azure.|
| RawProductName|   Detaljerat produktnamn som sålts till kunden|
| SKU|  Produkt-SKU|
| Månad|    Månad då användning och intäkter rapporteras|
| MPNId|    Identifierare för Microsoft Partner Network (MPN)|
| PartnerName|  Partnerns namn|
| PartnerLocation|  Partnerns geografiska plats|
| PartnerAttributionType|   Attributionstyp för partnern| 
| SalesChannel| Försäljningskanal|
| IsDuplicateRowForPGA| För flera partnerattributions under samma PGA anges det här värdet till 0 för endast ett MPNId. Om värdet är inställt på 1 indikerar det en dubblettrad|
| AvailableSeats|   Tillgängliga platser|
| BilledRevenueUSD| Fakturerade intäkter i amerikanska dollar|
| AzureConsumedRevenueUSD|  Azure-intäktsförbrukning i USD|

### <a name="reseller-performance-report"></a>**Prestandarapport för återförsäljare**

> [!Note]
> Data om intäkter och Azure-förbrukade intäkter (ACR) är endast tillgängliga för användare som är rapportanvändare.

| Kolumnnamn | Databeskrivning | 
| :--------- | :--------- | 
| PGAMpnId | Identifierare för MPN för partnerns globala konto |
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
|PGAMpnId| Identifierare för MPN för partnerns globala konto |
|SubscriptionId | GUID för prenumerationen|
|SubscriptionStartDate | Startdatum för prenumerationen|
|SubscriptionEndDate | Slutdatum för prenumerationen|
|SubscriptionState | Status för prenumerationen (aktiv eller omsättning)|
|Månad | Månad då användning och intäkter rapporteras|
|IsAutoRenew | Anger om prenumerationen förnyas automatiskt (Ja eller Nej)|
|CustomerName | Kundens namn|
|CustomerTenantId | GUID för kunden|
|CustomerTpid | Kundens främsta överordnade identifierare|
|DUNSNumber| Global Data Universal Number System Identifier för kund|
|CustomerSegment | Kundens marknadssegment|
|TopSegment| Segmentklassificering på högre nivå för kund|
|CustomerMarket | Kundens geografiska marknad|
|ReportingProductName| Detaljerad produktnamn|
|Produkt | Produkt som säljs till kunden av partnern|
|RawProductName| Detaljerat produktnamn som sålts till kunden|
|ProductPartNumber| Produktens delnummer|
|SKU | Produktens SKU|
|RevSumDivisionName| Namn på produkthierarki för intäktsrapportering|
|SolutionArea| Produktens klassificering av affärsprogram|
|MPNId | Microsoft Partner Network id för partnern|
|PartnerName | Partnerns namn|
|PartnerLocation | Partnerns geografiska plats|
|PartnerAttributionType | Attributionstyp för prenumerationen|
|SalesChannel | Kanal för försäljning – Direkt, CSP (Molnlösningsleverantör) och så vidare|
|PricingLevel| Försäljningsprispunkt|
|EnrollmentNumber| Prenumerationens registreringsnummer|
|IsDuplicateRowForPGA| För flera partnerattributions under samma PGA anges det här värdet till 0 för endast ett MPNId. Om värdet är inställt på 1 indikerar det en dubblettrad|
|SubscriptionStartMonth| Startmånad för prenumerationen|
|ResellerID| Id för återförsäljare|
|ResellerName| Återförsäljarens namn|
|AvailableSeatsEOP| Totalt antal tillgängliga platser fram till slutet av perioden|
|AvailableSeats | Tillgänglig platsskillnad månad för månad|
|BilledRevenueUSD | Intäkter i USD|
|AzureConsumedRevenueUSD| Azure-intäktsförbrukning i USD|

### <a name="azure-usage-report"></a>**Användningsrapport för Azure**

| Kolumnnamn | Databeskrivning | 
| :--------- | :--------- | 
|PGAMpnId| Identifierare för MPN för partnerns globala konto|
|SubscriptionId| GUID för prenumerationen|
|SubscriptionStartDate| Datumet för prenumerationens start|
|SubscriptionEndDate| Datumet för prenumerationens slut|
|FirstUseDate| Datum då Azure-tjänster användes först|
|SubscriptionState| Aktuellt tillstånd för prenumerationen (öppen, stängd aktiv eller respitperiod)|
|Månad| Datum aggregerat efter månad|
|ServiceLevel1| Servicenivå 1 – Motsvarar tjänstpelaren, till exempel containrar, databaser, nätverk osv.|
|ServiceLevel2| Servicenivå 2 – Motsvarar arbetsbelastningen för tjänstpelaren|
|ServiceLevel3| Tjänstnamn som används av Azure.Microsoft.Com när Azure-erbjudanden listas|
|ServiceLevel4| Logiska gruppningar av högnivåfunktionsuppsättnings differentieringar i tjänsten. Till exempel Generell användning Virtual Machines, minnesoptimerad Virtual Machines, enkel SQL Database, Elastic SQL Database osv. |
|ServiceGroup2| FIELD Revenue Accountability (FRA) områden som AI, App Dev, IoT osv. |
|ServiceGroup3| Ytterligare information för SKA, till exempel IoT Hub, Kartor för IoTLTE|
|ServiceInfluencer| PaaS-tjänster som driver förbrukning av infrastrukturresurser, till exempel Service Fabric, Azure Databricks, AKS osv.|
|ComputeOS| Beräkningsoperativsystemet|
|ComputeCoreSoftware| Compute Core Software|
|UsageUnits| Antalet enheter som används under faktureringsperioden|
|UsageQuantity| Kvantitet för resursanvändning|
|CustomerName| Kundens namn|
|CustomerTenantId| Klientorganisations-ID för kund|
|CustomerTpid| Kundens överordnade ID|
|CustomerSegment| Kundens segment|
|CustomerMarket| Kundens geografiska marknad|
|MPNId| Microsoft Partner Network id för kunden|
|PartnerName| Partnerns namn|
|PartnerLocation| Partnerns geografiska land|
|PartnerAttributionType| Attributionstyp för partnern|
|SalesChannel| Kanal för försäljningen (Direct/CSP, Indirect/CSP, Direct och så vidare)  |
|EnrollmentNumber| Prenumerationens registreringsnummer |
|IsACRDuplicateAtPGALevel| För flera partnerattributions under samma PGA anges det här värdet till 0 för endast ett MPNId. Om värdet är inställt på 1 indikerar det en dubblettrad|
|ResellerID| Id för återförsäljare|
|ResellerName| Återförsäljarens namn|
|AdminType| När partnerattributionstyp är "Partneradministratörslänk (PAL)" Anger den här kolumnen den tilldelade rollen i kundens prenumeration.|
|AssociationType| Typ av association|
|MonthlySubscriptionLevelACR| ACR på månadsnivå|
|ACR_USD| Azure-förbrukade intäkter (ACR) i amerikanska dollar|

### <a name="office-365-license-usage-report"></a>**Office 365 licensanvändningsrapport**

| Kolumnnamn | Databeskrivning | 
| :--------- | :--------- | 
| PGAMpnId | Identifierare för MPN för partnerns globala konto | 
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
| IsDuplicateRowForPGA | För flera partnerattributions under en enda PGA anges det här värdet till 0 för endast ett MPNId. Om värdet är inställt på 1 indikerar det en dubblettrad|

### <a name="enterprise-mobility-license-usage-report"></a>**Användningsrapport för Enterprise Mobility-licenser**

| Kolumnnamn | Databeskrivning | 
| :--------- | :--------- | 
| PGAMpnId| Identifierare för partnerns globala konto MPN| 
| SubscriptionId | GUID för prenumerationen| 
| SubscriptionStartDate | Datumet för prenumerationens start| 
| SubscriptionEndDate | Det datum då prenumerationen upphör| 
| SubscriptionStatus| Aktuellt tillstånd för prenumerationen (Öppen, Stängd, Aktiv eller Respitperiod)| 
| Månad | Datum aggregerat efter månad| 
| SKU| Produkt-SKU| 
| SKUId| SKU-ID för produkten| 
| FreeVsAvsKU| Anger kostnadsfri eller betald SKU| 
| SalesModel| Försäljningskanal som används för att sälja prenumerationen| 
| DetailedSalesModel| Detaljerad försäljningsmodell för prenumerationen| 
| CustomerName| Kundens namn| 
| CustomerTenantId | Klientorganisations-ID för kund| 
| CustomerTpid | Kundens överordnade ID| 
| CustomerSegment | Kundsegment| 
| CustomerMarket | Geografiskt land på kundens marknad| 
| MPNId | Microsoft Partner Network-ID| 
| PartnerName | Namnet på partnern| 
| PartnerLocation | Partnerns geografiska plats| 
| PartnerAttributionType | Attributionstyp för partner| 
| PartnerHierarki| Hierarki med partner (virtuell organisation, huvudkontor eller plats)| 
| PaidAvailableUnits | Antal betalda tillgängliga enheter| 
| MonthlyActiveUsers | Antal månatliga aktiva användare| 
| AATPActiveUsage| Aktiv användning av Azure Advanced Threat Protection (AATP)| 
| MCASActiveUsage| AKTIV MCAS-användning| 
| AADPAvailableUnits| Antal betalda tillgängliga enheter för Azure Active Directory Premium (AADP)| 
| IntuneAvailableUnits| Antal betalda tillgängliga enheter för Intune| 
| AzipAvailableUnits| Antal betalda tillgängliga enheter för Azip| 
| AADPMonthlyActiveUsers| Antal månatliga aktiva användare för Azure Active Directory Premium (AADP)| 
| IntuneMonthlyActiveUsers| Antal månatliga aktiva användare för Intune| 
| AzipMonthlyActiveUsers| Antal månatliga aktiva användare för Azip| 
| MDM| MDM| 
| MAM| MAM| 
| SSPR| SSPR| 

### <a name="dynamics-365-license-usage-report"></a>**Licensanvändningsrapport för Dynamics 365**

| Kolumnnamn | Databeskrivning | 
| :--------- | :--------- | 
| PGAMpnId | Identifierare för partnerns globala konto MPN | 
| SubscriptionId | GUID för prenumerationen | 
| SubscriptionStartDate | Startdatum för prenumerationen | 
| SubscriptionEndDate | Slutdatum för prenumerationen | 
| SubscriptionStatus | Status för prenumerationen | 
| Månad | Månad då användning rapporteras | 
| RevSumDivisionName | Namn på divisionen för rev-summa | 
| RevSumCategoryName | Namnet på kategorin för rev-summa | 
| SKU | Produktens SKU | 
| SKUId | SKU-ID för produkten | 
| FreeVsAvsKU | Anger om det är en kostnadsfri eller betald SKU | 
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
| AvailableSeats |  Aktuella betalda tillgängliga platser|
| AssignedSeats |   Aktuella tilldelade platser|
| ActiveSeats | Aktuella aktiva platser|
| DistributionOpportunity |   Distributionsmöjlighet är antalet platser som inte har tilldelats|
| ActiveUsagePercent |  Aktuell aktiv användning i procent av tillgängliga platser |

### <a name="power-bi-license-usage-report"></a>**Power BI licensanvändningsrapport**

| Kolumnnamn | Databeskrivning | 
| :--------- | :--------- | 
| PGAMpnId | Identifierare för MPN för partnerns globala konto | 
| SubscriptionId | GUID för prenumerationen | 
| SubscriptionStartDate | Startdatum för prenumerationen | 
| SubscriptionEndDate | Slutdatum för prenumerationen | 
| SubscriptionStatus | Status för prenumerationen (aktiv, inaktiv eller respitperiod) | 
| Månad | Datum aggregerat efter månad | 
| SKU | Produktens SKU | 
| SKUId | SKU-ID för produkten | 
| FreeVs IASKU | Kostnadsfri eller betald SKU-differentiator | 
| SalesModel | Försäljningsmodell som används för att sälja prenumerationen | 
| DetailedSalesModel | Detaljerad försäljningsmodell för prenumerationen | 
| CustomerName | Kundens namn | 
| CustomerTenantId | GUID för kundens klientorganisation | 
| CustomerTpid | Identifierare för kundens överordnade överordnade | 
| CustomerSegment | Kundens marknadssegment | 
| CustomerMarket | Kundens geografiska marknad | 
| MPNId | Identifierare för Microsoft Partner Network | 
| PartnerName | Partnerns namn | 
| PartnerLocation | Partnerns geografiska land | 
| PartnerAttachType | Attributionstyp för prenumerationen | 
| PartnerHierarki |    Hierarki för partner (virtuell organisation, huvudkontor eller plats)|
| AvailableSeats |  Aktuella betalda tillgängliga platser|
| AssignedSeats |   Aktuella tilldelade platser|
| ActiveSeats | Aktuella aktiva platser|
| DistributionOpportunity |   Distributionsmöjlighet är antalet platser som inte har tilldelats|
| ActiveUsagePercent |  Aktuell aktiv användning i procent av tillgängliga platser|

### <a name="teams-meetings-and-calls-report"></a>**Teams för möten och anrop**

| Kolumnnamn | Databeskrivning | 
| :--------- | :--------- | 
| PGAMpnId | Identifierare för MPN för partnerns globala konto | 
| CustomerTenantId | Kundens klientorganisations-ID | 
| CustomerId | Identifierare för kundens överordnade överordnade | 
| DateKey | Datum då användning rapporteras
| Underarbetslast | Underlast för vilken användning rapporteras (möten, samtal eller telefonsystem) | 
| Antal möten | Antal möten | 
| Varaktighet för möte | Total varaktighet för möte i timmar | 

### <a name="teams-monthly-usage-report"></a>**Teams månatlig användningsrapport**

| Kolumnnamn | Databeskrivning | 
| :--------- | :--------- | 
| PGAMpnId |    Identifierare för MPN för partnerns globala konto |
| CustomerTenantId |    Kundens klientorganisations-ID|
| CustomerId |  Identifierare för kundens överordnade överordnade|
| MonthKey |    Månad då användning rapporteras|
| Underbelastning | Underlast för vilken användning rapporteras (möten, samtal eller telefonsystem)|
| DesktopUsers |    Antal användare som använder Teams på skrivbordet|
| MobileUsers | Antal användare som använder Teams på mobila enheter|
| WebUsers |    Antal användare som använder Teams på webben|
| AllUpParticipants |   Antal unika användare av Teams för månaden|

### <a name="teams-usage-3p-apps-report"></a>**Teams 3P-appar för användning**

| Kolumnnamn | Databeskrivning | 
| :--------- | :--------- | 
| PGAMpnId  | Identifierare för MPN för partnerns globala konto |
| CustomerTenantId |    Kundens klientorganisations-ID |
| CustomerId |  Kundens överordnade ID |
| CustomerName |    Kundnamn |
| CustomerCountry | Kundland |
| DateKey | Datum då användning rapporteras |
| Appname | Namnet på Teams appen |
| Usercount |   Antal användare för appen |

### <a name="training-details-report"></a>**Rapport för träningsinformation**

| Kolumnnamn | Databeskrivning | 
| :--------- | :--------- | 
| PGAMpnId  | Identifierare för MPN för partnerns globala konto |
| TrainingActivityId | Identifierare för träningen | 
| TrainingTitle | Utbildningens titel | 
| TrainingType | Typ av utbildning (certifiering eller prov) | 
| IndividualFirstName | Kundens förnamn | 
| IndividualLastName | Kundens efternamn | 
| E-post | Kundens personliga e-post-ID | 
| CorpEmail | Office e-post-ID för kunden | 
| TrainingCompletionDate | Slutförandedatum för träningen | 
| ExpirationDate |  Certifieringens förfallodatum|
| ActivationStatus |    Status för certifieringen|
| Månad | Månad då data rapporteras | 
| IcMCP | Anger om användaren är Microsoft Certified Professional (MCP) | 
| MCPID | MCP-ID för användaren | 
| MPNId | Identifierare för Microsoft Partner Network | 
| PartnerName | Partnerns namn | 
| PartnerCityLocation | Partnerns geografiska plats | 
| PartnerCountryLocation | Partnerns geografiska land | 

### <a name="microsoft-learn-report"></a>**Microsoft Learn rapport**

| Kolumnnamn | Databeskrivning | 
| :--------- | :--------- | 
| PGAMpnId  | Identifierare för MPN för partnerns globala konto |
| Användarnamn | Användarens namn | 
| UserId | GUID för användaren | 
| TrainingName | Namnet på träningen | 
| TrainingType | Typ av utbildning (modul eller utbildningsväg) | 
| Produkter | Produkt som utbildningsmodulen gäller för | 
| Roller | Tillämpliga roller för träningen | 
| CompletionDate | Datum för slutförande av träningen | 
| MPNId | Identifierare för Microsoft Partner Network | 
| PartnerName | Partnerns namn | 
| Land | Partnerns geografiska land | 

### <a name="competency-summary-and-history-report"></a>**Sammanfattning av kompetens och historikrapport**

| Kolumnnamn | Databeskrivning | 
| :--------- | :--------- | 
| CompetencyName | Namn på kompetensen | 
| CompetencyLevel | Kompetensnivå (guld eller silver) | 
| CompetencyStatus | Aktuell status för kompetensen (aktiv, inaktiv eller respitperiod) | 
| CompetencyStartDate | Kompetensens startdatum | 
| CompetencyEndDate | Kompetensens slutdatum | 

### <a name="competency-performance-report"></a>**Prestandarapport för kompetens**

| Kolumnnamn | Databeskrivning | 
| :--------- | :--------- | 
| CompetencyName | Namn på kompetensen | 
| CompetencyAttainmentOptionName | Namn på kompetensalternativ | 
| Månad | Månad då måtten rapporteras | 
| MetricName | Namnet på det mått som är relevant för kompetensen | 
| MetricMonthlyContribution | Månatligt bidrag för måttet | 
| TTMAggregate | Aggregerat mått för de avslutande 12 månaderna | 
| AnniversaryYearAggregate | Aggregerat mått för det aktuella årsdagen | 
| GoldThreshold | Prestandakrav för att uppfylla guldkompetens | 
| SilverThreshold | Prestandakrav för att uppfylla Silver-kompetens | 

### <a name="cloud-ascent---microsoft-365-propensity-report"></a>**Cloud Ascent – Microsoft 365 rapport om benägenhet**

| Kolumnnamn | Databeskrivning | 
| :--------- | :--------- | 
| MPN-ID | Microsoft Partner Network-ID | 
| Partnernamn | Partnerns namn | 
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
| Aktivera fjärrarbete – Exchange Online | Kunder som har en aktiv Exchange Online-prenumeration, uppförsäljning till Microsoft 365 | 
| Aktivera fjärrarbete – lokalt förvärv (aktuell version) med Cloud Ascent-benägenhet – +10 licenser | Kund som har en aktuell lokal Office eller Windows klient. Klientversionen är alltså senare än en EOL-version (End of Life). Kunden har 10 eller fler licenser. Kund som har en benägenhetspoäng. Partnern bör rikta in sig på konvertering till Microsoft 365. | 
| Aktivera fjärrarbete – lokalt förvärv (aktuell version) med Cloud Ascent-benägenhet – <10 licenser | Kund som har en aktuell lokal Office eller Windows klient (det vill säga en senare version än EOL). Kunden har färre än 10 licenser. Kund som har en benägenhetspoäng. Partnern bör rikta in sig på konvertering till Microsoft 365. | 
| Aktivera fjärrarbete – lokalt förvärv (aktuell version) utan Cloud Ascent-benägenhet – +10 licenser | Kund som har en aktuell lokal Office eller Windows klient (det vill säga en senare version än EOL). Kunden har 10 eller fler licenser. Kunden har ingen benägenhetspoäng. Partnern bör rikta in sig på konvertering till Microsoft 365. | 
| Aktivera fjärrarbete – lokalt förvärv (aktuell version) utan Cloud Ascent-benägenhet – <10 licenser | Kund som har en aktuell lokal Office eller Windows klient (det vill säga en senare version än EOL). Kunden har färre än 10 licenser. Kunden har ingen benägenhetspoäng. Partnern bör rikta in sig på konvertering till Microsoft 365. | 
| Aktivera fjärrarbete – lokalt förvärv (EOL-version) med Cloud Ascent-benägenhet – +10 licenser | Kund som har en lokal EOL-Office eller Windows (det vill säga en EOL-version eller tidigare). Kunden har 10 eller fler licenser. Kunden har en benägenhetspoäng. Partnern bör rikta in sig på konvertering till Microsoft 365. | 
| Aktivera fjärrarbete – lokalt förvärv (EOL-version) med Cloud Ascent-benägenhet – <10 licenser | Kund som har en lokal EOL-Office eller Windows (det vill säga en EOL-version eller tidigare). Kunden har färre än 10 licenser. Kunden har en benägenhetspoäng. Partnern bör rikta in sig på konvertering till Microsoft 365. | 
| Aktivera fjärrarbete – lokalt förvärv (EOL-version) utan Cloud Ascent-benägenhet – +10 licenser | Kund som har en aktuell lokal Office eller Windows klient (det vill säga en EOL-version eller tidigare). Kunden har 10 eller fler licenser. Kunden har ingen benägenhetspoäng. Partnern bör rikta in sig på konvertering till Microsoft 365. | 
| Aktivera fjärrarbete – lokalt förvärv (EOL-version) utan Cloud Ascent-benägenhet – <10 licenser | Kund som har en aktuell lokal Office eller Windows klient (det vill säga en EOL-version eller tidigare). Kunden har färre än 10 licenser. Kunden har ingen benägenhetspoäng. Partnern bör rikta in sig på konvertering till Microsoft 365. | 
| Enable Remote Work – potentiell potentiell benägenhet för Microsoft 365 (Act NowithEvaluate) | Potentiell kund med hög benägenhet för Microsoft 365 | 
| Aktivera fjärrarbete – konkurrera (Zoom) med Microsoft 365 | Kund med Zoom och Microsoft 365, mål för konvertering till Teams | 
| Aktivera fjärrarbete – konkurrera (Zooma) utan Microsoft 365 | Kund med Zoom, mål för konvertering till Teams | 
| Minska kostnader och hantera – Microsoft 365 E3 mål för Microsoft 365 E5 | Befintlig kund med Microsoft 365 E3, mål för Microsoft 365 E5 | 
| Minska kostnader och hantera – Microsoft 365 Business Basic och Business Standard-kunder som är mål för Microsoft 365 Business Premium | Befintliga Microsoft 365 Business Basic och Business Standard-kunder, mål för Microsoft 365 Business Premium | 
| Transformera organisationsproduktivitet – surface-benägenhet | Kunden visar en benägenhet för Surface | 
| M365Cluster | Identifierar en kunds benägenhet att köpa Microsoft 365. Target Act Now och Evaluate clusters eftersom de ger högre avkastning. Rikta in sig på att utveckla och utbilda kunder endast om det fortfarande finns kapacitet efter att kunderna Act Now (Agera nu) och Evaluate (Utvärdera) har mål. | 
| M365Fit | Interna och externa datapunkter som definierar företagsgrafiska data. Fit scoring använder en lookalike-modell för våra bästa små eller medelstora företag (SBS) för att jämföra kunder och se om de är lämpliga för Microsofts molnprodukter. Bedömning av passning uppdateras kvartalsvis. | 
| M365Intent | Signaler som rör sociala medier och en kunds onlinebeteende definierar Intent. Avsiktsbedömningen överlagras i Anpassa för att definiera klustren. Avsiktsbedömningen uppdateras varje månad. | 
| SurfaceCluster | Identifierar en kunds återgivning av Surface genom att konsolidera rekommendationerna fit and intent i ett kluster. Target Act Now och Evaluate clusters eftersom de ger högre avkastning. Rikta in sig på att utveckla och utbilda kunder endast om det fortfarande finns kapacitet efter att kunderna Act Now (Agera nu) och Evaluate (Utvärdera) har mål. | 
| SurfaceFit | Interna och externa datapunkter som definierar företagsgrafiska data. Fit scoring använder en lookalike-modell till våra bästa SMI:er för att jämföra kunder och se om de är lämpliga för Microsofts molnprodukter. Bedömning av passning uppdateras kvartalsvis. | 
| SurfaceIntent | Signaler som rör sociala medier och en kunds onlinebeteende definierar Intent. Avsiktsbedömningen överlagras i Anpassa för att definiera klustren. Avsiktsbedömningen uppdateras varje månad. | 
| O365Cluster | Identifierar kundens benägenhet att köpa Office 365. Target Act Now och Evaluate clusters eftersom de ger högre avkastning. Rikta in sig på att utveckla och utbilda kunder endast om det fortfarande finns kapacitet efter att kunderna Act Now (Agera nu) och Evaluate (Utvärdera) har mål. | 
| O365Fit | Interna och externa datapunkter som definierar företagsgrafiska data. Fit scoring använder en lookalike-modell till våra bästa SMI:er för att jämföra kunder och se om de är lämpliga för Microsofts molnprodukter. Bedömning av passning uppdateras kvartalsvis. | 
| O365Intent | Signaler som rör sociala medier och en kunds onlinebeteende definierar Intent. Avsiktsbedömningen överlagras i Anpassa för att definiera klustren. Avsiktsbedömningen uppdateras varje månad. | 
| M365UpsellCustomer | Identifierar om kunden visar uppförsäljningsfördröjning för Microsoft 365 | 
| Har Google | Identifierar om kunden visar konkurrenssignaler för att äga Google-produkter | 
| Har AWS | Identifierar om kunden visar konkurrenssignaler för att äga Amazon Web Services (AWS)-produkter | 
| Har EA | Anger om en förnyelse är ett Enterprise-avtal (EA) eller en EA-prenumeration | 
| Har öppen | Anger om en förnyelse är ett Open- eller Open Value-avtal | 

### <a name="cloud-ascent---dynamics-365-propensity-report"></a>**Cloud Ascent – gångarrapport för Dynamics 365**

| Kolumnnamn | Databeskrivning | 
| :--------- | :--------- | 
| MPN-ID | Microsoft Partner Network (MPN) ID | 
| Partnernamn | Partnerns namn | 
| Kund-ID | Kundidentifierarnummer | 
| DUNS-nummer | Dun & Bradstreet-numret för den kund som poängsätts för berättigande | 
| Account Name | Namn på kontot | 
| Domain | Domänen för kontot | 
| Organisationsstorlek | Organisationens storlek | 
| Industri | Bransch som organisationen tillhör | 
| Lodrät | Vertikalen hos den kund som poängas för benägenhet enligt Microsoft, D&B och andra branschstandarder
| Område | Geografiskt område för platsen | 
| Dotterbolag | Dotterbolaget till den kund som poängas för benägenhet | 
| Säljområde | Försäljningsområde för den kund som poängsattes för benägenhet | 
| City | Geografisk ort | 
| Tillstånd | Geografisk plats | 
| Postnummer | Organisationens postnummer | 
| Land | Geografiskt land | 
| Segment | Marknadssegment | 
| Undersegment | Undersegment för marknad | 
| Sammanfattning av SMC-typ | Kategorisering av en kund: De främsta ohanterade användarbaserna är kunder med över 300 anställda, de främsta ohanterade beräkningsbaserna är kunder med tre års potential i Azure med 10 000 USD, medelstora företag är kunder med 25 anställda eller större och små företag är kunder med färre än 25 anställda. | 
| Översta ohanterade – beräkningsbas | De främsta ohanterade kunderna – beräkning | 
| Översta ohanterade – användarbas | De mest ohanterade kunderna – användare | 
| IsNonProfit | Anger om organisationen är ideell (Ja eller Nej) | 
| Activate Digital Selling - Microsoft 365 - seat size >= 25 seats (SalesPro propensity model) | Kund utan Dynamics 365. Platsstorlek: 25+. Partnern bör rikta sig mot korsförsäljning av Dynamics 365 SalesPro. | 
| Aktivera digital försäljning – Dynamics 365 SalesPro-benägenhet (agera nu eller utvärdera) | Kunder med hög benägenhet utan Dynamics 365. Partnern bör vara mål för Dynamics 365 SalesPro. | 
| Hantera finansiella risker & bedrägeri – Lokal Dynamics-installationsbas – Navision (Business Central-fundamentsmodell) | Befintlig kund med lokal Navision. Partnern bör vara mål för Dynamics 365 Business Central. | 
| Hantera finansiella risker & bedrägeri – Dynamics on-premises-installationsbas – Dynamics AX (Dynamics 365 Finance + Operations propensity model) | Befintlig kund med lokal AX. Partnern bör vara mål för Dynamics 365 Finance + Operations. | 
| Hantera finansiella risker & bedrägeri – Lokal Dynamics-installationsbas – Great Plains (Business Central-benägenhetsmodell) | Befintlig kund med lokala Great Plains. Partnern bör vara mål för Dynamics 365 Business Central. | 
| Hantera finansiella risker & bedrägeri – Dynamics on-premises install base – Dynamics (Business Central-benägenhetsmodell) | Befintlig kund med lokal snöjdhet. Partnern bör vara mål för Dynamics 365 Business Central. | 
| Hantera finansiella risker & bedrägeri – Lokal Dynamics-installationsbas – andra (Business Central-fundamentsmodellen) | Befintlig kund med andra lokala lösningar som inte tidigare listats. Partnern bör vara mål för Dynamics 365 Business Central. | 
| Skapa agila affärsprocesser – Lokal Dynamics-installation – AX/GP/SL/NAV/Other (365-benägenhetsmodell för Dynamics) | Skapa agila affärsprocesser – Lokal Dynamics-installation – AX/GP/SL/NAV/Other (365-benägenhetsmodell för Dynamics) | 
| Skapa agila affärsprocesser – Dynamics konkurrerar bas – Mendix/OutSystems/Salesforce (benägenhetsmodell för Dynamics 365) | Skapa agila affärsprocesser – Dynamics konkurrerar bas – Mendix/OutSystems/Salesforce (Dynamics 365-benägenhetsmodell) | 
| Skapa agila affärsprocesser – Installationsbas för Dynamics 365 Finance + Operations | Befintliga Dynamics 365 Finance + Operations-kunder. Partner till Power Apps. | 
| Skapa agila affärsprocesser – Installationsbas för Dynamics 365 Business Central | Befintliga Dynamics 365 Business Central-kunder. Partner till Power Apps. | 
| Skapa agila affärsprocesser – Installationsbas för Dynamics 365 för kundengagemang | Befintliga Dynamics 365 Customer Engagement-kunder. Partner till Power Apps. | 
| Skapa en motståndskraftig leveranskedja – Windows och aktivera första Dynamics 365-arbetsbelastning som Dynamics 365 Supply Chain Management med icke-Oracle- eller SAP ERP-kunder (resursplanering för företag) | Rikta in sig på kunder för Dynamics 365 Supply Chain Management | 
| Skapa en motståndskraftig leveranskedja – korsförsäljning av Dynamics 365 Supply Chain Management och/eller detaljhandel eller handel till befintliga Dynamics 365 Customer Engagement-kunder | Befintliga Dynamics 365 Customer Engagement-kunder som mål för crossförsäljning av Dynamics 365 Supply Chain Management. | 
| Skapa en motståndskraftig leveranskedja – korsförsäljning av Dynamics 365 Supply Chain Management och/eller detaljhandel eller handel till Dynamics 365 Customer Engagement och Oracle eller SAP | Befintliga Dynamics 365 Customer Engagement-kunder med Oracle eller SAP som mål för Dynamics 365 Supply Chain Management | 
| D365BCCluster | Identifierar kundens benägenhet att köpa Dynamics 365 Business Central. Kunder som visar en benägenhet för Business Central finns i kategorierna Medel och Liten. Target Act Now och Evaluate clusters, eftersom de ger högre avkastning. Rikta in dig på att utveckla och utbilda kunder endast om det fortfarande finns kapacitet efter att du riktar in dig på Agera nu och Utvärdera kunder. | 
| D365BCFit | Interna och externa datapunkter som definierar företagsgrafiska data. Fit scoring använder en lookalike-modell till vår bästa SMB för att jämföra kunder och se om de är lämpliga för Microsofts molnprodukter. Bedömning av passning uppdateras kvartalsvis. | 
| D365BCIntent | Signaler som rör sociala medier och en kunds onlinebeteende definierar Intent. Avsiktsbedömningen överlagras i Anpassa för att definiera klustren. Avsiktsbedömningen uppdateras varje månad. | 
| D365FOCluster | Identifierar kundens önskemål om att köpa Dynamics 365 Finance and Operations. Kunder som visar en benägenhet för Finance + Operations finns i de översta ohanterade kategorierna. Target Act Now och Evaluate clusters, eftersom de ger högre avkastning. Rikta in dig på att utveckla och utbilda kunder endast om det fortfarande finns kapacitet efter att du riktar in dig på Agera nu och Utvärdera kunder. | 
| D365FOFit | Interna och externa datapunkter som definierar företagsgrafiska data. Fit scoring använder en lookalike-modell till vår bästa SMB för att jämföra kunder och se om de är lämpliga för Microsofts molnprodukter. Bedömning av passning uppdateras kvartalsvis. | 
| D365FOIntent | Signaler som rör sociala medier och en kunds onlinebeteende definierar Avsikt. Avsiktsbedömningen överlagras i Anpassa för att definiera klustren. Avsiktsbedömningen uppdateras varje månad. | 
| D365CECluster | Identifierar kundens ighet att köpa Dynamics 365 Customer Engagement. Kunder som har en öjlighet för Customer Engagement finns i kategorierna Medel och Liten. Target Act Now och Evaluate clusters, eftersom de ger högre avkastning. Rikta in dig på att utbilda kunder om det fortfarande finns kapacitet efter att du riktar in dig på Agera nu och Utvärdera kunder. | 
| D365CEFit | Anger Anpassa för Dynamics 365 Customer Engagement | 
| D365CEIntent | Anger avsikt för Dynamics 365 Customer Engagement | 
| DynamicsOnPremAXorCRM_HasOpenRenewal | Anger om kunden har en öppen förnyelse för Dynamics on-premises AX eller CRM | 
| M365UpsellCustomer | Anger om kunden visar huruvida säljförsäljningen är Microsoft 365 | 
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
| Främsta ohanterade – beräkningsbas | De mest ohanterade kunderna – beräkning | 
| Översta ohanterade – användarbas | De mest ohanterade kunderna – användare | 
| IsNonProfit | Anger om organisationen är ideell (Ja eller Nej) | 
| Migrate – EOL Windows Server – EOL Windows Server IB med Cloud Ascent-skapacitet – fler än 5 licenser | Kund som har en EOL lokalt Windows Server (det vill säga en EOL-version eller tidigare). Kunden har 5 eller fler licenser. Kund som har en poäng. Partnern bör rikta in sig på kunden för migrering till Azure. | 
| Migrera – EOL Windows Server – EOL Windows Server IB med Cloud Ascent-skapacitet – <5 licenser | Kund som har en EOL lokalt Windows Server (det vill säga en EOL-version eller tidigare). Kunden har färre än 5 licenser. Kund som har en poäng. Partnern bör rikta in sig på kunden för migrering till Azure. | 
| Migrera – EOL Windows Server – EOL Windows Server IB utan Cloud Ascent-ighet – över 5 licenser | Kund som har en EOL lokalt Windows Server (det vill säga en EOL-version eller tidigare). Kunden har fler än 5 licenser. Kunden har ingen poäng. Partnern bör rikta in sig på kunden för migrering till Azure. | 
| Migrate - EOL Windows Server - EOL Windows Server IB without Cloud Ascent propensity - <5 licenses | Kund som har en EOL lokalt Windows Server (det vill säga en EOL-version eller tidigare). Har färre än 5 licenser. Kunden har ingen poäng. Partnern bör rikta in sig på kunden för migrering till Azure. | 
| Migrera – EOL SQL – EOL SQL Server IB med Cloud Ascent-skapacitet – över 5 licenser | Kund som har en lokal EOL-SQL Server (det vill säga en EOL-version eller tidigare). Kunden har fler än 5 licenser. Kunden har en ighetspoäng. Partnern bör rikta in sig på kunden för migrering till Azure. | 
| Migrera – EOL SQL – EOL SQL Server IB med Cloud Ascent-skapacitet – <5 licenser | Kund som har en lokal EOL-SQL Server (det vill säga en EOL-version eller tidigare). Har färre än 5 licenser. Kund som har en poäng. Partnern bör rikta in sig på kunden för migrering till Azure. | 
| Migrera – EOL SQL – EOL SQL Server IB utan Cloud Ascent-skapacitet – över 5 licenser | Kund som har en lokal EOL-SQL Server (det vill säga en EOL-version eller tidigare). Kunden har 5 eller fler licenser. Kunden har ingen poäng. Partnern bör rikta in sig på kunden för migrering till Azure. | 
| Migrera – EOL SQL – EOL SQL Server IB utan Cloud Ascent-skapacitet – <5 licenser | Kund som har en lokal EOL-SQL Server (det vill säga en EOL-version eller tidigare). Kunden har färre än 5 licenser. Kunden har ingen poäng. Partnern bör rikta in sig på kunden för migrering till Azure. | 
| Migrera – Migrera lokal Windows Server – aktuell Windows Server IB med Cloud Ascent-skapacitet – över 5 licenser | Kund som har en aktuell lokal Windows Server (det vill säga en senare version än EOL). Kunden har fler än 5 licenser. Kunden har en ighetspoäng. Partnern bör rikta in sig på kunden för migrering till Azure. | 
| Migrera – Migrera lokal Windows Server – aktuell Windows Server IB med Cloud Ascent-skapacitet – <5 licenser | Kund som har en aktuell lokal Windows Server (det vill säga en senare version än EOL). Kunden har färre än 5 licenser. Kunden har en poäng för Azure. Partnern bör rikta in sig på kunden för migrering till Azure. | 
| Migrera – Migrera lokal Windows Server – aktuell Windows Server IB utan Cloud Ascent-gångar – fler än 5 licenser | Kund som har en aktuell lokal Windows Server (det vill säga en senare version än EOL). Kunden har fler än 5 licenser. Kunden har ingen poäng. Partnern bör rikta in sig på kunden för migrering till Azure. | 
| Migrera – Migrera lokal Windows Server – aktuell Windows Server IB utan Cloud Ascent-gångar – <5 licenser | Kund som har en aktuell lokal Windows Server (det vill säga en senare version än EOL). Kunden har färre än 5 licenser. Kunden har ingen poäng. Partnern bör rikta in sig på kunden för migrering till Azure. | 
| Migrera – Migrera till Azure SQL eller SQL virtuella datorer (VM) – aktuell SQL Server IB med Cloud Ascent-ighet – över 5 licenser | Kund som har en aktuell lokal SQL Server (det vill säga en senare version än EOL). Kunden har fler än 5 licenser. Kunden har en ighetspoäng. Partnern bör rikta in sig på kunden för migrering till Azure. | 
| Migrera – Migrera till Azure SQL eller SQL virtuella datorer – aktuell SQL Server IB med Cloud Ascent-ighet – <5 licenser | Kund som har en aktuell lokal SQL Server (det vill säga en senare version än EOL). Kunden har färre än 5 licenser. Kunden har en ighetspoäng. Partnern bör rikta in sig på kunden för migrering till Azure. | 
| Migrera – Migrera till Azure SQL eller SQL virtuella datorer – aktuell SQL Server IB utan Cloud Ascent-ighet – 5+ licenser | Kund som har en aktuell lokal SQL Server (det vill säga en senare version än EOL). Kunden har fler än 5 licenser. Kunden har ingen poäng. Partnern bör rikta in sig på kunden för migrering till Azure. | 
| Migrera – Migrera till Azure SQL eller SQL virtuella datorer – aktuell SQL Server IB utan Cloud Ascent-gångar – <5 licenser | Kund som har en aktuell lokal SQL Server (det vill säga en senare version än EOL). Kunden har färre än 5 licenser. Kunden har ingen poäng. Partnern bör rikta in sig på kunden för migrering till Azure. | 
| Migrera – OSS – Migrera till DB för Open Source Använd Källkod (OSS) | Befintlig kund med någon av följande konkurrerande produkter: PostgreSQL, MySQL, MariaDB. Partnern bör rikta in sig på kunden för migrering till Azure. | 
| Migrera – OSS – Linux på Azure | Befintlig kund med Linux. Partnern bör rikta in sig på kunden för migrering till Azure. | 
| Migrera – SAP – SAP på Azure | Befintlig kund med SAP. Partnern bör rikta in sig på kunden för migrering till Azure. | 
| Migrera – Windows Virtual Desktop – Fjärrskrivbordstjänster IB | Identifierar kunder med aktiva Windows Fjärrskrivbordstjänster. Partnern bör rikta in sig på kunden för migrering till Azure. | 
| Migrera – Windows Virtual Desktop – Cross Sell Modern Work till Azure/WVD | Identifierar kunder med Microsoft 365 och inte har Azure. Partnern bör rikta in sig på kunden för migrering till Azure. | 
| Migrera – VMware IB | Befintlig kund med produkten: VMware. Partnern bör rikta in sig på kunden för migrering till Azure. | 
| Migrera – Citrix IB | Befintlig kund med produkten: Citrix Systems. Partnern bör rikta in sig på kunden för migrering till Azure. | 
| Innovate – Analytics – Power BI IB med hög heten i Azure | Kunder med och Active Power BI-prenumeration inklusive: Power BI – fristående Pro, Power BI – Azure-paket, Power BI – Office-paket, Power BI-paket – Microsoft 365 | 
| Aktivera – DevOps med GitHub – Visual Studio/MSDN IB | Identifierar kunder med aktiva Visual Studio versioner | 
| Windows Server Standard-version | Visar versionen av Windows Server Standard-köp av kunden | 
| Windows Server Standard-licens | Visar licenstypen för Windows Server Standard-köp av kunden | 
| Windows Server Data Center-version | Visar den version Windows datacentret köper av kunden | 
| Windows Licens för Server Data Center | Visar licenstypen för Windows Data Center-köp av kunden | 
| AzureFit | Interna och externa datapunkter som definierar företagsgrafiska data. Fit scoring använder en lookalike-modell till vår bästa SMB för att jämföra kunder och se om de är lämpliga för Microsofts molnprodukter. Bedömning av passning uppdateras kvartalsvis. | 
| AzureIntent | Signaler som rör sociala medier och en kunds onlinebeteende definierar Avsikt. Avsiktsbedömningen överlagras i Anpassa för att definiera klustren. Avsiktsbedömningen uppdateras varje månad. | 
| AzureCluster | Identifierar kundens återgivning av Azure genom att konsolidera rekommendationerna anpassa och avsikter i ett kluster. Target Act Now och Evaluate clusters, eftersom de ger högre avkastning. Rikta in dig på att utbilda kunder om det fortfarande finns kapacitet efter att du riktar in dig på Agera nu och Utvärdera kunder. | 
| WindowsServerDataCenter_HasOpenRenewal | Identifierar om kunden har en öppen förnyelse för Windows Server Datacenter | 
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
| Azure-kluster | Identifierar kundens benägenhet att köpa Azure. Target Act Now och Evaluate clusters, eftersom de ger högre avkastning. Rikta in dig på att utveckla och utbilda kunder om det fortfarande finns kapacitet efter att du riktar in dig på Agera nu och Utvärdera kunder. | 
| D365 Finance + Operations Cluster | Identifierar kundens önskemål om att köpa Dynamics 365 Finance and Operations. Kunder som visar en benägenhet för Finance + Operations finns i de översta ohanterade kategorierna. Target Act Now och Evaluate clusters, eftersom de ger högre avkastning. Rikta in dig på att utveckla och utbilda kunder om det fortfarande finns kapacitet efter att du riktar in dig på Agera nu och Utvärdera kunder. | 
| D365 CE-kluster | Identifierar kundens benägenhet att köpa Dynamics 365 Customer Engagement. Kunder som visar en benägenhet för Customer Engagement finns i kategorierna Medel och Liten. Target Act Now och Evaluate clusters, eftersom de ger högre avkastning. Rikta in dig på att utveckla och utbilda kunder om det fortfarande finns kapacitet efter att du riktar in dig på Agera nu och Utvärdera kunder. | 
| D365 BC-kluster | Identifierar kundens benägenhet att köpa Dynamics 365 Business Central. Kunder som visar en benägenhet för Business Central finns i kategorierna Medel och Liten. Target Act Now och Evaluate clusters, eftersom de ger högre avkastning. Rikta in dig på att utveckla och utbilda kunder om det fortfarande finns kapacitet efter att du riktar in dig på Agera nu och Utvärdera kunder. | 
| Microsoft 365 Kluster | Identifierar kundens benägenhet att köpa Microsoft 365. Target Act Now och Evaluate clusters, eftersom de ger högre avkastning. Rikta in dig på att utveckla och utbilda kunder om det fortfarande finns kapacitet efter att du riktar in dig på Agera nu och Utvärdera kunder. | 
| Licensprogram | Identifierar licensprogramtypen för förnyelsen | 
| Avtals-ID | Identifierare för avtalet | 
| Avtalets slutdatum | Avtalets slutdatum | 
| Förfallotyp | Typ av förfallotid | 
| Intäkter som går ut | Intäkter som är associerade med utgående prenumerationer | 
| Har EA | Anger om en förnyelse är en EA- eller EA-prenumeration | 
| Har öppen | Anger om en förnyelse är ett Open- eller Open Value-avtal | 
| Azure Upsell-kund | Identifierar om kunden visar huruvida säljförsäljning är huruvida Azure är specifikt | 
| Microsoft 365 Sälja kund | Anger om kunden visar huruvida säljförsäljningen är Microsoft 365 | 
| RevSumDivisionName | Identifierar den produkt som är upp för förnyelse | 

## <a name="next-steps"></a>Nästa steg

Mer information finns i Ladda [ned rapporter.](insights-download-reports.md)
