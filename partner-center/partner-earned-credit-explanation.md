---
title: Partner intjänad kredit för hanterade tjänster
ms.topic: article
ms.date: 11/30/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Lär dig hur Microsoft partner intjänad kredit (PEC) för hanterade tjänster beräknas och betalas och hur du garanterar att du är berättigad.
author: adamyeh
ms.author: adamyeh
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 97af446c4021e9785833374131eee2f08431b5fe
ms.sourcegitcommit: 4043c791402f0acebee6ede160a135e87fe92493
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 12/01/2020
ms.locfileid: "96474316"
---
# <a name="how-the-partner-earned-credit-is-calculated-and-paid"></a>Hur partnerintjänad kredit beräknas och betalas

**Lämpliga roller**

- Global administratör
- Användaradministratör
- Administratörs agent
- Faktureringsadministratör
- Försäljnings agent

Partner intjänad kredit för hanterade tjänster (PEC) känner av och fördelar partner som äger den dygnet runt IT-operativa styrning och hantering av delar av, eller hela, Azure-miljön för kunderna. Som standard beviljas partner i CSP de nödvändiga åtkomst rättigheterna till kundens prenumeration så att de kan utföra 24 X 7 drifts hantering och kontroll över resurserna i prenumerationen. Ytterligare sätt som kunden kan använda för att etablera åtkomst för att agera partner beskrivs i följande avsnitt. Det månatliga fakturabeloppet är efter av partner intjänad kredit. Partner kan se PEC-information om sina månatliga rekognoseringar-filer. Läs [Hantera prenumerationer och resurser i Azure-prenumerationen](azure-plan-manage.md)för ytterligare sätt som en kund kan använda för att etablera åtkomst för den inhandlande partnern.

Läs även [återställa administratörs behörighet för Azure CSP-prenumerationer](revoke-reinstate-csp.md)

## <a name="important-eligibility-and-calculation-information"></a>Viktig information om berättigande och beräkningar

- Partner bör ha ett aktivt MPN-avtal och en giltig RBAC-roll för att få intjänad kredit för de Azure-tillgångar som de hanterar. 

- När det gäller indirekta leverantörer och deras indirekta åter försäljare är den indirekta leverantören berättigad till PEC om antingen den indirekta leverantören eller den indirekta åter försäljaren eller både har drifts kontroll och hantering av kundens Azure-resurser i CSP.

- PEC är kopplad till fakturerad (debiterbar) förbrukning av kundens Azure-egendom i CSP som hanteras av partnern. PEC görs endast tillgängligt för partner i CSP som faktureras av Microsoft (indirekt leverantör och direkt fakturerings partner). 

- Berättigade tjänster: partner intjänad kredit är tillämplig på tjänster som anges i **prissättningen för Azure-abonnemang** som partner kan exportera från pris sidan för [Azure-prenumerationen](https://partner.microsoft.com/commerce/sales) . 

- Ej berättigade tjänster: partner intjänad kredit är **_inte_* _ tillämplig på följande:
    - Azure plan-reservationer
    - Produkter från tredje part som identifieras som en *tredje part** i **kolumnen Taggar** i priset för Azure plan-förbrukning    
    - Produkter i pris listan för Marketplace
   - [Virtual Machines för Azure-plats](https://partner.microsoft.com/resources/collection/azure-spot-in-csp#/)

- PEC beräknas dagligen och kan visas i den dagliga användnings filen och en månads faktura rekognoseringar-fil. En partner (indirekt provider eller indirekt åter försäljare) måste ha åtkomst för hela dagen (dygnet runt) för att säkerställa att de får PEC. PEC beräknas dagligen på de hanterade Azure-resurserna. Högsta PEC för en viss fakturerings period (månad) är 15%. Partner som bevarar beständig privilegie rad åtkomst under månaden (omfånget för åtkomst) och för alla berättigade resurser (åtkomstscope) får fullständig PEC på 15%. Omfångs-och span-reducering ger lägre PEC-pris för månaden. Dagligt klassificerad användnings fil visas på daglig basis på en Azure-till gång oavsett om PEC används eller inte. Partner kan också registrera sig i aviseringar för att upptäcka om det finns ändringar i beständig privilegie rad åtkomst.

- PEC är intjänad på Azure-resursnivå. Om partnern har giltig åtkomst till prenumerationen eller resurs grupps nivån får varje resurs som har rollen upp till den högre enheten PEC.  

- PEC-information kommer också att vara tillgänglig i [Azure Cost Management](/azure/cost-management-billing/costs/get-started-partners)

## <a name="azure-cost-management"></a>Azure Cost Management

Azure Cost Management (ACM) med hjälp av kostnads analys kan du som partner se de kostnader som har fått fördelen med PEC.  

1. Logga in på partner klienten i [Azure Portal](https://portal.azure.com)och välj **Cost Management + fakturering**.

2. Välj **kostnads hantering**

3. Välj **kostnads analys**

   I vyn kostnads analys visas kostnaderna för ditt fakturerings konto för alla tjänster som köpts och förbrukas enligt de priser som du betalar för Microsoft.

4. Välj **PartnerEarnedCreditApplied** i list rutan i ett pivot-diagram för att Visa kostnader där PEC har tillämpats. När **PartnerEarnedCreditApplied** -egenskapen är true, har den tillhör ande kostnaden nytta av partner intjänade kredit. 

När PartnerEarnedCreditApplied-egenskapen har värdet false har den tillhör ande kostnaden inte uppfyllt den nödvändiga behörigheten för krediten eller så är den köpta tjänsten inte berättigad till partner intjänad kredit.

>[!NOTE] 
>Normalt tar användningen av tjänster 8-24 timmar innan den visas i **Cost Management** och PEC-krediterna visas inom 48 timmar från tiden för åtkomst i Azure Cost Management.

5. Du kan också gruppera efter och filtrera efter, egenskapen **PartnerEarnedCreditApplied** med hjälp av **Group by och lägga till** filter funktioner för att öka detalj nivån för kostnader som har PEC och kostnader som inte har använts.

## <a name="next-steps"></a>Nästa steg

- [Partner intjänad kredit – översikt](partner-earned-credit.md)

- Detaljerade exempel på intjänade kredit beräkningar för partner finns i pris listan som du kan komma åt via instrument panelen för partner Center (inloggning krävs).

- [Flytta till Azure plan – kom igång](azure-plan-get-started.md)

- [Hantera prenumerationer och resurser under Azure-planen](azure-plan-manage.md)

- [Återkalla eller Omtillstånd administratörs behörighet för Azure CSP-prenumerationer](revoke-reinstate-csp.md)
