---
title: Partner-intjänad kredit för hanterade tjänster
ms.topic: article
ms.date: 08/12/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
description: Lär dig hur Microsoft-partners intjänade kredit (PEC) för hanterade tjänster beräknas och betalas och hur du säkerställer att du är berättigad.
author: adamyeh
ms.author: adamyeh
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 56884a5a6cbfbade881154275129c63dcd3456d8
ms.sourcegitcommit: eeb81ccb888239a0e8fbe4711de3ce07f3b00358
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/23/2021
ms.locfileid: "128312120"
---
# <a name="how-the-partner-earned-credit-is-calculated-and-paid"></a>Hur partnerintjänad kredit beräknas och betalas

**Lämpliga roller:** Globala | Administratörsbehörighet för | Administratörsagentens | Faktureringsadministratörskonto | Försäljningsagent

Partner intjänad kredit (PEC) för hanterade tjänster identifierar och delar ut förmåner till partner som äger IT-driftkontroll och hantering av en eller flera kunders Azure-miljöer. 

Som CSP-partner beviljas du som standard nödvändiga åtkomsträttigheter till kundens prenumeration, så att du kan utföra drifthantering och kontroll över resurserna i prenumerationen. Andra sätt på vilka kunder kan etablera åtkomst för att köpa partners beskrivs i följande avsnitt.

Det månatliga fakturabeloppet är netto för partnerns intjänade kredit. Du kan se PEC-information i din månatliga rekognoseringsfil. Mer information om hur en kund kan etablera åtkomst för den transacting-partnern finns i följande artiklar:

- [Hantera prenumerationer och resurser under Azure-planen](azure-plan-manage.md)
- [Återställ administratörsbehörigheter för Azure CSP-prenumerationer](revoke-reinstate-csp.md)

## <a name="eligibility"></a>Stödberättigande

För att få partner intjänad kredit (PEC) gäller följande krav:

