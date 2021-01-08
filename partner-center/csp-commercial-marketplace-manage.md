---
title: Hantera Marketplace-produkter & erbjudanden
ms.topic: how-to
ms.date: 07/02/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: I Partner Center kan du lära dig hur moln lösnings leverantörer kan hantera tredjeparts ISV-erbjudanden som köpts för kunder från den kommersiella marknaden.
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 5e6ca188aeb50cec6f847afb08be4a9d62b36984
ms.sourcegitcommit: a78dd3c532860d01867d116bfb4e2c88b84bcd25
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 01/08/2021
ms.locfileid: "97979684"
---
# <a name="manage-commercial-marketplace-products-and-offers-for-your-customers"></a>Hantera kommersiella Marketplace-produkter och erbjudanden för dina kunder


**Lämpliga roller**

- Global administratör
- Administratörs agent

Partner i CSP-programmet (Cloud Solution Provider) kan använda Partner Center-portalen för att köpa många ISV SaaS-erbjudanden eller prenumerationer för sina kunder från den kommersiella marknads platsen. När du har köpt ett erbjudande kan du hantera det på olika sätt.

## <a name="view-or-edit-a-subscription"></a>Visa eller redigera en prenumeration

När du har köpt en prenumeration från en tredjeparts ISV-utgivare kan du granska eller redigera den på följande sätt:

1. Logga in på Partner Center- [instrumentpanelen](https://partner.microsoft.com/dashboard)och välj sedan **kunder** i den vänstra navigerings menyn.

2. Välj en lämplig kund och välj sedan **prenumerationer**. Här listas alla licensbaserade prenumerationer som du har köpt för kunden.

3. I kolumnen **prenumeration** väljer du den prenumeration som du vill visa eller redigera. Detta ger dig mer information om hur du konfigurerar eller tillhandahåller erbjudandet. (Om det krävs mer åtgärd för erbjudandet kan du också se statusen "åtgärd krävs" i kolumnen Status. Detta kan också åtföljas av en länk till ISV-utgivarens webbplats.)

4. När du har valt den prenumeration som du vill visa eller redigera kan du redigera prenumerationen på sidan prenumerations information och göra saker som:

    - Ändra namnet på prenumerationen

    - Lägg till/minska antalet licenser i prenumerationen

    - Avbryt prenumerationen

    - Stäng av automatisk förnyelse

    - Lägg till ett MPN-ID för indirekt åter försäljare, om tillämpligt

> [!NOTE]
> Du kan behöva slutföra vissa steg som definierats av ISV-utgivaren innan du kan utföra vissa ändringar i en prenumeration, till exempel avbryta en prenumeration.

## <a name="assign-licenses-and-activate-a-subscription-on-behalf-of-a-customer"></a>Tilldela licenser och aktivera en prenumeration för en kunds räkning

När du köper ett SaaS-erbjudande (Software as a Service) som tillhandahålls av en oberoende program varu leverantör (ISV) utgivare på den kommersiella marknaden, hjälper ISV-utgivaren till att hantera processen för att tilldela licenser och aktivera prenumerationen åt kunden.

Utgivaren bör förse dig med en anpassad länk och en auktoriseringskod som identifierar ditt speciella köp.

1. Du kan hitta den här anpassade länken från ISV-utgivaren på några få sätt:

   - Du kan se länken från bekräftelse sidan som visas när du har köpt ett ISV SaaS-erbjudande. Du hittar den här länken på sidan genom att leta efter och välja **gå till utgivarens webbplats**.

   - Du kan se länken från den specifika kundens prenumerations sida. Den här Publisher-länken visas på den rad som är kopplad till ISV-erbjudandet eller prenumerationen som har köpts för kunden.

   - Du kan [Hämta länken med hjälp av API: er för partner Center](/partner-center/develop/get-activation-link-by-order-line-item).

   > [!NOTE]
   > För att göra detta åt kunden kan du behöva kopiera den anpassade länken, klistra in den i en privat webbläsare och ange kundens autentiseringsuppgifter.

2. När du befinner dig på ISV-utgivarens webbplats eller system kan utgivaren ta reda på eventuella ytterligare åtgärder som du måste vidta för att slutföra kund konfigurerings processen och etablera eller tilldela licenser.

3. Som partner i CSP-programmet som arbetar på uppdrag av din kund ansvarar du för att utföra följande uppgifter:

    - Skicka nödvändig information till utgivaren.

    - Skicka en nödvändig URL direkt till din kund (eller på annat sätt kommunicera direkt information om den här prenumerationen till kunden)

4. När du har angett nödvändig information till utgivaren kommer utgivaren att etablera och tilldela lämpliga licenser. Prenumerations faktureringen startar bara när följande händelser inträffar:

    - ISV-utgivaren har tilldelat lämpliga licenser

    - ISV-utgivaren har bekräftat till Microsoft (via en separat API för SaaS-utförande) att konto installationen har slutförts

## <a name="cancel-a-license-based-saas-subscription-from-an-isv-publisher"></a>Avbryta en licens beroende SaaS-prenumeration från en ISV-utgivare

När du prenumererar på en licensbaserade SaaS-produkt som erbjuds av en ISV-utgivare på den kommersiella Marketplace har du möjlighet att avbryta prenumerationen inom den angivna uppsägnings perioden. Den här uppsägnings perioden ändras beroende på om du har en månatlig eller årlig prenumeration. Du kan också välja om du vill förnya prenumerationen automatiskt.

Mer information om avbrotts perioder som är tillämpliga, hur du avbryter eller hur du förnyar en prenumeration automatiskt finns i:

- [Avbryta en prenumeration](create-a-new-subscription.md#cancel-a-subscription)

- [Förnya en prenumeration på kommersiellt marknads platser automatiskt](create-a-new-subscription.md#choose-whether-to-automatically-renew-a-commercial-marketplace-subscription)

## <a name="add-or-remove-licenses-for-a-saas-subscription"></a>Lägga till eller ta bort licenser för en SaaS-prenumeration

Om du har SaaS kan du lägga till eller ta bort användar licenser för en kund prenumeration.

1. Logga in på Partner Center- [instrumentpanelen](https://partner.microsoft.com/dashboard)och välj sedan **kunder** i den vänstra navigerings menyn.

2. Välj en lämplig kund och välj sedan **prenumerationer**. Här listas alla licensbaserade prenumerationer som du har köpt för kunden.

3. I kolumnen **prenumeration** väljer du den prenumeration som du vill ändra.

4. Leta upp fältet **kvantitet** på sidan prenumerations information. Här kan du öka eller minska antalet licenser.

5. Ändra antalet och välj sedan **Skicka**.

## <a name="manage-subscriptions-using-partner-center-apis"></a>Hantera prenumerationer med API: er för partner Center

Du kan också använda API: er för partner Center för att utföra livs cykel hantering och hantera fakturor för dina prenumerationer. Mer information finns i [skapa en prenumeration för kommersiella Marketplace-produkter](/partner-center/develop/create-subscription-azure-marketplace-products).

## <a name="next-steps"></a>Nästa steg

- [Köp kommersiella Marketplace-erbjudanden](csp-commercial-marketplace-purchase.md)
- [Läs om fakturering på den kommersiella marknads platsen](csp-commercial-marketplace-billing.md)