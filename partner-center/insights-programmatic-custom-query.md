---
title: Specifikation för anpassad fråga
description: Lär dig hur du skapar anpassade frågor för att extrahera data från analystabeller.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 07/14/2021
ms.openlocfilehash: 57f2109044e604dca21b0109b5be56f40170628e
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 07/16/2021
ms.locfileid: "114377165"
---
# <a name="custom-query-specification"></a><span data-ttu-id="6e399-103">Specifikation för anpassad fråga</span><span class="sxs-lookup"><span data-stu-id="6e399-103">Custom query specification</span></span>

<span data-ttu-id="6e399-104">Partner kan använda den här frågespecifikationen för att enkelt formulera anpassade frågor för att extrahera data från analystabeller.</span><span class="sxs-lookup"><span data-stu-id="6e399-104">Partners can use this query specification to easily formulate custom queries for extracting data from analytics tables.</span></span> <span data-ttu-id="6e399-105">Frågorna kan bara användas för att välja önskade kolumner och mått som matchar ett visst kriterium.</span><span class="sxs-lookup"><span data-stu-id="6e399-105">The queries can be used to select only the desired columns and metrics that match a certain criterion.</span></span> <span data-ttu-id="6e399-106">Kärnan i språkspecifikationen är datauppsättningsdefinitionen som en anpassad fråga kan skrivas på.</span><span class="sxs-lookup"><span data-stu-id="6e399-106">At the heart of the language specification is the dataset definition on which a custom query can be written.</span></span>

## <a name="datasets"></a><span data-ttu-id="6e399-107">Datauppsättningar</span><span class="sxs-lookup"><span data-stu-id="6e399-107">Datasets</span></span>

<span data-ttu-id="6e399-108">På samma sätt som vissa frågor körs mot en databas som har tabeller och kolumner fungerar en anpassad fråga på datauppsättningar som har kolumner och mått.</span><span class="sxs-lookup"><span data-stu-id="6e399-108">In the same way that some queries are run against a database that has tables and columns, a custom query works on Datasets that have columns and metrics.</span></span> <span data-ttu-id="6e399-109">En fullständig lista över tillgängliga datauppsättningar för att utforma en fråga kan hämtas med hjälp av datauppsättnings-API:et.</span><span class="sxs-lookup"><span data-stu-id="6e399-109">The full list of available datasets for formulating a query can be obtained by using the datasets API.</span></span>

<span data-ttu-id="6e399-110">Det här är ett exempel på en datauppsättning som visas som en JSON:</span><span class="sxs-lookup"><span data-stu-id="6e399-110">This is an example of a dataset shown as a JSON:</span></span>

```json
{ 
      "datasetName": "OfficeUsage", 
      "selectableColumns": [ 
        "CustomerTenantId", 
        "CustomerTpid", 
        "WorkloadName", 
        "Month", 
        "PaidAvailableUnits", 
        "MonthlyActiveUsers", 
        "CustomerName", 
        "CustomerMarket", 
        "CustomerSegment",  
        "MPNId", 
        "PartnerName", 
        "PartnerLocation", 
        "PartnerAttributionType", 
        "IsDuplicateRowForPGA" 
      ], 
      "availableMetrics": [ 
        "CustomerCount", 
        "CustomerTenantCount", 
        "TotalPaidAvailableUnits", 
        "TotalMonthlyActiveUsers" 
      ], 
      "availableDateRanges": [ 
        "LAST_MONTH", 
        "LAST_3_MONTHS", 
        "LAST_6_MONTHS", 
        "LAST_1_YEAR", 
        "LIFETIME" 
      ], 
      "minimumRecurrenceInterval": 24 
    },
```

## <a name="parts-of-a-dataset"></a><span data-ttu-id="6e399-111">Delar av en datauppsättning</span><span class="sxs-lookup"><span data-stu-id="6e399-111">Parts of a dataset</span></span>

