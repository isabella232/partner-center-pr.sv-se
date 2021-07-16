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
# <a name="update-report-api"></a>Uppdatera rapport-API

Det här API:et hjälper dig att ändra en rapportparameter.

**Begärandesyntax**

|    Metod    |    URI för förfrågan    |
|    ----    |    ----    |
|    PUT    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport/{Report ID}`    |
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

**Ordlista**

I den här tabellen visas viktiga definitioner av element i svaret.

|    Parameter    |    Krävs    |    Beskrivning    |    Tillåtna värden    |
|    ----    |    ----    |    ----    |    ----    |
|    ReportName     |    Ja     |    Namn som ska tilldelas till rapporten     |    Sträng     |
|    Beskrivning     |    Nej     |    Beskrivning av den skapade rapporten     |    Sträng     |
|    StartTime     |    Ja    |    Tidsstämpel som rapportgenereringen ska börja efter     |    Sträng     |
|    RecurrenceInterval     |    Inga     |    Hur ofta rapporten ska genereras i timmar. Minimivärdet är 4     |    Integer     |
|    RecurrenceCount     |    Inga     |    Antal rapporter som ska genereras. Standardvärdet är obegränsad.     |    Integer     |
|    Format     |    Inga    |    Filformat för den exporterade filen. Standardvärdet är CSV     |    CSV/TSV     |
|    CallbackURL     |    Inga     |    URL för https-motringning som ska anropas vid rapportgenerering     |    Sträng     |
|    CallbackMethod    |    Inga    |    HTTP-metod som ska användas för återanrop    |    GET/POST    |
|        |        |        |        |


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
|    ReportId     |    Universell unik identifierare (UUID) för den rapport som uppdateras     |
|    ReportName     |    Namn som ges till rapporten i nyttolasten för begäran     |
|    Description     |    Beskrivning som ges till rapporten i begärandenyttolasten     |
|    QueryId     |    Fråge-ID som skickades när rapporten skapades     |
|    Söka i data     |    Frågetext som ska köras för den här rapporten     |
|    Användare     |    Användar-ID som används för att skapa rapporten     |
|    CreatedTime     |    Tiden då rapporten skapades. Tidsformatet är yyyy-MM-ddTHH:mm:ssZ     |
|    ModifiedTime     |    Tid då rapporten senast ändrades. Tidsformatet är yyyy-MM-ddTHH:mm:ssZ     |
|    ExecuteNow     |    ExecuteNow-flaggan som angetts när rapporten skapades    |
|    StartTime     |    Den tid då rapportkörningen börjar. Tidsformatet är yyyy-MM-ddTHH:mm:ssZ     |
|    ReportStatus     |    Status för rapportkörningen. Möjliga värden är Pausad, Aktiv och Inaktiv.     |
|    RecurrenceInterval     |    Upprepningsintervall som anges i nyttolasten för begäran     |
|    RecurrenceCount     |    Upprepningsantal som anges i nyttolasten för begäran     |
|    CallbackUrl     |    Motringning-URL som anges i begäran     |
|    CallbackMethod    |    Återanropsmetod som anges i begäran    |
|    Format     |    Format för rapportfilerna     |
|    TotalCount     |    Antal datauppsättningar i värdematrisen     |
|    Meddelande     |    Statusmeddelande från körningen av API:et     |
|    StatusCode     |    Resultatkod. Möjliga värden är 200, 400, 401, 403, 500     |
|        |        |