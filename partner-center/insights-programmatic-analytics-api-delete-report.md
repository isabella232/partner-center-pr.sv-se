---
title: Ta bort rapport-API – Insights data
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-insights
description: Använd det här API:et för att ta bort alla rapporter i Partner Center-insikter.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: 358e08363c203b82a5e80e2660be6e04224f58df393c94f8af9062fcb5ec67a7
ms.sourcegitcommit: 121f1b9cbd88faeba60dc9b475f9c0647cdc933c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/06/2021
ms.locfileid: "115697218"
---
# <a name="delete-report-api"></a>Ta bort rapport-API

Vid körning tar detta API bort alla rapport- och rapportkörningsposter.

**Begärandesyntax**

|    Metod    |    URI för förfrågan    |
|    ----    |    ----    |
|    DELETE    |    ` https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport/{Report ID}`    |
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
|    reportId     |    sträng    |    No    |    ID för rapporten som tas bort    |
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
|    ReportId     |    Universell unik identifierare (UUID) för den borttagna rapporten     |
|    ReportName     |    Namn som ges till rapporten när den skapades     |
|    Description     |    Beskrivning som anges när rapporten skapas     |
|    QueryId     |    Fråge-ID som skickades när rapporten skapades     |
|    Söka i data     |    Frågetext som ska köras för den här rapporten     |
|    Användare     |    Användar-ID som används för att skapa rapporten     |
|    CreatedTime     |    Tiden då rapporten skapades. Tidsformatet är yyyy-MM-ddTHH:mm:ssZ     |
|    ModifiedTime     |    Tid då rapporten senast ändrades. Tidsformatet är yyyy-MM-ddTHH:mm:ssZ     |
|    ExecuteNow     |    ExecuteNow-flaggan som angetts när rapporten skapades     |
|    StartTime     |    Den tid då rapportkörningen börjar. Tidsformatet är yyyy-MM-ddTHH:mm:ssZ     |
|    ReportStatus     |    Status för rapportkörningen. Möjliga värden är Pausad, Aktiv och Inaktiv.     |
|    RecurrenceInterval     |    Upprepningsintervall som anges när rapporten skapas     |
|    RecurrenceCount     |    Antal upprepningar som anges när rapporten skapas     |
|    CallbackUrl     |    Motringning-URL som anges i begäran     |
|    CallbackMethod    |    Återanropsmetod som anges i begäran    |
|    Format     |    Format för rapportfilerna     |
|    TotalCount     |    Antal datauppsättningar i värdematrisen     |
|    Meddelande     |    Statusmeddelande från körningen av API:et     |
|    StatusCode     |    Resultatkod. Möjliga värden är 200, 400, 401, 403, 500     |
|        |        |
