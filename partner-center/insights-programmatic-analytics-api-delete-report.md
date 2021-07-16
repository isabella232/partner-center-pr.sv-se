---
title: Ta bort rapport-API – Insights data
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Använd det här API:et för att ta bort alla rapporter i Partner Center-insikter.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: e060104f8f09f69c213ab1b22d4be08d58babced
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 07/16/2021
ms.locfileid: "114377214"
---
# <a name="delete-report-api"></a><span data-ttu-id="0920d-103">Ta bort rapport-API</span><span class="sxs-lookup"><span data-stu-id="0920d-103">Delete report API</span></span>

<span data-ttu-id="0920d-104">Vid körning tar det här API:et bort alla rapport- och rapportkörningsposter.</span><span class="sxs-lookup"><span data-stu-id="0920d-104">On execution, this API deletes all of the report and report execution records.</span></span>

<span data-ttu-id="0920d-105">**Begärandesyntax**</span><span class="sxs-lookup"><span data-stu-id="0920d-105">**Request syntax**</span></span>

|    <span data-ttu-id="0920d-106">Metod</span><span class="sxs-lookup"><span data-stu-id="0920d-106">Method</span></span>    |    <span data-ttu-id="0920d-107">URI för förfrågan</span><span class="sxs-lookup"><span data-stu-id="0920d-107">Request URI</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="0920d-108">DELETE</span><span class="sxs-lookup"><span data-stu-id="0920d-108">DELETE</span></span>    |    ` https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport/{Report ID}`    |
|        |        |

<span data-ttu-id="0920d-109">**Begärandehuvud**</span><span class="sxs-lookup"><span data-stu-id="0920d-109">**Request header**</span></span>

|    <span data-ttu-id="0920d-110">Huvud</span><span class="sxs-lookup"><span data-stu-id="0920d-110">Header</span></span>    |    <span data-ttu-id="0920d-111">Typ</span><span class="sxs-lookup"><span data-stu-id="0920d-111">Type</span></span>    |    <span data-ttu-id="0920d-112">Description</span><span class="sxs-lookup"><span data-stu-id="0920d-112">Description</span></span>    |
|    ----    |    ----    |    ----    |
|    <span data-ttu-id="0920d-113">Auktorisering</span><span class="sxs-lookup"><span data-stu-id="0920d-113">Authorization</span></span>    |    <span data-ttu-id="0920d-114">sträng</span><span class="sxs-lookup"><span data-stu-id="0920d-114">string</span></span>    |    <span data-ttu-id="0920d-115">Krävs.</span><span class="sxs-lookup"><span data-stu-id="0920d-115">Required.</span></span> <span data-ttu-id="0920d-116">Åtkomsttoken Azure Active Directory (AAD) i formuläret`Bearer <token>`</span><span class="sxs-lookup"><span data-stu-id="0920d-116">The Azure Active Directory (AAD) access token in the form `Bearer <token>`</span></span>    |
|    <span data-ttu-id="0920d-117">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0920d-117">Content-Type</span></span>    |    <span data-ttu-id="0920d-118">sträng</span><span class="sxs-lookup"><span data-stu-id="0920d-118">string</span></span>    |    `Application/JSON`    |
|        |        |        |

<span data-ttu-id="0920d-119">**Sökvägsparameter**</span><span class="sxs-lookup"><span data-stu-id="0920d-119">**Path parameter**</span></span>

|    <span data-ttu-id="0920d-120">Parameternamn</span><span class="sxs-lookup"><span data-stu-id="0920d-120">Parameter Name</span></span>    |    <span data-ttu-id="0920d-121">Typ</span><span class="sxs-lookup"><span data-stu-id="0920d-121">Type</span></span>    |    <span data-ttu-id="0920d-122">Obligatorisk</span><span class="sxs-lookup"><span data-stu-id="0920d-122">Required</span></span>    |    <span data-ttu-id="0920d-123">Beskrivning</span><span class="sxs-lookup"><span data-stu-id="0920d-123">Description</span></span>    |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="0920d-124">reportId</span><span class="sxs-lookup"><span data-stu-id="0920d-124">reportId</span></span>     |    <span data-ttu-id="0920d-125">sträng</span><span class="sxs-lookup"><span data-stu-id="0920d-125">string</span></span>    |    <span data-ttu-id="0920d-126">No</span><span class="sxs-lookup"><span data-stu-id="0920d-126">No</span></span>    |    <span data-ttu-id="0920d-127">ID för rapporten som tas bort</span><span class="sxs-lookup"><span data-stu-id="0920d-127">ID of the report being deleted</span></span>    |
|        |        |        |        |

<span data-ttu-id="0920d-128">**Frågeparameter**</span><span class="sxs-lookup"><span data-stu-id="0920d-128">**Query parameter**</span></span>

<span data-ttu-id="0920d-129">Ingen</span><span class="sxs-lookup"><span data-stu-id="0920d-129">None</span></span>

