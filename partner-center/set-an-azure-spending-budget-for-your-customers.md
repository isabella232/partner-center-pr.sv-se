---
title: Ange en Azure utgifts budget för kunder
ms.topic: how-to
ms.date: 06/03/2020
description: Lär dig hur du ställer in eller tar bort månads utgifter för Azure-utgifter för dina kunder och även för att Visa Azures utgifts data och ange budgetrelaterade aviseringar.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 982d4ed310415349acde3d260afce04eb0d55ac5
ms.sourcegitcommit: 37b0b2a7141907c8d21839de3128fb8a98575886
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2020
ms.locfileid: "92531213"
---
# <a name="set-check-or-remove-monthly-azure-spending-budgets-for-customers-in-partner-center"></a>Ange, kontrol lera eller ta bort månads utgifts budgetar för kunder i Partner Center

Gäller för:

- Partnercenter
- Partner Center för Microsoft Cloud för amerikanska myndigheter

Du kan [ställa in en månatlig Azure utgifts budget för dina kunder](#set-azure-spending-budget) i Partner Center. Detta hjälper kunderna att hantera sina Azure-utgifter. Med det här alternativet kan du jämföra kundernas Azure-utgifter i budgeten under månaden. Det hjälper också kunderna att budgetera sina Azure-utgifter så att deras månatliga faktura inte är högre än förväntat.

> [!NOTE]  
> Den här funktionen är inte tillgänglig i ett begränsat läge eller test i produktions konton (TIP).

När du [har ställt in en Azure utgifts budget för din kund (er)](#set-azure-spending-budget)kan du också granska kund användningen på följande sätt. De här alternativen kan hjälpa dig att hitta felkonfigurerade tjänster eller ovanliga trender som kan föreslå bedrägerier. Sedan kan du arbeta med din kund (er) för att identifiera rotor saken och hantera kostnader. Om det behövs kan du även [ändra kundens budget](#set-azure-spending-budget) till en högre mängd.

- [Kontrol lera aktuella Azure-utgifter](#check-current-azure-spending)

- [Aktivera e-postaviseringar för när en kunds utgifter närmar sig sin budget gräns](#notifications-for-budget-limits)

- [Visa specificerade kostnader per tjänst för användnings prenumerationer](#itemized-costs-by-service)

Du kan också [ta bort en Azure utgifts budget](#remove-azure-spending-budget) för kunder när som helst.

## <a name="azure-spending-data"></a>Azure-utgifts data

Azures utgifts data är en *uppskattning* och de *faktiska fakturerings beloppen kan variera* . Data svärdet *återspeglar inte* skatter, krediter, justeringar eller andra avgifter som kan tillkomma.

Utgifts informationen *uppdateras en gång per dag* . Dina kunder kan fortsätta att använda (och debiteras för) Azure-tjänster och-resurser, om du inte ändrar konto inställningarna i Azure Portal.

## <a name="set-azure-spending-budget"></a>Ställ in Azure utgifts budget

Du kan *ställa in en månatlig Azure utgifts budget* för flera kunder i Partner Center:

1. Logga in på [partner Center-instrumentpanelen](https://partner.microsoft.com/dashboard/).

2. Välj **Azure-utgifter** i den vänstra menyn under **CSP** .

3. På sidan **Azure-utgifter** under **kunder med Microsoft Azure prenumerationer** väljer du de kunder för vilka du vill ställa in en budget.

4. Ange ett värde för **månatlig budget** .

5. Välj **Verkställ** för att spara ändringarna.

Du kan också *Ange en budget för en enskild kund* i prenumerations inställningarna:

1. Logga in på Partner Center-instrumentpanelen.

2. Välj **kunder** i den vänstra menyn under **CSP** .

3. På sidan **kunder** väljer du kundens **företags namn** .

4. På sidan kund **prenumerationer** , under **användnings-baserad prenumeration** , väljer du **ändra budget** .

5. Ange ett värde för budgeten.

6. Välj **Verkställ** för att spara ändringarna.

## <a name="remove-azure-spending-budget"></a>Ta bort utgifts budget för Azure

Du kan *ta bort en månatlig Azure utgifts budget* för din kund (er) i Partner Center:

1. Logga in på [partner Center-instrumentpanelen](https://partner.microsoft.com/dashboard/).

2. Välj **Azure-utgifter** i den vänstra menyn under **CSP** .

3. På sidan **Azure-utgifter** under **kunder med Microsoft Azure prenumerationer** väljer du den eller de kunder vars budget du vill ta bort.

4. Välj **ta bort budget** .

## <a name="check-current-azure-spending"></a>Kontrol lera aktuella Azure-utgifter

Du kan när som helst *spåra kundernas aktuella Azure-utgifter och månads budgetar* :

1. Logga in på [partner Center-instrumentpanelen](https://partner.microsoft.com/dashboard/).

2. Välj **Azure-utgifter** i den vänstra menyn under **CSP** .

3. På sidan **Azure-utgifter** under **kunder med Microsoft Azure prenumerationer** kan du se en översikt över kunders månads budgetar, aktuella utgifts uppskattningar och procent andel av budgeten som används.

## <a name="notifications-for-budget-limits"></a>Meddelanden för budget gränser

Du kan *Aktivera e-postaviseringar* för när kundens månads utgifter närmar sig budget gränsen. När du aktiverar det här alternativet får du ett meddelande när kunderna använder 80% eller mer av sin månads budget. Det här alternativet hjälper dig att hålla ett öga på din Azure-faktura. Så här konfigurerar du e-postmeddelanden:

1. Logga in på Partner Center.

2. Välj **Azure-utgifter** i den vänstra menyn under **CSP** .

3. På sidan **Azure-utgifter** , under **e-postaviseringar** , kan du växla inställningen **Hämta e-post** till **på** .

4. Välj **ändra e-postadress** för att se e-postadressen för meddelanden.

5. Om e-postadressen *inte är korrekt* anger du rätt e-postadress och väljer **Uppdatera** . Om e-postadressen *är korrekt* väljer du **Avbryt** .

## <a name="itemized-costs-by-service"></a>Specificerade kostnader per tjänst

Du kan *Visa de specificerade kostnaderna (och den uppskattade användningen) efter tjänst för användnings-baserade prenumerationer* :

1. Logga in på Partner Center.

2. Välj **kunder** i den vänstra menyn under **CSP** .

3. På sidan **kunder** väljer du kundens **företags namn** .

4. På sidan kund **prenumerationer** under **användnings prenumerationer** väljer du namnet på **prenumerationen** .

5. På prenumerationens sida kan du granska de **specificerade kostnaderna** per tjänst och den **beräknade användningen** för den aktuella månaden.
