---
title: 'Hämta alla datauppsättnings-API : Insights data'
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Använd det här API:et för att få information om alla tillgängliga datauppsättningar i Partner Center-insikter.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: 42ff7cc1f097e2423be5f1f7f9a7f62214d64949
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 07/16/2021
ms.locfileid: "114376959"
---
# <a name="get-all-datasets-api"></a><span data-ttu-id="365c8-103">Hämta alla datauppsättnings-API</span><span class="sxs-lookup"><span data-stu-id="365c8-103">Get all datasets API</span></span>

<span data-ttu-id="365c8-104">API:et Hämta alla datauppsättningar hämtar alla tillgängliga datauppsättningar.</span><span class="sxs-lookup"><span data-stu-id="365c8-104">The Get all datasets API gets all the available datasets.</span></span> <span data-ttu-id="365c8-105">Datauppsättningar listar tabeller, kolumner, mått och tidsintervall.</span><span class="sxs-lookup"><span data-stu-id="365c8-105">Datasets list the tables, columns, metrics, and time ranges.</span></span>

<span data-ttu-id="365c8-106">**Begärandesyntax**</span><span class="sxs-lookup"><span data-stu-id="365c8-106">**Request syntax**</span></span>

|    <span data-ttu-id="365c8-107">Metod</span><span class="sxs-lookup"><span data-stu-id="365c8-107">Method</span></span>    |    <span data-ttu-id="365c8-108">URI för förfrågan</span><span class="sxs-lookup"><span data-stu-id="365c8-108">Request URI</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="365c8-109">GET</span><span class="sxs-lookup"><span data-stu-id="365c8-109">GET</span></span>    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledDataset?datasetName={Dataset Name}`     |
|        |        |

<span data-ttu-id="365c8-110">**Begärandehuvud**</span><span class="sxs-lookup"><span data-stu-id="365c8-110">**Request header**</span></span>

|    <span data-ttu-id="365c8-111">Huvud</span><span class="sxs-lookup"><span data-stu-id="365c8-111">Header</span></span>    |    <span data-ttu-id="365c8-112">Typ</span><span class="sxs-lookup"><span data-stu-id="365c8-112">Type</span></span>    |    <span data-ttu-id="365c8-113">Description</span><span class="sxs-lookup"><span data-stu-id="365c8-113">Description</span></span>    |
|    ----    |    ----    |    ----    |
|    <span data-ttu-id="365c8-114">Auktorisering</span><span class="sxs-lookup"><span data-stu-id="365c8-114">Authorization</span></span>    |    <span data-ttu-id="365c8-115">sträng</span><span class="sxs-lookup"><span data-stu-id="365c8-115">string</span></span>    |    <span data-ttu-id="365c8-116">Krävs.</span><span class="sxs-lookup"><span data-stu-id="365c8-116">Required.</span></span> <span data-ttu-id="365c8-117">Åtkomsttoken Azure Active Directory (AAD) i formuläret`Bearer <token>`</span><span class="sxs-lookup"><span data-stu-id="365c8-117">The Azure Active Directory (AAD) access token in the form `Bearer <token>`</span></span>    |
|    <span data-ttu-id="365c8-118">Content-Type</span><span class="sxs-lookup"><span data-stu-id="365c8-118">Content-Type</span></span>    |    <span data-ttu-id="365c8-119">sträng</span><span class="sxs-lookup"><span data-stu-id="365c8-119">string</span></span>    |    `Application/JSON`    |
|        |        |        |

<span data-ttu-id="365c8-120">**Sökvägsparameter**</span><span class="sxs-lookup"><span data-stu-id="365c8-120">**Path parameter**</span></span>

<span data-ttu-id="365c8-121">Ingen</span><span class="sxs-lookup"><span data-stu-id="365c8-121">None</span></span>

<span data-ttu-id="365c8-122">**Frågeparameter**</span><span class="sxs-lookup"><span data-stu-id="365c8-122">**Query parameter**</span></span>

|    <span data-ttu-id="365c8-123">Parameternamn</span><span class="sxs-lookup"><span data-stu-id="365c8-123">Parameter Name</span></span>    |    <span data-ttu-id="365c8-124">Typ</span><span class="sxs-lookup"><span data-stu-id="365c8-124">Type</span></span>    |    <span data-ttu-id="365c8-125">Obligatorisk</span><span class="sxs-lookup"><span data-stu-id="365c8-125">Required</span></span>    |    <span data-ttu-id="365c8-126">Beskrivning</span><span class="sxs-lookup"><span data-stu-id="365c8-126">Description</span></span>    |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="365c8-127">datasetName</span><span class="sxs-lookup"><span data-stu-id="365c8-127">datasetName</span></span>    |    <span data-ttu-id="365c8-128">sträng</span><span class="sxs-lookup"><span data-stu-id="365c8-128">string</span></span>    |    <span data-ttu-id="365c8-129">No</span><span class="sxs-lookup"><span data-stu-id="365c8-129">No</span></span>    |    <span data-ttu-id="365c8-130">Filter för att hämta information om endast en datauppsättning</span><span class="sxs-lookup"><span data-stu-id="365c8-130">Filter to get details of only one dataset</span></span>    |
|        |        |        |        |

<span data-ttu-id="365c8-131">**Begära nyttolast**</span><span class="sxs-lookup"><span data-stu-id="365c8-131">**Request payload**</span></span>

<span data-ttu-id="365c8-132">Ingen</span><span class="sxs-lookup"><span data-stu-id="365c8-132">None</span></span>

<span data-ttu-id="365c8-133">**Ordlista**</span><span class="sxs-lookup"><span data-stu-id="365c8-133">**Glossary**</span></span>

<span data-ttu-id="365c8-134">Ingen</span><span class="sxs-lookup"><span data-stu-id="365c8-134">None</span></span>

<span data-ttu-id="365c8-135">**Response**</span><span class="sxs-lookup"><span data-stu-id="365c8-135">**Response**</span></span>

<span data-ttu-id="365c8-136">Svarsnyttolasten är strukturerad på följande sätt:</span><span class="sxs-lookup"><span data-stu-id="365c8-136">The response payload is structured as follows:</span></span>

<span data-ttu-id="365c8-137">Svarskod: 200, 400, 401, 403, 404, 500</span><span class="sxs-lookup"><span data-stu-id="365c8-137">Response code: 200, 400, 401, 403, 404, 500</span></span>

<span data-ttu-id="365c8-138">Exempel på nyttolast för svar:</span><span class="sxs-lookup"><span data-stu-id="365c8-138">Response payload example:</span></span>

```json
{ 
   "Value":[ 
      { 
         "DatasetName ":"string", 
         "SelectableColumns":[ 
            "string" 
         ], 
         "AvailableMetrics":[ 
            "string" 
         ], 
         "AvailableDateRanges":[ 
            "string" 
         ], 
         "minimumRecurrenceInterval":0 
      } 
   ], 
   "TotalCount":0, 
   "Message":"<Error Message>", 
   "StatusCode": 0, 
} 
```

<span data-ttu-id="365c8-139">**Ordlista**</span><span class="sxs-lookup"><span data-stu-id="365c8-139">**Glossary**</span></span>

<span data-ttu-id="365c8-140">Den här tabellen definierar nyckelelementen i svaret:</span><span class="sxs-lookup"><span data-stu-id="365c8-140">This table defines the key elements in the response:</span></span>

|    <span data-ttu-id="365c8-141">Parameter</span><span class="sxs-lookup"><span data-stu-id="365c8-141">Parameter</span></span>    |    <span data-ttu-id="365c8-142">Beskrivning</span><span class="sxs-lookup"><span data-stu-id="365c8-142">Description</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="365c8-143">DatasetName</span><span class="sxs-lookup"><span data-stu-id="365c8-143">DatasetName</span></span>     |    <span data-ttu-id="365c8-144">Namnet på den datauppsättning som matrisobjektet definierar</span><span class="sxs-lookup"><span data-stu-id="365c8-144">Name of the dataset that this array object defines</span></span>     |
|    <span data-ttu-id="365c8-145">SelectableColumns</span><span class="sxs-lookup"><span data-stu-id="365c8-145">SelectableColumns</span></span>     |    <span data-ttu-id="365c8-146">Råkolumner som kan anges i de valda kolumnerna</span><span class="sxs-lookup"><span data-stu-id="365c8-146">Raw columns that can be specified in the select columns</span></span>     |
|    <span data-ttu-id="365c8-147">AvailableMetrics</span><span class="sxs-lookup"><span data-stu-id="365c8-147">AvailableMetrics</span></span>     |    <span data-ttu-id="365c8-148">Sammansättnings-/måttkolumnnamn som kan anges i de valda kolumnerna</span><span class="sxs-lookup"><span data-stu-id="365c8-148">Aggregation/metric column names that can be specified in the select columns</span></span>     |
|    <span data-ttu-id="365c8-149">AvailableDateRanges</span><span class="sxs-lookup"><span data-stu-id="365c8-149">AvailableDateRanges</span></span>     |    <span data-ttu-id="365c8-150">Datumintervall som kan användas i rapportfrågor för datauppsättningen</span><span class="sxs-lookup"><span data-stu-id="365c8-150">Date range that can be used in report queries for the dataset</span></span>     |
|    <span data-ttu-id="365c8-151">minimumRecurrenceInterval</span><span class="sxs-lookup"><span data-stu-id="365c8-151">minimumRecurrenceInterval</span></span>     |    <span data-ttu-id="365c8-152">Minsta värde för upprepningsintervall</span><span class="sxs-lookup"><span data-stu-id="365c8-152">Minimum value of Recurrence Interval</span></span>     |
|    <span data-ttu-id="365c8-153">TotalCount</span><span class="sxs-lookup"><span data-stu-id="365c8-153">TotalCount</span></span>     |    <span data-ttu-id="365c8-154">Antal datauppsättningar i värdematrisen</span><span class="sxs-lookup"><span data-stu-id="365c8-154">Number of datasets in the Value array</span></span>     |
|    <span data-ttu-id="365c8-155">Meddelande</span><span class="sxs-lookup"><span data-stu-id="365c8-155">Message</span></span>     |    <span data-ttu-id="365c8-156">Statusmeddelande från körningen av API:et</span><span class="sxs-lookup"><span data-stu-id="365c8-156">Status message from the execution of the API</span></span>     |
|    <span data-ttu-id="365c8-157">StatusCode</span><span class="sxs-lookup"><span data-stu-id="365c8-157">StatusCode</span></span>     |    <span data-ttu-id="365c8-158">Resultatkod.</span><span class="sxs-lookup"><span data-stu-id="365c8-158">Result Code.</span></span> <span data-ttu-id="365c8-159">Möjliga värden är 200, 400, 401, 403, 500</span><span class="sxs-lookup"><span data-stu-id="365c8-159">The possible values are 200, 400, 401, 403, 500</span></span>     |
|        |        |
