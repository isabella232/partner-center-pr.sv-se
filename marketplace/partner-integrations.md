---
title: Partnerintegreringar för Azure Marketplace
description: Lär dig Azure Marketplace lösningar som integreras med din Azure-miljö och få en länk till distributionsguider från Microsoft-partner.
ms.service: partner-services
ms.topic: conceptual
author: JasonWHowell
ms.author: jasonh
ms.date: 11/16/2020
ms.openlocfilehash: 56e72af367cdcb264cc444446c5fcbedcd880451
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/17/2021
ms.locfileid: "112276492"
---
# <a name="azure-marketplace-partner-integrations"></a>Partnerintegreringar för Azure Marketplace

Lär dig hur du integrerar partnerlösningar i din Azure-miljö. Den här artikeln ger en översikt över varje lösning och länkar till detaljerade distributionsguider. Lösningar visas i alfabetisk ordning. 

## <a name="apache-kafka-on-confluent-cloud"></a>Apache Kafka på Confluent Cloud

![Confluent Cloud.](./media/partners/confluent-cloud.png)

Med Azure kan du integrera med Confluent Cloud utöver dina molnprogram. Confluent-kunder navigerar ofta mellan Azure Portal och Confluent Cloud. När en användare till exempel har köpt ett Confluent Cloud-erbjudande i Azure Marketplace förväntas de sedan konfigurera ett konto med Confluent Cloud. Den här processen ökar komplexiteten och tiden och kräver att användarna hanterar konfiguration och resurser mellan de två portalerna. För att minska hanteringsbelastningen mellan plattformar skapade Microsoft, i samarbete med Confluent Cloud, ett integrerat etableringslager från Azure till Confluent Cloud. Lösningen är tillgänglig i Azure Marketplace ger en sömlös upplevelse för att använda Confluent Cloud-erbjudandet på Azure

Lösningen använder en resursprovider som är aktiverad i Azure för att etablera Confluent Cloud-resurser. På så sätt kan användarna komma åt händelseströmning i realtid via Azure Portal, Azure CLI och Azure-SDK:er. Confluent Cloud äger och kör SaaS-programmet, som innehåller miljöer, kluster, ämnen, API-nycklar och hanterade anslutningsappar.

Den djupgående integreringen med Confluent Cloud möjliggör följande funktioner:

- Etablera en ny Confluent Cloud-organisationsresurs från Azure Portal med fullständigt hanterad infrastruktur.
- Effektivisera enkel inloggning från Azure till Confluent Cloud med Azure Active Directory; ingen separat autentisering krävs från Confluent Cloud-portalen.
- Få enhetlig fakturering av Confluent Cloud-förbrukningsavgifter via Azure-prenumerationsfakturering.
- Hantera Confluent Cloud-resurser från Azure Portal och spåra dem på **sidan Alla resurser** tillsammans med dina Azure-resurser.

[Distributionsguider för Confluent Cloud](https://docs.confluent.io/current/cloud/marketplace/index.html)

För problem som rör Confluent på Azure går du till [https://support.confluent.io](https://support.confluent.io) . Om du är första gången återställer du lösenordet innan du loggar in på Confluent-supportportalen. Om du inte har något konto med Confluent skickar du ett e-postmeddelande till [cloud-support@confluent.io](mailto:cloud-support@confluent.io) .

## <a name="datadog"></a>Datadog

![DataDog-logotyp.](./media/partners/datadog.png)

Datadog tillhandahåller verktyg för observerbarhet och säkerhet som Azure-användare kan använda för att förstå hälsotillståndet och prestandan hos sina program i hybridmiljöer och miljöer med flera moln. Men att konfigurera nödvändiga integreringar kräver ofta navigering mellan Azure Portal datadog. För att förenkla konfiguration och resurshantering i portaler arbetade Microsoft med Datadog för att skapa en integrerad Datadog-lösning i Azure. Den här Azure Marketplace är tillgänglig via internet och ger En sömlös upplevelse för Azure-kunder som kan använda Datadogs molnövervakningslösning.

Mer information [Azure Monitor den](/azure/azure-monitor/platform/partners#datadog) här lösningen och registrera dig för den offentliga förhandsversionen finns i dokumentationen för den offentliga förhandsversionen.

## <a name="next-steps"></a>Nästa steg

- [Azure Marketplace onlinebutik](https://azure.microsoft.com/marketplace/)
- [Microsoft Learn: Skapa ett Azure-konto](/learn/modules/create-an-azure-account/)
