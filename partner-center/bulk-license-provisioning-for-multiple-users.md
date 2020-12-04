---
title: Tilldela eller återkalla licenser till flera användare
ms.topic: how-to
ms.date: 07/02/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Lär dig hur du använder ett kund konto för att tilldela eller återkalla licenser och tjänster till en användare eller till flera användare på samma gång.
author: amitravat
ms.author: amrava
ms.localizationpriority: medium
ms.custom: SEOJUNE.20
ms.openlocfilehash: b2c59bc40b5092a4a2ee6e06bcb2e49a86e0201d
ms.sourcegitcommit: 6b03ff400d1350db9696f9b457fcfe710310c5d3
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 12/03/2020
ms.locfileid: "96570662"
---
# <a name="assign-or-revoke-licenses-at-the-same-time-to-multiple-users-in-a-customer-account"></a>Tilldela eller återkalla licenser på samma tid till flera användare i ett kund konto

**Lämpliga roller**

- Administratörs agent
- Global administratör
- Support agent
- Försäljnings agent
- Administratör för användar hantering

Du kan tilldela licenser och tjänster till en användare eller till flera användare samtidigt på ett kund konto och återkalla licens tilldelningar till användare.

Partner Center spårar och visar alla kundägda licens rättigheter.

## <a name="assign-licenses-to-multiple-users"></a>Tilldela licenser till flera användare

1. Från menyn **partner Center** väljer du **kunder** och väljer sedan en kund i listan.

2. Välj **användare och licenser**.

3. Markera kryss rutan för två eller flera användare i listan. (Om du vill markera alla användare på den aktuella sidan markerar du kryss rutan längst upp i kolumnen **användare** .)

    Du kan hitta och välja användare över flera sidor med hjälp av det **första**, **föregående**, **Nästa** och **sista** verktyget.

4. Välj länken **valda användare** . I listan som visas visas de valda användarna.

5. Välj länken **Hantera licenser** .

    Sidan hantera licenser visar listan över licens rättigheter för kund kontona och antalet **tillgängliga licenser** för varje produkt.

    - Kryss rutorna i kolumnen **produkt** visar status för alla valda användare för kunden berättigade produkter:

       - När alla valda användare redan har en licens fylls kryss rutan för produkten.

       - Om några av de valda användarna har en produkt licens är kryss rutan för produkten delvis ifylld.

       - Om ingen av de valda användarna har en produkt licens är kryss rutan avmarkerad.

    - Varje vald användare visas i en liten ruta längst upp på sidan. Användarna visas i sorterad ordning.

    - Välj en länk i kolumnen **tilldelad** om du vill visa en knapp beskrivnings lista med de valda användarna som redan har en licens.

    - Alla produkter utan tillgängliga licenser visar en **köp** länk. Du kan köpa fler licenser när kunder kräver det.

6. Under **tilldela och återkalla licenser** väljer du produkt licenser för de nya användarna. 

   Om till exempel ingen av de valda användarna har Office 365 Enterprise-licenser och du vill lägga till dem markerar du kryss rutan. Du behöver tillräckligt många licenser för varje vald produkt.

7. Välj mer än en produkt för användarna genom att markera kryss rutan för varje produkt.
    -   Välj **Visa Service planer** för valfri produkt för att visa och välja de tjänst planer som användarna behöver.

8. Välj **Spara**. Partner Center öppnar en bekräftelse sida med **licenser** som visar användarna och deras nya licenser.

>[!NOTE]
>Vissa Microsoft-produkter är kanske inte tillgängliga på vissa platser. Andra produkter är beroende av andra produkter eller tjänster, eller kan inte tilldelas tillsammans till samma användare. När du har sparat visar bekräftelse sidan alla användares resultat från slutförd licens tilldelning och eventuella fel från licens tilldelningen.

## <a name="revoke-users-license-assignments"></a>Återkalla användares licens tilldelningar

1. Från menyn **partner Center** väljer du **kunder** och väljer sedan en kund i listan.

2. Välj **användare och licenser**.

3. Markera kryss rutan för två eller flera användare i listan. (Om du vill markera alla användare på den aktuella sidan markerar du kryss rutan längst upp i kolumnen **användare** .)

    Bläddra igenom de **första**, **föregående**, **Nästa** och **sista** verktygen för att hitta och välja andra användare. Du kan välja mellan flera sidor.

4. När du har valt användare väljer du länken **valda användare** . Listan som visas visar bara de valda användarna.

5. Välj länken **Hantera licenser** .

6. Under **tilldela och återkalla licenser** avmarkerar du kryss rutorna för produkter som tilldelats till användarna.

   Om till exempel alla valda användare har Office 365 Enterprise-licenser och du vill återkalla dem markerar du kryss rutan för att avmarkera den.

7. Välj **Spara**.

## <a name="next-steps"></a>Nästa steg

- [Tilldela licenser till en användare](assign-licenses-to-users.md)

- [Återställa administratörs behörighet för en kunds Azure CSP-prenumeration](revoke-reinstate-csp.md)