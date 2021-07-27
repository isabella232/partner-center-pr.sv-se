---
title: Överföra En Azure-prenumeration under en Azure-plan till en annan CSP-partner
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Lär dig hur du ändrar Molnlösningsleverantör programpartner som är associerad med en kunds Azure-prenumerationer under en Azure-plan.
ms.custom: SEOMAY.20
ms.localizationpriority: medium
author: mckennaville
ms.author: mcville
ms.date: 07/21/2021
ms.openlocfilehash: 258b593935e9fd599e0f5c524cd7ec935c50bcad
ms.sourcegitcommit: d133c8b923b90ac5518cb989c0ce4dd69713abf4
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 07/22/2021
ms.locfileid: "114434140"
---
# <a name="transfer-a-customers-azure-subscriptions-to-a-different-partner-in-csp-under-an-azure-plan"></a>Överföra en kunds Azure-prenumerationer till en annan partner i CSP (enligt en Azure-plan)

**Lämpliga roller:** Kontoadministratörsroller | Försäljningsagentens | Faktureringsagent

Den här artikeln beskriver hur en kund kan växla sina Azure-prenumerationer från en partner inom Molnlösningsleverantör (CSP) till en annan under en Azure-plan.

Följ dessa steg om du vill byta en kunds Azure-prenumerationer från en annan partner. Både partnern och kunden har steg att slutföra.

> [!Note]  
> Endast partner med en direkt faktureringsrelation med Microsoft kan komma åt övergångsverktyget. Indirekta återförsäljare måste samarbeta med sina indirekta leverantörer för att utnyttja det här övergångsverktyget.

Kunden måste föra en konversation med båda partnerna (aktuell och framtida) innan det här verktyget används. En offline-konversation måste vara tvungen att undvika förvirring och omsättning. Dessutom bör partner och kunder förstå dessa överväganden och förutsättningar innan de påbörjar en övergång:

**Viktiga överväganden:**

