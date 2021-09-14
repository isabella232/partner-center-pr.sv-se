---
title: Vanliga frågor och svar om partners intjänade kredit
ms.topic: article
ms.date: 08/13/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
description: Få svar på vanliga frågor om partners intjänade kredit (PEC).
author: adamyeh
ms.author: adamyeh
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: ae78b13ae17b223e1cb540bea50168d02bcb9a1c
ms.sourcegitcommit: 37eac16c4339cb97831eb2a86d156c45bdf6a531
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/13/2021
ms.locfileid: "126246775"
---
# <a name="frequently-asked-questions-for-partner-earned-credit"></a>Vanliga frågor och svar om partner-intjänad kredit

Lämpliga roller: Globala | Administratörsbehörighet för användarhantering | Administratörsagentens | Faktureringsadministratörskonto | Försäljningsagent

Nedan visas en lista med vanliga frågor om partner-intjänad kredit.

## <a name="how-much-is-pec"></a>Hur mycket är PEC?

Hur mycket partner tjänar för PEC varierar (se [Beräkning).](partner-earned-credit-explanation.md#calculation) Priset finns på sidan med prislistor i Partnercenter.

## <a name="what-azure-services-are-eligible-for-pec"></a>Vilka Azure-tjänster är berättigade till PEC?

PEC är berättigat till alla tjänster relaterade till det nya Azure-erbjudandet i CSP (Azure-plan) förutom följande: 
- Nya Azure-erbjudandereservationer (Azure-plan)
- Produkter från tredje part som identifierats som tredje part i kolumnen Taggar i listan med förbrukningspris för Azure-plan
- Produkter i Marketplace-prislistan
- [Azure Spot Virtual Machines](https://partner.microsoft.com/resources/collection/azure-spot-in-csp#/)

## <a name="where-can-i-see-pec"></a>Var kan jag se PEC?

Se [Beräkning.](partner-earned-credit-explanation.md#calculation)

## <a name="where-can-i-find-pec-details"></a>Var hittar jag PEC-information?

PEC-information kan efterfrågas av API, [daglig rekognoseringsfil](partner-earned-credit-explanation.md#calculation) [och ACM (Azure Cost Mgmt)](partner-earned-credit-explanation.md#azure-cost-management-and-pec) av partner direkt.

## <a name="how-can-i-reconcile-my-pec-information-across-the-two-recon-files"></a>Hur kan jag stämma av min PEC-information mellan de två rekognoseringsfilerna?

Det finns två avstämningsfiler i Partnercenter under Fakturering som kan användas.

- Daglig beräknad aktivitet för avstämning av användning (.csv)
- Avstämningsaktivitet (.csv)

För att stämma av kan partnern jämföra fälten ProductID, SKUID och AvailabilityID från dessa två filer för varje SubscriptionID.

:::image type="content" source="images/advanced-specializations/partner-billing.png" alt-text="Skärmbild av fliken Fakturering i Partnercenter med återkommande köp och engångsköp." border="false":::

## <a name="for-an-indirect-reseller-working-with-an-indirect-provider-does-an-indirect-provider-need-to-add-the-indirect-resellers-account-as-an-rbac-identity-and-access-management-iam-role-to-the-end-customers-subscription-in-order-to-utilize-acm"></a>För en indirekt återförsäljare som arbetar med en indirekt leverantör, behöver en indirekt leverantör lägga till den indirekta återförsäljarens konto som en RBAC-roll för identitets- och åtkomsthantering (IAM) i slutanvändarens prenumeration för att kunna använda ACM?

Ja, CSP Indirect Provider aktivera [RBAC-åtkomst](/azure/role-based-access-control/overview) till den indirekta återförsäljaren i Azure-prenumerationen.

## <a name="what-happens-if-a-customer-removes-a-partners-rbac-admin-access"></a>Vad händer om en kund tar bort en partners RBAC-administratörsåtkomst?

En partner utan lämplig RBAC-åtkomst i CSP behåller fortfarande kundens Azure-faktureringsrelation och ansvar med Microsoft. Detta påverkar inte en partner som säljer det tidigare Azure-erbjudandet i CSP, men för det nya Azure-erbjudandet i CSP är den fakturerade partnern inte berättigad till PEC på sin Azure-faktura. Partner kan uppnå partiell administratörsåtkomst i CSP genom att få åtkomst via ett användarkonto via katalog-/gäståtkomst med hjälp av RBAC eller via Azure Lighthouse. Mer information finns i [Återställa administratörsbehörigheter för en kunds Azure CSP prenumerationer.](revoke-reinstate-csp.md)

:::image type="content" source="images/advanced-specializations/permissions.png" alt-text="Skärmbild av sidan Åtkomstkontroll där du kan återställa administratörsbehörigheter." border="false":::

## <a name="how-do-i-know-if-im-earning-pec"></a>Hur gör jag för att vet du om jag tjänar PEC?

Det finns flera sätt som en partner kan bekräfta att de har rätt åtkomst till en kunds Azure-resurser.

- Granska filen för daglig användning: Om en partner tar emot partnerns intjänade kredit för hanterade tjänster har de administratörsåtkomst. Detta kan fastställas genom att granska enhetspriset och det effektiva enhetspriset i filen för daglig användning och bekräfta om en rabatt tillämpas.
- Skapa en Azure Monitor-avisering: [](/azure/azure-monitor/platform/alerts-activity-log) Du kan skapa aktivitetsloggaviseringar med hjälp Azure Monitor att ta emot meddelanden när din RBAC-åtkomst tas bort från CSP-prenumerationer. Se guiden Om partners intjänade kredit och teknisk dokumentation.

## <a name="why-dont-i-see-pec-on-the-invoice"></a>Varför visas inte PEC på fakturan?

PEC anges inte explicit på fakturan och det finns inget separat radobjekt för att visa PEC, men PEC-intäkter räknas in i det justerade nettodelade avgiftsbeloppet på fakturan. Visa beräkningsavsnitten och How is PEC paid sections (Hur är PEC-betalavsnitt) om du vill veta mer om var du kan visa PEC-information.

## <a name="next-steps"></a>Nästa steg

- [Prislista för den nya handelsupplevelsen för Azure i CSP](azure-plan-price-list.md)
- [Hantera prenumerationer och resurser under Azure-planen](azure-plan-manage.md)
- [Ny handelsupplevelse i CSP – Azure-fakturering](azure-plan-billing.md)
- [Återställ administratörsbehörigheter för Azure CSP-prenumerationer](revoke-reinstate-csp.md)
- [Partner-intjänad kredit – översikt](partner-earned-credit.md)
- [Roller, behörigheter för partner-intjänad kredit](azure-roles-perms-pec.md)
- [Förstå partners intjänade kredit (guide)](https://partner.microsoft.com/resources/detail/understanding-partner-earned-credit-pdf) (inloggning krävs)
