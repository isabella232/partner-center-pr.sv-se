---
title: Testa API för rapportfrågor
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Använd det här API:et för att testa din fråga och validera resultaten i Partner Center Insights.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: 13ad6fe385a4d31390b6806d863da3f647105b2c
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 07/16/2021
ms.locfileid: "114377183"
---
# <a name="try-report-queries-api"></a><span data-ttu-id="77c8e-103">Testa API för rapportfrågor</span><span class="sxs-lookup"><span data-stu-id="77c8e-103">Try report queries API</span></span>

<span data-ttu-id="77c8e-104">Det här API:et kör en rapportfrågeutdrag.</span><span class="sxs-lookup"><span data-stu-id="77c8e-104">This API executes a Report query statement.</span></span> <span data-ttu-id="77c8e-105">API:et returnerar bara 100 poster som du som partner kan använda för att kontrollera om data är som förväntat.</span><span class="sxs-lookup"><span data-stu-id="77c8e-105">The API returns only 100 records that you as a partner can use to verify if the data is as you expected.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="77c8e-106">Det här API:et har en tidsgräns för frågekörning på 100 sekunder.</span><span class="sxs-lookup"><span data-stu-id="77c8e-106">This API has a query execution timeout of 100 seconds.</span></span> <span data-ttu-id="77c8e-107">Om du märker att API:et tar mer än 100 sekunder är det mycket troligt att frågan är syntaktiskt korrekt, annars skulle du ha fått en annan felkod än 200.</span><span class="sxs-lookup"><span data-stu-id="77c8e-107">If you notice the API is taking more than 100 seconds, it is highly likely that the query is syntactically correct or else you would have received an error code other than 200.</span></span> <span data-ttu-id="77c8e-108">Den faktiska rapportgenereringen skickar om frågesyntaxen är korrekt.</span><span class="sxs-lookup"><span data-stu-id="77c8e-108">The actual report generation will pass if the query syntax is correct.</span></span>

<span data-ttu-id="77c8e-109">**Begärandesyntax**</span><span class="sxs-lookup"><span data-stu-id="77c8e-109">**Request syntax**</span></span>

