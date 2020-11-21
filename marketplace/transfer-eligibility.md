---
title: Överförings berättigande – rikt linjer för överföring av en prenumeration mellan fakturerings konton, Azure Marketplace
description: Rikt linjer för kommersiella kontroller innan du överför en prenumeration mellan fakturerings konton i Azure Portal.
ms.prod: marketplace-customer
ms.topic: conceptual
author: Guyshu
ms.author: gushuchm
ms.date: 11/20/2020
ms.openlocfilehash: a6a3c8954643ea982ae5107ae417a900ed51e77d
ms.sourcegitcommit: 1aa43438ad181278052788f15e017f9ae7777943
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 11/21/2020
ms.locfileid: "95007601"
---
# <a name="transfer-eligibility-for-a-subscription-between-billing-accounts"></a>Överför berättigande för en prenumeration mellan fakturerings konton

Du kan [överföra en prenumeration](/azure/cost-management-billing/understand/subscription-transfer) från ett fakturerings konto till ett annat i fakturerings avsnittet i Azure Portal. Före en överföring genomsöks prenumerationen efter produkter från tredje part. Överföringen tillåts bara om *alla* produkter har rensats för överföring (se [kriterierna](#criteria-for-transfer-approval-or-denial) nedan). Systemet genererar relevanta fel meddelanden för de appar som inte kunde rensas för att hjälpa dig att fastställa nästa steg.

> [!NOTE]
> Den här artikeln gäller inte för SaaS-erbjudanden eftersom SaaS-resurser är kopplade till en klient, inte en prenumeration. SaaS-resurser kan överföras från ett fakturerings konto till ett annat, men detta görs per resurs och av Azure-support som en support förfrågan.

## <a name="criteria-for-transfer-approval-or-denial"></a>Villkor för godkännande eller avslag av överföring

Du kan inte överföra en prenumeration om någon av dess appar från tredje part uppfyller något av följande kriterier:

- Mål kontot är kommersiellt och appen är inte valbar för att säljas via partner.
- Appen är valbar för utvalda partner och mål kontot finns inte i listan över tillåtna.
- Erbjudandet var ett för hands erbjudande tidigare för valda prenumerationer eller var ett privat erbjudande och prenumerationen är inte längre i listan över tillåtna.
- Det nya fakturerings kontot finns i en annan region än där erbjudandet säljs och erbjudandet är inte att säljas i den regionen.

En blockerad överföring fortsätter att gälla tills du tar bort resursen från prenumerationen. därefter kan du prova överföringen igen.

## <a name="next-steps"></a>Nästa steg

[Få support för Microsoft AppSource och Azure Marketplace](get-support.md)

