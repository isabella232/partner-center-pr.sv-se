---
title: Paradigm för programmatisk åtkomst för Insights data
description: Förstå flödet på hög nivå i API-anropsmönstret för programmatisk analys. API:erna för åtkomst till analysrapporter med partnerinsikter omfattas också.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 07/14/2021
ms.openlocfilehash: dcdd54fcc744fdb1683259203188c309a3949eff
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 07/16/2021
ms.locfileid: "114376983"
---
# <a name="programmatic-access-paradigm"></a><span data-ttu-id="febb1-104">Paradigm för programmatisk åtkomst</span><span class="sxs-lookup"><span data-stu-id="febb1-104">Programmatic access paradigm</span></span>

<span data-ttu-id="febb1-105">Det här diagrammet visar api-anropsmönstret som används för att skapa en ny rapportmall, schemalägga den anpassade rapporten och hämta feldata.</span><span class="sxs-lookup"><span data-stu-id="febb1-105">This diagram shows the API call pattern used to create a new report template, schedule the custom report and retrieve failure data.</span></span>

:::image type="content" source="images/insights/prog-acc-paradigm.png" alt-text="Flöde på hög nivå":::
<span data-ttu-id="febb1-107">***Bild 1: Flöde på hög nivå för API-anropsmönstret***</span><span class="sxs-lookup"><span data-stu-id="febb1-107">***Figure 1: High level flow of the API call pattern***</span></span>

<span data-ttu-id="febb1-108">Den här listan innehåller mer information om bild 1.</span><span class="sxs-lookup"><span data-stu-id="febb1-108">This list provides more details about Figure 1.</span></span>

