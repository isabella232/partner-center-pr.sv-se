---
title: Köpa en Azure-plan
ms.topic: how-to
ms.date: 06/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Med Azure-planen kan du lära dig hur du köper en eller flera Azure-prenumerationer, Azure-reservationer, konfigurerar resurser och visar eller lägger till prenumerationer.
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 24eba2969552b0403de9828e86d4fc73abfec585
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/17/2021
ms.locfileid: "112276271"
---
# <a name="purchase-the-azure-plan-for-customers--access-the-latest-azure-services-at-pay-as-you-go-rates"></a>Köp Azure-planen för kunder & få åtkomst till de senaste Azure-tjänsterna till Betala enligt användning-priser

**Lämpliga roller:** Globala | Administratörsbehörighet för | Försäljningsagent

När du köper en Azure-plan för dina kunder under Microsoft-kundavtal får du tillgång till den fullständiga katalogen med de senaste Azure-tjänsterna till Betala enligt användning-priser. CSP-partner kommer nu att kunna komma åt alla Azure-tjänster när de blir allmänt tillgängliga. En partner kan ha flera Azure-prenumerationer under en Azure-plan. 

## <a name="countryregion-availability"></a>Tillgänglighet för land/region

Den nya handelsupplevelsen i CSP för Azure är schemalagd att vara tillgänglig i 139 länder. Se en fullständig lista över dessa [länder/regioner.](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE3QN0x) 

## <a name="how-to-purchase-azure-plan"></a>Så här köper du en Azure-plan

Hur du köper Azure-planen liknar att köpa andra prenumerationer. Den viktigaste skillnaden är att innan du faktiskt gör din beställning måste du bekräfta att kunden har signerat Microsoft-kundavtal.

1. Välj **Segment kommersiell** och skriv **Microsoft Azure** 
2. Under Azure-plan väljer du **Lägg till i kundvagn**

:::image type="content" source="images/azure/Azurepurchase1.png" alt-text="Köpa.":::

Partnern måste bekräfta att kunden har granskat och godkänt Microsoft-kundavtal villkor. Mer information om hur partnern kan göra detta finns i Bekräfta [kundens godkännande av Microsoft-kundavtal](confirm-customer-agreement.md). Andra resurser är tillgängliga i [resursgalleriet](https://partner.microsoft.com/resources/collection/Microsoft-Customer-Agreement-in-the-CSP-program#/).

**Bekräfta genom att antingen**: 

1. Bekräfta digitalt eller

2. Bjud in kunden att signera Microsoft-kundavtal direkt med Microsoft. 

### <a name="to-confirm"></a>Bekräfta 

1. På kundens **kontosida väljer** du **Uppdatera** bredvid **Microsoft-kundavtal**  

2. Fyll i informationen om personen på kundens företag som godkände MCuA.

3. Välj **Spara och fortsätt.**  

## <a name="review-and-buy"></a>Granska och köp

Du kommer tillbaka till **sidan Lägg till** en produkt där du kan se att Azure-planen har lagts till. Välj **Granska** för att granska köpet och välj sedan **Köp.** 

>[!Note]
>När du har köpt Azure-planen för en kund kan du inte längre köpa Microsoft Azure (0145p) för den kunden. Du måste skapa framtida prenumerationer via Azure-planen.

## <a name="purchase-azure-reservations-under-the-azure-plan"></a>Köpa Azure-reservationer enligt Azure-planen 
  
Du kan också köpa Microsoft Azure under Azure-plan åt dina kunder i Partnercenter. (Eller, om du vill, kan du ge dina kunder behörighet att köpa sina egna [Azure-reservationer](give-customers-permission.md) från en tidigare prenumeration som du har köpt för dem.)

1. I menyn i Partnercenter på [instrumentpanelen](https://partner.microsoft.com/dashboard/)väljer du **Kunder.** Hitta den kund som vill köpa Azure-reservationer och välj sedan nedåtpilen för att expandera kundens rad.

2. Välj **Lägg till produkter** och välj sedan **Azure**. 

   - Välj kundens marknadssegment i **listan** Segment.
   - Välj **Reservationer** i **listan Produkttyp.**
   - Välj den typ av reservation som kunden vill ha i **listan Reservationstyp.**

Azure-reservationer måste associeras med en aktiv Azure-plan. Välj den Azure-plan som du vill lägga till Azure-reservationer i från listan Kundprenumeration. 

>[!Important] 
>Om kunden inte redan har en aktiv Azure-plan väljer du Azure för att lägga till en nu. Mer information finns i Köpa [Azure-reservationer.](azure-reservations-buying.md#purchase-azure-reservations)

>[!Note]
>Omfånget för en reservation kan bara anges till **Delad**, för närvarande i Partnercenter. Om du vill välja ett enskilt prenumerationsomfång eller uppdatera från delat till enskilt prenumerationsomfång **går du Microsoft Azure hanteringsportalen med** hjälp av följande anvisningar. 

:::image type="content" source="images/azure/addprods1.png" alt-text="Inställning för reservationer med delat omfång.":::

Så här hanterar du kundens reservation i Azure Portal: 

1. Från **Kunder** väljer du den kund som du vill hantera. 

2. Med nedåtpilen expanderar du kundens rad och väljer Microsoft Azure **Hanteringsportalen.**  
 
## <a name="view-azure-subscriptions-under-the-azure-plan"></a>Visa Azure-prenumerationer under Azure-planen

På sidan **Prenumerationer** går du till avsnittet användningsbaserad och expanderar **Azure-plan för** att se associerade Azure-prenumerationer under Azure-planen.

:::image type="content" source="images/azure/addprods2.png" alt-text="Visa en lista över Azure-prenumerationer."::: 


## <a name="add-subscriptions-and-configure-resources"></a>Lägga till prenumerationer och konfigurera resurser

Du lägger till prenumerationer och konfigurerar resurser för din kund i Azure Portal. Du kan också separera kundens miljö efter arbetsbelastning eller projekt. Det är möjligt att hantera prenumerationer [Azure Lighthouse](https://azure.microsoft.com/services/azure-lighthouse/) och Azure Portal. 

För att hantera dina kunders resurser och prenumerationer behöver du AOBO-behörighet **(Admin on Behalf Of).** Information om hur du hanterar din åtkomst finns i [Hantera prenumerationer och resurser under Azure-planen](azure-plan-manage.md)

## <a name="next-steps"></a>Nästa steg

- [Kundövergångar till Azure-plan](azure-plan-transition.md)

- [Partner-intjänad kredit – översikt](partner-earned-credit.md)
