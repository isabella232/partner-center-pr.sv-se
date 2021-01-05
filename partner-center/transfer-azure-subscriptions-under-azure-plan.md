---
title: Överför Azure-prenumerationen under en Azure-prenumeration till en annan CSP-partner
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Lär dig hur du ändrar program partner för Cloud Solution Provider som är associerad med en kunds Azure-prenumerationer under en Azure-plan.
ms.custom: SEOMAY.20
ms.localizationpriority: medium
author: mckennaville
ms.author: mcville
ms.date: 07/29/2020
ms.openlocfilehash: e792e4af2999924ba8be77ec0517ce56c1db7a27
ms.sourcegitcommit: ed5c873d19f0464cc986fe6e852383cd4280daf6
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 01/05/2021
ms.locfileid: "97893214"
---
# <a name="transfer-a-customers-azure-plan-subscriptions-to-a-different-partner"></a>Överföra en kunds Azure plan-prenumeration till en annan partner

**Lämpliga roller**

- Partner i CSP-programmet (Cloud Solution Provider)

Den här artikeln beskriver hur en kund kan byta sina Azure-prenumerationer under en Azure-plan från en leverantör av moln lösningar till en annan.

Följ dessa steg om du vill byta en kunds Azure-prenumeration från en annan partner. Både partnern och kunden har steg för att slutföra.

>[!Note]  
>Endast partner med en direkt fakturerings relation med Microsoft kan komma åt över gångs verktyget. Indirekta åter försäljare måste arbeta med sina indirekta leverantörer för att kunna utnyttja det här över gångs verktyget.

Kunden måste vara i konversation med båda partnerna (aktuella och framtida) innan det här verktyget utnyttjas. En offline-konversation måste ha för att undvika förvirring och omsättning. Dessutom bör partner och kunder förstå dessa överväganden och krav innan en över gång påbörjas:

**Viktiga överväganden:**

- Azure Reservations kommer inte att flyttas med prenumerationen till en kommande partner
- CSP-prissättning för Azure-tjänster under den aktuella partnern kommer inte att övergå  
- Support ansvar för kunden kommer att gå över till en kommande partner
- Fakturering och fakturering flyttas till framtida partner vid överförings tillfället
- Azure Role-Based Access Control (RBAC) påverkas inte av överföringen
- Admin på uppdrag av (ADMINISTRATE) beviljas inte som standard till den framtida partnern
- Marketplace-produkter från tredje part överförs så länge produkterna uppfyller kontroll av marknads platsens berättigande.
    - Det finns inga särskilda rabatter eller regionala begränsningar
    - Produkterna är icke-prenumerationer baserade
    - Den framtida partnern bör arbeta med utgivaren för att se till att de finns med i listan över tillåtna program för distribution av produkten
    - Om inte alla dessa villkor uppfylls för att överföra Marketplace-produkterna bör avbrytas de Azure-prenumerationer som överförs, och sedan köpa om Marketplace-produkter med den nya partnern

**Krav:**

- Kunden engagerar sig av den aktuella CSP-partnern i avsikt att övergå
- Framtida CSP-partner arbetar med kunden för att säkerställa att kundernas behov kan uppfyllas
- En framtida CSP-partner upprättar en relation med kunden och köper en Azure-plan innan över gången börjar  
- Kunden måste teckna Microsofts kund avtal med en framtida CSP-partner
- Den framtida CSP-partnern måste ha undertecknat Microsoft partner Agreement för att kunna använda det här verktyget

## <a name="customer-tasks-to-be-completed"></a>Kund uppgifter som ska utföras

För att överföra en Azure-prenumeration under en Azure-plan måste kunden starta processen genom att kontakta den aktuella partnern. De bör samla in sin nuvarande partner företags namn och domän så att deras framtids partner kan fylla i formuläret för överförings förfrågan för deras räkning.

Kunden måste också identifiera de prenumerationer som de vill överföra från sin aktuella partner. Du kan inte ändra partner för Office 365, Enterprise Mobility Suite eller Microsoft Dynamics CRM-prenumerationer.

>[!Note]  
>Det är den framtida partnerns ansvar att fylla i formuläret för överförings begäran som initierar överförings processen. Microsoft kan inte ingripa för kundens räkning eller den aktuella partnern. Kunden bör planera att samar beta med sin framtida och aktuella partner för att få över gången att gå smidigt.

## <a name="future-partner-tasks-to-be-completed"></a>Framtida partner aktiviteter som ska slutföras

Den framtida partnern av prenumerationen måste slutföra ett överförings förfrågnings formulär från Partner Center för att begära en prenumerations överföring:

1.  Från menyn Partner Center väljer du **kunder** och väljer sedan den kund som du vill slutföra ett överförings förfrågnings formulär för.
2.  Från menyn kund väljer du **prenumerationer**.
3.  Välj avsnittet **överförings förfrågan** .
4.  I **avsnittet överförings förfrågan** väljer du **Lägg till ny begäran**.

    :::image type="content" source="images/modernazuretransfers/Transferrequestheader.png" alt-text="Avsnittet överföringar":::

5.  Slutför det **nya formuläret för överförings förfrågan** .

6.  Välj **skicka begäran**  >  **Skicka** överföring.

    :::image type="content" source="images/modernazuretransfers/CompleteTrnasferRequestForm.png" alt-text="Slutför formulär för överförings förfrågan":::

