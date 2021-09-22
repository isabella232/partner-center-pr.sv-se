---
title: Paradigm för programmatisk åtkomst för insikter
description: Förstå flödet på hög nivå i API-anropsmönstret för programmatisk analys. API:erna för åtkomst till partnerinsiktsanalysrapporter omfattas också.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-insights
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 07/14/2021
ms.openlocfilehash: 304607b5d79b0ad8a07c3efe690ccb7feef83331
ms.sourcegitcommit: 23ba623b50b06c866703fd876f1b40f3a49ce504
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/22/2021
ms.locfileid: "128074622"
---
# <a name="programmatic-access-paradigm"></a>Paradigm för programmatisk åtkomst

Det här diagrammet visar api-anropsmönstret som används för att skapa en ny rapportmall, schemalägga den anpassade rapporten och hämta feldata.

:::image type="content" source="images/insights/prog-acc-paradigm.png" alt-text="Flöde på hög nivå":::
***Bild 1: Flöde på hög nivå för API-anropsmönstret***

Den här listan innehåller mer information om bild 1.

1. Klientprogrammet kan definiera det anpassade rapportschemat/-mallen genom att anropa [API:et för att skapa rapportfråga.](#create-report-query-api) Du kan också välja en rapportmall (QueryId) från exemplen på rapportmallbiblioteket i Lista över systemfrågor för programmatisk åtkomst [till partnerinsikter.](insights-programmatic-system-queries.md)
2. Om det lyckas returnerar API:et Skapa rapportfråga QueryId.
3. Klientprogrammet måste sedan anropa [](#create-report-api) API:et Skapa rapport med hjälp av QueryId tillsammans med rapportens startdatum, upprepningsintervall, upprepning och en valfri motringning-URI.
4. Vid lyckad, [returnerar API:et](#create-report-api) Skapa rapport ReportId.
5. Klientprogrammet meddelas på återanrops-URL:en så snart rapportdata är klara för nedladdning.
6. Klientprogrammet använder sedan [API:et Hämta rapportkörningar för](#get-report-execution-api) att fråga efter rapportens status med rapport-ID och datumintervall.
7. Om det lyckas returneras nedladdningslänken för rapporten och programmet kan starta nedladdningen av data.

## <a name="report-query-language-specification"></a>Specifikation för rapportfrågespråk

Vi tillhandahåller [systemfrågor som du kan](insights-programmatic-system-queries.md) använda för att skapa rapporter, men du kan också skapa egna frågor baserat på dina affärsbehov. Mer information om anpassade frågor finns i [Custom Query Specification](insights-programmatic-custom-query.md).

## <a name="create-report-query-api"></a>Skapa API för rapportfråga

API:et hjälper till att skapa anpassade frågor som definierar datauppsättningen som kolumner och mått måste exporteras från. API:et ger flexibiliteten att skapa en ny rapporteringsmall baserat på dina affärsbehov.  

Du kan också använda [de systemfrågor som](insights-programmatic-system-queries.md) vi tillhandahåller. När anpassade rapportmallar inte behövs kan du anropa [Skapa rapport-API](#create-report-api) direkt med hjälp av QueryIds för de systemfrågor som tillhandahålls.  

I följande exempel visas hur du skapar en anpassad fråga för att hämta de 10 främsta kunderna efter intäkter för den senaste månaden.

### <a name="request-syntax"></a>Begärandesyntax

|    Metod     |    URI för förfrågan     |
|----- | -----|
|    POST     |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledQueries`|
|||

### <a name="request-header"></a>Begärandehuvud

|    Huvud     |    Typ     |    Description     |
|-------|-----|------|
|    Auktorisering     |    sträng |Krävs. Åtkomsttoken Azure Active Directory (Azure AD). Formatet är  `Bearer <token>` .|
|    Content-Type     |sträng |`Application/JSON` |
||||

### <a name="path-parameter"></a>Sökvägsparameter

Ingen

### <a name="query-parameter"></a>Frågeparameter

Ingen

### <a name="sample-request-payload"></a>Nyttolast för exempelbegäran

```json
{ 
  "Name": "CustomersRevenueQuery", 
  "Description": "Query to get top 10 customers by revenue for last month", 
  "Query": "SELECT CustomerName, Product, BilledRevenueUSD FROM CustomersAndTenants ORDER BY BilledRevenueUSD LIMIT 10 TIMESPAN LAST_MONTH" 
}
```

### <a name="glossary"></a>Ordlista

Den här tabellen innehåller viktiga definitioner av element i begärandenyttolasten.

|Parameter|    Krävs     |    Beskrivning     |    Tillåtna värden     |
|-----|    -----    |    -----    |    -----    |
|Name |    Yes     |    Eget namn på frågan     |    sträng     |
|    Beskrivning     |    Nej     |    Beskrivning av vad frågan returnerar     |    sträng     |
|    Söka i data     |    Yes     |    Rapportfrågesträng     |    Datatyp: sträng <br> [Anpassad fråga](insights-programmatic-custom-query.md) baserat på affärs behov |
|        |        |        |        |

> [!Note]
> Anpassade frågeexempel finns i [Exempel på exempelfrågor.](insights-programmatic-sample-queries.md)

### <a name="sample-response"></a>Exempelsvar

Svarsnyttolasten är strukturerad på följande sätt:

Svarskoder: 200, 400, 401, 403, 500

Exempel på nyttolast för svar:

```json
{ 
  "value": [ 
    { 
      "queryId": "ec8366a4-d96e-4194-8c37-d5dbc0639033",
      "name": "CustomersRevenueQuery",
      "description": "Query to get top 10 customers by revenue for last month",
      "query": "SELECT CustomerName, Product, BilledRevenueUSD FROM CustomersAndTenants ORDER BY BilledRevenueUSD LIMIT 10 TIMESPAN LAST_MONTH",
      "type": "userDefined",
      "user": "GAUser@PITEST2.ccsctp.net", 
      "createdTime": "2021-03-30T12:52:39Z" 
    }
  ], 
  "nextLink": null,
  "totalCount": 1,
  "message": "Query created successfully",
  "statusCode": 200,
  "dataRedacted": false
} 
```

### <a name="glossary"></a>Ordlista

Den här tabellen innehåller viktiga definitioner av element i begärandenyttolasten.

|    Parameter     |    Beskrivning     |
|    ----    |    ----    |
|    QueryId     |    Universell unik identifierare (UUID) för den fråga som du skapade     |
|    Name     |    Eget namn som anges för frågan i begärandenyttolasten     |
|    Description     |    Beskrivning som anges när frågan skapas     |
|    Söka i data     |    Rapportfrågan skickades som indata när frågan skapades     |
|    Typ     |    Ange till `userDefined`     |
|    Användare     |    Användar-ID som användes för att skapa frågan     |
|    CreatedTime     |    UTC-tid då frågan skapades i det här formatet: yyyy-MM-ddTHH:mm:ssZ     |
|    TotalCount     |    Antal datauppsättningar i värdematrisen     |
|    StatusCode     |    Resultatkod <br> Möjliga värden är 200, 400, 401, 403, 500     |
|    meddelande     |    Statusmeddelande från körningen av API:et     |
|        |        |

## <a name="create-report-api"></a>Skapa rapport-API

När du skapar en anpassad rapportmall och [](#create-report-query-api) tar emot QueryID som en del av svaret från Skapa rapportfråga kan det här API:et anropas för att schemalägga en fråga som ska köras med jämna mellanrum. Du kan ange en frekvens och ett schema för rapporten som ska levereras.
För systemfrågor som vi tillhandahåller kan API:et Skapa rapport också anropas med [QueryId.](insights-programmatic-system-queries.md)

### <a name="callback-url"></a>Callback URL (Webbadress för återanrop)

API:et för att skapa rapport accepterar en återanrops-URL. Den här URL:en anropas när rapportgenereringen har lyckats. Motringning-URL:en ska vara offentligt åtkomlig. Förutom URL:en kan en motringningsmetod också ges. Motringningsmetoden kan bara vara "GET" eller "POST". Standardmetoden om inget värde skickas blir "POST". Det reportId som har slutfört genereringen skickas alltid tillbaka under återanropet.

POST-återanrop: Om URL:en som skickades var kommer den `https://www.contosso.com/callback` återanropade URL:en att vara `https://www.contosso.com/callback/<reportID>` 

GET-återanrop: Om URL:en som skickades var blir den `https://www.contosso.com/callback` anropade bakåt-URL:en `https://www.contosso.com/callback?reportId=<reportID>` 

### <a name="executenow-reports"></a>ExecuteNow-rapporter

Det finns en etablering för att generera en rapport utan schemaläggning. Api-nyttolasten för rapport som skapas kan acceptera en parameter , som kommer att lägga rapporten i en sekvens som ska genereras `ExecuteNow` så snart API:et anropas. När `ExecuteNow` är inställt på true ignoreras fälten: `StartTime` , eftersom dessa rapporter inte `RecurrenceCount` `RecurrenceInterval` schemaläggs.

Två ytterligare fält kan skickas när `ExecuteNow` är sant, `QueryStartTime` och `QueryEndTime` . De här två fälten `TIMESPAN` åsidosätter fältet i frågan. De här fälten gäller inte för schemalagda rapporter eftersom data genereras kontinuerligt under en fast tidsperiod som inte ändras.

### <a name="request-syntax"></a>Begärandesyntax

|    Metod     |    URI för förfrågan     |
|----- | -----|
|    POST     |`https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport` |

### <a name="request-header"></a>Begärandehuvud

|    Huvud     |    Typ     |    Description     |
|-------|-----|------|
|    Auktorisering     |    sträng |Krävs. Åtkomsttoken Azure Active Directory (Azure AD). Formatet är  `Bearer <token>` .|
|    Content-Type     |sträng |`Application/JSON` |

### <a name="path-parameter"></a>Sökvägsparameter

Ingen

### <a name="query-parameter"></a>Frågeparameter

Ingen

### <a name="sample-request-payload"></a>Nyttolast för exempelbegäran

```json
{
  "ReportName": "Top10_CustomersReport",
  "Description": "Top 10 customers by revenue for last month",
  "QueryId": "ec8366a4-d96e-4194-8c37-d5dbc0639033",
  "StartTime": "2021-03-31T18:41:00Z",
  "ExecuteNow": false,
  "QueryStartTime": null,
  "QueryEndTime": null,
  "RecurrenceInterval": 24,
  "RecurrenceCount": 100,
  "Format": "CSV",
  "CallbackUrl": "https://<SampleCallbackUrl>",
  "CallbackMethod": "GET"
}
```

### <a name="glossary"></a>Ordlista

Viktiga definitioner av element i nyttolasten för begäran förklaras nedan:

|    Parameter     |    Krävs     |    Beskrivning     |    Tillåtna värden     |
|    ----    |    ----    |    ----    |    ----    |
|    ReportName     |    Yes     |    Namn som ska tilldelas till rapporten     |    sträng     |
|    Beskrivning     |    Nej     |    Beskrivning av den skapade rapporten     |    sträng     |
|    QueryId     |    Yes     |    Rapportfråge-ID     |    sträng     |
|    StartTime     |    Yes     |    UTC-tidsstämpel där rapportgenereringen ska börja. <br> Formatet ska vara: yyyy-MM-ddTHH:mm:ssZ       |    sträng     |
|    ExecuteNow     |    No     |    Den här parametern ska användas för att skapa en rapport som bara ska köras en gång. `StartTime`, `RecurrenceInterval` och `RecurrenceCount` ignoreras om detta är inställt på true. Rapporten körs omedelbart på ett asynkront sätt     |    sant/falskt     |
|    QueryStartTime     |    No     |    Du kan också ange starttiden för frågan som extraherar data. Den här parametern gäller endast för körningsrapporter med en gång som har `ExecuteNow` angetts till true. Ange åsidosättningar för den `TIMESPAN` här parametern i frågan. Formatet ska vara yyyy-MM-ddTHH:mm:ssZ     |    Tidsstämpel som sträng     |
|    QueryEndTime     |    No     |    Du kan också ange sluttiden för frågan som extraherar data. Den här parametern gäller endast för en körningsrapport som har `ExecuteNow` angetts till true. Ange åsidosättningar för den `TIMESPAN` här parametern i frågan. Formatet ska vara yyyy-MM-ddTHH:mm:ssZ     |    Tidsstämpel som sträng     |
|    RecurrenceInterval     |    Yes     |    Frekvens i timmar då rapporten ska genereras. <br> Minimivärdet är 4 och Det högsta värdet är 2160.      |    heltal     |
|    RecurrenceCount     |    No     |    Antal rapporter som ska genereras.     |    heltal     |
|    Format     |    No     |    Filformat för den exporterade filen. <br> Standardvärdet är CSV.    |    "CSV"/"TSV"     |
|    CallbackUrl     |    No     |    Offentligt nåbar URL som kan konfigureras som återanropsmål     |    Sträng (http-URL)     |
|    CallbackMethod     |    No     |    Den metod som ska användas för återanrop     |    GET/POST     |
|        |        |        |        |

### <a name="sample-response"></a>Exempelsvar

Svarsnyttolasten är strukturerad på följande sätt:

Svarskoder: 200, 400, 401, 403, 404, 500

Exempel på nyttolast för svar:

```json
{ 
  "value": [
    { 
      "reportId": "d9548477-16d4-492a-bf9c-0cf91a9f69bf", 
      "reportName": "Top10_CustomersReport", 
      "description": "Top 10 customers by revenue for last month", 
      "queryId": "ec8366a4-d96e-4194-8c37-d5dbc0639033", 
      "query": "SELECT CustomerName, Product, BilledRevenueUSD FROM CustomersAndTenants ORDER BY BilledRevenueUSD LIMIT 10 TIMESPAN LAST_MONTH", 
      "user": "GAUser@PITEST2.ccsctp.net", 
      "createdTime": "2021-03-30T13:11:58Z", 
      "modifiedTime": null, 
      "executeNow": false, 
      "startTime": "2021-03-31T18:41:00Z", 
      "reportStatus": "Active", 
      "recurrenceInterval": 24, 
      "recurrenceCount": 100, 
      "callbackUrl": "https://<SampleCallbackUrl>", 
      "callbackMethod": "GET", 
      "format": "csv"
    } 
  ], 
  "nextLink": null, 
  "totalCount": 1, 
  "message": "Report created successfully", 
  "statusCode": 200, 
  "dataRedacted": false 
}
```

### <a name="glossary"></a>Ordlista

Viktiga definitioner av element i svaret förklaras nedan:

|    Parameter     |    Beskrivning     |
|    ----    |    ----    |
|    ReportId     |    Universell unik identifierare (UUID) för den rapport som du skapade     |
|    ReportName     |    Namn som ges till rapporten i nyttolasten för begäran     |
|    Description     |    Beskrivning som anges när rapporten skapas     |
|    QueryId     |    Fråge-ID som skickades när du skapade rapporten     |
|    Söka i data     |    Frågetext som ska köras för den här rapporten     |
|    Användare     |    Användar-ID som används för att skapa rapporten     |
|    CreatedTime     |    UTC-tid då rapporten skapades i det här formatet: yyyy-MM-ddTHH:mm:ssZ     |
|    ModifiedTime     |    UTC-tid då rapporten senast ändrades i det här formatet: yyyy-MM-ddTHH:mm:ssZ     |
|    ExecuteNow     |    `ExecuteNow` flagga som angetts när rapporten skapades     |
|    StartTime     |    UTC-tid då rapportkörningen börjar i det här formatet: yyyy-MM-ddTHH:mm:ssZ     |
|    ReportStatus     |    Status för rapportkörningen. Möjliga värden är `Paused` , `Active` och `Inactive`     |
|    RecurrenceInterval     |    Upprepningsintervall som anges när rapporten skapas     |
|    RecurrenceCount     |    Upprepningsantal som anges när rapporten skapas.      |
|    CallbackUrl     |    Motringning-URL som anges i begäran     |
|    CallbackMethod     |    Återanropsmetod som anges i begäran     |
|    Format     |    Format för rapportfilerna. Möjliga värden är `CSV` eller `TSV` .     |
|    TotalCount     |    Antal poster i värdematrisen     |
|    StatusCode     |    Resultatkod     |
|    meddelande     |    Möjliga värden är 200, 400, 401, 403, 500. Statusmeddelande från körningen av API:et     |
|        |        |

## <a name="get-report-execution-api"></a>Hämta API för rapportkörning

Du kan använda den här metoden för att fråga efter status för en rapportkörning med hjälp av ReportId som togs emot från Create Report API ( [Skapa rapport-API).](#create-report-api) Metoden returnerar nedladdningslänken för rapporten om rapporten är redo för nedladdning. Annars returnerar metoden statusen. Du kan också använda det här API:et för att hämta alla körningar som har inträffat för en viss rapport.  

>[!IMPORTANT]
>Det här API:et har standardfrågeparametrar för `executionStatus=Completed` och `getLatestExecution=true` . Om API:et anropas innan den första lyckade körningen av rapporten returneras därför 404. Väntande körningar kan hämtas genom att ange `executionStatus=Pending` .

### <a name="request-syntax"></a>Begärandesyntax

|    Metod     |    URI för förfrågan     |
|----- | -----|
|    GET    |`https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport/execution/{reportId}?executionId={executionId}&executionStatus={executionStatus}&getLatestExecution={getLatestExecution}`  |

### <a name="request-header"></a>Begärandehuvud

|    Huvud     |    Typ     |    Description     |
|-------|-----|------|
|    Auktorisering     |    sträng |Krävs. Åtkomsttoken Azure Active Directory (Azure AD). Formatet är  `Bearer <token>` .|
|    Content-Type     |sträng |`Application/JSON` |

### <a name="path-parameter"></a>Sökvägsparameter

|    Parameternamn    |    Krävs    |    Typ    |    Description    |
|    ----    |    ----    |    ----    |    ----    |
|    reportId    |    Yes    |    sträng    |    Filtrera för att hämta körningsinformation för endast rapporter med reportId som anges i det här argumentet. Flera reportIds kan anges genom att avgränsa dem med ett semikolon ";".    |
|        |        |        |        |

### <a name="query-parameter"></a>Frågeparameter

|    Parameternamn    |    Krävs    |    Typ    |    Description    |
|    ----    |    ----    |    ----    |    ----    |
|    executionId    |    No    |    sträng    |    Filtrera för att hämta information om endast rapporter med executionId som anges i det här argumentet. Flera executionIds kan anges genom att avgränsa dem med ett semikolon ";".    |
|    executionStatus    |    No    |    Sträng/uppräkning    |    Filtrera för att hämta information om endast rapporter med executionStatus som anges i det här argumentet. <br> Giltiga värden är: `Pending` , `Running` , och `Paused` `Completed` . <br> Standardvärdet är `Completed`. <br> Flera statusar kan anges genom att avgränsa dem med semikolon ";".    |
|    getLatestExecution    |    No    |    boolean    |    API:et returnerar information om den senaste körningen. Som standard är den här parametern inställd på true.<br> Om du väljer att skicka värdet för den här parametern som false returnerar API:et de senaste 90 dagarnas körningsinstanser.    |
|        |        |        |        |

### <a name="sample-request-payload"></a>Exempel på nyttolast för begäran

Ingen

### <a name="sample-response"></a>Exempelsvar

Svarsnyttolasten är strukturerad på följande sätt:

Svarskoder: 200, 400, 401, 403, 404, 500

Exempel på nyttolast för svar:

```json
{
  "value": [
    {
      "executionId": "906931dc-4f2f-4195-bbb2-d7295c7550d3",
      "reportId": "d9548477-16d4-492a-bf9c-0cf91a9f69bf",
      "recurrenceInterval": 24,
      "recurrenceCount": 100,
      "callbackUrl": null,
      "callbackMethod": null,
      "format": "csv",
      "executionStatus": "Completed",
      "reportLocation": null,
      "reportAccessSecureLink": "https://<path to report for download>",
      "reportExpiryTime": null,
      "reportGeneratedTime": "2021-03-31T18:41:00Z"
    }
  ],
  "nextLink": null,
  "totalCount": 1,
  "message": null,
  "statusCode": 200,
  "dataRedacted": false
}
```

När rapportkörningen är klar visas `Completed` körningsstatusen. Du kan ladda ned rapporten genom att välja URL:en i `reportAccessSecureLink` .

### <a name="glossary"></a>Ordlista

Viktiga definitioner av element i svaret.

|    Parameter    |    Beskrivning    |
|    ----    |    ----    |
|    ExecutionId    |    Universell unik identifierare (UUID) för körningsinstansen    |
|    ReportId    |    Rapport-ID som är associerat med körningsinstansen    |
|    RecurrenceInterval    |    Upprepningsintervall som anges när rapporten skapas    |
|    RecurrenceCount    |    Antal upprepningar som anges när rapporten skapas    |
|    CallbackUrl    |    Motringning-URL som är associerad med körningsinstansen    |
|    CallbackMethod    |    Återanropsmetod som är associerad med körningsinstansen    |
|    Format    |    Format för den genererade filen i slutet av körningen    |
|    ExecutionStatus    |    Status för rapportkörningsinstansen. <br> Giltiga värden är: `Pending` `Running` , , `Paused` och `Completed`    |
|    ReportAccessSecureLink    |Länk genom vilken rapporten kan nås på ett säkert sätt        |
|    ReportExpiryTime    |    UTC-tid efter vilken rapportlänken upphör att gälla i det här formatet: yyyy-MM-ddTHH:mm:ssZ    |
|    ReportGeneratedTime    |    UTC-tid då rapporten genererades i det här formatet: yyyy-MM-ddTHH:mm:ssZ    |
|    TotalCount    |    Antal datauppsättningar i värdematrisen    |
|    StatusCode    |    Resultatkod <br> Möjliga värden är 200, 400, 401, 403, 404 och 500    |
|    meddelande    |    Statusmeddelande från körningen av API:et    |
|        |        |

## <a name="next-steps"></a>Nästa steg

- Testa API:erna via [Swagger API-URL:en](https://api.partnercenter.microsoft.com/insights/v1/mpn/swagger/index.html)
- [Gör ditt första API-anrop] (insights-programmatic-first-api-call.md
