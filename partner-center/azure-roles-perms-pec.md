---
title: Roller, behörigheter för partner intjänad kredit
ms.topic: article
ms.date: 05/04/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Lär dig mer om roller och behörigheter för partner att kunna ta del av partner intjänade krediter (PEC). Dessa skiljer sig från roller som fungerar i Partner Center.
author: adamyeh
ms.author: adamyeh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: f48774cb830ceb575a84177efb57431afdcb9b25
ms.sourcegitcommit: 5fc28f6f81eaebb84e1faa71848afb504e181f37
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/11/2020
ms.locfileid: "92531417"
---
# <a name="roles-and-permissions-eligible-to-earn-partner-earned-credit"></a>Roller och behörigheter som kan tjäna partner intjänade kredit

Följande roller mappar till behörighets nivåer som avgör om en partner är berättigad till partner intjänade krediter.

>[!Important]
>Dessa roller och behörigheter är inte samma som de roller och behörigheter som en användare behöver för att arbeta i Partner Center.

|**Role**   |**Beskrivning**   |**PEC-berättigande**   |
|-----------------|:------------------|:--------------|
|Ägare  |Du hanterar allt, inklusive åtkomst till resurser.|Yes|
|Deltagare |Du hanterar allt förutom att bevilja åtkomst till resurser.|Yes|
|Läsare|Du kan visa allt, men inte göra några ändringar|No|
|ACRDelete|ta bort ACR|Yes|
|ACRImageSigner|ACR-bildsignerare|Yes|
|ACRPull|ACR pull|Yes|
|AcrPush|ACR-push|Yes|
|AcrQuarantineReader|ACR Quarantine data Reader|No|
|AcrQuarantineWriter| ACR karantän data skrivare|Yes|
|API Management Service Contributor|Kan hantera tjänster och API: er|Yes|
|Rollen API Management tjänst operatör|Kan hantera tjänsten men inte API: erna|Yes|
|Rollen API Management tjänst läsare|Skrivskyddad åtkomst till tjänster och API: er|No|
|Application Insights komponent deltagare|Hanterar Application Insights-komponenter|Yes|
|Application Insights Snapshot Debugger|Ger användaren behörighet att visa och hämta fel söknings ögonblicks bilder som samlats in med Application Insights Snapshot Debugger. Observera att dessa behörigheter inte ingår i ägaren eller deltagar rollerna.|Yes|
Automatiserings jobb operatör | Skapa och hantera jobb med hjälp av Automation-runbooks. | Yes | 
Automation-operatör | Automation-operatörer kan starta, stoppa, pausa och återuppta jobb | Yes | 
Automation Runbook-operator | Läs Runbook-egenskaperna – för att kunna skapa jobb för runbooken. | Yes | 
Aver deltagare | Kan skapa och hantera ett AVERT vFXT-kluster. | Yes | 
Aver operator | Används av det Avera vFXT-klustret för att hantera klustret | Yes | 
Azure Event Hubs data ägare | Ger fullständig åtkomst till Azure Event Hubs-resurser. | Yes | 
Azure Event Hubs data mottagare | Tillåter åtkomst till Azure Event Hubs-resurser. | Yes | 
Azure Event Hubs data avsändare | Tillåter skicka åtkomst till Azure Event Hubs-resurser. | Yes | 
Administratörs roll för Azure Kubernetes service Cluster | Visa lista med autentiseringsuppgifter för kluster administratör. | Yes | 
Användar roll för Azure Kubernetes service-kluster | Visa lista över autentiseringsuppgifter för kluster användare. | Yes | 
Azure Maps data läsare (förhands granskning) | Beviljar åtkomst till läsa kartdata relaterade data från ett Azure Maps-konto. | No | 
Azure Service Bus data ägare | Ger fullständig åtkomst till Azure Service Bus resurser. | Yes | 
Azure Service Bus data mottagare | Ger åtkomst till Azure Service Bus resurser. | Yes | 
Azure Service Bus data avsändare | Tillåter att åtkomst till Azure Service Bus-resurser skickas. | Yes | 
Azure Stack registrerings ägare | Låter dig hantera Azure Stack-registreringar. | Yes | 
Säkerhets kopierings deltagare | Låter dig hantera säkerhets kopierings tjänsten, men kan inte skapa valv och ge åtkomst till andra | Yes | 
Ansvarig för säkerhets kopiering | Låter dig hantera säkerhets kopierings tjänster, förutom att ta bort säkerhets kopiering, skapa valv och ge till gång till andra | Yes | 
Säkerhets kopierings läsare | Kan visa säkerhets kopierings tjänster, men kan inte göra ändringar | No | 
Faktureringsläsare | Tillåter Läs åtkomst till fakturerings data | No | 
BizTalk-deltagare | Gör att du kan hantera BizTalk Services, men inte till gång till dem. | Yes | 
Blockchain för medlems Node (för hands version) | Tillåter åtkomst till blockchain-medlems noder | Yes | 
Skiss deltagare | Kan hantera skiss definitioner, men tilldela dem inte. | Yes | 
Skiss operator | Kan tilldela befintliga publicerade ritningar, men kan inte skapa nya ritningar. OBS! detta fungerar endast om tilldelningen görs med en tilldelad hanterad identitet. | Yes | 
CDN-slutpunkts deltagare | Kan hantera CDN-slutpunkter, men kan inte bevilja åtkomst till andra användare. | Yes | 
CDN-slutpunkt läsare | Kan visa CDN-slutpunkter, men kan inte göra ändringar. | No | 
CDN-profil deltagare | Kan hantera CDN-profiler och deras slut punkter, men kan inte bevilja åtkomst till andra användare. | Yes | 
CDN profil läsare | Kan visa CDN-profiler och deras slut punkter, men kan inte göra ändringar. | No | 
Klassisk nätverksdeltagare | Gör att du kan hantera klassiska nätverk, men inte till gång till dem. | Yes | 
Klassisk lagrings konto deltagare | Gör att du kan hantera klassiska lagrings konton, men inte till gång till dem. | Yes | 
Klassisk lagrings kontots nyckel operatörs tjänst roll | Klassiska lagrings konto nyckel operatörer får lista och återskapa nycklar på klassiska lagrings konton | Yes | 
Klassisk virtuell dator deltagare | Låter dig hantera klassiska virtuella datorer, men inte åtkomst till dem, inte det virtuella nätverk eller lagrings konto som de är anslutna till. | Yes | 
Cognitive Services deltagare | Gör att du kan skapa, läsa, uppdatera, ta bort och hantera nycklar för Cognitive Services. | Yes | 
Cognitive Services data läsare (förhands granskning) | Gör att du kan läsa Cognitive Services data. | No | 
Cognitive Services användare | Gör att du kan läsa och Visa nycklar för Cognitive Services. | No | 
Cosmos DB konto läsar roll | Kan läsa Azure Cosmos DB konto data. Se DocumentDB Account Contributor för att hantera Azure Cosmos DB-konton. | No | 
Cosmos DB operatör | Låter dig hantera Azure Cosmos DB konton, men inte komma åt data i dem. Förhindrar åtkomst till konto nycklar och anslutnings strängar. | Yes | 
CosmosBackupOperator | Kan skicka en Restore-begäran för en Cosmos DB databas eller en behållare för ett konto | Yes | 
Cost Management deltagare | Kan visa kostnader och hantera kostnads konfiguration (t. ex. budgetar, exporter) | Yes | 
Cost Management läsare | Kan visa kostnads data och konfiguration (t. ex. budgetar, exporter) | No | 
Data Box-enhet deltagare | Låter dig hantera allt under Data Box-enhet tjänst, förutom att ge till gång till andra. | Yes | 
Data Box-enhet läsare | Låter dig hantera Data Box-enhet tjänst, förutom att skapa order-eller redigerings beställnings detaljer och ge åtkomst till andra. | No | 
Data Factory deltagare | Skapa och hantera data fabriker, samt underordnade resurser i dem. | Yes | 
Data Lake Analytics utvecklare | Låter dig skicka, övervaka och hantera dina egna jobb, men inte skapa eller ta bort Data Lake Analytics konton. | Yes | 
Data rensning | Kan rensa analys data | Yes | 
DevTest Labs-användare | Låter dig ansluta, starta, starta om och stänga av dina virtuella datorer i din Azure DevTest Labs. | Yes | 
DNS-zon deltagare | Gör att du kan hantera DNS-zoner och post uppsättningar i Azure DNS, men du kan inte styra vem som har åtkomst till dem. | Yes | 
DocumentDB-konto deltagare | Kan hantera Azure Cosmos DB-konton. Azure Cosmos DB är tidigare känt som DocumentDB. | Yes | 
EventGrid EventSubscription-deltagare | Låter dig hantera EventGrid händelse prenumerations åtgärder. | Yes | 
EventGrid EventSubscription-läsare | Låter dig läsa EventGrid händelse prenumerationer. | No | 
HDInsight-kluster operator | Gör att du kan läsa och ändra HDInsight-klusterkonfigurationer. | Yes | 
HDInsight Domain Services-deltagare | Kan läsa, skapa, ändra och ta bort åtgärder för domän tjänster som krävs för HDInsight-Enterprise Security Package | Yes | 
Konto deltagare i Intelligent Systems | Gör att du kan hantera intelligenta system konton, men inte åtkomst till dem. | Yes | 
Key Vault deltagare | Låter dig hantera nyckel valv, men inte åtkomst till dem. | Yes | 
Labb skapare | Gör att du kan skapa, hantera och ta bort dina hanterade labb under dina Azure Lab-konton. | Yes | 
Log Analytics Contributor | Log Analytics deltagare kan läsa alla övervaknings data och redigera övervaknings inställningar. Genom att redigera övervaknings inställningarna lägger du till VM-tillägget till virtuella datorer. läsning av lagrings konto nycklar för att kunna konfigurera samling av loggar från Azure Storage. Skapa och konfigurera Automation-konton. lägga till lösningar. och konfigurera Azure Diagnostics på alla Azure-resurser. | Yes | 
Log Analytics Reader | Log Analytics läsaren kan visa och söka i alla övervaknings data samt Visa övervaknings inställningar, inklusive Visa konfigurationen av Azure Diagnostics på alla Azure-resurser. | No | 
Logic app-deltagare | Låter dig hantera Logi Kap par, men ändra inte åtkomsten till dem. | Yes | 
Logic app-operatör | Låter dig läsa, aktivera och inaktivera Logi Kap par, men inte redigera eller uppdatera dem. | Yes | 
Rollen hanterad program operatör | Gör att du kan läsa och utföra åtgärder på hanterade program resurser | Yes | 
Läsare för hanterade program | Låter dig läsa resurser i en hanterad app och begära JIT-åtkomst. | No | 
Hanterad identitets deltagare | Skapa, läsa, uppdatera och ta bort användare tilldelad identitet | Yes | 
Hanterad identitets operator | Läs och tilldela en tilldelad identitet | Yes | 
Deltagare i hanterings grupp | Rollen hanterings grupp deltagare | Yes | 
Hanterings grupp läsare | Rollen hanterings grupp läsare | No | 
Övervaknings deltagare | Kan läsa alla övervaknings data och redigera övervaknings inställningar. Se även komma igång med roller, behörigheter och säkerhet med Azure Monitor. | Yes | 
Övervaknings mått utgivare | Möjliggör publicering av mått mot Azure-resurser | Yes | 
Övervaknings läsare | Kan läsa alla övervaknings data (mått, loggar osv.). Se även komma igång med roller, behörigheter och säkerhet med Azure Monitor. | No | 
Nätverksdeltagare | Gör att du kan hantera nätverk, men inte till gång till dem. | Yes | 
Ny Relic APM-konto deltagare | Låter dig hantera New Relic Application Performance Management konton och program, men inte till gång till dem. | Yes | 
Läsare och data åtkomst | Gör att du kan visa allting men du kan inte ta bort eller skapa ett lagrings konto eller en resurs som saknas. Den kommer också att tillåta Läs-/skriv åtkomst till alla data som finns i ett lagrings konto via åtkomst till lagrings konto nycklar. | Yes | 
Redis Cache deltagare | Låter dig hantera Redis-cacheer, men inte till gång till dem. | Yes | 
Resurs princip deltagare (för hands version) | Förhandsgranskningsvyn Användare med egna användare från EA, med behörighet att skapa/ändra resurs principer, skapa support ärende och läsa resurser/hierarki. | Yes | 
Jobb samlings deltagare i Scheduler | Gör att du kan hantera jobb samlingar i Scheduler, men inte till gång till dem. | Yes | 
Search Service deltagare | Låter dig hantera Sök tjänster, men inte till gång till dem. | Yes | 
Säkerhetsadministratör | Endast i Security Center: kan visa säkerhets principer, Visa säkerhets tillstånd, redigera säkerhets principer, Visa aviseringar och rekommendationer, ignorera aviseringar och rekommendationer | Yes | 
Säkerhets hanterare (bakåtkompatibelt) | Detta är en äldre roll. Använd säkerhets administratör istället | Yes | 
Säkerhetsläsare | Endast i Security Center: kan visa rekommendationer och aviseringar, Visa säkerhets principer, Visa säkerhets tillstånd, men kan inte göra ändringar | No | 
Site Recovery deltagare | Låter dig hantera Site Recovery tjänst förutom att skapa valv och roll tilldelning | Yes | 
Site Recovery operatör | Låter dig redundansväxla och failback men inte utföra andra Site Recovery hanterings åtgärder | Yes | 
Site Recovery läsare | Låter dig Visa Site Recovery status men inte utföra andra hanterings åtgärder | No | 
Konto deltagare för spatiala ankare | Låter dig hantera spatiala ankare i ditt konto, men ta inte bort dem | Yes | 
Konto ägare för spatiala ankare | Låter dig hantera spatialdata i ditt konto, inklusive att ta bort dem | Yes | 
Konto läsare för spatiala ankare | Gör att du kan hitta och läsa egenskaper för spatiala ankare i ditt konto | No | 
SQL DB-deltagare | Gör att du kan hantera SQL-databaser, men inte åtkomst till dem. Du kan inte heller hantera säkerhets relaterade principer eller överordnade SQL-servrar. | Yes | 
SQL-hanterad instans deltagare | Låter dig hantera SQL-hanterade instanser och nödvändig nätverks konfiguration, men kan inte ge åtkomst till andra. | Yes | 
SQL-säkerhetshanteraren | Gör att du kan hantera säkerhetsrelaterade principer för SQL-servrar och databaser, men inte åtkomst till dem. | Yes | 
SQL Server deltagare | Gör att du kan hantera SQL-servrar och databaser, men inte åtkomst till dem och inte deras säkerhetsrelaterade principer. | Yes | 
Lagringskontodeltagare | Tillåter hantering av lagrings konton. Ger åtkomst till konto nyckeln, som kan användas för att få åtkomst till data via autentisering med delad nyckel. | Yes | 
Lagrings kontots nyckel operatörs tjänst roll | Tillåter att du visar och återskapar åtkomst nycklar för lagrings kontot. | Yes | 
Storage Blob Data-deltagare | Läsa, skriva och ta bort Azure Storage behållare och blobbar. Information om vilka åtgärder som krävs för en specifik data åtgärd finns i behörigheter för att anropa blob-och Queue data-åtgärder. | Yes | 
Storage Blob Data-ägare | Ger fullständig åtkomst till Azure Storage BLOB-behållare och data, inklusive att tilldela POSIX-åtkomstkontroll. Information om vilka åtgärder som krävs för en specifik data åtgärd finns i behörigheter för att anropa blob-och Queue data-åtgärder. | Yes | 
Storage Blob Data-läsare | Läs och Visa Azure Storage behållare och blobbar. Information om vilka åtgärder som krävs för en specifik data åtgärd finns i behörigheter för att anropa blob-och Queue data-åtgärder. | No | 
Storage BLOB-delegerare | Hämta en användar Delegerings nyckel som sedan kan användas för att skapa en signatur för delad åtkomst för en behållare eller BLOB som är signerad med Azure AD-autentiseringsuppgifter. Mer information finns i skapa en användar Delegerings-SAS. | Yes | 
Storage-fildata för SMB-resursdeltagare | Tillåter Läs-, skriv-och borttagnings åtkomst i Azure Storage fil resurser över SMB | Yes | 
Storage-fildata för upphöjd SMB-resursdeltagare | Tillåter behörighet att läsa, skriva, ta bort och ändra NTFS-behörighet i Azure Storage fil resurser över SMB | Yes | 
Storage-fildata för SMB-resursläsare | Tillåter Läs åtkomst till Azure-filresurs via SMB | No | 
Data deltagare i Storage Queue | Läsa, skriva och ta bort Azure Storage köer och köa meddelanden. Information om vilka åtgärder som krävs för en specifik data åtgärd finns i behörigheter för att anropa blob-och Queue data-åtgärder. | Yes | 
Processor för data meddelande i lagrings kön | Granska, hämta och ta bort ett meddelande från en Azure Storage kö. Information om vilka åtgärder som krävs för en specifik data åtgärd finns i behörigheter för att anropa blob-och Queue data-åtgärder. | Yes | 
Avsändare av data meddelande i lagrings köer | Lägg till meddelanden i en Azure Storage-kö. Information om vilka åtgärder som krävs för en specifik data åtgärd finns i behörigheter för att anropa blob-och Queue data-åtgärder. | Yes | 
Data läsare för lagrings kön | Läs och Visa Azure Storage köer och köa meddelanden. Information om vilka åtgärder som krävs för en specifik data åtgärd finns i behörigheter för att anropa blob-och Queue data-åtgärder. | No | 
Support förfrågan deltagare | Gör att du kan skapa och hantera support förfrågningar | Yes | 
Traffic Manager deltagare | Låter dig hantera Traffic Manager profiler, men låter dig inte kontrol lera vem som har åtkomst till dem. | Yes | 
Administratör för användaråtkomst | Gör att du kan hantera användar åtkomst till Azure-resurser. | Yes | 
Administratörs inloggning för virtuell dator | Visa Virtual Machines i portalen och logga in som administratör | Yes | 
Virtuell datordeltagare | Låter dig hantera virtuella datorer, men inte åtkomst till dem, inte det virtuella nätverk eller lagrings konto som de är anslutna till. | Yes | 
Användar inloggning för virtuell dator | Visa Virtual Machines i portalen och logga in som en vanlig användare. | Yes | 
Webb Plans deltagare | Gör att du kan hantera webb planer för webbplatser, men inte till gång till dem. | Yes | 
Webbplats deltagare | Gör att du kan hantera webbplatser (inte webb planer), men inte åtkomst till dem | Yes |
