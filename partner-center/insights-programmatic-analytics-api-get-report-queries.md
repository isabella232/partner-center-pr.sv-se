---
title: HÄMTA API för rapportfrågor – Insights data
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Använd det här API:et för att hämta alla tillgängliga frågor som ska användas i rapport-API:et.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: 3bf140576a19439990405cfef23190045e0a98be
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 07/16/2021
ms.locfileid: "114377207"
---
# <a name="get-report-queries-api"></a><span data-ttu-id="bac1d-103">HÄMTA API för rapportfrågor</span><span class="sxs-lookup"><span data-stu-id="bac1d-103">Get report queries API</span></span>

<span data-ttu-id="bac1d-104">API:et Hämta rapportfrågor hämtar alla frågor som är tillgängliga för användning i rapporter.</span><span class="sxs-lookup"><span data-stu-id="bac1d-104">The Get report queries API gets all the queries that are available for use in reports.</span></span> <span data-ttu-id="bac1d-105">Den hämtar alla system- och användardefinierade frågor som standard.</span><span class="sxs-lookup"><span data-stu-id="bac1d-105">It gets all the system and user-defined queries by default.</span></span>

<span data-ttu-id="bac1d-106">**Begärandesyntax**</span><span class="sxs-lookup"><span data-stu-id="bac1d-106">**Request syntax**</span></span>