- <span data-ttu-id="6e399-112">Ett datauppsättningsnamn är som ett databastabellnamn.</span><span class="sxs-lookup"><span data-stu-id="6e399-112">A dataset name is like a database table name.</span></span> <span data-ttu-id="6e399-113">Till exempel OfficeUsage.</span><span class="sxs-lookup"><span data-stu-id="6e399-113">For example, OfficeUsage.</span></span> <span data-ttu-id="6e399-114">En datauppsättning har en lista över kolumner som kan väljas, till exempel CustomerTenantId.</span><span class="sxs-lookup"><span data-stu-id="6e399-114">A dataset has a list of columns that can be selected, such as CustomerTenantId.</span></span>
- <span data-ttu-id="6e399-115">En datauppsättning har också mått, som fungerar som aggregeringsfunktioner i en databas.</span><span class="sxs-lookup"><span data-stu-id="6e399-115">A dataset also has metrics, which are like aggregation functions in a database.</span></span> <span data-ttu-id="6e399-116">Till exempel TotalMonthlyActiveUsers.</span><span class="sxs-lookup"><span data-stu-id="6e399-116">For example, TotalMonthlyActiveUsers.</span></span>
- <span data-ttu-id="6e399-117">Det finns fasta tidsintervall som data kan exporteras över.</span><span class="sxs-lookup"><span data-stu-id="6e399-117">There are fixed time spans over which data can be exported.</span></span>

## <a name="formulating-a-query-on-a-dataset"></a><span data-ttu-id="6e399-118">Utforma en fråga på en datauppsättning</span><span class="sxs-lookup"><span data-stu-id="6e399-118">Formulating a query on a dataset</span></span>

<span data-ttu-id="6e399-119">Det här är några exempelfrågor som visar hur du extraherar olika typer av data.</span><span class="sxs-lookup"><span data-stu-id="6e399-119">These are some sample queries that show how to extract various types of data.</span></span>

