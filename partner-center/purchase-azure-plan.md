---
title: Köpa en Azure-plan
ms.topic: how-to
ms.date: 07/21/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
description: Med Hjälp av Azure-planen kan du lära dig hur du köper en eller flera Azure-prenumerationer, Azure-reservationer, konfigurerar resurser och visar eller lägger till prenumerationer.
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 1493d22c53915f3a4364981a77c249492b342595
ms.sourcegitcommit: 1161d5bcb345e368348c535a7211f0d353c5a471
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/09/2021
ms.locfileid: "123960023"
---
# <a name="purchase-the-azure-plan-for-customers-and-access-the-latest-azure-services"></a>Köp Azure-planen för kunder och få åtkomst till de senaste Azure-tjänsterna

**Gäller för:** Partnercenter 

**Lämpliga roller:** Globala | Administratörsbehörighet för | Försäljningsagent

När du köper en Azure-plan för dina kunder under Microsoft-kundavtal får du tillgång till den fullständiga katalogen med de senaste Azure-tjänsterna till Betala enligt användning-priser. Molnlösningsleverantör(CSP)-partner kan nu komma åt alla Azure-tjänster när de blir allmänt tillgängliga. En partner kan ha flera Azure-prenumerationer under en Azure-plan. 

## <a name="countryregion-availability"></a>Tillgänglighet för land/region

Den nya handelsupplevelsen i CSP för Azure är schemalagd att vara tillgänglig i 137 länder. Se en fullständig lista över dessa [länder/regioner.](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE3QN0x) 

## <a name="how-to-purchase-azure-plan"></a>Så här köper du en Azure-plan

Hur du köper Azure-planen liknar att köpa andra prenumerationer. Den viktigaste skillnaden är att innan du faktiskt gör din beställning måste du bekräfta att kunden har signerat Microsoft-kundavtal.

1. Välj **Segment kommersiell** och skriv sedan "Microsoft Azure".
2. Under **Azure-plan** väljer du **Lägg till i kundvagn.**

   :::image type="content" source="images/azure/Azurepurchase1.png" alt-text="Köpa.":::

