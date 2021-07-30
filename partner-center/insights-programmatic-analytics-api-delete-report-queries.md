---
title: API för att ta bort rapportfrågor – Insights data
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-insights
description: Använd det här API:et för att ta bort användardefinierad fråga i Partner center-insikter.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: f755bc13ff4e0c4bc3a2c6ceda123c6a2bc47dc5
ms.sourcegitcommit: ad1af627f5ee6b6e3a70655f90927e932cf4c985
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 07/29/2021
ms.locfileid: "114836395"
---
# <a name="delete-report-queries-api"></a>API för att ta bort rapportfrågor

Det här API:et tar bort användardefinierade frågor.

**Begärandesyntax**

|    Metod    |    URI för förfrågan    |
|    ----    |    ----    |
|    DELETE    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledQueries/{queryId}` |
|        |        |

**Begärandehuvud**

|    Huvud    |    Typ    |    Beskrivning    |
|    ----    |    ----    |    ----    |
|    Auktorisering    |    sträng    |    Krävs. Åtkomsttoken Azure Active Directory (AAD) i formuläret`Bearer <token>`    |
|    Content-Type    |    sträng    |    `Application/JSON`    |
|        |        |        |

**Sökvägsparameter**

|    Parameternamn    |    Typ    |    Obligatorisk    |    Beskrivning    |
|    ----    |    ----    |    ----    |    ----    |
|    queryId     |    sträng     |    No    |    Filtrera för att hämta information om endast frågor med det ID som anges i argumentet     |
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
|    QueryId     |    Unikt UUID för frågan som togs bort    |
|    Namn     |    Namnet på den fråga som togs bort    |
|    Beskrivning     |    Beskrivning av den borttagna frågan     |
|    Söka i data     |    Rapportfrågesträng för den borttagna frågan    |
|    Typ     |    Ställ in på userDefined för användarskapade frågor     |
|    Användare     |    Användar-ID som skapade frågan     |
|    CreatedTime     |    Tid då frågan skapades     |
|    TotalCount     |    Antal datauppsättningar i värdematrisen     |
|    Meddelande     |    Statusmeddelande från körningen av API:et     |
|    StatusCode     |    Resultatkod. Möjliga värden är 200, 400, 401, 403, 500     |
|        |        |
