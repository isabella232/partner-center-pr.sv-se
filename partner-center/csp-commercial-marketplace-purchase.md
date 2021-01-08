---
title: Köp kommersiella Marketplace-erbjudanden
ms.topic: how-to
ms.date: 05/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Lär dig hur CSP-programpartner kan använda Partner Center Marketplace för att göra kund inköp av SaaS-erbjudanden från oberoende program varu leverantörer (ISV).
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 841308d535d4071ee0a8eabf3e70325edea5777c
ms.sourcegitcommit: a78dd3c532860d01867d116bfb4e2c88b84bcd25
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 01/08/2021
ms.locfileid: "97979725"
---
# <a name="purchase-commercial-marketplace-products-for-your-customers-in-partner-center"></a>Köp kommersiella Marketplace-produkter för dina kunder i Partner Center


**Lämpliga roller**

- Global administratör
- Administratörs agent

Som partner i ett CSP-program (Cloud Solution Provider) kan du använda den kommersiella Marketplace för att köpa prenumerationer för dina kunder till vissa SaaS-produkter (Software as a Service) som erbjuds av oberoende program varu leverantörer (ISV).

Genom att erbjuda ISV SaaS-prenumerationer till dina kunder kan du hjälpa företaget att särskilja din verksamhet. Du kan också ge kunderna till gång till program varu paket som åtgärdar sina specifika affärs behov. Du hanterar licenser och prenumerationer för dessa Marketplace SaaS-produkter från ISV-utgivare, precis som du hanterar licenser och prenumerationer för Microsoft-produkter.

Du kan köpa antingen **licensbaserade** SaaS-prenumerationer eller **användnings baserade** prenumerationer. Mer information om skillnaden mellan licensierad och Använd fakturering finns i [fakturerings grunderna](billing-basics.md).

## <a name="purchase-license-based-and-metered-saas-subscriptions-in-partner-center"></a>Köp licensbaserade och avgiftsbelagda SaaS-prenumerationer i Partner Center

Du köper prenumerationer för licensbaserade eller avgiftsbelagda SaaS-produkter som erbjuds av ISV-utgivare med samma process som du använder för att köpa prenumerationer för Microsoft-produkter.

Om du vill köpa en licensierad eller avgiftsbelagd SaaS-prenumeration i Partner Center, se [skapa, pausa eller annullera kund prenumerationer](create-a-new-subscription.md#create-a-new-subscription).

Du kan också använda [API: er för partner Center](/partner-center/develop/) för att skapa prenumerationer på kommersiella marknads platser för dina kunder. (Mer information om hur du använder API: er för partner Center finns i [skapa en prenumeration för kommersiella Marketplace-produkter](/partner-center/develop/create-subscription-azure-marketplace-products).)

>[!IMPORTANT]
> Som partner i CSP-programmet kan du köpa **licensbaserade** eller **avgiftsbelagda** SaaS-prenumerationer från ISV-utgivare i Partner Center. Det innebär att du kan köpa alla **licensbaserade** eller **avgiftsbelagda** SaaS-erbjudanden som ISV-utgivaren har gjort tillgängligt för dig, inklusive [exklusiva erbjudanden](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) som du har åtkomst till. För att köpa eller hantera andra erbjudanden från kommersiella Marketplace från ISV: er (till exempel användnings erbjudanden som rör Azure-program, behållare eller virtuella datorer) måste du gå till [Azure Portal](https://portal.azure.com/).

## <a name="purchase-usage-based-subscriptions-in-the-azure-portal"></a>Köp användnings prenumerationer i Azure Portal

Till skillnad från SaaS-prenumerationer från tredjeparts ISV-utgivare kräver användnings-baserade prenumerationer först en kund som har en Azure-prenumeration. Fakturering för kommersiell marknads plats är användnings baserade resurser under kundens Azure-prenumeration. När kunden har en Azure-prenumeration kan en partner i CSP-programmet följa de här stegen för att köpa en prenumeration på kommersiell marknads plats för dem:

1. Logga in på Partner Center- [instrumentpanelen](https://partner.microsoft.com/dashboard)och välj sedan **kunder** på menyn till vänster.

2. Välj den specifika kunden och välj sedan **prenumerationer**.  

3. Under de **användnings baserade prenumerationerna** väljer du **alla resurser**. Då går du till hanterings portalen för Azure.

4. I hanterings portalen för Azure väljer du **skapa en resurs** i den vänstra menyn.

5. Välj **Se alla** överst i listan Azure Marketplace.

6. Om du vill begränsa listan använder du filter överst i Marketplace-listan. Du kan till exempel välja **Microsoft** eller **partner** i list rutan **utgivare** om du bara vill visa erbjudanden från Microsoft eller från en ISV-utgivare.

7. Välj ett Special erbjudande och välj sedan **skapa**.

## <a name="next-steps"></a>Nästa steg

- [Hantera kommersiella Marketplace-erbjudanden](csp-commercial-marketplace-purchase.md)