- Azure-reservationer flyttas inte med prenumerationen till framtida partner
- CSP-priser för Azure-tjänster under aktuell partner kommer inte att övergå
- Överföring av [tidigare Azure-erbjudandeprenumerationer (MS-AZR-0145p)](https://go.microsoft.com/fwlink/p/?linkid=2164140) resulterar i att dessa Azure-prenumerationer konverteras samtidigt till nya Azure-erbjudandeprenumerationer i en Azure-plan
- Kundens supportansvar flyttas till framtida partner
- Fakturering och fakturering flyttas till framtida partner vid tidpunkten för överföringen
- Azure Role-Based Access Control (RBAC) påverkas inte av överföringen
- Admin on Behalf Of (AOBO) beviljas inte som standard till den framtida partnern
- Marketplace-produkter från tredje part överförs så länge produkterna klarar berättigandekontrollen för Marketplace.
    - Det finns inga särskilda rabatter eller regionala begränsningar
    - Produkterna är inte prenumerationsbaserade
    - Den framtida partnern bör samarbeta med utgivaren för att se till att de finns på listan över tillåtna för distribution av produkten
    - Om inte alla dessa villkor uppfylls för att överföra Marketplace-produkterna ska avbrytas, överförs Azure-prenumerationerna och sedan på nytt av Marketplace-produkter med den nya partnern

**Krav:**

- Kunden engagerar den aktuella CSP-partnern om sin avsikt att övergå
- Framtida CSP-partner samarbetar med kunden för att säkerställa att kundernas behov kan uppfyllas
- En framtida CSP-partner upprättar en relation med kunden och köper en Azure-plan innan övergången börjar  
- Kunden måste signera Microsoft-kundavtal med en framtida CSP-partner
- En framtida CSP-partner måste ha signerat Microsoft-partneravtal att använda det här verktyget

> [!NOTE]
> Den här självbetjäningsverktygen kan användas när kundens nuvarande partner har antingen det tidigare Azure-erbjudandet (MS-AZR-0145p) eller det nya Azure-erbjudandet (Azure-plan). I båda fallen resulterar slutförandet av den här överföringen i Azure-prenumerationerna under en Azure-plan med den framtida partnern.

## <a name="customer-tasks-to-be-completed"></a>Kunduppgifter som ska slutföras

För att överföra Azure-prenumerationer måste kunden starta processen genom att kontakta sin nuvarande partner. De bör samla in den aktuella partnerns företagsnamn och Microsoft-ID så att deras framtida partner kan fylla i formuläret för överföringsbegäran för sin räkning.

Kunden måste också identifiera de prenumerationer som de vill överföra från den aktuella partnern. Du kan inte byta partner för Office 365, Enterprise Mobility Suite eller Microsoft Dynamics CRM prenumerationer.

> [!NOTE]  
> Det är den framtida partnerns ansvar att fylla i formuläret för överföringsbegäran som initierar överföringsprocessen. Microsoft kan inte göra något åt kunden eller den aktuella partnern. Kunden bör planera ett nära samarbete med sin framtida och nuvarande partner för att övergången ska gå smidigt.

## <a name="future-partner-tasks-to-be-completed"></a>Framtida partneruppgifter som ska slutföras

Prenumerationens framtida partner måste fylla i ett formulär för överföringsbegäran från Partnercenter för att begära en prenumerationsöverföring:

1.  I menyn i Partnercenter väljer du **Kunder** och sedan den kund som du vill fylla i ett formulär för överföringsbegäran för.
2.  Välj Prenumerationer på menyn **Kund.**
3.  Välj avsnittet **Överföringsbegäran.**
4.  I avsnittet **Överföringsbegäran väljer** du Lägg **till ny begäran.**

    :::image type="content" source="images/modernazuretransfers/Transferrequestheader.png" alt-text="Avsnittet Överföringar.":::

5.  Fyll i **formuläret Ny överföringsbegäran.**

6.  Välj **Skicka överföringsbegäran**  >  **Skicka**.

    :::image type="content" source="images/modernazuretransfers/CompleteTrnasferRequestForm.png" alt-text="Fyll i formuläret för överföringsbegäran.":::

7.  Granska bekräftelse av överföringsbegäran

    :::image type="content" source="images/modernazuretransfers/TransferPending.png" alt-text="Granska väntande överföring.":::

    > [!NOTE]
    > Den framtida partnern kan avbryta  överföringsbegäran genom att välja Avbryt begäran i det övre högra hörnet endast när statusen för överföringsbegäran är "väntande". När statusen för överföringsbegäran är "pågår" eller "klar" går det inte att avbryta.

## <a name="current-partner-tasks-to-be-completed"></a>Aktuella partneruppgifter som ska slutföras

Den aktuella partnerns administratörsagent för kunden får ett e-postmeddelande om att kunden begär överföring av sina prenumerationer:

:::image type="content" source="images/modernazuretransfers/SourceReviewEmail.png" alt-text="Recension.":::

Granska och acceptera formuläret för överföringsbegäran från Partnercenter för att slutföra prenumerationsöverföringen.

> [!NOTE]  
> Om ingen åtgärd vidtas av den aktuella partnern inom 30 dagar upphör begäran att gälla och den framtida partnern har en för att skapa en ny överföringsbegäran.

- Välj **Granska överföringsbegäran från** e-postmeddelandet

   \- eller -

1. I menyn i Partnercenter väljer **du Kunder** och sedan den kund som en överföringsbegäran har skickats för.
2. Välj Prenumerationer på menyn **Kund.**
3. Välj avsnittet **Överföringsbegäran.**
4.Expandera överföringsinformation genom att välja det valda **ID:t för överföringsbegäran** under **Mottagna begäranden**

:::image type="content" source="images/modernazuretransfers/ReviewRequest.png" alt-text="Överföringsbegäran för källgranskningar.":::

5. Granska överföringsbegäran. Välj de Azure-prenumerationer som ska överföras.
 
Observera följande innan du fortsätter:
- Du kommer inte längre att ha åtkomst till de valda prenumerationerna.
- Du faktureras inte för ytterligare användning.
- Azure-reservationer överförs inte med prenumerationerna.

6. Välj sedan **Acceptera och överför** för att slutföra överföringsprocessen.

:::image type="content" source="images/modernazuretransfers/SelectSubs.png" alt-text="Välj prenumerationer som ska överföras under dina Azure-planer.":::

Om den aktuella partnern har en kund med tidigare prenumerationer på Azure-erbjudanden (MS-AZR-0145p) fortsätter kunden på samma sätt genom att välja de prenumerationer som ska överföras och sedan välja Acceptera och överföra för att slutföra överföringen.

7. Visa bekräftelse på överföringsgodkännande.

   Nu meddelas den framtida partnern, kunden och den aktuella partnern om den accepterade överföringsbegäran via e-post.

   Efter att övergången har godkänts kan överföringsstatusen vara Väntande i upp till 15 minuter medan systemet uppdateras. Om det tar längre tid fortsätter systemet att försöka i tre dagar. Om överföringsstatusen fortfarande är Väntande bör partnern skicka en tjänstbegäran.

   När överföringen är klar visas de prenumerationer som ingår i begäran i Azure-planen för den framtida partnern och visas inte längre med dig.

>[!Note]  
>För indirekta leverantörer: Informera den indirekta återförsäljaren om att överföringsbegäran har accepterats.

### <a name="managing-your-transferred-customer-subscriptions"></a>Hantera dina överförda kundprenumerationer

- Åtkomst till befintliga användare, grupper eller tjänsthuvudnamn som tilldelades med hjälp av Azure RBAC (rollbaserad åtkomstkontroll) påverkas inte under övergången. Rollbaserad åtkomstkontroll [i Azure (Azure RBAC)](/azure/role-based-access-control/overview) hjälper kunden att hantera vem som har åtkomst till Azure-resurser, vad de kan göra med dessa resurser och vilka områden de har åtkomst till. Som ny partner får du ingen RBAC-åtkomst till kundens resurser efter prenumerationsöverföringen. Kundens tidigare partner behåller sin RBAC-åtkomst. Samarbeta med kunden för att förstå vem som har insyn i sina prenumerationer och hur du gör önskade ändringar.

- Därför är det viktigt att kunden tar bort Azure RBAC-åtkomst för sin tidigare partner och lägger till åtkomst för den nya partnern. Mer information om hur din kund ger ny åtkomst finns i [Vad är rollbaserad åtkomstkontroll i Azure (Azure RBAC)?](/azure/role-based-access-control/overview) Mer information om hur kunden tar bort din tidigare partners RBAC-åtkomst finns i [Ta bort en rolltilldelning.](/azure/role-based-access-control/role-assignments-portal#remove-a-role-assignment)

- Dessutom får du inte automatiskt [AOBO-åtkomst (Admin on Behalf Of)](https://channel9.msdn.com/Series/cspdev/Module-11-Admin-On-Behalf-Of-AOBO) till dina prenumerationer. AOBO är nödvändigt för att partnern ska kunna hantera kundens Azure-prenumerationer åt dem. Mer information om Azure-behörigheter finns i [Skaffa behörigheter för att hantera en kunds tjänst eller prenumeration.](./customers-revoke-admin-privileges.md)

## <a name="next-steps"></a>Nästa steg:

- [(Azure RBAC)](/azure/role-based-access-control/overview)
- [Få behörighet att hantera en kunds tjänst eller prenumeration.](./customers-revoke-admin-privileges.md)
