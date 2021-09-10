---
title: Livscykelhantering för SaaS-prenumeration (Programvara som en tjänst)
description: Livscykelhantering för SaaS-prenumeration (Programvara som en tjänst) i Azure Marketplace.
ms.service: marketplace
ms.subservice: partnercenter-marketplace-publisher
ms.topic: conceptual
ms.date: 08/20/2021
ms.author: yonits
author: yonits
ms.openlocfilehash: fed2b2f7b951a7dc6ee16fb126f3f5f774df18c9
ms.sourcegitcommit: 1161d5bcb345e368348c535a7211f0d353c5a471
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/09/2021
ms.locfileid: "123936991"
---
# <a name="saas-subscription-lifecycle-management"></a>Livscykelhantering för SaaS-prenumeration

Den här artikeln beskriver hur du identifierar en SaaS-resurs, skillnaderna mellan SaaS och SaaS Classic och SaaS-resurshantering i Azure Portal.

## <a name="find-a-saas-resource"></a>Hitta en SaaS-resurs

När du köper ett SaaS-erbjudande från Azure Marketplace skapas en SaaS-prenumeration (programvara som en tjänst) i Azure Portal (mer information finns i Köpa ett [SaaS-erbjudande i Azure Portal](purchase-saas-offer-in-azure-portal.md)). Så här hittar du en SaaS-resurs i portalen:

- **Fönstret Global sökning** (överst) – Sök efter din SaaS-prenumeration efter namn.
- **SaaS** – visar en lista över alla dina SaaS-prenumerationer. Det finns två typer av SaaS-listor: se följande avsnitt.
- **Prenumerationer** – Visar en lista över alla Azure-prenumerationer som du har åtkomst till som en del av din klientorganisation. Om du vill hitta en viss prenumeration använder du filter- eller sökfönstret.
- **Alla resurser** – Visar en lista över alla resurser som skapats under alla prenumerationer som du har åtkomst till. Om du vill hitta en viss prenumeration använder du filtret (skriv > SaaS) eller söker i listan.

## <a name="differences-between-saas-and-saas-classic-lists-of-resources-in-the-azure-portal"></a>Skillnader mellan den klassiska SaaS- och SaaS-listan över resurser i Azure Portal

Skillnaden mellan dessa två typer är att med SaaS Classic kan du hitta SaaS-prenumerationer som har skapats under din klientorganisation och inte under en resursgrupp.
Om du har köpt en SaaS-prenumeration i Azure Portal före februari 2021 skapades den under din klientorganisation och du hittar den under SaaS Classic. Alla inköp som görs i Microsoft AppSource finns i den här listan.

Om du har köpt en SaaS-prenumeration i Azure Portal före februari 2021 och vill flytta den från under klientorganisationen till en resursgrupp (rekommenderas) går du till SaaS-prenumerationen i avsnittet **Klassisk SaaS** och väljer Flytta **till resursgrupp.** Du kan bara flytta prenumerationer i **tillståndet Väntar** **eller** Aktiv. När saaS-prenumerationen har flyttats visas den nu i **SaaS-vyn,** inte **i Den klassiska SaaS-vyn.** Du kan inte flytta en SaaS-prenumeration till en resursgrupp om den köptes i AppSource.

Flytten ger följande fördelar:

- Förbättrad åtkomst till och kontroll av din SaaS-resurs med ärvda principer och behörigheter från Azure-prenumerationen och resursgrupper (fullständig RBAC-kontroll)
- SaaS-livscykeln är kopplad till Azure-prenumerationens livscykel för åtgärder som överföringar och borttagningar
- Enklare identifiering med SaaS-resurser som hittas med hjälp av global sökning
- Användning av Azure Cost Management – Övervaka utgifter för SaaS-resurser
- Resurser på prenumerationsnivå har resurshändelser i aktivitetsloggen

## <a name="manage-your-saas-service"></a>Hantera saaS-tjänsten

Det finns flera sätt att hantera dina SaaS-prenumerationer

