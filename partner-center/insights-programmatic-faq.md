---
title: Vanliga frågor för programmatisk åtkomst till partnerinsikter
description: Få svar på vanliga frågor om åtkomst till partnerinsiktsdata via API.
ms.topic: troubleshooting
ms.service: partner-dashboard
ms.subservice: partnercenter-insights
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 07/14/2021
ms.openlocfilehash: 418af23ae50e1f8d9086b2eb6247ba964e4c1516
ms.sourcegitcommit: ad1af627f5ee6b6e3a70655f90927e932cf4c985
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 07/29/2021
ms.locfileid: "114836973"
---
# <a name="programmatic-access-of-analytics-data-common-questions"></a>Vanliga frågor om programmatisk åtkomst till analysdata

Den här artikeln tar upp vanliga frågor om hur du kommer åt partnerinsiktsdata programmatiskt i Partnercenter.

## <a name="api-responses"></a>API-svar

Under vilka olika scenarier kan jag få ett annat API-svar än 200 (lyckades)?

I den här tabellen beskrivs API-svaren och vad du kan göra om du får dem.

|    Felbeskrivning     |    Felkod     |    Felsöka     |
|    ----    |    ----    |    ----    |
|    Behörighet saknas     |    401     |    Det här är ett autentiseringsfel. Kontrollera att AAD-token Azure Active Directory korrekt. AAD-token är giltig i 60 minuter. Därefter måste du återskapa AAD-token.     |
|    Ogiltigt tabellnamn     |    400     |    Namnet på datauppsättningen är fel. Kontrollera datauppsättningens namn igen genom att anropa API:et "Hämta alla datauppsättningar".     |
|    Felaktigt kolumnnamn     |    400     |    Namnet på kolumnen i frågan är felaktigt. Kontrollera kolumnnamnet igen genom att anropa API:et "Hämta alla datauppsättningar" eller referera till kolumnnamnen i datadefinitionerna    |
|    Null- eller saknat värde     |    400     |    Du kanske saknar obligatoriska parametrar som en del av API:ets nyttolast för begäran.     |
|    Ogiltiga rapportparametrar     |    400     |    Kontrollera att rapportparametrarna är korrekta. Du kan till exempel ge ett värde på mindre än 4 för parametern RecurrenceInterval.     |
|    Upprepningsintervallet måste vara mellan 4 och 2160     |    400     |    Kontrollera att värdet för request-parametern RecurrenceInterval är mellan 4 och 2160.     |
|    Ogiltigt QueryId     |    400     |    Kontrollera det genererade QueryId igen.     |
|    Ogiltiga rapportparametrar för skapande – Starttiden för rapporten bör vara minst 4 timmar från aktuell UTC-tid     |    400     |    Starttidsparametern som en del av nyttolasten för begäran bör inte vara i det förflutna. Rapportens starttid bör vara minst 4 timmar från den aktuella UTC-tiden.     |
|    Det begärda värdet "sträng" hittades inte     |    400     |    Kontrollera om du har uppdaterat begärandeparametrarna `callbackurl` eller formatet.     |
|    Inget objekt hittades med angivna filter.     |    404     |    Kontrollera reportID-parametern som används i API:et För att hämta rapportkörningar.     |
|    Det finns inga körningar som har inträffat för de angivna filtervillkoren. Dubbelkolla reportId eller executionId och försök igen efter rapportens schemalagda körningstid     |    404     |    Kontrollera att reportId är korrekt. Försök igen med API:et efter rapportens schemalagda körningstid enligt vad som anges i nyttolasten för begäran.     |
|    Ett internt fel inträffade när rapporten skulle skapas. Korrelations-ID <>     |    500     |    Kontrollera att datumformatet för fälten *StartTime,* *QueryStartTime* och *QueryEndTime* är korrekta.     |
|    Tjänsten är inte tillgänglig    |    500     |    Om du kontinuerligt får en otillgänglig tjänst (5xx-fel) öppnar du en supportbiljett.    |
|        |        |        |

## <a name="no-records"></a>Inga poster

Jag får API-svar 200 när jag laddar ned rapporten från den säkra platsen. Varför får jag inga poster?
Kontrollera om strängen i frågan har ett av de tillåtna värdena för kolumnrubriken. Den här frågan returnerar till exempel noll resultat:

```sql
SELECT CustomerTenantId, CustomerTpId, WorkloadName, Month, MonthlyActiveUsers 
FROM OfficeUsage 
WHERE IsDuplicateRowForPGA = 'False' 
ORDER BY CustomerTenantId DESC
```

I det här exemplet är de tillåtna värdena `IsDuplicateRowForPGA` för 0 eller 1. Se [Datadefinitioner för](insights-data-definitions.md) alla möjliga värden för de olika kolumnerna.
