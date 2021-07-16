---
title: Lista över systemfrågor för programmatisk åtkomst till partnerinsikter
description: Läs mer om de systemfrågor som du kan använda för att få åtkomst till analysdata för partnerinsikter.
ms.topic: reference
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 07/14/2021
ms.openlocfilehash: 4b0bd5411d02463b015cf812cde78e34ef853814
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 07/16/2021
ms.locfileid: "114376919"
---
# <a name="list-of-system-queries-for-partner-insights-programmatic-access"></a><span data-ttu-id="443bd-103">Lista över systemfrågor för programmatisk åtkomst till partnerinsikter</span><span class="sxs-lookup"><span data-stu-id="443bd-103">List of system queries for partner insights programmatic access</span></span>

<span data-ttu-id="443bd-104">Följande systemfrågor kan användas i API:et [för att skapa rapport](insights-programmatic-access-paradigm.md#create-report-api) direkt med ett QueryId.</span><span class="sxs-lookup"><span data-stu-id="443bd-104">The following system queries can be used in the [Create Report API](insights-programmatic-access-paradigm.md#create-report-api) directly with a QueryId.</span></span> <span data-ttu-id="443bd-105">Systemfrågorna liknar exportrapporterna i Partnercenter under en beräkningsperiod på sex månader (6 miljoner).</span><span class="sxs-lookup"><span data-stu-id="443bd-105">The system queries are like the export reports in Partner Center for a six-month (6M) computation period.</span></span>

<span data-ttu-id="443bd-106">Mer information om kolumnnamn, attribut och beskrivning finns i [Datadefinitioner](insights-data-definitions.md)</span><span class="sxs-lookup"><span data-stu-id="443bd-106">For more details on the column names, attributes, and description, please refer to the [Data Definitions](insights-data-definitions.md)</span></span>

<span data-ttu-id="443bd-107">Följande avsnitt innehåller rapportfrågor för olika rapporter.</span><span class="sxs-lookup"><span data-stu-id="443bd-107">The following sections provide report queries for various reports.</span></span>

## <a name="customers"></a><span data-ttu-id="443bd-108">Kunder</span><span class="sxs-lookup"><span data-stu-id="443bd-108">Customers</span></span>

<span data-ttu-id="443bd-109">Rapporten Kunder för de senaste sex månaderna</span><span class="sxs-lookup"><span data-stu-id="443bd-109">The Customers report for the last six months</span></span>

<span data-ttu-id="443bd-110">Fråge-ID: `6664daf3-c161-423a-92a1-0ea6db2c0384`</span><span class="sxs-lookup"><span data-stu-id="443bd-110">Query ID: `6664daf3-c161-423a-92a1-0ea6db2c0384`</span></span>

### <a name="report-query"></a><span data-ttu-id="443bd-111">Rapportfråga</span><span class="sxs-lookup"><span data-stu-id="443bd-111">Report query</span></span>
```sql
SELECT PGAMpnId,MpnId,PartnerName,CustomerName,CustomerTpid,DUNSNumber,CustomerSegment,TopSegment,
CustomerMarket,CustomerStatus,CustomerTenantId,CustomerTenantName,CustomerTenantCountry,TenantDomainName,
Product,RawProductName,ProductPartNumber,SKU,Month,PartnerLocation,PartnerAttributionType,SalesChannel,
IsDuplicateRowForPGA,AvailableSeats,BilledRevenueUSD,AzureConsumedRevenueUSD 
FROM CustomersAndTenants TIMESPAN LAST_6_MONTHS
```

## <a name="seats-subscriptions-and-revenue"></a><span data-ttu-id="443bd-112">Prenumerationer och intäkter för platser</span><span class="sxs-lookup"><span data-stu-id="443bd-112">Seats Subscriptions and Revenue</span></span>

<span data-ttu-id="443bd-113">Plats, prenumerationer och intäktsrapport för de senaste sex månaderna</span><span class="sxs-lookup"><span data-stu-id="443bd-113">Seats, subscriptions, and revenue report for the last six months</span></span>

<span data-ttu-id="443bd-114">Fråge-ID: `c9fc1c79-4408-49ff-97f9-e1aa3f155804`</span><span class="sxs-lookup"><span data-stu-id="443bd-114">Query ID: `c9fc1c79-4408-49ff-97f9-e1aa3f155804`</span></span>

### <a name="report-query"></a><span data-ttu-id="443bd-115">Rapportfråga</span><span class="sxs-lookup"><span data-stu-id="443bd-115">Report query</span></span>

```sql
SELECT PGAMpnId,MpnId,SubscriptionId,SubscriptionStartDate,SubscriptionEndDate,SubscriptionState,month,
IsAutoRenew,CustomerName,CustomerTenantId,CustomerTpid,DUNSNumber,CustomerSegment,TopSegment,CustomerMarket,
ProductFamily,ReportingProductName,Product,RawProductName,ProductPartNumber,SKU,RevSumDivisionName,PartnerName,
SolutionArea,PartnerLocation,PartnerAttributionType,SalesChannel,PricingLevel,EnrollmentNumber,
IsDuplicateRowForPGA,SubscriptionStartMonth,TotalSoldSeats,TotalAssignedSeats,BilledRevenueUSD,
AzureConsumedRevenueUSD FROM SeatsSubscriptionsAndRevenue TIMESPAN LAST_6_MONTHS
```

## <a name="partner-profile"></a><span data-ttu-id="443bd-116">Partnerprofil</span><span class="sxs-lookup"><span data-stu-id="443bd-116">Partner Profile</span></span>

<span data-ttu-id="443bd-117">Profildata</span><span class="sxs-lookup"><span data-stu-id="443bd-117">Profile data</span></span>

<span data-ttu-id="443bd-118">Fråge-ID: `e65f3a4f-fb99-4319-97ff-59e57566a871`</span><span class="sxs-lookup"><span data-stu-id="443bd-118">Query ID: `e65f3a4f-fb99-4319-97ff-59e57566a871`</span></span>

### <a name="report-query"></a><span data-ttu-id="443bd-119">Rapportfråga</span><span class="sxs-lookup"><span data-stu-id="443bd-119">Report query</span></span>

```sql
SELECT MPNId,PartnerName,PGA_MPNId,PGA_PartnerName,City,Country,HierarchyLevel 
FROM Profile
```

## <a name="azure-usage"></a><span data-ttu-id="443bd-120">Azure-användning</span><span class="sxs-lookup"><span data-stu-id="443bd-120">Azure Usage</span></span>

<span data-ttu-id="443bd-121">AzureUsage-rapport för de senaste sex månaderna</span><span class="sxs-lookup"><span data-stu-id="443bd-121">AzureUsage report for the last six months</span></span>

<span data-ttu-id="443bd-122">Fråge-ID: `d1a4d75e-5ca8-4847-845f-ee0a9be6f07b`</span><span class="sxs-lookup"><span data-stu-id="443bd-122">Query ID: `d1a4d75e-5ca8-4847-845f-ee0a9be6f07b`</span></span>

### <a name="report-query"></a><span data-ttu-id="443bd-123">Rapportfråga</span><span class="sxs-lookup"><span data-stu-id="443bd-123">Report query</span></span>

```sql
SELECT PGAMpnId,SubscriptionId,SubscriptionStartDate,SubscriptionEndDate,FirstUseDate,SubscriptionState,Month,
ServiceName,MeterCategory,UsageUnits,UsageQuantity,CustomerName,CustomerTenantId,CustomerTpid,CustomerSegment,
CustomerMarket,MpnId,PartnerName,PartnerLocation,PartnerAttributionType,SalesChannel,EnrollmentNumber,
IsACRDuplicateAtPGALevel,ResellerID,ResellerName,MonthlySubscriptionLevelACR,TotalACR 
FROM AzureUsage TIMESPAN LAST_6_MONTHS
```

## <a name="office-usage"></a><span data-ttu-id="443bd-124">Office Användning</span><span class="sxs-lookup"><span data-stu-id="443bd-124">Office Usage</span></span>

<span data-ttu-id="443bd-125">OfficeAnvändarrapport för de senaste sex månaderna</span><span class="sxs-lookup"><span data-stu-id="443bd-125">OfficeUsage report for the last six months</span></span>

<span data-ttu-id="443bd-126">Fråge-ID: `d8349f7b-a7d1-467e-b26d-434d4a50f26a`</span><span class="sxs-lookup"><span data-stu-id="443bd-126">Query ID: `d8349f7b-a7d1-467e-b26d-434d4a50f26a`</span></span>

### <a name="report-query"></a><span data-ttu-id="443bd-127">Rapportfråga</span><span class="sxs-lookup"><span data-stu-id="443bd-127">Report query</span></span>

```sql
SELECT CustomerTenantId,CustomerTpid,WorkloadName,Month,PaidAvailableUnits,MonthlyActiveUsers,CustomerName,
CustomerMarket,CustomerSegment,MPNId,PartnerName,PartnerLocation,PartnerAttributionType,IsDuplicateRowForPGA
FROM OfficeUsage TIMESPAN LAST_6_MONTHS
```

## <a name="dynamics-usage"></a><span data-ttu-id="443bd-128">Dynamics-användning</span><span class="sxs-lookup"><span data-stu-id="443bd-128">Dynamics Usage</span></span>

<span data-ttu-id="443bd-129">DynamicsUsage-rapport i sex månader</span><span class="sxs-lookup"><span data-stu-id="443bd-129">DynamicsUsage report for six months</span></span>

<span data-ttu-id="443bd-130">Fråge-ID: `6209a8fd-93af-442e-8b3f-3df0f77e8463`</span><span class="sxs-lookup"><span data-stu-id="443bd-130">Query ID: `6209a8fd-93af-442e-8b3f-3df0f77e8463`</span></span>

### <a name="report-query"></a><span data-ttu-id="443bd-131">Rapportfråga</span><span class="sxs-lookup"><span data-stu-id="443bd-131">Report query</span></span>

```sql
SELECT SubscriptionId,SubscriptionStartDate,SubscriptionEndDate,SubscriptionStatus,Month,RevSumDivisionName,
RevSumCategoryName,SKU,SKUId,FreeVsPaidSKU,SalesModel,DetailedSalesModel,CustomerName,CustomerTenantId,
CustomerTpid,CustomerSegment,CustomerMarket,MPNId,PartnerName,PartnerLocation,PartnerAttachType,AvailableSeats,
AssignedSeats,ActiveSeats,DeploymentOpportunity,ActiveUsagePercent 
FROM DynamicsUsage TIMESPAN LAST_6_MONTHS
```

## <a name="power-bi-usage"></a><span data-ttu-id="443bd-132">Power BI-användning</span><span class="sxs-lookup"><span data-stu-id="443bd-132">Power BI usage</span></span>

<span data-ttu-id="443bd-133">PowerBIUsage-rapport i sex månader</span><span class="sxs-lookup"><span data-stu-id="443bd-133">PowerBIUsage report for six months</span></span>

<span data-ttu-id="443bd-134">Fråge-ID: `40ebfe2f-7183-4427-a911-5c9b45b6df15`</span><span class="sxs-lookup"><span data-stu-id="443bd-134">Query ID: `40ebfe2f-7183-4427-a911-5c9b45b6df15`</span></span>

### <a name="report-query"></a><span data-ttu-id="443bd-135">Rapportfråga</span><span class="sxs-lookup"><span data-stu-id="443bd-135">Report query</span></span>

```sql
SELECT SubscriptionId,SubscriptionStartDate,SubscriptionEndDate,SubscriptionStatus,Month,SKU,SKUId,
FreeVsPaidSKU,SalesModel,DetailedSalesModel,CustomerName,CustomerTenantId,CustomerTpid,CustomerSegment,
CustomerMarket,MPNId,PartnerName,PartnerLocation,PartnerAttachType,PartnerHierarchy,AvailableSeats,
AssignedSeats,ActiveSeats,DeploymentOpportunity,ActiveUsagePercent 
FROM PowerBIUsage TIMESPAN LAST_6_MONTHS
```

## <a name="ems-usage"></a><span data-ttu-id="443bd-136">EMS-användning</span><span class="sxs-lookup"><span data-stu-id="443bd-136">EMS Usage</span></span>

<span data-ttu-id="443bd-137">EMSUsage-rapport i sex månader</span><span class="sxs-lookup"><span data-stu-id="443bd-137">EMSUsage report for six months</span></span>

<span data-ttu-id="443bd-138">Fråge-ID: `d7f20ea4-8751-4d6b-b1d7-821c316acd6a`</span><span class="sxs-lookup"><span data-stu-id="443bd-138">Query ID: `d7f20ea4-8751-4d6b-b1d7-821c316acd6a`</span></span>

### <a name="report-query"></a><span data-ttu-id="443bd-139">Rapportfråga</span><span class="sxs-lookup"><span data-stu-id="443bd-139">Report query</span></span>

```sql
SELECT SubscriptionId,SubscriptionStartDate,SubscriptionEndDate,SubscriptionStatus,Month,SKU,SKUId,
FreeVsPaidSKU,SalesModel,DetailedSalesModel,CustomerName,CustomerTenantId,CustomerTpid,CustomerSegment,
CustomerMarket,MPNId,PartnerName,PartnerLocation,PartnerAttachType,PartnerHierarchy,PaidAvailableUnits,
MonthlyActiveUsers,AADPPaidAvailableUnits,IntunePaidAvailableUnits,AzipPaidAvailableUnits,
AADPMonthlyActiveUsers,IntuneMonthlyActiveUsers,AzipMonthlyActiveUsers FROM EMSUsage TIMESPAN LAST_6_MONTHS
```

## <a name="competency-performance-requirement-report"></a><span data-ttu-id="443bd-140">Rapport om prestandakrav för kompetens</span><span class="sxs-lookup"><span data-stu-id="443bd-140">Competency Performance requirement report</span></span>

<span data-ttu-id="443bd-141">CompetencyPeformanceRequirement-rapport i sex månader</span><span class="sxs-lookup"><span data-stu-id="443bd-141">CompetencyPeformanceRequirement report for six months</span></span>

<span data-ttu-id="443bd-142">Fråge-ID: `3a0e1adc-f5c1-42ac-9422-8e944bf81ae5`</span><span class="sxs-lookup"><span data-stu-id="443bd-142">Query ID: `3a0e1adc-f5c1-42ac-9422-8e944bf81ae5`</span></span>

### <a name="report-query"></a><span data-ttu-id="443bd-143">Rapportfråga</span><span class="sxs-lookup"><span data-stu-id="443bd-143">Report query</span></span>

```sql
SELECT CompetencyName,CompetencyAttainmentOptionName,Month,MetricName,MetricMonthlyContribution,TTMAggregate,
AnniversaryYearAggregate,GoldThreshold,SilverThreshold 
FROM CompetencyPeformanceRequirement 
TIMESPAN LAST_6_MONTHS
```

## <a name="cloud-products-reseller-performance"></a><span data-ttu-id="443bd-144">Prestanda för återförsäljare av molnprodukter</span><span class="sxs-lookup"><span data-stu-id="443bd-144">Cloud products reseller performance</span></span>

### <a name="report-description"></a><span data-ttu-id="443bd-145">Rapportbeskrivning</span><span class="sxs-lookup"><span data-stu-id="443bd-145">Report description</span></span>

<span data-ttu-id="443bd-146">CloudProductsResellerPerformance-rapport i sex månader</span><span class="sxs-lookup"><span data-stu-id="443bd-146">CloudProductsResellerPerformance report for six months</span></span>

<span data-ttu-id="443bd-147">Fråge-ID: `c09c2eda-861b-4664-8ee8-48a14745a26a`</span><span class="sxs-lookup"><span data-stu-id="443bd-147">Query ID: `c09c2eda-861b-4664-8ee8-48a14745a26a`</span></span>

### <a name="report-query"></a><span data-ttu-id="443bd-148">Rapportfråga</span><span class="sxs-lookup"><span data-stu-id="443bd-148">Report query</span></span>

```sql
SELECT ResellerMpnid,ResellerName,ResellerMarket,IndirectProviderMPNId,IndirectProviderName,Month,Product,
SubscriptionID,AvailableSeats,AssignedSeats,BilledRevenueUSD,CustomerName,CustomerTPid,CustomerSegment,
CustomerMarket,ResellerStatus 
FROM CloudProductsResellerPerformance TIMESPAN LAST_6_MONTHS
```

## <a name="clas-agreement-renewal-propensity"></a><span data-ttu-id="443bd-149">Benägenhet att förnya CLAS-avtal</span><span class="sxs-lookup"><span data-stu-id="443bd-149">CLAS Agreement Renewal propensity</span></span>

<span data-ttu-id="443bd-150">CLASAgreementRenewalsPropensity-rapport i sex månader</span><span class="sxs-lookup"><span data-stu-id="443bd-150">CLASAgreementRenewalsPropensity report for six months</span></span>

<span data-ttu-id="443bd-151">Fråge-ID: `c4fc87ac-4cca-44cd-bf4d-835ac513f9ee`</span><span class="sxs-lookup"><span data-stu-id="443bd-151">Query ID: `c4fc87ac-4cca-44cd-bf4d-835ac513f9ee`</span></span>

### <a name="report-query"></a><span data-ttu-id="443bd-152">Rapportfråga</span><span class="sxs-lookup"><span data-stu-id="443bd-152">Report query</span></span>

```sql
SELECT MPNID,PartnerName,CustomerID,DUNSNumber,AccountName,Domain,OrgSize,Industry,Vertical,Area,Subsidiary,
SalesTerritory,City,State,PostalCode,Country,Segment,SubSegment,SMCTypeSummary,TopUnmanagedComputeBase,
TopUnmanagedUserBase,IsNonProfit,HasGoogle,HasAWS,AzureCluster,D365FOCluster,D365CECluster,D365BCCluster,
M365Cluster,LicenseProgram,AgreementID,AgreementEndDate,ExpirationType,ExpiringRevenue,HasEA,HasOpen,
AzureUpsellCustomer,M365UpsellCustomer,RevSumDivisionName 
FROM CLASAgreementRenewalsPropensity
```

## <a name="clas-azure-propensity"></a><span data-ttu-id="443bd-153">CLAS Azure-benägenhet</span><span class="sxs-lookup"><span data-stu-id="443bd-153">CLAS Azure propensity</span></span>

<span data-ttu-id="443bd-154">CLASAzurePropensity-rapport i sex månader</span><span class="sxs-lookup"><span data-stu-id="443bd-154">CLASAzurePropensity report for six months</span></span>

<span data-ttu-id="443bd-155">Fråge-ID: `9a18bd70-8f90-4bd2-8266-5f6e453e3ee7`</span><span class="sxs-lookup"><span data-stu-id="443bd-155">Query ID: `9a18bd70-8f90-4bd2-8266-5f6e453e3ee7`</span></span>

### <a name="report-query"></a><span data-ttu-id="443bd-156">Rapportfråga</span><span class="sxs-lookup"><span data-stu-id="443bd-156">Report query</span></span>

```sql
SELECT MPNID,PartnerName,CustomerID,DUNSNumber,AccountName,Domain,OrgSize,Industry,Vertical,Area,Subsidiary,
SalesTerritory,City,State,PostalCode,Country,Segment,SubSegment,SMCTypeSummary,TopUnmanagedComputeBase,
TopUnmanagedUserBase,IsNonProfit,MigrateEOSWinServerWithCLASPropensityAbove5Licenses,
MigrateEOSWinServerWithCLASPropensityBelow5Licenses,
MigrateEOSWinServerWithoutCLASPropensityAbove5Licenses,
MigrateEOSWinServerWithoutCLASPropensityBelow5Licenses,MigrateEOSSQLWithCLASPropensityAbove5Licenses,
MigrateEOSSQLWithCLASPropensityBelow5Licenses,MigrateEOSSQLWithoutCLASPropensityAbove5Licenses,
MigrateEOSSQLWithoutCLASPropensityBelow5Licenses,
MigrateOnPremWinServerCurrentWindowsServerWithCLASPropensityAbove5Licenses,
MigrateOnPremWinServerCurrentWindowsServerWithCLASPropensityBelow5Licenses,
MigrateOnPremWinServerCurrentWindowsServerWithoutCLASPropensityAbove5Licenses,
MigrateOnPremWinServerCurrentWindowsServerIBWithoutCLASPropensityBelow5Licenses,
MigrateToAzureSQLOrSQLVMsCurrentSQLServerWithCLASPropensityAbove5Licenses,
MigrateToAzureSQLOrSQLVMsCurrentSQLServerWithCLASPropensityBelow5Licenses,
MigrateToAzureSQLOrSQLVMsCurrentSQLServerWithoutCLASPropensityAbove5Licenses,
MigrateToAzureSQLOrSQLVMsCurrentSQLServerWithoutCLASPropensityBelow5Licenses,MigrateOSSMigrateToOSSDB,
MigrateOSSLinuxOnAzure,MigrateSAPOnAzure,MigrateWVDRDSIB,MigrateWVDCrossSellModernWorkToAzureWVD,
MigrateVMWareIB,MigrateCitrixIB,InnovateAnalyticsPowerBIIBWithHighAzurepropensity,
EnableDevOpsWithGitHubVisualStudioMSDNIB,WinServerStandardVersion,WinServerStandardLicense,
WinServerDataCenterVersion,WinServerDataCenterLicense,AzureFit,AzureIntent,AzureCluster,
WindowsServerDataCenter_HasOpenRenewal,WindowsServerStandard_HasOpenRenewal,AzureUpsellCustomer,HasGoogle,
HasAWS,HasEA,HasOpen 
FROM CLASAzurePropensity
```

## <a name="clas-d365-propensity"></a><span data-ttu-id="443bd-157">CLAS D365-benägenhet</span><span class="sxs-lookup"><span data-stu-id="443bd-157">CLAS D365 propensity</span></span>

<span data-ttu-id="443bd-158">CLASD365Propensity-rapport i sex månader</span><span class="sxs-lookup"><span data-stu-id="443bd-158">CLASD365Propensity report for six months</span></span>

<span data-ttu-id="443bd-159">Fråge-ID: `258fdcac-6e9c-4072-af27-b1b3d97be16c`</span><span class="sxs-lookup"><span data-stu-id="443bd-159">Query ID: `258fdcac-6e9c-4072-af27-b1b3d97be16c`</span></span>

### <a name="report-query"></a><span data-ttu-id="443bd-160">Rapportfråga</span><span class="sxs-lookup"><span data-stu-id="443bd-160">Report query</span></span>

```sql
SELECT MPNID,PartnerName,CustomerID,DUNSNumber,AccountName,Domain,OrgSize,Industry,Vertical,Area,Subsidiary,
SalesTerritory,City,State,PostalCode,Country,Segment,SubSegment,SMCTypeSummary,TopUnmanagedComputeBase,
TopUnmanagedUserBase,IsNonProfit,ActivateDigitalSellingM365SeatSizeAbove25SeatsSalesProPropensityModel,
ActivateDigitalSellingD365SalesProPropensityActNowOrEvaluate,
ManagingFinancialRiskAndFraudDynamicsOnPremInstallBaseNavisionBCPropensityModel,
ManagingFinancialRiskAndFraudDynamicsOnPremInstallBaseAXFAndOPropensityModel,
ManagingFinancialRiskAndFraudDynamicsOnPremInstallBaseGreatPlainsBCPropensityModel,
ManagingFinancialRiskAndFraudDynamicsOnPremInstallBaseSolomonBCPropensityModel,
ManagingFinancialRiskAndFraudDynamicsOnPremInstallBaseOthersBCPropensityModel,
ManagingFinancialRiskAndFraudNewCustomerAcquisitionFAndOPropensityModel,
ManagingFinancialRiskAndFraudNewCustomerAcquisitionBCPropensityModel,
BuildAgileBusinessProcessesDynamicsOnPremInstallBaseAXGPSLNAVOtherD365PropensityModel,
BuildAgileBusinessProcessesDynamicsCompeteBaseMendixOutsystemsSalesforceD365PropensityModel,
BuildAgileBusinessProcessesD365FAndOInstallBase,BuildAgileBusinessProcessesD365BCInstallBase,
BuildAgileBusinessProcessesD365CEInstallBase,
BuildaResilientSupplyChainWinandActivateFirstD365WorkloadasD365SupplyChainwithNonOracleSAPERPCustomers,
BuildaResilientSupplyChainCrossSellD365SupplyChainANDORRetailCommercetoExistingD365CECustomers,
BuildaResilientSupplyChainCrossSellD365SupChainANDORRetailCommercetoD365CEANDOracleORSAP,D365BCCluster,
D365BCFit,D365BCIntent,D365FOCluster,D365FOFit,D365FOIntent,D365CECluster,D365CEFit,D365CEIntent,
DynamicsOnPremAXorCRM_HasOpenRenewal,M365UpsellCustomer,HasGoogle,HasAWS,HasEA,HasOpen 
FROM CLASD365Propensity
```

## <a name="clas-m365-propensity"></a><span data-ttu-id="443bd-161">CLAS M365-benägenhet</span><span class="sxs-lookup"><span data-stu-id="443bd-161">CLAS M365 propensity</span></span>

<span data-ttu-id="443bd-162">CLASM365Propensity-rapport i sex månader</span><span class="sxs-lookup"><span data-stu-id="443bd-162">CLASM365Propensity report for six months</span></span>

<span data-ttu-id="443bd-163">Fråge-ID: `fbe00e32-fdde-4465-b3e4-41bbd021a130`</span><span class="sxs-lookup"><span data-stu-id="443bd-163">Query ID: `fbe00e32-fdde-4465-b3e4-41bbd021a130`</span></span>

### <a name="report-query"></a><span data-ttu-id="443bd-164">Rapportfråga</span><span class="sxs-lookup"><span data-stu-id="443bd-164">Report query</span></span>

```sql
SELECT MPNID,PartnerName,CustomerID,DUNSNumber,AccountName,Domain,OrgSize,Industry,Vertical,Area,Subsidiary,
SalesTerritory,City,State,PostalCode,Country,Segment,SubSegment,SMCTypeSummary,TopUnmanagedComputeBase,
TopUnmanagedUserBase,IsNonProfit,EnableRemoteWorkTargetExchangeOnline,
EnableRemoteWorkOnPremAcquisitionCurrentVersionwithCLASPropensityAbove10Licenses,
EnableRemoteWorkOnPremAcquisitionCurrentVersionwithCLASPropensityBelow10Licenses,
EnableRemoteWorkOnPremAcquisitionCurrentVersionwithoutCLASPropensityAbove10Licenses,
EnableRemoteWorkOnPremAcquisitionCurrentVersionwithoutCLASPropensityBelow10Licenses,
EnableRemoteWorkOnPremAcquisitionEOSwithCLASPropensityAbove10Licenses,
EnableRemoteWorkOnPremAcquisitionEOSwithCLASPropensityBelow10Licenses,
EnableRemoteWorkOnPremAcquisitionEOSwithoutCLASPropensityAbove10Licenses,
EnableRemoteWorkOnPremAcquisitionEOSwithoutCLASPropensityBelow10Licenses,
EnableRemoteWorkHighPropensityProspectforM365ActNowEvaluate,EnableRemoteWorkCompeteZoomwithM365,
EnableRemoteWorkCompeteZoomwithoutM365,ReduceCostandManageM365E3targetedforM365E5,
ReduceCostandManageM365BBandBScustomerstargetedforM365BP,TransformOrganizationalProductivitySurfacePropensity,
M365Cluster,M365Fit,M365Intent,SurfaceCluster,SurfaceFit,SurfaceIntent,O365Cluster,O365Fit,O365Intent,
M365UpsellCustomer,HasGoogle,HasAWS,HasEA,HasOpen 
FROM CLASM365Propensity
```

## <a name="teams-usage-3p-apps"></a><span data-ttu-id="443bd-165">Teams Användning 3P-appar</span><span class="sxs-lookup"><span data-stu-id="443bd-165">Teams Usage 3P Apps</span></span>

<span data-ttu-id="443bd-166">TeamsUsage3PApps-rapport i sex månader</span><span class="sxs-lookup"><span data-stu-id="443bd-166">TeamsUsage3PApps report for six months</span></span>

<span data-ttu-id="443bd-167">Fråge-ID: `42d287be-cc76-4109-a066-f3140ad97fe2`</span><span class="sxs-lookup"><span data-stu-id="443bd-167">Query ID: `42d287be-cc76-4109-a066-f3140ad97fe2`</span></span>

### <a name="report-query"></a><span data-ttu-id="443bd-168">Rapportfråga</span><span class="sxs-lookup"><span data-stu-id="443bd-168">Report query</span></span>

```sql
SELECT CustomerId,CustomerTenantId,CustomerName,CustomerCountry,DateKey,AppName,UserCount 
FROM TeamsUsage3PApps TIMESPAN LAST_6_MONTHS
```

## <a name="teams-usage-workload"></a><span data-ttu-id="443bd-169">Teams användningsarbetsbelastning</span><span class="sxs-lookup"><span data-stu-id="443bd-169">Teams usage workload</span></span>

<span data-ttu-id="443bd-170">TeamsUsageWorkload-rapport i sex månader</span><span class="sxs-lookup"><span data-stu-id="443bd-170">TeamsUsageWorkload report for six months</span></span>

<span data-ttu-id="443bd-171">Fråge-ID: `817fe875-acb0-4c45-9201-b7a35a60235a`</span><span class="sxs-lookup"><span data-stu-id="443bd-171">Query ID: `817fe875-acb0-4c45-9201-b7a35a60235a`</span></span>

### <a name="report-query"></a><span data-ttu-id="443bd-172">Rapportfråga</span><span class="sxs-lookup"><span data-stu-id="443bd-172">Report query</span></span>

```sql
SELECT CustomerId,CustomerTenantId,MonthKey,SubWorkload,DesktopUsers,WebUsers,MobileUsers,AllUpPartiticipants
FROM TeamsUsageWorkload TIMESPAN LAST_6_MONTHS
```

## <a name="teams-usage-meetings-and-calls"></a><span data-ttu-id="443bd-173">Teams användningsmöten och anrop</span><span class="sxs-lookup"><span data-stu-id="443bd-173">Teams usage meetings and calls</span></span>

<span data-ttu-id="443bd-174">TeamsUsageMeetingsAndCalls-rapport i sex månader</span><span class="sxs-lookup"><span data-stu-id="443bd-174">TeamsUsageMeetingsAndCalls report for six months</span></span>

<span data-ttu-id="443bd-175">Fråge-ID: `b7bd73a8-47e8-4c57-b915-445708cfd7bf`</span><span class="sxs-lookup"><span data-stu-id="443bd-175">Query ID: `b7bd73a8-47e8-4c57-b915-445708cfd7bf`</span></span>

### <a name="report-query"></a><span data-ttu-id="443bd-176">Rapportfråga</span><span class="sxs-lookup"><span data-stu-id="443bd-176">Report query</span></span>

```sql
SELECT CustomerId,CustomerTenantId,DateKey,SubWorkload,MeetingCount,MeetingDuration 
FROM TeamsUsageMeetingsAndCalls TIMESPAN LAST_6_MONTHS
```

## <a name="competency-summary-history"></a><span data-ttu-id="443bd-177">Sammanfattningshistorik för kompetens</span><span class="sxs-lookup"><span data-stu-id="443bd-177">Competency summary history</span></span>

<span data-ttu-id="443bd-178">CompetencySummaryHistory-rapport i sex månader</span><span class="sxs-lookup"><span data-stu-id="443bd-178">CompetencySummaryHistory report for six months</span></span>

<span data-ttu-id="443bd-179">Fråge-ID: `fddab2aa-523d-47f6-90fe-588557306db4`</span><span class="sxs-lookup"><span data-stu-id="443bd-179">Query ID: `fddab2aa-523d-47f6-90fe-588557306db4`</span></span>

### <a name="report-query"></a><span data-ttu-id="443bd-180">Rapportfråga</span><span class="sxs-lookup"><span data-stu-id="443bd-180">Report query</span></span>

```sql
SELECT CompetencyName,CompetencyLevel,CompetencyStatus,CompetencyStartDate,CompetencyEndDate 
FROM CompetencySummaryHistory TIMESPAN LAST_6_MONTHS
```

## <a name="training-completion"></a><span data-ttu-id="443bd-181">Slutförande av träning</span><span class="sxs-lookup"><span data-stu-id="443bd-181">Training completion</span></span>

<span data-ttu-id="443bd-182">Rapport om slutförd träning i sex månader</span><span class="sxs-lookup"><span data-stu-id="443bd-182">Training Completions report for six months</span></span>

<span data-ttu-id="443bd-183">Fråge-ID: `20f5da57-3c2a-481b-b6a0-ec34d6db14e2`</span><span class="sxs-lookup"><span data-stu-id="443bd-183">Query ID: `20f5da57-3c2a-481b-b6a0-ec34d6db14e2`</span></span>

### <a name="report-query"></a><span data-ttu-id="443bd-184">Rapportfråga</span><span class="sxs-lookup"><span data-stu-id="443bd-184">Report query</span></span>

```sql
SELECT TrainingActivityId,TrainingTitle,TrainingType,AADUserId,TrainingCompletionDate,Month,IcMCP,MCPID,MPNId,
PartnerName,PartnerCityLocation,PartnerCountryLocation 
FROM TrainingCompletions TIMESPAN LAST_6_MONTHS
```

## <a name="microsoft-learn"></a><span data-ttu-id="443bd-185">Microsoft Learn</span><span class="sxs-lookup"><span data-stu-id="443bd-185">Microsoft Learn</span></span>

<span data-ttu-id="443bd-186">Microsoft Learn rapport för de senaste sex månaderna</span><span class="sxs-lookup"><span data-stu-id="443bd-186">Microsoft Learn report for the last six months</span></span>

<span data-ttu-id="443bd-187">Fråge-ID: `0e06c7c3-75ab-4cd5-8178-8cf1a2de49cc`</span><span class="sxs-lookup"><span data-stu-id="443bd-187">Query ID: `0e06c7c3-75ab-4cd5-8178-8cf1a2de49cc`</span></span>

### <a name="report-query"></a><span data-ttu-id="443bd-188">Rapportfråga</span><span class="sxs-lookup"><span data-stu-id="443bd-188">Report query</span></span>

```sql
SELECT UserName,UserId,TrainingName,TrainingType,Products,Roles,CompletionDate,MPNId,PartnerName,CustomerMarket 
FROM MSLearn TIMESPAN LAST_6_MONTHS
```

## <a name="next-steps"></a><span data-ttu-id="443bd-189">Nästa steg</span><span class="sxs-lookup"><span data-stu-id="443bd-189">Next steps</span></span>

- [<span data-ttu-id="443bd-190">API:er för åtkomst till analysdata för partnerinsikter</span><span class="sxs-lookup"><span data-stu-id="443bd-190">APIs for accessing partner insights analytics data</span></span>](insights-programmatic-analytics-available-api.md)
- [<span data-ttu-id="443bd-191">Exempelprogram för åtkomst till analysdata för partnerinsikter</span><span class="sxs-lookup"><span data-stu-id="443bd-191">Sample application for accessing partner insights analytics data</span></span>](insights-programmatic-sample-application.md)