|    <span data-ttu-id="bac1d-107">Metod</span><span class="sxs-lookup"><span data-stu-id="bac1d-107">Method</span></span>    |    <span data-ttu-id="bac1d-108">URI för förfrågan</span><span class="sxs-lookup"><span data-stu-id="bac1d-108">Request URI</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="bac1d-109">GET</span><span class="sxs-lookup"><span data-stu-id="bac1d-109">GET</span></span>    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledQueries?queryId={QueryID}&queryName={QueryName}&includeSystemQueries={include_system_queries}&includeOnlySystemQueries={include_only_system_queries}`     |
|        |        |

<span data-ttu-id="bac1d-110">**Begärandehuvud**</span><span class="sxs-lookup"><span data-stu-id="bac1d-110">**Request header**</span></span>

|    <span data-ttu-id="bac1d-111">Huvud</span><span class="sxs-lookup"><span data-stu-id="bac1d-111">Header</span></span>    |    <span data-ttu-id="bac1d-112">Typ</span><span class="sxs-lookup"><span data-stu-id="bac1d-112">Type</span></span>    |    <span data-ttu-id="bac1d-113">Description</span><span class="sxs-lookup"><span data-stu-id="bac1d-113">Description</span></span>    |
|    ----    |    ----    |    ----    |
|    <span data-ttu-id="bac1d-114">Auktorisering</span><span class="sxs-lookup"><span data-stu-id="bac1d-114">Authorization</span></span>    |    <span data-ttu-id="bac1d-115">sträng</span><span class="sxs-lookup"><span data-stu-id="bac1d-115">string</span></span>    |    <span data-ttu-id="bac1d-116">Krävs.</span><span class="sxs-lookup"><span data-stu-id="bac1d-116">Required.</span></span> <span data-ttu-id="bac1d-117">Åtkomsttoken Azure Active Directory (AAD) i formuläret`Bearer <token>`</span><span class="sxs-lookup"><span data-stu-id="bac1d-117">The Azure Active Directory (AAD) access token in the form `Bearer <token>`</span></span>    |
|    <span data-ttu-id="bac1d-118">Content-Type</span><span class="sxs-lookup"><span data-stu-id="bac1d-118">Content-Type</span></span>    |    <span data-ttu-id="bac1d-119">sträng</span><span class="sxs-lookup"><span data-stu-id="bac1d-119">string</span></span>    |    `Application/JSON`    |
|        |        |        |

<span data-ttu-id="bac1d-120">**Sökvägsparameter**</span><span class="sxs-lookup"><span data-stu-id="bac1d-120">**Path parameter**</span></span>

<span data-ttu-id="bac1d-121">Ingen</span><span class="sxs-lookup"><span data-stu-id="bac1d-121">None</span></span>

<span data-ttu-id="bac1d-122">**Frågeparameter**</span><span class="sxs-lookup"><span data-stu-id="bac1d-122">**Query parameter**</span></span>

|    <span data-ttu-id="bac1d-123">Parameternamn</span><span class="sxs-lookup"><span data-stu-id="bac1d-123">Parameter Name</span></span>    |    <span data-ttu-id="bac1d-124">Typ</span><span class="sxs-lookup"><span data-stu-id="bac1d-124">Type</span></span>    |    <span data-ttu-id="bac1d-125">Obligatorisk</span><span class="sxs-lookup"><span data-stu-id="bac1d-125">Required</span></span>    |    <span data-ttu-id="bac1d-126">Beskrivning</span><span class="sxs-lookup"><span data-stu-id="bac1d-126">Description</span></span>    |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="bac1d-127">queryId</span><span class="sxs-lookup"><span data-stu-id="bac1d-127">queryId</span></span>     |    <span data-ttu-id="bac1d-128">sträng</span><span class="sxs-lookup"><span data-stu-id="bac1d-128">string</span></span>     |    <span data-ttu-id="bac1d-129">No</span><span class="sxs-lookup"><span data-stu-id="bac1d-129">No</span></span>    |    <span data-ttu-id="bac1d-130">Filtrera för att hämta information om endast frågor med det ID som anges i argumentet</span><span class="sxs-lookup"><span data-stu-id="bac1d-130">Filter to get details of only queries with the ID given in the argument</span></span>     |
|    <span data-ttu-id="bac1d-131">queryName</span><span class="sxs-lookup"><span data-stu-id="bac1d-131">queryName</span></span>     |    <span data-ttu-id="bac1d-132">sträng</span><span class="sxs-lookup"><span data-stu-id="bac1d-132">string</span></span>     |    <span data-ttu-id="bac1d-133">No</span><span class="sxs-lookup"><span data-stu-id="bac1d-133">No</span></span>    |    <span data-ttu-id="bac1d-134">Filter för att hämta information om endast frågor med det namn som anges i argumentet</span><span class="sxs-lookup"><span data-stu-id="bac1d-134">Filter to get details of only queries with the name given in the argument</span></span>     |
|    <span data-ttu-id="bac1d-135">IncludeSystemQueries</span><span class="sxs-lookup"><span data-stu-id="bac1d-135">IncludeSystemQueries</span></span>     |    <span data-ttu-id="bac1d-136">boolean</span><span class="sxs-lookup"><span data-stu-id="bac1d-136">boolean</span></span>     |    <span data-ttu-id="bac1d-137">Inga</span><span class="sxs-lookup"><span data-stu-id="bac1d-137">No</span></span>    |    <span data-ttu-id="bac1d-138">Inkludera fördefinierade systemfrågor i svaret</span><span class="sxs-lookup"><span data-stu-id="bac1d-138">Include predefined system queries in the response</span></span>     |
|    <span data-ttu-id="bac1d-139">IncludeOnlySystemQueries</span><span class="sxs-lookup"><span data-stu-id="bac1d-139">IncludeOnlySystemQueries</span></span>     |    <span data-ttu-id="bac1d-140">boolean</span><span class="sxs-lookup"><span data-stu-id="bac1d-140">boolean</span></span>     |    <span data-ttu-id="bac1d-141">Inga</span><span class="sxs-lookup"><span data-stu-id="bac1d-141">No</span></span>    |    <span data-ttu-id="bac1d-142">Inkludera endast systemfrågor i svaret</span><span class="sxs-lookup"><span data-stu-id="bac1d-142">Include only system queries in the response</span></span>     |
|        |        |        |        |


<span data-ttu-id="bac1d-143">**Begära nyttolast**</span><span class="sxs-lookup"><span data-stu-id="bac1d-143">**Request payload**</span></span>

<span data-ttu-id="bac1d-144">Ingen</span><span class="sxs-lookup"><span data-stu-id="bac1d-144">None</span></span>

<span data-ttu-id="bac1d-145">**Ordlista**</span><span class="sxs-lookup"><span data-stu-id="bac1d-145">**Glossary**</span></span>

<span data-ttu-id="bac1d-146">Ingen</span><span class="sxs-lookup"><span data-stu-id="bac1d-146">None</span></span>

<span data-ttu-id="bac1d-147">**Response**</span><span class="sxs-lookup"><span data-stu-id="bac1d-147">**Response**</span></span>

<span data-ttu-id="bac1d-148">Svarsnyttolasten är strukturerad på följande sätt:</span><span class="sxs-lookup"><span data-stu-id="bac1d-148">The response payload is structured as follows:</span></span>

<span data-ttu-id="bac1d-149">Svarskod: 200, 400, 401, 403, 404, 500</span><span class="sxs-lookup"><span data-stu-id="bac1d-149">Response code: 200, 400, 401, 403, 404, 500</span></span>

<span data-ttu-id="bac1d-150">Exempel på nyttolast för svar:</span><span class="sxs-lookup"><span data-stu-id="bac1d-150">Response payload example:</span></span>

```json
{ 
  "Value": [ 
    { 
      "QueryId": "string", 
      "Name": "string", 
      "Description": "string", 
      "Query": "string", 
      "Type": "string", 
      "User": "string", 
      "CreatedTime": "string", 
    } 
  ], 
  "TotalCount": 0, 
  "Message": "string", 
  "StatusCode": 0, 
} 
```

<span data-ttu-id="bac1d-151">**Ordlista**</span><span class="sxs-lookup"><span data-stu-id="bac1d-151">**Glossary**</span></span>

<span data-ttu-id="bac1d-152">Den här tabellen definierar nyckelelementen i svaret:</span><span class="sxs-lookup"><span data-stu-id="bac1d-152">This table defines the key elements in the response:</span></span>

|    <span data-ttu-id="bac1d-153">Parameter</span><span class="sxs-lookup"><span data-stu-id="bac1d-153">Parameter</span></span>    |    <span data-ttu-id="bac1d-154">Beskrivning</span><span class="sxs-lookup"><span data-stu-id="bac1d-154">Description</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="bac1d-155">QueryId</span><span class="sxs-lookup"><span data-stu-id="bac1d-155">QueryId</span></span>     |    <span data-ttu-id="bac1d-156">Unikt UUID för frågan</span><span class="sxs-lookup"><span data-stu-id="bac1d-156">Unique UUID of the query</span></span>     |
|    <span data-ttu-id="bac1d-157">Name</span><span class="sxs-lookup"><span data-stu-id="bac1d-157">Name</span></span>     |    <span data-ttu-id="bac1d-158">Namn som gavs till frågan när frågan skapades</span><span class="sxs-lookup"><span data-stu-id="bac1d-158">Name given to the query at the time of query creation</span></span>     |
|    <span data-ttu-id="bac1d-159">Description</span><span class="sxs-lookup"><span data-stu-id="bac1d-159">Description</span></span>     |    <span data-ttu-id="bac1d-160">Beskrivning som anges när frågan skapas</span><span class="sxs-lookup"><span data-stu-id="bac1d-160">Description given during creation of the query</span></span>     |
|    <span data-ttu-id="bac1d-161">Söka i data</span><span class="sxs-lookup"><span data-stu-id="bac1d-161">Query</span></span>     |    <span data-ttu-id="bac1d-162">Rapportfrågesträng</span><span class="sxs-lookup"><span data-stu-id="bac1d-162">Report query string</span></span>     |
|    <span data-ttu-id="bac1d-163">Typ</span><span class="sxs-lookup"><span data-stu-id="bac1d-163">Type</span></span>     |    <span data-ttu-id="bac1d-164">Ange till userDefined för användarskapade frågor och system för fördefinierade systemfrågor</span><span class="sxs-lookup"><span data-stu-id="bac1d-164">Set to userDefined for user created queries and system for predefined system queries</span></span>     |
|    <span data-ttu-id="bac1d-165">Användare</span><span class="sxs-lookup"><span data-stu-id="bac1d-165">User</span></span>     |    <span data-ttu-id="bac1d-166">Användar-ID som skapade frågan</span><span class="sxs-lookup"><span data-stu-id="bac1d-166">User ID who created the query</span></span>     |
|    <span data-ttu-id="bac1d-167">CreatedTime</span><span class="sxs-lookup"><span data-stu-id="bac1d-167">CreatedTime</span></span>     |    <span data-ttu-id="bac1d-168">Tid då frågan skapades</span><span class="sxs-lookup"><span data-stu-id="bac1d-168">Time of creation of query</span></span>     |
|    <span data-ttu-id="bac1d-169">TotalCount</span><span class="sxs-lookup"><span data-stu-id="bac1d-169">TotalCount</span></span>     |    <span data-ttu-id="bac1d-170">Antal datauppsättningar i värdematrisen</span><span class="sxs-lookup"><span data-stu-id="bac1d-170">Number of datasets in the Value array</span></span>     |
|    <span data-ttu-id="bac1d-171">Meddelande</span><span class="sxs-lookup"><span data-stu-id="bac1d-171">Message</span></span>     |    <span data-ttu-id="bac1d-172">Statusmeddelande från körningen av API:et</span><span class="sxs-lookup"><span data-stu-id="bac1d-172">Status message from the execution of the API</span></span>     |
|    <span data-ttu-id="bac1d-173">StatusCode</span><span class="sxs-lookup"><span data-stu-id="bac1d-173">StatusCode</span></span>     |    <span data-ttu-id="bac1d-174">Resultatkod.</span><span class="sxs-lookup"><span data-stu-id="bac1d-174">Result Code.</span></span> <span data-ttu-id="bac1d-175">Möjliga värden är 200, 400, 401, 403, 500</span><span class="sxs-lookup"><span data-stu-id="bac1d-175">The possible values are 200, 400, 401, 403, 500</span></span>     |
|        |        |