1. <span data-ttu-id="febb1-109">Klientprogrammet kan definiera det anpassade rapportschemat/mallen genom att anropa API:et [Skapa rapportfråga.](#create-report-query-api)</span><span class="sxs-lookup"><span data-stu-id="febb1-109">The Client Application can define the custom report schema/template by calling the [Create Report Query API](#create-report-query-api).</span></span> <span data-ttu-id="febb1-110">Alternativt kan du välja en rapportmall (QueryId) från de exempel på rapportmallbibliotek som anges [här.](insights-programmatic-system-queries.md)</span><span class="sxs-lookup"><span data-stu-id="febb1-110">Alternately, you can pick a report template (QueryId) from the report template library samples listed [here.](insights-programmatic-system-queries.md)</span></span>
2. <span data-ttu-id="febb1-111">Om det lyckas returnerar API:et för att skapa rapportfråga QueryId.</span><span class="sxs-lookup"><span data-stu-id="febb1-111">On success, the Create Report Query API returns the QueryId.</span></span>
3. <span data-ttu-id="febb1-112">Klientprogrammet måste sedan anropa [](#create-report-api) API:et Skapa rapport med queryId tillsammans med rapportens startdatum, upprepningsintervall, upprepning och en valfri motringning-URI.</span><span class="sxs-lookup"><span data-stu-id="febb1-112">The client application then needs to call the [Create Report API](#create-report-api) using the QueryId along with the report start date, Repeat Interval, Recurrence, and an optional Callback URI.</span></span>
4. <span data-ttu-id="febb1-113">Vid Lyckad [returnerar API:et](#create-report-api) Skapa rapport ReportId.</span><span class="sxs-lookup"><span data-stu-id="febb1-113">On Success, the [Create Report API](#create-report-api) returns the ReportId.</span></span>
5. <span data-ttu-id="febb1-114">Klientprogrammet meddelas via motringning-URL:en så snart rapportdata är redo för nedladdning.</span><span class="sxs-lookup"><span data-stu-id="febb1-114">The client application gets notified at the callback URL as soon as the report data is ready for download.</span></span>
6. <span data-ttu-id="febb1-115">Klientprogrammet använder sedan API:et [Hämta rapportkörningar för](#get-report-execution-api) att fråga efter rapportens status med rapport-ID och datumintervall.</span><span class="sxs-lookup"><span data-stu-id="febb1-115">The client application then uses the [Get Report Executions API](#get-report-execution-api) to query the status of the report with the Report ID and date range.</span></span>
7. <span data-ttu-id="febb1-116">Om det lyckas returneras nedladdningslänken för rapporten och programmet kan starta nedladdningen av data.</span><span class="sxs-lookup"><span data-stu-id="febb1-116">On success, the report download link is returned and the application can initiate download of the data.</span></span>

## <a name="report-query-language-specification"></a><span data-ttu-id="febb1-117">Specifikation för rapportfrågespråk</span><span class="sxs-lookup"><span data-stu-id="febb1-117">Report query language specification</span></span>

<span data-ttu-id="febb1-118">Vi tillhandahåller [systemfrågor som du](insights-programmatic-system-queries.md) kan använda för att skapa rapporter, men du kan också skapa egna frågor baserat på dina affärsbehov.</span><span class="sxs-lookup"><span data-stu-id="febb1-118">While we do provide [system queries](insights-programmatic-system-queries.md) you can use to create reports, you can also create your own queries based on your business needs.</span></span> <span data-ttu-id="febb1-119">Mer information om anpassade frågor finns i Custom Query Specification ( [Anpassad frågespecifikation).](insights-programmatic-custom-query.md)</span><span class="sxs-lookup"><span data-stu-id="febb1-119">To learn more about custom queries, see [Custom Query Specification](insights-programmatic-custom-query.md).</span></span>

## <a name="create-report-query-api"></a><span data-ttu-id="febb1-120">Skapa API för rapportfråga</span><span class="sxs-lookup"><span data-stu-id="febb1-120">Create report query API</span></span>

<span data-ttu-id="febb1-121">API:et hjälper till att skapa anpassade frågor som definierar datauppsättningen som kolumner och mått måste exporteras från.</span><span class="sxs-lookup"><span data-stu-id="febb1-121">The API helps to create custom queries that define the dataset from which columns and metrics need to be exported.</span></span> <span data-ttu-id="febb1-122">API:et ger flexibiliteten att skapa en ny rapporteringsmall baserat på dina affärsbehov.</span><span class="sxs-lookup"><span data-stu-id="febb1-122">The API provides the flexibility to create a new reporting template based on your business needs.</span></span>  

<span data-ttu-id="febb1-123">Du kan också använda [de systemfrågor som](insights-programmatic-system-queries.md) vi tillhandahåller.</span><span class="sxs-lookup"><span data-stu-id="febb1-123">You can also use the [system queries](insights-programmatic-system-queries.md) we provide.</span></span> <span data-ttu-id="febb1-124">När anpassade rapportmallar inte behövs kan du anropa [Skapa rapport-API](#create-report-api) direkt med hjälp av QueryIds för de systemfrågor som tillhandahålls.</span><span class="sxs-lookup"><span data-stu-id="febb1-124">When custom report templates are not needed, you can call [Create Report API](#create-report-api) directly using the QueryIds of the system queries that are provided.</span></span>  

<span data-ttu-id="febb1-125">I följande exempel visas hur du skapar en anpassad fråga för att hämta de 10 främsta kunderna efter intäkter för den senaste månaden.</span><span class="sxs-lookup"><span data-stu-id="febb1-125">The following example shows how to create a custom query to get top 10 customers by revenue for last month.</span></span>

### <a name="request-syntax"></a><span data-ttu-id="febb1-126">Begärandesyntax</span><span class="sxs-lookup"><span data-stu-id="febb1-126">Request syntax</span></span>

|    <span data-ttu-id="febb1-127">Metod</span><span class="sxs-lookup"><span data-stu-id="febb1-127">Method</span></span>     |    <span data-ttu-id="febb1-128">URI för förfrågan</span><span class="sxs-lookup"><span data-stu-id="febb1-128">Request URI</span></span>     |
|----- | -----|
|    <span data-ttu-id="febb1-129">POST</span><span class="sxs-lookup"><span data-stu-id="febb1-129">POST</span></span>     |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledQueries`|
|||

### <a name="request-header"></a><span data-ttu-id="febb1-130">Begärandehuvud</span><span class="sxs-lookup"><span data-stu-id="febb1-130">Request header</span></span>

|    <span data-ttu-id="febb1-131">Huvud</span><span class="sxs-lookup"><span data-stu-id="febb1-131">Header</span></span>     |    <span data-ttu-id="febb1-132">Typ</span><span class="sxs-lookup"><span data-stu-id="febb1-132">Type</span></span>     |    <span data-ttu-id="febb1-133">Description</span><span class="sxs-lookup"><span data-stu-id="febb1-133">Description</span></span>     |
|-------|-----|------|
|    <span data-ttu-id="febb1-134">Auktorisering</span><span class="sxs-lookup"><span data-stu-id="febb1-134">Authorization</span></span>     |    <span data-ttu-id="febb1-135">sträng</span><span class="sxs-lookup"><span data-stu-id="febb1-135">string</span></span> |<span data-ttu-id="febb1-136">Krävs.</span><span class="sxs-lookup"><span data-stu-id="febb1-136">Required.</span></span> <span data-ttu-id="febb1-137">Åtkomsttoken Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="febb1-137">The Azure Active Directory (Azure AD) access token.</span></span> <span data-ttu-id="febb1-138">Formatet är  `Bearer <token>` .</span><span class="sxs-lookup"><span data-stu-id="febb1-138">The format is `Bearer <token>`.</span></span>|
|    <span data-ttu-id="febb1-139">Content-Type</span><span class="sxs-lookup"><span data-stu-id="febb1-139">Content-Type</span></span>     |<span data-ttu-id="febb1-140">sträng</span><span class="sxs-lookup"><span data-stu-id="febb1-140">string</span></span> |`Application/JSON` |
||||

### <a name="path-parameter"></a><span data-ttu-id="febb1-141">Sökvägsparameter</span><span class="sxs-lookup"><span data-stu-id="febb1-141">Path parameter</span></span>

<span data-ttu-id="febb1-142">Ingen</span><span class="sxs-lookup"><span data-stu-id="febb1-142">None</span></span>

### <a name="query-parameter"></a><span data-ttu-id="febb1-143">Frågeparameter</span><span class="sxs-lookup"><span data-stu-id="febb1-143">Query parameter</span></span>

<span data-ttu-id="febb1-144">Ingen</span><span class="sxs-lookup"><span data-stu-id="febb1-144">None</span></span>

### <a name="sample-request-payload"></a><span data-ttu-id="febb1-145">Nyttolast för exempelbegäran</span><span class="sxs-lookup"><span data-stu-id="febb1-145">Sample request payload</span></span>

```json
{ 
  "Name": "CustomersRevenueQuery", 
  "Description": "Query to get top 10 customers by revenue for last month", 
  "Query": "SELECT CustomerName, Product, BilledRevenueUSD FROM CustomersAndTenants ORDER BY BilledRevenueUSD LIMIT 10 TIMESPAN LAST_MONTH" 
}
```

### <a name="glossary"></a><span data-ttu-id="febb1-146">Ordlista</span><span class="sxs-lookup"><span data-stu-id="febb1-146">Glossary</span></span>

<span data-ttu-id="febb1-147">Den här tabellen innehåller viktiga definitioner av element i begärandenyttolasten.</span><span class="sxs-lookup"><span data-stu-id="febb1-147">This table provides the key definitions of elements in the request payload.</span></span>

|<span data-ttu-id="febb1-148">Parameter</span><span class="sxs-lookup"><span data-stu-id="febb1-148">Parameter</span></span>|    <span data-ttu-id="febb1-149">Krävs</span><span class="sxs-lookup"><span data-stu-id="febb1-149">Required</span></span>     |    <span data-ttu-id="febb1-150">Beskrivning</span><span class="sxs-lookup"><span data-stu-id="febb1-150">Description</span></span>     |    <span data-ttu-id="febb1-151">Tillåtna värden</span><span class="sxs-lookup"><span data-stu-id="febb1-151">Allowed Values</span></span>     |
|-----|    -----    |    -----    |    -----    |
|<span data-ttu-id="febb1-152">Name</span><span class="sxs-lookup"><span data-stu-id="febb1-152">Name</span></span> |    <span data-ttu-id="febb1-153">Ja</span><span class="sxs-lookup"><span data-stu-id="febb1-153">Yes</span></span>     |    <span data-ttu-id="febb1-154">Eget namn på frågan</span><span class="sxs-lookup"><span data-stu-id="febb1-154">Friendly name of the query</span></span>     |    <span data-ttu-id="febb1-155">sträng</span><span class="sxs-lookup"><span data-stu-id="febb1-155">string</span></span>     |
|    <span data-ttu-id="febb1-156">Beskrivning</span><span class="sxs-lookup"><span data-stu-id="febb1-156">Description</span></span>     |    <span data-ttu-id="febb1-157">Nej</span><span class="sxs-lookup"><span data-stu-id="febb1-157">No</span></span>     |    <span data-ttu-id="febb1-158">Beskrivning av vad frågan returnerar</span><span class="sxs-lookup"><span data-stu-id="febb1-158">Description of what the query returns</span></span>     |    <span data-ttu-id="febb1-159">sträng</span><span class="sxs-lookup"><span data-stu-id="febb1-159">string</span></span>     |
|    <span data-ttu-id="febb1-160">Söka i data</span><span class="sxs-lookup"><span data-stu-id="febb1-160">Query</span></span>     |    <span data-ttu-id="febb1-161">Ja</span><span class="sxs-lookup"><span data-stu-id="febb1-161">Yes</span></span>     |    <span data-ttu-id="febb1-162">Rapportfrågesträng</span><span class="sxs-lookup"><span data-stu-id="febb1-162">Report query string</span></span>     |    <span data-ttu-id="febb1-163">Datatyp: sträng</span><span class="sxs-lookup"><span data-stu-id="febb1-163">Data type: string</span></span> <br> <span data-ttu-id="febb1-164">[Anpassad fråga](insights-programmatic-custom-query.md) baserat på affärs behov</span><span class="sxs-lookup"><span data-stu-id="febb1-164">[Custom query](insights-programmatic-custom-query.md) based on business need</span></span> |
|        |        |        |        |

> [!Note]
> <span data-ttu-id="febb1-165">Anpassade frågeexempel finns i [Exempel på exempelfrågor.](insights-programmatic-sample-queries.md)</span><span class="sxs-lookup"><span data-stu-id="febb1-165">For custom query samples, see [Examples of sample queries.](insights-programmatic-sample-queries.md)</span></span>

### <a name="sample-response"></a><span data-ttu-id="febb1-166">Exempelsvar</span><span class="sxs-lookup"><span data-stu-id="febb1-166">Sample response</span></span>

<span data-ttu-id="febb1-167">Svarsnyttolasten är strukturerad på följande sätt:</span><span class="sxs-lookup"><span data-stu-id="febb1-167">The response payload is structured as follows:</span></span>

<span data-ttu-id="febb1-168">Svarskoder: 200, 400, 401, 403, 500</span><span class="sxs-lookup"><span data-stu-id="febb1-168">Response Codes: 200, 400, 401, 403, 500</span></span>

<span data-ttu-id="febb1-169">Exempel på nyttolast för svar:</span><span class="sxs-lookup"><span data-stu-id="febb1-169">Response payload example:</span></span>

```json
{ 
  "value": [ 
    { 
      "queryId": "ec8366a4-d96e-4194-8c37-d5dbc0639033",
      "name": "CustomersRevenueQuery",
      "description": "Query to get top 10 customers by revenue for last month",
      "query": "SELECT CustomerName, Product, BilledRevenueUSD FROM CustomersAndTenants ORDER BY BilledRevenueUSD LIMIT 10 TIMESPAN LAST_MONTH",
      "type": "userDefined",
      "user": "GAUser@PITEST2.ccsctp.net", 
      "createdTime": "2021-03-30T12:52:39Z" 
    }
  ], 
  "nextLink": null,
  "totalCount": 1,
  "message": "Query created successfully",
  "statusCode": 200,
  "dataRedacted": false
} 
```

### <a name="glossary"></a><span data-ttu-id="febb1-170">Ordlista</span><span class="sxs-lookup"><span data-stu-id="febb1-170">Glossary</span></span>

<span data-ttu-id="febb1-171">Den här tabellen innehåller viktiga definitioner av element i begärandenyttolasten.</span><span class="sxs-lookup"><span data-stu-id="febb1-171">This table provides the key definitions of elements in the request payload.</span></span>

|    <span data-ttu-id="febb1-172">Parameter</span><span class="sxs-lookup"><span data-stu-id="febb1-172">Parameter</span></span>     |    <span data-ttu-id="febb1-173">Beskrivning</span><span class="sxs-lookup"><span data-stu-id="febb1-173">Description</span></span>     |
|    ----    |    ----    |
|    <span data-ttu-id="febb1-174">QueryId</span><span class="sxs-lookup"><span data-stu-id="febb1-174">QueryId</span></span>     |    <span data-ttu-id="febb1-175">Universell unik identifierare (UUID) för den fråga som du skapade</span><span class="sxs-lookup"><span data-stu-id="febb1-175">Universally unique identifier (UUID) of the query you created</span></span>     |
|    <span data-ttu-id="febb1-176">Name</span><span class="sxs-lookup"><span data-stu-id="febb1-176">Name</span></span>     |    <span data-ttu-id="febb1-177">Eget namn som anges för frågan i nyttolasten för begäran</span><span class="sxs-lookup"><span data-stu-id="febb1-177">Friendly name given to the query in the request payload</span></span>     |
|    <span data-ttu-id="febb1-178">Description</span><span class="sxs-lookup"><span data-stu-id="febb1-178">Description</span></span>     |    <span data-ttu-id="febb1-179">Beskrivning som ges när frågan skapas</span><span class="sxs-lookup"><span data-stu-id="febb1-179">Description given during creation of the query</span></span>     |
|    <span data-ttu-id="febb1-180">Söka i data</span><span class="sxs-lookup"><span data-stu-id="febb1-180">Query</span></span>     |    <span data-ttu-id="febb1-181">Rapportfråga som skickas som indata när frågan skapas</span><span class="sxs-lookup"><span data-stu-id="febb1-181">Report query passed as input during query creation</span></span>     |
|    <span data-ttu-id="febb1-182">Typ</span><span class="sxs-lookup"><span data-stu-id="febb1-182">Type</span></span>     |    <span data-ttu-id="febb1-183">Ange till `userDefined`</span><span class="sxs-lookup"><span data-stu-id="febb1-183">Set to `userDefined`</span></span>     |
|    <span data-ttu-id="febb1-184">Användare</span><span class="sxs-lookup"><span data-stu-id="febb1-184">User</span></span>     |    <span data-ttu-id="febb1-185">Användar-ID som användes för att skapa frågan</span><span class="sxs-lookup"><span data-stu-id="febb1-185">User ID used to create of the query</span></span>     |
|    <span data-ttu-id="febb1-186">CreatedTime</span><span class="sxs-lookup"><span data-stu-id="febb1-186">CreatedTime</span></span>     |    <span data-ttu-id="febb1-187">UTC-tid då frågan skapades i det här formatet: yyyy-MM-ddTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="febb1-187">UTC Time the query was created in this format: yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="febb1-188">TotalCount</span><span class="sxs-lookup"><span data-stu-id="febb1-188">TotalCount</span></span>     |    <span data-ttu-id="febb1-189">Antal datauppsättningar i värdematrisen</span><span class="sxs-lookup"><span data-stu-id="febb1-189">Number of datasets in the Value array</span></span>     |
|    <span data-ttu-id="febb1-190">StatusCode</span><span class="sxs-lookup"><span data-stu-id="febb1-190">StatusCode</span></span>     |    <span data-ttu-id="febb1-191">Resultatkod</span><span class="sxs-lookup"><span data-stu-id="febb1-191">Result Code</span></span> <br> <span data-ttu-id="febb1-192">Möjliga värden är 200, 400, 401, 403, 500</span><span class="sxs-lookup"><span data-stu-id="febb1-192">The possible values are 200, 400, 401, 403, 500</span></span>     |
|    <span data-ttu-id="febb1-193">meddelande</span><span class="sxs-lookup"><span data-stu-id="febb1-193">message</span></span>     |    <span data-ttu-id="febb1-194">Statusmeddelande från körningen av API:et</span><span class="sxs-lookup"><span data-stu-id="febb1-194">Status message from the execution of the API</span></span>     |
|        |        |

## <a name="create-report-api"></a><span data-ttu-id="febb1-195">Skapa rapport-API</span><span class="sxs-lookup"><span data-stu-id="febb1-195">Create report API</span></span>

<span data-ttu-id="febb1-196">När du skapar en anpassad rapportmall och [](#create-report-query-api) tar emot QueryID som en del av svaret från Skapa rapportfråga kan det här API:et anropas för att schemalägga en fråga som ska köras med jämna mellanrum.</span><span class="sxs-lookup"><span data-stu-id="febb1-196">On creating a custom report template successfully and receiving the QueryID as part of [Create Report Query](#create-report-query-api) response, this API can be called to schedule a query to be executed at regular intervals.</span></span> <span data-ttu-id="febb1-197">Du kan ange en frekvens och ett schema för rapporten som ska levereras.</span><span class="sxs-lookup"><span data-stu-id="febb1-197">You can set a frequency and schedule for the report to be delivered.</span></span>
<span data-ttu-id="febb1-198">För systemfrågor som vi tillhandahåller kan API:et Skapa rapport också anropas med [QueryId.](insights-programmatic-system-queries.md)</span><span class="sxs-lookup"><span data-stu-id="febb1-198">For system queries we provide, the Create Report API can also be called with [QueryId](insights-programmatic-system-queries.md).</span></span>

### <a name="callback-url"></a><span data-ttu-id="febb1-199">Callback URL (Webbadress för återanrop)</span><span class="sxs-lookup"><span data-stu-id="febb1-199">Callback URL</span></span>

<span data-ttu-id="febb1-200">API:et för att skapa rapport accepterar en återanrops-URL.</span><span class="sxs-lookup"><span data-stu-id="febb1-200">The create report API accepts a callback URL.</span></span> <span data-ttu-id="febb1-201">Den här URL:en anropas när rapportgenereringen har lyckats.</span><span class="sxs-lookup"><span data-stu-id="febb1-201">This URL will be called once the report generation is successful.</span></span> <span data-ttu-id="febb1-202">Motringning-URL:en ska vara offentligt åtkomlig.</span><span class="sxs-lookup"><span data-stu-id="febb1-202">The callback URL should be publicly reachable.</span></span> <span data-ttu-id="febb1-203">Förutom URL:en kan en motringningsmetod också anges.</span><span class="sxs-lookup"><span data-stu-id="febb1-203">In addition to the URL a callback method can also be given.</span></span> <span data-ttu-id="febb1-204">Motringningsmetoden kan bara vara "GET" eller "POST".</span><span class="sxs-lookup"><span data-stu-id="febb1-204">The callback method can only be "GET" or "POST".</span></span> <span data-ttu-id="febb1-205">Standardmetoden om inget värde skickas blir "POST".</span><span class="sxs-lookup"><span data-stu-id="febb1-205">The default method if no value is passed will be "POST".</span></span> <span data-ttu-id="febb1-206">Det reportId som har slutfört genereringen skickas alltid tillbaka under återanropet.</span><span class="sxs-lookup"><span data-stu-id="febb1-206">The reportId that has completed generation will always be passed back during the callback.</span></span>

<span data-ttu-id="febb1-207">POST-återanrop: Om url:en som skickades var `https://www.contosso.com/callback` kommer den anropade bakåt-URL:en att vara `https://www.contosso.com/callback/<reportID>`</span><span class="sxs-lookup"><span data-stu-id="febb1-207">POST callback: If the URL passed was `https://www.contosso.com/callback`, then the called back URL will be `https://www.contosso.com/callback/<reportID>`</span></span> 

<span data-ttu-id="febb1-208">GET-återanrop: Om url:en som skickades var `https://www.contosso.com/callback` kommer den anropade url:en att bli `https://www.contosso.com/callback?reportId=<reportID>`</span><span class="sxs-lookup"><span data-stu-id="febb1-208">GET callback: If the URL passed was `https://www.contosso.com/callback`, then the called back URL will be `https://www.contosso.com/callback?reportId=<reportID>`</span></span> 

### <a name="executenow-reports"></a><span data-ttu-id="febb1-209">ExecuteNow-rapporter</span><span class="sxs-lookup"><span data-stu-id="febb1-209">ExecuteNow reports</span></span>

<span data-ttu-id="febb1-210">Det finns en etablering för att generera en rapport utan schemaläggning.</span><span class="sxs-lookup"><span data-stu-id="febb1-210">There is a provision to generate a report without scheduling.</span></span> <span data-ttu-id="febb1-211">API-nyttolasten för att skapa rapport kan acceptera en parameter , som kommer att lägga rapporten i en sekvens som ska genereras `ExecuteNow` så snart API:et anropas.</span><span class="sxs-lookup"><span data-stu-id="febb1-211">The report create API payload can accept a parameter `ExecuteNow`, which will enqueue the report to be generated as soon as the API is called.</span></span> <span data-ttu-id="febb1-212">När `ExecuteNow` är inställt på true ignoreras fälten: `StartTime` , eftersom dessa rapporter inte `RecurrenceCount` `RecurrenceInterval` schemaläggs.</span><span class="sxs-lookup"><span data-stu-id="febb1-212">When `ExecuteNow` is set to true, the fields: `StartTime`, `RecurrenceCount`, `RecurrenceInterval` are ignored as these reports are not scheduled.</span></span>

<span data-ttu-id="febb1-213">Två ytterligare fält kan skickas när `ExecuteNow` är sant, `QueryStartTime` och `QueryEndTime` .</span><span class="sxs-lookup"><span data-stu-id="febb1-213">Two additional fields can be passed when `ExecuteNow` is true, `QueryStartTime` and `QueryEndTime`.</span></span> <span data-ttu-id="febb1-214">De här två fälten `TIMESPAN` åsidosätter fältet i frågan.</span><span class="sxs-lookup"><span data-stu-id="febb1-214">These two fields will override the `TIMESPAN` field in the query.</span></span> <span data-ttu-id="febb1-215">De här fälten gäller inte för schemalagda rapporter eftersom data genereras kontinuerligt under en fast tidsperiod som inte ändras.</span><span class="sxs-lookup"><span data-stu-id="febb1-215">These fields are not applicable for scheduled reports as data will get continuously generated for a fixed time period that does not change.</span></span>

### <a name="request-syntax"></a><span data-ttu-id="febb1-216">Begärandesyntax</span><span class="sxs-lookup"><span data-stu-id="febb1-216">Request syntax</span></span>

|    <span data-ttu-id="febb1-217">Metod</span><span class="sxs-lookup"><span data-stu-id="febb1-217">Method</span></span>     |    <span data-ttu-id="febb1-218">URI för förfrågan</span><span class="sxs-lookup"><span data-stu-id="febb1-218">Request URI</span></span>     |
|----- | -----|
|    <span data-ttu-id="febb1-219">POST</span><span class="sxs-lookup"><span data-stu-id="febb1-219">POST</span></span>     |`https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport` |

### <a name="request-header"></a><span data-ttu-id="febb1-220">Begärandehuvud</span><span class="sxs-lookup"><span data-stu-id="febb1-220">Request header</span></span>

|    <span data-ttu-id="febb1-221">Huvud</span><span class="sxs-lookup"><span data-stu-id="febb1-221">Header</span></span>     |    <span data-ttu-id="febb1-222">Typ</span><span class="sxs-lookup"><span data-stu-id="febb1-222">Type</span></span>     |    <span data-ttu-id="febb1-223">Description</span><span class="sxs-lookup"><span data-stu-id="febb1-223">Description</span></span>     |
|-------|-----|------|
|    <span data-ttu-id="febb1-224">Auktorisering</span><span class="sxs-lookup"><span data-stu-id="febb1-224">Authorization</span></span>     |    <span data-ttu-id="febb1-225">sträng</span><span class="sxs-lookup"><span data-stu-id="febb1-225">string</span></span> |<span data-ttu-id="febb1-226">Krävs.</span><span class="sxs-lookup"><span data-stu-id="febb1-226">Required.</span></span> <span data-ttu-id="febb1-227">Åtkomsttoken Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="febb1-227">The Azure Active Directory (Azure AD) access token.</span></span> <span data-ttu-id="febb1-228">Formatet är  `Bearer <token>` .</span><span class="sxs-lookup"><span data-stu-id="febb1-228">The format is `Bearer <token>`.</span></span>|
|    <span data-ttu-id="febb1-229">Content-Type</span><span class="sxs-lookup"><span data-stu-id="febb1-229">Content-Type</span></span>     |<span data-ttu-id="febb1-230">sträng</span><span class="sxs-lookup"><span data-stu-id="febb1-230">string</span></span> |`Application/JSON` |

### <a name="path-parameter"></a><span data-ttu-id="febb1-231">Sökvägsparameter</span><span class="sxs-lookup"><span data-stu-id="febb1-231">Path Parameter</span></span>

<span data-ttu-id="febb1-232">Ingen</span><span class="sxs-lookup"><span data-stu-id="febb1-232">None</span></span>

### <a name="query-parameter"></a><span data-ttu-id="febb1-233">Frågeparameter</span><span class="sxs-lookup"><span data-stu-id="febb1-233">Query Parameter</span></span>

<span data-ttu-id="febb1-234">Ingen</span><span class="sxs-lookup"><span data-stu-id="febb1-234">None</span></span>

### <a name="sample-request-payload"></a><span data-ttu-id="febb1-235">Nyttolast för exempelbegäran</span><span class="sxs-lookup"><span data-stu-id="febb1-235">Sample request payload</span></span>

```json
{
  "ReportName": "Top10_CustomersReport",
  "Description": "Top 10 customers by revenue for last month",
  "QueryId": "ec8366a4-d96e-4194-8c37-d5dbc0639033",
  "StartTime": "2021-03-31T18:41:00Z",
  "ExecuteNow": false,
  "QueryStartTime": null,
  "QueryEndTime": null,
  "RecurrenceInterval": 24,
  "RecurrenceCount": 100,
  "Format": "CSV",
  "CallbackUrl": "https://<SampleCallbackUrl>",
  "CallbackMethod": "GET"
}
```

### <a name="glossary"></a><span data-ttu-id="febb1-236">Ordlista</span><span class="sxs-lookup"><span data-stu-id="febb1-236">Glossary</span></span>

<span data-ttu-id="febb1-237">Viktiga definitioner av elementen i nyttolasten för begäran förklaras nedan:</span><span class="sxs-lookup"><span data-stu-id="febb1-237">Key definitions of elements in the request payload are articulated below:</span></span>

|    <span data-ttu-id="febb1-238">Parameter</span><span class="sxs-lookup"><span data-stu-id="febb1-238">Parameter</span></span>     |    <span data-ttu-id="febb1-239">Krävs</span><span class="sxs-lookup"><span data-stu-id="febb1-239">Required</span></span>     |    <span data-ttu-id="febb1-240">Beskrivning</span><span class="sxs-lookup"><span data-stu-id="febb1-240">Description</span></span>     |    <span data-ttu-id="febb1-241">Tillåtna värden</span><span class="sxs-lookup"><span data-stu-id="febb1-241">Allowed Values</span></span>     |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="febb1-242">ReportName</span><span class="sxs-lookup"><span data-stu-id="febb1-242">ReportName</span></span>     |    <span data-ttu-id="febb1-243">Ja</span><span class="sxs-lookup"><span data-stu-id="febb1-243">Yes</span></span>     |    <span data-ttu-id="febb1-244">Namn som ska tilldelas till rapporten</span><span class="sxs-lookup"><span data-stu-id="febb1-244">Name to be assigned to the report</span></span>     |    <span data-ttu-id="febb1-245">sträng</span><span class="sxs-lookup"><span data-stu-id="febb1-245">string</span></span>     |
|    <span data-ttu-id="febb1-246">Beskrivning</span><span class="sxs-lookup"><span data-stu-id="febb1-246">Description</span></span>     |    <span data-ttu-id="febb1-247">Nej</span><span class="sxs-lookup"><span data-stu-id="febb1-247">No</span></span>     |    <span data-ttu-id="febb1-248">Beskrivning av den skapade rapporten</span><span class="sxs-lookup"><span data-stu-id="febb1-248">Description of the created report</span></span>     |    <span data-ttu-id="febb1-249">sträng</span><span class="sxs-lookup"><span data-stu-id="febb1-249">string</span></span>     |
|    <span data-ttu-id="febb1-250">QueryId</span><span class="sxs-lookup"><span data-stu-id="febb1-250">QueryId</span></span>     |    <span data-ttu-id="febb1-251">Ja</span><span class="sxs-lookup"><span data-stu-id="febb1-251">Yes</span></span>     |    <span data-ttu-id="febb1-252">Rapportfråge-ID</span><span class="sxs-lookup"><span data-stu-id="febb1-252">Report query ID</span></span>     |    <span data-ttu-id="febb1-253">sträng</span><span class="sxs-lookup"><span data-stu-id="febb1-253">string</span></span>     |
|    <span data-ttu-id="febb1-254">StartTime</span><span class="sxs-lookup"><span data-stu-id="febb1-254">StartTime</span></span>     |    <span data-ttu-id="febb1-255">Ja</span><span class="sxs-lookup"><span data-stu-id="febb1-255">Yes</span></span>     |    <span data-ttu-id="febb1-256">UTC-tidsstämpel där rapportgenereringen ska börja.</span><span class="sxs-lookup"><span data-stu-id="febb1-256">UTC Timestamp at which the report generation will begin.</span></span> <br> <span data-ttu-id="febb1-257">Formatet ska vara: yyyy-MM-ddTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="febb1-257">The format should be: yyyy-MM-ddTHH:mm:ssZ</span></span>       |    <span data-ttu-id="febb1-258">sträng</span><span class="sxs-lookup"><span data-stu-id="febb1-258">string</span></span>     |
|    <span data-ttu-id="febb1-259">ExecuteNow</span><span class="sxs-lookup"><span data-stu-id="febb1-259">ExecuteNow</span></span>     |    <span data-ttu-id="febb1-260">Inga</span><span class="sxs-lookup"><span data-stu-id="febb1-260">No</span></span>     |    <span data-ttu-id="febb1-261">Den här parametern ska användas för att skapa en rapport som bara ska köras en gång.</span><span class="sxs-lookup"><span data-stu-id="febb1-261">This parameter should be used to create a report that will be executed only once.</span></span> <span data-ttu-id="febb1-262">`StartTime`och `RecurrenceInterval` `RecurrenceCount` ignoreras om detta är inställt på true.</span><span class="sxs-lookup"><span data-stu-id="febb1-262">`StartTime`, `RecurrenceInterval` and `RecurrenceCount` are ignored if this is set to true.</span></span> <span data-ttu-id="febb1-263">Rapporten körs omedelbart på ett asynkront sätt</span><span class="sxs-lookup"><span data-stu-id="febb1-263">The report is executed immediately in an asynchronous fashion</span></span>     |    <span data-ttu-id="febb1-264">sant/falskt</span><span class="sxs-lookup"><span data-stu-id="febb1-264">true/false</span></span>     |
|    <span data-ttu-id="febb1-265">QueryStartTime</span><span class="sxs-lookup"><span data-stu-id="febb1-265">QueryStartTime</span></span>     |    <span data-ttu-id="febb1-266">Inga</span><span class="sxs-lookup"><span data-stu-id="febb1-266">No</span></span>     |    <span data-ttu-id="febb1-267">Du kan också ange starttiden för frågan som extraherar data.</span><span class="sxs-lookup"><span data-stu-id="febb1-267">Optionally specifies the start time for the query extracting the data.</span></span> <span data-ttu-id="febb1-268">Den här parametern gäller endast för en körningsrapport som har `ExecuteNow` angetts till true.</span><span class="sxs-lookup"><span data-stu-id="febb1-268">This parameter is applicable only for one time execution report that have `ExecuteNow` set to true.</span></span> <span data-ttu-id="febb1-269">Ange åsidosättningar för den `TIMESPAN` här parametern som anges i frågan.</span><span class="sxs-lookup"><span data-stu-id="febb1-269">Setting this parameter overrides `TIMESPAN` given in the query.</span></span> <span data-ttu-id="febb1-270">Formatet ska vara yyyy-MM-ddTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="febb1-270">The format should be yyyy-MM-ddTHH:mm:ssZ</span></span>     |    <span data-ttu-id="febb1-271">Tidsstämpel som sträng</span><span class="sxs-lookup"><span data-stu-id="febb1-271">Timestamp as string</span></span>     |
|    <span data-ttu-id="febb1-272">QueryEndTime</span><span class="sxs-lookup"><span data-stu-id="febb1-272">QueryEndTime</span></span>     |    <span data-ttu-id="febb1-273">Inga</span><span class="sxs-lookup"><span data-stu-id="febb1-273">No</span></span>     |    <span data-ttu-id="febb1-274">Du kan också ange sluttiden för frågan som extraherar data.</span><span class="sxs-lookup"><span data-stu-id="febb1-274">Optionally specifies the end time for the query extracting the data.</span></span> <span data-ttu-id="febb1-275">Den här parametern gäller endast för en körningsrapport som har `ExecuteNow` angetts till true.</span><span class="sxs-lookup"><span data-stu-id="febb1-275">This parameter is applicable only for one time execution report that have `ExecuteNow` set to true.</span></span> <span data-ttu-id="febb1-276">Ange åsidosättningar för den `TIMESPAN` här parametern som anges i frågan.</span><span class="sxs-lookup"><span data-stu-id="febb1-276">Setting this parameter overrides `TIMESPAN` given in the query.</span></span> <span data-ttu-id="febb1-277">Formatet ska vara yyyy-MM-ddTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="febb1-277">The format should be yyyy-MM-ddTHH:mm:ssZ</span></span>     |    <span data-ttu-id="febb1-278">Tidsstämpel som sträng</span><span class="sxs-lookup"><span data-stu-id="febb1-278">Timestamp as string</span></span>     |
|    <span data-ttu-id="febb1-279">RecurrenceInterval</span><span class="sxs-lookup"><span data-stu-id="febb1-279">RecurrenceInterval</span></span>     |    <span data-ttu-id="febb1-280">Ja</span><span class="sxs-lookup"><span data-stu-id="febb1-280">Yes</span></span>     |    <span data-ttu-id="febb1-281">Frekvens i timmar då rapporten ska genereras.</span><span class="sxs-lookup"><span data-stu-id="febb1-281">Frequency in hours at which the report should be generated.</span></span> <br> <span data-ttu-id="febb1-282">Minimivärdet är 4 och Det högsta värdet är 2160.</span><span class="sxs-lookup"><span data-stu-id="febb1-282">Minimum value is 4 and Maximum value is 2160.</span></span>      |    <span data-ttu-id="febb1-283">heltal</span><span class="sxs-lookup"><span data-stu-id="febb1-283">integer</span></span>     |
|    <span data-ttu-id="febb1-284">RecurrenceCount</span><span class="sxs-lookup"><span data-stu-id="febb1-284">RecurrenceCount</span></span>     |    <span data-ttu-id="febb1-285">Inga</span><span class="sxs-lookup"><span data-stu-id="febb1-285">No</span></span>     |    <span data-ttu-id="febb1-286">Antal rapporter som ska genereras.</span><span class="sxs-lookup"><span data-stu-id="febb1-286">Number of reports to be generated.</span></span>     |    <span data-ttu-id="febb1-287">heltal</span><span class="sxs-lookup"><span data-stu-id="febb1-287">integer</span></span>     |
|    <span data-ttu-id="febb1-288">Format</span><span class="sxs-lookup"><span data-stu-id="febb1-288">Format</span></span>     |    <span data-ttu-id="febb1-289">Inga</span><span class="sxs-lookup"><span data-stu-id="febb1-289">No</span></span>     |    <span data-ttu-id="febb1-290">Filformat för den exporterade filen.</span><span class="sxs-lookup"><span data-stu-id="febb1-290">File format of the exported file.</span></span> <br> <span data-ttu-id="febb1-291">Standardvärdet är CSV.</span><span class="sxs-lookup"><span data-stu-id="febb1-291">Default is CSV.</span></span>    |    <span data-ttu-id="febb1-292">"CSV"/"TSV"</span><span class="sxs-lookup"><span data-stu-id="febb1-292">"CSV"/"TSV"</span></span>     |
|    <span data-ttu-id="febb1-293">CallbackUrl</span><span class="sxs-lookup"><span data-stu-id="febb1-293">CallbackUrl</span></span>     |    <span data-ttu-id="febb1-294">Inga</span><span class="sxs-lookup"><span data-stu-id="febb1-294">No</span></span>     |    <span data-ttu-id="febb1-295">Offentligt nåbar URL som kan konfigureras som återanropsmål</span><span class="sxs-lookup"><span data-stu-id="febb1-295">Publicly reachable URL that can be optionally configured as callback destination</span></span>     |    <span data-ttu-id="febb1-296">Sträng (http-URL)</span><span class="sxs-lookup"><span data-stu-id="febb1-296">String (http URL)</span></span>     |
|    <span data-ttu-id="febb1-297">CallbackMethod</span><span class="sxs-lookup"><span data-stu-id="febb1-297">CallbackMethod</span></span>     |    <span data-ttu-id="febb1-298">Inga</span><span class="sxs-lookup"><span data-stu-id="febb1-298">No</span></span>     |    <span data-ttu-id="febb1-299">Metoden som ska användas för återanrop</span><span class="sxs-lookup"><span data-stu-id="febb1-299">The method to be used for callback</span></span>     |    <span data-ttu-id="febb1-300">GET/POST</span><span class="sxs-lookup"><span data-stu-id="febb1-300">GET/POST</span></span>     |
|        |        |        |        |

### <a name="sample-response"></a><span data-ttu-id="febb1-301">Exempelsvar</span><span class="sxs-lookup"><span data-stu-id="febb1-301">Sample response</span></span>

<span data-ttu-id="febb1-302">Svarsnyttolasten är strukturerad på följande sätt:</span><span class="sxs-lookup"><span data-stu-id="febb1-302">The response payload is structured as follows:</span></span>

<span data-ttu-id="febb1-303">Svarskoder: 200, 400, 401, 403, 404, 500</span><span class="sxs-lookup"><span data-stu-id="febb1-303">Response Codes: 200, 400, 401, 403, 404, 500</span></span>

<span data-ttu-id="febb1-304">Exempel på nyttolast för svar:</span><span class="sxs-lookup"><span data-stu-id="febb1-304">Response payload example:</span></span>

```json
{ 
  "value": [
    { 
      "reportId": "d9548477-16d4-492a-bf9c-0cf91a9f69bf", 
      "reportName": "Top10_CustomersReport", 
      "description": "Top 10 customers by revenue for last month", 
      "queryId": "ec8366a4-d96e-4194-8c37-d5dbc0639033", 
      "query": "SELECT CustomerName, Product, BilledRevenueUSD FROM CustomersAndTenants ORDER BY BilledRevenueUSD LIMIT 10 TIMESPAN LAST_MONTH", 
      "user": "GAUser@PITEST2.ccsctp.net", 
      "createdTime": "2021-03-30T13:11:58Z", 
      "modifiedTime": null, 
      "executeNow": false, 
      "startTime": "2021-03-31T18:41:00Z", 
      "reportStatus": "Active", 
      "recurrenceInterval": 24, 
      "recurrenceCount": 100, 
      "callbackUrl": "https://<SampleCallbackUrl>", 
      "callbackMethod": "GET", 
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

### <a name="glossary"></a><span data-ttu-id="febb1-305">Ordlista</span><span class="sxs-lookup"><span data-stu-id="febb1-305">Glossary</span></span>

<span data-ttu-id="febb1-306">Viktiga definitioner av element i svaret förklaras nedan:</span><span class="sxs-lookup"><span data-stu-id="febb1-306">Key definitions of elements in the response are articulated below:</span></span>

|    <span data-ttu-id="febb1-307">Parameter</span><span class="sxs-lookup"><span data-stu-id="febb1-307">Parameter</span></span>     |    <span data-ttu-id="febb1-308">Beskrivning</span><span class="sxs-lookup"><span data-stu-id="febb1-308">Description</span></span>     |
|    ----    |    ----    |
|    <span data-ttu-id="febb1-309">ReportId</span><span class="sxs-lookup"><span data-stu-id="febb1-309">ReportId</span></span>     |    <span data-ttu-id="febb1-310">Universell unik identifierare (UUID) för den rapport som du skapade</span><span class="sxs-lookup"><span data-stu-id="febb1-310">Universally unique identifier (UUID) of the report you created</span></span>     |
|    <span data-ttu-id="febb1-311">ReportName</span><span class="sxs-lookup"><span data-stu-id="febb1-311">ReportName</span></span>     |    <span data-ttu-id="febb1-312">Namn som ges till rapporten i nyttolasten för begäran</span><span class="sxs-lookup"><span data-stu-id="febb1-312">Name given to the report in the request payload</span></span>     |
|    <span data-ttu-id="febb1-313">Description</span><span class="sxs-lookup"><span data-stu-id="febb1-313">Description</span></span>     |    <span data-ttu-id="febb1-314">Beskrivning som anges när rapporten skapas</span><span class="sxs-lookup"><span data-stu-id="febb1-314">Description given during creation of the report</span></span>     |
|    <span data-ttu-id="febb1-315">QueryId</span><span class="sxs-lookup"><span data-stu-id="febb1-315">QueryId</span></span>     |    <span data-ttu-id="febb1-316">Fråge-ID som skickades när du skapade rapporten</span><span class="sxs-lookup"><span data-stu-id="febb1-316">Query ID passed at the time you created the report</span></span>     |
|    <span data-ttu-id="febb1-317">Söka i data</span><span class="sxs-lookup"><span data-stu-id="febb1-317">Query</span></span>     |    <span data-ttu-id="febb1-318">Frågetext som ska köras för den här rapporten</span><span class="sxs-lookup"><span data-stu-id="febb1-318">Query text that will be executed for this report</span></span>     |
|    <span data-ttu-id="febb1-319">Användare</span><span class="sxs-lookup"><span data-stu-id="febb1-319">User</span></span>     |    <span data-ttu-id="febb1-320">Användar-ID som används för att skapa rapporten</span><span class="sxs-lookup"><span data-stu-id="febb1-320">User ID used to create the report</span></span>     |
|    <span data-ttu-id="febb1-321">CreatedTime</span><span class="sxs-lookup"><span data-stu-id="febb1-321">CreatedTime</span></span>     |    <span data-ttu-id="febb1-322">UTC-tid då rapporten skapades i det här formatet: yyyy-MM-ddTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="febb1-322">UTC Time the report was created in this format: yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="febb1-323">ModifiedTime</span><span class="sxs-lookup"><span data-stu-id="febb1-323">ModifiedTime</span></span>     |    <span data-ttu-id="febb1-324">UTC-tid då rapporten senast ändrades i det här formatet: yyyy-MM-ddTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="febb1-324">UTC Time the report was last modified in this format: yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="febb1-325">ExecuteNow</span><span class="sxs-lookup"><span data-stu-id="febb1-325">ExecuteNow</span></span>     |    <span data-ttu-id="febb1-326">`ExecuteNow` flagga som angetts när rapporten skapades</span><span class="sxs-lookup"><span data-stu-id="febb1-326">`ExecuteNow` flag set at the time the report was created</span></span>     |
|    <span data-ttu-id="febb1-327">StartTime</span><span class="sxs-lookup"><span data-stu-id="febb1-327">StartTime</span></span>     |    <span data-ttu-id="febb1-328">UTC-tid då rapportkörningen börjar i det här formatet: yyyy-MM-ddTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="febb1-328">UTC Time the report execution will begin in this format: yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="febb1-329">ReportStatus</span><span class="sxs-lookup"><span data-stu-id="febb1-329">ReportStatus</span></span>     |    <span data-ttu-id="febb1-330">Status för rapportkörningen.</span><span class="sxs-lookup"><span data-stu-id="febb1-330">Status of the report execution.</span></span> <span data-ttu-id="febb1-331">Möjliga värden är `Paused` , `Active` och `Inactive`</span><span class="sxs-lookup"><span data-stu-id="febb1-331">The possible values are `Paused`, `Active`, and `Inactive`</span></span>     |
|    <span data-ttu-id="febb1-332">RecurrenceInterval</span><span class="sxs-lookup"><span data-stu-id="febb1-332">RecurrenceInterval</span></span>     |    <span data-ttu-id="febb1-333">Upprepningsintervall som anges när rapporten skapas</span><span class="sxs-lookup"><span data-stu-id="febb1-333">Recurrence interval provided during report creation</span></span>     |
|    <span data-ttu-id="febb1-334">RecurrenceCount</span><span class="sxs-lookup"><span data-stu-id="febb1-334">RecurrenceCount</span></span>     |    <span data-ttu-id="febb1-335">Upprepningsantal som anges när rapporten skapas.</span><span class="sxs-lookup"><span data-stu-id="febb1-335">Recurrence count provided during report creation.</span></span>      |
|    <span data-ttu-id="febb1-336">CallbackUrl</span><span class="sxs-lookup"><span data-stu-id="febb1-336">CallbackUrl</span></span>     |    <span data-ttu-id="febb1-337">Motringning-URL som anges i begäran</span><span class="sxs-lookup"><span data-stu-id="febb1-337">Callback URL provided in the request</span></span>     |
|    <span data-ttu-id="febb1-338">CallbackMethod</span><span class="sxs-lookup"><span data-stu-id="febb1-338">CallbackMethod</span></span>     |    <span data-ttu-id="febb1-339">Återanropsmetod som anges i begäran</span><span class="sxs-lookup"><span data-stu-id="febb1-339">Callback method provided in the request</span></span>     |
|    <span data-ttu-id="febb1-340">Format</span><span class="sxs-lookup"><span data-stu-id="febb1-340">Format</span></span>     |    <span data-ttu-id="febb1-341">Format för rapportfilerna.</span><span class="sxs-lookup"><span data-stu-id="febb1-341">Format of the report files.</span></span> <span data-ttu-id="febb1-342">Möjliga värden är `CSV` eller `TSV` .</span><span class="sxs-lookup"><span data-stu-id="febb1-342">The possible values are `CSV` or `TSV`.</span></span>     |
|    <span data-ttu-id="febb1-343">TotalCount</span><span class="sxs-lookup"><span data-stu-id="febb1-343">TotalCount</span></span>     |    <span data-ttu-id="febb1-344">Antal poster i värdematrisen</span><span class="sxs-lookup"><span data-stu-id="febb1-344">Number of records in the Value array</span></span>     |
|    <span data-ttu-id="febb1-345">StatusCode</span><span class="sxs-lookup"><span data-stu-id="febb1-345">StatusCode</span></span>     |    <span data-ttu-id="febb1-346">Resultatkod</span><span class="sxs-lookup"><span data-stu-id="febb1-346">Result Code</span></span>     |
|    <span data-ttu-id="febb1-347">meddelande</span><span class="sxs-lookup"><span data-stu-id="febb1-347">message</span></span>     |    <span data-ttu-id="febb1-348">Möjliga värden är 200, 400, 401, 403, 500.</span><span class="sxs-lookup"><span data-stu-id="febb1-348">The possible values are 200, 400, 401, 403, 500.</span></span> <span data-ttu-id="febb1-349">Statusmeddelande från körningen av API:et</span><span class="sxs-lookup"><span data-stu-id="febb1-349">Status message from the execution of the API</span></span>     |
|        |        |

## <a name="get-report-execution-api"></a><span data-ttu-id="febb1-350">Hämta API för rapportkörning</span><span class="sxs-lookup"><span data-stu-id="febb1-350">Get report execution API</span></span>

<span data-ttu-id="febb1-351">Du kan använda den här metoden för att fråga efter status för en rapportkörning med hjälp av ReportId som togs emot från [API:et För att skapa rapport.](#create-report-api)</span><span class="sxs-lookup"><span data-stu-id="febb1-351">You can use this method to query the status of a report execution using the ReportId received from [Create Report API](#create-report-api).</span></span> <span data-ttu-id="febb1-352">Metoden returnerar nedladdningslänken för rapporten om rapporten är redo för nedladdning.</span><span class="sxs-lookup"><span data-stu-id="febb1-352">The method returns the report download link if the report is ready for download.</span></span> <span data-ttu-id="febb1-353">Annars returnerar metoden statusen.</span><span class="sxs-lookup"><span data-stu-id="febb1-353">Otherwise, the method returns the status.</span></span> <span data-ttu-id="febb1-354">Du kan också använda det här API:et för att hämta alla körningar som har inträffat för en viss rapport.</span><span class="sxs-lookup"><span data-stu-id="febb1-354">You can also use this API to get all the executions that have happened for a given report.</span></span>  

>[!IMPORTANT]
><span data-ttu-id="febb1-355">Det här API:et har standardfrågeparametrar för `executionStatus=Completed` och `getLatestExecution=true` .</span><span class="sxs-lookup"><span data-stu-id="febb1-355">This API has default query parameters set for `executionStatus=Completed` and `getLatestExecution=true`.</span></span> <span data-ttu-id="febb1-356">Om API:et anropas innan den första lyckade körningen av rapporten returneras därför 404.</span><span class="sxs-lookup"><span data-stu-id="febb1-356">Hence, calling the API before the first successful execution of the report will return 404.</span></span> <span data-ttu-id="febb1-357">Väntande körningar kan hämtas genom att ange `executionStatus=Pending` .</span><span class="sxs-lookup"><span data-stu-id="febb1-357">Pending executions can be obtained by setting `executionStatus=Pending`.</span></span>

### <a name="request-syntax"></a><span data-ttu-id="febb1-358">Begärandesyntax</span><span class="sxs-lookup"><span data-stu-id="febb1-358">Request syntax</span></span>

|    <span data-ttu-id="febb1-359">Metod</span><span class="sxs-lookup"><span data-stu-id="febb1-359">Method</span></span>     |    <span data-ttu-id="febb1-360">URI för förfrågan</span><span class="sxs-lookup"><span data-stu-id="febb1-360">Request URI</span></span>     |
|----- | -----|
|    <span data-ttu-id="febb1-361">GET</span><span class="sxs-lookup"><span data-stu-id="febb1-361">GET</span></span>    |`https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport/execution/{reportId}?executionId={executionId}&executionStatus={executionStatus}&getLatestExecution={getLatestExecution}`  |

### <a name="request-header"></a><span data-ttu-id="febb1-362">Begärandehuvud</span><span class="sxs-lookup"><span data-stu-id="febb1-362">Request header</span></span>

|    <span data-ttu-id="febb1-363">Huvud</span><span class="sxs-lookup"><span data-stu-id="febb1-363">Header</span></span>     |    <span data-ttu-id="febb1-364">Typ</span><span class="sxs-lookup"><span data-stu-id="febb1-364">Type</span></span>     |    <span data-ttu-id="febb1-365">Description</span><span class="sxs-lookup"><span data-stu-id="febb1-365">Description</span></span>     |
|-------|-----|------|
|    <span data-ttu-id="febb1-366">Auktorisering</span><span class="sxs-lookup"><span data-stu-id="febb1-366">Authorization</span></span>     |    <span data-ttu-id="febb1-367">sträng</span><span class="sxs-lookup"><span data-stu-id="febb1-367">string</span></span> |<span data-ttu-id="febb1-368">Krävs.</span><span class="sxs-lookup"><span data-stu-id="febb1-368">Required.</span></span> <span data-ttu-id="febb1-369">Åtkomsttoken Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="febb1-369">The Azure Active Directory (Azure AD) access token.</span></span> <span data-ttu-id="febb1-370">Formatet är  `Bearer <token>` .</span><span class="sxs-lookup"><span data-stu-id="febb1-370">The format is `Bearer <token>`.</span></span>|
|    <span data-ttu-id="febb1-371">Content-Type</span><span class="sxs-lookup"><span data-stu-id="febb1-371">Content-Type</span></span>     |<span data-ttu-id="febb1-372">sträng</span><span class="sxs-lookup"><span data-stu-id="febb1-372">string</span></span> |`Application/JSON` |

### <a name="path-parameter"></a><span data-ttu-id="febb1-373">Sökvägsparameter</span><span class="sxs-lookup"><span data-stu-id="febb1-373">Path parameter</span></span>

|    <span data-ttu-id="febb1-374">Parameternamn</span><span class="sxs-lookup"><span data-stu-id="febb1-374">Parameter Name</span></span>    |    <span data-ttu-id="febb1-375">Krävs</span><span class="sxs-lookup"><span data-stu-id="febb1-375">Required</span></span>    |    <span data-ttu-id="febb1-376">Typ</span><span class="sxs-lookup"><span data-stu-id="febb1-376">Type</span></span>    |    <span data-ttu-id="febb1-377">Description</span><span class="sxs-lookup"><span data-stu-id="febb1-377">Description</span></span>    |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="febb1-378">reportId</span><span class="sxs-lookup"><span data-stu-id="febb1-378">reportId</span></span>    |    <span data-ttu-id="febb1-379">Ja</span><span class="sxs-lookup"><span data-stu-id="febb1-379">Yes</span></span>    |    <span data-ttu-id="febb1-380">sträng</span><span class="sxs-lookup"><span data-stu-id="febb1-380">string</span></span>    |    <span data-ttu-id="febb1-381">Filtrera för att hämta körningsinformation för endast rapporter med reportId som anges i det här argumentet.</span><span class="sxs-lookup"><span data-stu-id="febb1-381">Filter to get execution details of only reports with the reportId given in this argument.</span></span> <span data-ttu-id="febb1-382">Flera reportIds kan anges genom att avgränsa dem med ett semikolon ";".</span><span class="sxs-lookup"><span data-stu-id="febb1-382">Multiple reportIds can be specified by separating them with a semicolon ";".</span></span>    |
|        |        |        |        |

### <a name="query-parameter"></a><span data-ttu-id="febb1-383">Frågeparameter</span><span class="sxs-lookup"><span data-stu-id="febb1-383">Query parameter</span></span>

|    <span data-ttu-id="febb1-384">Parameternamn</span><span class="sxs-lookup"><span data-stu-id="febb1-384">Parameter Name</span></span>    |    <span data-ttu-id="febb1-385">Krävs</span><span class="sxs-lookup"><span data-stu-id="febb1-385">Required</span></span>    |    <span data-ttu-id="febb1-386">Typ</span><span class="sxs-lookup"><span data-stu-id="febb1-386">Type</span></span>    |    <span data-ttu-id="febb1-387">Description</span><span class="sxs-lookup"><span data-stu-id="febb1-387">Description</span></span>    |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="febb1-388">executionId</span><span class="sxs-lookup"><span data-stu-id="febb1-388">executionId</span></span>    |    <span data-ttu-id="febb1-389">Inga</span><span class="sxs-lookup"><span data-stu-id="febb1-389">No</span></span>    |    <span data-ttu-id="febb1-390">sträng</span><span class="sxs-lookup"><span data-stu-id="febb1-390">string</span></span>    |    <span data-ttu-id="febb1-391">Filtrera för att hämta information om endast rapporter med executionId som anges i det här argumentet.</span><span class="sxs-lookup"><span data-stu-id="febb1-391">Filter to get details of only reports with the executionId given in this argument.</span></span> <span data-ttu-id="febb1-392">Flera executionIds kan anges genom att avgränsa dem med ett semikolon ";".</span><span class="sxs-lookup"><span data-stu-id="febb1-392">Multiple executionIds can be specified by separating them with a semicolon ";".</span></span>    |
|    <span data-ttu-id="febb1-393">executionStatus</span><span class="sxs-lookup"><span data-stu-id="febb1-393">executionStatus</span></span>    |    <span data-ttu-id="febb1-394">Inga</span><span class="sxs-lookup"><span data-stu-id="febb1-394">No</span></span>    |    <span data-ttu-id="febb1-395">Sträng/uppräkning</span><span class="sxs-lookup"><span data-stu-id="febb1-395">String/enum</span></span>    |    <span data-ttu-id="febb1-396">Filtrera för att hämta information om endast rapporter med executionStatus som anges i det här argumentet.</span><span class="sxs-lookup"><span data-stu-id="febb1-396">Filter to get details of only reports with the executionStatus given in this argument.</span></span> <br> <span data-ttu-id="febb1-397">Giltiga värden är: `Pending` `Running` , och `Paused` `Completed` .</span><span class="sxs-lookup"><span data-stu-id="febb1-397">Valid values are: `Pending`, `Running`, `Paused` and `Completed`.</span></span> <br> <span data-ttu-id="febb1-398">Standardvärdet är `Completed`.</span><span class="sxs-lookup"><span data-stu-id="febb1-398">The default value is `Completed`.</span></span> <br> <span data-ttu-id="febb1-399">Flera statusar kan anges genom att avgränsa dem med semikolon ";".</span><span class="sxs-lookup"><span data-stu-id="febb1-399">Multiple statuses can be specified by separating them with a semicolon ";".</span></span>    |
|    <span data-ttu-id="febb1-400">getLatestExecution</span><span class="sxs-lookup"><span data-stu-id="febb1-400">getLatestExecution</span></span>    |    <span data-ttu-id="febb1-401">Inga</span><span class="sxs-lookup"><span data-stu-id="febb1-401">No</span></span>    |    <span data-ttu-id="febb1-402">boolean</span><span class="sxs-lookup"><span data-stu-id="febb1-402">boolean</span></span>    |    <span data-ttu-id="febb1-403">API:et returnerar information om den senaste körningen.</span><span class="sxs-lookup"><span data-stu-id="febb1-403">The API will return details of the latest execution.</span></span> <span data-ttu-id="febb1-404">Som standard är den här parametern inställd på true.</span><span class="sxs-lookup"><span data-stu-id="febb1-404">By default, this parameter is set to true.</span></span><br> <span data-ttu-id="febb1-405">Om du väljer att skicka värdet för den här parametern som false returnerar API:et de senaste 90 dagarnas körningsinstanser.</span><span class="sxs-lookup"><span data-stu-id="febb1-405">If you choose to pass the value of this parameter as false, then the API will return the last 90 days execution instances.</span></span>    |
|        |        |        |        |

### <a name="sample-request-payload"></a><span data-ttu-id="febb1-406">Exempel på nyttolast för begäran</span><span class="sxs-lookup"><span data-stu-id="febb1-406">Sample Request Payload</span></span>

<span data-ttu-id="febb1-407">Ingen</span><span class="sxs-lookup"><span data-stu-id="febb1-407">None</span></span>

### <a name="sample-response"></a><span data-ttu-id="febb1-408">Exempelsvar</span><span class="sxs-lookup"><span data-stu-id="febb1-408">Sample Response</span></span>

<span data-ttu-id="febb1-409">Svarsnyttolasten är strukturerad på följande sätt:</span><span class="sxs-lookup"><span data-stu-id="febb1-409">The response payload is structured as follows:</span></span>

<span data-ttu-id="febb1-410">Svarskoder: 200, 400, 401, 403, 404, 500</span><span class="sxs-lookup"><span data-stu-id="febb1-410">Response Codes: 200, 400, 401, 403, 404, 500</span></span>

<span data-ttu-id="febb1-411">Exempel på nyttolast för svar:</span><span class="sxs-lookup"><span data-stu-id="febb1-411">Response payload example:</span></span>

```json
{
  "value": [
    {
      "executionId": "906931dc-4f2f-4195-bbb2-d7295c7550d3",
      "reportId": "d9548477-16d4-492a-bf9c-0cf91a9f69bf",
      "recurrenceInterval": 24,
      "recurrenceCount": 100,
      "callbackUrl": null,
      "callbackMethod": null,
      "format": "csv",
      "executionStatus": "Completed",
      "reportLocation": null,
      "reportAccessSecureLink": "https://<path to report for download>",
      "reportExpiryTime": null,
      "reportGeneratedTime": "2021-03-31T18:41:00Z"
    }
  ],
  "nextLink": null,
  "totalCount": 1,
  "message": null,
  "statusCode": 200,
  "dataRedacted": false
}
```

<span data-ttu-id="febb1-412">När rapportkörningen är klar visas `Completed` körningsstatusen.</span><span class="sxs-lookup"><span data-stu-id="febb1-412">Once report execution is complete, the execution status `Completed` is shown.</span></span> <span data-ttu-id="febb1-413">Du kan ladda ned rapporten genom att välja URL:en i `reportAccessSecureLink` .</span><span class="sxs-lookup"><span data-stu-id="febb1-413">You can download the report by selecting the URL in the `reportAccessSecureLink`.</span></span>

### <a name="glossary"></a><span data-ttu-id="febb1-414">Ordlista</span><span class="sxs-lookup"><span data-stu-id="febb1-414">Glossary</span></span>

<span data-ttu-id="febb1-415">Viktiga definitioner av element i svaret.</span><span class="sxs-lookup"><span data-stu-id="febb1-415">Key definitions of elements in the response.</span></span>

|    <span data-ttu-id="febb1-416">Parameter</span><span class="sxs-lookup"><span data-stu-id="febb1-416">Parameter</span></span>    |    <span data-ttu-id="febb1-417">Beskrivning</span><span class="sxs-lookup"><span data-stu-id="febb1-417">Description</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="febb1-418">ExecutionId</span><span class="sxs-lookup"><span data-stu-id="febb1-418">ExecutionId</span></span>    |    <span data-ttu-id="febb1-419">Universell unik identifierare (UUID) för körningsinstansen</span><span class="sxs-lookup"><span data-stu-id="febb1-419">Universally unique identifier (UUID) of the execution instance</span></span>    |
|    <span data-ttu-id="febb1-420">ReportId</span><span class="sxs-lookup"><span data-stu-id="febb1-420">ReportId</span></span>    |    <span data-ttu-id="febb1-421">Rapport-ID som är associerat med körningsinstansen</span><span class="sxs-lookup"><span data-stu-id="febb1-421">Report ID associated with the execution instance</span></span>    |
|    <span data-ttu-id="febb1-422">RecurrenceInterval</span><span class="sxs-lookup"><span data-stu-id="febb1-422">RecurrenceInterval</span></span>    |    <span data-ttu-id="febb1-423">Upprepningsintervall som anges när rapporten skapas</span><span class="sxs-lookup"><span data-stu-id="febb1-423">Recurrence interval provided during report creation</span></span>    |
|    <span data-ttu-id="febb1-424">RecurrenceCount</span><span class="sxs-lookup"><span data-stu-id="febb1-424">RecurrenceCount</span></span>    |    <span data-ttu-id="febb1-425">Antal upprepningar som anges när rapporten skapas</span><span class="sxs-lookup"><span data-stu-id="febb1-425">Recurrence count provided during report creation</span></span>    |
|    <span data-ttu-id="febb1-426">CallbackUrl</span><span class="sxs-lookup"><span data-stu-id="febb1-426">CallbackUrl</span></span>    |    <span data-ttu-id="febb1-427">Motringning-URL som är associerad med körningsinstansen</span><span class="sxs-lookup"><span data-stu-id="febb1-427">Callback URL associated with the execution instance</span></span>    |
|    <span data-ttu-id="febb1-428">CallbackMethod</span><span class="sxs-lookup"><span data-stu-id="febb1-428">CallbackMethod</span></span>    |    <span data-ttu-id="febb1-429">Återanropsmetod som är associerad med körningsinstansen</span><span class="sxs-lookup"><span data-stu-id="febb1-429">Callback method associated with the execution instance</span></span>    |
|    <span data-ttu-id="febb1-430">Format</span><span class="sxs-lookup"><span data-stu-id="febb1-430">Format</span></span>    |    <span data-ttu-id="febb1-431">Format för den genererade filen i slutet av körningen</span><span class="sxs-lookup"><span data-stu-id="febb1-431">Format of the generated file at the end of execution</span></span>    |
|    <span data-ttu-id="febb1-432">ExecutionStatus</span><span class="sxs-lookup"><span data-stu-id="febb1-432">ExecutionStatus</span></span>    |    <span data-ttu-id="febb1-433">Status för rapportkörningsinstansen.</span><span class="sxs-lookup"><span data-stu-id="febb1-433">Status of the report execution instance.</span></span> <br> <span data-ttu-id="febb1-434">Giltiga värden är: `Pending` `Running` , , `Paused` och `Completed`</span><span class="sxs-lookup"><span data-stu-id="febb1-434">Valid values are: `Pending`, `Running`, `Paused`, and `Completed`</span></span>    |
|    <span data-ttu-id="febb1-435">ReportAccessSecureLink</span><span class="sxs-lookup"><span data-stu-id="febb1-435">ReportAccessSecureLink</span></span>    |<span data-ttu-id="febb1-436">Länk genom vilken rapporten kan nås på ett säkert sätt</span><span class="sxs-lookup"><span data-stu-id="febb1-436">Link through which the report can be accessed securely</span></span>        |
|    <span data-ttu-id="febb1-437">ReportExpiryTime</span><span class="sxs-lookup"><span data-stu-id="febb1-437">ReportExpiryTime</span></span>    |    <span data-ttu-id="febb1-438">UTC-tid efter vilken rapportlänken upphör att gälla i det här formatet: yyyy-MM-ddTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="febb1-438">UTC Time after which the report link will expire in this format: yyyy-MM-ddTHH:mm:ssZ</span></span>    |
|    <span data-ttu-id="febb1-439">ReportGeneratedTime</span><span class="sxs-lookup"><span data-stu-id="febb1-439">ReportGeneratedTime</span></span>    |    <span data-ttu-id="febb1-440">UTC-tid då rapporten genererades i det här formatet: yyyy-MM-ddTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="febb1-440">UTC Time at which the report was generated in this format: yyyy-MM-ddTHH:mm:ssZ</span></span>    |
|    <span data-ttu-id="febb1-441">TotalCount</span><span class="sxs-lookup"><span data-stu-id="febb1-441">TotalCount</span></span>    |    <span data-ttu-id="febb1-442">Antal datauppsättningar i värdematrisen</span><span class="sxs-lookup"><span data-stu-id="febb1-442">Number of datasets in the Value array</span></span>    |
|    <span data-ttu-id="febb1-443">StatusCode</span><span class="sxs-lookup"><span data-stu-id="febb1-443">StatusCode</span></span>    |    <span data-ttu-id="febb1-444">Resultatkod</span><span class="sxs-lookup"><span data-stu-id="febb1-444">Result Code</span></span> <br> <span data-ttu-id="febb1-445">Möjliga värden är 200, 400, 401, 403, 404 och 500</span><span class="sxs-lookup"><span data-stu-id="febb1-445">The possible values are 200, 400, 401, 403, 404 and 500</span></span>    |
|    <span data-ttu-id="febb1-446">meddelande</span><span class="sxs-lookup"><span data-stu-id="febb1-446">message</span></span>    |    <span data-ttu-id="febb1-447">Statusmeddelande från körningen av API:et</span><span class="sxs-lookup"><span data-stu-id="febb1-447">Status message from the execution of the API</span></span>    |
|        |        |

## <a name="next-steps"></a><span data-ttu-id="febb1-448">Nästa steg</span><span class="sxs-lookup"><span data-stu-id="febb1-448">Next steps</span></span>

- <span data-ttu-id="febb1-449">Testa API:erna via [Swagger API-URL:en](https://api.partnercenter.microsoft.com/insights/v1/mpn/swagger/index.html)</span><span class="sxs-lookup"><span data-stu-id="febb1-449">Try out the APIs through the [swagger API URL](https://api.partnercenter.microsoft.com/insights/v1/mpn/swagger/index.html)</span></span>
- [<span data-ttu-id="febb1-450">Gör ditt första API-anrop</span><span class="sxs-lookup"><span data-stu-id="febb1-450">Make your first API call</span></span>](insights-programmatic-first-api-call.md)