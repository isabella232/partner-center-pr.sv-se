---
title: Låt kunderna köpa sina egna tjänster i CSP
description: Lär dig hur CSP-programpartner kan låta kunderna köpa sina egna tjänster, t. ex. Azure-reservationer, för en prenumeration som köpts för dem i Partner Center.
ms.topic: how-to
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: amitravat
ms.author: amrava
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 4feaa8cba8ba17f553b5e936dcf892ffbf7ccc82
ms.sourcegitcommit: 3c26a61982082787bbdaf5d1e92553b26f3a5076
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/06/2021
ms.locfileid: "106441310"
---
# <a name="give-customers-permission-in-partner-center-to-buy-their-own-products-or-services"></a>Ge kunderna tillstånd i Partner Center att köpa sina egna produkter eller tjänster

**Lämpliga roller**

- Administratörs agent
- Försäljnings agent

Den här artikeln visar hur en partner i ett CSP-program (Cloud Solution Provider) kan ge en kund behörighet att köpa vissa av sina egna tjänster eller resurser.

Partner i CSP-programmet använder ofta Partner Center och dess kommersiella marknads plats för att köpa lösningar och tjänster för sina kunder. Partner gör det möjligt för vissa kunder att etablera dessa tjänster direkt från Azure Portal.

Här är ett exempel. Anta att du köper en Azure plan-prenumeration för en kund i Partner Center. Sedan bestämmer du dig för att lägga till andra resurser eller tjänster i prenumerationen på kundens räkning. I det här fallet kan du lägga till Azure-reservationer till kundens prenumeration (till exempel lägga till reserverade virtuella dator instanser). Du kan sedan tillåta kunden att ytterligare etablera Azure reservations resurserna själva i Azure Portal.

Med funktionen **kund behörigheter** ger du nu kunderna fler självbetjänings alternativ med Azure-resurser. Genom att aktivera behörighet för kunden kan kunderna köpa sina egna resurser (till exempel genom att köpa sina egna Azure-reservationer).  

## <a name="overview-of-customer-permissions-in-partner-center"></a>Översikt över kund behörigheter i Partner Center

Använd sidan kund **konto** för att aktivera (eller inaktivera) kund behörigheter. Den här funktionen stöder för närvarande:

- **Azure-reservationer:** Genom att aktivera den här behörigheten kan kunden köpa sina egna Azure-reservationer för en specifik Azure-prenumeration som du har köpt för dem.

Observera följande viktiga punkter innan du aktiverar kund behörigheter:

- Som standard inaktive ras kund behörigheter automatiskt (inaktiverat) i Partner Center.

- Innan du kan aktivera (eller inaktivera) behörigheter för en kund måste du ha tilldelats rollen som administratörs agent i Partner Center.

  Partners tilldelade rollen som försäljnings agent eller supportavdelningen har skrivskyddad åtkomst och kan inte aktivera eller inaktivera kund behörighet.

- Du kan aktivera (aktivera) behörigheter för alla kunder du väljer.

- Du kan aktivera (eller inaktivera) kund behörigheter med hjälp av instrument panelen för partner Center eller [API: er för partner Center](/partner-center/develop/manage-customers).

- När du har aktiverat (aktivera) behörigheter för en specifik kund ansvarar du för att betala för eventuella efterföljande köp som görs av kunden. Om kunderna vill byta ut, säga upp eller förnya ett köp som de har gjort (eller vill ändra det ursprungliga omfånget för en reservation), kan de inte göra det själva. De behöver fråga dig, som partner, för att hjälpa dem att utbyta, avbryta och förnya inköp, eller göra senare ändringar i en reservations omfattning.  

- När du har aktiverat behörigheter för en specifik kund kommer du **inte att** meddelas om eventuella senare köp som kunden har gjort.

- Senare köp som görs av kunden kommer att visas i Partner Center tillsammans med eventuella köp som du har gjort. Du hittar dessa inköp på kundens **order historik** sida, på sidan **reservation** eller i [**aktivitets loggen**](activity-logs.md).

