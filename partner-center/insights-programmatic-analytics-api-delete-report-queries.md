---
title: TA bort API för rapportfrågor – Insights data
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Använd det här API:et för att ta bort användardefinierade frågor i Partner center-insikter.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: e608068613edad1fca277ba5886c9c4bc962ffd2
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 07/16/2021
ms.locfileid: "114376978"
---
# <a name="delete-report-queries-api"></a><span data-ttu-id="d6f7e-103">API för att ta bort rapportfrågor</span><span class="sxs-lookup"><span data-stu-id="d6f7e-103">Delete report queries API</span></span>

<span data-ttu-id="d6f7e-104">Det här API:et tar bort användardefinierade frågor.</span><span class="sxs-lookup"><span data-stu-id="d6f7e-104">This API deletes user-defined queries.</span></span>

<span data-ttu-id="d6f7e-105">**Begärandesyntax**</span><span class="sxs-lookup"><span data-stu-id="d6f7e-105">**Request syntax**</span></span>

|    <span data-ttu-id="d6f7e-106">Metod</span><span class="sxs-lookup"><span data-stu-id="d6f7e-106">Method</span></span>    |    <span data-ttu-id="d6f7e-107">URI för förfrågan</span><span class="sxs-lookup"><span data-stu-id="d6f7e-107">Request URI</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="d6f7e-108">DELETE</span><span class="sxs-lookup"><span data-stu-id="d6f7e-108">DELETE</span></span>    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledQueries/{queryId}` |
|        |        |

<span data-ttu-id="d6f7e-109">**Begärandehuvud**</span><span class="sxs-lookup"><span data-stu-id="d6f7e-109">**Request header**</span></span>

|    <span data-ttu-id="d6f7e-110">Huvud</span><span class="sxs-lookup"><span data-stu-id="d6f7e-110">Header</span></span>    |    <span data-ttu-id="d6f7e-111">Typ</span><span class="sxs-lookup"><span data-stu-id="d6f7e-111">Type</span></span>    |    <span data-ttu-id="d6f7e-112">Description</span><span class="sxs-lookup"><span data-stu-id="d6f7e-112">Description</span></span>    |
|    ----    |    ----    |    ----    |
|    <span data-ttu-id="d6f7e-113">Auktorisering</span><span class="sxs-lookup"><span data-stu-id="d6f7e-113">Authorization</span></span>    |    <span data-ttu-id="d6f7e-114">sträng</span><span class="sxs-lookup"><span data-stu-id="d6f7e-114">string</span></span>    |    <span data-ttu-id="d6f7e-115">Krävs.</span><span class="sxs-lookup"><span data-stu-id="d6f7e-115">Required.</span></span> <span data-ttu-id="d6f7e-116">Åtkomsttoken Azure Active Directory (AAD) i formuläret`Bearer <token>`</span><span class="sxs-lookup"><span data-stu-id="d6f7e-116">The Azure Active Directory (AAD) access token in the form `Bearer <token>`</span></span>    |
|    <span data-ttu-id="d6f7e-117">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d6f7e-117">Content-Type</span></span>    |    <span data-ttu-id="d6f7e-118">sträng</span><span class="sxs-lookup"><span data-stu-id="d6f7e-118">string</span></span>    |    `Application/JSON`    |
|        |        |        |

<span data-ttu-id="d6f7e-119">**Sökvägsparameter**</span><span class="sxs-lookup"><span data-stu-id="d6f7e-119">**Path parameter**</span></span>

|    <span data-ttu-id="d6f7e-120">Parameternamn</span><span class="sxs-lookup"><span data-stu-id="d6f7e-120">Parameter Name</span></span>    |    <span data-ttu-id="d6f7e-121">Typ</span><span class="sxs-lookup"><span data-stu-id="d6f7e-121">Type</span></span>    |    <span data-ttu-id="d6f7e-122">Obligatorisk</span><span class="sxs-lookup"><span data-stu-id="d6f7e-122">Required</span></span>    |    <span data-ttu-id="d6f7e-123">Beskrivning</span><span class="sxs-lookup"><span data-stu-id="d6f7e-123">Description</span></span>    |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="d6f7e-124">queryId</span><span class="sxs-lookup"><span data-stu-id="d6f7e-124">queryId</span></span>     |    <span data-ttu-id="d6f7e-125">sträng</span><span class="sxs-lookup"><span data-stu-id="d6f7e-125">string</span></span>     |    <span data-ttu-id="d6f7e-126">No</span><span class="sxs-lookup"><span data-stu-id="d6f7e-126">No</span></span>    |    <span data-ttu-id="d6f7e-127">Filtrera för att hämta information om endast frågor med det ID som anges i argumentet</span><span class="sxs-lookup"><span data-stu-id="d6f7e-127">Filter to get details of only queries with the ID given in the argument</span></span>     |
|        |        |        |        |

<span data-ttu-id="d6f7e-128">**Frågeparameter**</span><span class="sxs-lookup"><span data-stu-id="d6f7e-128">**Query parameter**</span></span>

<span data-ttu-id="d6f7e-129">Ingen</span><span class="sxs-lookup"><span data-stu-id="d6f7e-129">None</span></span>

<span data-ttu-id="d6f7e-130">**Begära nyttolast**</span><span class="sxs-lookup"><span data-stu-id="d6f7e-130">**Request payload**</span></span>

<span data-ttu-id="d6f7e-131">Ingen</span><span class="sxs-lookup"><span data-stu-id="d6f7e-131">None</span></span>

<span data-ttu-id="d6f7e-132">**Ordlista**</span><span class="sxs-lookup"><span data-stu-id="d6f7e-132">**Glossary**</span></span>

<span data-ttu-id="d6f7e-133">Ingen</span><span class="sxs-lookup"><span data-stu-id="d6f7e-133">None</span></span>

<span data-ttu-id="d6f7e-134">**Response**</span><span class="sxs-lookup"><span data-stu-id="d6f7e-134">**Response**</span></span>

<span data-ttu-id="d6f7e-135">Svarsnyttolasten är strukturerad på följande sätt:</span><span class="sxs-lookup"><span data-stu-id="d6f7e-135">The response payload is structured as follows:</span></span>

<span data-ttu-id="d6f7e-136">Svarskod: 200, 400, 401, 403, 404, 500</span><span class="sxs-lookup"><span data-stu-id="d6f7e-136">Response code: 200, 400, 401, 403, 404, 500</span></span>

<span data-ttu-id="d6f7e-137">Exempel på nyttolast för svar:</span><span class="sxs-lookup"><span data-stu-id="d6f7e-137">Response payload example:</span></span>

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

<span data-ttu-id="d6f7e-138">**Ordlista**</span><span class="sxs-lookup"><span data-stu-id="d6f7e-138">**Glossary**</span></span>

<span data-ttu-id="d6f7e-139">Den här tabellen definierar nyckelelementen i svaret:</span><span class="sxs-lookup"><span data-stu-id="d6f7e-139">This table defines the key elements in the response:</span></span>

|    <span data-ttu-id="d6f7e-140">Parameter</span><span class="sxs-lookup"><span data-stu-id="d6f7e-140">Parameter</span></span>    |    <span data-ttu-id="d6f7e-141">Beskrivning</span><span class="sxs-lookup"><span data-stu-id="d6f7e-141">Description</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="d6f7e-142">QueryId</span><span class="sxs-lookup"><span data-stu-id="d6f7e-142">QueryId</span></span>     |    <span data-ttu-id="d6f7e-143">Unikt UUID för frågan som togs bort</span><span class="sxs-lookup"><span data-stu-id="d6f7e-143">Unique UUID of the query that was deleted</span></span>    |
|    <span data-ttu-id="d6f7e-144">Name</span><span class="sxs-lookup"><span data-stu-id="d6f7e-144">Name</span></span>     |    <span data-ttu-id="d6f7e-145">Namnet på den fråga som togs bort</span><span class="sxs-lookup"><span data-stu-id="d6f7e-145">Name of the query that was deleted</span></span>    |
|    <span data-ttu-id="d6f7e-146">Description</span><span class="sxs-lookup"><span data-stu-id="d6f7e-146">Description</span></span>     |    <span data-ttu-id="d6f7e-147">Beskrivning av den borttagna frågan</span><span class="sxs-lookup"><span data-stu-id="d6f7e-147">Description of the deleted query</span></span>     |
|    <span data-ttu-id="d6f7e-148">Söka i data</span><span class="sxs-lookup"><span data-stu-id="d6f7e-148">Query</span></span>     |    <span data-ttu-id="d6f7e-149">Rapportfrågesträng för den borttagna frågan</span><span class="sxs-lookup"><span data-stu-id="d6f7e-149">Report query string of the deleted query</span></span>    |
|    <span data-ttu-id="d6f7e-150">Typ</span><span class="sxs-lookup"><span data-stu-id="d6f7e-150">Type</span></span>     |    <span data-ttu-id="d6f7e-151">Ställ in på userDefined för användarskapade frågor</span><span class="sxs-lookup"><span data-stu-id="d6f7e-151">Set to userDefined for user created queries</span></span>     |
|    <span data-ttu-id="d6f7e-152">Användare</span><span class="sxs-lookup"><span data-stu-id="d6f7e-152">User</span></span>     |    <span data-ttu-id="d6f7e-153">Användar-ID som skapade frågan</span><span class="sxs-lookup"><span data-stu-id="d6f7e-153">User ID who created the query</span></span>     |
|    <span data-ttu-id="d6f7e-154">CreatedTime</span><span class="sxs-lookup"><span data-stu-id="d6f7e-154">CreatedTime</span></span>     |    <span data-ttu-id="d6f7e-155">Tid då frågan skapades</span><span class="sxs-lookup"><span data-stu-id="d6f7e-155">Time of creation of query</span></span>     |
|    <span data-ttu-id="d6f7e-156">TotalCount</span><span class="sxs-lookup"><span data-stu-id="d6f7e-156">TotalCount</span></span>     |    <span data-ttu-id="d6f7e-157">Antal datauppsättningar i värdematrisen</span><span class="sxs-lookup"><span data-stu-id="d6f7e-157">Number of datasets in the Value array</span></span>     |
|    <span data-ttu-id="d6f7e-158">Meddelande</span><span class="sxs-lookup"><span data-stu-id="d6f7e-158">Message</span></span>     |    <span data-ttu-id="d6f7e-159">Statusmeddelande från körningen av API:et</span><span class="sxs-lookup"><span data-stu-id="d6f7e-159">Status message from the execution of the API</span></span>     |
|    <span data-ttu-id="d6f7e-160">StatusCode</span><span class="sxs-lookup"><span data-stu-id="d6f7e-160">StatusCode</span></span>     |    <span data-ttu-id="d6f7e-161">Resultatkod.</span><span class="sxs-lookup"><span data-stu-id="d6f7e-161">Result Code.</span></span> <span data-ttu-id="d6f7e-162">Möjliga värden är 200, 400, 401, 403, 500</span><span class="sxs-lookup"><span data-stu-id="d6f7e-162">The possible values are 200, 400, 401, 403, 500</span></span>     |
|        |        |
