---
title: Roller, behörigheter för partner-intjänad kredit
ms.topic: article
ms.date: 05/04/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
description: Lär dig mer om roller och behörigheter för partner för att kunna tjäna partner-intjänade krediter (PEC). Dessa skiljer sig från roller för att arbeta i Partnercenter.
author: adamyeh
ms.author: adamyeh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: ca9cd1b09c840531c3652f71afbd9c66f657f877
ms.sourcegitcommit: ad1af627f5ee6b6e3a70655f90927e932cf4c985
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 07/29/2021
ms.locfileid: "114840390"
---
# <a name="roles-and-permissions-required-to-earn-partner-earned-credit"></a>Roller och behörigheter som krävs för att få partner-intjänad kredit

Följande roller mappar till behörighetsnivåer som avgör om en partner är berättigad till partner-intjänade krediter.

>[!Important]
>Dessa roller och behörigheter är inte samma som de roller och behörigheter som en användare behöver för att arbeta i Partnercenter.

|**Role**   |**Beskrivning**   |**PEC-berättigad**   |
|-----------------|:------------------|:--------------|
|Ägare  |Du hanterar allt, inklusive åtkomst till resurser.|Ja|
|Deltagare |Du hanterar allt utom att bevilja åtkomst till resurser.|Ja|
|Läsare|Du kan visa allt, men inte göra några ändringar|Inga|
|ACRDelete|acr delete|Ja|
|ACRImageSigner|acr image signer|Ja|
|ACRPull|acr pull|Ja|
|AcrPush|acr push|Ja|
|AcrQuarantineReader|acr quarantine data reader|Inga|
|AcrQuarantineWriter| acr quarantine data writer|Ja|
|API Management tjänstdeltagare|Kan hantera tjänsten och API:erna|Ja|
|API Management tjänstoperatörsroll|Kan hantera tjänsten men inte API:erna|Ja|
|API Management-tjänstläsarroll|Skrivskyddade åtkomst till tjänsten och API:er|Inga|
|Deltagare Insights programkomponent|Hanterar program Insights komponenter|Ja|
|Program Insights Snapshot Debugger|Ger användaren behörighet att visa och ladda ned ögonblicksbilder av felsökning som samlats in med Insights Snapshot Debugger. Observera att dessa behörigheter inte ingår i rollerna Ägare eller Deltagare.|Ja|
Automation-jobboperator | Skapa och hantera jobb med Automation Runbooks. | Ja | 
Automation-operatör | Automation-operatörer kan starta, stoppa, pausa och återuppta jobb | Ja | 
Automation Runbook-operatör | Läsa Runbook-egenskaper – för att kunna skapa jobb för runbooken. | Ja | 
Avere-deltagare | Kan skapa och hantera ett Avere vFXT kluster. | Ja | 
Avere-operator | Används av Avere vFXT för att hantera klustret | Ja | 
Azure Event Hubs dataägare | Ger fullständig åtkomst till Azure Event Hubs resurser. | Ja | 
Azure Event Hubs datamottagare | Tillåter åtkomst till Azure Event Hubs resurser. | Ja | 
Azure Event Hubs Data Sender | Tillåter att åtkomst skickas till Azure Event Hubs resurser. | Ja | 
Azure Kubernetes Service administratörsroll för kluster | Visa en lista över autentiseringsuppgifter för klusteradministratör. | Ja | 
Azure Kubernetes Service klusteranvändarroll | Visa en lista över åtgärder för klusteranvändares autentiseringsuppgifter. | Ja | 
Azure Kartor Data Reader (förhandsversion) | Ger åtkomst till läsmappningsrelaterade data från ett Azure Maps-konto. | Inga | 
Azure Service Bus dataägare | Ger fullständig åtkomst till Azure Service Bus resurser. | Ja | 
Azure Service Bus Data Receiver | Tillåter åtkomst till Azure Service Bus resurser. | Ja | 
Azure Service Bus Data Sender | Tillåter att du skickar åtkomst till Azure Service Bus resurser. | Ja | 
Azure Stack registreringsägare | Låter dig hantera Azure Stack registreringar. | Ja | 
Säkerhetskopieringsdeltagare | Låter dig hantera säkerhetskopieringstjänsten, men kan inte skapa valv och ge åtkomst till andra | Ja | 
Operator för säkerhetskopiering | Låter dig hantera säkerhetskopieringstjänster, förutom borttagning av säkerhetskopiering, valvskapande och att ge åtkomst till andra | Ja | 
Backup Reader | Kan visa säkerhetskopieringstjänster, men kan inte göra ändringar | Inga | 
Faktureringsläsare | Ger läsåtkomst till faktureringsdata | Inga | 
BizTalk-deltagare | Låter dig hantera BizTalk-tjänster, men inte åtkomst till dem. | Ja | 
Åtkomst till blockkedjemedlemsnod (förhandsversion) | Tillåter åtkomst till blockkedjemedlemsnoder | Ja | 
Skissdeltagare | Kan hantera skissdefinitioner, men inte tilldela dem. | Ja | 
Skissoperatör | Kan tilldela befintliga publicerade skisser, men kan inte skapa nya skisser. Obs! Detta fungerar bara om tilldelningen görs med en användar tilldelad hanterad identitet. | Ja | 
CDN Slutpunktsdeltagare | Kan hantera CDN slutpunkter, men kan inte bevilja åtkomst till andra användare. | Ja | 
CDN Slutpunktsläsare | Kan visa CDN slutpunkter, men kan inte göra ändringar. | Inga | 
CDN Profildeltagare | Kan hantera CDN profiler och deras slutpunkter, men kan inte bevilja åtkomst till andra användare. | Ja | 
CDN Profilläsare | Kan visa CDN profiler och deras slutpunkter, men kan inte göra ändringar. | Inga | 
Klassisk nätverksdeltagare | Låter dig hantera klassiska nätverk, men inte åtkomst till dem. | Ja | 
Klassisk Storage-kontodeltagare | Låter dig hantera klassiska lagringskonton, men inte åtkomst till dem. | Ja | 
Tjänstroll Storage klassisk Storage-kontonyckeloperatör | Operatorer Storage klassiska kontonycklar kan visa och återskapa nycklar på klassiska Storage konton | Ja | 
Klassisk virtuell datordeltagare | Låter dig hantera klassiska virtuella datorer, men inte åtkomst till dem, och inte det virtuella nätverket eller lagringskontot som de är anslutna till. | Ja | 
Cognitive Services deltagare | Låter dig skapa, läsa, uppdatera, ta bort och hantera nycklar för Cognitive Services. | Ja | 
Cognitive Services dataläsare (förhandsversion) | Låter dig läsa Cognitive Services data. | Inga | 
Cognitive Services användare | Låter dig läsa och lista nycklar för Cognitive Services. | Inga | 
Cosmos DB rollen Kontoläsare | Kan läsa Azure Cosmos DB-kontodata. Se DocumentDB-kontodeltagare för att hantera Azure Cosmos DB konton. | Inga | 
Cosmos DB Operator | Låter dig hantera Azure Cosmos DB-konton, men inte komma åt data i dem. Förhindrar åtkomst till kontonycklar och anslutningssträngar. | Ja | 
CosmosBackupOperator | Kan skicka återställningsbegäran för en Cosmos DB databas eller en container för ett konto | Ja | 
Cost Management-deltagare | Kan visa kostnader och hantera kostnadskonfiguration (t.ex. budgetar, exporter) | Ja | 
Cost Management Läsare | Kan visa kostnadsdata och konfiguration (t.ex. budgetar, exporter) | Inga | 
Data Box-enhet deltagare | Låter dig hantera allt under Data Box-enhet service förutom att ge åtkomst till andra. | Ja | 
Data Box-enhet Läsare | Låter dig hantera Data Box-enhet-tjänsten, förutom att skapa beställnings- eller redigeringsinformation och ge åtkomst till andra. | Inga | 
Data Factory deltagare | Skapa och hantera datafabriker samt underordnade resurser i dem. | Ja | 
Data Lake Analytics utvecklare | Låter dig skicka, övervaka och hantera dina egna jobb, men inte skapa eller ta bort Data Lake Analytics konton. | Ja | 
Datarensning | Kan rensa analysdata | Ja | 
DevTest Labs-användare | Låter dig ansluta, starta, starta om och stänga av dina virtuella datorer i Azure DevTest Labs. | Ja | 
DNS-zondeltagare | Låter dig hantera DNS-zoner och postuppsättningar i Azure DNS, men låter dig inte styra vem som har åtkomst till dem. | Ja | 
DocumentDB-kontodeltagare | Kan hantera Azure Cosmos DB konton. Azure Cosmos DB kallades tidigare DocumentDB. | Ja | 
EventGrid EventSubscription-deltagare | Låter dig hantera eventGrid-händelseprenumerationsåtgärder. | Ja | 
EventGrid EventSubscription-läsare | Låter dig läsa EventGrid-händelseprenumerationer. | Inga | 
HDInsight-klusteroperator | Gör att du kan läsa och ändra HDInsight-klusterkonfigurationer. | Ja | 
HDInsight Domain Services-deltagare | Kan läsa, skapa, ändra och ta bort Domain Services-relaterade åtgärder som krävs för HDInsight-Enterprise Security Package | Ja | 
Intelligent Systems-kontodeltagare | Låter dig hantera konton för intelligenta system, men inte åtkomst till dem. | Ja | 
Key Vault deltagare | Låter dig hantera nyckelvalv, men inte åtkomst till dem. | Ja | 
Labbskapare | Låter dig skapa, hantera och ta bort dina hanterade labb under dina Azure Lab-konton. | Ja | 
Log Analytics Contributor | Log Analytics-deltagare kan läsa alla övervakningsdata och redigera övervakningsinställningar. Redigering av övervakningsinställningar omfattar att lägga till VM-tillägget till virtuella datorer. läsa lagringskontonycklar för att kunna konfigurera insamling av loggar från Azure Storage; skapa och konfigurera Automation-konton; lägga till lösningar; och konfigurera Azure Diagnostics på alla Azure-resurser. | Ja | 
Log Analytics Reader | Log Analytics-läsare kan visa och söka efter alla övervakningsdata samt visa övervakningsinställningar, inklusive att visa konfigurationen av Azure Diagnostics på alla Azure-resurser. | Inga | 
Logic App-deltagare | Låter dig hantera logikappar, men inte ändra åtkomsten till dem. | Ja | 
Logic App-operatör | Låter dig läsa, aktivera och inaktivera logikappar, men inte redigera eller uppdatera dem. | Ja | 
Operatörsroll för hanterat program | Låter dig läsa och utföra åtgärder på hanterade programresurser | Ja | 
Läsare för hanterade program | Låter dig läsa resurser i en hanterad app och begära JIT-åtkomst. | Inga | 
Hanterad identitetsdeltagare | Skapa, läsa, uppdatera och ta bort användar tilldelad identitet | Ja | 
Operatör för hanterad identitet | Läsa och tilldela användar tilldelad identitet | Ja | 
Deltagare i hanteringsgrupp | Deltagarroll för hanteringsgrupp | Ja | 
Läsare för hanteringsgrupp | Läsarroll för hanteringsgrupp | Inga | 
Övervakningsdeltagare | Kan läsa alla övervakningsdata och redigera övervakningsinställningar. Se även Kom igång med roller, behörigheter och säkerhet med Azure Monitor. | Ja | 
Övervaka Publisher | Aktiverar publiceringsmått mot Azure-resurser | Ja | 
Övervakningsläsare | Kan läsa alla övervakningsdata (mått, loggar osv.). Se även Kom igång med roller, behörigheter och säkerhet med Azure Monitor. | Inga | 
Nätverksdeltagare | Låter dig hantera nätverk, men inte åtkomst till dem. | Ja | 
New Relic APM-kontodeltagare | Låter dig hantera New Relic Application Performance Management och program, men inte åtkomst till dem. | Ja | 
Läsar- och dataåtkomst | Låter dig visa allt, men du kan inte ta bort eller skapa ett lagringskonto eller en innesluten resurs. Det ger också läs-/skrivåtkomst till alla data som finns i ett lagringskonto via åtkomst till lagringskontonycklar. | Ja | 
Redis Cache deltagare | Låter dig hantera Redis-cacher, men inte åtkomst till dem. | Ja | 
Resursprincipdeltagare (förhandsversion) | (Förhandsversion) Återifyllda användare från EA, med behörighet att skapa/ändra resursprincip, skapa supportbiljett och läsa resurser/hierarki. | Ja | 
Deltagare i Scheduler-jobbsamlingar | Låter dig hantera Scheduler-jobbsamlingar, men inte åtkomst till dem. | Ja | 
Search Service Contributor | Låter dig hantera Söktjänster, men inte åtkomst till dem. | Ja | 
Säkerhetsadministratör | Endast Security Center: Kan visa säkerhetsprinciper, visa säkerhets tillstånd, redigera säkerhetsprinciper, visa aviseringar och rekommendationer, stänga aviseringar och rekommendationer | Ja | 
Security Manager (äldre) | Det här är en äldre roll. Använd säkerhetsadministratören i stället | Ja | 
Säkerhetsläsare | Endast Security Center: Kan visa rekommendationer och aviseringar, visa säkerhetsprinciper, visa säkerhets tillstånd, men kan inte göra ändringar | Inga | 
Site Recovery-deltagare | Låter dig hantera Site Recovery förutom valvskapande och rolltilldelning | Ja | 
Site Recovery-operatör | Låter dig redundans och återställning efter fel, men inte utföra Site Recovery av hanteringsåtgärder | Ja | 
Site Recovery-läsare | Låter dig visa Site Recovery status men inte utföra andra hanteringsåtgärder | Inga | 
Spatial Anchors-kontodeltagare | Låter dig hantera spatiala fästpunkter i ditt konto, men inte ta bort dem | Ja | 
Spatial Anchors kontoägare | Låter dig hantera spatiala fästpunkter i ditt konto, inklusive att ta bort dem | Ja | 
Spatial Anchors-kontoläsare | Gör att du kan hitta och läsa egenskaper för spatiala fästpunkter i ditt konto | Inga | 
SQL DB-deltagare | Låter dig hantera SQL databaser, men inte åtkomst till dem. Du kan inte heller hantera deras säkerhetsrelaterade principer eller deras överordnade SQL servrar. | Ja | 
SQL Deltagare för hanterad instans | Låter dig hantera SQL hanterade instanser och nödvändig nätverkskonfiguration, men kan inte ge åtkomst till andra. | Ja | 
SQL-säkerhetshanteraren | Låter dig hantera säkerhetsrelaterade principer för SQL och databaser, men inte åtkomst till dem. | Ja | 
SQL Server Bidragsgivare | Låter dig hantera SQL och databaser, men inte åtkomst till dem, och inte deras säkerhetsrelaterade principer. | Ja | 
Lagringskontodeltagare | Tillåter hantering av lagringskonton. Ger åtkomst till kontonyckeln, som kan användas för att komma åt data via auktorisering med delad nyckel. | Ja | 
Storage Tjänstroll för kontonyckeloperatör | Tillåter att åtkomstnycklar för lagringskontot listas och återskapas. | Ja | 
Storage Blob Data-deltagare | Läsa, skriva och ta bort Azure Storage containrar och blobar. Information om vilka åtgärder som krävs för en viss dataåtgärd finns i Behörigheter för att anropa blob- och ködataåtgärder. | Ja | 
Storage Blob Data-ägare | Ger fullständig åtkomst till Azure Storage blobcontainrar och data, inklusive tilldelning av POSIX-åtkomstkontroll. Information om vilka åtgärder som krävs för en viss dataåtgärd finns i Behörigheter för att anropa blob- och ködataåtgärder. | Ja | 
Storage Blob Data-läsare | Läs och lista Azure Storage containrar och blobar. Information om vilka åtgärder som krävs för en viss dataåtgärd finns i Behörigheter för att anropa blob- och ködataåtgärder. | Inga | 
Storage Blob Dele blob | Hämta en nyckel för användardelegering som sedan kan användas för att skapa en signatur för delad åtkomst för en container eller blob som har signerats med Azure AD-autentiseringsuppgifter. Mer information finns i Skapa en SAS för användardelegering. | Ja | 
Storage-fildata för SMB-resursdeltagare | Tillåter läs-, skriv- och borttagningsåtkomst i Azure Storage över SMB | Ja | 
Storage-fildata för upphöjd SMB-resursdeltagare | Tillåter läs-, skriv-, borttagnings- och ändringsbehörighet för NTFS i Azure Storage över SMB | Ja | 
Storage-fildata för SMB-resursläsare | Tillåter läsåtkomst till Azure-filresurs via SMB | Inga | 
Storage Ködatadeltagare | Läsa, skriva och ta bort Azure Storage köer och kömeddelanden. Information om vilka åtgärder som krävs för en viss dataåtgärd finns i Behörigheter för att anropa blob- och ködataåtgärder. | Ja | 
Storage Processor för ködatameddelande | Granska, hämta och ta bort ett meddelande från en Azure Storage kö. Information om vilka åtgärder som krävs för en viss dataåtgärd finns i Behörigheter för att anropa blob- och ködataåtgärder. | Ja | 
Storage Avsändare av ködatameddelande | Lägga till meddelanden i en Azure Storage kö. Information om vilka åtgärder som krävs för en viss dataåtgärd finns i Behörigheter för att anropa blob- och ködataåtgärder. | Ja | 
Storage Ködataläsare | Läsa och lista Azure Storage köer och kömeddelanden. Information om vilka åtgärder som krävs för en viss dataåtgärd finns i Behörigheter för att anropa blob- och ködataåtgärder. | Inga | 
Supportbegärandedeltagare | Låter dig skapa och hantera supportbegäranden | Ja | 
Traffic Manager Bidragsgivare | Låter dig hantera Traffic Manager profiler, men låter dig inte styra vem som har åtkomst till dem. | Ja | 
Administratör för användaråtkomst | Låter dig hantera användaråtkomst till Azure-resurser. | Ja | 
Administratörsinloggning för virtuell dator | Visa Virtual Machines i portalen och logga in som administratör | Ja | 
Virtuell datordeltagare | Låter dig hantera virtuella datorer, men inte åtkomst till dem, och inte det virtuella nätverket eller lagringskontot som de är anslutna till. | Ja | 
Användarinloggning för virtuell dator | Visa Virtual Machines i portalen och logga in som en vanlig användare. | Ja | 
Webbplansdeltagare | Låter dig hantera webbplaner för webbplatser, men inte åtkomst till dem. | Ja | 
Webbplatsdeltagare | Låter dig hantera webbplatser (inte webbplaner), men inte åtkomst till dem | Ja |

## <a name="next-steps"></a>Nästa steg

- [Partner-intjänad kredit – en översikt över hur det fungerar i den nya handelsupplevelsen i CSP](partner-earned-credit.md)
