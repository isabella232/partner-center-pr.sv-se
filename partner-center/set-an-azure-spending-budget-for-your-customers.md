---
title: Ange en Azure-utgiftsbudget för kunder
ms.topic: how-to
ms.date: 09/27/2021
description: Lär dig hur du ställer in eller tar bort månatliga Azure-utgiftsbudgetar för dina kunder och hur du visar azure-utgiftsdata och anger budgetrelaterade meddelanden.
ms.service: partner-dashboard
ms.subservice: partnercenter-billing
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: add447f6d9b0332bea9bbddd0ccf66efc5e146fd
ms.sourcegitcommit: e1da62b36420d78bf44e3962358d0af65ebc3402
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/27/2021
ms.locfileid: "129088781"
---
# <a name="set-check-or-remove-monthly-azure-spending-budgets-for-customers-in-partner-center"></a>Ange, kontrollera eller ta bort månatliga Azure-utgiftsbudgetar för kunder i Partnercenter

**Lämpliga roller:** Administratörsagent

Du kan ange en [månatlig Azure-utgiftsbudget](#set-azure-spending-budget) för dina kunder i Partnercenter. Detta hjälper dina kunder att hantera sina Azure-utgifter. Med det här alternativet kan du jämföra dina kunders Azure-utgifter med budgeten under månaden. Det hjälper även dina kunder att budgetera sina Azure-utgifter så att deras månadsfaktura inte blir högre än förväntat.

> [!NOTE]  
> Den här funktionen är inte tillgänglig i sandbox- eller Test in Production-konton (TIPS).

När du har angett en Azure-utgiftsbudget för kunden kan du även granska kundanvändningen. De här alternativen kan hjälpa dig att upptäcka felkonfigurerade tjänster eller ovanliga trender som kan tyda på bedrägerier. Du kan sedan arbeta med dina kunder för att identifiera rotorsaken och hantera kostnader. Om det behövs kan du också ändra kundens budget till ett högre belopp.

## <a name="azure-spending-data"></a>Utgiftsdata i Azure

Azure-utgiftsdata är en *uppskattning och* de *faktiska faktureringsbeloppen kan variera*. Datavärdet *återspeglar inte skatter,* krediter, justeringar eller andra avgifter som kan tillkomma.

Utgiftsdata uppdateras *en gång per dag.* Dina kunder kan fortsätta att använda (och debiteras för) Azure-tjänster och -resurser, såvida du inte ändrar deras kontoinställningar i Azure Portal.

## <a name="set-azure-spending-budget"></a>Ange utgiftsbudget för Azure

> [!NOTE]
> Mer information om gränssnittet för arbetsytor finns i [Getting around Partner Center (Ta sig runt i Partnercenter).](get-around-partner-center.md#turn-workspaces-on-and-off)

#### <a name="workspaces-view"></a>[Vyn Arbetsytor](#tab/workspaces-view)

Du kan *ange en månatlig Azure-utgiftsbudget* för flera kunder i Partnercenter:

1. Logga in på [instrumentpanelen i Partnercenter](https://partner.microsoft.com/dashboard/).

2. Välj panelen **Fakturering** och välj sedan **Azure-utgifter.**

3. På **sidan Azure-utgifter** går **du till Microsoft Azure prenumerationer** och väljer de kunder som du vill ange en budget för.

4. Ange ett värde för **Månadsbudget**.

5. Spara **ändringarna genom** att välja Tillämpa.

Du kan *ange en budget för en enskild kund i* prenumerationsinställningarna.

1. Logga in på [instrumentpanelen i Partnercenter](https://partner.microsoft.com/dashboard/).

2. Välj **panelen** Kunder.

3. På **sidan** Kunder väljer du kundens **företagsnamn**.

4. På kundens **prenumerationssida går** du till **Användningsbaserad prenumeration och** väljer Ändra **budget.**

5. Ange ett värde för budgeten.

6. Spara **ändringarna genom** att välja Tillämpa.

Du kan *ta bort en månatlig Azure-utgiftsbudget* för dina kunder i Partnercenter.

1. Logga in på [instrumentpanelen i Partnercenter](https://partner.microsoft.com/dashboard/).

2. Välj panelen **Fakturering** och välj sedan **Azure-utgifter.**

3. På sidan **Azure-utgifter** går **du till Microsoft Azure prenumerationer** och väljer de kunder vars budget du vill ta bort.

4. Välj **Ta bort budget.**

Du kan *spåra dina kunders aktuella Azure-utgifter och månatliga budgetar* när som helst.

1. Logga in på [instrumentpanelen i Partnercenter](https://partner.microsoft.com/dashboard/).

2. Välj panelen **Fakturering** och välj sedan **Azure-utgifter.**

3. På **sidan Azure-utgifter** under **Kunder med Microsoft Azure prenumerationer** kan du se en översikt över kundernas månatliga budgetar, aktuella utgiftsuppskattningar och procentandelen budget som används.

#### <a name="current-view"></a>[Aktuell vy](#tab/current-view)

Du kan *ange en månatlig Azure-utgiftsbudget* för flera kunder:

1. Logga in på [instrumentpanelen i Partnercenter](https://partner.microsoft.com/dashboard/).

2. I den vänstra menyn under **CSP väljer** du **Azure-utgifter.**

3. På **sidan Azure-utgifter** går **du till Microsoft Azure prenumerationer** och väljer de kunder som du vill ange en budget för.

4. Ange ett värde för **Månadsbudget**.

5. Spara **ändringarna genom** att välja Tillämpa.

Du kan *ange en budget för en enskild kund i* prenumerationsinställningarna.

1. Logga in på [instrumentpanelen i Partnercenter](https://partner.microsoft.com/dashboard/).

2. I den vänstra menyn under **CSP väljer** du **Kunder**.

3. På **sidan** Kunder väljer du kundens **företagsnamn**.

4. På kundens **prenumerationssida går** du till **Användningsbaserad prenumeration och** väljer Ändra **budget.**

5. Ange ett värde för budgeten.

6. Spara **ändringarna genom** att välja Tillämpa.

**Ta bort azure-utgiftsbudget**

Du kan *ta bort en månatlig Azure-utgiftsbudget* för dina kunder i Partnercenter:

1. Logga in på [instrumentpanelen i Partnercenter](https://partner.microsoft.com/dashboard/).

2. I den vänstra menyn under **CSP väljer** du **Azure-utgifter.**

3. På sidan **Azure-utgifter** går **du till Microsoft Azure prenumerationer** och väljer de kunder vars budget du vill ta bort.

4. Välj **Ta bort budget.**

* * *

## <a name="notifications-for-budget-limits"></a>Meddelanden om budgetgränser

Du kan *aktivera e-postaviseringar* när kundens månatliga utgifter närmar sig sin budgetgräns. När du aktiverar det här alternativet får du ett meddelande när kunderna använder 80 % eller mer av sin månadsbudget. Det här alternativet hjälper dig att hålla ett öga på Din Azure-faktura. Så här konfigurerar du e-postaviseringar:

1. Logga in på Partner Center.

2. Välj kugghjulsikonen Inställningar och välj sedan **Mina inställningar.**

3. Konfigurera en önskad e-postadress om du inte har gjort det.

4. Konfigurera det föredragna språket för meddelandet.

5. Välj **fliken CSP** under **avsnittet Meddelandeinställningar.**

6. Markera alternativet E-post för Azure Spending notification **(Azure-utgiftsavisering)** och **Spara**.

## <a name="itemized-costs-by-service"></a>Specificerade kostnader per tjänst

Du kan visa specificerade kostnader (och beräknad användning) per tjänst för användningsbaserade prenumerationer*:

> [!NOTE]
> Mer information om gränssnittet för arbetsytor finns i [Getting around Partner Center (Ta sig runt i Partnercenter).](get-around-partner-center.md#turn-workspaces-on-and-off)

#### <a name="workspaces-view"></a>[Vyn Arbetsytor](#tab/workspaces-view)

1. Logga in på [instrumentpanelen i Partnercenter](https://partner.microsoft.com/dashboard).

2. Välj **panelen** Kunder.

3. Välj kundens **företagsnamn**.

4. På kundens **prenumerationssida** går du till **Användningsbaserade prenumerationer** och väljer namnet på **prenumerationen**.

5. På prenumerationens sida kan du granska De beräknade **kostnaderna** per tjänst och **Beräknad användning för** den aktuella månaden.

#### <a name="current-view"></a>[Aktuell vy](#tab/current-view)

1. Logga in på [instrumentpanelen i Partnercenter](https://partner.microsoft.com/dashboard).

2. I den vänstra menyn under **CSP väljer** du **Kunder**.

3. På **sidan** Kunder väljer du kundens **företagsnamn**.

4. På kundens **prenumerationssida** går du till **Användningsbaserade prenumerationer** och väljer namnet på **prenumerationen**.

5. På prenumerationens sida kan du granska De beräknade **kostnaderna** per tjänst och **Beräknad användning för** den aktuella månaden.

* * *

## <a name="next-steps"></a>Nästa steg

- [Ny handelsupplevelse i CSP – Azure-fakturering](azure-plan-billing.md)
