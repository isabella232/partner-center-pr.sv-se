---
title: Gör ditt första API-anrop för att få åtkomst till analysdata för partnerinsikter
description: Exempel för att lära dig att använda API:et för att få åtkomst till analysdata från partnerinsikter.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 07/14/2021
ms.openlocfilehash: d2252ccfb601ae22ce106d87fb06b67bf0927df5
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 07/16/2021
ms.locfileid: "114376955"
---
# <a name="make-your-first-api-call-to-access-partner-insights-analytics-data"></a><span data-ttu-id="1f9b6-103">Gör ditt första API-anrop för att få åtkomst till analysdata för partnerinsikter</span><span class="sxs-lookup"><span data-stu-id="1f9b6-103">Make your first API call to access partner insights analytics data</span></span>

<span data-ttu-id="1f9b6-104">En lista över API:er för åtkomst till analysdata för partnerinsikter finns i [API:er för åtkomst till analysdata för partnerinsikter.](insights-programmatic-analytics-available-api.md)</span><span class="sxs-lookup"><span data-stu-id="1f9b6-104">For a list of the APIs for accessing partner insights analytics data, see [APIs for accessing partner insights analytics data](insights-programmatic-analytics-available-api.md).</span></span> <span data-ttu-id="1f9b6-105">Innan du gör ditt första [API-anrop](insights-programmatic-prerequisites.md) måste du se till att du har uppfyllt kraven för att programmatiskt få åtkomst till Partner Insights-analysdata.</span><span class="sxs-lookup"><span data-stu-id="1f9b6-105">Before you make your first API call, make sure that you met the [pre-requisites](insights-programmatic-prerequisites.md) to programmatically access Partner Insights analytics data.</span></span>

## <a name="token-generation"></a><span data-ttu-id="1f9b6-106">Tokengenerering</span><span class="sxs-lookup"><span data-stu-id="1f9b6-106">Token generation</span></span>

<span data-ttu-id="1f9b6-107">Innan du anropar någon av metoderna måste du först hämta en Azure Active Directory (AAD) åtkomsttoken.</span><span class="sxs-lookup"><span data-stu-id="1f9b6-107">Before calling any of the methods, you must first obtain an Azure Active Directory (AAD) access token.</span></span> <span data-ttu-id="1f9b6-108">Du måste skicka Azure AD-åtkomsttoken till auktoriseringsrubriken för varje metod i API:et.</span><span class="sxs-lookup"><span data-stu-id="1f9b6-108">You need to pass the Azure AD access token to the Authorization header of each method in the API.</span></span> <span data-ttu-id="1f9b6-109">När du har fått en åtkomsttoken har du 60 minuter på dig att använda den innan den upphör att gälla.</span><span class="sxs-lookup"><span data-stu-id="1f9b6-109">After obtaining an access token, you have 60 minutes to use it before it expires.</span></span> <span data-ttu-id="1f9b6-110">När token har upphört att gälla kan du uppdatera token och fortsätta att använda den för ytterligare anrop till API:et.</span><span class="sxs-lookup"><span data-stu-id="1f9b6-110">After the token expires, you can refresh the token and can continue to use it for further calls to the API.</span></span>

<span data-ttu-id="1f9b6-111">Se en exempelbegäran nedan för att generera en token.</span><span class="sxs-lookup"><span data-stu-id="1f9b6-111">Refer to a sample request below for generating a token.</span></span> <span data-ttu-id="1f9b6-112">De tre värden som krävs för att generera token är `clientId` , `clientSecret` och `tenantId` .</span><span class="sxs-lookup"><span data-stu-id="1f9b6-112">The three values that are required to generate the token are `clientId`, `clientSecret`, and `tenantId`.</span></span> <span data-ttu-id="1f9b6-113">Resursparametern ska vara inställd på `https://api.partnercenter.microsoft.com`</span><span class="sxs-lookup"><span data-stu-id="1f9b6-113">The resource parameter should be set to `https://api.partnercenter.microsoft.com`</span></span>

#### <a name="request-example"></a><span data-ttu-id="1f9b6-114">Exempel på begäran</span><span class="sxs-lookup"><span data-stu-id="1f9b6-114">Request example</span></span>