<span data-ttu-id="0920d-130">**Begära nyttolast**</span><span class="sxs-lookup"><span data-stu-id="0920d-130">**Request payload**</span></span>

<span data-ttu-id="0920d-131">Ingen</span><span class="sxs-lookup"><span data-stu-id="0920d-131">None</span></span>

<span data-ttu-id="0920d-132">**Ordlista**</span><span class="sxs-lookup"><span data-stu-id="0920d-132">**Glossary**</span></span>

<span data-ttu-id="0920d-133">Ingen</span><span class="sxs-lookup"><span data-stu-id="0920d-133">None</span></span>

<span data-ttu-id="0920d-134">**Response**</span><span class="sxs-lookup"><span data-stu-id="0920d-134">**Response**</span></span>

<span data-ttu-id="0920d-135">Svarsnyttolasten är strukturerad på följande sätt:</span><span class="sxs-lookup"><span data-stu-id="0920d-135">The response payload is structured as follows:</span></span>

<span data-ttu-id="0920d-136">Svarskod: 200, 400, 401, 403, 404, 500</span><span class="sxs-lookup"><span data-stu-id="0920d-136">Response code: 200, 400, 401, 403, 404, 500</span></span>

<span data-ttu-id="0920d-137">Exempel på nyttolast för svar:</span><span class="sxs-lookup"><span data-stu-id="0920d-137">Response payload example:</span></span>

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

<span data-ttu-id="0920d-138">**Ordlista**</span><span class="sxs-lookup"><span data-stu-id="0920d-138">**Glossary**</span></span>

<span data-ttu-id="0920d-139">Den här tabellen definierar nyckelelementen i svaret:</span><span class="sxs-lookup"><span data-stu-id="0920d-139">This table defines the key elements in the response:</span></span>