7.  Granska bekräftelse av överförings förfrågan

    :::image type="content" source="images/modernazuretransfers/TransferPending.png" alt-text="Granska väntande överföring":::

    >[!Note]
    >Den framtida partnern kan avbryta överföringsbegäran genom att välja **Cancel Request** i det övre högra hörnet endast när status för överförings förfrågan är "väntar". När statusen för överförings förfrågan är "pågående" eller "slutförd" går det inte att avbryta.

## <a name="current-partner-tasks-to-be-completed"></a>Aktuella partner aktiviteter som ska slutföras

Den aktuella partnerns administratörs agent för kunden får ett e-postmeddelande om att deras kund begär en överföring av sina prenumerationer:

:::image type="content" source="images/modernazuretransfers/SourceReviewEmail.png" alt-text="Genomgång":::

Granska och Godkänn formuläret för överförings förfrågan från Partner Center för att slutföra prenumerations överföringen.

>[!Note]  
>Om ingen åtgärd vidtas av den aktuella partnern inom 30 dagar upphör begäran att gälla och den framtida partnern kommer att ha en för att skapa en ny överförings förfrågan.

1.  Välj **Granska överförings förfrågan** från e-postmeddelandet eller
1.  Från menyn Partner Center väljer du **kunder** och väljer sedan den kund som en överföringsbegäran har skickats åt för.
2.  Från menyn kund väljer du **prenumerationer**.
3.  Välj avsnittet **överförings förfrågan** .
4.  Expandera överförings information genom att välja det valda **överföringsbegäran-ID: t** under **mottagna begär Anden**

:::image type="content" source="images/modernazuretransfers/ReviewRequest.png" alt-text="Begäran om käll gransknings överföring":::

5.  Granska överförings förfrågan. Välj de begärda Azure-prenumerationerna som ska överföras.

>[!Note]  
> Innan du fortsätter bör du tänka på följande: du kommer inte längre att ha åtkomst till de valda prenumerationerna.
> Du kommer inte att faktureras för ytterligare användning.
> Azure-reservationer överförs inte med prenumerationerna.

6.  Välj sedan **Godkänn och överför** för att slutföra överförings processen.

:::image type="content" source="images/modernazuretransfers/SelectSubs.png" alt-text="Välj prenumerationer som ska överföras under dina Azure-planer":::

7.  Visa bekräftelse av godkännande av överföring.

   I det här läget meddelas den framtida partnern, kunden och den aktuella partnern om den godkända överföringsbegäran via e-post.

   Efter att över gången har godkänts kan överförings statusen vara väntande i upp till 15 minuter medan systemet uppdateras. Om det tar längre tid fortsätter systemet att försöka i tre dagar. Om överförings statusen fortfarande är väntande bör partnern skicka en tjänstbegäran.

   När överföringen är klar visas de prenumerationer som ingår i förfrågan i Azure-planen för den framtida partnern och visas inte längre med dig.

>[!Note]  
>För indirekta leverantörer: informera din indirekta åter försäljare att överföringsbegäran har accepterats.

### <a name="managing-your-transferred-customer-subscriptions"></a>Hantera dina överförda kund prenumerationer
- Åtkomst till befintliga användare, grupper eller tjänsthuvudnamn som tilldelades med hjälp av Azure RBAC (rollbaserad åtkomstkontroll) påverkas inte under övergången. Azure rollbaserad åtkomst kontroll [(Azure RBAC)](/azure/role-based-access-control/overview) hjälper din kund att hantera vem som har åtkomst till Azure-resurser, vad de kan göra med dessa resurser och vilka områden de har åtkomst till. Som den nya partnern får du inga RBAC-åtkomst till kundens resurser efter prenumerations överföringen. Din kunds tidigare partner behåller sin RBAC-åtkomst. Arbeta med kunden för att förstå vem som har insikt i sina prenumerationer och hur du gör de ändringar som önskas.

- Det är därför viktigt att kunden tar bort Azure RBAC-åtkomst för sin tidigare partner och lägger till åtkomst för den nya partnern. Mer information om din kund ger ny åtkomst finns i [Vad är Azures rollbaserad åtkomst kontroll (Azure RBAC)?](/azure/role-based-access-control/overview) Mer information om din kund som tar bort din tidigare partners RBAC-åtkomst finns i [ta bort en roll tilldelning](/azure/role-based-access-control/role-assignments-portal#remove-a-role-assignment).

- Dessutom får du inte automatiskt [Administratörer på uppdrag av (administrate)](https://channel9.msdn.com/Series/cspdev/Module-11-Admin-On-Behalf-Of-AOBO) åtkomst till dina prenumerationer. ADMINISTRATE krävs för att partner ska kunna hantera sina kunders Azure-prenumerationer för deras räkning. Mer information om Azure-behörigheter finns i [Hämta behörigheter för att hantera en kunds tjänst eller prenumeration.](./customers-revoke-admin-privileges.md)

## <a name="next-steps"></a>Nästa steg:

- [(Azure RBAC)](/azure/role-based-access-control/overview)
- [Få behörighet att hantera en kunds tjänst eller prenumeration.](./customers-revoke-admin-privileges.md)
