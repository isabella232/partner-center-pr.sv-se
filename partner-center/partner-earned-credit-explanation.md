---
title: Partner intjänad kredit för hanterade tjänster
ms.topic: article
ms.date: 12/16/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Lär dig hur Microsoft partner intjänad kredit (PEC) för hanterade tjänster beräknas och betalas och hur du garanterar att du är berättigad.
author: adamyeh
ms.author: adamyeh
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 3acc078b3de3c0443ee64fdaaba2d486d9c466c8
ms.sourcegitcommit: e9066768ab8e242c03f0a7e3ce460ae8cd2e3fda
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 12/17/2020
ms.locfileid: "97622175"
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

## <a name="eligibility"></a>Behörighet

Följande krav gäller för att få partner företaget intjänade kredit (PEC): 

- Du måste ha ett aktivt MPN-avtal och en giltig rollbaserad åtkomst kontroll (RBAC) för att få intjänad kredit för de Azure-tillgångar som du hanterar.

- Du måste ha dygnet runt drifts kontroll och hantering av kundens Azure-resurser i CSP. Det innebär att du måste ha administratörs behörighet för kundens Azure-prenumeration, Azure-resurs grupp, Azure-resurs. Om det gäller indirekta leverantörer och deras indirekta åter försäljare är den indirekta leverantören berättigad till PEC om antingen den indirekta leverantören eller den indirekta åter försäljaren eller båda har denna operativa kontroll. Läs mer om det här i [återställa administratörs behörigheter för Azure CSP-prenumerationer](https://docs.microsoft.com/partner-center/revoke-reinstate-csp).

- Utöver kraven ovan gäller PEC endast för tjänster som anges i prissättningen för Azure-abonnemang, som du kan exportera från pris sidan för [Azure-prenumerationen](https://partner.microsoft.com/commerce/sales) .

- PEC gäller **inte** för följande tjänster:
    - Azure plan-reservationer
    - Produkter från tredje part som identifieras som tredje part i kolumnen Taggar i pris för Azure plan-förbrukning
    - Produkter i pris listan för Marketplace
    - [Virtual Machines för Azure-plats](https://partner.microsoft.com/resources/collection/azure-spot-in-csp#/)

- PEC är intjänad på Azure-resursnivå. Om du har giltig åtkomst på antingen prenumerations-eller resurs grupps nivå får du PEC genom att varje resurs som slås samman till den högre enheten.

- Information om PEC finns också på sidan för [Azure Cost Management](https://docs.microsoft.com/azure/cost-management-billing/costs/get-started-partners) .

### <a name="calculation"></a>Beräkning

PEC beräknas dagligen och kan visas i den dagliga användnings filen och en månads faktura rekognoseringar-fil. En partner (indirekt provider eller indirekt åter försäljare) måste ha åtkomst för hela dagen (dygnet runt) för att säkerställa att de får PEC. PEC beräknas dagligen på de hanterade Azure-resurserna. Högsta PEC för en viss fakturerings period (månad) är 15%. Partner som bevarar beständig privilegie rad åtkomst under månaden (omfånget för åtkomst) och för alla berättigade resurser (åtkomstscope) får fullständig PEC på 15%. Omfångs-och span-reducering ger lägre PEC-pris för månaden. Dagligt klassificerad användnings fil visas dagligen på en Azure-till gång, oavsett om PEC används eller inte. Partner kan också registrera aviseringar för att övervaka ändringar i beständig privilegie rad åtkomst.

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
