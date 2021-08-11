---
title: HÄMTA API för rapportfrågor – Insights data
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-insights
description: Använd det här API:et för att hämta alla tillgängliga frågor som ska användas i rapport-API:et.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: 943eea26a08f1072b6ddcaf8136b7f9f757d52b8c0170f03519b8787c1877bd3
ms.sourcegitcommit: 121f1b9cbd88faeba60dc9b475f9c0647cdc933c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/06/2021
ms.locfileid: "115695194"
---
# <a name="get-report-queries-api"></a>HÄMTA API för rapportfrågor

API:et Hämta rapportfrågor hämtar alla frågor som är tillgängliga för användning i rapporter. Den hämtar alla system- och användardefinierade frågor som standard.

**Begärandesyntax**

|    Metod    |    URI för förfrågan    |
|    ----    |    ----    |
|    GET    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledQueries?queryId={QueryID}&queryName={QueryName}&includeSystemQueries={include_system_queries}&includeOnlySystemQueries={include_only_system_queries}`     |
|        |        |

**Begärandehuvud**

|    Huvud    |    Typ    |    Description    |
|    ----    |    ----    |    ----    |
|    Auktorisering    |    sträng    |    Krävs. Åtkomsttoken Azure Active Directory (AAD) i formuläret`Bearer <token>`    |
|    Content-Type    |    sträng    |    `Application/JSON`    |
|        |        |        |

**Sökvägsparameter**

Ingen

**Frågeparameter**

|    Parameternamn    |    Typ    |    Obligatorisk    |    Beskrivning    |
|    ----    |    ----    |    ----    |    ----    |
|    queryId     |    sträng     |    No    |    Filtrera för att hämta information om endast frågor med det ID som anges i argumentet     |
|    queryName     |    sträng     |    No    |    Filter för att hämta information om endast frågor med det namn som anges i argumentet     |
|    IncludeSystemQueries     |    boolean     |    No    |    Inkludera fördefinierade systemfrågor i svaret     |
|    IncludeOnlySystemQueries     |    boolean     |    No    |    Inkludera endast systemfrågor i svaret     |
|        |        |        |        |


**Begära nyttolast**

Ingen

**Ordlista**

Ingen

**Response**

Svarsnyttolasten är strukturerad på följande sätt:

Svarskod: 200, 400, 401, 403, 404, 500

Exempel på nyttolast för svar:

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

**Ordlista**

Den här tabellen definierar nyckelelementen i svaret:

|    Parameter    |    Beskrivning    |
|    ----    |    ----    |
|    QueryId     |    Unikt UUID för frågan     |
|    Name     |    Namn som gavs till frågan när frågan skapades     |
|    Description     |    Beskrivning som anges när frågan skapas     |
|    Söka i data     |    Rapportfrågesträng     |
|    Typ     |    Ange till userDefined för användarskapade frågor och system för fördefinierade systemfrågor     |
|    Användare     |    Användar-ID som skapade frågan     |
|    CreatedTime     |    Tid då frågan skapades     |
|    TotalCount     |    Antal datauppsättningar i värdematrisen     |
|    Meddelande     |    Statusmeddelande från körningen av API:et     |
|    StatusCode     |    Resultatkod. Möjliga värden är 200, 400, 401, 403, 500     |
|        |        |
