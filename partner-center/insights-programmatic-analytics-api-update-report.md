---
title: Uppdatera rapport-API
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-insights
description: Använd det här API:et för att uppdatera rapportparametrar i Partner Center-insikter.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: c4425f6444603852e87d9287db720ec1b29ee57818bc949c82eed2179ac6149e
ms.sourcegitcommit: 121f1b9cbd88faeba60dc9b475f9c0647cdc933c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/06/2021
ms.locfileid: "115696926"
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
|    reportId     |    sträng    |    No    |    ID för rapporten som ändras     |
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
|    ReportName     |    Yes     |    Namn som ska tilldelas till rapporten     |    Sträng     |
|    Beskrivning     |    Nej     |    Beskrivning av den skapade rapporten     |    Sträng     |
|    StartTime     |    Yes    |    Tidsstämpel som rapportgenereringen ska börja efter     |    Sträng     |
|    RecurrenceInterval     |    No     |    Hur ofta rapporten ska genereras i timmar. Minimivärdet är 4     |    Integer     |
|    RecurrenceCount     |    No     |    Antal rapporter som ska genereras. Standardvärdet är obestämd.     |    Integer     |
|    Format     |    No    |    Filformat för den exporterade filen. Standardvärdet är CSV     |    CSV/TSV     |
|    CallbackURL     |    No     |    HTTPS-motringning URL som ska anropas vid rapportgenerering     |    Sträng     |
|    CallbackMethod    |    No    |    HTTP-metod som ska användas för återanrop    |    GET/POST    |
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
|    Description     |    Beskrivning som ges till rapporten i nyttolasten för begäran     |
|    QueryId     |    Fråge-ID som skickades när rapporten skapades     |
|    Söka i data     |    Frågetext som ska köras för den här rapporten     |
|    Användare     |    Användar-ID som används för att skapa rapporten     |
|    CreatedTime     |    Den tid då rapporten skapades. Tidsformatet är yyyy-MM-ddTHH:mm:ssZ     |
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