|<span data-ttu-id="6e399-120">Söka i data</span><span class="sxs-lookup"><span data-stu-id="6e399-120">Query</span></span>|    <span data-ttu-id="6e399-121">Description</span><span class="sxs-lookup"><span data-stu-id="6e399-121">Description</span></span>    |
|----|    ----    |
|<span data-ttu-id="6e399-122">**SELECT** CustomerTenantId, PaidAvailableUnits **FROM**</span><span class="sxs-lookup"><span data-stu-id="6e399-122">**SELECT** CustomerTenantId, PaidAvailableUnits **FROM**</span></span> <br><span data-ttu-id="6e399-123">OfficeUsage **TIMESPAN** LAST_MONTH</span><span class="sxs-lookup"><span data-stu-id="6e399-123">OfficeUsage **TIMESPAN** LAST_MONTH</span></span>|    <span data-ttu-id="6e399-124">Den här frågan hämtar varje CusotmerTenantID och dess motsvarande PaidAvailableUnits under den senaste månaden.</span><span class="sxs-lookup"><span data-stu-id="6e399-124">This query will get every CusotmerTenantID and its corresponding PaidAvailableUnits in the last 1 month.</span></span>    |
|<span data-ttu-id="6e399-125">**SELECT** CustomerTenantId, PaidAvailableUnits **FROM**</span><span class="sxs-lookup"><span data-stu-id="6e399-125">**SELECT** CustomerTenantId, PaidAvailableUnits **FROM**</span></span> <br><span data-ttu-id="6e399-126">OfficeUsage **ORDER** BY PaidAvailableUnits **LIMIT** 10</span><span class="sxs-lookup"><span data-stu-id="6e399-126">OfficeUsage **ORDER** BY PaidAvailableUnits **LIMIT** 10</span></span>|    <span data-ttu-id="6e399-127">Den här frågan hämtar de 10 främsta kundklienterna i fallande ordning efter antalet betalda tillgängliga enheter.</span><span class="sxs-lookup"><span data-stu-id="6e399-127">This query will get the top 10 customer tenants in decreasing order of the number of paid available units.</span></span>     |
|<span data-ttu-id="6e399-128">**SELECT** CustomerTenantId, PaidAvailableUnits, MonthlyActiveUsers **FROM** OfficeUsage **WHERE** MonthlyActiveUsers > 100000 **ORDER BY** MonthlyActiveUsers **TIMESPAN** LAST_6_MONTHS</span><span class="sxs-lookup"><span data-stu-id="6e399-128">**SELECT** CustomerTenantId, PaidAvailableUnits, MonthlyActiveUsers **FROM** OfficeUsage **WHERE** MonthlyActiveUsers > 100000 **ORDER BY** MonthlyActiveUsers **TIMESPAN** LAST_6_MONTHS</span></span> |    <span data-ttu-id="6e399-129">Den här frågan hämtar PaidAvailableUnits och MonthlyActiveUsers för alla kunder som har MonthlyActiveUsers större än 100 000.</span><span class="sxs-lookup"><span data-stu-id="6e399-129">This query will get the PaidAvailableUnits and MonthlyActiveUsers of all the Customers who have MonthlyActiveUsers greater than 100,000.</span></span>     |
|<span data-ttu-id="6e399-130">**SELECT** CustomerTenantId, Month, MonthlyActiveUsers **FROM**</span><span class="sxs-lookup"><span data-stu-id="6e399-130">**SELECT** CustomerTenantId, Month, MonthlyActiveUsers **FROM**</span></span> <br><span data-ttu-id="6e399-131">OfficeUsage **WHERE** CustomerTpId IN ('2a31c234-1f4e-4c60-909e-76d234f93161', '80780748-3f9a-11eb-b378-0242ac130002')</span><span class="sxs-lookup"><span data-stu-id="6e399-131">OfficeUsage **WHERE** CustomerTpId IN ('2a31c234-1f4e-4c60-909e-76d234f93161', '80780748-3f9a-11eb-b378-0242ac130002')</span></span> |    <span data-ttu-id="6e399-132">Den här frågan hämtar CustomerTenantId och de månatliga aktiva användarna för varje månad av de två CustomerTpId-värdena: '2a31c234-1f4e-4c60-909e-76d234f93161" och "80780748-3f9a-11eb-b378-0242ac130002".</span><span class="sxs-lookup"><span data-stu-id="6e399-132">This query will get the CustomerTenantId and the monthly active users for every month by the two CustomerTpId values: '2a31c234-1f4e-4c60-909e-76d234f93161' and '80780748-3f9a-11eb-b378-0242ac130002'.</span></span>     |
|        |        |

## <a name="query-specification"></a><span data-ttu-id="6e399-133">Frågespecifikation</span><span class="sxs-lookup"><span data-stu-id="6e399-133">Query specification</span></span>

<span data-ttu-id="6e399-134">I det här avsnittet beskrivs frågedefinitionen och strukturen.</span><span class="sxs-lookup"><span data-stu-id="6e399-134">This section describes the query definition and structure.</span></span>

## <a name="grammar-reference"></a><span data-ttu-id="6e399-135">Grammatikreferens</span><span class="sxs-lookup"><span data-stu-id="6e399-135">Grammar reference</span></span>

<span data-ttu-id="6e399-136">I den här tabellen beskrivs de symboler som används i frågor.</span><span class="sxs-lookup"><span data-stu-id="6e399-136">This table describes the symbols used in queries.</span></span>

|    <span data-ttu-id="6e399-137">Söka i data</span><span class="sxs-lookup"><span data-stu-id="6e399-137">Query</span></span>    |    <span data-ttu-id="6e399-138">Description</span><span class="sxs-lookup"><span data-stu-id="6e399-138">Description</span></span>    |
|    ----    |    ----    |
|    `?`    |    <span data-ttu-id="6e399-139">Valfritt</span><span class="sxs-lookup"><span data-stu-id="6e399-139">Optional</span></span>    |
|    `*`    |    <span data-ttu-id="6e399-140">Noll eller mer</span><span class="sxs-lookup"><span data-stu-id="6e399-140">Zero or more</span></span>    |
|    `+`    |    <span data-ttu-id="6e399-141">En eller flera</span><span class="sxs-lookup"><span data-stu-id="6e399-141">One or more</span></span>    |
|    `\|`    |    <span data-ttu-id="6e399-142">Eller / en av listorna</span><span class="sxs-lookup"><span data-stu-id="6e399-142">Or / One of the lists</span></span>    |
|        |        |

