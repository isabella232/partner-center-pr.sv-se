---
title: Tillgängliga Azure-tjänster i Azure CSP
description: I den här artikeln beskrivs de Azure-tjänster som är och inte är tillgängliga i Programmet Azure Molnlösningsleverantör (CSP).
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
author: amitravat
ms.author: amrava
ms.localizationpriority: high
ms.date: 05/13/2020
ms.custom: SEOMAY.20
ms.openlocfilehash: 6037044a72bd9bd71131ddbc66fec0555bbd5f86
ms.sourcegitcommit: 1161d5bcb345e368348c535a7211f0d353c5a471
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/09/2021
ms.locfileid: "123961216"
---
# <a name="azure-services-available-in-the-azure-cloud-solution-provider-csp-program"></a>Azure-tjänster som är tillgängliga i Programmet Azure Molnlösningsleverantör (CSP)

**Lämpliga roller:** Administratörsagent | Faktureringsadministratörskonto | Globala | Supportagent | Försäljningsagent | Administratör för användarhantering

## <a name="available-azure-services-in-azure-csp"></a>Tillgängliga Azure-tjänster i Azure CSP

I den här artikeln listas de Azure-tjänster som är och inte är tillgängliga i Programmet Azure Molnlösningsleverantör (CSP). Den beskriver också tjänsttillgänglighet i de nationella molnen [Microsoft Azure Tyskland](https://azure.microsoft.com/overview/clouds/germany/) och [Microsoft Azure myndigheter.](https://azure.microsoft.com/overview/clouds/government/)

>[!Note]
> [Azure China](https://www.azure.cn/) är inte tillgängligt i Azure CSP program.

## <a name="global-cloud"></a>Globalt moln

Alla tjänster baserat på Azure Resource Manager är tillgängliga i CSP-programmet.  Icke-Azure Resource Manager tjänster som klassiska distributionsmodelltjänster är inte tillgängliga i CSP-programmet.  

## <a name="csp-specific-service-configurations"></a>CSP-Specific servicekonfigurationer

Följande tjänster kräver särskilda konfigurationer i CSP:

- [StorSimple](/azure/storsimple/storsimple-partner-csp-overview)

- [Azure Active Directory Domain Services](/azure/active-directory-domain-services/active-directory-ds-csp)

- [Key Vault](https://azurecsp.blob.core.windows.net/files/key-vault-in-csp.docx)

- [Azure Time Series-Insights](https://azure.microsoft.com/services/time-series-insights/) Endast användare från kundklientorganisationen kan komma åt data i sin Time Series Insights miljö. Partner kan hantera sina kunders time series-Insights som standard, men om de behöver åtkomst till data i den måste de läggas till i kundens klientorganisation.

- Hanteringscertifikat för autentisering av Azure SDK-bibliotek via certifikat stöds inte i CSP-modellen.  Använd autentisering med Azure AD-tjänstens huvudnamn och Azure.Identity-biblioteket i stället.  Referens [för autentisering med Azure SDK för .NET](/dotnet/azure/sdk/authentication)

## <a name="visual-studio-marketplace"></a>Visual Studio Marketplace

Du kan nu köpa objekten nedan från Visual Studio Marketplace, med undantag för tillägg från tredje part.

- [Azure DevOps](https://www.visualstudio.com/team-services/)

- [Visual Studio prenumerationer](https://www.visualstudio.com/subscriptions/)

- [Xamarin University utbildning](https://marketplace.visualstudio.com/items?itemName=ms.xamarin-university)

För att hjälpa dig att komma igång har vi skapat videor och dokumentation om hur du ställer in, köper och [hanterar Azure DevOps](/vsts/billing/csp/set-up-csp-customer) i CSP.

## <a name="azure-marketplace-items-in-azure-csp"></a>Azure Marketplace-objekt i Azure CSP

För närvarande är Azure Marketplace objekt inte tillgängliga i Azure CSP prenumerationer.

- Microsoft-baserade Azure-tjänster: Dessa tjänster är tillgängliga. Granska föregående tabell och kommentarer.

- Bring your own license (BYOL): Dessa objekt är tillgängliga. En fullständig lista över BYOL-aktiverade Azure Marketplace objekt finns på sidan [Azure Marketplace BYOL](https://azuremarketplace.microsoft.com/marketplace/apps?filters=byol).

- Information om tredjepartsobjekt med betalas Azure Marketplace: De här objekten är tillgängliga om leverantören har publicerat till CSP-kanalen. Mer information finns i Sälja [prenumerationer till Azure Marketplace produkter.](csp-commercial-marketplace-overview.md)

- Citrix XenApp Essentials: Partner kan köpa XenApp Essentials kunder i CSP. Mer information finns i följande Citrix-blogg – [Distribution av XenApp Essentials nu tillgänglig via Leverantör av Microsoft-molnlösningar Channel](https://www.citrix.com/blogs/2018/02/01/xenapp-essentials-now-available-through-microsoft-cloud-solution-provider-channel/).

## <a name="national-clouds"></a>Nationella moln

I följande tabell visas en regelbundet uppdaterad lista över tillgängliga Produkter, tjänster och funktioner från första part för CSP i nationella moln.

| Azure-produkt, -tjänst eller -funktion | US Government | Tyskland |
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
|  Location-Based Services  |    |    |
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

- [Lär](/azure/cloud-solution-provider/overview/partner-center-overview) dig mer om de tillgängliga funktionerna för Azure i Partnercenter.

- [Skapa](/azure/cloud-solution-provider/customer-management/create-new-customer) din första kund i Azure CSP och distribuera Azure-tjänster.
