---
title: Hämta rapport-API – Insights data
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Använd det här API:et för att hämta alla tillgängliga rapport-ID:n i Partnercenter-insikter.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: 174a2f60a36cb46b287b787b177dd32236cef4eb
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 07/16/2021
ms.locfileid: "114377202"
---
# <a name="get-report-api"></a><span data-ttu-id="70ef8-103">Hämta rapport-API</span><span class="sxs-lookup"><span data-stu-id="70ef8-103">Get report API</span></span>

<span data-ttu-id="70ef8-104">Det här API:et hämtar alla rapporter som har schemalagts.</span><span class="sxs-lookup"><span data-stu-id="70ef8-104">This API gets all the reports that have been scheduled.</span></span>

<span data-ttu-id="70ef8-105">**Begärandesyntax**</span><span class="sxs-lookup"><span data-stu-id="70ef8-105">**Request syntax**</span></span>

|    <span data-ttu-id="70ef8-106">Metod</span><span class="sxs-lookup"><span data-stu-id="70ef8-106">Method</span></span>    |    <span data-ttu-id="70ef8-107">URI för förfrågan</span><span class="sxs-lookup"><span data-stu-id="70ef8-107">Request URI</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="70ef8-108">GET</span><span class="sxs-lookup"><span data-stu-id="70ef8-108">GET</span></span>    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport?reportId={Report ID}&reportName={Report Name}&queryId={Query ID}` |
|        |        |

<span data-ttu-id="70ef8-109">**Begärandehuvud**</span><span class="sxs-lookup"><span data-stu-id="70ef8-109">**Request header**</span></span>

|    <span data-ttu-id="70ef8-110">Huvud</span><span class="sxs-lookup"><span data-stu-id="70ef8-110">Header</span></span>    |    <span data-ttu-id="70ef8-111">Typ</span><span class="sxs-lookup"><span data-stu-id="70ef8-111">Type</span></span>    |    <span data-ttu-id="70ef8-112">Description</span><span class="sxs-lookup"><span data-stu-id="70ef8-112">Description</span></span>    |
|    ----    |    ----    |    ----    |
|    <span data-ttu-id="70ef8-113">Auktorisering</span><span class="sxs-lookup"><span data-stu-id="70ef8-113">Authorization</span></span>    |    <span data-ttu-id="70ef8-114">sträng</span><span class="sxs-lookup"><span data-stu-id="70ef8-114">string</span></span>    |    <span data-ttu-id="70ef8-115">Krävs.</span><span class="sxs-lookup"><span data-stu-id="70ef8-115">Required.</span></span> <span data-ttu-id="70ef8-116">Åtkomsttoken Azure Active Directory (AAD) i formuläret`Bearer <token>`</span><span class="sxs-lookup"><span data-stu-id="70ef8-116">The Azure Active Directory (AAD) access token in the form `Bearer <token>`</span></span>    |
|    <span data-ttu-id="70ef8-117">Content-Type</span><span class="sxs-lookup"><span data-stu-id="70ef8-117">Content-Type</span></span>    |    <span data-ttu-id="70ef8-118">sträng</span><span class="sxs-lookup"><span data-stu-id="70ef8-118">string</span></span>    |    `Application/JSON`    |
|        |        |        |

<span data-ttu-id="70ef8-119">**Sökvägsparameter**</span><span class="sxs-lookup"><span data-stu-id="70ef8-119">**Path parameter**</span></span>

<span data-ttu-id="70ef8-120">Ingen</span><span class="sxs-lookup"><span data-stu-id="70ef8-120">None</span></span>

<span data-ttu-id="70ef8-121">**Frågeparameter**</span><span class="sxs-lookup"><span data-stu-id="70ef8-121">**Query parameter**</span></span>

|    <span data-ttu-id="70ef8-122">Parameternamn</span><span class="sxs-lookup"><span data-stu-id="70ef8-122">Parameter Name</span></span>    |    <span data-ttu-id="70ef8-123">Typ</span><span class="sxs-lookup"><span data-stu-id="70ef8-123">Type</span></span>    |    <span data-ttu-id="70ef8-124">Obligatorisk</span><span class="sxs-lookup"><span data-stu-id="70ef8-124">Required</span></span>    |    <span data-ttu-id="70ef8-125">Beskrivning</span><span class="sxs-lookup"><span data-stu-id="70ef8-125">Description</span></span>    |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="70ef8-126">reportId</span><span class="sxs-lookup"><span data-stu-id="70ef8-126">reportId</span></span>     |    <span data-ttu-id="70ef8-127">sträng</span><span class="sxs-lookup"><span data-stu-id="70ef8-127">string</span></span>    |    <span data-ttu-id="70ef8-128">No</span><span class="sxs-lookup"><span data-stu-id="70ef8-128">No</span></span>    |    <span data-ttu-id="70ef8-129">Filtrera för att hämta information om endast rapporter med reportId som anges i det här argumentet</span><span class="sxs-lookup"><span data-stu-id="70ef8-129">Filter to get details of only reports with the reportId given in this argument</span></span>     |
|    <span data-ttu-id="70ef8-130">reportName</span><span class="sxs-lookup"><span data-stu-id="70ef8-130">reportName</span></span>     |    <span data-ttu-id="70ef8-131">sträng</span><span class="sxs-lookup"><span data-stu-id="70ef8-131">string</span></span>    |    <span data-ttu-id="70ef8-132">No</span><span class="sxs-lookup"><span data-stu-id="70ef8-132">No</span></span>    |    <span data-ttu-id="70ef8-133">Filtrera för att hämta information om endast rapporter med reportName som anges i det här argumentet</span><span class="sxs-lookup"><span data-stu-id="70ef8-133">Filter to get details of only reports with the reportName given in this argument</span></span>     |
|    <span data-ttu-id="70ef8-134">queryId</span><span class="sxs-lookup"><span data-stu-id="70ef8-134">queryId</span></span>     |    <span data-ttu-id="70ef8-135">sträng</span><span class="sxs-lookup"><span data-stu-id="70ef8-135">string</span></span>    |    <span data-ttu-id="70ef8-136">No</span><span class="sxs-lookup"><span data-stu-id="70ef8-136">No</span></span>    |    <span data-ttu-id="70ef8-137">Filtrera för att hämta information om endast rapporter med queryId som anges i det här argumentet</span><span class="sxs-lookup"><span data-stu-id="70ef8-137">Filter to get details of only reports with the queryId given in this argument</span></span>     |
|        |        |        |        |


<span data-ttu-id="70ef8-138">**Begära nyttolast**</span><span class="sxs-lookup"><span data-stu-id="70ef8-138">**Request payload**</span></span>

<span data-ttu-id="70ef8-139">Ingen</span><span class="sxs-lookup"><span data-stu-id="70ef8-139">None</span></span>

<span data-ttu-id="70ef8-140">**Ordlista**</span><span class="sxs-lookup"><span data-stu-id="70ef8-140">**Glossary**</span></span>

<span data-ttu-id="70ef8-141">Ingen</span><span class="sxs-lookup"><span data-stu-id="70ef8-141">None</span></span>

<span data-ttu-id="70ef8-142">**Response**</span><span class="sxs-lookup"><span data-stu-id="70ef8-142">**Response**</span></span>

<span data-ttu-id="70ef8-143">Svarsnyttolasten är strukturerad på följande sätt:</span><span class="sxs-lookup"><span data-stu-id="70ef8-143">The response payload is structured as follows:</span></span>

<span data-ttu-id="70ef8-144">Svarskod: 200, 400, 401, 403, 404, 500</span><span class="sxs-lookup"><span data-stu-id="70ef8-144">Response code: 200, 400, 401, 403, 404, 500</span></span>

<span data-ttu-id="70ef8-145">Exempel på nyttolast för svar:</span><span class="sxs-lookup"><span data-stu-id="70ef8-145">Response payload example:</span></span>

```json
{ 
  "Value": [ 
    { 
      "ReportId": "string", 
      "ReportName": "string", 
      "Description": "string", 
      "QueryId": "string", 
      "Query": "string", 
      "User": "string", 
      "CreatedTime": "string", 
      "ModifiedTime": "string", 
      "executeNow": true, 
      "StartTime": "string", 
      "ReportStatus": "string", 
      "RecurrenceInterval": 0, 
      " RecurrenceCount": 0, 
      "CallbackUrl": "string",
      "CallbackMethod": null,
      "Format": "string" 
    } 
  ], 
  "TotalCount": 0, 
  "Message": "string", 
  "StatusCode": 0 
}
```

<span data-ttu-id="70ef8-146">**Ordlista**</span><span class="sxs-lookup"><span data-stu-id="70ef8-146">**Glossary**</span></span>

<span data-ttu-id="70ef8-147">Den här tabellen definierar nyckelelementen i svaret:</span><span class="sxs-lookup"><span data-stu-id="70ef8-147">This table defines the key elements in the response:</span></span>

|    <span data-ttu-id="70ef8-148">Parameter</span><span class="sxs-lookup"><span data-stu-id="70ef8-148">Parameter</span></span>    |    <span data-ttu-id="70ef8-149">Beskrivning</span><span class="sxs-lookup"><span data-stu-id="70ef8-149">Description</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="70ef8-150">ReportId</span><span class="sxs-lookup"><span data-stu-id="70ef8-150">ReportId</span></span>     |    <span data-ttu-id="70ef8-151">Unikt UUID för rapporten som skapades</span><span class="sxs-lookup"><span data-stu-id="70ef8-151">Unique UUID of the report that was created</span></span>     |
|    <span data-ttu-id="70ef8-152">ReportName</span><span class="sxs-lookup"><span data-stu-id="70ef8-152">ReportName</span></span>     |    <span data-ttu-id="70ef8-153">Namn som ges till rapporten i nyttolasten för begäran</span><span class="sxs-lookup"><span data-stu-id="70ef8-153">Name given to the report in the request payload</span></span>     |
|    <span data-ttu-id="70ef8-154">Description</span><span class="sxs-lookup"><span data-stu-id="70ef8-154">Description</span></span>     |    <span data-ttu-id="70ef8-155">Beskrivning som gavs när rapporten skapades</span><span class="sxs-lookup"><span data-stu-id="70ef8-155">Description given when the report was created</span></span>     |
|    <span data-ttu-id="70ef8-156">QueryId</span><span class="sxs-lookup"><span data-stu-id="70ef8-156">QueryId</span></span>     |    <span data-ttu-id="70ef8-157">Fråge-ID som skickades när rapporten skapades</span><span class="sxs-lookup"><span data-stu-id="70ef8-157">Query ID passed at the time the report was created</span></span>     |
|    <span data-ttu-id="70ef8-158">Söka i data</span><span class="sxs-lookup"><span data-stu-id="70ef8-158">Query</span></span>     |    <span data-ttu-id="70ef8-159">Frågetext som ska köras för den här rapporten</span><span class="sxs-lookup"><span data-stu-id="70ef8-159">Query text that will be executed for this report</span></span>     |
|    <span data-ttu-id="70ef8-160">Användare</span><span class="sxs-lookup"><span data-stu-id="70ef8-160">User</span></span>     |    <span data-ttu-id="70ef8-161">Användar-ID som används för att skapa rapporten</span><span class="sxs-lookup"><span data-stu-id="70ef8-161">User ID used to create the report</span></span>     |
|    <span data-ttu-id="70ef8-162">CreatedTime</span><span class="sxs-lookup"><span data-stu-id="70ef8-162">CreatedTime</span></span>     |    <span data-ttu-id="70ef8-163">Tid då rapporten skapades.</span><span class="sxs-lookup"><span data-stu-id="70ef8-163">Time the report was created.</span></span> <span data-ttu-id="70ef8-164">Tidsformatet är yyyy-MM-ddTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="70ef8-164">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="70ef8-165">ModifiedTime</span><span class="sxs-lookup"><span data-stu-id="70ef8-165">ModifiedTime</span></span>     |    <span data-ttu-id="70ef8-166">Tid då rapporten senast ändrades.</span><span class="sxs-lookup"><span data-stu-id="70ef8-166">Time the report was last modified.</span></span> <span data-ttu-id="70ef8-167">Tidsformatet är yyyy-MM-ddTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="70ef8-167">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="70ef8-168">executeNow</span><span class="sxs-lookup"><span data-stu-id="70ef8-168">executeNow</span></span>     |    <span data-ttu-id="70ef8-169">ExecuteNow-flaggan som angetts när rapporten skapades</span><span class="sxs-lookup"><span data-stu-id="70ef8-169">ExecuteNow flag set at the time the report was created</span></span>    |
|    <span data-ttu-id="70ef8-170">StartTime</span><span class="sxs-lookup"><span data-stu-id="70ef8-170">StartTime</span></span>     |    <span data-ttu-id="70ef8-171">Tidskörningen börjar.</span><span class="sxs-lookup"><span data-stu-id="70ef8-171">Time execution will begin.</span></span> <span data-ttu-id="70ef8-172">Tidsformatet är yyyy-MM-ddTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="70ef8-172">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="70ef8-173">ReportStatus</span><span class="sxs-lookup"><span data-stu-id="70ef8-173">ReportStatus</span></span>     |    <span data-ttu-id="70ef8-174">Status för rapportkörningen.</span><span class="sxs-lookup"><span data-stu-id="70ef8-174">Status of the report execution.</span></span> <span data-ttu-id="70ef8-175">Möjliga värden är Pausad, Aktiv och Inaktiv.</span><span class="sxs-lookup"><span data-stu-id="70ef8-175">The possible values are Paused, Active, and Inactive.</span></span>     |
|    <span data-ttu-id="70ef8-176">RecurrenceInterval</span><span class="sxs-lookup"><span data-stu-id="70ef8-176">RecurrenceInterval</span></span>     |    <span data-ttu-id="70ef8-177">Upprepningsintervall som angavs när rapporten skapades</span><span class="sxs-lookup"><span data-stu-id="70ef8-177">Recurrence interval provided during report creation</span></span>     |
|    <span data-ttu-id="70ef8-178">RecurrenceCount</span><span class="sxs-lookup"><span data-stu-id="70ef8-178">RecurrenceCount</span></span>     |    <span data-ttu-id="70ef8-179">Antal upprepningar som angavs när rapporten skapades</span><span class="sxs-lookup"><span data-stu-id="70ef8-179">Recurrence count provided during report creation</span></span>     |
|    <span data-ttu-id="70ef8-180">CallbackUrl</span><span class="sxs-lookup"><span data-stu-id="70ef8-180">CallbackUrl</span></span>     |    <span data-ttu-id="70ef8-181">Motringning-URL som anges i begäran</span><span class="sxs-lookup"><span data-stu-id="70ef8-181">Callback URL provided in the request</span></span>     |
|    <span data-ttu-id="70ef8-182">CallbackMethod</span><span class="sxs-lookup"><span data-stu-id="70ef8-182">CallbackMethod</span></span>    |    <span data-ttu-id="70ef8-183">Återanropsmetod som anges i begäran</span><span class="sxs-lookup"><span data-stu-id="70ef8-183">Callback method provided in the request</span></span>    |
|    <span data-ttu-id="70ef8-184">Format</span><span class="sxs-lookup"><span data-stu-id="70ef8-184">Format</span></span>     |    <span data-ttu-id="70ef8-185">Format för rapportfilerna</span><span class="sxs-lookup"><span data-stu-id="70ef8-185">Format of the report files</span></span>     |
|    <span data-ttu-id="70ef8-186">TotalCount</span><span class="sxs-lookup"><span data-stu-id="70ef8-186">TotalCount</span></span>     |    <span data-ttu-id="70ef8-187">Antal datauppsättningar i värdematrisen</span><span class="sxs-lookup"><span data-stu-id="70ef8-187">Number of datasets in the Value array</span></span>     |
|    <span data-ttu-id="70ef8-188">Meddelande</span><span class="sxs-lookup"><span data-stu-id="70ef8-188">Message</span></span>     |    <span data-ttu-id="70ef8-189">Statusmeddelande från körningen av API:et</span><span class="sxs-lookup"><span data-stu-id="70ef8-189">Status message from the execution of the API</span></span>     |
|    <span data-ttu-id="70ef8-190">StatusCode</span><span class="sxs-lookup"><span data-stu-id="70ef8-190">StatusCode</span></span>     |    <span data-ttu-id="70ef8-191">Resultatkod.</span><span class="sxs-lookup"><span data-stu-id="70ef8-191">Result Code.</span></span> <span data-ttu-id="70ef8-192">Möjliga värden är 200, 400, 401, 403, 500</span><span class="sxs-lookup"><span data-stu-id="70ef8-192">The possible values are 200, 400, 401, 403, 500</span></span>     |
|        |        |