## <a name="query-definition"></a><span data-ttu-id="6e399-143">Frågedefinition</span><span class="sxs-lookup"><span data-stu-id="6e399-143">Query definition</span></span>

<span data-ttu-id="6e399-144">Frågesatsen har följande satser: SelectClause, FromClause, WhereClause, OrderClause, LimitClause och TimeSpan.</span><span class="sxs-lookup"><span data-stu-id="6e399-144">The query statement has the following clauses: SelectClause, FromClause, WhereClause, OrderClause, LimitClause, and TimeSpan.</span></span>

- <span data-ttu-id="6e399-145">**VäljClause:**`SELECT ColumOrMetricName (, ColumOrMetricName)*`</span><span class="sxs-lookup"><span data-stu-id="6e399-145">**SelectClause**: `SELECT ColumOrMetricName (, ColumOrMetricName)*`</span></span>
    - <span data-ttu-id="6e399-146">**ColumOrMetricName:** Kolumner och mått som definierats i datauppsättningen</span><span class="sxs-lookup"><span data-stu-id="6e399-146">**ColumOrMetricName**: Columns and Metrics defined within the Dataset</span></span>
- <span data-ttu-id="6e399-147">**FromClause**: `FROM DatasetName`</span><span class="sxs-lookup"><span data-stu-id="6e399-147">**FromClause**: `FROM DatasetName`</span></span>
    - <span data-ttu-id="6e399-148">**DatasetName:** Datauppsättningens namn som definierats i datauppsättningen</span><span class="sxs-lookup"><span data-stu-id="6e399-148">**DatasetName**: Dataset name defined within the Dataset</span></span>
- <span data-ttu-id="6e399-149">**WhereClause**: `WHERE FilterCondition (AND FilterCondition)`</span><span class="sxs-lookup"><span data-stu-id="6e399-149">**WhereClause**: `WHERE FilterCondition (AND FilterCondition)`</span></span>
    - <span data-ttu-id="6e399-150">**FilterCondition:** ColumOrMetricName Operator Value</span><span class="sxs-lookup"><span data-stu-id="6e399-150">**FilterCondition**: ColumOrMetricName Operator Value</span></span>
        - <span data-ttu-id="6e399-151">**Operator**:  `=` | `>` | `<` | `>=` | `<=` | `!=` | `LIKE` | `NOT LIKE` | `IN` | `NOT IN`</span><span class="sxs-lookup"><span data-stu-id="6e399-151">**Operator**:  `=` | `>` | `<` | `>=` | `<=` | `!=` | `LIKE` | `NOT LIKE` | `IN` | `NOT IN`</span></span>
        - <span data-ttu-id="6e399-152">**Värde:**| StringLiteral-| MultiNumberList-| MultiStringList</span><span class="sxs-lookup"><span data-stu-id="6e399-152">**Value**: Number | StringLiteral | MultiNumberList | MultiStringList</span></span>
            - <span data-ttu-id="6e399-153">**Nummer**: `-? [0-9]+ (. [0-9] [0-9]*)?`</span><span class="sxs-lookup"><span data-stu-id="6e399-153">**Number**: `-? [0-9]+ (. [0-9] [0-9]*)?`</span></span>
            - <span data-ttu-id="6e399-154">**StringLiteral**:  `' [a-zA-Z0-9_]*'`</span><span class="sxs-lookup"><span data-stu-id="6e399-154">**StringLiteral**:  `' [a-zA-Z0-9_]*'`</span></span>
            - <span data-ttu-id="6e399-155">**MultiNumberList:**`(Number (,Number)*)`</span><span class="sxs-lookup"><span data-stu-id="6e399-155">**MultiNumberList**: `(Number (,Number)*)`</span></span>
            - <span data-ttu-id="6e399-156">**MultiStringList:**`(StringLiteral (,StringLiteral)*)`</span><span class="sxs-lookup"><span data-stu-id="6e399-156">**MultiStringList**: `(StringLiteral (,StringLiteral)*)`</span></span>
