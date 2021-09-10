---
title: Hantera Marketplace-produkter & erbjudanden
ms.topic: how-to
ms.date: 07/02/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
description: Med Partnercenter kan du lära dig hur molnlösningsleverantörer kan hantera ISV-erbjudanden från tredje part som köpts för kunder från den kommersiella marknadsplatsen.
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 14901b47b7363b2d87861be43a7071d9f23545cc
ms.sourcegitcommit: 1161d5bcb345e368348c535a7211f0d353c5a471
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/09/2021
ms.locfileid: "123960083"
---
# <a name="manage-commercial-marketplace-products-and-offers-for-your-customers"></a>Hantera produkter och erbjudanden på den kommersiella marknadsplatsen för dina kunder


**Lämpliga roller:** Globala | Administratörsagent

Partner i Molnlösningsleverantör-programmet (CSP) kan använda Partner Center-portalen för att köpa många ISV SaaS-erbjudanden eller prenumerationer till sina kunder från den kommersiella marknadsplatsen. När du har köpt ett erbjudande kan du hantera det på olika sätt.

## <a name="view-or-edit-a-subscription"></a>Visa eller redigera en prenumeration

När du har köpt en prenumeration från en ISV-utgivare från tredje part kan du granska eller redigera den på följande sätt:

1. Logga in på instrumentpanelen [i Partnercenter](https://partner.microsoft.com/dashboard)och välj **sedan Kunder** i den vänstra navigeringsmenyn.

2. Välj en lämplig kund och välj sedan **Prenumerationer.** Här visas alla licensbaserade prenumerationer som du har köpt för kunden.

3. I kolumnen **Prenumeration** väljer du den prenumeration som du vill visa eller redigera. Detta ger dig mer information för att konfigurera eller etablera erbjudandet. (Om det krävs fler åtgärder i erbjudandet kan du även se statusen "Åtgärd krävs" i kolumnen Status. Detta kan också åtföljas av en länk till ISV-utgivarens webbplats.)

4. När du har valt den prenumeration som du vill visa eller redigera kan du på sidan med prenumerationsdetaljer redigera prenumerationen och bland annat göra följande:

    - Ändra prenumerationens smeknamn

    - Lägga till/minska antalet licenser i prenumerationen

    - Avbryta prenumerationen

    - Stäng av automatisk förnyelse

    - Lägg till ett MPN-ID för indirekt återförsäljare, om tillämpligt

> [!NOTE]
> Du kan behöva slutföra vissa steg som definierats av ISV-utgivaren innan du kan göra några ändringar i en prenumeration, till exempel att avbryta en prenumeration.

## <a name="assign-licenses-and-activate-a-subscription-on-behalf-of-a-customer"></a>Tilldela licenser och aktivera en prenumeration åt en kund

När du köper ett SaaS-erbjudande (Programvara som en tjänst) som tillhandahålls av en oberoende programvaruleverantör (ISV) på den kommersiella marknadsplatsen hjälper ISV-utgivaren till att hantera processen med att tilldela licenser och aktivera prenumerationen för din kunds räkning.

Utgivaren bör ge dig en anpassad länk och en auktoriseringskod som identifierar ditt specifika köp.

1. Du hittar den här anpassade länken från ISV-utgivaren på några olika sätt:

   - Du kan se länken från bekräftelsesidan som visas när du har köpt ett ISV SaaS-erbjudande. Du hittar den här länken på sidan genom att leta upp och **välja Gå till utgivarens webbplats.**

   - Du kan se länken från den specifika kundens prenumerationssida. Den här utgivarlänken visas på raden som är associerad med ISV-erbjudandet eller prenumerationen som köpts för kunden.

   - Du kan [hämta länken med partnercenter-API:er.](/partner-center/develop/get-activation-link-by-order-line-item)

   > [!NOTE]
   > Om du vill göra detta för din kunds räkning kan du behöva kopiera den anpassade länken, klistra in den i en privat webbläsare och ange kundens autentiseringsuppgifter.

2. När du befinner dig på ISV-utgivarens webbplats eller system, kommer utgivaren att meddela dig om eventuella ytterligare steg som du behöver vidta för att slutföra kundens konfigurationsprocess och etablera eller tilldela licenser.

3. Som partner i CSP-programmet som arbetar för din kunds räkning ansvarar du för att utföra följande uppgifter:

    - Skicka all nödvändig information till utgivaren.

    - Skicka eventuella nödvändiga URL:er direkt till kunden (eller på annat sätt direkt kommunicera information om prenumerationen till kunden)

4. När du har uppgivt nödvändig information till utgivaren etablerar och tilldelar utgivaren lämpliga licenser. Prenumerationsfakturering startar först efter att följande händelser har inträffat:

    - ISV-utgivaren har tilldelat lämpliga licenser

    - ISV-utgivaren har bekräftat till Microsoft (via ett separat API för uppfyllning av SaaS) att kontokonfigurationen har slutförts

## <a name="cancel-a-license-based-saas-subscription-from-an-isv-publisher"></a>Avbryta en licensbaserad SaaS-prenumeration från en ISV-utgivare

När du prenumererar på en licensbaserad SaaS-produkt som erbjuds av en ISV-utgivare på den kommersiella marknadsplatsen har du möjlighet att avbryta prenumerationen inom den angivna annulleringsperioden. Den här uppsägningsperioden ändras beroende på om du har en månatlig eller årlig prenumeration. Du kan också välja om du vill förnya prenumerationen automatiskt.

Mer information om uppsägningsperioder som gäller, hur du avbryter eller förnyar en prenumeration automatiskt finns i [Avbryta en prenumeration.](create-a-new-subscription.md#cancel-a-subscription)

## <a name="add-or-remove-licenses-for-a-saas-subscription"></a>Lägga till eller ta bort licenser för en SaaS-prenumeration

För saaS-erbjudanden på den kommersiella marknadsplatsen kan du lägga till eller ta bort användarlicenser för en kundprenumeration.

1. Logga in på instrumentpanelen [i Partnercenter](https://partner.microsoft.com/dashboard)och välj **sedan Kunder** i den vänstra navigeringsmenyn.

2. Välj en lämplig kund och välj sedan **Prenumerationer.** Här visas alla licensbaserade prenumerationer som du har köpt för kunden.

3. I kolumnen **Prenumeration** väljer du den prenumeration som du vill ändra.

4. På sidan prenumerationsinformation letar du upp **fältet** Kvantitet. Det är här du kan öka eller minska antalet licenser.

5. Ändra kvantiteten och välj sedan **Skicka**.

## <a name="manage-subscriptions-using-partner-center-apis"></a>Hantera prenumerationer med partnercenter-API:er

Du kan också använda Partner Center-API:er för att utföra livscykelhantering och hantera fakturor för dina prenumerationer. Mer information finns i Skapa [en prenumeration för produkter på den kommersiella marknadsplatsen.](/partner-center/develop/create-subscription-azure-marketplace-products)

## <a name="next-steps"></a>Nästa steg

- [Köpa erbjudanden på den kommersiella marknadsplatsen](csp-commercial-marketplace-purchase.md)
- [Läs mer om fakturering på den kommersiella marknadsplatsen](csp-commercial-marketplace-billing.md)
