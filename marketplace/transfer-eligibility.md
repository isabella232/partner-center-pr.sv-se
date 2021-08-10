---
title: Överföringsberättigande – Riktlinjer för överföring av en prenumeration mellan faktureringskonton, Azure Marketplace
description: Riktlinjer för kommersiella kontroller innan du överför en prenumeration mellan faktureringskonton i Azure Portal.
ms.service: marketplace-customer
ms.topic: conceptual
author: Guyshu
ms.author: gushuchm
ms.date: 11/20/2020
ms.openlocfilehash: 22c53238fd74501f32a56d66f15133cbbe8765cffe67a04c4f66779c15b16c37
ms.sourcegitcommit: 121f1b9cbd88faeba60dc9b475f9c0647cdc933c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/06/2021
ms.locfileid: "115688325"
---
# <a name="transfer-eligibility-for-a-subscription-between-billing-accounts"></a>Överföra behörighet för en prenumeration mellan faktureringskonton

Du kan [överföra en prenumeration](/azure/cost-management-billing/understand/subscription-transfer) från ett faktureringskonto till ett annat i faktureringsavsnittet i Azure Portal. Innan en överföring genomsöks prenumerationen efter produkter från tredje part. Överföringen tillåts endast om *alla* produkter har rensats för överföring (se [villkoren](#criteria-for-transfer-approval-or-denial) nedan). Systemet genererar relevanta felmeddelanden för de appar som inte kunde rensas för att hjälpa dig att avgöra nästa steg.

> [!NOTE]
> Den här artikeln gäller inte för SaaS-erbjudanden eftersom SaaS-resurser är kopplade till en klientorganisation, inte en prenumeration. SaaS-resurser kan överföras från ett faktureringskonto till ett annat, men detta görs per resurs och av Azure-supporten som en supportbegäran.

## <a name="criteria-for-transfer-approval-or-denial"></a>Kriterier för godkännande eller nekande av överföring

Du kan inte överföra en prenumeration om någon av dess appar från tredje part uppfyller något av följande villkor:

- Målkontot är kommersiellt och appen avanmäls från att säljas via partner.
- Appen väljer valda partner och målkontot finns inte med i listan över tillåtna partner.
- Erbjudandet var ett tidigare förhandsversionserbjudande för valda prenumerationer eller var ett privat erbjudande och prenumerationen finns inte längre i listan över tillåtna.
- Det nya faktureringskontot finns i en annan region än där erbjudandet säljs och erbjudandet ska inte säljas i den regionen.

En blockerad överföring fortsätter att gälla tills du tar bort resursen från prenumerationen. Därefter kan du försöka med överföringen igen.

## <a name="next-steps"></a>Nästa steg

[Få support för Microsoft AppSource och Azure Marketplace](get-support.md)