```console
curl --location --request POST 'https://login.microsoftonline.com/<tenantId>/oauth2/token' \
--header 'return-client-request-id: true' \
--header 'Content-Type: application/x-www-form-urlencoded' \
--header 'Cookie: fpc=Ar2GMei7JwdKg4Y4onHrMpvxqd4FAQAAAEhU_tcOAAAA; stsservicecookie=estsfd; x-ms-gateway-slice=estsfd' \
--data-urlencode 'resource= https://api.partnercenter.microsoft.com' \
--data-urlencode 'client_id= ' \
--data-urlencode 'client_secret= ' \
--data-urlencode 'grant_type=password' \
--data-urlencode 'scope=openid' \
--data-urlencode 'username= ' \
--data-urlencode 'password= '
```

#### <a name="response-example"></a><span data-ttu-id="1f9b6-115">Exempel på svar</span><span class="sxs-lookup"><span data-stu-id="1f9b6-115">Response example</span></span>

```json
{
    "token_type": "Bearer",
    "expires_in": "3599",
    "ext_expires_in": "3599",
    "expires_on": "1612794445",
    "not_before": "1612790545",
    "resource": "https://api.partnercenter.microsoft.com",
    "access_token": {Token}
}
```

<span data-ttu-id="1f9b6-116">Mer information om hur du hämtar en Azure AD-token för ditt program finns i [Åtkomst till analysdata med Store-tjänster.](/windows/uwp/monetize/access-analytics-data-using-windows-store-services#step-2-obtain-an-azure-ad-access-token)</span><span class="sxs-lookup"><span data-stu-id="1f9b6-116">For more information about how to obtain an Azure AD token for your application, see [Access analytics data using Store services.](/windows/uwp/monetize/access-analytics-data-using-windows-store-services#step-2-obtain-an-azure-ad-access-token)</span></span>

## <a name="programmatic-api-call"></a><span data-ttu-id="1f9b6-117">Programmatiskt API-anrop</span><span class="sxs-lookup"><span data-stu-id="1f9b6-117">Programmatic API call</span></span>

<span data-ttu-id="1f9b6-118">När du har fått AAD-token enligt beskrivningen i föregående avsnitt följer du dessa steg för att skapa din första programmässiga åtkomstrapport.</span><span class="sxs-lookup"><span data-stu-id="1f9b6-118">After you obtain the AAD Token as described in the previous section, follow these steps to create your first programmatic access report.</span></span>

<span data-ttu-id="1f9b6-119">Data kan laddas ned från följande datauppsättningar (datasetName):</span><span class="sxs-lookup"><span data-stu-id="1f9b6-119">Data can be downloaded from the following datasets (datasetName):</span></span>

- <span data-ttu-id="1f9b6-120">CustomersAndTenants</span><span class="sxs-lookup"><span data-stu-id="1f9b6-120">CustomersAndTenants</span></span>
- <span data-ttu-id="1f9b6-121">SeatsSubscriptionsAndRevenue</span><span class="sxs-lookup"><span data-stu-id="1f9b6-121">SeatsSubscriptionsAndRevenue</span></span>
- <span data-ttu-id="1f9b6-122">AzureUsage</span><span class="sxs-lookup"><span data-stu-id="1f9b6-122">AzureUsage</span></span>
- <span data-ttu-id="1f9b6-123">MSLearn</span><span class="sxs-lookup"><span data-stu-id="1f9b6-123">MSLearn</span></span>
- <span data-ttu-id="1f9b6-124">OfficeUsage</span><span class="sxs-lookup"><span data-stu-id="1f9b6-124">OfficeUsage</span></span>
- <span data-ttu-id="1f9b6-125">Profil</span><span class="sxs-lookup"><span data-stu-id="1f9b6-125">Profile</span></span>
- <span data-ttu-id="1f9b6-126">TrainingCompletions</span><span class="sxs-lookup"><span data-stu-id="1f9b6-126">TrainingCompletions</span></span>
- <span data-ttu-id="1f9b6-127">DynamicsUsage</span><span class="sxs-lookup"><span data-stu-id="1f9b6-127">DynamicsUsage</span></span>
- <span data-ttu-id="1f9b6-128">CompetencySummaryHistory</span><span class="sxs-lookup"><span data-stu-id="1f9b6-128">CompetencySummaryHistory</span></span>
- <span data-ttu-id="1f9b6-129">PowerBIUsage</span><span class="sxs-lookup"><span data-stu-id="1f9b6-129">PowerBIUsage</span></span>
- <span data-ttu-id="1f9b6-130">EMSUsage</span><span class="sxs-lookup"><span data-stu-id="1f9b6-130">EMSUsage</span></span>
- <span data-ttu-id="1f9b6-131">CompetencyPeformanceRequirement</span><span class="sxs-lookup"><span data-stu-id="1f9b6-131">CompetencyPeformanceRequirement</span></span>
- <span data-ttu-id="1f9b6-132">ResellerPerformance</span><span class="sxs-lookup"><span data-stu-id="1f9b6-132">ResellerPerformance</span></span>
- <span data-ttu-id="1f9b6-133">CLASAgreementRenewalsPropensity</span><span class="sxs-lookup"><span data-stu-id="1f9b6-133">CLASAgreementRenewalsPropensity</span></span>
- <span data-ttu-id="1f9b6-134">CLASAzurePropensity</span><span class="sxs-lookup"><span data-stu-id="1f9b6-134">CLASAzurePropensity</span></span>
- <span data-ttu-id="1f9b6-135">CLASD365Propensity</span><span class="sxs-lookup"><span data-stu-id="1f9b6-135">CLASD365Propensity</span></span>
- <span data-ttu-id="1f9b6-136">CLASM365Propensity</span><span class="sxs-lookup"><span data-stu-id="1f9b6-136">CLASM365Propensity</span></span>
- <span data-ttu-id="1f9b6-137">TeamsUsage3PApps</span><span class="sxs-lookup"><span data-stu-id="1f9b6-137">TeamsUsage3PApps</span></span>
- <span data-ttu-id="1f9b6-138">TeamsUsageWorkload</span><span class="sxs-lookup"><span data-stu-id="1f9b6-138">TeamsUsageWorkload</span></span>
- <span data-ttu-id="1f9b6-139">TeamsUsageMeetingsAndCalls</span><span class="sxs-lookup"><span data-stu-id="1f9b6-139">TeamsUsageMeetingsAndCalls</span></span>

<span data-ttu-id="1f9b6-140">I följande avsnitt visas exempel på hur du kommer åt via programmering från `SubscriptionId` DynamicsUsage-datauppsättningen.</span><span class="sxs-lookup"><span data-stu-id="1f9b6-140">In the following section, we will see examples of how to programmatically access `SubscriptionId` from the DynamicsUsage dataset.</span></span>

### <a name="step-1-make-a-rest-call-using-the-get-datasets-api"></a><span data-ttu-id="1f9b6-141">Steg 1: Gör ett REST-anrop med hjälp av API:et för att hämta datauppsättningar</span><span class="sxs-lookup"><span data-stu-id="1f9b6-141">Step 1: Make a REST call using the get datasets API</span></span>

<span data-ttu-id="1f9b6-142">API-svaret innehåller datauppsättningens namn där du kan ladda ned rapporten.</span><span class="sxs-lookup"><span data-stu-id="1f9b6-142">The API response provides the dataset name from where you can download the report.</span></span> <span data-ttu-id="1f9b6-143">För den specifika datauppsättningen innehåller API-svaret även en lista över valbara kolumner som kan användas för din anpassade rapportmall.</span><span class="sxs-lookup"><span data-stu-id="1f9b6-143">For the specific dataset, the API response also provides the list of selectable columns that can be used for your custom report template.</span></span> <span data-ttu-id="1f9b6-144">Du kan också referera till [Datadefinitioner](insights-data-definitions.md) för att hämta namnen på kolumnerna.</span><span class="sxs-lookup"><span data-stu-id="1f9b6-144">You can also refer to the [Data Definitions](insights-data-definitions.md) to get the names of the columns.</span></span>

#### <a name="request-example"></a><span data-ttu-id="1f9b6-145">Exempel på begäran</span><span class="sxs-lookup"><span data-stu-id="1f9b6-145">Request example</span></span>

```cli
curl 
--location 
--request GET 'https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledDataset'\
--header 'Authorization: Bearer <AADToken>'
```

#### <a name="response-example"></a><span data-ttu-id="1f9b6-146">Exempel på svar</span><span class="sxs-lookup"><span data-stu-id="1f9b6-146">Response example</span></span>

```json
{
  "value": [
    {
      "datasetName": "DynamicsUsage",
      "selectableColumns": [
        "PGAMpnId",
        "SubscriptionId",
        "SubscriptionStartDate",
        "SubscriptionEndDate",
        "SubscriptionStatus",
        "Month",
        "RevSumDivisionName",
        "RevSumCategoryName",
        "SKU",
        "SKUId",
        "FreeVsPaidSKU",
        "SalesModel",
        "DetailedSalesModel",
        "CustomerName",
        "CustomerTenantId",
        "CustomerTpid",
        "CustomerSegment",
        "CustomerMarket",
        "MPNId",
        "PartnerName",
        "PartnerLocation",
        "PartnerAttachType",
        "AvailableSeats",
        "AssignedSeats",
        "ActiveSeats",
        "DeploymentOpportunity",
        "ActiveUsagePercent"
      ],
      "availableMetrics": [
        "SubscriptionCount",
        "TotalAssignedSeats",
        "TotalSoldSeats",
        "TotalActiveSeats",
        "TotalRevenueAndACR",
        "CustomerCount",
        "CustomerTenantCount"
      ],
      "availableDateRanges": [
        "LAST_MONTH",
        "LAST_3_MONTHS",
        "LAST_6_MONTHS",
        "LAST_1_YEAR",
        "LIFETIME"
      ],
      "minimumRecurrenceInterval": 24
    }
  ],
  "nextLink": null,
  "totalCount": 1,
  "message": "Dataset fetched successfully",
  "statusCode": 200,
  "dataRedacted": false
}
```

### <a name="step-2-create-the-custom-query"></a><span data-ttu-id="1f9b6-147">Steg 2: Skapa den anpassade frågan</span><span class="sxs-lookup"><span data-stu-id="1f9b6-147">Step 2: Create the Custom Query</span></span>

<span data-ttu-id="1f9b6-148">I det här steget använder vi SubscriptionId från DynamicsUsage-datauppsättningen för att skapa en anpassad fråga för den rapport som vi vill ha.</span><span class="sxs-lookup"><span data-stu-id="1f9b6-148">In this step, we will use SubscriptionId from the DynamicsUsage dataset to create a custom query for the report we want.</span></span> <span data-ttu-id="1f9b6-149">Standardtidsspanet om det inte anges i frågan är 6 månader.</span><span class="sxs-lookup"><span data-stu-id="1f9b6-149">The default timespan if not specified in the query is 6 months.</span></span>

#### <a name="request-example"></a><span data-ttu-id="1f9b6-150">Exempel på begäran</span><span class="sxs-lookup"><span data-stu-id="1f9b6-150">Request example</span></span>

```cli
curl 
--location 
--request POST 'https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledQueries' \ 
--header ' Authorization: Bearer <AADToken>' \ 
--header 'Content-Type: application/json' \ 
--data-raw 
{
  "Name": "SubscriptionId Dynamics ",
  "Description": "List of Subscription Id from DynamicsUsage",
  "Query": "SELECT SubscriptionId from DynamicsUsage "
            }"
```

#### <a name="response-example"></a><span data-ttu-id="1f9b6-151">Exempel på svar</span><span class="sxs-lookup"><span data-stu-id="1f9b6-151">Response example</span></span>

```json
{
  "value": [
    {
      "queryId": "7d19305c-56db-4edc-b776-428340e3a9c8",
      "name": "SubscriptionId Dynamics",
      "description": "List of Subscription Id from DynamicsUsage",
      "query": "SELECT SubscriptionId from DynamicsUsage",
      "type": "userDefined",
      "user": "GAUser@PITEST2.ccsctp.net",
      "createdTime": "2021-03-31T07:28:37Z"
    }
 ],
  "nextLink": null,
  "totalCount": 1,
  "message": "Query created successfully",
  "statusCode": 200,
  "dataRedacted": false
}
```

<span data-ttu-id="1f9b6-152">Vid lyckad körning av frågan `queryId` genereras en som måste användas för att generera rapporten.</span><span class="sxs-lookup"><span data-stu-id="1f9b6-152">On successful execution of the query, a `queryId` is generated that needs to be used to generate the report.</span></span>

### <a name="step-3-execute-test-query-api"></a><span data-ttu-id="1f9b6-153">Steg 3: Kör testfråge-API</span><span class="sxs-lookup"><span data-stu-id="1f9b6-153">Step 3: Execute test query API</span></span>

<span data-ttu-id="1f9b6-154">I det här steget använder vi TEST QUERY-API:et för att hämta de översta 100 raderna för frågan som skapades.</span><span class="sxs-lookup"><span data-stu-id="1f9b6-154">In this step, we will use the test query API to get the top 100 rows for the query that was created.</span></span>

#### <a name="request-example"></a><span data-ttu-id="1f9b6-155">Exempel på begäran</span><span class="sxs-lookup"><span data-stu-id="1f9b6-155">Request example</span></span>

```cli
curl 
--location 
--request GET 'https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledQueries/testQueryResult?queryId=7d19305c-56db-4edc-b776-428340e3a9c8' \
--header ' Authorization: Bearer <AADToken>'
```

#### <a name="response-example"></a><span data-ttu-id="1f9b6-156">Exempel på svar</span><span class="sxs-lookup"><span data-stu-id="1f9b6-156">Response example</span></span>

```json
{
  "value": [
    {
      "SubscriptionId": "251DE3D4-8868-4032-B518-F142DA50522F"
    },
    {
      "SubscriptionId": "758A0647-790C-435B-BEAA-652DF47E327C"
    },
    {
      "SubscriptionId": "ACE5A84B-9794-4480-82C5-AF9462DE2589"
    },
    {
      "SubscriptionId": "C75163EE-A0CA-4822-8275-E29E2490FF1C"
    },
    {
      "SubscriptionId": "082A8A18-0834-4376-A9A4-3AA4ECD02826"
    },
    .
    .
    .
    {
      "SubscriptionId": "5E10B817-7FCB-43CE-9F32-9CB60CF14658"
    },
    {
      "SubscriptionId": "7578872A-18C1-4E6B-8F51-469555337389"
    },
    {
      "SubscriptionId": "00601E10-4C05-4BA2-B977-6578F5C81D69"
    },
    {
      "SubscriptionId": "7EBFC3A9-D502-4EA2-87E7-C42971639E8C"
    },
    {
      "SubscriptionId": "2AC30AE1-5934-48FB-A0E5-EF6985761138"
    }
  ],
  "nextLink": null,
  "totalCount": 100,
  "message": null,
  "statusCode": 200,
  "dataRedacted": false
}
```

### <a name="step-4-create-the-report"></a><span data-ttu-id="1f9b6-157">Steg 4: Skapa rapporten</span><span class="sxs-lookup"><span data-stu-id="1f9b6-157">Step 4: Create the report</span></span>

<span data-ttu-id="1f9b6-158">I det här steget använder vi det tidigare genererade QueryId för att skapa rapporten.</span><span class="sxs-lookup"><span data-stu-id="1f9b6-158">In this step, we will use the previously generated QueryId to create the report.</span></span>

#### <a name="request-example"></a><span data-ttu-id="1f9b6-159">Exempel på begäran</span><span class="sxs-lookup"><span data-stu-id="1f9b6-159">Request example</span></span>

```cli
curl 
--location 
--request POST 'https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport'\
--header ' Authorization: Bearer <AADToken>' \ 
--header 'Content-Type: application/json' \ 
--data-raw 
'{
  "ReportName": "DynamicsUsage Subscription ID Report",
  "Description": "Report for getting list of Subscription Id for Dynamics Usage",
  "QueryId": "7d19305c-56db-4edc-b776-428340e3a9c8",
  "StartTime": "2021-04-01T18:41:00Z",
  "ExecuteNow": false,
  "QueryStartTime": "2021-03-31T18:41:00Z",
  "QueryEndTime": "2021-06-30T18:41:00Z",
  "RecurrenceInterval": 48,
  "RecurrenceCount": 20,
  "Format": "csv",
  "CallbackUrl": "https://<SampleCallbackUrl>",
  "CallbackMethod": "GET"
}'
```

#### <a name="response-example"></a><span data-ttu-id="1f9b6-160">Exempel på svar</span><span class="sxs-lookup"><span data-stu-id="1f9b6-160">Response example</span></span>

```json
{
  "value": [
    {
      "reportId": "cdc61cfe-d028-4333-a215-a1df51ccbfd4",
      "reportName": "DynamicsUsage Subscription ID Report",
      "description": "Report for getting list of Subscription Id for Dynamics Usage",
      "queryId": "7d19305c-56db-4edc-b776-428340e3a9c8",
      "query": "SELECT SubscriptionId from DynamicsUsage",
      "user": "GAUser@PITEST2.ccsctp.net",
      "createdTime": "2021-03-31T08:15:15Z",
      "modifiedTime": null,
      "executeNow": false,
      "startTime": "2021-04-01T18:41:00Z",
      "reportStatus": "Active",
      "recurrenceInterval": 48,
      "recurrenceCount": 20,
      "callbackUrl": "https://<SampleCallbackUrl>",
      "CallbackMethod": "GET",
      "format": "csv"
    }
  ],
  "nextLink": null,
  "totalCount": 1,
  "message": "Report created successfully",
  "statusCode": 200,
  "dataRedacted": false
}
```

<span data-ttu-id="1f9b6-161">Vid lyckad körning genereras `reportId` en som måste användas för att schemalägga en nedladdning av rapporten.</span><span class="sxs-lookup"><span data-stu-id="1f9b6-161">On successful execution, a `reportId` is generated that needs to be used to schedule a download of the report.</span></span>

### <a name="step-5-execute-report-executions-api"></a><span data-ttu-id="1f9b6-162">Steg 5: Köra API för rapportkörningar</span><span class="sxs-lookup"><span data-stu-id="1f9b6-162">Step 5: Execute Report Executions API</span></span>

<span data-ttu-id="1f9b6-163">I det här steget använder vi API:et för rapportkörningar för att hämta rapportens säkra plats (URL).</span><span class="sxs-lookup"><span data-stu-id="1f9b6-163">In this step, we will use the Report Executions API to get the secure location (URL) of the report.</span></span>

#### <a name="request-example"></a><span data-ttu-id="1f9b6-164">Exempel på begäran</span><span class="sxs-lookup"><span data-stu-id="1f9b6-164">Request example</span></span>

```cli
Curl
--location 
--request GET 'https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport/execution/ cdc61cfe-d028-4333-a215-a1df51ccbfd4?getLatestExecution=true'\
--header ' Authorization: Bearer <AADToken>' \
```

#### <a name="response-example"></a><span data-ttu-id="1f9b6-165">Exempel på svar</span><span class="sxs-lookup"><span data-stu-id="1f9b6-165">Response example</span></span>

```json
{
  "value": [
    {
      "executionId": "315eb63e-e2b2-41a2-ad8e-790b040fdce3",
      "reportId": "cdc61cfe-d028-4333-a215-a1df51ccbfd4",
      "recurrenceInterval": 48,
      "recurrenceCount": 20,
      "callbackUrl": null,
      "CallbackMethod": null,
      "format": "csv",
      "executionStatus": "Pending",
      "reportLocation": null,
      "reportAccessSecureLink": null,
      "reportExpiryTime": null,
      "reportGeneratedTime": null
    }
  ],
  "nextLink": null,
  "totalCount": 1,
  "message": null,
  "statusCode": 200,
  "dataRedacted": false
}
```

## <a name="next-steps"></a><span data-ttu-id="1f9b6-166">Nästa steg</span><span class="sxs-lookup"><span data-stu-id="1f9b6-166">Next steps</span></span>

- <span data-ttu-id="1f9b6-167">Prova API:erna via [Swagger API-URL:en](https://api.partnercenter.microsoft.com/insights/v1/mpn/swagger/index.html)</span><span class="sxs-lookup"><span data-stu-id="1f9b6-167">Try out the APIs through the [swagger API URL](https://api.partnercenter.microsoft.com/insights/v1/mpn/swagger/index.html)</span></span>