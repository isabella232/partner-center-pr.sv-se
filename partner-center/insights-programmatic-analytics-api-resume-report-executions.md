---
title: Återuppta API för rapportkörning – Insights data
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Använd det här API:et för att återuppta körningen av pausade rapporter i Partner Center-insikter.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: 1372823425f3aefd025ffc3441623c1ceee34e1e
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 07/16/2021
ms.locfileid: "114377195"
---
# <a name="resume-report-executions-api"></a><span data-ttu-id="d5c64-103">ÅTERUPPTA API för rapportkörningar</span><span class="sxs-lookup"><span data-stu-id="d5c64-103">Resume report executions API</span></span>

<span data-ttu-id="d5c64-104">Vid körning återupptar detta API den schemalagda körningen av en pausad rapport.</span><span class="sxs-lookup"><span data-stu-id="d5c64-104">On execution, this API resumes the scheduled execution of a paused report.</span></span>

<span data-ttu-id="d5c64-105">**Begärandesyntax**</span><span class="sxs-lookup"><span data-stu-id="d5c64-105">**Request syntax**</span></span>

|    <span data-ttu-id="d5c64-106">Metod</span><span class="sxs-lookup"><span data-stu-id="d5c64-106">Method</span></span>    |    <span data-ttu-id="d5c64-107">URI för förfrågan</span><span class="sxs-lookup"><span data-stu-id="d5c64-107">Request URI</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="d5c64-108">PUT</span><span class="sxs-lookup"><span data-stu-id="d5c64-108">PUT</span></span>    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport/resume/{ReportID}`    |
|        |        |

<span data-ttu-id="d5c64-109">**Begärandehuvud**</span><span class="sxs-lookup"><span data-stu-id="d5c64-109">**Request header**</span></span>

|    <span data-ttu-id="d5c64-110">Huvud</span><span class="sxs-lookup"><span data-stu-id="d5c64-110">Header</span></span>    |    <span data-ttu-id="d5c64-111">Typ</span><span class="sxs-lookup"><span data-stu-id="d5c64-111">Type</span></span>    |    <span data-ttu-id="d5c64-112">Description</span><span class="sxs-lookup"><span data-stu-id="d5c64-112">Description</span></span>    |
|    ----    |    ----    |    ----    |
|    <span data-ttu-id="d5c64-113">Auktorisering</span><span class="sxs-lookup"><span data-stu-id="d5c64-113">Authorization</span></span>    |    <span data-ttu-id="d5c64-114">sträng</span><span class="sxs-lookup"><span data-stu-id="d5c64-114">string</span></span>    |    <span data-ttu-id="d5c64-115">Krävs.</span><span class="sxs-lookup"><span data-stu-id="d5c64-115">Required.</span></span> <span data-ttu-id="d5c64-116">Åtkomsttoken Azure Active Directory (AAD) i formuläret`Bearer <token>`</span><span class="sxs-lookup"><span data-stu-id="d5c64-116">The Azure Active Directory (AAD) access token in the form `Bearer <token>`</span></span>    |
|    <span data-ttu-id="d5c64-117">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d5c64-117">Content-Type</span></span>    |    <span data-ttu-id="d5c64-118">sträng</span><span class="sxs-lookup"><span data-stu-id="d5c64-118">string</span></span>    |    `Application/JSON`    |
|        |        |        |

<span data-ttu-id="d5c64-119">**Sökvägsparameter**</span><span class="sxs-lookup"><span data-stu-id="d5c64-119">**Path parameter**</span></span>

|    <span data-ttu-id="d5c64-120">Parameternamn</span><span class="sxs-lookup"><span data-stu-id="d5c64-120">Parameter Name</span></span>    |    <span data-ttu-id="d5c64-121">Typ</span><span class="sxs-lookup"><span data-stu-id="d5c64-121">Type</span></span>    |    <span data-ttu-id="d5c64-122">Obligatorisk</span><span class="sxs-lookup"><span data-stu-id="d5c64-122">Required</span></span>    |    <span data-ttu-id="d5c64-123">Beskrivning</span><span class="sxs-lookup"><span data-stu-id="d5c64-123">Description</span></span>    |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="d5c64-124">reportId</span><span class="sxs-lookup"><span data-stu-id="d5c64-124">reportId</span></span>     |    <span data-ttu-id="d5c64-125">sträng</span><span class="sxs-lookup"><span data-stu-id="d5c64-125">string</span></span>    |    <span data-ttu-id="d5c64-126">No</span><span class="sxs-lookup"><span data-stu-id="d5c64-126">No</span></span>    |    <span data-ttu-id="d5c64-127">ID för den rapport som ändras</span><span class="sxs-lookup"><span data-stu-id="d5c64-127">ID of the report being modified</span></span>     |
|        |        |        |        |

<span data-ttu-id="d5c64-128">**Frågeparameter**</span><span class="sxs-lookup"><span data-stu-id="d5c64-128">**Query parameter**</span></span>

<span data-ttu-id="d5c64-129">Ingen</span><span class="sxs-lookup"><span data-stu-id="d5c64-129">None</span></span>

<span data-ttu-id="d5c64-130">**Begära nyttolast**</span><span class="sxs-lookup"><span data-stu-id="d5c64-130">**Request payload**</span></span>

<span data-ttu-id="d5c64-131">Ingen</span><span class="sxs-lookup"><span data-stu-id="d5c64-131">None</span></span>

<span data-ttu-id="d5c64-132">**Ordlista**</span><span class="sxs-lookup"><span data-stu-id="d5c64-132">**Glossary**</span></span>

<span data-ttu-id="d5c64-133">Ingen</span><span class="sxs-lookup"><span data-stu-id="d5c64-133">None</span></span>

<span data-ttu-id="d5c64-134">**Response**</span><span class="sxs-lookup"><span data-stu-id="d5c64-134">**Response**</span></span>

<span data-ttu-id="d5c64-135">Svarsnyttolasten är strukturerad på följande sätt:</span><span class="sxs-lookup"><span data-stu-id="d5c64-135">The response payload is structured as follows:</span></span>

<span data-ttu-id="d5c64-136">Svarskod: 200, 400, 401, 403, 404, 500</span><span class="sxs-lookup"><span data-stu-id="d5c64-136">Response code: 200, 400, 401, 403, 404, 500</span></span>

<span data-ttu-id="d5c64-137">Exempel på nyttolast för svar:</span><span class="sxs-lookup"><span data-stu-id="d5c64-137">Response payload example:</span></span>

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
      "ExecuteNow": true, 
      "StartTime": "string", 
      "ReportStatus": "string", 
      "RecurrenceInterval": 0, 
      "RecurrenceCount": 0, 
      "CallbackUrl": "string", 
      "CallbackMethod": "string", 
      "Format": "string" 
    } 
  ], 
  "TotalCount": 0, 
  "Message": "string", 
  "StatusCode": 0, 
} 
```

