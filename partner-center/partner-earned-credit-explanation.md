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
ms.openlocfilehash: 3583614b1bf89a3c9297f123f12355b8a2ad7d1e
ms.sourcegitcommit: 37eac16c4339cb97831eb2a86d156c45bdf6a531
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/13/2021
ms.locfileid: "126246780"
---
# <a name="how-the-partner-earned-credit-is-calculated-and-paid"></a>Hur partnerintjänad kredit beräknas och betalas

**Lämpliga roller:** Global | Administratörsbehörighet för användarhantering | Administratörsagentens | Faktureringsadministratörskonto | Försäljningsagent

Partner-intjänad kredit (PEC) för hanterade tjänster identifierar och premierar partner som äger IT-driftkontroll och hantering av vissa eller alla kunders Azure-miljöer. 

Som standard beviljas du som CSP-partner nödvändiga åtkomsträttigheter till kundens prenumeration, så att du kan utföra drifthantering och kontroll över resurserna i prenumerationen. Andra sätt på vilka kunder kan etablera åtkomst för partner som gör en överträdelse beskrivs i följande avsnitt.

Det månatliga fakturabeloppet är nettot av partnerns intjänade kredit. Du kan se PEC-information om din månatliga rekognoseringsfil. Mer information om hur en kund kan etablera åtkomst för den transacting-partnern finns i följande artiklar:

- [Hantera prenumerationer och resurser under Azure-planen](azure-plan-manage.md)
- [Återställ administratörsbehörigheter för Azure CSP-prenumerationer](/revoke-reinstate-csp.md)

## <a name="eligibility"></a>Stödberättigande

Följande krav gäller för att ta emot partners intjänade kredit (PEC):

