---
title: Lista över API för åtkomst till partnerinsiktsdata
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Lista över API för åtkomst till partnerinsiktsdata.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: 71d04b6927e27b1d7a8d72bbdaa56b41cb113625
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 07/16/2021
ms.locfileid: "114377171"
---
# <a name="available-apis-for-partner-insights-analytics"></a><span data-ttu-id="77965-103">Tillgängliga API:er för analys av partnerinsikter</span><span class="sxs-lookup"><span data-stu-id="77965-103">Available APIs for partner insights analytics</span></span>

<span data-ttu-id="77965-104">Nedan visas en lista över API:er för analys av partnerinsikter och deras associerade funktioner.</span><span class="sxs-lookup"><span data-stu-id="77965-104">Following are the list of APIs for partner insights analytics and their associated functionalities.</span></span>

## <a name="dataset-pull-apis"></a><span data-ttu-id="77965-105">HÄMTA API:er för datauppsättningar</span><span class="sxs-lookup"><span data-stu-id="77965-105">Dataset pull APIs</span></span>

<span data-ttu-id="77965-106">***Tabell 1: HÄMTA API:er för datauppsättningar***</span><span class="sxs-lookup"><span data-stu-id="77965-106">***Table 1: Dataset pull APIs***</span></span>

| <span data-ttu-id="77965-107">**API**</span><span class="sxs-lookup"><span data-stu-id="77965-107">**API**</span></span> | <span data-ttu-id="77965-108">**Funktioner**</span><span class="sxs-lookup"><span data-stu-id="77965-108">**Functionality**</span></span> |
| --- | --- |
| [<span data-ttu-id="77965-109">Hämta alla datauppsättningar</span><span class="sxs-lookup"><span data-stu-id="77965-109">Get all datasets</span></span>](insights-programmatic-analytics-api-get-dataset.md) | <span data-ttu-id="77965-110">Hämtar alla tillgängliga datauppsättningar.</span><span class="sxs-lookup"><span data-stu-id="77965-110">Gets all the available datasets.</span></span> <span data-ttu-id="77965-111">Datauppsättningar listar tabeller, kolumner, mått och tidsintervall.</span><span class="sxs-lookup"><span data-stu-id="77965-111">Datasets list the tables, columns, metrics, and time ranges.</span></span> |
|||

## <a name="query-management-apis"></a><span data-ttu-id="77965-112">API:er för frågehantering</span><span class="sxs-lookup"><span data-stu-id="77965-112">Query management APIs</span></span>

<span data-ttu-id="77965-113">***Tabell 2: API:er för frågehantering***</span><span class="sxs-lookup"><span data-stu-id="77965-113">***Table 2: Query management APIs***</span></span>

