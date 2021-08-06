---
title: Specifikation för anpassad fråga
description: Lär dig hur du skapar anpassade frågor för att extrahera data från analystabeller.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-insights
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 07/14/2021
ms.openlocfilehash: 8749e9c65a232514028e0842a020267d0df7fcadcd9f36ac9dd9ba165377f401
ms.sourcegitcommit: 121f1b9cbd88faeba60dc9b475f9c0647cdc933c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/06/2021
ms.locfileid: "115696927"
---
# <a name="custom-query-specification"></a>Specifikation för anpassad fråga

Partner kan använda den här frågespecifikationen för att enkelt formulera anpassade frågor för att extrahera data från analystabeller. Frågorna kan bara användas för att välja önskade kolumner och mått som matchar ett visst kriterium. Kärnan i språkspecifikationen är datauppsättningsdefinitionen som en anpassad fråga kan skrivas på.

## <a name="datasets"></a>Datauppsättningar

På samma sätt som vissa frågor körs mot en databas som har tabeller och kolumner fungerar en anpassad fråga på datauppsättningar som har kolumner och mått. En fullständig lista över tillgängliga datauppsättningar för att utforma en fråga kan hämtas med hjälp av API:et för datauppsättningar.

Det här är ett exempel på en datauppsättning som visas som en JSON:

```json
{ 
      "datasetName": "OfficeUsage", 
      "selectableColumns": [ 
        "CustomerTenantId", 
        "CustomerTpid", 
        "WorkloadName", 
        "Month", 
        "PaidAvailableUnits", 
        "MonthlyActiveUsers", 
        "CustomerName", 
        "CustomerMarket", 
        "CustomerSegment",  
        "MPNId", 
        "PartnerName", 
        "PartnerLocation", 
        "PartnerAttributionType", 
        "IsDuplicateRowForPGA" 
      ], 
      "availableMetrics": [ 
        "CustomerCount", 
        "CustomerTenantCount", 
        "TotalPaidAvailableUnits", 
        "TotalMonthlyActiveUsers" 
      ], 
      "availableDateRanges": [ 
        "LAST_MONTH", 
        "LAST_3_MONTHS", 
        "LAST_6_MONTHS", 
        "LAST_1_YEAR", 
        "LIFETIME" 
      ], 
      "minimumRecurrenceInterval": 24 
    },
```

## <a name="parts-of-a-dataset"></a>Delar av en datauppsättning

- Ett datauppsättningsnamn är som ett databastabellnamn. Till exempel OfficeUsage. En datauppsättning har en lista över kolumner som kan väljas, till exempel CustomerTenantId.
- En datauppsättning har också mått, som är som aggregeringsfunktioner i en databas. Till exempel TotalMonthlyActiveUsers.
- Det finns fasta tidsintervall för vilka data kan exporteras.

## <a name="formulating-a-query-on-a-dataset"></a>Utforma en fråga på en datauppsättning

Det här är några exempelfrågor som visar hur du extraherar olika typer av data.

|Söka i data|    Description    |
|----|    ----    |
|**SELECT** CustomerTenantId, PaidAvailableUnits **FROM** <br>OfficeUsage **TIMESPAN** LAST_MONTH|    Den här frågan hämtar varje CusotmerTenantID och dess motsvarande PaidAvailableUnits under den senaste månaden.    |
|**SELECT** CustomerTenantId, PaidAvailableUnits **FROM** <br>OfficeUsage **ORDER** BY PaidAvailableUnits **LIMIT** 10|    Den här frågan hämtar de 10 främsta kundklienterna i fallande ordning efter antalet betalda tillgängliga enheter.     |
|**SELECT** CustomerTenantId, PaidAvailableUnits, MonthlyActiveUsers **FROM** OfficeUsage **WHERE** MonthlyActiveUsers > 100000 **ORDER BY** MonthlyActiveUsers **TIMESPAN** LAST_6_MONTHS |    Den här frågan hämtar PaidAvailableUnits och MonthlyActiveUsers för alla kunder som har MonthlyActiveUsers som är större än 100 000.     |
|**SELECT** CustomerTenantId, Month, MonthlyActiveUsers **FROM** <br>OfficeUsage **WHERE** CustomerTpId IN ('2a31c234-1f4e-4c60-909e-76d234f93161', '80780748-3f9a-11eb-b378-0242ac130002') |    Den här frågan hämtar CustomerTenantId och de månatliga aktiva användarna för varje månad med de två CustomerTpId-värdena: "2a31c234-1f4e-4c60-909e-76d234f93161" och "80780748-3f9a-11eb-b378-0242ac130002".     |
|        |        |

## <a name="query-specification"></a>Frågespecifikation

I det här avsnittet beskrivs frågedefinitionen och strukturen.

## <a name="grammar-reference"></a>Grammatikreferens

I den här tabellen beskrivs de symboler som används i frågor.

|    Söka i data    |    Description    |
|    ----    |    ----    |
|    `?`    |    Valfritt    |
|    `*`    |    Noll eller mer    |
|    `+`    |    En eller flera    |
|    `\|`    |    Eller/ en av listorna    |
|        |        |

## <a name="query-definition"></a>Frågedefinition

Frågesatsen har följande satser: SelectClause, FromClause, WhereClause, OrderClause, LimitClause och TimeSpan.

