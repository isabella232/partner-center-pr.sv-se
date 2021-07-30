---
title: Lista över API för åtkomst till partnerinsiktsdata
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-insights
description: Lista över API för åtkomst till partnerinsiktsdata.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: cbd9f7fd08dfc4cfd247a0ed07a2c12845c5514c
ms.sourcegitcommit: ad1af627f5ee6b6e3a70655f90927e932cf4c985
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 07/29/2021
ms.locfileid: "114837007"
---
# <a name="available-apis-for-partner-insights-analytics"></a>Tillgängliga API:er för analys av partnerinsikter

Nedan visas en lista över API:er för analys av partnerinsikter och deras associerade funktioner.

## <a name="dataset-pull-apis"></a>HÄMTA API:er för datauppsättningar

***Tabell 1: HÄMTA API:er för datauppsättningar***

| **API** | **Funktioner** |
| --- | --- |
| [Hämta alla datauppsättningar](insights-programmatic-analytics-api-get-dataset.md) | Hämtar alla tillgängliga datauppsättningar. Datauppsättningar listar tabeller, kolumner, mått och tidsintervall. |
|||

## <a name="query-management-apis"></a>API:er för frågehantering

***Tabell 2: API:er för frågehantering***

| **API** | **Funktioner** |
| --- | --- |
| [Skapa rapportfråga](insights-programmatic-access-paradigm.md#create-report-query-api) | Skapar anpassade frågor som definierar datauppsättningen som kolumner och mått behöver exporteras från. |
| [HÄMTA rapportfråga](insights-programmatic-analytics-api-get-report-queries.md) | Hämtar alla frågor som är tillgängliga för användning i rapporter. Hämtar alla system- och användardefinierade frågor som standard. |
| [TA BORT rapportfråga](insights-programmatic-analytics-api-delete-report-queries.md) | Tar bort användardefinierade frågor. |
|||

## <a name="report-management-apis"></a>API:er för rapporthantering

***Tabell 3: API:er för rapporthantering***

| **API** | **Funktioner** |
| --- | --- |
| [Skapa rapport](insights-programmatic-access-paradigm.md#create-report-api) | Schemalägger en fråga som ska köras med jämna mellanrum. |
| [TESTA rapportfråga](insights-programmatic-analytics-api-try-report-queries.md) | Kör en rapportfrågeutdrag. Returnerar endast 10 poster som en partner kan använda för att verifiera om data är som förväntat. |
| [Hämta rapport](insights-programmatic-analytics-api-get-report.md) | Hämta alla rapporter som har schemalagts. |
| [Uppdatera rapport](insights-programmatic-analytics-api-update-report.md) | Ändra en rapportparameter. |
| [Ta bort rapport](insights-programmatic-analytics-api-delete-report.md) | Tar bort alla rapport- och rapportkörningsposter. |
| [Pausa rapportkörningar](insights-programmatic-analytics-api-pause-report-executions.md) | Pausar den schemalagda körningen av rapporter. |
| [Återuppta rapportkörningar](insights-programmatic-analytics-api-resume-report-executions.md) | Återupptar den schemalagda körningen av en pausad rapport. |
|||

## <a name="report-execution-pull-apis"></a>PULL-API:er för rapportkörning

***Tabell 4: PULL-API:er för rapportkörning***

| **API** | **Funktioner** |
| --- | --- |
| [Hämta rapportkörningar](insights-programmatic-access-paradigm.md#get-report-execution-api) | Hämta alla körningar som har inträffat för en viss rapport. |
|||

## <a name="next-steps"></a>Nästa steg

- Du kan prova API:erna via [Swagger API-URL:en](https://api.partnercenter.microsoft.com/insights/v1/mpn/swagger/index.html).