---
title: Ge kunderna behörighet att köpa sina egna produkter och tjänster
description: Lär dig hur CSP-programpartner kan låta kunder köpa sina egna tjänster, till exempel Azure-reservationer, för en prenumeration som köpts åt dem i Partnercenter.
ms.topic: how-to
ms.date: 09/27/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-customers
author: amitravat
ms.author: amrava
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 8bcaae55bdef9971fa111328a004f1ddb0192030
ms.sourcegitcommit: e1da62b36420d78bf44e3962358d0af65ebc3402
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/27/2021
ms.locfileid: "129089138"
---
# <a name="give-customers-permissions-to-buy-their-own-products-and-services"></a>Ge kunderna behörighet att köpa sina egna produkter och tjänster

**Lämpliga roller:** Administratörsagent | Försäljningsagent

Den här artikeln visar hur en partner i Molnlösningsleverantör-programmet (CSP) kan ge en kund tillstånd att köpa några av sina egna tjänster eller resurser.

Partner i CSP-programmet använder ofta PartnerCenter och dess kommersiella marknadsplats för att köpa lösningar och tjänster för sina kunder. Partner låter sedan vissa kunder etablera dessa tjänster själva direkt från Azure Portal.

Här är ett exempel. Anta att du köper en Azure-planprenumeration för en kund i Partnercenter. Sedan bestämmer du dig för att lägga till andra resurser eller tjänster i prenumerationen för kundens räkning. I det här fallet kan du lägga till Azure-reservationer i kundens prenumeration (till exempel lägga till reserverade instanser av virtuella datorinstanser). Du kan sedan tillåta kunden att ytterligare etablera Azure-reservationsresurserna själva i Azure Portal.

Med funktionen **Kundbehörigheter kan** du nu ge kunderna fler självbetjäningsalternativ med Azure-resurser. Genom att aktivera behörigheter för kunden kan du låta kunderna köpa sina egna resurser (till exempel köpa sina egna Azure-reservationer).  

## <a name="overview-of-customer-permissions-in-partner-center"></a>Översikt över kundbehörigheter i Partnercenter

Använd sidan **Kundkonto** för att aktivera (eller inaktivera) kundbehörigheter. Den här funktionen stöder för närvarande:

- **Azure-reservationer:** Genom att aktivera den här behörigheten kan kunden köpa sina egna Azure-reservationer för en specifik Azure-prenumeration som du har köpt för dem.

Observera följande viktiga punkter innan du aktiverar kundbehörigheter:

- Som standard inaktiveras kundbehörigheter automatiskt (inaktiverat) i Partnercenter.

- Innan du kan aktivera (eller inaktivera) behörigheter för en kund måste du tilldelas rollen som administratörsagent i Partnercenter.

  Partner som tilldelats rollen Försäljningsagent eller Supportagent har skrivskyddad åtkomst och kan inte aktivera eller inaktivera kundbehörigheter.

- Du kan aktivera (aktivera) behörigheter för alla kunder som du väljer.

- Du kan aktivera (eller inaktivera) kundbehörigheter med hjälp av Partnercenter-instrumentpanelen eller [Partnercenter-API:er.](/partner-center/develop/manage-customers)

- När du aktiverar (aktiverar) behörigheter för en specifik kund är du ansvarig för att betala för efterföljande köp som görs av kunden. Om kunderna vill byta, avbryta eller förnya ett köp som de har gjort (eller om de vill ändra den ursprungliga omfattningen för en reservation) kan de inte göra det själva. De måste be dig som partner att hjälpa dem att byta, avbryta och förnya inköp eller göra senare ändringar i en reservations omfång.  

- När du aktiverar behörigheter för en specifik kund meddelas **du** inte om senare köp som görs av kunden.

- Senare köp som görs av kunden visas i Partnercenter tillsammans med eventuella inköp som görs av dig. Du hittar dessa inköp på kundens sida för **orderhistorik,** på sidan **Reservationer** eller i [**aktivitetsloggen**](activity-logs.md).

