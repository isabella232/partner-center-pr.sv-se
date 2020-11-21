---
title: Partnerintegreringar för Azure Marketplace
description: Lär dig om Azure Marketplace-lösningar som integreras med din Azure-miljö och få länkar till distributions guider från Microsoft-partner.
ms.service: partner-services
ms.topic: conceptual
author: JasonWHowell
ms.author: jasonh
ms.date: 11/16/2020
ms.openlocfilehash: b31486000e59f3d85ee30019ecea000252b297a8
ms.sourcegitcommit: 1aa43438ad181278052788f15e017f9ae7777943
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 11/21/2020
ms.locfileid: "95006913"
---
# <a name="azure-marketplace-partner-integrations"></a>Partnerintegreringar för Azure Marketplace

Lär dig hur du integrerar partner lösningar i din Azure-miljö. Den här artikeln ger en översikt över varje lösning och länkar till detaljerade distributions guider. Lösningar visas i alfabetisk ordning. 

## <a name="apache-kafka-on-confluent-cloud"></a>Apache Kafka i ett samfluent-moln

![Flytande moln](./media/partners/confluent-cloud.png)

Med Azure kan du integrera med ett hanterings moln, förutom dina moln program. Det går ofta att navigera mellan Azure Portal och molnet. När en användare t. ex. köper ett erbjudande om moln erbjudande i Azure Marketplace förväntas de konfigurera ett konto med ett moln. Den här processen ökar komplexiteten och tiden och kräver att användare hanterar konfiguration och resurser mellan de två portalerna. För att minska belastningen på att hantera mellan plattformar, är Microsoft i samarbete med samarbetes molnet byggt ett integrerat etablerings lager från Azure till ett integrerat moln. Lösningen är tillgänglig i Azure Marketplace och ger en sömlös upplevelse för att använda sig av ett kunskaps moln erbjudande i Azure

Lösningen använder en resurs leverantör som är aktive rad i Azure för att etablera moln resurser i molnet. Detta gör det möjligt för användare att komma åt händelse strömning i real tid via Azure Portal, Azure CLI och Azure SDK: er. Samarbets molnet äger och kör SaaS-programmet, som innehåller miljöer, kluster, ämnen, API-nycklar och hanterade anslutningar.

Den djupgående integrationen med samordnings molnet möjliggör följande funktioner:

- Etablera en ny miljö organisations resurs från Azure Portal med helt hanterad infrastruktur.
- Effektivisera enkel inloggning från Azure till att avhjälpa molnet med Azure Active Directory; ingen separat autentisering krävs från samarbets moln portalen.
- Få en enhetlig fakturering av samkostnader för moln förbrukning via prenumerations fakturering i Azure.
- Hantera moln resurser från Azure Portal och spåra dem på sidan **alla resurser** , tillsammans med dina Azure-resurser.

[Distributions guider för distributions moln](https://docs.confluent.io/current/cloud/marketplace/index.html)

Om du har problem med att komma igång med Azure går du till [https://support.confluent.io](https://support.confluent.io) . Om du är en första gången måste du återställa ditt lösen ord innan du loggar in på den omvända support portalen. Om du inte har ett konto med överföring kan du skicka ett e-postmeddelande till [cloud-support@confluent.io](mailto:cloud-support@confluent.io) .

## <a name="datadog"></a>Datadog

![DataDog-logotyp](./media/partners/datadog.png)

Datadog tillhandahåller kortsiktiga och säkerhets verktyg som Azure-användare kan använda för att förstå hälso tillståndet och prestandan för sina program i hybrid miljöer och miljöer med flera moln. Men om du konfigurerar nödvändiga integreringar måste du ofta navigera mellan Azure Portal-och Datadog. För att förenkla konfiguration och resurs hantering i portaler har Microsoft arbetat med Datadog för att skapa en integrerad Datadog-lösning på Azure. Den här lösningen är tillgänglig via Azure Marketplace och ger en sömlös upplevelse för Azure-kunder att använda Datadogs lösning för moln övervakning.

Se [Azure Monitor-dokumentationen](/azure/azure-monitor/platform/partners#datadog) om du vill veta mer om den här lösningen och registrera dig för den offentliga för hands versionen.

## <a name="next-steps"></a>Nästa steg

- [Azure Marketplace-onlinebutik](https://azure.microsoft.com/marketplace/)
- [Microsoft Learn: skapa ett Azure-konto](/learn/modules/create-an-azure-account/)
