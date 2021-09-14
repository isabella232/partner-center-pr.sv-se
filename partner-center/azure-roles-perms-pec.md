---
title: Roller, behörigheter för partner-intjänad kredit
ms.topic: article
ms.date: 05/04/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
description: Lär dig mer om roller och behörigheter för partner för att kunna tjäna partner-intjänade krediter (PEC). Dessa skiljer sig från roller som ska fungera i Partnercenter.
author: adamyeh
ms.author: adamyeh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: ca9cd1b09c840531c3652f71afbd9c66f657f877
ms.sourcegitcommit: 37eac16c4339cb97831eb2a86d156c45bdf6a531
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/13/2021
ms.locfileid: "126246330"
---
# <a name="roles-and-permissions-required-to-earn-partner-earned-credit"></a>Roller och behörigheter som krävs för att få partner-intjänad kredit

Följande roller mappar till behörighetsnivåer som avgör om en partner är berättigad till partner-intjänade krediter.

>[!Important]
>Dessa roller och behörigheter är inte samma som de roller och behörigheter som en användare behöver för att arbeta i Partnercenter.

|**Role**   |**Beskrivning**   |**PEC-berättigad**   |
|-----------------|:------------------|:--------------|
|Ägare  |Du hanterar allt, inklusive åtkomst till resurser.|Yes|
|Deltagare |Du hanterar allt utom att bevilja åtkomst till resurser.|Yes|
|Läsare|Du kan visa allt, men inte göra några ändringar|No|
|ACRDelete|acr delete|Yes|
|ACRImageSigner|acr image signer|Yes|
|ACRPull|acr pull|Yes|
|AcrPush|acr push|Yes|
|AcrQuarantineReader|acr quarantine data reader|No|
|AcrQuarantineWriter| acr quarantine data writer|Yes|
|API Management tjänstdeltagare|Kan hantera tjänsten och API:erna|Yes|
|API Management tjänstoperatörsroll|Kan hantera tjänsten men inte API:erna|Yes|
|API Management rollen Tjänstläsare|Skrivskyddade åtkomst till tjänsten och API:er|No|
|Deltagare Insights programkomponent|Hanterar program Insights komponenter|Yes|
|Program Insights Snapshot Debugger|Ger användaren behörighet att visa och ladda ned ögonblicksbilder av felsökning som samlats in med Insights Snapshot Debugger. Observera att dessa behörigheter inte ingår i rollerna Ägare eller Deltagare.|Yes|
Automation-jobboperator | Skapa och hantera jobb med Automation Runbooks. | Yes | 
Automation-operatör | Automation-operatörer kan starta, stoppa, pausa och återuppta jobb | Yes | 
Automation Runbook-operatör | Läsa Runbook-egenskaper – för att kunna skapa jobb för runbooken. | Yes | 
Avere-deltagare | Kan skapa och hantera ett Avere vFXT kluster. | Yes | 
Avere-operator | Används av Avere vFXT för att hantera klustret | Yes | 
Azure Event Hubs dataägare | Ger fullständig åtkomst till Azure Event Hubs resurser. | Yes | 
Azure Event Hubs datamottagare | Tillåter åtkomst till Azure Event Hubs resurser. | Yes | 
Azure Event Hubs Data Sender | Tillåter att åtkomst skickas till Azure Event Hubs resurser. | Yes | 
Azure Kubernetes Service administratörsroll för kluster | Visa en lista över autentiseringsuppgifter för klusteradministratör. | Yes | 
Azure Kubernetes Service klusteranvändarroll | Visa en lista över åtgärder för klusteranvändares autentiseringsuppgifter. | Yes | 
Azure Kartor Data Reader (förhandsversion) | Ger åtkomst till läsmappningsrelaterade data från ett Azure Maps-konto. | No | 
Azure Service Bus dataägare | Ger fullständig åtkomst till Azure Service Bus resurser. | Yes | 
Azure Service Bus Data Receiver | Tillåter åtkomst till Azure Service Bus resurser. | Yes | 
Azure Service Bus Data Sender | Tillåter att du skickar åtkomst till Azure Service Bus resurser. | Yes | 
Azure Stack registreringsägare | Låter dig hantera Azure Stack registreringar. | Yes | 
Säkerhetskopieringsdeltagare | Låter dig hantera säkerhetskopieringstjänsten, men kan inte skapa valv och ge åtkomst till andra | Yes | 
Operator för säkerhetskopiering | Låter dig hantera säkerhetskopieringstjänster, förutom borttagning av säkerhetskopiering, valvskapande och att ge åtkomst till andra | Yes | 
Backup Reader | Kan visa säkerhetskopieringstjänster, men kan inte göra ändringar | No | 
Faktureringsläsare | Ger läsåtkomst till faktureringsdata | No | 
BizTalk-deltagare | Låter dig hantera BizTalk-tjänster, men inte åtkomst till dem. | Yes | 
Åtkomst till blockkedjemedlemsnod (förhandsversion) | Tillåter åtkomst till blockkedjemedlemsnoder | Yes | 
Skissdeltagare | Kan hantera skissdefinitioner, men inte tilldela dem. | Yes | 
Skissoperatör | Kan tilldela befintliga publicerade skisser, men kan inte skapa nya skisser. Obs! Detta fungerar bara om tilldelningen görs med en användar tilldelad hanterad identitet. | Yes | 
CDN Slutpunktsdeltagare | Kan hantera CDN slutpunkter, men kan inte bevilja åtkomst till andra användare. | Yes | 
CDN Slutpunktsläsare | Kan visa CDN slutpunkter, men kan inte göra ändringar. | No | 
CDN Profildeltagare | Kan hantera CDN profiler och deras slutpunkter, men kan inte bevilja åtkomst till andra användare. | Yes | 
CDN Profilläsare | Kan visa CDN profiler och deras slutpunkter, men kan inte göra ändringar. | No | 
Klassisk nätverksdeltagare | Låter dig hantera klassiska nätverk, men inte åtkomst till dem. | Yes | 
Klassisk Storage-kontodeltagare | Låter dig hantera klassiska lagringskonton, men inte åtkomst till dem. | Yes | 
Tjänstroll Storage klassisk Storage-kontonyckeloperatör | Operatorer Storage klassiska kontonycklar kan visa och återskapa nycklar på klassiska Storage konton | Yes | 
Klassisk virtuell datordeltagare | Låter dig hantera klassiska virtuella datorer, men inte åtkomst till dem, och inte det virtuella nätverket eller lagringskontot som de är anslutna till. | Yes | 
Cognitive Services deltagare | Låter dig skapa, läsa, uppdatera, ta bort och hantera nycklar för Cognitive Services. | Yes | 
Cognitive Services Data Reader (förhandsversion) | Låter dig läsa Cognitive Services data. | No | 
Cognitive Services användare | Låter dig läsa och lista nycklar för Cognitive Services. | No | 
Cosmos DB rollen Kontoläsare | Kan läsa Azure Cosmos DB-kontodata. Se DocumentDB-kontodeltagare för att hantera Azure Cosmos DB konton. | No | 
Cosmos DB Operator | Låter dig hantera Azure Cosmos DB-konton, men inte komma åt data i dem. Förhindrar åtkomst till kontonycklar och anslutningssträngar. | Yes | 
CosmosBackupOperator | Kan skicka återställningsbegäran för en Cosmos DB databas eller en container för ett konto | Yes | 
Cost Management-deltagare | Kan visa kostnader och hantera kostnadskonfiguration (t.ex. budgetar, exporter) | Yes | 
Cost Management Läsare | Kan visa kostnadsdata och konfiguration (t.ex. budgetar, exporter) | No | 
Data Box-enhet deltagare | Låter dig hantera allt under Data Box-enhet Service förutom att ge åtkomst till andra. | Yes | 
Data Box-enhet Läsare | Låter dig hantera Data Box-enhet service förutom att skapa beställnings- eller redigeringsinformation och ge åtkomst till andra. | No | 
Data Factory deltagare | Skapa och hantera datafabriker samt underordnade resurser i dem. | Yes | 
Data Lake Analytics utvecklare | Låter dig skicka, övervaka och hantera dina egna jobb, men inte skapa eller ta bort Data Lake Analytics konton. | Yes | 
Datarensning | Kan rensa analysdata | Yes | 
DevTest Labs-användare | Låter dig ansluta, starta, starta om och stänga av dina virtuella datorer i Azure DevTest Labs. | Yes | 
DNS-zondeltagare | Låter dig hantera DNS-zoner och postuppsättningar i Azure DNS, men låter dig inte styra vem som har åtkomst till dem. | Yes | 
DocumentDB-kontodeltagare | Kan hantera Azure Cosmos DB konton. Azure Cosmos DB kallades tidigare DocumentDB. | Yes | 
EventGrid EventSubscription-deltagare | Låter dig hantera eventGrid-händelseprenumerationsåtgärder. | Yes | 
EventGrid EventSubscription-läsare | Låter dig läsa EventGrid-händelseprenumerationer. | No | 
HDInsight-klusteroperator | Låter dig läsa och ändra HDInsight-klusterkonfigurationer. | Yes | 
HDInsight Domain Services-deltagare | Can Read, Create, Modify and Delete Domain Services related operations needed for HDInsight Enterprise Security Package | Yes | 
Intelligent Systems-kontodeltagare | Låter dig hantera konton för intelligenta system, men inte åtkomst till dem. | Yes | 
Key Vault deltagare | Låter dig hantera nyckelvalv, men inte åtkomst till dem. | Yes | 
Labbskapare | Låter dig skapa, hantera och ta bort dina hanterade labb under dina Azure Lab-konton. | Yes | 
Log Analytics Contributor | Log Analytics-deltagare kan läsa alla övervakningsdata och redigera övervakningsinställningar. Redigering av övervakningsinställningar omfattar att lägga till VM-tillägget till virtuella datorer. läsa lagringskontonycklar för att kunna konfigurera insamling av loggar från Azure Storage; skapa och konfigurera Automation-konton; lägga till lösningar; och konfigurera Azure Diagnostics på alla Azure-resurser. | Yes | 
Log Analytics Reader | Log Analytics-läsare kan visa och söka i alla övervakningsdata samt visa övervakningsinställningar, inklusive att visa konfigurationen av Azure Diagnostics på alla Azure-resurser. | No | 
Logic App-deltagare | Låter dig hantera logikappar, men inte ändra åtkomsten till dem. | Yes | 
Logic App-operatör | Låter dig läsa, aktivera och inaktivera logikappar, men inte redigera eller uppdatera dem. | Yes | 
Operatörsroll för hanterat program | Låter dig läsa och utföra åtgärder på hanterade programresurser | Yes | 
Läsare för hanterade program | Låter dig läsa resurser i en hanterad app och begära JIT-åtkomst. | No | 
Hanterad identitetsdeltagare | Skapa, läsa, uppdatera och ta bort användar tilldelad identitet | Yes | 
Operatör för hanterad identitet | Läsa och tilldela användar tilldelad identitet | Yes | 
Deltagare i hanteringsgrupp | Deltagarroll för hanteringsgrupp | Yes | 
Läsare för hanteringsgrupp | Läsarroll för hanteringsgrupp | No | 
Övervakningsdeltagare | Kan läsa alla övervakningsdata och redigera övervakningsinställningar. Se även Kom igång med roller, behörigheter och säkerhet med Azure Monitor. | Yes | 
Övervaka Publisher | Aktiverar publiceringsmått mot Azure-resurser | Yes | 
Övervakningsläsare | Kan läsa alla övervakningsdata (mått, loggar osv.). Se även Kom igång med roller, behörigheter och säkerhet med Azure Monitor. | No | 
Nätverksdeltagare | Låter dig hantera nätverk, men inte åtkomst till dem. | Yes | 
New Relic APM-kontodeltagare | Låter dig hantera New Relic Application Performance Management och program, men inte åtkomst till dem. | Yes | 
Läsar- och dataåtkomst | Låter dig visa allt, men du kan inte ta bort eller skapa ett lagringskonto eller en innesluten resurs. Det ger också läs-/skrivåtkomst till alla data som finns i ett lagringskonto via åtkomst till lagringskontonycklar. | Yes | 
Redis Cache deltagare | Låter dig hantera Redis-cacher, men inte åtkomst till dem. | Yes | 
Resursprincipdeltagare (förhandsversion) | (Förhandsversion) Återifyllda användare från EA, med behörighet att skapa/ändra resursprincip, skapa supportbiljett och läsa resurser/hierarki. | Yes | 
Deltagare i Scheduler-jobbsamlingar | Låter dig hantera Scheduler-jobbsamlingar, men inte åtkomst till dem. | Yes | 
Search Service Contributor | Låter dig hantera Söktjänster, men inte åtkomst till dem. | Yes | 
Säkerhetsadministratör | Endast Security Center: Kan visa säkerhetsprinciper, visa säkerhets tillstånd, redigera säkerhetsprinciper, visa aviseringar och rekommendationer, stänga aviseringar och rekommendationer | Yes | 
Security Manager (äldre) | Det här är en äldre roll. Använd säkerhetsadministratören i stället | Yes | 
Säkerhetsläsare | Endast Security Center: Kan visa rekommendationer och aviseringar, visa säkerhetsprinciper, visa säkerhets tillstånd, men inte göra ändringar | No | 
Site Recovery-deltagare | Låter dig hantera Site Recovery förutom valvskapande och rolltilldelning | Yes | 
Site Recovery-operatör | Låter dig redundans och återställning efter fel men inte utföra Site Recovery av hanteringsåtgärder | Yes | 
Site Recovery-läsare | Låter dig visa Site Recovery status men inte utföra andra hanteringsåtgärder | No | 
Spatial Anchors kontodeltagare | Låter dig hantera spatiala fästpunkter i ditt konto, men inte ta bort dem | Yes | 
Spatial Anchors kontoägare | Låter dig hantera spatiala fästpunkter i ditt konto, inklusive att ta bort dem | Yes | 
Spatial Anchors-kontoläsare | Gör att du kan hitta och läsa egenskaper för spatiala fästpunkter i ditt konto | No | 
SQL DB-deltagare | Låter dig hantera SQL databaser, men inte åtkomst till dem. Du kan inte heller hantera deras säkerhetsrelaterade principer eller deras överordnade SQL servrar. | Yes | 
SQL Deltagare för hanterad instans | Låter dig hantera SQL hanterade instanser och nödvändig nätverkskonfiguration, men kan inte ge åtkomst till andra. | Yes | 
SQL-säkerhetshanteraren | Låter dig hantera säkerhetsrelaterade principer för SQL och databaser, men inte åtkomst till dem. | Yes | 
SQL Server Bidragsgivare | Låter dig hantera SQL servrar och databaser, men inte åtkomst till dem, och inte deras säkerhetsrelaterade principer. | Yes | 
Lagringskontodeltagare | Tillåter hantering av lagringskonton. Ger åtkomst till kontonyckeln, som kan användas för att komma åt data via auktorisering med delad nyckel. | Yes | 
Storage Tjänstroll för kontonyckeloperatör | Tillåter att åtkomstnycklar för lagringskontot listas och återskapas. | Yes | 
Storage Blob Data-deltagare | Läsa, skriva och ta bort Azure Storage containrar och blobar. Information om vilka åtgärder som krävs för en viss dataåtgärd finns i Behörigheter för att anropa blob- och ködataåtgärder. | Yes | 
Storage Blob Data-ägare | Ger fullständig åtkomst till Azure Storage blobcontainrar och data, inklusive tilldelning av POSIX-åtkomstkontroll. Information om vilka åtgärder som krävs för en viss dataåtgärd finns i Behörigheter för att anropa blob- och ködataåtgärder. | Yes | 
Storage Blob Data-läsare | Läs och lista Azure Storage containrar och blobar. Information om vilka åtgärder som krävs för en viss dataåtgärd finns i Behörigheter för att anropa blob- och ködataåtgärder. | No | 
Storage Blob Dele blob | Hämta en nyckel för användardelegering som sedan kan användas för att skapa en signatur för delad åtkomst för en container eller blob som har signerats med Azure AD-autentiseringsuppgifter. Mer information finns i Skapa en SAS för användardelegering. | Yes | 
Storage-fildata för SMB-resursdeltagare | Tillåter läs-, skriv- och borttagningsåtkomst i Azure Storage filresurser via SMB | Yes | 
Storage-fildata för upphöjd SMB-resursdeltagare | Tillåter läs-, skriv-, borttagnings- och ändringsbehörighet för NTFS i Azure Storage över SMB | Yes | 
Storage-fildata för SMB-resursläsare | Tillåter läsåtkomst till Azure-filresurs via SMB | No | 
Storage Ködatadeltagare | Läsa, skriva och ta bort Azure Storage köer och kömeddelanden. Information om vilka åtgärder som krävs för en viss dataåtgärd finns i Behörigheter för att anropa blob- och ködataåtgärder. | Yes | 
Storage Processor för ködatameddelande | Granska, hämta och ta bort ett meddelande från en Azure Storage kö. Information om vilka åtgärder som krävs för en viss dataåtgärd finns i Behörigheter för att anropa blob- och ködataåtgärder. | Yes | 
Storage Avsändare av ködatameddelande | Lägga till meddelanden i en Azure Storage kö. Information om vilka åtgärder som krävs för en viss dataåtgärd finns i Behörigheter för att anropa blob- och ködataåtgärder. | Yes | 
Storage Ködataläsare | Läsa och lista Azure Storage köer och kömeddelanden. Information om vilka åtgärder som krävs för en viss dataåtgärd finns i Behörigheter för att anropa blob- och ködataåtgärder. | No | 
Supportbegärandedeltagare | Låter dig skapa och hantera supportbegäranden | Yes | 
Traffic Manager Bidragsgivare | Låter dig hantera Traffic Manager profiler, men låter dig inte styra vem som har åtkomst till dem. | Yes | 
Administratör för användaråtkomst | Låter dig hantera användaråtkomst till Azure-resurser. | Yes | 
Administratörsinloggning för virtuell dator | Visa Virtual Machines i portalen och logga in som administratör | Yes | 
Virtuell datordeltagare | Låter dig hantera virtuella datorer, men inte åtkomst till dem, och inte det virtuella nätverket eller lagringskontot som de är anslutna till. | Yes | 
Användarinloggning för virtuell dator | Visa Virtual Machines i portalen och logga in som en vanlig användare. | Yes | 
Webbplansdeltagare | Låter dig hantera webbplaner för webbplatser, men inte åtkomst till dem. | Yes | 
Webbplatsdeltagare | Låter dig hantera webbplatser (inte webbplaner), men inte åtkomst till dem | Ja |

## <a name="next-steps"></a>Nästa steg

- [Partner-intjänad kredit – en översikt över hur det fungerar i den nya handelsupplevelsen i CSP](partner-earned-credit.md)
