---
title: Uppdatera rapport-API
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Använd det här API:et för att uppdatera rapportparametrar i Partner Center-insikter.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: c5ab1059e9be9b42918d268da6a6c1a3cbfe52af
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 07/16/2021
ms.locfileid: "114377178"
---
# <a name="update-report-api"></a><span data-ttu-id="e60c7-103">Uppdatera rapport-API</span><span class="sxs-lookup"><span data-stu-id="e60c7-103">Update report API</span></span>

<span data-ttu-id="e60c7-104">Det här API:et hjälper dig att ändra en rapportparameter.</span><span class="sxs-lookup"><span data-stu-id="e60c7-104">This API helps you modify a report parameter.</span></span>

<span data-ttu-id="e60c7-105">**Begärandesyntax**</span><span class="sxs-lookup"><span data-stu-id="e60c7-105">**Request syntax**</span></span>

|    <span data-ttu-id="e60c7-106">Metod</span><span class="sxs-lookup"><span data-stu-id="e60c7-106">Method</span></span>    |    <span data-ttu-id="e60c7-107">URI för förfrågan</span><span class="sxs-lookup"><span data-stu-id="e60c7-107">Request URI</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="e60c7-108">PUT</span><span class="sxs-lookup"><span data-stu-id="e60c7-108">PUT</span></span>    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport/{Report ID}`    |
|        |        |

<span data-ttu-id="e60c7-109">**Begärandehuvud**</span><span class="sxs-lookup"><span data-stu-id="e60c7-109">**Request header**</span></span>

|    <span data-ttu-id="e60c7-110">Huvud</span><span class="sxs-lookup"><span data-stu-id="e60c7-110">Header</span></span>    |    <span data-ttu-id="e60c7-111">Typ</span><span class="sxs-lookup"><span data-stu-id="e60c7-111">Type</span></span>    |    <span data-ttu-id="e60c7-112">Description</span><span class="sxs-lookup"><span data-stu-id="e60c7-112">Description</span></span>    |
|    ----    |    ----    |    ----    |
|    <span data-ttu-id="e60c7-113">Auktorisering</span><span class="sxs-lookup"><span data-stu-id="e60c7-113">Authorization</span></span>    |    <span data-ttu-id="e60c7-114">sträng</span><span class="sxs-lookup"><span data-stu-id="e60c7-114">string</span></span>    |    <span data-ttu-id="e60c7-115">Krävs.</span><span class="sxs-lookup"><span data-stu-id="e60c7-115">Required.</span></span> <span data-ttu-id="e60c7-116">Åtkomsttoken Azure Active Directory (AAD) i formuläret`Bearer <token>`</span><span class="sxs-lookup"><span data-stu-id="e60c7-116">The Azure Active Directory (AAD) access token in the form `Bearer <token>`</span></span>    |
|    <span data-ttu-id="e60c7-117">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e60c7-117">Content-Type</span></span>    |    <span data-ttu-id="e60c7-118">sträng</span><span class="sxs-lookup"><span data-stu-id="e60c7-118">string</span></span>    |    `Application/JSON`    |
|        |        |        |

<span data-ttu-id="e60c7-119">**Sökvägsparameter**</span><span class="sxs-lookup"><span data-stu-id="e60c7-119">**Path parameter**</span></span>

|    <span data-ttu-id="e60c7-120">Parameternamn</span><span class="sxs-lookup"><span data-stu-id="e60c7-120">Parameter Name</span></span>    |    <span data-ttu-id="e60c7-121">Typ</span><span class="sxs-lookup"><span data-stu-id="e60c7-121">Type</span></span>    |    <span data-ttu-id="e60c7-122">Obligatorisk</span><span class="sxs-lookup"><span data-stu-id="e60c7-122">Required</span></span>    |    <span data-ttu-id="e60c7-123">Beskrivning</span><span class="sxs-lookup"><span data-stu-id="e60c7-123">Description</span></span>    |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="e60c7-124">reportId</span><span class="sxs-lookup"><span data-stu-id="e60c7-124">reportId</span></span>     |    <span data-ttu-id="e60c7-125">sträng</span><span class="sxs-lookup"><span data-stu-id="e60c7-125">string</span></span>    |    <span data-ttu-id="e60c7-126">No</span><span class="sxs-lookup"><span data-stu-id="e60c7-126">No</span></span>    |    <span data-ttu-id="e60c7-127">ID för den rapport som ändras</span><span class="sxs-lookup"><span data-stu-id="e60c7-127">ID of the report being modified</span></span>     |
|        |        |        |        |

<span data-ttu-id="e60c7-128">**Frågeparameter**</span><span class="sxs-lookup"><span data-stu-id="e60c7-128">**Query parameter**</span></span>

<span data-ttu-id="e60c7-129">Ingen</span><span class="sxs-lookup"><span data-stu-id="e60c7-129">None</span></span>

<span data-ttu-id="e60c7-130">**Begära nyttolast**</span><span class="sxs-lookup"><span data-stu-id="e60c7-130">**Request payload**</span></span>

```json
{ 
  "ReportName": "string", 
  "Description": "string", 
  "StartTime": "string", 
  "RecurrenceInterval": 0, 
  "RecurrenceCount": 0, 
  "Format": "string", 
  "CallbackUrl": "string",
 "CallbackMethod": "string"
}
```

<span data-ttu-id="e60c7-131">**Ordlista**</span><span class="sxs-lookup"><span data-stu-id="e60c7-131">**Glossary**</span></span>

<span data-ttu-id="e60c7-132">I den här tabellen visas viktiga definitioner av element i svaret.</span><span class="sxs-lookup"><span data-stu-id="e60c7-132">This table lists the key definitions of elements in the response.</span></span>

|    <span data-ttu-id="e60c7-133">Parameter</span><span class="sxs-lookup"><span data-stu-id="e60c7-133">Parameter</span></span>    |    <span data-ttu-id="e60c7-134">Krävs</span><span class="sxs-lookup"><span data-stu-id="e60c7-134">Required</span></span>    |    <span data-ttu-id="e60c7-135">Beskrivning</span><span class="sxs-lookup"><span data-stu-id="e60c7-135">Description</span></span>    |    <span data-ttu-id="e60c7-136">Tillåtna värden</span><span class="sxs-lookup"><span data-stu-id="e60c7-136">Allowed Values</span></span>    |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="e60c7-137">ReportName</span><span class="sxs-lookup"><span data-stu-id="e60c7-137">ReportName</span></span>     |    <span data-ttu-id="e60c7-138">Ja</span><span class="sxs-lookup"><span data-stu-id="e60c7-138">Yes</span></span>     |    <span data-ttu-id="e60c7-139">Namn som ska tilldelas till rapporten</span><span class="sxs-lookup"><span data-stu-id="e60c7-139">Name to be assigned to the report</span></span>     |    <span data-ttu-id="e60c7-140">Sträng</span><span class="sxs-lookup"><span data-stu-id="e60c7-140">String</span></span>     |
|    <span data-ttu-id="e60c7-141">Beskrivning</span><span class="sxs-lookup"><span data-stu-id="e60c7-141">Description</span></span>     |    <span data-ttu-id="e60c7-142">Nej</span><span class="sxs-lookup"><span data-stu-id="e60c7-142">No</span></span>     |    <span data-ttu-id="e60c7-143">Beskrivning av den skapade rapporten</span><span class="sxs-lookup"><span data-stu-id="e60c7-143">Description of the created report</span></span>     |    <span data-ttu-id="e60c7-144">Sträng</span><span class="sxs-lookup"><span data-stu-id="e60c7-144">String</span></span>     |
|    <span data-ttu-id="e60c7-145">StartTime</span><span class="sxs-lookup"><span data-stu-id="e60c7-145">StartTime</span></span>     |    <span data-ttu-id="e60c7-146">Ja</span><span class="sxs-lookup"><span data-stu-id="e60c7-146">Yes</span></span>    |    <span data-ttu-id="e60c7-147">Tidsstämpel som rapportgenereringen ska börja efter</span><span class="sxs-lookup"><span data-stu-id="e60c7-147">Timestamp after which the report generation will begin</span></span>     |    <span data-ttu-id="e60c7-148">Sträng</span><span class="sxs-lookup"><span data-stu-id="e60c7-148">String</span></span>     |
|    <span data-ttu-id="e60c7-149">RecurrenceInterval</span><span class="sxs-lookup"><span data-stu-id="e60c7-149">RecurrenceInterval</span></span>     |    <span data-ttu-id="e60c7-150">Inga</span><span class="sxs-lookup"><span data-stu-id="e60c7-150">No</span></span>     |    <span data-ttu-id="e60c7-151">Hur ofta rapporten ska genereras i timmar.</span><span class="sxs-lookup"><span data-stu-id="e60c7-151">Frequency at which the report should be generated in hours.</span></span> <span data-ttu-id="e60c7-152">Minimivärdet är 4</span><span class="sxs-lookup"><span data-stu-id="e60c7-152">Minimum value is 4</span></span>     |    <span data-ttu-id="e60c7-153">Integer</span><span class="sxs-lookup"><span data-stu-id="e60c7-153">Integer</span></span>     |
|    <span data-ttu-id="e60c7-154">RecurrenceCount</span><span class="sxs-lookup"><span data-stu-id="e60c7-154">RecurrenceCount</span></span>     |    <span data-ttu-id="e60c7-155">Inga</span><span class="sxs-lookup"><span data-stu-id="e60c7-155">No</span></span>     |    <span data-ttu-id="e60c7-156">Antal rapporter som ska genereras.</span><span class="sxs-lookup"><span data-stu-id="e60c7-156">Numbers of report to be generated.</span></span> <span data-ttu-id="e60c7-157">Standardvärdet är obegränsad.</span><span class="sxs-lookup"><span data-stu-id="e60c7-157">Default is indefinite.</span></span>     |    <span data-ttu-id="e60c7-158">Integer</span><span class="sxs-lookup"><span data-stu-id="e60c7-158">Integer</span></span>     |
|    <span data-ttu-id="e60c7-159">Format</span><span class="sxs-lookup"><span data-stu-id="e60c7-159">Format</span></span>     |    <span data-ttu-id="e60c7-160">Inga</span><span class="sxs-lookup"><span data-stu-id="e60c7-160">No</span></span>    |    <span data-ttu-id="e60c7-161">Filformat för den exporterade filen.</span><span class="sxs-lookup"><span data-stu-id="e60c7-161">File format of the exported file.</span></span> <span data-ttu-id="e60c7-162">Standardvärdet är CSV</span><span class="sxs-lookup"><span data-stu-id="e60c7-162">Default is CSV</span></span>     |    <span data-ttu-id="e60c7-163">CSV/TSV</span><span class="sxs-lookup"><span data-stu-id="e60c7-163">CSV/TSV</span></span>     |
|    <span data-ttu-id="e60c7-164">CallbackURL</span><span class="sxs-lookup"><span data-stu-id="e60c7-164">CallbackURL</span></span>     |    <span data-ttu-id="e60c7-165">Inga</span><span class="sxs-lookup"><span data-stu-id="e60c7-165">No</span></span>     |    <span data-ttu-id="e60c7-166">URL för https-motringning som ska anropas vid rapportgenerering</span><span class="sxs-lookup"><span data-stu-id="e60c7-166">https callback URL to be called on report generation</span></span>     |    <span data-ttu-id="e60c7-167">Sträng</span><span class="sxs-lookup"><span data-stu-id="e60c7-167">String</span></span>     |
|    <span data-ttu-id="e60c7-168">CallbackMethod</span><span class="sxs-lookup"><span data-stu-id="e60c7-168">CallbackMethod</span></span>    |    <span data-ttu-id="e60c7-169">Inga</span><span class="sxs-lookup"><span data-stu-id="e60c7-169">No</span></span>    |    <span data-ttu-id="e60c7-170">HTTP-metod som ska användas för återanrop</span><span class="sxs-lookup"><span data-stu-id="e60c7-170">Http method to be used for callback</span></span>    |    <span data-ttu-id="e60c7-171">GET/POST</span><span class="sxs-lookup"><span data-stu-id="e60c7-171">GET/POST</span></span>    |
|        |        |        |        |


<span data-ttu-id="e60c7-172">**Response**</span><span class="sxs-lookup"><span data-stu-id="e60c7-172">**Response**</span></span>

<span data-ttu-id="e60c7-173">Svarsnyttolasten är strukturerad på följande sätt:</span><span class="sxs-lookup"><span data-stu-id="e60c7-173">The response payload is structured as follows:</span></span>

<span data-ttu-id="e60c7-174">Svarskod: 200, 400, 401, 403, 404, 500</span><span class="sxs-lookup"><span data-stu-id="e60c7-174">Response code: 200, 400, 401, 403, 404, 500</span></span>

<span data-ttu-id="e60c7-175">Exempel på nyttolast för svar:</span><span class="sxs-lookup"><span data-stu-id="e60c7-175">Response payload example:</span></span>

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

<span data-ttu-id="e60c7-176">**Ordlista**</span><span class="sxs-lookup"><span data-stu-id="e60c7-176">**Glossary**</span></span>

<span data-ttu-id="e60c7-177">Den här tabellen definierar nyckelelementen i svaret:</span><span class="sxs-lookup"><span data-stu-id="e60c7-177">This table defines the key elements in the response:</span></span>

|    <span data-ttu-id="e60c7-178">Parameter</span><span class="sxs-lookup"><span data-stu-id="e60c7-178">Parameter</span></span>    |    <span data-ttu-id="e60c7-179">Beskrivning</span><span class="sxs-lookup"><span data-stu-id="e60c7-179">Description</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="e60c7-180">ReportId</span><span class="sxs-lookup"><span data-stu-id="e60c7-180">ReportId</span></span>     |    <span data-ttu-id="e60c7-181">Universell unik identifierare (UUID) för den rapport som uppdateras</span><span class="sxs-lookup"><span data-stu-id="e60c7-181">Universally unique identifier (UUID) of the report being updated</span></span>     |
|    <span data-ttu-id="e60c7-182">ReportName</span><span class="sxs-lookup"><span data-stu-id="e60c7-182">ReportName</span></span>     |    <span data-ttu-id="e60c7-183">Namn som ges till rapporten i nyttolasten för begäran</span><span class="sxs-lookup"><span data-stu-id="e60c7-183">Name given to the report in the request payload</span></span>     |
|    <span data-ttu-id="e60c7-184">Description</span><span class="sxs-lookup"><span data-stu-id="e60c7-184">Description</span></span>     |    <span data-ttu-id="e60c7-185">Beskrivning som ges till rapporten i begärandenyttolasten</span><span class="sxs-lookup"><span data-stu-id="e60c7-185">Description given to the report in the request payload</span></span>     |
|    <span data-ttu-id="e60c7-186">QueryId</span><span class="sxs-lookup"><span data-stu-id="e60c7-186">QueryId</span></span>     |    <span data-ttu-id="e60c7-187">Fråge-ID som skickades när rapporten skapades</span><span class="sxs-lookup"><span data-stu-id="e60c7-187">Query ID passed at the time the report was created</span></span>     |
|    <span data-ttu-id="e60c7-188">Söka i data</span><span class="sxs-lookup"><span data-stu-id="e60c7-188">Query</span></span>     |    <span data-ttu-id="e60c7-189">Frågetext som ska köras för den här rapporten</span><span class="sxs-lookup"><span data-stu-id="e60c7-189">Query text that will be executed for this report</span></span>     |
|    <span data-ttu-id="e60c7-190">Användare</span><span class="sxs-lookup"><span data-stu-id="e60c7-190">User</span></span>     |    <span data-ttu-id="e60c7-191">Användar-ID som används för att skapa rapporten</span><span class="sxs-lookup"><span data-stu-id="e60c7-191">User ID used to create the report</span></span>     |
|    <span data-ttu-id="e60c7-192">CreatedTime</span><span class="sxs-lookup"><span data-stu-id="e60c7-192">CreatedTime</span></span>     |    <span data-ttu-id="e60c7-193">Tiden då rapporten skapades.</span><span class="sxs-lookup"><span data-stu-id="e60c7-193">Time the report was created.</span></span> <span data-ttu-id="e60c7-194">Tidsformatet är yyyy-MM-ddTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="e60c7-194">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="e60c7-195">ModifiedTime</span><span class="sxs-lookup"><span data-stu-id="e60c7-195">ModifiedTime</span></span>     |    <span data-ttu-id="e60c7-196">Tid då rapporten senast ändrades.</span><span class="sxs-lookup"><span data-stu-id="e60c7-196">Time the report was last modified.</span></span> <span data-ttu-id="e60c7-197">Tidsformatet är yyyy-MM-ddTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="e60c7-197">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="e60c7-198">ExecuteNow</span><span class="sxs-lookup"><span data-stu-id="e60c7-198">ExecuteNow</span></span>     |    <span data-ttu-id="e60c7-199">ExecuteNow-flaggan som angetts när rapporten skapades</span><span class="sxs-lookup"><span data-stu-id="e60c7-199">ExecuteNow flag set at the time the report was created</span></span>    |
|    <span data-ttu-id="e60c7-200">StartTime</span><span class="sxs-lookup"><span data-stu-id="e60c7-200">StartTime</span></span>     |    <span data-ttu-id="e60c7-201">Den tid då rapportkörningen börjar.</span><span class="sxs-lookup"><span data-stu-id="e60c7-201">Time the report execution will begin.</span></span> <span data-ttu-id="e60c7-202">Tidsformatet är yyyy-MM-ddTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="e60c7-202">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="e60c7-203">ReportStatus</span><span class="sxs-lookup"><span data-stu-id="e60c7-203">ReportStatus</span></span>     |    <span data-ttu-id="e60c7-204">Status för rapportkörningen.</span><span class="sxs-lookup"><span data-stu-id="e60c7-204">Status of the report execution.</span></span> <span data-ttu-id="e60c7-205">Möjliga värden är Pausad, Aktiv och Inaktiv.</span><span class="sxs-lookup"><span data-stu-id="e60c7-205">The possible values are Paused, Active, and Inactive.</span></span>     |
|    <span data-ttu-id="e60c7-206">RecurrenceInterval</span><span class="sxs-lookup"><span data-stu-id="e60c7-206">RecurrenceInterval</span></span>     |    <span data-ttu-id="e60c7-207">Upprepningsintervall som anges i nyttolasten för begäran</span><span class="sxs-lookup"><span data-stu-id="e60c7-207">Recurrence interval provided in the request payload</span></span>     |
|    <span data-ttu-id="e60c7-208">RecurrenceCount</span><span class="sxs-lookup"><span data-stu-id="e60c7-208">RecurrenceCount</span></span>     |    <span data-ttu-id="e60c7-209">Upprepningsantal som anges i nyttolasten för begäran</span><span class="sxs-lookup"><span data-stu-id="e60c7-209">Recurrence count provided in the request payload</span></span>     |
|    <span data-ttu-id="e60c7-210">CallbackUrl</span><span class="sxs-lookup"><span data-stu-id="e60c7-210">CallbackUrl</span></span>     |    <span data-ttu-id="e60c7-211">Motringning-URL som anges i begäran</span><span class="sxs-lookup"><span data-stu-id="e60c7-211">Callback URL provided in the request</span></span>     |
|    <span data-ttu-id="e60c7-212">CallbackMethod</span><span class="sxs-lookup"><span data-stu-id="e60c7-212">CallbackMethod</span></span>    |    <span data-ttu-id="e60c7-213">Återanropsmetod som anges i begäran</span><span class="sxs-lookup"><span data-stu-id="e60c7-213">Callback method provided in the request</span></span>    |
|    <span data-ttu-id="e60c7-214">Format</span><span class="sxs-lookup"><span data-stu-id="e60c7-214">Format</span></span>     |    <span data-ttu-id="e60c7-215">Format för rapportfilerna</span><span class="sxs-lookup"><span data-stu-id="e60c7-215">Format of the report files</span></span>     |
|    <span data-ttu-id="e60c7-216">TotalCount</span><span class="sxs-lookup"><span data-stu-id="e60c7-216">TotalCount</span></span>     |    <span data-ttu-id="e60c7-217">Antal datauppsättningar i värdematrisen</span><span class="sxs-lookup"><span data-stu-id="e60c7-217">Number of datasets in the Value array</span></span>     |
|    <span data-ttu-id="e60c7-218">Meddelande</span><span class="sxs-lookup"><span data-stu-id="e60c7-218">Message</span></span>     |    <span data-ttu-id="e60c7-219">Statusmeddelande från körningen av API:et</span><span class="sxs-lookup"><span data-stu-id="e60c7-219">Status message from the execution of the API</span></span>     |
|    <span data-ttu-id="e60c7-220">StatusCode</span><span class="sxs-lookup"><span data-stu-id="e60c7-220">StatusCode</span></span>     |    <span data-ttu-id="e60c7-221">Resultatkod.</span><span class="sxs-lookup"><span data-stu-id="e60c7-221">Result Code.</span></span> <span data-ttu-id="e60c7-222">Möjliga värden är 200, 400, 401, 403, 500</span><span class="sxs-lookup"><span data-stu-id="e60c7-222">The possible values are 200, 400, 401, 403, 500</span></span>     |
|        |        |