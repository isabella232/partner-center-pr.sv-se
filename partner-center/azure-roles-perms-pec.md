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
ms.openlocfilehash: 8c36883dc7d12b7ea0ce8f2644dbac86595ab131
ms.sourcegitcommit: 2d9aab15ddc20cb3d9537e68ace33d36f7d8a250
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 12/02/2020
ms.locfileid: "96534598"
---
# <a name="roles-and-permissions-required-to-earn-partner-earned-credit"></a>Roller och behörigheter som krävs för att få partner intjänad kredit

Följande roller mappar till behörighets nivåer som avgör om en partner är berättigad till partner intjänade krediter.

>[!Important]
>Dessa roller och behörigheter är inte samma som de roller och behörigheter som en användare behöver för att arbeta i Partner Center.

|**Role**   |**Beskrivning**   |**PEC-berättigande**   |
|-----------------|:------------------|:--------------|
|Ägare  |Du hanterar allt, inklusive åtkomst till resurser.|Ja|
|Deltagare |Du hanterar allt förutom att bevilja åtkomst till resurser.|Ja|
|Läsare|Du kan visa allt, men inte göra några ändringar|Nej|
|ACRDelete|ta bort ACR|Ja|
|ACRImageSigner|ACR-bildsignerare|Ja|
|ACRPull|ACR pull|Ja|
|AcrPush|ACR-push|Ja|
|AcrQuarantineReader|ACR Quarantine data Reader|Nej|
|AcrQuarantineWriter| ACR karantän data skrivare|Ja|
|API Management Service Contributor|Kan hantera tjänster och API: er|Ja|
|Rollen API Management tjänst operatör|Kan hantera tjänsten men inte API: erna|Ja|
|Rollen API Management tjänst läsare|Skrivskyddad åtkomst till tjänster och API: er|Nej|
|Application Insights komponent deltagare|Hanterar Application Insights-komponenter|Ja|
|Application Insights Snapshot Debugger|Ger användaren behörighet att visa och hämta fel söknings ögonblicks bilder som samlats in med Application Insights Snapshot Debugger. Observera att dessa behörigheter inte ingår i ägaren eller deltagar rollerna.|Ja|
Automatiserings jobb operatör | Skapa och hantera jobb med hjälp av Automation-runbooks. | Ja | 
Automation-operatör | Automation-operatörer kan starta, stoppa, pausa och återuppta jobb | Ja | 
Automation Runbook-operator | Läs Runbook-egenskaperna – för att kunna skapa jobb för runbooken. | Ja | 
Aver deltagare | Kan skapa och hantera ett AVERT vFXT-kluster. | Ja | 
Aver operator | Används av det Avera vFXT-klustret för att hantera klustret | Ja | 
Azure Event Hubs data ägare | Ger fullständig åtkomst till Azure Event Hubs-resurser. | Ja | 
Azure Event Hubs data mottagare | Tillåter åtkomst till Azure Event Hubs-resurser. | Ja | 
Azure Event Hubs data avsändare | Tillåter skicka åtkomst till Azure Event Hubs-resurser. | Ja | 
Administratörs roll för Azure Kubernetes service Cluster | Visa lista med autentiseringsuppgifter för kluster administratör. | Ja | 
Användar roll för Azure Kubernetes service-kluster | Visa lista över autentiseringsuppgifter för kluster användare. | Ja | 
Azure Maps data läsare (förhands granskning) | Beviljar åtkomst till läsa kartdata relaterade data från ett Azure Maps-konto. | Nej | 
Azure Service Bus data ägare | Ger fullständig åtkomst till Azure Service Bus resurser. | Ja | 
Azure Service Bus data mottagare | Ger åtkomst till Azure Service Bus resurser. | Ja | 
Azure Service Bus data avsändare | Tillåter att åtkomst till Azure Service Bus-resurser skickas. | Ja | 
Azure Stack registrerings ägare | Låter dig hantera Azure Stack-registreringar. | Ja | 
Säkerhets kopierings deltagare | Låter dig hantera säkerhets kopierings tjänsten, men kan inte skapa valv och ge åtkomst till andra | Ja | 
Operator för säkerhetskopiering | Låter dig hantera säkerhets kopierings tjänster, förutom att ta bort säkerhets kopiering, skapa valv och ge till gång till andra | Ja | 
Säkerhets kopierings läsare | Kan visa säkerhets kopierings tjänster, men kan inte göra ändringar | Nej | 
Faktureringsläsare | Tillåter Läs åtkomst till fakturerings data | Nej | 
BizTalk-deltagare | Gör att du kan hantera BizTalk Services, men inte till gång till dem. | Ja | 
Blockchain för medlems Node (för hands version) | Tillåter åtkomst till blockchain-medlems noder | Ja | 
Skiss deltagare | Kan hantera skiss definitioner, men tilldela dem inte. | Ja | 
Skiss operator | Kan tilldela befintliga publicerade ritningar, men kan inte skapa nya ritningar. OBS! detta fungerar endast om tilldelningen görs med en tilldelad hanterad identitet. | Ja | 
CDN-slutpunkts deltagare | Kan hantera CDN-slutpunkter, men kan inte bevilja åtkomst till andra användare. | Ja | 
CDN-slutpunkt läsare | Kan visa CDN-slutpunkter, men kan inte göra ändringar. | Nej | 
CDN-profil deltagare | Kan hantera CDN-profiler och deras slut punkter, men kan inte bevilja åtkomst till andra användare. | Ja | 
CDN profil läsare | Kan visa CDN-profiler och deras slut punkter, men kan inte göra ändringar. | Nej | 
Klassisk nätverksdeltagare | Gör att du kan hantera klassiska nätverk, men inte till gång till dem. | Ja | 
Klassisk lagrings konto deltagare | Gör att du kan hantera klassiska lagrings konton, men inte till gång till dem. | Ja | 
Klassisk lagrings kontots nyckel operatörs tjänst roll | Klassiska lagrings konto nyckel operatörer får lista och återskapa nycklar på klassiska lagrings konton | Ja | 
Klassisk virtuell dator deltagare | Låter dig hantera klassiska virtuella datorer, men inte åtkomst till dem, inte det virtuella nätverk eller lagrings konto som de är anslutna till. | Ja | 
Cognitive Services deltagare | Gör att du kan skapa, läsa, uppdatera, ta bort och hantera nycklar för Cognitive Services. | Ja | 
Cognitive Services data läsare (förhands granskning) | Gör att du kan läsa Cognitive Services data. | Nej | 
Cognitive Services användare | Gör att du kan läsa och Visa nycklar för Cognitive Services. | Nej | 
Cosmos DB konto läsar roll | Kan läsa Azure Cosmos DB konto data. Se DocumentDB Account Contributor för att hantera Azure Cosmos DB-konton. | Nej | 
Cosmos DB operatör | Låter dig hantera Azure Cosmos DB konton, men inte komma åt data i dem. Förhindrar åtkomst till konto nycklar och anslutnings strängar. | Ja | 
CosmosBackupOperator | Kan skicka en Restore-begäran för en Cosmos DB databas eller en behållare för ett konto | Ja | 
Cost Management deltagare | Kan visa kostnader och hantera kostnads konfiguration (t. ex. budgetar, exporter) | Ja | 
Cost Management läsare | Kan visa kostnads data och konfiguration (t. ex. budgetar, exporter) | Nej | 
Data Box-enhet deltagare | Låter dig hantera allt under Data Box-enhet tjänst, förutom att ge till gång till andra. | Ja | 
Data Box-enhet läsare | Låter dig hantera Data Box-enhet tjänst, förutom att skapa order-eller redigerings beställnings detaljer och ge åtkomst till andra. | Nej | 
Data Factory deltagare | Skapa och hantera data fabriker, samt underordnade resurser i dem. | Ja | 
Data Lake Analytics utvecklare | Låter dig skicka, övervaka och hantera dina egna jobb, men inte skapa eller ta bort Data Lake Analytics konton. | Ja | 
Data rensning | Kan rensa analys data | Ja | 
DevTest Labs-användare | Låter dig ansluta, starta, starta om och stänga av dina virtuella datorer i din Azure DevTest Labs. | Ja | 
DNS-zon deltagare | Gör att du kan hantera DNS-zoner och post uppsättningar i Azure DNS, men du kan inte styra vem som har åtkomst till dem. | Ja | 
DocumentDB-konto deltagare | Kan hantera Azure Cosmos DB-konton. Azure Cosmos DB är tidigare känt som DocumentDB. | Ja | 
EventGrid EventSubscription-deltagare | Låter dig hantera EventGrid händelse prenumerations åtgärder. | Ja | 
EventGrid EventSubscription-läsare | Låter dig läsa EventGrid händelse prenumerationer. | Nej | 
HDInsight-kluster operator | Gör att du kan läsa och ändra HDInsight-klusterkonfigurationer. | Ja | 
HDInsight Domain Services-deltagare | Kan läsa, skapa, ändra och ta bort åtgärder för domän tjänster som krävs för HDInsight-Enterprise Security Package | Ja | 
Konto deltagare i Intelligent Systems | Gör att du kan hantera intelligenta system konton, men inte åtkomst till dem. | Ja | 
Key Vault deltagare | Låter dig hantera nyckel valv, men inte åtkomst till dem. | Ja | 
Labb skapare | Gör att du kan skapa, hantera och ta bort dina hanterade labb under dina Azure Lab-konton. | Ja | 
Log Analytics Contributor | Log Analytics deltagare kan läsa alla övervaknings data och redigera övervaknings inställningar. Genom att redigera övervaknings inställningarna lägger du till VM-tillägget till virtuella datorer. läsning av lagrings konto nycklar för att kunna konfigurera samling av loggar från Azure Storage. Skapa och konfigurera Automation-konton. lägga till lösningar. och konfigurera Azure Diagnostics på alla Azure-resurser. | Ja | 
Log Analytics Reader | Log Analytics läsaren kan visa och söka i alla övervaknings data samt Visa övervaknings inställningar, inklusive Visa konfigurationen av Azure Diagnostics på alla Azure-resurser. | Nej | 
Logic app-deltagare | Låter dig hantera Logi Kap par, men ändra inte åtkomsten till dem. | Ja | 
Logic app-operatör | Låter dig läsa, aktivera och inaktivera Logi Kap par, men inte redigera eller uppdatera dem. | Ja | 
Rollen hanterad program operatör | Gör att du kan läsa och utföra åtgärder på hanterade program resurser | Ja | 
Läsare för hanterade program | Låter dig läsa resurser i en hanterad app och begära JIT-åtkomst. | Nej | 
Hanterad identitets deltagare | Skapa, läsa, uppdatera och ta bort användare tilldelad identitet | Ja | 
Hanterad identitets operator | Läs och tilldela en tilldelad identitet | Ja | 
Deltagare i hanterings grupp | Rollen hanterings grupp deltagare | Ja | 
Hanterings grupp läsare | Rollen hanterings grupp läsare | Nej | 
Övervaknings deltagare | Kan läsa alla övervaknings data och redigera övervaknings inställningar. Se även komma igång med roller, behörigheter och säkerhet med Azure Monitor. | Ja | 
Övervaknings mått utgivare | Möjliggör publicering av mått mot Azure-resurser | Ja | 
Övervaknings läsare | Kan läsa alla övervaknings data (mått, loggar osv.). Se även komma igång med roller, behörigheter och säkerhet med Azure Monitor. | Nej | 
Nätverksdeltagare | Gör att du kan hantera nätverk, men inte till gång till dem. | Ja | 
Ny Relic APM-konto deltagare | Låter dig hantera New Relic Application Performance Management konton och program, men inte till gång till dem. | Ja | 
Läsare och data åtkomst | Gör att du kan visa allting men du kan inte ta bort eller skapa ett lagrings konto eller en resurs som saknas. Den kommer också att tillåta Läs-/skriv åtkomst till alla data som finns i ett lagrings konto via åtkomst till lagrings konto nycklar. | Ja | 
Redis Cache deltagare | Låter dig hantera Redis-cacheer, men inte till gång till dem. | Ja | 
Resurs princip deltagare (för hands version) | Förhandsgranskningsvyn Användare med egna användare från EA, med behörighet att skapa/ändra resurs principer, skapa support ärende och läsa resurser/hierarki. | Ja | 
Jobb samlings deltagare i Scheduler | Gör att du kan hantera jobb samlingar i Scheduler, men inte till gång till dem. | Ja | 
Search Service deltagare | Låter dig hantera Sök tjänster, men inte till gång till dem. | Ja | 
Säkerhetsadministratör | Endast i Security Center: kan visa säkerhets principer, Visa säkerhets tillstånd, redigera säkerhets principer, Visa aviseringar och rekommendationer, ignorera aviseringar och rekommendationer | Ja | 
Säkerhets hanterare (bakåtkompatibelt) | Detta är en äldre roll. Använd säkerhets administratör istället | Ja | 
Säkerhetsläsare | Endast i Security Center: kan visa rekommendationer och aviseringar, Visa säkerhets principer, Visa säkerhets tillstånd, men kan inte göra ändringar | Nej | 
Site Recovery-deltagare | Låter dig hantera Site Recovery tjänst förutom att skapa valv och roll tilldelning | Ja | 
Site Recovery-operatör | Låter dig redundansväxla och failback men inte utföra andra Site Recovery hanterings åtgärder | Ja | 
Site Recovery-läsare | Låter dig Visa Site Recovery status men inte utföra andra hanterings åtgärder | Nej | 
Konto deltagare för spatiala ankare | Låter dig hantera spatiala ankare i ditt konto, men ta inte bort dem | Ja | 
Konto ägare för spatiala ankare | Låter dig hantera spatialdata i ditt konto, inklusive att ta bort dem | Ja | 
Konto läsare för spatiala ankare | Gör att du kan hitta och läsa egenskaper för spatiala ankare i ditt konto | Nej | 
SQL DB-deltagare | Gör att du kan hantera SQL-databaser, men inte åtkomst till dem. Du kan inte heller hantera säkerhets relaterade principer eller överordnade SQL-servrar. | Ja | 
SQL-hanterad instans deltagare | Låter dig hantera SQL-hanterade instanser och nödvändig nätverks konfiguration, men kan inte ge åtkomst till andra. | Ja | 
SQL-säkerhetshanteraren | Gör att du kan hantera säkerhetsrelaterade principer för SQL-servrar och databaser, men inte åtkomst till dem. | Ja | 
SQL Server deltagare | Gör att du kan hantera SQL-servrar och databaser, men inte åtkomst till dem och inte deras säkerhetsrelaterade principer. | Ja | 
Lagringskontodeltagare | Tillåter hantering av lagrings konton. Ger åtkomst till konto nyckeln, som kan användas för att få åtkomst till data via autentisering med delad nyckel. | Ja | 
Lagrings kontots nyckel operatörs tjänst roll | Tillåter att du visar och återskapar åtkomst nycklar för lagrings kontot. | Ja | 
Storage Blob Data-deltagare | Läsa, skriva och ta bort Azure Storage behållare och blobbar. Information om vilka åtgärder som krävs för en specifik data åtgärd finns i behörigheter för att anropa blob-och Queue data-åtgärder. | Ja | 
Storage Blob Data-ägare | Ger fullständig åtkomst till Azure Storage BLOB-behållare och data, inklusive att tilldela POSIX-åtkomstkontroll. Information om vilka åtgärder som krävs för en specifik data åtgärd finns i behörigheter för att anropa blob-och Queue data-åtgärder. | Ja | 
Storage Blob Data-läsare | Läs och Visa Azure Storage behållare och blobbar. Information om vilka åtgärder som krävs för en specifik data åtgärd finns i behörigheter för att anropa blob-och Queue data-åtgärder. | Nej | 
Storage BLOB-delegerare | Hämta en användar Delegerings nyckel som sedan kan användas för att skapa en signatur för delad åtkomst för en behållare eller BLOB som är signerad med Azure AD-autentiseringsuppgifter. Mer information finns i skapa en användar Delegerings-SAS. | Ja | 
Storage-fildata för SMB-resursdeltagare | Tillåter Läs-, skriv-och borttagnings åtkomst i Azure Storage fil resurser över SMB | Ja | 
Storage-fildata för upphöjd SMB-resursdeltagare | Tillåter behörighet att läsa, skriva, ta bort och ändra NTFS-behörighet i Azure Storage fil resurser över SMB | Ja | 
Storage-fildata för SMB-resursläsare | Tillåter Läs åtkomst till Azure-filresurs via SMB | Nej | 
Data deltagare i Storage Queue | Läsa, skriva och ta bort Azure Storage köer och köa meddelanden. Information om vilka åtgärder som krävs för en specifik data åtgärd finns i behörigheter för att anropa blob-och Queue data-åtgärder. | Ja | 
Processor för data meddelande i lagrings kön | Granska, hämta och ta bort ett meddelande från en Azure Storage kö. Information om vilka åtgärder som krävs för en specifik data åtgärd finns i behörigheter för att anropa blob-och Queue data-åtgärder. | Ja | 
Avsändare av data meddelande i lagrings köer | Lägg till meddelanden i en Azure Storage-kö. Information om vilka åtgärder som krävs för en specifik data åtgärd finns i behörigheter för att anropa blob-och Queue data-åtgärder. | Ja | 
Data läsare för lagrings kön | Läs och Visa Azure Storage köer och köa meddelanden. Information om vilka åtgärder som krävs för en specifik data åtgärd finns i behörigheter för att anropa blob-och Queue data-åtgärder. | Nej | 
Support förfrågan deltagare | Gör att du kan skapa och hantera support förfrågningar | Ja | 
Traffic Manager deltagare | Låter dig hantera Traffic Manager profiler, men låter dig inte kontrol lera vem som har åtkomst till dem. | Ja | 
Administratör för användaråtkomst | Gör att du kan hantera användar åtkomst till Azure-resurser. | Ja | 
Administratörs inloggning för virtuell dator | Visa Virtual Machines i portalen och logga in som administratör | Ja | 
Virtuell datordeltagare | Låter dig hantera virtuella datorer, men inte åtkomst till dem, inte det virtuella nätverk eller lagrings konto som de är anslutna till. | Ja | 
Användar inloggning för virtuell dator | Visa Virtual Machines i portalen och logga in som en vanlig användare. | Ja | 
Webb Plans deltagare | Gör att du kan hantera webb planer för webbplatser, men inte till gång till dem. | Ja | 
Webbplats deltagare | Gör att du kan hantera webbplatser (inte webb planer), men inte åtkomst till dem | Ja |

## <a name="next-steps"></a>Nästa steg

- [Partner intjänad kredit – en översikt över hur det fungerar i den nya Commerce-upplevelsen i CSP](partner-earned-credit.md)
