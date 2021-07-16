---
title: Pausa API för rapportkörning – Insights data
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Använd det här API:et för att pausa körningen av alla rapporter i PartnerCenter-insikter.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: 1e490a6d5120d729f0ea4979a201e9a80ba2991c
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 07/16/2021
ms.locfileid: "114377201"
---
# <a name="pause-report-executions-api"></a><span data-ttu-id="8c388-103">Pausa API för rapportkörningar</span><span class="sxs-lookup"><span data-stu-id="8c388-103">Pause report executions API</span></span>

<span data-ttu-id="8c388-104">Vid körning pausar detta API den schemalagda körningen av rapporter.</span><span class="sxs-lookup"><span data-stu-id="8c388-104">On execution, this API pauses the scheduled execution of reports.</span></span>

<span data-ttu-id="8c388-105">**Begärandesyntax**</span><span class="sxs-lookup"><span data-stu-id="8c388-105">**Request syntax**</span></span>

|    <span data-ttu-id="8c388-106">Metod</span><span class="sxs-lookup"><span data-stu-id="8c388-106">Method</span></span>    |    <span data-ttu-id="8c388-107">URI för förfrågan</span><span class="sxs-lookup"><span data-stu-id="8c388-107">Request URI</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="8c388-108">PUT</span><span class="sxs-lookup"><span data-stu-id="8c388-108">PUT</span></span>    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport/pause/{ReportID}`    |
|        |        |

<span data-ttu-id="8c388-109">**Begärandehuvud**</span><span class="sxs-lookup"><span data-stu-id="8c388-109">**Request header**</span></span>

|    <span data-ttu-id="8c388-110">Huvud</span><span class="sxs-lookup"><span data-stu-id="8c388-110">Header</span></span>    |    <span data-ttu-id="8c388-111">Typ</span><span class="sxs-lookup"><span data-stu-id="8c388-111">Type</span></span>    |    <span data-ttu-id="8c388-112">Description</span><span class="sxs-lookup"><span data-stu-id="8c388-112">Description</span></span>    |
|    ----    |    ----    |    ----    |
|    <span data-ttu-id="8c388-113">Auktorisering</span><span class="sxs-lookup"><span data-stu-id="8c388-113">Authorization</span></span>    |    <span data-ttu-id="8c388-114">sträng</span><span class="sxs-lookup"><span data-stu-id="8c388-114">string</span></span>    |    <span data-ttu-id="8c388-115">Krävs.</span><span class="sxs-lookup"><span data-stu-id="8c388-115">Required.</span></span> <span data-ttu-id="8c388-116">Åtkomsttoken Azure Active Directory (AAD) i formuläret`Bearer <token>`</span><span class="sxs-lookup"><span data-stu-id="8c388-116">The Azure Active Directory (AAD) access token in the form `Bearer <token>`</span></span>    |
|    <span data-ttu-id="8c388-117">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8c388-117">Content-Type</span></span>    |    <span data-ttu-id="8c388-118">sträng</span><span class="sxs-lookup"><span data-stu-id="8c388-118">string</span></span>    |    `Application/JSON`    |
|        |        |        |

<span data-ttu-id="8c388-119">**Sökvägsparameter**</span><span class="sxs-lookup"><span data-stu-id="8c388-119">**Path parameter**</span></span>

|    <span data-ttu-id="8c388-120">Parameternamn</span><span class="sxs-lookup"><span data-stu-id="8c388-120">Parameter Name</span></span>    |    <span data-ttu-id="8c388-121">Typ</span><span class="sxs-lookup"><span data-stu-id="8c388-121">Type</span></span>    |    <span data-ttu-id="8c388-122">Obligatorisk</span><span class="sxs-lookup"><span data-stu-id="8c388-122">Required</span></span>    |    <span data-ttu-id="8c388-123">Beskrivning</span><span class="sxs-lookup"><span data-stu-id="8c388-123">Description</span></span>    |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="8c388-124">reportId</span><span class="sxs-lookup"><span data-stu-id="8c388-124">reportId</span></span>     |    <span data-ttu-id="8c388-125">sträng</span><span class="sxs-lookup"><span data-stu-id="8c388-125">string</span></span>    |    <span data-ttu-id="8c388-126">No</span><span class="sxs-lookup"><span data-stu-id="8c388-126">No</span></span>    |    <span data-ttu-id="8c388-127">ID för den rapport som ändras</span><span class="sxs-lookup"><span data-stu-id="8c388-127">ID of the report being modified</span></span>     |
|        |        |        |        |

<span data-ttu-id="8c388-128">**Frågeparameter**</span><span class="sxs-lookup"><span data-stu-id="8c388-128">**Query parameter**</span></span>

<span data-ttu-id="8c388-129">Ingen</span><span class="sxs-lookup"><span data-stu-id="8c388-129">None</span></span>

<span data-ttu-id="8c388-130">**Begära nyttolast**</span><span class="sxs-lookup"><span data-stu-id="8c388-130">**Request payload**</span></span>

<span data-ttu-id="8c388-131">Ingen</span><span class="sxs-lookup"><span data-stu-id="8c388-131">None</span></span>

<span data-ttu-id="8c388-132">**Ordlista**</span><span class="sxs-lookup"><span data-stu-id="8c388-132">**Glossary**</span></span>

<span data-ttu-id="8c388-133">Ingen</span><span class="sxs-lookup"><span data-stu-id="8c388-133">None</span></span>

<span data-ttu-id="8c388-134">**Response**</span><span class="sxs-lookup"><span data-stu-id="8c388-134">**Response**</span></span>

<span data-ttu-id="8c388-135">Svarsnyttolasten är strukturerad på följande sätt:</span><span class="sxs-lookup"><span data-stu-id="8c388-135">The response payload is structured as follows:</span></span>

<span data-ttu-id="8c388-136">Svarskod: 200, 400, 401, 403, 404, 500</span><span class="sxs-lookup"><span data-stu-id="8c388-136">Response code: 200, 400, 401, 403, 404, 500</span></span>

<span data-ttu-id="8c388-137">Exempel på nyttolast för svar:</span><span class="sxs-lookup"><span data-stu-id="8c388-137">Response payload example:</span></span>

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

<span data-ttu-id="8c388-138">**Ordlista**</span><span class="sxs-lookup"><span data-stu-id="8c388-138">**Glossary**</span></span>

<span data-ttu-id="8c388-139">Den här tabellen definierar nyckelelementen i svaret:</span><span class="sxs-lookup"><span data-stu-id="8c388-139">This table defines the key elements in the response:</span></span>

|    <span data-ttu-id="8c388-140">Parameter</span><span class="sxs-lookup"><span data-stu-id="8c388-140">Parameter</span></span>    |    <span data-ttu-id="8c388-141">Beskrivning</span><span class="sxs-lookup"><span data-stu-id="8c388-141">Description</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="8c388-142">ReportId</span><span class="sxs-lookup"><span data-stu-id="8c388-142">ReportId</span></span>     |    <span data-ttu-id="8c388-143">Universell unik identifierare (UUID) för den pausade rapporten</span><span class="sxs-lookup"><span data-stu-id="8c388-143">Universally unique identifier (UUID) of the paused report</span></span>     |
|    <span data-ttu-id="8c388-144">ReportName</span><span class="sxs-lookup"><span data-stu-id="8c388-144">ReportName</span></span>     |    <span data-ttu-id="8c388-145">Namn som ges till rapporten när den skapades</span><span class="sxs-lookup"><span data-stu-id="8c388-145">Name given to the report during creation</span></span>     |
|    <span data-ttu-id="8c388-146">Description</span><span class="sxs-lookup"><span data-stu-id="8c388-146">Description</span></span>     |    <span data-ttu-id="8c388-147">Beskrivning som anges när rapporten skapas</span><span class="sxs-lookup"><span data-stu-id="8c388-147">Description given during creation of the report</span></span>     |
|    <span data-ttu-id="8c388-148">QueryId</span><span class="sxs-lookup"><span data-stu-id="8c388-148">QueryId</span></span>     |    <span data-ttu-id="8c388-149">Fråge-ID som skickades när rapporten skapades</span><span class="sxs-lookup"><span data-stu-id="8c388-149">Query ID passed at the time the report was created</span></span>     |
|    <span data-ttu-id="8c388-150">Söka i data</span><span class="sxs-lookup"><span data-stu-id="8c388-150">Query</span></span>     |    <span data-ttu-id="8c388-151">Frågetext som ska köras för den här rapporten</span><span class="sxs-lookup"><span data-stu-id="8c388-151">Query text that will be executed for this report</span></span>     |
|    <span data-ttu-id="8c388-152">Användare</span><span class="sxs-lookup"><span data-stu-id="8c388-152">User</span></span>     |    <span data-ttu-id="8c388-153">Användar-ID som används för att skapa rapporten</span><span class="sxs-lookup"><span data-stu-id="8c388-153">User ID used to create the report</span></span>     |
|    <span data-ttu-id="8c388-154">CreatedTime</span><span class="sxs-lookup"><span data-stu-id="8c388-154">CreatedTime</span></span>     |    <span data-ttu-id="8c388-155">Tiden då rapporten skapades.</span><span class="sxs-lookup"><span data-stu-id="8c388-155">Time the report was created.</span></span> <span data-ttu-id="8c388-156">Tidsformatet är yyyy-MM-ddTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="8c388-156">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="8c388-157">ModifiedTime</span><span class="sxs-lookup"><span data-stu-id="8c388-157">ModifiedTime</span></span>     |    <span data-ttu-id="8c388-158">Tid då rapporten senast ändrades.</span><span class="sxs-lookup"><span data-stu-id="8c388-158">Time the report was last modified.</span></span> <span data-ttu-id="8c388-159">Tidsformatet är yyyy-MM-ddTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="8c388-159">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="8c388-160">ExecuteNow</span><span class="sxs-lookup"><span data-stu-id="8c388-160">ExecuteNow</span></span>     |    <span data-ttu-id="8c388-161">ExecuteNow-flaggan som angetts när rapporten skapades</span><span class="sxs-lookup"><span data-stu-id="8c388-161">ExecuteNow flag set at the time the report was created</span></span>     |
|    <span data-ttu-id="8c388-162">StartTime</span><span class="sxs-lookup"><span data-stu-id="8c388-162">StartTime</span></span>     |    <span data-ttu-id="8c388-163">Den tid då rapportkörningen börjar.</span><span class="sxs-lookup"><span data-stu-id="8c388-163">Time the report execution will begin.</span></span> <span data-ttu-id="8c388-164">Tidsformatet är yyyy-MM-ddTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="8c388-164">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="8c388-165">ReportStatus</span><span class="sxs-lookup"><span data-stu-id="8c388-165">ReportStatus</span></span>     |    <span data-ttu-id="8c388-166">Status för rapportkörningen.</span><span class="sxs-lookup"><span data-stu-id="8c388-166">Status of the report execution.</span></span> <span data-ttu-id="8c388-167">Möjliga värden är Pausad, Aktiv och Inaktiv.</span><span class="sxs-lookup"><span data-stu-id="8c388-167">The possible values are Paused, Active, and Inactive.</span></span>     |
|    <span data-ttu-id="8c388-168">RecurrenceInterval</span><span class="sxs-lookup"><span data-stu-id="8c388-168">RecurrenceInterval</span></span>     |    <span data-ttu-id="8c388-169">Upprepningsintervall som anges när rapporten skapas</span><span class="sxs-lookup"><span data-stu-id="8c388-169">Recurrence interval provided during report creation</span></span>     |
|    <span data-ttu-id="8c388-170">RecurrenceCount</span><span class="sxs-lookup"><span data-stu-id="8c388-170">RecurrenceCount</span></span>     |    <span data-ttu-id="8c388-171">Antal upprepningar som anges när rapporten skapas</span><span class="sxs-lookup"><span data-stu-id="8c388-171">Recurrence count provided during report creation</span></span>     |
|    <span data-ttu-id="8c388-172">CallbackUrl</span><span class="sxs-lookup"><span data-stu-id="8c388-172">CallbackUrl</span></span>     |    <span data-ttu-id="8c388-173">Motringning-URL som anges i begäran</span><span class="sxs-lookup"><span data-stu-id="8c388-173">Callback URL provided in the request</span></span>     |
|    <span data-ttu-id="8c388-174">CallbackMethod</span><span class="sxs-lookup"><span data-stu-id="8c388-174">CallbackMethod</span></span>    |    <span data-ttu-id="8c388-175">Återanropsmetod som anges i begäran</span><span class="sxs-lookup"><span data-stu-id="8c388-175">Callback method provided in the request</span></span>    |
|    <span data-ttu-id="8c388-176">Format</span><span class="sxs-lookup"><span data-stu-id="8c388-176">Format</span></span>     |    <span data-ttu-id="8c388-177">Format för rapportfilerna</span><span class="sxs-lookup"><span data-stu-id="8c388-177">Format of the report files</span></span>     |
|    <span data-ttu-id="8c388-178">TotalCount</span><span class="sxs-lookup"><span data-stu-id="8c388-178">TotalCount</span></span>     |    <span data-ttu-id="8c388-179">Antal datauppsättningar i värdematrisen</span><span class="sxs-lookup"><span data-stu-id="8c388-179">Number of datasets in the Value array</span></span>     |
|    <span data-ttu-id="8c388-180">Meddelande</span><span class="sxs-lookup"><span data-stu-id="8c388-180">Message</span></span>     |    <span data-ttu-id="8c388-181">Statusmeddelande från körningen av API:et</span><span class="sxs-lookup"><span data-stu-id="8c388-181">Status message from the execution of the API</span></span>     |
|    <span data-ttu-id="8c388-182">StatusCode</span><span class="sxs-lookup"><span data-stu-id="8c388-182">StatusCode</span></span>     |    <span data-ttu-id="8c388-183">Resultatkod.</span><span class="sxs-lookup"><span data-stu-id="8c388-183">Result Code.</span></span> <span data-ttu-id="8c388-184">Möjliga värden är 200, 400, 401, 403, 500</span><span class="sxs-lookup"><span data-stu-id="8c388-184">The possible values are 200, 400, 401, 403, 500</span></span>     |
|        |        |