<span data-ttu-id="d5c64-138">**Ordlista**</span><span class="sxs-lookup"><span data-stu-id="d5c64-138">**Glossary**</span></span>

<span data-ttu-id="d5c64-139">Den här tabellen definierar nyckelelementen i svaret:</span><span class="sxs-lookup"><span data-stu-id="d5c64-139">This table defines the key elements in the response:</span></span>

|    <span data-ttu-id="d5c64-140">Parameter</span><span class="sxs-lookup"><span data-stu-id="d5c64-140">Parameter</span></span>    |    <span data-ttu-id="d5c64-141">Beskrivning</span><span class="sxs-lookup"><span data-stu-id="d5c64-141">Description</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="d5c64-142">ReportId</span><span class="sxs-lookup"><span data-stu-id="d5c64-142">ReportId</span></span>     |    <span data-ttu-id="d5c64-143">Universell unik identifierare (UUID) för den återupptagit rapporten</span><span class="sxs-lookup"><span data-stu-id="d5c64-143">Universally unique identifier (UUID) of the resumed report</span></span>     |
|    <span data-ttu-id="d5c64-144">ReportName</span><span class="sxs-lookup"><span data-stu-id="d5c64-144">ReportName</span></span>     |    <span data-ttu-id="d5c64-145">Namn som ges till rapporten när den skapas</span><span class="sxs-lookup"><span data-stu-id="d5c64-145">Name given to the report during creation</span></span>     |
|    <span data-ttu-id="d5c64-146">Description</span><span class="sxs-lookup"><span data-stu-id="d5c64-146">Description</span></span>     |    <span data-ttu-id="d5c64-147">Beskrivning som ges när rapporten skapas</span><span class="sxs-lookup"><span data-stu-id="d5c64-147">Description given during creation of the report</span></span>     |
|    <span data-ttu-id="d5c64-148">QueryId</span><span class="sxs-lookup"><span data-stu-id="d5c64-148">QueryId</span></span>     |    <span data-ttu-id="d5c64-149">Fråge-ID som skickades när rapporten skapades</span><span class="sxs-lookup"><span data-stu-id="d5c64-149">Query ID passed at the time the report was created</span></span>     |
|    <span data-ttu-id="d5c64-150">Söka i data</span><span class="sxs-lookup"><span data-stu-id="d5c64-150">Query</span></span>     |    <span data-ttu-id="d5c64-151">Frågetext som ska köras för den här rapporten</span><span class="sxs-lookup"><span data-stu-id="d5c64-151">Query text that will be executed for this report</span></span>     |
|    <span data-ttu-id="d5c64-152">Användare</span><span class="sxs-lookup"><span data-stu-id="d5c64-152">User</span></span>     |    <span data-ttu-id="d5c64-153">Användar-ID som används för att skapa rapporten</span><span class="sxs-lookup"><span data-stu-id="d5c64-153">User ID used to create the report</span></span>     |
|    <span data-ttu-id="d5c64-154">CreatedTime</span><span class="sxs-lookup"><span data-stu-id="d5c64-154">CreatedTime</span></span>     |    <span data-ttu-id="d5c64-155">Tid då rapporten skapades.</span><span class="sxs-lookup"><span data-stu-id="d5c64-155">Time the report was created.</span></span> <span data-ttu-id="d5c64-156">Tidsformatet är yyyy-MM-ddTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="d5c64-156">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="d5c64-157">ModifiedTime</span><span class="sxs-lookup"><span data-stu-id="d5c64-157">ModifiedTime</span></span>     |    <span data-ttu-id="d5c64-158">Tid då rapporten senast ändrades.</span><span class="sxs-lookup"><span data-stu-id="d5c64-158">Time the report was last modified.</span></span> <span data-ttu-id="d5c64-159">Tidsformatet är yyyy-MM-ddTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="d5c64-159">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="d5c64-160">ExecuteNow</span><span class="sxs-lookup"><span data-stu-id="d5c64-160">ExecuteNow</span></span>     |    <span data-ttu-id="d5c64-161">ExecuteNow-flaggan som angetts när rapporten skapades</span><span class="sxs-lookup"><span data-stu-id="d5c64-161">ExecuteNow flag set at the time the report was created</span></span>    |
|    <span data-ttu-id="d5c64-162">StartTime</span><span class="sxs-lookup"><span data-stu-id="d5c64-162">StartTime</span></span>     |    <span data-ttu-id="d5c64-163">Den tid då rapportkörningen börjar.</span><span class="sxs-lookup"><span data-stu-id="d5c64-163">Time the report execution will begin.</span></span> <span data-ttu-id="d5c64-164">Tidsformatet är yyyy-MM-ddTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="d5c64-164">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="d5c64-165">ReportStatus</span><span class="sxs-lookup"><span data-stu-id="d5c64-165">ReportStatus</span></span>     |    <span data-ttu-id="d5c64-166">Status för rapportkörningen.</span><span class="sxs-lookup"><span data-stu-id="d5c64-166">Status of the report execution.</span></span> <span data-ttu-id="d5c64-167">Möjliga värden är Pausad, Aktiv och Inaktiv.</span><span class="sxs-lookup"><span data-stu-id="d5c64-167">The possible values are Paused, Active, and Inactive.</span></span>     |
|    <span data-ttu-id="d5c64-168">RecurrenceInterval</span><span class="sxs-lookup"><span data-stu-id="d5c64-168">RecurrenceInterval</span></span>     |    <span data-ttu-id="d5c64-169">Upprepningsintervall som angavs när rapporten skapades</span><span class="sxs-lookup"><span data-stu-id="d5c64-169">Recurrence interval provided during report creation</span></span>     |
|    <span data-ttu-id="d5c64-170">RecurrenceCount</span><span class="sxs-lookup"><span data-stu-id="d5c64-170">RecurrenceCount</span></span>     |    <span data-ttu-id="d5c64-171">Antal upprepningar som angavs när rapporten skapades</span><span class="sxs-lookup"><span data-stu-id="d5c64-171">Recurrence count provided during report creation</span></span>     |
|    <span data-ttu-id="d5c64-172">CallbackUrl</span><span class="sxs-lookup"><span data-stu-id="d5c64-172">CallbackUrl</span></span>     |    <span data-ttu-id="d5c64-173">Motringning-URL som anges i begäran</span><span class="sxs-lookup"><span data-stu-id="d5c64-173">Callback URL provided in the request</span></span>     |
|    <span data-ttu-id="d5c64-174">CallbackMethod</span><span class="sxs-lookup"><span data-stu-id="d5c64-174">CallbackMethod</span></span>    |    <span data-ttu-id="d5c64-175">Återanropsmetod som anges i begäran</span><span class="sxs-lookup"><span data-stu-id="d5c64-175">Callback method provided in the request</span></span>    |
|    <span data-ttu-id="d5c64-176">Format</span><span class="sxs-lookup"><span data-stu-id="d5c64-176">Format</span></span>     |    <span data-ttu-id="d5c64-177">Format för rapportfilerna</span><span class="sxs-lookup"><span data-stu-id="d5c64-177">Format of the report files</span></span>     |
|    <span data-ttu-id="d5c64-178">TotalCount</span><span class="sxs-lookup"><span data-stu-id="d5c64-178">TotalCount</span></span>     |    <span data-ttu-id="d5c64-179">Antal datauppsättningar i värdematrisen</span><span class="sxs-lookup"><span data-stu-id="d5c64-179">Number of datasets in the Value array</span></span>     |
|    <span data-ttu-id="d5c64-180">Meddelande</span><span class="sxs-lookup"><span data-stu-id="d5c64-180">Message</span></span>     |    <span data-ttu-id="d5c64-181">Statusmeddelande från körningen av API:et</span><span class="sxs-lookup"><span data-stu-id="d5c64-181">Status message from the execution of the API</span></span>     |
|    <span data-ttu-id="d5c64-182">StatusCode</span><span class="sxs-lookup"><span data-stu-id="d5c64-182">StatusCode</span></span>     |    <span data-ttu-id="d5c64-183">Resultatkod.</span><span class="sxs-lookup"><span data-stu-id="d5c64-183">Result Code.</span></span> <span data-ttu-id="d5c64-184">Möjliga värden är 200, 400, 401, 403, 500</span><span class="sxs-lookup"><span data-stu-id="d5c64-184">The possible values are 200, 400, 401, 403, 500</span></span>     |
|        |        |