| <span data-ttu-id="77965-114">**API**</span><span class="sxs-lookup"><span data-stu-id="77965-114">**API**</span></span> | <span data-ttu-id="77965-115">**Funktioner**</span><span class="sxs-lookup"><span data-stu-id="77965-115">**Functionality**</span></span> |
| --- | --- |
| [<span data-ttu-id="77965-116">Skapa rapportfråga</span><span class="sxs-lookup"><span data-stu-id="77965-116">Create Report Query</span></span>](insights-programmatic-access-paradigm.md#create-report-query-api) | <span data-ttu-id="77965-117">Skapar anpassade frågor som definierar datauppsättningen som kolumner och mått behöver exporteras från.</span><span class="sxs-lookup"><span data-stu-id="77965-117">Creates custom queries that define the dataset from which columns and metrics need to be exported.</span></span> |
| [<span data-ttu-id="77965-118">HÄMTA rapportfråga</span><span class="sxs-lookup"><span data-stu-id="77965-118">GET Report Query</span></span>](insights-programmatic-analytics-api-get-report-queries.md) | <span data-ttu-id="77965-119">Hämtar alla frågor som är tillgängliga för användning i rapporter.</span><span class="sxs-lookup"><span data-stu-id="77965-119">Gets all the queries available for use in reports.</span></span> <span data-ttu-id="77965-120">Hämtar alla system- och användardefinierade frågor som standard.</span><span class="sxs-lookup"><span data-stu-id="77965-120">Gets all the system and user-defined queries by default.</span></span> |
| [<span data-ttu-id="77965-121">TA BORT rapportfråga</span><span class="sxs-lookup"><span data-stu-id="77965-121">DELETE Report Query</span></span>](insights-programmatic-analytics-api-delete-report-queries.md) | <span data-ttu-id="77965-122">Tar bort användardefinierade frågor.</span><span class="sxs-lookup"><span data-stu-id="77965-122">Deletes user-defined queries.</span></span> |
|||

## <a name="report-management-apis"></a><span data-ttu-id="77965-123">API:er för rapporthantering</span><span class="sxs-lookup"><span data-stu-id="77965-123">Report management APIs</span></span>

<span data-ttu-id="77965-124">***Tabell 3: API:er för rapporthantering***</span><span class="sxs-lookup"><span data-stu-id="77965-124">***Table 3: Report management APIs***</span></span>

| <span data-ttu-id="77965-125">**API**</span><span class="sxs-lookup"><span data-stu-id="77965-125">**API**</span></span> | <span data-ttu-id="77965-126">**Funktioner**</span><span class="sxs-lookup"><span data-stu-id="77965-126">**Functionality**</span></span> |
| --- | --- |
| [<span data-ttu-id="77965-127">Skapa rapport</span><span class="sxs-lookup"><span data-stu-id="77965-127">Create Report</span></span>](insights-programmatic-access-paradigm.md#create-report-api) | <span data-ttu-id="77965-128">Schemalägger en fråga som ska köras med jämna mellanrum.</span><span class="sxs-lookup"><span data-stu-id="77965-128">Schedules a query to be executed at regular intervals.</span></span> |
| [<span data-ttu-id="77965-129">Testa rapportfråga</span><span class="sxs-lookup"><span data-stu-id="77965-129">TRY Report Query</span></span>](insights-programmatic-analytics-api-try-report-queries.md) | <span data-ttu-id="77965-130">Kör en rapportfrågeutdrag.</span><span class="sxs-lookup"><span data-stu-id="77965-130">Executes a Report query statement.</span></span> <span data-ttu-id="77965-131">Returnerar endast 10 poster som en partner kan använda för att verifiera om data är som förväntat.</span><span class="sxs-lookup"><span data-stu-id="77965-131">Returns only 10 records that a partner can use to verify if the data is as expected.</span></span> |
| [<span data-ttu-id="77965-132">Hämta rapport</span><span class="sxs-lookup"><span data-stu-id="77965-132">Get Report</span></span>](insights-programmatic-analytics-api-get-report.md) | <span data-ttu-id="77965-133">Hämta alla rapporter som har schemalagts.</span><span class="sxs-lookup"><span data-stu-id="77965-133">Get all the reports that have been scheduled.</span></span> |
| [<span data-ttu-id="77965-134">Uppdatera rapport</span><span class="sxs-lookup"><span data-stu-id="77965-134">Update Report</span></span>](insights-programmatic-analytics-api-update-report.md) | <span data-ttu-id="77965-135">Ändra en rapportparameter.</span><span class="sxs-lookup"><span data-stu-id="77965-135">Modify a report parameter.</span></span> |
| [<span data-ttu-id="77965-136">Ta bort rapport</span><span class="sxs-lookup"><span data-stu-id="77965-136">Delete Report</span></span>](insights-programmatic-analytics-api-delete-report.md) | <span data-ttu-id="77965-137">Tar bort alla rapport- och rapportkörningsposter.</span><span class="sxs-lookup"><span data-stu-id="77965-137">Deletes all the report and report execution records.</span></span> |
| [<span data-ttu-id="77965-138">Pausa rapportkörningar</span><span class="sxs-lookup"><span data-stu-id="77965-138">Pause Report Executions</span></span>](insights-programmatic-analytics-api-pause-report-executions.md) | <span data-ttu-id="77965-139">Pausar den schemalagda körningen av rapporter.</span><span class="sxs-lookup"><span data-stu-id="77965-139">Pauses the scheduled execution of reports.</span></span> |
| [<span data-ttu-id="77965-140">Återuppta rapportkörningar</span><span class="sxs-lookup"><span data-stu-id="77965-140">Resume Report Executions</span></span>](insights-programmatic-analytics-api-resume-report-executions.md) | <span data-ttu-id="77965-141">Återupptar den schemalagda körningen av en pausad rapport.</span><span class="sxs-lookup"><span data-stu-id="77965-141">Resumes the scheduled execution of a paused report.</span></span> |
|||

## <a name="report-execution-pull-apis"></a><span data-ttu-id="77965-142">PULL-API:er för rapportkörning</span><span class="sxs-lookup"><span data-stu-id="77965-142">Report execution pull APIs</span></span>

<span data-ttu-id="77965-143">***Tabell 4: PULL-API:er för rapportkörning***</span><span class="sxs-lookup"><span data-stu-id="77965-143">***Table 4: Report execution pull APIs***</span></span>

| <span data-ttu-id="77965-144">**API**</span><span class="sxs-lookup"><span data-stu-id="77965-144">**API**</span></span> | <span data-ttu-id="77965-145">**Funktioner**</span><span class="sxs-lookup"><span data-stu-id="77965-145">**Functionality**</span></span> |
| --- | --- |
| [<span data-ttu-id="77965-146">Hämta rapportkörningar</span><span class="sxs-lookup"><span data-stu-id="77965-146">Get Report Executions</span></span>](insights-programmatic-access-paradigm.md#get-report-execution-api) | <span data-ttu-id="77965-147">Hämta alla körningar som har inträffat för en viss rapport.</span><span class="sxs-lookup"><span data-stu-id="77965-147">Get all the executions that have happened for a given report.</span></span> |
|||

## <a name="next-steps"></a><span data-ttu-id="77965-148">Nästa steg</span><span class="sxs-lookup"><span data-stu-id="77965-148">Next steps</span></span>

- <span data-ttu-id="77965-149">Du kan prova API:erna via [Swagger API-URL:en](https://api.partnercenter.microsoft.com/insights/v1/mpn/swagger/index.html).</span><span class="sxs-lookup"><span data-stu-id="77965-149">You can try out the APIs through the [Swagger API URL](https://api.partnercenter.microsoft.com/insights/v1/mpn/swagger/index.html).</span></span>