- <span data-ttu-id="6e399-157">**OrderClause:**`ORDER BY OrderCondition (,OrderCondition)`</span><span class="sxs-lookup"><span data-stu-id="6e399-157">**OrderClause**: `ORDER BY OrderCondition (,OrderCondition)`</span></span>
    - <span data-ttu-id="6e399-158">**OrderCondition**: `ColumOrMetricName (ASC | DESC)*`</span><span class="sxs-lookup"><span data-stu-id="6e399-158">**OrderCondition**: `ColumOrMetricName (ASC | DESC)*`</span></span>
- <span data-ttu-id="6e399-159">**LimitClause:**`LIMIT [0-9]+`</span><span class="sxs-lookup"><span data-stu-id="6e399-159">**LimitClause**: `LIMIT [0-9]+`</span></span>
- <span data-ttu-id="6e399-160">**TimeSpan**: `TIMESPAN ( TODAY | YESTERDAY | LAST_7_DAYS | LAST_14_DAYS |LAST_30_DAYS | LAST_90_DAYS | LAST_180_DAYS | LAST_365_DAYS |LAST_MONTH | LAST_3_MONTHS | LAST_6_MONTHS | LAST_1_YEAR | LIFETIME)`</span><span class="sxs-lookup"><span data-stu-id="6e399-160">**TimeSpan**: `TIMESPAN ( TODAY | YESTERDAY | LAST_7_DAYS | LAST_14_DAYS |LAST_30_DAYS | LAST_90_DAYS | LAST_180_DAYS | LAST_365_DAYS |LAST_MONTH | LAST_3_MONTHS | LAST_6_MONTHS | LAST_1_YEAR | LIFETIME)`</span></span>

## <a name="query-structure"></a><span data-ttu-id="6e399-161">Frågestruktur</span><span class="sxs-lookup"><span data-stu-id="6e399-161">Query Structure</span></span>

<span data-ttu-id="6e399-162">En rapportfråga består av flera delar:</span><span class="sxs-lookup"><span data-stu-id="6e399-162">A Report query is made up of multiple parts:</span></span>
- `SELECT`
- `FROM`
- `WHERE`
- `ORDER BY`
- `LIMIT`
- `TIMESPAN`

<span data-ttu-id="6e399-163">Varje del beskrivs nedan.</span><span class="sxs-lookup"><span data-stu-id="6e399-163">Each part is described below.</span></span>

### `SELECT`

<span data-ttu-id="6e399-164">Den här delen av frågan anger de kolumner som ska exporteras.</span><span class="sxs-lookup"><span data-stu-id="6e399-164">This part of the query specifies the columns that will get exported.</span></span> <span data-ttu-id="6e399-165">De kolumner som kan väljas är de fält som listas *i selectableColumns* *och availableMetrics-avsnitten* i en datauppsättning.</span><span class="sxs-lookup"><span data-stu-id="6e399-165">The columns that can be selected are the fields listed in *selectableColumns* and *availableMetrics* sections of a dataset.</span></span>

