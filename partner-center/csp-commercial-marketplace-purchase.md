---
title: Köpa erbjudanden på den kommersiella marknadsplatsen
ms.topic: how-to
ms.date: 05/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
description: Lär dig hur CSP-programpartner kan använda Partner Center Marketplace för att göra kundköp av SaaS-erbjudanden från oberoende programvaruleverantörer (ISV).
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 2984dbb3a02df91d5a2a284182476bf348a24f47
ms.sourcegitcommit: 1161d5bcb345e368348c535a7211f0d353c5a471
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/09/2021
ms.locfileid: "123960096"
---
# <a name="purchase-commercial-marketplace-products-for-your-customers-in-partner-center"></a>Köpa produkter från den kommersiella marknadsplatsen för dina kunder i Partnercenter


**Lämpliga roller:** Globala | Administratörsagent

Som partner i Molnlösningsleverantör-programmet (CSP) kan du använda den kommersiella marknadsplatsen för att köpa prenumerationer för dina kunder till vissa SaaS-produkter (Programvara som en tjänst) som erbjuds av oberoende programvaruleverantörer (ISV:er).

Genom att erbjuda ISV SaaS-prenumerationer till dina kunder kan du göra skillnad på din verksamhet. Du kan också ge kunderna åtkomst till programvarupaket som tillgodoser deras specifika affärsbehov. Du hanterar licenser och prenumerationer för dessa Marketplace SaaS-produkter från ISV-utgivare på samma sätt som du hanterar licenser och prenumerationer för Microsoft-produkter.

Du kan köpa **antingen licensbaserade** SaaS-prenumerationer **eller användningsbaserade** prenumerationer. Mer information om skillnaden mellan licensbaserad och användningsbaserad fakturering finns i [Fakturerings grunder.](billing-basics.md)

## <a name="purchase-license-based-and-metered-saas-subscriptions-in-partner-center"></a>Köpa licensbaserade och uppmätta SaaS-prenumerationer i Partnercenter

Du köper prenumerationer för licensbaserade eller uppmätta SaaS-produkter som erbjuds av ISV-utgivare med samma process som du använder för att köpa prenumerationer för Microsoft-produkter.

Om du vill köpa en licensbaserad eller uppmätt SaaS-prenumeration i Partnercenter kan du läsa [Skapa, pausa eller avbryta kundprenumerationer.](create-a-new-subscription.md#create-a-new-subscription)

Du kan också använda [Partner Center-API:er för](/partner-center/develop/) att skapa prenumerationer på den kommersiella marknadsplatsen för dina kunder. (Mer information om hur du använder Partner Center-API:er finns i [Skapa en prenumeration för produkter på den kommersiella marknadsplatsen](/partner-center/develop/create-subscription-azure-marketplace-products).)

>[!IMPORTANT]
> Som partner i CSP-programmet kan du köpa  licensbaserade eller uppmätta SaaS-prenumerationer från **ISV-utgivare** i Partnercenter. Det innebär att du kan köpa alla licensbaserade eller uppmätta SaaS-erbjudanden [](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) som  **ISV-utgivaren** har gjort tillgängliga för dig, inklusive exklusiva erbjudanden som du har åtkomst till. Om du vill köpa eller hantera andra erbjudanden på den kommersiella marknadsplatsen från ISV:er (till exempel användningsbaserade erbjudanden som rör Azure-program, containrar eller virtuella datorer) måste du [gå till Azure Portal](https://portal.azure.com/).

## <a name="purchase-usage-based-subscriptions-in-the-azure-portal"></a>Köpa användningsbaserade prenumerationer i Azure Portal

Till skillnad från licensbaserade SaaS-prenumerationer från tredjeparts-ISV-utgivare kräver användningsbaserade prenumerationer först att kunden har en Azure-prenumeration. Fakturering för den kommersiella marknadsplatsen, användningsbaserade resurser faller under kundens Azure-prenumeration. När kunden har en Azure-prenumeration kan en partner i CSP-programmet följa dessa steg för att köpa en prenumeration på den kommersiella marknadsplatsen åt dem:

1. Logga in på [instrumentpanelen i Partnercenter](https://partner.microsoft.com/dashboard)och **välj** sedan Kunder på den vänstra menyn.

2. Välj den specifika kunden och välj sedan **Prenumerationer.**  

3. Under **Användningsbaserade prenumerationer väljer** du **Alla resurser**. Nu kommer du till Azure-hanteringsportalen.

4. I Azure-hanteringsportalen **väljer du Skapa en** resurs på menyn till vänster.

5. Välj **Visa alla** överst i Azure Marketplace listan.

6. Använd filter överst i Marketplace-listan för att begränsa listan. Du kan till exempel välja **Microsoft** eller **Partner** **från listrutan Publisher** att endast visa erbjudanden från Microsoft eller från en ISV-utgivare.

7. Välj ett specifikt erbjudande och välj sedan **Skapa**.

## <a name="next-steps"></a>Nästa steg

- [Hantera erbjudanden på den kommersiella marknadsplatsen](csp-commercial-marketplace-purchase.md)