|    <span data-ttu-id="77c8e-110">Metod</span><span class="sxs-lookup"><span data-stu-id="77c8e-110">Method</span></span>    |    <span data-ttu-id="77c8e-111">URI för förfrågan</span><span class="sxs-lookup"><span data-stu-id="77c8e-111">Request URI</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="77c8e-112">GET</span><span class="sxs-lookup"><span data-stu-id="77c8e-112">GET</span></span>    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledQueries/testQueryResult?<exportQuery={query text}|queryId={queryId}>`    |
|        |        |

<span data-ttu-id="77c8e-113">**Begärandehuvud**</span><span class="sxs-lookup"><span data-stu-id="77c8e-113">**Request header**</span></span>

|    <span data-ttu-id="77c8e-114">Huvud</span><span class="sxs-lookup"><span data-stu-id="77c8e-114">Header</span></span>    |    <span data-ttu-id="77c8e-115">Typ</span><span class="sxs-lookup"><span data-stu-id="77c8e-115">Type</span></span>    |    <span data-ttu-id="77c8e-116">Description</span><span class="sxs-lookup"><span data-stu-id="77c8e-116">Description</span></span>    |
|    ----    |    ----    |    ----    |
|    <span data-ttu-id="77c8e-117">Auktorisering</span><span class="sxs-lookup"><span data-stu-id="77c8e-117">Authorization</span></span>    |    <span data-ttu-id="77c8e-118">sträng</span><span class="sxs-lookup"><span data-stu-id="77c8e-118">string</span></span>    |    <span data-ttu-id="77c8e-119">Krävs.</span><span class="sxs-lookup"><span data-stu-id="77c8e-119">Required.</span></span> <span data-ttu-id="77c8e-120">Åtkomsttoken Azure Active Directory (AAD) i formuläret`Bearer <token>`</span><span class="sxs-lookup"><span data-stu-id="77c8e-120">The Azure Active Directory (AAD) access token in the form `Bearer <token>`</span></span>    |
|    <span data-ttu-id="77c8e-121">Content-Type</span><span class="sxs-lookup"><span data-stu-id="77c8e-121">Content-Type</span></span>    |    <span data-ttu-id="77c8e-122">sträng</span><span class="sxs-lookup"><span data-stu-id="77c8e-122">string</span></span>    |    `Application/JSON`    |
|        |        |        |

<span data-ttu-id="77c8e-123">**Sökvägsparameter**</span><span class="sxs-lookup"><span data-stu-id="77c8e-123">**Path parameter**</span></span>

<span data-ttu-id="77c8e-124">Ingen</span><span class="sxs-lookup"><span data-stu-id="77c8e-124">None</span></span>

<span data-ttu-id="77c8e-125">**Frågeparameter**</span><span class="sxs-lookup"><span data-stu-id="77c8e-125">**Query parameter**</span></span>

|    <span data-ttu-id="77c8e-126">Parameternamn</span><span class="sxs-lookup"><span data-stu-id="77c8e-126">Parameter Name</span></span>    |    <span data-ttu-id="77c8e-127">Typ</span><span class="sxs-lookup"><span data-stu-id="77c8e-127">Type</span></span>    |    <span data-ttu-id="77c8e-128">Obligatorisk</span><span class="sxs-lookup"><span data-stu-id="77c8e-128">Required</span></span>    |    <span data-ttu-id="77c8e-129">Beskrivning</span><span class="sxs-lookup"><span data-stu-id="77c8e-129">Description</span></span>    |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="77c8e-130">exportQuery</span><span class="sxs-lookup"><span data-stu-id="77c8e-130">exportQuery</span></span>     |    <span data-ttu-id="77c8e-131">sträng</span><span class="sxs-lookup"><span data-stu-id="77c8e-131">string</span></span>    |    <span data-ttu-id="77c8e-132">No</span><span class="sxs-lookup"><span data-stu-id="77c8e-132">No</span></span>    |    <span data-ttu-id="77c8e-133">Rapportfrågesträng som måste köras</span><span class="sxs-lookup"><span data-stu-id="77c8e-133">Report query string that needs to be executed</span></span>     |
|    <span data-ttu-id="77c8e-134">queryId</span><span class="sxs-lookup"><span data-stu-id="77c8e-134">queryId</span></span>     |    <span data-ttu-id="77c8e-135">sträng</span><span class="sxs-lookup"><span data-stu-id="77c8e-135">string</span></span>    |    <span data-ttu-id="77c8e-136">No</span><span class="sxs-lookup"><span data-stu-id="77c8e-136">No</span></span>    |    <span data-ttu-id="77c8e-137">Ett giltigt befintligt fråge-ID.</span><span class="sxs-lookup"><span data-stu-id="77c8e-137">A valid existing query ID.</span></span> <span data-ttu-id="77c8e-138">Ömsesidigt uteslutande med frågesträng som anges i exportQuery-parametern</span><span class="sxs-lookup"><span data-stu-id="77c8e-138">Mutually exclusive with query string specified in exportQuery parameter</span></span>    |
|    <span data-ttu-id="77c8e-139">startTime</span><span class="sxs-lookup"><span data-stu-id="77c8e-139">startTime</span></span>     |    <span data-ttu-id="77c8e-140">sträng</span><span class="sxs-lookup"><span data-stu-id="77c8e-140">string</span></span>    |    <span data-ttu-id="77c8e-141">No</span><span class="sxs-lookup"><span data-stu-id="77c8e-141">No</span></span>    |    <span data-ttu-id="77c8e-142">Starttid från vilken vi vill ha data.</span><span class="sxs-lookup"><span data-stu-id="77c8e-142">Start time from which we want the data.</span></span> <span data-ttu-id="77c8e-143">Det åsidosätter det tidsspann som anges i frågan</span><span class="sxs-lookup"><span data-stu-id="77c8e-143">It overrides timespan specified in the query</span></span>    |
|    <span data-ttu-id="77c8e-144">endTime</span><span class="sxs-lookup"><span data-stu-id="77c8e-144">endTime</span></span>     |    <span data-ttu-id="77c8e-145">sträng</span><span class="sxs-lookup"><span data-stu-id="77c8e-145">string</span></span>    |    <span data-ttu-id="77c8e-146">No</span><span class="sxs-lookup"><span data-stu-id="77c8e-146">No</span></span>    |    <span data-ttu-id="77c8e-147">Sluttid tills vi vill ha data.</span><span class="sxs-lookup"><span data-stu-id="77c8e-147">End time till which we want the data.</span></span> <span data-ttu-id="77c8e-148">Det åsidosätter det tidsspann som anges i frågan</span><span class="sxs-lookup"><span data-stu-id="77c8e-148">It overrides timespan specified in the query</span></span>    |
|        |        |        |        |

<span data-ttu-id="77c8e-149">**Begära nyttolast**</span><span class="sxs-lookup"><span data-stu-id="77c8e-149">**Request payload**</span></span>

<span data-ttu-id="77c8e-150">Ingen</span><span class="sxs-lookup"><span data-stu-id="77c8e-150">None</span></span>

<span data-ttu-id="77c8e-151">**Ordlista**</span><span class="sxs-lookup"><span data-stu-id="77c8e-151">**Glossary**</span></span>

<span data-ttu-id="77c8e-152">Ingen</span><span class="sxs-lookup"><span data-stu-id="77c8e-152">None</span></span>

<span data-ttu-id="77c8e-153">**Response**</span><span class="sxs-lookup"><span data-stu-id="77c8e-153">**Response**</span></span>

<span data-ttu-id="77c8e-154">Svarsnyttolasten är strukturerad på följande sätt:</span><span class="sxs-lookup"><span data-stu-id="77c8e-154">The response payload is structured as follows:</span></span>

<span data-ttu-id="77c8e-155">Svarskod: 200, 400, 401, 403, 404, 500</span><span class="sxs-lookup"><span data-stu-id="77c8e-155">Response code: 200, 400, 401, 403, 404, 500</span></span>

<span data-ttu-id="77c8e-156">Exempel på nyttolast för svar:</span><span class="sxs-lookup"><span data-stu-id="77c8e-156">Response payload example:</span></span>

```json
Top 100 rows of query execution 
{ 
  "Value": [ 
    { 
    } 
  ], 
  "TotalCount": 0, 
  "Message": "string", 
  "StatusCode": 0, 
} 
```

<span data-ttu-id="77c8e-157">**Ordlista**</span><span class="sxs-lookup"><span data-stu-id="77c8e-157">**Glossary**</span></span>

<span data-ttu-id="77c8e-158">Den här tabellen definierar nyckelelementen i svaret:</span><span class="sxs-lookup"><span data-stu-id="77c8e-158">This table defines the key elements in the response:</span></span>

|    <span data-ttu-id="77c8e-159">Parameter</span><span class="sxs-lookup"><span data-stu-id="77c8e-159">Parameter</span></span>    |    <span data-ttu-id="77c8e-160">Beskrivning</span><span class="sxs-lookup"><span data-stu-id="77c8e-160">Description</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="77c8e-161">TotalCount</span><span class="sxs-lookup"><span data-stu-id="77c8e-161">TotalCount</span></span>     |    <span data-ttu-id="77c8e-162">Antal datauppsättningar i värdematrisen</span><span class="sxs-lookup"><span data-stu-id="77c8e-162">Number of datasets in the Value array</span></span>     |
|    <span data-ttu-id="77c8e-163">Meddelande</span><span class="sxs-lookup"><span data-stu-id="77c8e-163">Message</span></span>     |    <span data-ttu-id="77c8e-164">Statusmeddelande från körningen av API:et</span><span class="sxs-lookup"><span data-stu-id="77c8e-164">Status message from the execution of the API</span></span>     |
|    <span data-ttu-id="77c8e-165">StatusCode</span><span class="sxs-lookup"><span data-stu-id="77c8e-165">StatusCode</span></span>     |    <span data-ttu-id="77c8e-166">Resultatkod.</span><span class="sxs-lookup"><span data-stu-id="77c8e-166">Result Code.</span></span> <span data-ttu-id="77c8e-167">Möjliga värden är 200, 400, 401, 403, 500</span><span class="sxs-lookup"><span data-stu-id="77c8e-167">The possible values are 200, 400, 401, 403, 500</span></span>     |
|        |        |