- **VäljClause**: `SELECT ColumOrMetricName (, ColumOrMetricName)*`
    - **ColumOrMetricName:** Kolumner och mått som definierats i datauppsättningen
- **FromClause**: `FROM DatasetName`
    - **DatasetName:** Datauppsättningens namn som definierats i datauppsättningen
- **WhereClause**: `WHERE FilterCondition (AND FilterCondition)`
    - **FilterCondition:** ColumOrMetricName Operator Value
        - **Operator**:  `=` | `>` | `<` | `>=` | `<=` | `!=` | `LIKE` | `NOT LIKE` | `IN` | `NOT IN`
        - **Värde:**| StringLiteral-| MultiNumberList-| MultiStringList
            - **Nummer**: `-? [0-9]+ (. [0-9] [0-9]*)?`
            - **StringLiteral**:  `' [a-zA-Z0-9_]*'`
            - **MultiNumberList:**`(Number (,Number)*)`
            - **MultiStringList:**`(StringLiteral (,StringLiteral)*)`
- **OrderClause**: `ORDER BY OrderCondition (,OrderCondition)`
    - **OrderCondition**: `ColumOrMetricName (ASC | DESC)*`
- **LimitClause:**`LIMIT [0-9]+`
- **TimeSpan**: `TIMESPAN ( TODAY | YESTERDAY | LAST_7_DAYS | LAST_14_DAYS |LAST_30_DAYS | LAST_90_DAYS | LAST_180_DAYS | LAST_365_DAYS |LAST_MONTH | LAST_3_MONTHS | LAST_6_MONTHS | LAST_1_YEAR | LIFETIME)`

## <a name="query-structure"></a>Frågestruktur

En rapportfråga består av flera delar:
- `SELECT`
- `FROM`
- `WHERE`
- `ORDER BY`
- `LIMIT`
- `TIMESPAN`

Varje del beskrivs nedan.

### `SELECT`

Den här delen av frågan anger vilka kolumner som ska exporteras. De kolumner som kan väljas är de fält som listas i *selectableColumns och* *availableMetrics-avsnitten* i en datauppsättning.

Nyckelord kan `DISTINCT` också anges efter `SELECT` . Om `DISTINCT` anges innehåller de slutliga exporterade raderna alltid distinkta värden för de valda kolumnerna. Mått beräknas för varje distinkt kombination av de valda kolumnerna, och därför krävs inte nyckelord när en måttkolumn ingår `DISTINCT` i listan välj kolumn.

**Exempel:**

```sql
SELECT CustomerTenantId, PaidAvailableUnits; 
SELECT DISTINCT CustomerTenantId
```

### `FROM`

Den här delen av frågan anger datauppsättningen som data behöver exporteras från. Datauppsättningens namn som anges här måste vara ett giltigt datauppsättningsnamn som returneras av API:et för datauppsättningar.

**Exempel:**

- `FROM  OfficeUsage`
- `FROM  AzureUsage`

### `WHERE`

Den här delen av frågan används för att ange filtervillkor för datauppsättningen. Endast rader som matchar alla villkor som anges i den här satsen finns i den slutliga exporterade filen. Filtervillkoret kan finnas på vilken som helst av kolumnerna som anges *i selectableColumns* och *availableMetrics*. Värdena som anges i filtervillkoret kan vara en lista med tal eller en lista med strängar endast när operatorn `IN` är eller `NOT IN` . Värdena kan alltid anges som en literalsträng och de konverteras till de interna typerna av kolumner. Flera filtervillkor måste avgränsas med en AND-åtgärd.

**Exempel:**

- `CustomerTenantId= '868368da-957d-4959-8992-3c12dc7e6260'`
- `CustomerName LIKE '%Contoso%'`
- `CustomerId NOT IN (1000, 1001, 1002)`
- `OrderQuantity=100`
- `CustomerTenantId='7b487ac0-ce12-b732-dcd6-91a1e4e74a50' AND CustomerTpId=' 0f8b7fa0-eb83-a183-1225-ca153ef807aa'`

### `ORDER BY`

Den här delen av frågan anger ordningskriterierna för de exporterade raderna. Kolumnerna som ordningen kan definieras på måste vara från *selectableColumns* och *availableMetrics för* datauppsättningen. Om det inte finns någon angiven ordningsriktning anges den som standard till DESC i kolumnen. Du kan definiera ordning på flera kolumner genom att avgränsa villkoren med ett kommatecken.

**Exempel:**

- `ORDER BY  MonthlyActiveUsers ASC,  Month DESC`
- `ORDER BY CustomerName ASC,  Month`

### `LIMIT`

Den här delen av frågan anger antalet rader som ska exporteras. Talet du anger måste vara ett positivt heltal som inte är noll.

### `TIMESPAN`

Den här delen av frågan anger hur länge data ska exporteras. Möjliga värden ska vara från fältet *availableDateRanges* i datauppsättningens definition.

### <a name="case-sensitivity-in-query-specification"></a>Ärendekänslighet i frågespecifikationen

Specifikationen är helt okänslig. Fördefinierade nyckelord, kolumnnamn och värden kan anges med versaler eller gemener.

## <a name="next-steps"></a>Nästa steg

- [Lista över systemfrågor](insights-programmatic-system-queries.md)
- [Lista över exempelfrågor](insights-programmatic-sample-queries.md)