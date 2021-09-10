---
title: Testa API för rapportfrågor
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-insights
description: Använd det här API:et för att testa din fråga och validera resultaten i Partner Center-insikter.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: c83b56b7d52e0b9feb598597b4a8e1fdaec98a3b
ms.sourcegitcommit: 1161d5bcb345e368348c535a7211f0d353c5a471
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/09/2021
ms.locfileid: "123960923"
---
# <a name="try-report-queries-api"></a>Testa API för rapportfrågor

Det här API:et kör en rapportfrågesats. API:et returnerar bara 100 poster som du som partner kan använda för att kontrollera om data är som förväntat.

> [!IMPORTANT]
> Det här API:et har en tidsgräns för frågekörning på 100 sekunder. Om du märker att API:et tar mer än 100 sekunder är det mycket troligt att frågan är syntaktiskt korrekt, annars skulle du ha fått en annan felkod än 200. Den faktiska rapportgenereringen skickar om frågesyntaxen är korrekt.

**Begärandesyntax**

|    Metod    |    URI för förfrågan    |
|    ----    |    ----    |
|    GET    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledQueries/testQueryResult?<exportQuery={query text}|queryId={queryId}>`    |
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
|    exportQuery     |    sträng    |    No    |    Rapportfrågesträng som måste köras     |
|    queryId     |    sträng    |    No    |    Ett giltigt befintligt fråge-ID. Ömsesidigt uteslutande med frågesträngen som anges i exportQuery-parametern    |
|    startTime     |    sträng    |    No    |    Starttid från vilken vi vill ha data. Det åsidosätter det tidsspann som anges i frågan    |
|    endTime     |    sträng    |    No    |    Sluttid tills vi vill ha data. Det åsidosätter det tidsspann som anges i frågan    |
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
Top 100 rows of query execution 
{ 
  "Value": [ 
    { 
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
|    TotalCount     |    Antal datauppsättningar i värdematrisen     |
|    Meddelande     |    Statusmeddelande från körningen av API:et     |
|    StatusCode     |    Resultatkod. Möjliga värden är 200, 400, 401, 403, 500     |
|        |        |
