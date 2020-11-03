---
title: Köp Azure-prenumerationen
ms.topic: how-to
ms.date: 06/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Använd Azure-planen för att lära dig att köpa en eller flera Azure-prenumerationer, Azure-reservationer, för att konfigurera resurser och för att visa eller lägga till prenumerationer.
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 6f9908be183983c590c52b38465041c908c91d7c
ms.sourcegitcommit: 37b0b2a7141907c8d21839de3128fb8a98575886
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2020
ms.locfileid: "92531196"
---
# <a name="purchase-the-azure-plan-for-customers--access-the-latest-azure-services-at-pay-as-you-go-rates"></a>Köp Azure-planen för kunder & få till gång till de senaste Azure-tjänsterna enligt priser enligt principen betala per användning

**Lämpliga roller**
- Global administratör
- Användaradministratör
- Försäljnings agent

När du köper en Azure-plan för dina kunder enligt Microsofts kund avtal har du till gång till den fullständiga katalogen med de senaste Azure-tjänsterna enligt priser enligt principen betala per användning. CSP-partner kommer nu att kunna komma åt alla Azure-tjänster när de blir allmänt tillgängliga. En partner kan ha flera Azure-prenumerationer under en Azure-plan. 

## <a name="countryregion-availability"></a>Tillgänglighet för land/region
Den nya Commerce-upplevelsen i CSP för Azure är för närvarande schemalagd för att vara tillgänglig i 139-länder. Se den fullständiga listan över dessa [länder/regioner](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE3QN0x). 

## <a name="how-to-purchase-azure-plan"></a>Så här köper du Azure-plan

Hur du köper Azure-planen liknar att köpa en annan prenumeration. Den viktigaste skillnaden är att innan du faktiskt placerar din beställning måste du bekräfta att kunden har undertecknat Microsofts kund avtal.

1. Välj **segment handels** -och typ **Microsoft Azure** 
2. Under Azure plan väljer **du Lägg till i kundvagn**

:::image type="content" source="images/azure/Azurepurchase1.png" alt-text="Köp":::

Partnern måste bekräfta att kunden har granskat och godkänt villkoren för Microsofts kund avtal. Mer information om hur partner kan göra detta finns i [bekräfta kund godkännande av Microsofts kund avtal](confirm-customer-agreement.md). Andra resurser är tillgängliga i [resurs galleriet](https://partner.microsoft.com/resources/collection/Microsoft-Customer-Agreement-in-the-CSP-program#/).

**För att bekräfta kan du antingen** : 

1. Bekräfta digitalt eller,

2. Bjud in kunden att logga Microsofts kund avtal direkt med Microsoft. 

### <a name="to-confirm"></a>För att bekräfta 

1. På sidan kund **konto** väljer du **Uppdatera** bredvid **Microsofts kund avtal**  

2. Fyll i informationen om den person som har godkänts av MCuA på kundens företag.

3. Välj **Spara och fortsätt.**  

## <a name="review-and-buy"></a>Granska och Köp

Du kommer tillbaka till sidan **Lägg till en produkt** där du kan se att Azure-planen har lagts till. Välj **Granska** för att granska ditt köp och välj sedan **köp** . 

>[!Note]
>När du har köpt Azure-prenumerationen för en kund kan du inte längre köpa Microsoft Azure (0145p) för kunden. Du måste skapa framtida prenumerationer via Azure-planen.

## <a name="purchase-azure-reservations-under-the-azure-plan"></a>Köp Azure-reservationer i Azure-planen 
  
Du kan också köpa Microsoft Azure reservationer under Azure-abonnemang åt dina kunder i Partner Center. (Om du vill kan du [ge dina kunder behörighet att köpa sina egna Azure-reservationer](give-customers-permission.md) från en tidigare prenumeration som du har köpt för dem.)

1. Från menyn Partner Center på [instrument panelen](https://partner.microsoft.com/dashboard/)väljer du **kunder** . Hitta kunden som vill köpa Azure-reservationer och välj sedan nedpilen för att expandera kundens rad.

2. Välj **Lägg till produkter** och välj sedan **Azure** . 

   - Välj kundens marknads segment i listan **segment** .
   - Välj **reservationer** i listan **produkt typ** .
   - Välj den typ av reservation som kunden vill ha från listan **reservations typ** .

Azure-reservationer måste associeras med en aktiv Azure-plan. Välj den Azure-plan som du vill lägga till Azure-reservationer i från listan med kund prenumerationer. 

>[!Important] 
>Om kunden inte redan har en aktiv Azure-plan väljer du Azure för att lägga till en nu. Mer information finns i [köpa Azure-reservationer](azure-reservations-buying.md#purchase-azure-reservations).

>[!Note]
>En reservations omfattning kan bara anges som **delad** , för närvarande i Partner Center. Om du vill välja en enskild prenumerations omfattning eller uppdatera från delad till en enda prenumeration går du till **Microsoft Azure hanterings Portal** med hjälp av följande instruktioner. 

:::image type="content" source="images/azure/addprods1.png" alt-text="Köp":::

Så här hanterar du kundens reservation i Azure Portal: 

1. Från **kunder** väljer du den kund som du vill hantera. 

2. Använd nedåtpilen och expandera kundens rad och välj **Microsoft Azure hanterings Portal** .  
 
## <a name="view-azure-subscriptions-under-the-azure-plan"></a>Visa Azure-prenumerationer under Azure-planen

På sidan **prenumerationer** i avsnittet användning, expanderar du **Azure plan** för att se associerade Azure-prenumerationer i Azure-planen.

:::image type="content" source="images/azure/addprods2.png" alt-text="Köp"::: 


## <a name="add-subscriptions-and-configure-resources"></a>Lägg till prenumerationer och konfigurera resurser

Du kommer att lägga till prenumerationer och konfigurera resurser för din kund i Azure Portal. Du kan också separera kundens miljö efter arbets belastning eller projekt. Det går att hantera prenumerationer via [Azure-Lighthouse](https://azure.microsoft.com/services/azure-lighthouse/) samt Azure Portal. 

Om du vill hantera kundens resurser och prenumerationer behöver du **administratör på uppdrag av** (administrate) privilegier. Information om hur du hanterar åtkomsten finns i [Hantera prenumerationer och resurser under Azure-prenumerationen](azure-plan-manage.md)

## <a name="next-steps"></a>Nästa steg

- [Kund över gångar till Azure-plan](azure-plan-transition.md)

- [Partner intjänad kredit – översikt](partner-earned-credit.md)
