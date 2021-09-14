---
title: Tilldela eller återkalla licenser till flera användare
ms.topic: how-to
ms.date: 07/02/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-customers
description: Lär dig hur du använder ett kundkonto för att tilldela eller återkalla licenser och tjänster till en användare eller till flera användare samtidigt.
author: amitravat
ms.author: amrava
ms.localizationpriority: medium
ms.custom: SEOJUNE.20
ms.openlocfilehash: 256e93499a3a9b2786d8d1a309077b645aecd81c
ms.sourcegitcommit: 37eac16c4339cb97831eb2a86d156c45bdf6a531
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/13/2021
ms.locfileid: "126246301"
---
# <a name="assign-or-revoke-licenses-at-the-same-time-to-multiple-users-in-a-customer-account"></a>Tilldela eller återkalla licenser på samma gång till flera användare i ett kundkonto

**Lämpliga roller:** Administratörsagent | Global | Supportagent | Försäljningsagent | Administratör för användarhantering

Du kan tilldela licenser och tjänster till en användare eller till flera användare samtidigt på ett kundkonto och återkalla licenstilldelningar till användare.

Partnercenter spårar och visar alla kundägda licensrättigheter.

## <a name="assign-licenses-to-multiple-users"></a>Tilldela licenser till flera användare

1. I **menyn i Partnercenter** väljer **du Kunder** och sedan en kund i listan.

2. Välj **Användare och licenser.**

3. Markera kryssrutan för två eller flera användare i listan. (Markera alla användare på den aktuella sidan genom att markera kryssrutan överst i **kolumnen** Användare.)

    Du kan hitta och välja användare på flera sidor med hjälp av **verktygen First**, **Previous**, **Next** **och Last.**

4. Välj länken **Valda** användare. Den visade listan visar de valda användarna.

5. Välj länken **Hantera** licenser.

    Sidan Hantera licenser visar en lista över licensrättigheter för kundkontona och antalet **tillgängliga licenser** för varje produkt.

    - Kryssrutorna i **kolumnen** Produkt visar status för alla valda användare för de kundberättigade produkterna:

       - När alla valda användare redan har en licens fylls kryssrutan för produkten i.

       - Om några av de valda användarna har en produktlicens är kryssrutan för produkten delvis ifylld.

       - Om ingen av de valda användarna har en produktlicens är kryssrutan avmarkerad.

    - Varje vald användare visas i en liten ruta längst upp på sidan. Användarna visas i sorterad ordning.

    - Välj en länk i kolumnen **Tilldelad** för att visa en knappbeskrivningslista som visar de valda användare som redan har en licens.

    - Alla produkter utan tillgängliga licenser visar länken **Köp** mer. Du kan köpa fler licenser när kunderna behöver dem.

6. Under **Tilldela och återkalla licenser** väljer du produktlicenser för de nya användarna. 

   Om ingen av de valda användarna till exempel har Office 365 Enterprise licenser och du vill lägga till dem markerar du kryssrutan. Du behöver tillräckligt med licenser för varje vald produkt.

7. Markera fler än en produkt för användarna genom att markera kryssrutan för varje produkt.
    -   Välj **Visa tjänstplaner** för alla produkter för att visa och välja de tjänstplaner som användarna behöver.

8. Välj **Spara**. Partnercenter öppnar en uppdaterad **bekräftelsesida** för licenser som visar användarna och deras nya licenser.

>[!NOTE]
>Vissa Microsoft-produkter kanske inte är tillgängliga på vissa platser. Andra produkter är beroende av andra produkter eller tjänster eller kan inte tilldelas tillsammans till samma användare. När du har sparat visar bekräftelsesidan alla användares resultat från en lyckad licenstilldelning och eventuella fel från licenstilldelningen.

## <a name="revoke-users-license-assignments"></a>Återkalla användares licenstilldelningar

1. I **menyn i Partnercenter** väljer **du Kunder** och sedan en kund i listan.

2. Välj **Användare och licenser.**

3. Markera kryssrutan för två eller flera användare i listan. (Markera alla användare på den aktuella sidan genom att markera kryssrutan överst i **kolumnen** Användare.)

    Bläddra igenom verktygen **First**, **Previous**, **Next** och **Last för** att hitta och välja andra användare. Du kan välja mellan flera sidor.

4. När du har valt användare väljer du **länken Valda** användare. Den visade listan visar endast de valda användarna.

5. Välj länken **Hantera** licenser.

6. Under **Tilldela och återkalla licenser avmarkerar** du kryssrutorna för produkter som tilldelats till användarna.

   Om till exempel alla valda användare har Office 365 Enterprise licenser och du vill återkalla dem, markerar du kryssrutan för att rensa den.

7. Välj **Spara**.

## <a name="next-steps"></a>Nästa steg

- [Tilldela licenser till en användare](assign-licenses-to-users.md)

- [Återställa administratörsbehörigheter för en kunds Azure CSP prenumerationer](revoke-reinstate-csp.md)