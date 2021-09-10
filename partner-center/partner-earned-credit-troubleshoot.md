---
title: Felsöka partner-intjänad kredit
ms.topic: article
ms.date: 07/22/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
description: Lär dig hur du kan lösa fakturaproblem och andra problem med partner-intjänad kredit (PEC).
author: adamyeh
ms.author: adamyeh
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 7ce31bd688c32da956f466d63beede3f0fc9f9ef
ms.sourcegitcommit: 1161d5bcb345e368348c535a7211f0d353c5a471
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/09/2021
ms.locfileid: "123961496"
---
# <a name="troubleshooting-partner-earned-credit"></a>Felsöka partner-intjänad kredit

**Lämpliga roller:** Globala | Administratörsbehörighet för användarhantering | Administratörsagentens | Faktureringsadministratörskonto | Försäljningsagent

## <a name="troubleshooting-guide"></a>Felsökningsguide

Om du har problem med PEC, till exempel åtkomst eller information som saknas, kontrollerar du objekten nedan i den ordning som anges.

1. Kontrollera att du tittar på fakturan för G (modern) och rekognoseringsfilen. Azure Plan och PEC visas inte på fakturan för D (äldre) eller rekognoseringsfilen.

2. Identifiera typen av partner. (Indirekta återförsäljare är inte berättigade.)

3. Bekräfta att DITT MPN-avtal är aktivt.

4. För indirekta leverantörer kontrollerar du att återförsäljarens MPN-ID som anges i Partnercenter (eller via API) matchar återförsäljarens MPN-ID som anges i Azure Portal.

5. Bekräfta att ditt erbjudande är berättigat. (Gamla Azure-erbjudanden, Azure Reserved Instances och produkter från tredje part är inte berättigade.)

6. Bekräfta att du har en giltig roll för administration på uppdrag av (AOBO) eller Role-Based Access Control (RBAC) för prenumerationen/resursgruppen/resursen.

7. Ta reda på om kunden har tagit bort din RBAC-roll. I så fall kan du se Återställa administratörsbehörighet för en kunds Azure CSP prenumerationer

8. Bekräfta att du har administratörsåtkomst för hela dagen.

9. Bekräfta att du granskar rätt kolumner i filen för daglig användning.

## <a name="next-steps"></a>Nästa steg

- [Prislista för den nya handelsupplevelsen för Azure i CSP](azure-plan-price-list.md)
- [Hantera prenumerationer och resurser under Azure-planen](azure-plan-manage.md)
- [Ny handelsupplevelse i CSP – Azure-fakturering](azure-plan-billing.md)
- [Återställ administratörsbehörigheter för Azure CSP-prenumerationer](revoke-reinstate-csp.md)
- [Partner-intjänad kredit – översikt](partner-earned-credit.md)
- [Roller, behörigheter för partner-intjänad kredit](azure-roles-perms-pec.md)
- [Förstå partners intjänade kredit (guide)](https://partner.microsoft.com/resources/detail/understanding-partner-earned-credit-pdf) (inloggning krävs)
