---
title: Hämta alla datauppsättnings-API :Insights data
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-insights
description: Använd det här API:et för att få information om alla tillgängliga datauppsättningar i Partner Center-insikter.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: 96bbb039c022d3587183b8dbec014bc362255b750ac6670fe3c1906629b7e291
ms.sourcegitcommit: 121f1b9cbd88faeba60dc9b475f9c0647cdc933c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/06/2021
ms.locfileid: "115693341"
---
# <a name="get-all-datasets-api"></a>Hämta alla datauppsättnings-API

API:et Hämta alla datauppsättningar hämtar alla tillgängliga datauppsättningar. Datauppsättningar visar tabeller, kolumner, mått och tidsintervall.

**Begärandesyntax**

|    Metod    |    URI för förfrågan    |
|    ----    |    ----    |
|    GET    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledDataset?datasetName={Dataset Name}`     |
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
|    datasetName    |    sträng    |    No    |    Filter för att hämta information om endast en datauppsättning    |
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

**Ordlista**

Den här tabellen definierar nyckelelementen i svaret:

|    Parameter    |    Beskrivning    |
|    ----    |    ----    |
|    DatasetName     |    Namnet på den datauppsättning som matrisobjektet definierar     |
|    SelectableColumns     |    Råkolumner som kan anges i select-kolumnerna     |
|    AvailableMetrics     |    Sammansättnings-/måttkolumnnamn som kan anges i select-kolumnerna     |
|    AvailableDateRanges     |    Datumintervall som kan användas i rapportfrågor för datauppsättningen     |
|    minimumRecurrenceInterval     |    Minsta värde för upprepningsintervall     |
|    TotalCount     |    Antal datauppsättningar i värdematrisen     |
|    Meddelande     |    Statusmeddelande från körningen av API:et     |
|    StatusCode     |    Resultatkod. Möjliga värden är 200, 400, 401, 403, 500     |
|        |        |
