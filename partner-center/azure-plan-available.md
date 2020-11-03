---
title: Tillgängliga Azure-tjänster i Azure CSP
description: I det här avsnittet beskrivs de Azure-tjänster som är och inte är tillgängliga i Azure Cloud Solution Provider (CSP)-programmet.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: amitravat
ms.author: amrava
ms.localizationpriority: high
ms.date: 05/13/2020
ms.custom: SEOMAY.20
ms.openlocfilehash: 094aa585be3114c198a8581b3d23bd4b212393c9
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/22/2020
ms.locfileid: "92531561"
---
# <a name="azure-services-available-in-the-azure-cloud-solution-provider-csp-program"></a>Azure-tjänster som är tillgängliga i Azure Cloud Solution Provider (CSP)-programmet

**Lämpliga roller**

- Administratörs agent
- Faktureringsadministratör
- Global administratör
- Support agent
- Försäljnings agent
- Administratör för användar hantering

## <a name="available-azure-services-in-azure-csp"></a>Tillgängliga Azure-tjänster i Azure CSP

Den här artikeln innehåller de Azure-tjänster som är och inte är tillgängliga i Azure Cloud Solution Provider-programmet (CSP). Tjänsten diskuterar också tjänstens tillgänglighet i de nationella molnen [Microsoft Azure Tyskland](https://azure.microsoft.com/overview/clouds/germany/) och [Microsoft Azure Government](https://azure.microsoft.com/overview/clouds/government/).

>[!Note]
> [Azure Kina](https://www.azure.cn/) är inte tillgänglig i Azure CSP-programmet.

## <a name="global-cloud"></a>Globalt moln

Alla tjänster som baseras på Azure Resource Manager modell är tillgängliga i CSP-programmet.  Icke-Azure Resource Manager tjänster är inte tillgängliga i CSP-programmet.  

## <a name="csp-specific-service-configurations"></a>CSP-Specific-tjänstekonfigurationer

Följande tjänster kräver särskilda konfigurationer i CSP:

- [StorSimple](/azure/storsimple/storsimple-partner-csp-overview)

- [Azure Active Directory Domain Services](/azure/active-directory-domain-services/active-directory-ds-csp)

- [Key Vault](https://azurecsp.blob.core.windows.net/files/key-vault-in-csp.docx)

- [Azure Time Series Insights](https://azure.microsoft.com/services/time-series-insights/) Endast användare från kund innehavaren kan komma åt data i sin Time Series Insightss miljö. Partner kan hantera sin kunds Time Series Insights miljö som standard, men om de behöver åtkomst till data i den måste de läggas till i kund klienten.

## <a name="visual-studio-marketplace"></a>Visual Studio Marketplace

Nu kan du köpa de objekt som anges nedan från Visual Studio Marketplace, med undantag för tillägg från tredje part.

- [Azure DevOps](https://www.visualstudio.com/team-services/)

- [Visual Studio-prenumerationer](https://www.visualstudio.com/subscriptions/)

- [Xamarin University utbildning](https://marketplace.visualstudio.com/items?itemName=ms.xamarin-university)

För att hjälpa dig att komma igång har vi skapat videor och dokumentation om [hur du konfigurerar, köper och hanterar Azure-DevOps](/vsts/billing/csp/set-up-csp-customer) i CSP.

## <a name="azure-marketplace-items-in-azure-csp"></a>Azure Marketplace-objekt i Azure CSP

Alla Azure Marketplace-objekt är för närvarande inte tillgängliga i Azure CSP-prenumerationer.

- Microsoft-baserade Azure-tjänster: de här tjänsterna är tillgängliga. Granska föregående tabell och kommentarer.

- Bring your own license (BYOL): objekten är tillgängliga. En fullständig lista över BYOL-aktiverade Azure Marketplace-objekt finns på [Azure Marketplace BYOL-sidan](https://azuremarketplace.microsoft.com/marketplace/apps?filters=byol).

- Betala per användning för Azure Marketplace-objekt från tredje part: dessa objekt är tillgängliga om providern har publicerats på CSP-kanalen. Mer information finns i [Sälj prenumerationer på Azure Marketplace-produkter](csp-commercial-marketplace-overview.md).

- Citrix XenApp Essentials: partner kan köpa XenApp Essentials för kunder i CSP. Mer information finns i följande Citrix- [distribution av XenApp Essentials som nu är tillgängligt via kanalen för Microsoft Cloud Solution Provider](https://www.citrix.com/blogs/2018/02/01/xenapp-essentials-now-available-through-microsoft-cloud-solution-provider-channel/).

## <a name="national-clouds"></a>Nationella moln

I följande tabell visas en regelbundet uppdaterad lista över tillgängliga Azure-produkter, tjänster och funktioner från första part för CSP i nationella moln.

| Azure-produkt, tjänst eller funktion | US Government | Tyskland |
| ------ | :-----------: | :-----------: |
|  **Beräkning**  |    |    |
|  Virtual Machines  |  X  |  X  |
|  Cloud Services  |    |    |
|  Skalningsuppsättningar för virtuella datorer  |  X  |  X  |
|  Functions  |    |    |
|  Azure Container Service  |    |    |
|  **Nätverk**  |    |    |
|  Azure DNS  |    |    |
|  Content Delivery Network  |    |    |
|  Traffic Manager  |    |    |
|  ExpressRoute  |  X  |  X  |
|  Virtual Network  |  X  |  X  |
|  Load Balancer  |  X  |  X  |
|  VPN Gateway  |  X  |  X  |
|  Application Gateway  |  X  |  X  |
|  Network Watcher  |  X  |  X  |
|  **Storage**  |    |    |
|  Storage  |  X  |  X  |
|  Backup  |  X  |  X  |
|  StorSimple  |    |  X  |
|  Site Recovery  |  X  |  X  |
|  Data Lake Store  |    |    |
|  Managed Disks  |  X  |  X  |
|  **Webb och mobilt**  |    |    |
|  App Service  |  X  |  X  |
|  App Service på Linux  |    |  X  |
|  API Management  |  X  |    |
|  Content Delivery Network  |    |    |
|  Media Services  |  X  |  X  |
|  Notification Hubs  |  X  |  X  |
|  Azure Search  |    |    |
|  Logic Apps funktion i Azure App Service  |    |    |
|  **Containrar**  |    |    |
|  App Service  |  X  |  X  |
|  App Service på Linux  |    |  X  |
|  Batch  |  X  |  X  |
|  Container Registry  |    |    |
|  Container Instances  |    |    |
|  Service Fabric  |  X  |  X  |
|  Container Service  |    |    |
|  **Databaser**  |    |    |
|  SQL Database  |  X  |  X  |
|  Azure Cosmos DB  |  X  |  X  |
|  SQL Data Warehouse  |  X  |  X  |
|  Redis Cache  |  X  |  X  |
|  SQL Server Stretch Database  |  X  |  X  |
|  Azure Database for MySQL  |    |    |
|  Azure Database for PostgreSQL  |    |    |
|  **Data och analys**  |    |    |
|  Databricks  |    |    |
|  HDInsight  |  X  |  X  |
|  Stream Analytics  |    |  X  |
|  Data Factory  |    |    |
|  Log Analytics  |  X  |    |
|  Data Catalog  |    |    |
|  Data Lake Store  |    |    |
|  Data Lake Analytics  |    |    |
|  Azure Analysis Services  |    |    |
|  Power BI Embedded  |    |    |
|  **Artificiell intelligens och Cognitive Services**  |    |    |
|  Machine Learning  |    |  X  |
|  Azure Bot Service  |    |    |
|  Cognitive Services  |    |    |
|  Azure Batch AI  |    |    |
|  **Internet of Things**  |    |    |
|  IoT Hub  |  X  |  X  |
|  IoT Central  |    |    |
|  Machine Learning  |    |  X  |
|  Stream Analytics  |    |  X  |
|  Event Hubs  |  X  |  X  |
|  Location-Based tjänster  |    |    |
|  Notification Hubs  |  X  |  X  |
|  Time Series Insights  |    |    |
|  **Enterprise-integration**  |    |    |
|  StorSimple  |  X  |    |
|  API Management  |    |    |
|  Event Grid  |    |    |
|  Data Factory  |    |    |
|  Service Bus  |  X  |  X  |
|  Data Catalog  |    |    |
|  SQL Server Stretch Database  |    |  X  |
|  Logic Apps funktion i Azure App Service  |    |    |
|  **Säkerhet och identitet**  |    |    |
|  Azure Active Directory  |  X  |  X  |
|  Azure Active Directory B2C  |    |    |
|  Multi-Factor Authentication  |    |    |
|  Azure Active Directory Domain Services  |    |    |
|  Key Vault  |  X  |  X  |
|  Security Center  |  X  |  X  |
|  **Utvecklarverktyg**  |    |    |
|  Visual Studio Team Services  |    |    |
|  Application Insights  |    |    |
|  DevTest Labs  |    |    |
|  Visual Studio App Center  |    |    |
|  Xamarin University  |    |    |
|  **Övervakning och hantering**  |    |    |
|  Advisor  |    |    |
|  Backup  |  X  |  X  |
|  Site Recovery  |  X  |  X  |
|  Scheduler  |  X  |  X  |
|  Automation  |  X  |  X  |
|  Log Analytics  |  X  |    |
|  Azure Monitor  |    |    |
|  Azure-Managed program  |    |    |
|  Azure Migrate  |    |    |
|  Hanteringsgrupper  |    |  

## <a name="next-steps"></a>Nästa steg

- [Lär dig](/azure/cloud-solution-provider/overview/partner-center-overview) mer om tillgängliga funktioner för Azure i Partner Center.

- [Skapa](/azure/cloud-solution-provider/customer-management/create-new-customer) din första kund i Azure CSP och Distribuera Azure-tjänster.
