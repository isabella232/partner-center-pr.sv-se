---
title: Överföra En Azure-prenumeration under en Azure-plan till en annan CSP-partner
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
description: Lär dig hur du ändrar Molnlösningsleverantör partner som är associerad med en kunds Azure-prenumerationer under en Azure-plan.
ms.custom: SEOMAY.20
ms.localizationpriority: medium
author: mckennaville
ms.author: mcville
ms.date: 07/21/2021
ms.openlocfilehash: 14f03a8eb899f7224a38b0f998edd72077b34b3b
ms.sourcegitcommit: ad1af627f5ee6b6e3a70655f90927e932cf4c985
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 07/29/2021
ms.locfileid: "114844283"
---
# <a name="transfer-a-customers-azure-subscriptions-to-a-different-csp-under-an-azure-plan"></a>Överföra en kunds Azure-prenumerationer till en annan CSP (under en Azure-plan)

**Lämpliga roller:** Kontoadministratörsroller | Försäljningsagent | Faktureringsagent

I den här artikeln beskrivs hur kunder kan ändra sina Azure-prenumerationer från en partner i Molnlösningsleverantör-programmet (CSP) till en annan under en Azure-plan.

Följ dessa steg om du vill byta en kunds Azure-prenumerationer från en annan partner. Den aktuella partnern, den framtida partnern och kunden har alla steg att slutföra.

> [!Note]  
> Endast partner som har en direktfaktureringsrelation med Microsoft kan komma åt övergångsverktyget. Indirekta återförsäljare måste samarbeta med sina indirekta leverantörer för att använda det här övergångsverktyget.

Kunden måste kommunicera med både den aktuella och framtida partnern innan övergångsverktyget kan användas. En offline-konversation måste ske för att undvika förvirring och omsättning. Partner och kunder bör förstå följande överväganden och förutsättningar innan en övergång påbörjas.

## <a name="considerations"></a>Överväganden

