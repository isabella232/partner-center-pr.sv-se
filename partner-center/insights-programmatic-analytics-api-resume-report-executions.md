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
# <a name="resume-report-executions-api"></a>ÅTERUPPTA API för rapportkörningar

Vid körning återupptar detta API den schemalagda körningen av en pausad rapport.

**Begärandesyntax**

|    Metod    |    URI för förfrågan    |
|    ----    |    ----    |
|    PUT    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport/resume/{ReportID}`    |
|        |        |

**Begärandehuvud**

|    Huvud    |    Typ    |    Description    |
|    ----    |    ----    |    ----    |
|    Auktorisering    |    sträng    |    Krävs. Åtkomsttoken Azure Active Directory (AAD) i formuläret`Bearer <token>`    |
|    Content-Type    |    sträng    |    `Application/JSON`    |
|        |        |        |

**Sökvägsparameter**

|    Parameternamn    |    Typ    |    Obligatorisk    |    Beskrivning    |
|    ----    |    ----    |    ----    |    ----    |
|    reportId     |    sträng    |    No    |    ID för den rapport som ändras     |
|        |        |        |        |

**Frågeparameter**

Ingen

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

**Ordlista**

Den här tabellen definierar nyckelelementen i svaret:

|    Parameter    |    Beskrivning    |
|    ----    |    ----    |
|    ReportId     |    Universell unik identifierare (UUID) för den återupptagit rapporten     |
|    ReportName     |    Namn som ges till rapporten när den skapas     |
|    Description     |    Beskrivning som ges när rapporten skapas     |
|    QueryId     |    Fråge-ID som skickades när rapporten skapades     |
|    Söka i data     |    Frågetext som ska köras för den här rapporten     |
|    Användare     |    Användar-ID som används för att skapa rapporten     |
|    CreatedTime     |    Tid då rapporten skapades. Tidsformatet är yyyy-MM-ddTHH:mm:ssZ     |
|    ModifiedTime     |    Tid då rapporten senast ändrades. Tidsformatet är yyyy-MM-ddTHH:mm:ssZ     |
|    ExecuteNow     |    ExecuteNow-flaggan som angetts när rapporten skapades    |
|    StartTime     |    Den tid då rapportkörningen börjar. Tidsformatet är yyyy-MM-ddTHH:mm:ssZ     |
|    ReportStatus     |    Status för rapportkörningen. Möjliga värden är Pausad, Aktiv och Inaktiv.     |
|    RecurrenceInterval     |    Upprepningsintervall som angavs när rapporten skapades     |
|    RecurrenceCount     |    Antal upprepningar som angavs när rapporten skapades     |
|    CallbackUrl     |    Motringning-URL som anges i begäran     |
|    CallbackMethod    |    Återanropsmetod som anges i begäran    |
|    Format     |    Format för rapportfilerna     |
|    TotalCount     |    Antal datauppsättningar i värdematrisen     |
|    Meddelande     |    Statusmeddelande från körningen av API:et     |
|    StatusCode     |    Resultatkod. Möjliga värden är 200, 400, 401, 403, 500     |
|        |        |