- Du måste ha ett aktivt MPN-avtal och en giltig rollbaserad [åtkomstkontrollroll](azure-roles-perms-pec.md) [(RBAC).](/azure/role-based-access-control/overview)
- Du måste ha [AOBO-behörigheter (Admin on Behalf of)](https://channel9.msdn.com/Series/cspdev/Module-11-Admin-On-Behalf-Of-AOBO) för kundens Azure-prenumeration, Azure-resursgrupp eller Azure-resurs, eller en giltig [RBAC-roll.](azure-roles-perms-pec.md)
- När det gäller indirekta leverantörer och deras indirekta återförsäljare är en indirekt leverantör berättigad till PEC om antingen den indirekta leverantören eller den indirekta återförsäljaren eller båda har AOBO-privilegier eller en berättigad RBAC-roll. Mer information finns i Återställa [administratörsbehörigheter för Azure CSP prenumerationer.](revoke-reinstate-csp.md)
- Partnerns MPN-ID måste tillhöra samma v-organisation som inköparens MPN-ID eller MPN-ID:t Partner of Record (MPN). Mer information finns i [Länka ditt partner-ID för att se hur du påverkar delegerade resurser](/azure/lighthouse/how-to/partner-earned-credit).
- PEC intjänas på Azure-resursnivå, resursgrupp eller prenumeration. Om en partner har giltig åtkomst på prenumerations- eller resursgruppsnivå får varje resurs som ingår i den högre entiteten PEC.
- PEC gäller inte för följande tjänster:
    - Azure-planreservationer
    - Produkter från tredje part som identifierats som tredje part i kolumnen Taggar i azure-planens förbrukningspris
    - Produkter i Marketplace-prislistan
    - [Azure Spot Virtual Machines](https://partner.microsoft.com/resources/collection/azure-spot-in-csp#/)

Utöver kraven ovan gäller PEC endast för tjänster som anges i prissättningen för Azure-planförbrukning. Du kan visa och exportera detta från [prissättningssidan för Azure-plan.](https://partner.microsoft.com/commerce/sales)

Mer information om PEC finns på sidan [om Azure Cost Management.](/azure/cost-management-billing/costs/get-started-partners)

Mer information om berättigande finns i Roller [och behörigheter som krävs för att få partner-intjänad kredit.](azure-roles-perms-pec.md)

## <a name="calculation"></a>Beräkning

PEC beräknas dagligen. Du betalar för varje dag som du har PEC-berättigad åtkomst för varje prenumeration. Även om PEC-information inte visas på månadsfakturan räknas PEC-intäkter in i den justerade nettodelade debiteringsraden på fakturan. Du hittar mer PEC-information i filen [för daglig användning och](daily-rated-usage-recon-files.md) i avse-filen med månadsfakturan.

:::image type="content" source="images/advanced-specializations/recon-file.png" alt-text="Skärmbild av en Partner Center-avstämningsfil som identifierar kolumner." border="false":::

I tabellen nedan beskrivs de PEC-element som finns i rekognoseringsfilen för månadsfakturan. Alla värden är i USD, som du ser i kolumnen AI, PricingCurrency.

| Kolumn  | Beskrivning  |
| --------  | -------  |
| Kolumn C  | CustomerName  |
| Kolumn P | UnitPrice |
| Kolumn AD | EffectiveUnitPrice. Det här är priset när PEC har tillämpats och kraven har uppfyllts. När PEC tillämpas ser du att EffectiveUnitPrice i kolumn AD är en procentandel mindre än UnitPrice i kolumn P.   |
| Kolumn V  | PriceAdjustmentDescription. Detta är tomt om inga krav för PEC är uppfyllda eller har PEC % som kommer att tillämpas på Enhetspris. Du kan dock vara berättigad till ytterligare krediter. I så fall visas de i den här kolumnen. Exempel: Rabatt på 100 % nivå 1.   |

Så här övervakar du PEC-åtkomst:

- **Filen med daglig beräknad** användning visar var PEC tillämpas (eller inte) dagligen

- [**Azure Monitor-aviseringar**](azure-plan-manage.md) övervakar ändringar av beständig privilegierad åtkomst.

Filen med daglig klassificerad användning:

:::image type="content" source="images/advanced-specializations/partner-daily.png" alt-text="Skärmbild av en daglig klassificerad användningsfil i Partnercenter som visar det effektiva enhetspriset." border="false":::

## <a name="partner-earned-credit-api"></a>API för partners intjänade kredit

Ett PEC-API är tillgängligt som en del av Azure API-verktygsuppsättningen. Information om PowerShell och CLI-API:er finns i [Länka ett Azure-konto till ett partner-ID.](/azure/cost-management-billing/manage/link-partner-id)

## <a name="azure-cost-management-and-pec"></a>Azure Cost Management och PEC

Azure Cost Management (ACM) med hjälp av kostnadsanalys kan du som partner visa de kostnader som har fått fördelen med PEC. En detaljerad presentation om ACM finns i CSP Spotlight-anropet [från maj 2021.](https://commercial_licensing.eventbuilder.com/2021MayCSPSpotlight)

## <a name="use-acm-to-view-your-partner-earned-credit"></a>Använda ACM för att visa din partners intjänade kredit

1. I den [Azure Portal loggar](https://portal.azure.com/)du in på din partnerklientorganisation och **väljer Cost Management + Billing**.
2. Välj **Kostnadshantering.**
3. Välj **Kostnadsanalys.**
I vyn Kostnadsanalys visas kostnaderna för ditt faktureringskonto för alla tjänster som köpts och förbrukats till de priser som du betalar för Microsoft.

:::image type="content" source="images/advanced-specializations/partner-cost.png" alt-text="Skärmbild av en kostnadsanalyssida för kostnadshantering." border="false":::

4. I listrutan pivotdiagram väljer du PartnerEarnedCreditApplied. 

    Om det här värdet **är Sant** har den associerade kostnaden fördelen med partnerns intjänade kredit.

    Om det här värdet **är Falskt** har den associerade kostnaden inte uppfyllt det nödvändiga berättigandet för krediten, eller så är den köpta tjänsten inte berättigad till partner-intjänad kredit.

>[!NOTE]
>Användning för tjänster tar vanligtvis 8–24 timmar att visas i Cost Management och PEC-krediterna visas inom 48 timmar från åtkomsten i Azure Cost Management.

Du kan också gruppera efter och filtrera efter egenskapen **PartnerEarnedCreditApplied** med hjälp av funktionerna **Gruppera efter** och **Lägg** till filter. Med dessa kan du gå in på detalj i kostnader som har PEC och de kostnader som inte har någon tillämpad PEC.

## <a name="how-is-pec-paid"></a>Hur betalas PEC?
PEC-intäkter räknas in i raden med justerade nettoavgifter på fakturan. Summan **av** fakturan som visas nedan illustrerar detta. Mer information om justeringar finns i filen för månatlig fakturaavstämning och Azures dagliga klassificerade användningsfil.

:::image type="content" source="images/advanced-specializations/invoice.png" alt-text="Skärmbild av en Partnercenter-faktura som anger att justeringsinformation visas på rekognoserings- och Azure-filer för daglig användning." border="false":::

## <a name="next-steps"></a>Nästa steg

- [Prislista för den nya handelsupplevelsen för Azure i CSP](azure-plan-price-list.md)
- [Hantera prenumerationer och resurser under Azure-planen](azure-plan-manage.md)
- [Ny handelsupplevelse i CSP – Azure-fakturering](azure-plan-billing.md)
- [Återställ administratörsbehörigheter för Azure CSP-prenumerationer](revoke-reinstate-csp.md)
- [Partner-intjänad kredit – översikt](partner-earned-credit.md)
- [Roller, behörigheter för partner-intjänad kredit](azure-roles-perms-pec.md)
- [Förstå partners intjänade kredit (guide)](https://partner.microsoft.com/resources/detail/understanding-partner-earned-credit-pdf) (inloggning krävs)