>[!NOTE]
> För information om priser som kunden betalar och hur de kan hjälpa kunder att hantera sina inköp, se [Hjälp kunderna att hantera reservationer som de köper](give-customers-permission.md#help-customers-manage-reservations-they-purchase).

## <a name="give-customers-permission-to-buy-their-own-azure-reservations"></a>Ge kunderna tillstånd att köpa sina egna Azure-reservationer

Azure-reservationer är ett bra sätt att köpa Azure-tjänster till ett rabatterat pris. Läs mer om fördelarna med Azure-reservationer i [Vad är Azure reservations?](/azure/cost-management-billing/reservations/save-compute-costs-reservations)

Nu har du möjlighet att köpa Azure-reservationer för kundernas räkning, eftersom du redan har gjort det. Du kan också ge kunderna tillstånd att köpa sina egna Azure-reservationer.

>[!NOTE]
> När du ger kunderna tillstånd att köpa sina egna Azure-reservationer, kan de hantera alla reservationer som de köper. Mer information finns i [Hjälp kunderna att hantera reservationer som de köper](give-customers-permission.md#help-customers-manage-reservations-they-purchase).

### <a name="to-enable-customers-to-buy-their-own-azure-reservations"></a>Så att kunderna kan köpa sina egna Azure-reservationer

1. Kontrol lera att kunden har en befintlig Azure-plan eller Global Azure-prenumeration som du har köpt för deras räkning.

2. Verifiera att kunden har tilldelats **ägar** rollen för den här prenumerationen.

3. Aktivera kund behörigheter (aktivera den här funktionen **på**) för att köpa sina egna Azure-reservationer.

Varje steg visas nedan.

### <a name="verify-the-customer-has-an-existing-azure-subscription"></a>Verifiera att kunden har en befintlig Azure-prenumeration

Innan du ger kunderna tillstånd att köpa sina egna Azure-reservationer måste du kontrol lera att kunden har en befintlig Azure-plan eller Global Azure-prenumeration. Om kunden inte visar någon aktuell Azure-prenumeration i Partner Center måste du köpa en prenumeration för dem innan du aktiverar deras kund behörigheter.

- Om du vill se om en kund redan har en Azure-prenumeration loggar du in på Partner Center-instrumentpanelen och väljer sedan **CSP** följt av **kunder**. Välj den specifika kunden i listan. Välj sedan **prenumerationer** och leta efter eventuella användnings prenumerationer för antingen Azure-plan eller Azure Global.

- Om en kund inte har en befintlig Azure-prenumeration kan du köpa en prenumeration för dem. Se [köpa Azure-prenumerationen](purchase-azure-plan.md).

### <a name="verify-the-customer-has-been-assigned-the-correct-role-in-azure"></a>Kontrol lera att kunden har tilldelats rätt roll i Azure

När du har kontrollerat att kunden har en befintlig Azure-prenumeration måste du också kontrol lera att de viktiga användare som är kopplade till din kund har tilldelats rätt **ägar** roll för Azure-prenumerationen. Detta är den rollbaserad åtkomst (RBAC) som kunden behöver för att köpa Azure-reservationer för en Azure-prenumeration som du har köpt.

Vissa partner kanske redan har tilldelat **ägar** rollen till kunder som vill hantera och etablera sina egna Azure-resurser. Om du redan har tilldelat **ägar** status till en kund för att hantera tidigare prenumerationer som du har köpt för dem kan du hoppa över det här steget.  

> [!IMPORTANT]
> Om en kund inte har tilldelats **ägar** rollen får de ett fel meddelande i Azure Portal som gör att de inte kan köpa Azure-reservationer.

För att verifiera att kunden har tilldelats **ägar** rollen för en Azure-prenumeration:

1. Logga in på [instrument panelen](https://partner.microsoft.com/dashboard)för partner Center.

2. Välj **CSP**, sedan **kunder** och välj den specifika kunden.

3. Välj **prenumerationer** för kunden och leta upp den specifika Azure-prenumerationen.

4. Välj knappen **Hantera** bredvid kundens prenumeration. Om du gör det öppnas [Azure Portal](https://portal.azure.com/).

5. Om du vill tilldela **ägar** rollen till en speciell användare följer du dessa steg [för att tilldela en användare som administratör](/azure/cost-management-billing/manage/add-change-subscription-administrator#to-assign-a-user-as-an-administrator).

### <a name="turn-on-or-turn-off-customer-permissions-to-purchase-their-own-azure-reservations"></a>Aktivera eller inaktivera kund behörigheter för att köpa sina egna Azure-reservationer

När du har kontrollerat att kunden har en befintlig Azure-prenumeration och användare tilldelas **ägar** rollen för den prenumerationen är du redo att aktivera (aktivera) kund behörigheter. Du kan också använda de här stegen för att inaktivera (inaktivera) kund behörigheter. Du kan aktivera eller inaktivera kund behörigheter med hjälp av instrument panelen för partner Center eller [API: er för partner Center](/partner-center/develop/manage-customers).

Aktivera (eller inaktivera) kund behörigheter i Partner Center:

1. Logga in på [instrument panelen](https://partner.microsoft.com/dashboard)för partner Center.

2. I den vänstra navigerings menyn väljer du **CSP** och sedan **kunder**. En kund lista visas.

3. Välj ett namn på en specifik kund.

4. Välj **konto** på menyn kund. Sidan kund **konto** visas.

5. Leta upp avsnittet med **kund behörigheter** längst ned på sidan.

   :::image type="content" source="images/give-customers-permission-reservations.png" alt-text="Sidan kund behörigheter på konto." border="true":::

6. Under **Azure-reservationer** letar du upp alternativet **Tillåt kund till köp** .

7. Om du vill aktivera kund behörigheter flyttar du växeln bredvid alternativet **till position.** Om du vill inaktivera kund behörigheter flyttar du växeln till **off** -läge.

>[!NOTE]
> Om du vill lära dig mer om vad som händer när du aktiverar en kunds behörigheter för att köpa sina egna Azure-reservationer, se [Översikt över kund behörigheter i Partner Center](give-customers-permission.md#overview-of-customer-permissions-in-partner-center).
>
>När du aktiverar (eller inaktiverar) kund behörigheter registrerar aktivitets loggen varje åtgärd. (Den här loggen är tillgänglig när du väljer kugg hjuls ikonen överst i instrument panelen för partner Center). När du aktiverar eller inaktiverar kund behörigheter visas åtgärden som antingen **Skapa kund inköps behörigheter** eller **ta bort kund inköps behörigheter** i aktivitets loggen.

## <a name="help-customers-manage-reservations-they-purchase"></a>Hjälp kunderna att hantera reservationer som de köper

När du ger kunderna tillstånd att köpa sina egna Azure-reservationer kan du hjälpa dem att hantera alla resurser som de köper. Kunder kan hantera många aspekter av Azure-reservationer direkt från [Azure Portal](https://portal.azure.com/). De behöver din hjälp att hantera några andra aspekter av de Azure-reservationer som de köper i din CSP-prenumeration.  

Hjälp kunderna att förstå mer om att hantera dessa aspekter av Azure-reservationer:

- Priserna för kunder kommer att betala för Azure-reservationer
- Hur kunder kan optimera användningen av Azure-reservationer
- Vad händer när kunder köper reservationer med en delad omfattning?
- Vad händer om kunder vill ändra, avbryta och förnya en reservation eller ändra dess omfattning?

**Priserna för kunderna debiteras för sina reservationer.** Kunden kommer att köpa Azure-reservationer baserat på en prenumeration som du tidigare har köpt för dem i ditt fakturerings konto för CSP-partner. Kundens pris för alla Azure-reservationer som de köper utifrån den här prenumerationen anges också av dig. Priset kan skilja sig från det WebDirect-pris som kunden ser i Azure Portal.

**Hur kunderna kan optimera användningen av en reservation.** Vissa kunder kan dra nytta av att lära sig mer om hur man optimerar användningen av en reservation eller hur man tilldelar en reservations ursprungliga omfattning under köpet. Om du vill ha mer information ber du kunderna att läsa [hantera reservationer för Azure-resurser](/azure/cost-management-billing/reservations/manage-reserved-vm-instance).

**Vad händer när en kund köper en reservation med en delad omfattning?** När kunderna köper en reservation baserat på en tidigare CSP-prenumeration och tilldelar en delad omfattning till den reservationen, kommer eventuella rabatter som kunden har fått av CSP: n att gälla för att matcha användning för alla prenumerationer som CSP-partnern har köpt för kunden.

**Vad bör kunderna göra om de vill byta ut, avbryta eller förnya ett köp som de har gjort eller ändra den ursprungliga omfånget för en reservation?** Kunder behöver be sin partner att hjälpa dem att ändra en reservations ursprungliga omfattning. De behöver också en partners hjälp för att utbyta, avbryta eller förnya en reservation. De kan inte utföra dessa uppgifter själva med reservationer baserat på prenumerationer som köpts av en CSP-partner.

## <a name="next-steps"></a>Nästa steg

- [Köp Azure-reservationer för kundernas räkning](azure-reservations-buying.md)

- [Partner Center – Sälj Microsoft-reservationer](azure-reservations.md)

- [Hantera Azure-reservationer för kundernas räkning](azure-reservations-manage.md)