- Azure-reservationer flyttas inte med en prenumeration till den framtida partnern.
- CSP-priser för Azure-tjänster under den aktuella partnern kommer inte att övergå.
- Om du överför tidigare [Azure-prenumerationer (MS-AZR-0145p)](https://go.microsoft.com/fwlink/p/?linkid=2164140) konverteras dessa Azure-prenumerationer samtidigt till prenumerationer med nya Azure-erbjudanden i en Azure-plan.
- Kundens supportansvar flyttas till den framtida partnern.
- Faktureringen flyttas till den framtida partnern när prenumerationen överförs.
- Rollbaserad åtkomstkontroll (RBAC) i Azure påverkas inte av överföringar.
- Admin on Behalf Of (AOBO) beviljas inte som standard till den framtida partnern.
- Tredjepartsprodukter Azure Marketplace överförs så länge produkterna uppfyller behörighetskontrollen Azure Marketplace behörighet.
    - Det finns inga särskilda rabatter eller regionala begränsningar.
    - Produkterna är inte prenumerationsbaserade.
    - Den framtida partnern bör samarbeta med utgivaren för att se till att utgivaren finns på listan över tillåtna för distribution av produkten.
    - Om något av dessa villkor inte uppfylls bör Azure Marketplace produkter avbrytas. Sedan ska Azure-prenumerationerna överföras och Azure Marketplace bör köpas med den nya partnern.

## <a name="prerequisites"></a>Förutsättningar

- Kunden meddelar den aktuella CSP-partnern om avsikten att övergå.
- Den framtida CSP-partnern samarbetar med kunden för att säkerställa att kundens behov kan uppfyllas.
- Den framtida CSP-partnern upprättar en relation med kunden och köper en Azure-plan innan övergången börjar.
- Kunden signerar en Microsoft-kundavtal med den framtida CSP-partnern.
- Den framtida CSP-partnern signerar Microsoft-partneravtal innan du använder övergångsverktyget.

> [!NOTE]
> Övergångsverktyget med självbetjäning kan användas när kundens nuvarande partner har antingen det tidigare Azure-erbjudandet (MS-AZR-0145p) eller det nya Azure-erbjudandet (Azure-plan). I båda fallen, när överföringen är klar, kommer Azure-prenumerationerna att finnas under en Azure-plan med den framtida partnern.

## <a name="customer-tasks"></a>Kunduppgifter

För att överföra Azure-prenumerationer måste kunden starta processen genom att kontakta den aktuella partnern. Kunden bör samla in den aktuella partnerns företagsnamn och Microsoft-ID så att den framtida partnern kan fylla i formuläret för överföringsbegäran för kundens räkning.

Kunderna måste också identifiera de prenumerationer som de vill överföra från den aktuella partnern. Du kan inte byta partner för Office 365, Enterprise Mobility Suite eller Microsoft Dynamics CRM prenumerationer.

> [!NOTE]  
> Det är den framtida partnerns ansvar att fylla i formuläret för överföringsbegäran som initierar överföringsprocessen. Microsoft kan inte ingriper åt kunden eller den aktuella partnern. Kunden bör planera ett nära samarbete med framtida och aktuella partner för att säkerställa att övergången går smidigt.

## <a name="future-partner-tasks"></a>Framtida partneruppgifter 

Prenumerationens framtida partner måste fylla i ett formulär för överföringsbegäran från Partnercenter för att begära en prenumerationsöverföring:

1.  I den vänstra rutan i Partnercenter **väljer du Kunder** och sedan den kund som du vill slutföra överföringsbegäran för.
2.  På den kundspecifika menyn väljer du **Prenumerationer**.
3.  På fliken **Överföringsbegäranden** väljer du Lägg **till ny begäran:**

    :::image type="content" source="images/modernazuretransfers/Transferrequestheader.png" alt-text="Skärmbild som visar fliken Överföringsbegäranden.":::

5.  Fyll i **formuläret Ny överföringsbegäran:**

    :::image type="content" source="images/modernazuretransfers/CompleteTrnasferRequestForm.png" alt-text="Skärmbild som visar formuläret Ny överföringsbegäran.":::

6.  Välj **Skicka överföringsbegäran**  >  **Skicka**.

7.  Granska bekräftelsen av överföringsbegäran:

    :::image type="content" source="images/modernazuretransfers/TransferPending.png" alt-text="Skärmbild som visar en bekräftelse av överföringsbegäran.":::

    > [!NOTE]
    > Den framtida partnern kan avbryta  överföringsbegäran genom att välja Avbryt begäran i det övre högra hörnet i fönstret endast när statusen för överföringsbegäran är "väntande". När statusen för överföringsbegäran är "pågående" eller "klar" går det inte att avbryta.

## <a name="current-partner-tasks"></a>Aktuella partneruppgifter 

Den aktuella partnerns administratörsagent för kunden får ett e-postmeddelande om att en kund begär överföring av prenumerationer:

:::image type="content" source="images/modernazuretransfers/SourceReviewEmail.png" alt-text="Skärmbild som visar ett e-postmeddelande om en kundbegäran om överföring.":::

Den aktuella partnern måste granska och acceptera formuläret för överföringsbegäran från Partnercenter för att slutföra prenumerationsöverföringen.

> [!NOTE]  
> Om den aktuella partnern inte svarar inom 30 dagar går begäran ut och den framtida partnern behöver en för att skapa en ny överföringsbegäran.

1. Välj en av följande åtgärder: 
   - Välj **Granska överföringsbegäran i** e-postmeddelandet.

     eller

    - I den vänstra rutan i Partnercenter väljer **du Kunder** och sedan den kund som överföringsbegäran har skickats för.
      1. På den kundspecifika menyn väljer du **Prenumerationer**.
      1. På fliken **Överföringsbegäranden** expanderar du överföringsinformationen genom att välja **ID för överföringsbegäran** under **Mottagna begäranden:**

      :::image type="content" source="images/modernazuretransfers/ReviewRequest.png" alt-text="Skärmbild som visar fliken Överföringsbegäranden som visas av den aktuella partnern.":::

5. Granska överföringsbegäran. Välj de Azure-prenumerationer som ska överföras.
 
   Observera följande innan du fortsätter:
   - Du har inte längre åtkomst till de valda prenumerationerna.
   - Du faktureras inte för ytterligare användning.
   - Azure-reservationer överförs inte med prenumerationer.

6. Välj **Acceptera och överför** för att slutföra överföringsprocessen:

   :::image type="content" source="images/modernazuretransfers/SelectSubs.png" alt-text="Skärmbild som visar skärmen Granska överföringsbegäran.":::

   Om du har en kund med tidigare prenumerationer på Azure-erbjudanden (MS-AZR-0145p) fortsätter  du på samma sätt, väljer de prenumerationer som ska överföras och väljer sedan Godkänn och överför för att slutföra överföringsprocessen.

7. Visa bekräftelsen för överföringsgodkännande.

   Nu meddelar ett e-postmeddelande den framtida partnern, kunden och den aktuella partnern om den accepterade överföringsbegäran.

   När övergången har godkänts kan överföringsstatusen vara "väntande" i upp till 15 minuter medan systemet uppdateras. Om den här processen tar längre tid fortsätter systemet att försöka i tre dagar. Om överföringsstatusen är "väntande" längre än tre dagar ska partnern skicka en tjänstbegäran.

   När överföringen är klar visas prenumerationerna som ingår i begäran i Azure-planen för den framtida partnern. Den visas inte längre med den aktuella partnern.

>[!Note]  
>Indirekta leverantörer bör informera sina indirekta återförsäljare om att överföringsbegäran har godkänts.

### <a name="managing-your-transferred-customer-subscriptions"></a>Hantera dina överförda kundprenumerationer

Åtkomst till befintliga användare, grupper eller tjänsthuvudnamn som tilldelades via Azure RBAC påverkas inte under övergången. [Azure RBAC](/azure/role-based-access-control/overview) hjälper kunden att hantera vem som har åtkomst till Azure-resurser, vad de kan göra med dessa resurser och vilka områden de har åtkomst till. 

Som ny partner har du ingen RBAC-åtkomst till kundens resurser efter prenumerationsöverföringen. Kundens tidigare partner behåller RBAC-åtkomst. Samarbeta med kunden för att förstå vem som har insyn i prenumerationerna och hur du gör nödvändiga ändringar.

Kunden måste ta bort Azure RBAC-åtkomst för den tidigare partnern och lägga till åtkomst åt dig. Mer information om hur du ger åtkomst finns [i Vad är rollbaserad åtkomstkontroll i Azure (Azure RBAC)?](/azure/role-based-access-control/overview). Mer information om hur du tar bort åtkomst finns i [Ta bort en rolltilldelning.](/azure/role-based-access-control/role-assignments-portal#remove-a-role-assignment)

Dessutom får du inte automatiskt [AOBO-åtkomst (Admin on Behalf Of)](https://channel9.msdn.com/Series/cspdev/Module-11-Admin-On-Behalf-Of-AOBO) till dina prenumerationer. AOBO är nödvändigt så att du kan hantera kundens Azure-prenumerationer. Mer information om Azure-behörigheter finns [Få behörighet att hantera en kunds tjänst eller prenumeration](./customers-revoke-admin-privileges.md).

## <a name="next-steps"></a>Nästa steg

- [Azure RBAC](/azure/role-based-access-control/overview)
- [Få behörighet att hantera en kunds tjänst eller prenumeration](./customers-revoke-admin-privileges.md)
