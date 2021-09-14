---
title: Överföringsberättigande – Riktlinjer för överföring av en prenumeration mellan faktureringskonton, Azure Marketplace
description: Riktlinjer för kommersiella kontroller innan du överför en prenumeration mellan faktureringskonton i Azure Portal.
ms.service: marketplace-customer
ms.topic: conceptual
author: Guyshu
ms.author: gushuchm
ms.date: 11/20/2020
ms.openlocfilehash: 4b235bd462915fc205813ae86e92f98b4fd49fe4
ms.sourcegitcommit: 37eac16c4339cb97831eb2a86d156c45bdf6a531
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/13/2021
ms.locfileid: "126247243"
---
# <a name="transfer-eligibility-for-a-subscription-between-billing-accounts"></a>Överföra behörighet för en prenumeration mellan faktureringskonton

Du kan [överföra en prenumeration](/azure/cost-management-billing/understand/subscription-transfer) från ett faktureringskonto till ett annat i faktureringsavsnittet i Azure Portal. Före en överföring genomsöks prenumerationen efter produkter från tredje part. Överföringen tillåts endast om *alla* produkter har rensats för överföring (se [villkoren](#criteria-for-transfer-approval-or-denial) nedan). Systemet genererar relevanta felmeddelanden för de appar som inte kunde rensas för att hjälpa dig att avgöra nästa steg.

> [!NOTE]
> Den här artikeln gäller inte för SaaS-erbjudanden eftersom SaaS-resurser är kopplade till en klientorganisation, inte en prenumeration. SaaS-resurser kan överföras från ett faktureringskonto till ett annat, men detta görs per resurs och av Azure-supporten som en supportbegäran.

## <a name="criteria-for-transfer-approval-or-denial"></a>Kriterier för överföringsgodkännande eller nekande

Du kan inte överföra en prenumeration om någon av dess appar från tredje part uppfyller något av följande villkor:

- Målkontot är kommersiellt och appen avanmäls från att säljas via partner.
- Appen är anmäld för valda partner och målkontot finns inte med i listan över tillåtna partner.
- Erbjudandet var ett tidigare förhandsversionserbjudande för valda prenumerationer eller var ett privat erbjudande och prenumerationen finns inte längre i listan över tillåtna prenumerationer.
- Det nya faktureringskontot finns i en annan region än där erbjudandet säljs OCH erbjudandet ska inte säljas i den regionen.

En blockerad överföring fortsätter att gälla tills du tar bort resursen från prenumerationen. Därefter kan du försöka överföra igen.

## <a name="next-steps"></a>Nästa steg

[Få support för Microsoft AppSource och Azure Marketplace](get-support.md)

