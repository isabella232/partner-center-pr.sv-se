---
title: Köpa erbjudanden på den kommersiella marknadsplatsen
ms.topic: how-to
ms.date: 09/27/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
description: Lär dig hur CSP-programpartner kan använda Partner Center Marketplace för att göra kundinköp av SaaS-erbjudanden från oberoende programvaruleverantörer (ISV).
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 4f837fb9319d49657f10ea7e01684ab5fb0fb9aa
ms.sourcegitcommit: e1da62b36420d78bf44e3962358d0af65ebc3402
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/27/2021
ms.locfileid: "129089581"
---
# <a name="purchase-commercial-marketplace-products-for-your-customers-in-partner-center"></a>Köpa produkter på den kommersiella marknadsplatsen för dina kunder i Partnercenter


**Lämpliga roller:** Global | Administratörsagent

Som partner i programmet Molnlösningsleverantör (CSP) kan du använda den kommersiella marknadsplatsen för att köpa prenumerationer för dina kunder till vissa SaaS-produkter (Programvara som en tjänst) som erbjuds av oberoende programvaruleverantörer (ISV).

Genom att erbjuda ISV SaaS-prenumerationer till dina kunder kan du hjälpa dig att särskilja din verksamhet. Du kan också ge kunderna åtkomst till programvarupaket som tillgodoser deras specifika affärsbehov. Du hanterar licenser och prenumerationer för dessa Marketplace SaaS-produkter från ISV-utgivare precis som du hanterar licenser och prenumerationer för Microsoft-produkter.

Du kan köpa **antingen licensbaserade** SaaS-prenumerationer eller **användningsbaserade** prenumerationer. Mer information om skillnaden mellan licensbaserad och användningsbaserad fakturering finns i [Fakturerings grunder.](billing-basics.md)

## <a name="purchase-license-based-and-metered-saas-subscriptions-in-partner-center"></a>Köpa licensbaserade och uppmätta SaaS-prenumerationer i Partnercenter

Du köper prenumerationer för licensbaserade eller uppmätta SaaS-produkter som erbjuds av ISV-utgivare med samma process som du använder för att köpa prenumerationer för Microsoft-produkter.

Om du vill köpa en licensbaserad eller uppmätt SaaS-prenumeration i Partnercenter kan du läsa [Skapa, pausa eller avbryta kundprenumerationer.](create-a-new-subscription.md#create-a-new-subscription)

Du kan också använda [Partner Center-API:er för](/partner-center/develop/) att skapa prenumerationer på den kommersiella marknadsplatsen för dina kunder. (Mer information om hur du använder Partner Center-API:er finns i [Skapa en prenumeration för produkter på den kommersiella marknadsplatsen](/partner-center/develop/create-subscription-azure-marketplace-products).)

> [!IMPORTANT]
> Som partner i CSP-programmet kan du köpa  licensbaserade eller uppmätta SaaS-prenumerationer från **ISV-utgivare** i Partnercenter. Det innebär att du kan köpa alla licensbaserade eller **uppmätta** SaaS-erbjudanden [](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) som **ISV-utgivaren** har gjort tillgängliga för dig, inklusive exklusiva erbjudanden som du har åtkomst till. Om du vill köpa eller hantera andra erbjudanden på den kommersiella marknadsplatsen från ISV:er (till exempel användningsbaserade erbjudanden som rör Azure-program, containrar eller virtuella datorer) måste du [gå till Azure Portal](https://portal.azure.com/).

## <a name="purchase-usage-based-subscriptions-in-the-azure-portal"></a>Köpa användningsbaserade prenumerationer i Azure Portal

Till skillnad från licensbaserade SaaS-prenumerationer från tredjeparts ISV-utgivare kräver användningsbaserade prenumerationer först att kunden har en Azure-prenumeration. Fakturering för den kommersiella marknadsplatsen, användningsbaserade resurser faller under kundens Azure-prenumeration. När kunden har en Azure-prenumeration kan en partner i CSP-programmet följa dessa steg för att köpa en prenumeration på den kommersiella marknadsplatsen för dem:

> [!NOTE]
> Mer information om gränssnittet för arbetsytor finns i [Getting around Partner Center (Ta sig runt i Partnercenter).](get-around-partner-center.md#turn-workspaces-on-and-off)

#### <a name="workspaces-view"></a>[Vy över arbetsytor](#tab/workspaces-view)

1. Logga in på [instrumentpanelen i Partnercenter](https://partner.microsoft.com/dashboard)och välj **sedan panelen** Kunder.

2. Välj den specifika kunden och välj sedan **Prenumerationer.**  

3. Under **Användningsbaserade prenumerationer väljer** du **Alla resurser**. Då kommer du till Azure-hanteringsportalen.

4. I Azure-hanteringsportalen **väljer du Skapa en** resurs på den vänstra menyn.

5. Välj **Visa alla** överst i listan Azure Marketplace listan.

6. Om du vill begränsa listan använder du filter överst i Marketplace-listan. Du kan till exempel välja **Microsoft** eller **Partner** **Publisher** listrutan om du bara vill visa erbjudanden från Microsoft eller från en ISV-utgivare.

7. Välj ett specifikt erbjudande och välj sedan **Skapa.**

#### <a name="current-view"></a>[Aktuell vy](#tab/current-view)

1. Logga in på [instrumentpanelen i Partnercenter](https://partner.microsoft.com/dashboard)och **välj** sedan Kunder på den vänstra menyn.

2. Välj den specifika kunden och välj sedan **Prenumerationer.**  

3. Under **Användningsbaserade prenumerationer väljer** du **Alla resurser**. Då kommer du till Azure-hanteringsportalen.

4. I Azure-hanteringsportalen **väljer du Skapa en** resurs på den vänstra menyn.

5. Välj **Visa alla** överst i listan Azure Marketplace listan.

6. Om du vill begränsa listan använder du filter överst i Marketplace-listan. Du kan till exempel välja **Microsoft** eller **Partner** **Publisher** listrutan om du bara vill visa erbjudanden från Microsoft eller från en ISV-utgivare.

7. Välj ett specifikt erbjudande och välj sedan **Skapa.**

* * *

## <a name="next-steps"></a>Nästa steg

- [Hantera erbjudanden på den kommersiella marknadsplatsen](csp-commercial-marketplace-purchase.md)