<span data-ttu-id="6e399-166">Nyckelord kan `DISTINCT` också anges efter `SELECT` .</span><span class="sxs-lookup"><span data-stu-id="6e399-166">Optionally, `DISTINCT` keyword can be specified after `SELECT`.</span></span> <span data-ttu-id="6e399-167">Om `DISTINCT` anges innehåller de slutliga exporterade raderna alltid distinkta värden för de valda kolumnerna.</span><span class="sxs-lookup"><span data-stu-id="6e399-167">If `DISTINCT` is specified, then the final exported rows will always contain distinct values of the selected columns.</span></span> <span data-ttu-id="6e399-168">Mått beräknas för varje distinkt kombination av de valda kolumnerna, och därför krävs inte nyckelord när en måttkolumn `DISTINCT` ingår i listan välj kolumn.</span><span class="sxs-lookup"><span data-stu-id="6e399-168">Metrics will be calculated for every distinct combination of the selected columns, hence `DISTINCT` keyword is not required when a metric column is included in the select column list.</span></span>

<span data-ttu-id="6e399-169">**Exempel:**</span><span class="sxs-lookup"><span data-stu-id="6e399-169">**Example:**</span></span>

```sql
SELECT CustomerTenantId, PaidAvailableUnits; 
SELECT DISTINCT CustomerTenantId
```

### `FROM`

<span data-ttu-id="6e399-170">Den här delen av frågan anger datauppsättningen som data behöver exporteras från.</span><span class="sxs-lookup"><span data-stu-id="6e399-170">This part of the query indicates the dataset from which data needs to be exported.</span></span> <span data-ttu-id="6e399-171">Datauppsättningens namn som anges här måste vara ett giltigt datauppsättningsnamn som returneras av datauppsättnings-API:et.</span><span class="sxs-lookup"><span data-stu-id="6e399-171">The dataset name given here needs to be a valid dataset name returned by the datasets API.</span></span>

<span data-ttu-id="6e399-172">**Exempel:**</span><span class="sxs-lookup"><span data-stu-id="6e399-172">**Example:**</span></span>

- `FROM  OfficeUsage`
- `FROM  AzureUsage`

### `WHERE`

<span data-ttu-id="6e399-173">Den här delen av frågan används för att ange filtervillkor för datauppsättningen.</span><span class="sxs-lookup"><span data-stu-id="6e399-173">This part of the query is used to specify filter conditions on the dataset.</span></span> <span data-ttu-id="6e399-174">Endast rader som matchar alla villkor som anges i den här satsen finns i den slutgiltiga exporterade filen.</span><span class="sxs-lookup"><span data-stu-id="6e399-174">Only rows matching all the conditions listed in this clause will be present in the final exported file.</span></span> <span data-ttu-id="6e399-175">Filtervillkoret kan finnas på vilken som helst av kolumnerna som anges *i selectableColumns* och *availableMetrics*.</span><span class="sxs-lookup"><span data-stu-id="6e399-175">The filter condition can be on any of the columns listed in *selectableColumns* and *availableMetrics*.</span></span> <span data-ttu-id="6e399-176">Värdena som anges i filtervillkoret kan vara en lista med tal eller en lista med strängar endast när operatorn `IN` är eller `NOT IN` .</span><span class="sxs-lookup"><span data-stu-id="6e399-176">The values specified in the filter condition can be a list of numbers or a list of strings only when the operator is `IN` or `NOT IN`.</span></span> <span data-ttu-id="6e399-177">Värdena kan alltid anges som en literalsträng och de konverteras till de interna typerna av kolumner.</span><span class="sxs-lookup"><span data-stu-id="6e399-177">The values can always be given as a literal string and they will be converted to the native types of columns.</span></span> <span data-ttu-id="6e399-178">Flera filtervillkor måste avgränsas med en AND-åtgärd.</span><span class="sxs-lookup"><span data-stu-id="6e399-178">Multiple filter conditions need to be separated with an AND operation.</span></span>

<span data-ttu-id="6e399-179">**Exempel:**</span><span class="sxs-lookup"><span data-stu-id="6e399-179">**Example:**</span></span>

- `CustomerTenantId= '868368da-957d-4959-8992-3c12dc7e6260'`
- `CustomerName LIKE '%Contoso%'`
- `CustomerId NOT IN (1000, 1001, 1002)`
- `OrderQuantity=100`
- `CustomerTenantId='7b487ac0-ce12-b732-dcd6-91a1e4e74a50' AND CustomerTpId=' 0f8b7fa0-eb83-a183-1225-ca153ef807aa'`