|    <span data-ttu-id="0920d-140">Parameter</span><span class="sxs-lookup"><span data-stu-id="0920d-140">Parameter</span></span>    |    <span data-ttu-id="0920d-141">Beskrivning</span><span class="sxs-lookup"><span data-stu-id="0920d-141">Description</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="0920d-142">ReportId</span><span class="sxs-lookup"><span data-stu-id="0920d-142">ReportId</span></span>     |    <span data-ttu-id="0920d-143">Universell unik identifierare (UUID) för den borttagna rapporten</span><span class="sxs-lookup"><span data-stu-id="0920d-143">Universally unique identifier (UUID) of the deleted report</span></span>     |
|    <span data-ttu-id="0920d-144">ReportName</span><span class="sxs-lookup"><span data-stu-id="0920d-144">ReportName</span></span>     |    <span data-ttu-id="0920d-145">Namn som ges till rapporten när den skapas</span><span class="sxs-lookup"><span data-stu-id="0920d-145">Name given to the report during creation</span></span>     |
|    <span data-ttu-id="0920d-146">Description</span><span class="sxs-lookup"><span data-stu-id="0920d-146">Description</span></span>     |    <span data-ttu-id="0920d-147">Beskrivning som ges när rapporten skapas</span><span class="sxs-lookup"><span data-stu-id="0920d-147">Description given during creation of the report</span></span>     |
|    <span data-ttu-id="0920d-148">QueryId</span><span class="sxs-lookup"><span data-stu-id="0920d-148">QueryId</span></span>     |    <span data-ttu-id="0920d-149">Fråge-ID som skickades när rapporten skapades</span><span class="sxs-lookup"><span data-stu-id="0920d-149">Query ID passed at the time the report was created</span></span>     |
|    <span data-ttu-id="0920d-150">Söka i data</span><span class="sxs-lookup"><span data-stu-id="0920d-150">Query</span></span>     |    <span data-ttu-id="0920d-151">Frågetext som ska köras för den här rapporten</span><span class="sxs-lookup"><span data-stu-id="0920d-151">Query text that will be executed for this report</span></span>     |
|    <span data-ttu-id="0920d-152">Användare</span><span class="sxs-lookup"><span data-stu-id="0920d-152">User</span></span>     |    <span data-ttu-id="0920d-153">Användar-ID som används för att skapa rapporten</span><span class="sxs-lookup"><span data-stu-id="0920d-153">User ID used to create the report</span></span>     |
|    <span data-ttu-id="0920d-154">CreatedTime</span><span class="sxs-lookup"><span data-stu-id="0920d-154">CreatedTime</span></span>     |    <span data-ttu-id="0920d-155">Den tid då rapporten skapades.</span><span class="sxs-lookup"><span data-stu-id="0920d-155">Time the report was created.</span></span> <span data-ttu-id="0920d-156">Tidsformatet är yyyy-MM-ddTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="0920d-156">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="0920d-157">ModifiedTime</span><span class="sxs-lookup"><span data-stu-id="0920d-157">ModifiedTime</span></span>     |    <span data-ttu-id="0920d-158">Tid då rapporten senast ändrades.</span><span class="sxs-lookup"><span data-stu-id="0920d-158">Time the report was last modified.</span></span> <span data-ttu-id="0920d-159">Tidsformatet är yyyy-MM-ddTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="0920d-159">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="0920d-160">ExecuteNow</span><span class="sxs-lookup"><span data-stu-id="0920d-160">ExecuteNow</span></span>     |    <span data-ttu-id="0920d-161">ExecuteNow-flaggan som angetts när rapporten skapades</span><span class="sxs-lookup"><span data-stu-id="0920d-161">ExecuteNow flag set at the time the report was created</span></span>     |
|    <span data-ttu-id="0920d-162">StartTime</span><span class="sxs-lookup"><span data-stu-id="0920d-162">StartTime</span></span>     |    <span data-ttu-id="0920d-163">Den tid då rapportkörningen börjar.</span><span class="sxs-lookup"><span data-stu-id="0920d-163">Time the report execution will begin.</span></span> <span data-ttu-id="0920d-164">Tidsformatet är yyyy-MM-ddTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="0920d-164">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="0920d-165">ReportStatus</span><span class="sxs-lookup"><span data-stu-id="0920d-165">ReportStatus</span></span>     |    <span data-ttu-id="0920d-166">Status för rapportkörningen.</span><span class="sxs-lookup"><span data-stu-id="0920d-166">Status of the report execution.</span></span> <span data-ttu-id="0920d-167">Möjliga värden är Pausad, Aktiv och Inaktiv.</span><span class="sxs-lookup"><span data-stu-id="0920d-167">The possible values are Paused, Active, and Inactive.</span></span>     |
|    <span data-ttu-id="0920d-168">RecurrenceInterval</span><span class="sxs-lookup"><span data-stu-id="0920d-168">RecurrenceInterval</span></span>     |    <span data-ttu-id="0920d-169">Upprepningsintervall som angavs när rapporten skapades</span><span class="sxs-lookup"><span data-stu-id="0920d-169">Recurrence interval provided during report creation</span></span>     |
|    <span data-ttu-id="0920d-170">RecurrenceCount</span><span class="sxs-lookup"><span data-stu-id="0920d-170">RecurrenceCount</span></span>     |    <span data-ttu-id="0920d-171">Antal upprepningar som angavs när rapporten skapades</span><span class="sxs-lookup"><span data-stu-id="0920d-171">Recurrence count provided during report creation</span></span>     |
|    <span data-ttu-id="0920d-172">CallbackUrl</span><span class="sxs-lookup"><span data-stu-id="0920d-172">CallbackUrl</span></span>     |    <span data-ttu-id="0920d-173">Motringning-URL som anges i begäran</span><span class="sxs-lookup"><span data-stu-id="0920d-173">Callback URL provided in the request</span></span>     |
|    <span data-ttu-id="0920d-174">CallbackMethod</span><span class="sxs-lookup"><span data-stu-id="0920d-174">CallbackMethod</span></span>    |    <span data-ttu-id="0920d-175">Återanropsmetod som anges i begäran</span><span class="sxs-lookup"><span data-stu-id="0920d-175">Callback method provided in the request</span></span>    |
|    <span data-ttu-id="0920d-176">Format</span><span class="sxs-lookup"><span data-stu-id="0920d-176">Format</span></span>     |    <span data-ttu-id="0920d-177">Format för rapportfilerna</span><span class="sxs-lookup"><span data-stu-id="0920d-177">Format of the report files</span></span>     |
|    <span data-ttu-id="0920d-178">TotalCount</span><span class="sxs-lookup"><span data-stu-id="0920d-178">TotalCount</span></span>     |    <span data-ttu-id="0920d-179">Antal datauppsättningar i värdematrisen</span><span class="sxs-lookup"><span data-stu-id="0920d-179">Number of datasets in the Value array</span></span>     |
|    <span data-ttu-id="0920d-180">Meddelande</span><span class="sxs-lookup"><span data-stu-id="0920d-180">Message</span></span>     |    <span data-ttu-id="0920d-181">Statusmeddelande från körningen av API:et</span><span class="sxs-lookup"><span data-stu-id="0920d-181">Status message from the execution of the API</span></span>     |
|    <span data-ttu-id="0920d-182">StatusCode</span><span class="sxs-lookup"><span data-stu-id="0920d-182">StatusCode</span></span>     |    <span data-ttu-id="0920d-183">Resultatkod.</span><span class="sxs-lookup"><span data-stu-id="0920d-183">Result Code.</span></span> <span data-ttu-id="0920d-184">Möjliga värden är 200, 400, 401, 403, 500</span><span class="sxs-lookup"><span data-stu-id="0920d-184">The possible values are 200, 400, 401, 403, 500</span></span>     |
|        |        |