Partnern måste bekräfta att kunden har granskat och godkänt Microsoft-kundavtal villkoren. Mer information om hur partnern kan göra detta finns i Bekräfta [kundens godkännande av Microsoft-kundavtal](./confirm-customer-agreement.md). Andra resurser är tillgängliga i [resursgalleriet](https://partner.microsoft.com/resources/collection/Microsoft-Customer-Agreement-in-the-CSP-program#/).

Bekräfta sedan digitalt eller bjud in kunden att signera Microsoft-kundavtal direkt med Microsoft. 

### <a name="to-invite-the-customer-to-sign-the-agreement-directly"></a>Så här bjuder du in kunden att signera avtalet direkt 

1. På kundens kontosida **väljer** du **Uppdatera bredvid** **Microsoft-kundavtal**.

2. Fyll i informationen om personen på kundens företag som godkände MCuA.

3. Välj **Spara och fortsätt**.  

Som en del av den nya köpupplevelsen för Azure i CSP har vi introducerat ett [nytt Azure-erbjudande](./azure-plan-lp.md). Viktiga datum som rör det tidigare Azure-erbjudandet (MS-AZR-0145p) finns i [det här dokumentet](https://go.microsoft.com/fwlink/p/?linkid=2164140).

**Om du har registrerat dig *före* 21 juli 2021**
- Du kommer att kunna lägga till det tidigare Azure-erbjudandet i kundvagnen för kunder som har köpt det tidigare.
- Om du har registrerat dig  före 21 juli och har kunder som registrerats efter den 21 juli kan du inte lägga till det tidigare Azure-erbjudandet i kundvagnen.

**Partner som registrerats *den 21* juli 2021 eller senare**
- Du kommer inte att kunna lägga till det tidigare Azure-erbjudandet i kundvagnen.

Följande fel uppstår om du försöker lägga till det tidigare Azure-erbjudandet men inte är berättigade på grund av ovanstående affärsprincip. 

:::image type="content" source="images/add-products.png" alt-text="Skärmbild som visar skärmen Lägg till produkter.":::

Information om hur du hittar den nya Azure-planen med Partner Center-API:er finns [i Skapa en Azure-plan.](/partner-center/develop/create-azure-plan#get-the-catalog-item-for-azure-plan)

## <a name="review-and-buy"></a>Granska och köp

Gå tillbaka till **sidan Lägg till** en produkt där du kan se att Azure-planen har lagts till. Välj **Granska** för att granska köpet och välj sedan **Köp.** 

> [!NOTE]
> När du har köpt Azure-planen för en kund kan du inte längre köpa Microsoft Azure (0145p) för den kunden. Du måste skapa framtida prenumerationer via Azure-planen.

## <a name="purchase-azure-reservations-under-the-azure-plan"></a>Köpa Azure-reservationer enligt Azure-planen 
  
Du kan också köpa Microsoft Azure reservationer under Azure-plan åt dina kunder i Partnercenter. (Eller, om du vill, kan du ge dina kunder behörighet att köpa sina egna [Azure-reservationer](give-customers-permission.md) från en tidigare prenumeration som du har köpt för dem.)

1. I menyn i Partnercenter på [instrumentpanelen](https://partner.microsoft.com/dashboard/)väljer du **Kunder.** Hitta den kund som vill köpa Azure-reservationer och välj sedan nedåtpilen för att expandera kundens rad.

2. Välj **Lägg till produkter** och välj sedan **Azure**. 

   - Välj kundens marknadssegment i **listan** Segment.
   - Välj **Reservationer** i **listan Produkttyp.**
   - Välj den typ av reservation som kunden vill ha i **listan Reservationstyp.**

Azure-reservationer måste associeras med en aktiv Azure-plan. Välj den Azure-plan som du vill lägga till Azure-reservationer i från listan Kundprenumeration. 

> [!IMPORTANT] 
> Om kunden inte redan har en aktiv Azure-plan väljer du Azure för att lägga till en nu. Mer information finns i Köpa [Azure-reservationer.](azure-reservations-buying.md#purchase-azure-reservations)

> [!NOTE]
> Omfånget för en reservation kan bara anges till **Delad**, för närvarande i Partnercenter. Om du vill välja ett prenumerationsomfång eller uppdatera från delat till enskilt prenumerationsomfång **går du Microsoft Azure hanteringsportalen med** hjälp av följande anvisningar. 

:::image type="content" source="images/azure/addprods1.png" alt-text="Inställning för reservationer med delat omfång.":::

Så här hanterar du kundens reservation i Azure Portal: 

1. Från **Kunder** väljer du den kund som du vill hantera. 

2. Med nedåtpilen expanderar du kundens rad och väljer Microsoft Azure **Hanteringsportalen.**  
 
## <a name="view-azure-subscriptions-under-the-azure-plan"></a>Visa Azure-prenumerationer under Azure-planen

På sidan **Prenumerationer** går du till avsnittet användningsbaserad och expanderar **Azure-plan för** att se associerade Azure-prenumerationer under Azure-planen.

:::image type="content" source="images/azure/addprods2.png" alt-text="Visa en lista över Azure-prenumerationer."::: 

## <a name="add-subscriptions-and-configure-resources"></a>Lägga till prenumerationer och konfigurera resurser

Du lägger till prenumerationer och konfigurerar resurser för kunden i Azure Portal. Du kan också separera kundens miljö efter arbetsbelastning eller projekt. Det är möjligt att hantera prenumerationer [via Azure Lighthouse](https://azure.microsoft.com/services/azure-lighthouse/) och Azure Portal. 

För att hantera dina kunders resurser och prenumerationer behöver du AOBO-behörighet **(Admin on Behalf Of).** Information om hur du hanterar din åtkomst finns i [Hantera prenumerationer och resurser under Azure-planen](azure-plan-manage.md)

## <a name="next-steps"></a>Nästa steg

- [Kundövergångar till Azure-plan](azure-plan-transition.md)

- [Partner-intjänad kredit – översikt](partner-earned-credit.md)