* För SaaS-prenumerationer som köpts i Azure Portal hanterar du dem där.
* För SaaS-prenumerationer som köpts i AppSource hanterar du dem i Azure Portal och [Microsoft 365 Admin Center;](https://admin.microsoft.com/Adminportal/Home?#/subscriptions) Mer information om hur du använder Microsoft 365 Admin Center finns [i Hantera appprenumerationer från tredje part för din organisation.](/microsoft-365/commerce/manage-saas-apps?view=o365-worldwide&preserve-view=true)
* Med vissa utgivare kan du hantera SaaS-prenumerationer direkt på deras plattform. Besök utgivarens webbplats med hjälp av en länk på SaaS-prenumerationssidan i Azure Portal.

Det finns flera åtgärder som du kan vidta efter köpet: vissa kräver behörighet som ägare eller deltagare:

### <a name="change-plans"></a>Ändra planer

Ändringar som du gör i en plan som du prenumererar på börjar gälla omedelbart. Faktureringen kommer att ske enligt faktureringsperioden för den aktuella planen. Ändring av planer kräver **behörighet som** ägare **eller** deltagare.

> [!NOTE]
> Utgivaren kan neka att godkänna ändringen om de ändringar du väljer inte är möjliga i tjänsten. I det här fallet misslyckas ändringen.

Det finns vissa fall när **ändringsplanen** kanske inte fungerar:

- Om din prenumeration finns på klientorganisationsnivå **med läsbehörighet** kan du inte ändra planen. I det här fallet begär du behörighet från den person som **har rollen** Ägare för prenumerationen.
- Om det inte finns något betalningsmedel (PI) associerat med Azure-prenumerationen kan du inte ändra din kostnadsfria plan till en betald plan. Du kan dock välja en annan Azure-prenumeration och sedan välja en betald plan eller lägga till en PI i den valda Azure-prenumerationen.
- Om den plan som du valde har en begränsning för lägsta/högsta användare som inte inkluderar det aktuella antalet användare, väljer du en annan plan med samma antal användare som ingår i det ursprungliga abonnemanget som du köpte eller kontaktar utgivaren.
- Om utgivaren inte kan uppfylla begäran kontaktar du den direkt.

### <a name="change-number-of-users"></a>Ändra antal användare

För platsbaserade planer kan du lägga till eller minska antalet användare som du definierade under inköpsprocessen. Om du ändrar antalet användare som du prenumererar på börjar faktureringen gälla omedelbart och faktureringen faktureras enligt faktureringsperioden för den aktuella planen. Ändringar i platser är endast möjliga inom det lägsta och högsta antalet platser enligt utgivarens definition. I vissa fall måste du ändra en plan innan du byter plats, och vice versa.

- Om din prenumeration finns på klientorganisationsnivå med läsbehörighet kan du inte ändra antalet användare. I stället begär du deltagarbehörighet från den person som har rollen Ägare för prenumerationen.
- Om utgivaren inte kan uppfylla begäran kontaktar du den direkt.

> [!NOTE]
> Utgivaren kan neka att godkänna ändringen om det inte är möjligt i tjänsten. I det här fallet misslyckas ändringen.

### <a name="edit-recurring-billing"></a>Redigera återkommande fakturering

Med återkommande fakturering kan du hantera förnyelsen av saaS-prenumerationen. När återkommande fakturering är inaktiverat avslutas SaaS-prenumerationen och SaaS-tjänsten på förnyelsedatumet. Du kan bara ändra förnyelsealternativet när prenumerationen är aktiv. En avslutad och/eller avbruten SaaS-prenumeration kan inte återaktiveras. en ny SaaS-prenumeration måste skapas i dess ställe.

### <a name="view-billing"></a>Visa fakturering

Visa fakturor för din Azure-prenumeration och Azure Marketplace produkter som köpts med den här prenumerationen. För SaaS som köpts i portalen går du till faktureringssidan  på sidan SaaS-prenumeration i avsnittet Fakturering, som omdirigerar dig till **Cost Management**.

Cost Management hjälper dig att förstå din fakturauppdelning, hantera ditt faktureringskonto och dina prenumerationer, övervaka/kontrollera Azure-utgifter och optimera resursanvändningen. Med den kan du analysera kostnader, skapa och hantera budgetar med mera. Du kan till exempel spåra din anpassade mätaranvändning (för SaaS-prenumerationer som skapats efter februari 2021 eller flyttats till en resursgrupp). Läs mer om kostnadshantering i [dokumentationen Azure Cost Management + Billing .](/azure/cost-management-billing/)

Om köpet har gjorts via Microsoft AppSource kan du visa dina fakturor i Microsoft Admin Center under **Fakturor & betalningar.**

### <a name="cancel-subscription"></a>Avbryt prenumerationen

Om du avbryter tas din åtkomst till den programvara som du har köpt som en del av den här SaaS-prenumerationen bort. Återbetalningar bearbetas enligt återbetalningsprincipen. Mer information finns i [Återbetalningsprinciper för Microsoft AppSource och Azure Marketplace](refund-policies.md).

Om din prenumeration finns på klientorganisationsnivå **med läsbehörighet** kan du inte avbryta en prenumeration. Kontakta i stället personen med **ägarbehörighet.**

Om du har haft en månatlig SaaS-prenumeration i mer än 24 timmar eller en års- eller flerårsprenumeration under mer än 14 dagar kommer ingen återbetalning att användas för prenumerationens aktuella period (se annulleringsprincip). Fakturering baserat på förbrukning efter att ett SaaS-konto har konfigurerats är inte heller berättigat till återbetalning.

### <a name="delete-subscription"></a>Ta bort prenumeration

Den här åtgärden är som att avbryta, med tillägget att ta bort SaaS-resursen från din lista över SaaS-prenumerationer. När du har tagit bort en prenumeration kan du inte komma åt den från Azure Portal.

Om din prenumeration finns på klientorganisationsnivå **med läsbehörighet** kan du inte ta bort en prenumeration. Kontakta i stället personen med **ägarbehörighet.**

### <a name="change-azure-subscription-andor-resource-group"></a>Ändra Azure-prenumeration och/eller resursgrupp

Så här ändrar du en prenumeration/resursgrupp som är associerad med ett erbjudande som har köpts i Azure Portal:

1. Gå till **SaaS-avsnittet.**
2. Välj den prenumeration som ska ändras.
3. Under **Fakturering** väljer du **Ändra fakturerad prenumeration.**
4. Välj önskad prenumeration/resursgrupp eller skapa en ny resursgrupp att flytta SaaS-resursen till.
5. Välj **Ändra** längst ned för att slutföra processen.

Det finns vissa fall när ändringen kanske inte fungerar:

- Om saaS-prenumerationen inte har statusen Prenumerera kontrollerar du prenumerationstillståndet i SaaS-avsnittet eller på **saaS-prenumerationssidan.**
- Om SaaS-prenumerationen är en resurs på klientorganisationsnivå:
    - Du bör ha *ägar-/deltagarbehörighet* för Azure-målprenumerationen.
- Om SaaS-prenumerationen är en resurs på prenumerationsnivå:
    - Du måste *ha läs-* *eller ägar-/deltagarbehörighet* till Azure-målprenumerationen.
    - Du behöver *ägar-/deltagarbehörighet* för målresursgruppen.
    - Om det redan finns en SaaS-prenumeration med samma namn i målresursgruppen väljer du en annan målresursgrupp.
- Azure-målprenumerationen och resursprenumerationen genomgår alla kontroller som utförs under köpet. Mer information om köpkontroller finns i avsnittet [SaaS-prenumeration och saaS-konfiguration](purchase-saas-offer-in-azure-portal.md#saas-subscription-and-configuration) i Köpa **ett SaaS-erbjudande i Azure Portal**.

## <a name="next-steps"></a>Nästa steg

- Om du redan har köpt ett erbjudande på Marketplace går du [till Fakturering](billing-invoicing.md)
- Läs mer om [alternativ för privat](private-offers.md) plan