### `ORDER BY`

<span data-ttu-id="6e399-180">Den här delen av frågan anger ordningskriterierna för de exporterade raderna.</span><span class="sxs-lookup"><span data-stu-id="6e399-180">This part of the query specifies the ordering criteria for the exported rows.</span></span> <span data-ttu-id="6e399-181">Kolumnerna som du kan definiera ordning på måste vara från *selectableColumns* och *availableMetrics för* datauppsättningen.</span><span class="sxs-lookup"><span data-stu-id="6e399-181">The columns on which ordering can be defined need to be from the *selectableColumns* and *availableMetrics* of the dataset.</span></span> <span data-ttu-id="6e399-182">Om det inte finns någon angiven ordningsriktning anges den som standard till DESC i kolumnen.</span><span class="sxs-lookup"><span data-stu-id="6e399-182">If there is no ordering direction specified, it will be defaulted to DESC on the column.</span></span> <span data-ttu-id="6e399-183">Du kan definiera ordning på flera kolumner genom att avgränsa villkoren med ett kommatecken.</span><span class="sxs-lookup"><span data-stu-id="6e399-183">Ordering can be defined on multiple columns by separating the criteria with a comma.</span></span>

<span data-ttu-id="6e399-184">**Exempel:**</span><span class="sxs-lookup"><span data-stu-id="6e399-184">**Example:**</span></span>

- `ORDER BY  MonthlyActiveUsers ASC,  Month DESC`
- `ORDER BY CustomerName ASC,  Month`

### `LIMIT`

<span data-ttu-id="6e399-185">Den här delen av frågan anger antalet rader som ska exporteras.</span><span class="sxs-lookup"><span data-stu-id="6e399-185">This part of the query specifies the number of rows that will be exported.</span></span> <span data-ttu-id="6e399-186">Talet du anger måste vara ett positivt heltal som inte är noll.</span><span class="sxs-lookup"><span data-stu-id="6e399-186">The number you specify needs to be a positive nonzero integer.</span></span>

### `TIMESPAN`

<span data-ttu-id="6e399-187">Den här delen av frågan anger hur länge data ska exporteras.</span><span class="sxs-lookup"><span data-stu-id="6e399-187">This part of the query specifies the time duration for which the data needs to be exported.</span></span> <span data-ttu-id="6e399-188">Möjliga värden ska vara från fältet *availableDateRanges* i datauppsättningens definition.</span><span class="sxs-lookup"><span data-stu-id="6e399-188">The possible values should be from the *availableDateRanges* field in the dataset definition.</span></span>

### <a name="case-sensitivity-in-query-specification"></a><span data-ttu-id="6e399-189">Ärendekänslighet i frågespecifikationen</span><span class="sxs-lookup"><span data-stu-id="6e399-189">Case sensitivity in query specification</span></span>

<span data-ttu-id="6e399-190">Specifikationen är helt okänslig.</span><span class="sxs-lookup"><span data-stu-id="6e399-190">The specification is completely case insensitive.</span></span> <span data-ttu-id="6e399-191">Fördefinierade nyckelord, kolumnnamn och värden kan anges med versaler eller gemener.</span><span class="sxs-lookup"><span data-stu-id="6e399-191">Predefined keywords, column names and values can be specified using upper or lower case.</span></span>

## <a name="next-steps"></a><span data-ttu-id="6e399-192">Nästa steg</span><span class="sxs-lookup"><span data-stu-id="6e399-192">Next steps</span></span>

- [<span data-ttu-id="6e399-193">Lista över systemfrågor</span><span class="sxs-lookup"><span data-stu-id="6e399-193">List of system queries</span></span>](insights-programmatic-system-queries.md)
- [<span data-ttu-id="6e399-194">Lista över exempelfrågor</span><span class="sxs-lookup"><span data-stu-id="6e399-194">List of sample queries</span></span>](insights-programmatic-sample-queries.md)