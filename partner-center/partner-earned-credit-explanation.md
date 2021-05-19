---
title: Partner-intjänad kredit för hanterade tjänster
ms.topic: article
ms.date: 12/16/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Lär dig hur Microsoft-partners intjänade kredit (PEC) för hanterade tjänster beräknas och betalas och hur du säkerställer att du är berättigad.
author: adamyeh
ms.author: adamyeh
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: ba422a2feae2affb9c2b60ad345c4d6bb0d525c7
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 05/19/2021
ms.locfileid: "110145872"
---
# <a name="how-the-partner-earned-credit-is-calculated-and-paid"></a>Hur partnerintjänad kredit beräknas och betalas

**Lämpliga roller:** Globala | Administratörsbehörighet för | Administratörsagent | Faktureringsadministratörskonto | Försäljningsagent

Partnerns intjänade kredit för hanterade tjänster (PEC) identifierar och delar ut förmåner till partner som äger DEN operativa kontrollen och hanteringen av delar av, eller hela Azure-miljön för sina kunder, dygnet runt. Som standard beviljas partner i CSP de nödvändiga åtkomsträttigheterna till kundens prenumeration så att de kan utföra drifthantering dygnet runt och kontrollera resurserna i prenumerationen. Andra sätt på vilka kunder kan etablera åtkomst för att köpa partners beskrivs i följande avsnitt. Det månatliga fakturabeloppet är nettot av partnerns intjänade kredit. Partner kan se PEC-informationen i sin månatliga rekognoseringsfil. Mer information om hur en kund kan etablera åtkomst för den hanterande partnern finns i [Hantera prenumerationer och resurser i Azure-planen.](azure-plan-manage.md)

Läs även [Återställa administratörsbehörigheter för Azure CSP prenumerationer](revoke-reinstate-csp.md)

## <a name="eligibility"></a>Stödberättigande

För att få partnerns intjänade kredit (PEC) gäller följande krav: 

- Du måste ha ett aktivt MPN-avtal och en giltig rollbaserad åtkomstkontrollroll (RBAC) för att få intjänad kredit för de Azure-tillgångar som du hanterar.

- Du måste ha driftkontroll dygnet runt och hantering av kundens Azure-resurser i CSP. Det innebär att du måste ha administratörsbehörighet för kundens Azure-prenumeration, Azure-resursgrupp och Azure-resurs. När det gäller indirekta leverantörer och deras indirekta återförsäljare är den indirekta leverantören berättigad till PEC om antingen den indirekta leverantören eller den indirekta återförsäljaren eller båda har denna operativa kontroll. Mer information om detta finns i [Återställa administratörsbehörigheter för Azure CSP prenumerationer.](./revoke-reinstate-csp.md)

- Utöver kraven ovan gäller PEC endast för tjänster som anges i prissättningen för Azure-planförbrukning, som du kan exportera från sidan med priser [för Azure-plan.](https://partner.microsoft.com/commerce/sales)

- PEC **gäller** inte för följande tjänster:
    - Azure-planreservationer
    - Produkter från tredje part som identifierats som tredje part i kolumnen Taggar i Azure-planens förbrukningspris
    - Produkter i Marketplace-prislistan
    - [Azure Spot Virtual Machines](https://partner.microsoft.com/resources/collection/azure-spot-in-csp#/)

- PEC intjänas till Azure-resursnivån. Om du har giltig åtkomst på prenumerations- eller resursgruppsnivå får varje resurs som ingår i den högre entiteten PEC.

- Information om PEC finns också på sidan [Azure Cost Management.](/azure/cost-management-billing/costs/get-started-partners)

### <a name="calculation"></a>Beräkning

PEC beräknas dagligen och kan visas i filen med daglig användning och månatliga fakturarekognoseringsfiler. En partner (indirekt leverantör eller indirekt återförsäljare) måste ha åtkomst för hela dagen (dygnet runt) för att säkerställa att de tjänar PEC. PEC beräknas dagligen utifrån de hanterade Azure-tillgångarna. Partner som behåller beständig privilegierad åtkomst under månaden (åtkomstomfånget) och för alla berättigade resurser (åtkomstomfång) får fullständig PEC. Omfångs- och spannminskning resulterar i lägre PEC-frekvens för månaden. Den dagliga klassificerade användningsfilen visas dagligen på en Azure-tillgång, oavsett om PEC tillämpas eller inte. Partner kan också registrera sig i aviseringar för att övervaka ändringar av beständig privilegierad åtkomst.

## <a name="azure-cost-management"></a>Azure Cost Management

Azure Cost Management (ACM) med hjälp av kostnadsanalys kan du som partner visa de kostnader som har fått förmånen av PEC.  

1. I den [Azure Portal](https://portal.azure.com)loggar du in på din partnerklientorganisation och **väljer Cost Management + Billing**.

2. Välj **Kostnadshantering**

3. Välj **Kostnadsanalys**

   I vyn Kostnadsanalys visas kostnaderna för ditt faktureringskonto för alla tjänster som köpts och förbrukats till de priser som du betalar Microsoft.

4. Välj **PartnerEarnedCreditApplied** i listrutan i ett pivotdiagram för att se kostnader som har tillämpats av PEC. När **egenskapen PartnerEarnedCreditApplied** är True får den associerade kostnaden fördelen med partnerns intjänade kredit. 

   När egenskapen PartnerEarnedCreditApplied är False har den tillhörande kostnaden inte uppfyllt den berättigande som krävs för krediten, eller så är den köpta tjänsten inte berättigad till partnerintjänad kredit.

   >[!NOTE] 
   >Användningen av tjänster tar vanligtvis 8–24 timmar att visas **i Cost Management** och PEC-krediterna visas inom 48 timmar från åtkomsten i Azure Cost Management.

5. Du kan också gruppera efter och filtrera efter egenskapen **PartnerEarnedCreditApplied** med hjälp av funktionerna **Gruppera** efter och Lägg till filter för att granska kostnader som har PEC och de kostnader som inte har någon tillämpad PEC.

## <a name="next-steps"></a>Nästa steg

- [Partner-intjänad kredit – översikt](partner-earned-credit.md)

- Detaljerade exempel på beräkning av partners intjänade kredit finns i prislistan som du kan nå via instrumentpanelen i Partnercenter (inloggning krävs).

- [Flytta till Azure-plan – kom igång](azure-plan-get-started.md)

- [Hantera prenumerationer och resurser under Azure-planen](azure-plan-manage.md)

- [Återkalla eller återställa administratörsbehörigheter för Azure CSP prenumerationer](revoke-reinstate-csp.md)