- Du måste ha ett aktivt MPN-avtal och en giltig [rollbaserad åtkomstkontrollroll](azure-roles-perms-pec.md) [(RBAC).](/azure/role-based-access-control/overview)
- Du måste ha [AOBO-behörighet (Admin on Behalf of)](https://channel9.msdn.com/Series/cspdev/Module-11-Admin-On-Behalf-Of-AOBO) för kundens Azure-prenumeration, Azure-resursgrupp eller Azure-resurs eller en giltig [RBAC-roll.](azure-roles-perms-pec.md)
- När det gäller indirekta leverantörer och deras indirekta återförsäljare är en indirekt leverantör berättigad till PEC om antingen den indirekta leverantören eller den indirekta återförsäljaren eller båda har AOBO-privilegier eller en berättigad RBAC-roll. Mer information finns i Återställa [administratörsbehörigheter för Azure CSP prenumerationer.](revoke-reinstate-csp.md)
- Partnerns MPN-ID måste tillhöra samma v-organisation som inköparens MPN-ID eller MPN-ID:t för partner för post (MPN). Mer information finns i [Länka ditt partner-ID för att se hur du påverkar delegerade resurser](/azure/lighthouse/how-to/partner-earned-credit).
- PEC intjänas på Azure-resursnivå, resursgrupp eller prenumeration. Om en partner har giltig åtkomst på prenumerations- eller resursgruppsnivå får varje resurs som ingår i den högre entiteten PEC.
- PEC gäller inte för följande tjänster:
    - Reservationer för Azure-plan
    - Produkter från tredje part som identifieras som tredje part i kolumnen Taggar i Azure-planens förbrukningspris
    - Produkter i Marketplace-prislistan
    - [Azure Spot Virtual Machines](https://partner.microsoft.com/resources/collection/azure-spot-in-csp#/)

Utöver kraven ovan gäller PEC endast för tjänster som anges i prissättningen för Azure-planförbrukning. Du kan visa och exportera detta från [prissättningssidan för Azure-planen.](https://partner.microsoft.com/commerce/sales)

Mer information om PEC finns på sidan [om Azure Cost Management.](/azure/cost-management-billing/costs/get-started-partners)

Mer information om berättigande finns i Roller [och behörigheter som krävs för att få partnertjänad kredit.](azure-roles-perms-pec.md)

## <a name="calculation"></a>Beräkning

PEC beräknas dagligen. Du betalar för varje dag som du har PEC-berättigad åtkomst för varje prenumeration. Även om PEC-information inte visas på månadsfakturan räknas PEC-intäkter in i raden med justerade nettoavgifter på fakturan. Du hittar mer information om PEC i filen [med daglig användning och](daily-rated-usage-recon-files.md) i rekognoseringsfilen för månadsfakturan.

:::image type="content" source="images/advanced-specializations/recon-file.png" alt-text="Skärmbild av en Avstämningsfil i Partnercenter som identifierar kolumner." border="false":::

I tabellen nedan beskrivs de PEC-element som finns i rekognoseringsfilen för månadsfaktura. Alla värden anges i USD, som du ser i kolumnen AI, PricingCurrency.

| Kolumn  | Beskrivning  |
| --------  | -------  |
| Kolumn C  | CustomerName  |
| Kolumn P | UnitPrice |
| Kolumn AD | EffectiveUnitPrice. Det här är priset när PEC har tillämpats och kraven har uppfyllts. När PEC används ser du att EffectiveUnitPrice i kolumn AD är en procentandel mindre än Enhetspris i kolumn P.   |
| Kolumn V  | PriceAdjustmentDescription. Detta är tomt om inga krav för PEC är uppfyllda eller har PEC % som kommer att tillämpas på enhetspris. Du kan dock vara berättigad till ytterligare krediter. I så fall visas de i den här kolumnen. Exempel: 100 % rabatt på nivå 1.   |

Så här övervakar du PEC-åtkomst:

- **Den dagliga klassificerade** användningsfilen visar var PEC tillämpas (eller inte) dagligen

- [**Azure Monitor-aviseringar**](azure-plan-manage.md) övervakar ändringar i beständig privilegierad åtkomst.

Den dagliga klassificerade användningsfilen:

:::image type="content" source="images/advanced-specializations/partner-daily.png" alt-text="Skärmbild av en daglig klassificerad användningsfil i Partnercenter som visar det effektiva enhetspriset." border="false":::

## <a name="partner-earned-credit-api"></a>API för partners intjänade kredit

Ett PEC-API är tillgängligt som en del av Azure API-verktygsuppsättningen. Information om PowerShell och CLI-API:er finns i [Länka ett Azure-konto till ett partner-ID.](/azure/cost-management-billing/manage/link-partner-id)

## <a name="azure-cost-management-and-pec"></a>Azure Cost Management och PEC

Azure Cost Management (ACM) med hjälp av kostnadsanalys kan du som partner visa de kostnader som har fått fördelen med PEC. En detaljerad presentation av ACM finns i CSP Spotlight-anropet från maj [2021.](https://commercial_licensing.eventbuilder.com/2021MayCSPSpotlight)

## <a name="use-acm-to-view-your-partner-earned-credit"></a>Använda ACM för att visa din partners intjänade kredit

1. I den [Azure Portal](https://portal.azure.com/)loggar du in på din partnerklientorganisation och **väljer Cost Management + Billing**.
2. Välj **Kostnadshantering.**
3. Välj **Kostnadsanalys.**
I vyn Kostnadsanalys visas kostnaderna för ditt faktureringskonto för alla tjänster som köpts och förbrukats till de priser som du betalar Microsoft.

:::image type="content" source="images/advanced-specializations/partner-cost.png" alt-text="Skärmbild av en kostnadsanalyssida för kostnadshantering." border="false":::

4. I listrutan pivotdiagram väljer du PartnerEarnedCreditApplied. 

    Om det här värdet **är Sant** har den associerade kostnaden fördelen med partnerns intjänade kredit.

    Om det här värdet **är Falskt** har den associerade kostnaden inte uppfyllt den berättigandenivå som krävs för krediten, eller så är den köpta tjänsten inte berättigad till partnerintjänad kredit.

>[!NOTE]
>Användningen av tjänster tar vanligtvis 8–24 timmar att visas i Cost Management och PEC-krediterna visas inom 48 timmar från åtkomsten i Azure Cost Management.

Du kan också gruppera efter och filtrera efter egenskapen **PartnerEarnedCreditApplied** med hjälp av funktionerna **Gruppera efter** **och Lägg** till filter. På så sätt kan du gå in på kostnader som har PEC och de kostnader som inte har någon tillämpad PEC.

## <a name="how-is-pec-paid"></a>Hur betalas PEC?
PEC-intäkter räknas in i raden med justerade nettoavgifter på fakturan. Summan **av** fakturan som visas nedan illustrerar detta. Mer information om justeringar finns i filen för månatlig fakturaavstämning och Azures dagliga klassificerade användningsfil.

:::image type="content" source="images/advanced-specializations/invoice.png" alt-text="Skärmbild av en Partnercenter-faktura som anger att justeringsinformationen visas på rekognoserings- och Azure-filer för daglig användning." border="false":::

## <a name="next-steps"></a>Nästa steg

- [Prislista för den nya handelsupplevelsen för Azure i CSP](azure-plan-price-list.md)
- [Hantera prenumerationer och resurser under Azure-planen](azure-plan-manage.md)
- [Ny handelsupplevelse i CSP – Azure-fakturering](azure-plan-billing.md)
- [Återställ administratörsbehörigheter för Azure CSP-prenumerationer](revoke-reinstate-csp.md)
- [Partner-intjänad kredit – översikt](partner-earned-credit.md)
- [Roller, behörigheter för partner-intjänad kredit](azure-roles-perms-pec.md)
- [Förstå partners intjänade kredit (guide)](https://partner.microsoft.com/resources/detail/understanding-partner-earned-credit-pdf) (inloggning krävs)