> [!NOTE]
> Information om priser som kunden betalar och hur du hjälper kunder att hantera sina inköp finns i [Hjälpa kunder att hantera reservationer som de köper.](give-customers-permission.md#help-customers-manage-reservations-they-purchase)

## <a name="give-customers-permission-to-buy-their-own-azure-reservations"></a>Ge kunderna behörighet att köpa sina egna Azure-reservationer

Azure-reservationer är ett bra sätt att köpa Azure-tjänster till ett rabatterat pris. Mer information om fördelarna med Azure-reservationer finns i [Vad är Azure-reservationer?](/azure/cost-management-billing/reservations/save-compute-costs-reservations)

Nu har du möjlighet att köpa Azure-reservationer åt dina kunder, vilket du kanske redan har gjort. Eller så kan du ge kunderna behörighet att köpa sina egna Azure-reservationer.

> [!NOTE]
> När du har gett kunderna behörighet att köpa sina egna Azure-reservationer kan du hjälpa dem att hantera eventuella reservationer som de köper. Mer information finns i Hjälpa [kunder att hantera reservationer som de köper.](give-customers-permission.md#help-customers-manage-reservations-they-purchase)

### <a name="to-enable-customers-to-buy-their-own-azure-reservations"></a>Så här gör du det möjligt för kunder att köpa egna Azure-reservationer

1. Kontrollera att kunden har en befintlig Azure-plan eller Azure Global-prenumeration som du har köpt för kundens räkning.

2. Kontrollera att kunden har tilldelats rollen **Ägare för** den här prenumerationen.

3. Aktivera kundbehörigheter (aktivera den här **funktionen)** för att köpa sina egna Azure-reservationer.

Varje steg visas nedan.

### <a name="verify-the-customer-has-an-existing-azure-subscription"></a>Kontrollera att kunden har en befintlig Azure-prenumeration

Innan du ger kunderna behörighet att köpa sina egna Azure-reservationer måste du kontrollera att kunden har en befintlig Azure-plan eller en global Azure-prenumeration. Om kunden inte visar någon aktuell Azure-prenumeration i Partnercenter måste du köpa en prenumeration för dem innan du aktiverar deras kundbehörigheter.

- Om du vill se om en kund redan har en Azure-prenumeration går du till [partnercenterkundlistan](https://partner.microsoft.com/commerce/customers/list) och väljer den specifika kunden i listan. Välj sedan **Prenumerationer** och leta efter användningsbaserade prenumerationer för antingen Azure-plan eller Azure Global.

- Om en kund inte har en befintlig Azure-prenumeration kan du köpa en prenumeration åt dem. Se [Köpa Azure-planen.](purchase-azure-plan.md)

### <a name="verify-the-customer-has-been-assigned-the-correct-role-in-azure"></a>Kontrollera att kunden har tilldelats rätt roll i Azure

När du har verifierat att kunden har en befintlig Azure-prenumeration måste du också  kontrollera att nyckelanvändarna som är kopplade till kunden har tilldelats rätt ägarroll för den Azure-prenumerationen. Det här är den rollbaserade åtkomst (RBAC) som kunden behöver för att köpa Azure-reservationer för en Azure-prenumeration som du har köpt.

Vissa partner kan redan ha tilldelat rollen **Ägare** till kunder som aktivt vill hantera och etablera sina egna Azure-resurser. Om du redan har tilldelat **ägarstatus** till en kund för att hantera tidigare prenumerationer som du har köpt för dem kan du hoppa över det här steget.  

> [!IMPORTANT]
> Om en kund inte har tilldelats rollen **Ägare** får han eller hon ett felmeddelande i Azure Portal hindrar dem från att köpa Azure-reservationer.

Så här kontrollerar du att kunden har tilldelats **rollen Ägare** för en Azure-prenumeration:

> [!NOTE]
> Mer information om gränssnittet för arbetsytor finns i [Getting around Partner Center (Ta sig runt i Partnercenter).](get-around-partner-center.md#turn-workspaces-on-and-off)

#### <a name="workspaces-view"></a>[Vyn Arbetsytor](#tab/workspaces-view)

1. Logga in på instrumentpanelen i [Partnercenter.](https://partner.microsoft.com/dashboard)

2. Välj panelen **Kunder** och välj sedan den specifika kunden.

3. Välj **Prenumerationer** för kunden och leta upp den specifika Azure-prenumerationen.

4. Välj **knappen** Hantera bredvid kundens prenumeration. När du gör det öppnas [Azure Portal](https://portal.azure.com/).

5. Om du vill **tilldela** rollen Ägare till en specifik användare följer du de här stegen [för att tilldela en användare som administratör.](/azure/cost-management-billing/manage/add-change-subscription-administrator#to-assign-a-user-as-an-administrator)

#### <a name="current-view"></a>[Aktuell vy](#tab/current-view)

1. Logga in på instrumentpanelen i [Partnercenter.](https://partner.microsoft.com/dashboard)

2. Välj **CSP**, sedan **Kunder** och välj den specifika kunden.

3. Välj **Prenumerationer** för kunden och leta upp den specifika Azure-prenumerationen.

4. Välj **knappen** Hantera bredvid kundens prenumeration. När du gör det öppnas [Azure Portal](https://portal.azure.com/).

5. Om du vill **tilldela** rollen Ägare till en specifik användare följer du de här stegen [för att tilldela en användare som administratör.](/azure/cost-management-billing/manage/add-change-subscription-administrator#to-assign-a-user-as-an-administrator)

* * *

### <a name="turn-on-or-turn-off-customer-permissions-to-purchase-their-own-azure-reservations"></a>Aktivera eller inaktivera kundbehörigheter för att köpa egna Azure-reservationer

När du har verifierat att kunden har  en befintlig Azure-prenumeration och användarna har tilldelats rollen Ägare för prenumerationen är du redo att aktivera (aktivera) kundbehörigheter. Du kan också använda de här stegen för att stänga av (inaktivera) kundbehörigheter. Du kan aktivera eller inaktivera kundbehörigheter med hjälp av Partnercenter-instrumentpanelen eller [Partnercenter-API:er.](/partner-center/develop/manage-customers)

Så här aktiverar eller inaktiverar du kundbehörigheter i Partnercenter:

> [!NOTE]
> Mer information om gränssnittet för arbetsytor finns i [Getting around Partner Center (Ta sig runt i Partnercenter).](get-around-partner-center.md#turn-workspaces-on-and-off)

#### <a name="workspaces-view"></a>[Vyn Arbetsytor](#tab/workspaces-view)

1. Logga in på instrumentpanelen i [Partnercenter.](https://partner.microsoft.com/dashboard)

2. Välj panelen **Kunder** och välj sedan en specifik kund.

3. Välj **Konto** på kundmenyn. Sidan **Kundkonto** visas.

4. Leta upp **området Kundbehörigheter** längst ned på sidan.

   :::image type="content" source="images/give-customers-permission-reservations.png" alt-text="Kundbehörigheter på kontosidan." border="true":::

5. Under **Azure-reservationer** letar du **upp alternativet Tillåt kund att** köpa.

6. Om du vill aktivera kundbehörigheter flyttar du växeln bredvid det här alternativet till **läget På.** Om du vill inaktivera kundbehörigheter flyttar du växeln till **läget Av.**

> [!NOTE]
> Mer information om vad som händer när du aktiverar en kunds behörighet att köpa egna Azure-reservationer finns i [Översikt över kundbehörigheter i Partnercenter.](give-customers-permission.md#overview-of-customer-permissions-in-partner-center)
>
> När du aktiverar (eller inaktiverar) kundbehörigheter registrerar aktivitetsloggen varje åtgärd. (Den här loggen är tillgänglig när du väljer kugghjulsikonen överst på Partnercenter-instrumentpanelen). När du aktiverar eller inaktiverar kundbehörigheter  visas åtgärden antingen som Skapa kundinköpsbehörigheter eller Ta bort **kundinköpsbehörigheter** i aktivitetsloggen.

#### <a name="current-view"></a>[Aktuell vy](#tab/current-view)

1. Logga in på instrumentpanelen i [Partnercenter.](https://partner.microsoft.com/dashboard)

2. I den vänstra navigeringsmenyn väljer **du CSP** och sedan **Kunder**. En kundlista visas.

3. Välj ett specifikt kundnamn.

4. Välj **Konto** på kundmenyn. Sidan **Kundkonto** visas.

5. Leta upp **området Kundbehörigheter** längst ned på sidan.

   :::image type="content" source="images/give-customers-permission-reservations.png" alt-text="Kundbehörigheter på kontosidan." border="true":::

6. Under **Azure-reservationer** letar du **upp alternativet Tillåt kund att** köpa.

7. Om du vill aktivera kundbehörigheter flyttar du växeln bredvid det här alternativet till **läget På.** Om du vill inaktivera kundbehörigheter flyttar du växeln till **läget Av.**

> [!NOTE]
> Mer information om vad som händer när du aktiverar en kunds behörighet att köpa egna Azure-reservationer finns i [Översikt över kundbehörigheter i Partnercenter.](give-customers-permission.md#overview-of-customer-permissions-in-partner-center)
>
> När du aktiverar (eller inaktiverar) kundbehörigheter registrerar aktivitetsloggen varje åtgärd. (Den här loggen är tillgänglig när du väljer kugghjulsikonen överst på Partnercenter-instrumentpanelen). När du aktiverar eller inaktiverar kundbehörigheter  visas åtgärden antingen som Skapa kundinköpsbehörigheter eller Ta bort **kundinköpsbehörigheter** i aktivitetsloggen.

* * *

## <a name="help-customers-manage-reservations-they-purchase"></a>Hjälpa kunder att hantera reservationer som de köper

När du ger kunderna behörighet att köpa sina egna Azure-reservationer kan du hjälpa dem att bättre hantera de resurser de köper. Kunder kan själva hantera många aspekter av Azure-reservationer direkt från [Azure Portal](https://portal.azure.com/). De behöver din hjälp med att hantera några andra aspekter av Azure-reservationer som de köper i din CSP-prenumeration.  

Hjälp kunderna att förstå mer om att hantera dessa aspekter av Azure-reservationer:

- Priser som kunder betalar för Azure-reservationer
- Hur kunder kan optimera användningen av Azure-reservationer
- Vad händer när kunder köper reservationer med ett delat omfång?
- Vad händer om kunder vill ändra, avbryta och förnya en reservation eller ändra dess omfång?

**Priser som kunder betalar för sina reservationer.** Kunden kommer att köpa Azure-reservationer baserat på en prenumeration som du tidigare har köpt för dem i faktureringskontot för din CSP-partner. Kundens pris för eventuella Azure-reservationer som de köper baserat på den här prenumerationen anges också av dig. Det här priset kan vara något annat än det Web Direct-pris som kunden ser i Azure Portal.

**Hur kunder kan optimera sin användning av en reservation.** Vissa kunder kan ha nytta av att lära sig mer om hur de optimerar sin användning av en reservation eller hur de tilldelar en reservation första omfånget under köpet. Mer information finns i Hantera reservationer för [Azure-resurser.](/azure/cost-management-billing/reservations/manage-reserved-vm-instance)

**Vad händer när en kund köper en reservation med ett delat omfång?** När kunder köper en reservation baserat på en tidigare CSP-prenumeration och tilldelar ett delat omfång till reservationen gäller eventuella rabatter som kunden har fått av CSP:en för matchande användning för alla prenumerationer som CSP-partnern har köpt för kunden.

**Vad ska kunder göra om de vill byta ut, avbryta eller förnya ett köp som de har gjort eller ändra den ursprungliga omfattningen för en reservation?** Kunder måste be sin partner att hjälpa dem att ändra en reservations ursprungliga omfång. De behöver också en partners hjälp med att byta, avbryta eller förnya en reservation. De kan inte utföra dessa uppgifter själva med reservationer baserat på prenumerationer som köpts åt dem av en CSP-partner.

## <a name="next-steps"></a>Nästa steg

- [Köpa Azure-reservationer åt dina kunder](azure-reservations-buying.md)

- [PartnerCenter – Sälja Microsoft-reservationer](azure-reservations.md)

- [Hantera Azure-reservationer åt dina kunder](azure-reservations-manage.md)