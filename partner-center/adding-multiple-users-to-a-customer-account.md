---
title: Lägga till flera användare för ett kundkonto
ms.topic: how-to
ms.date: 09/27/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-customers
description: Om du vill lägga till flera användare till en kunds konto laddar du upp en datafil till Partnercenter med hjälp av filformatet med kommaavgränsade värden (.csv).
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: a76190a4bbea62a3b8da11b165e148b8fc2a9551
ms.sourcegitcommit: e1da62b36420d78bf44e3962358d0af65ebc3402
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/27/2021
ms.locfileid: "129089204"
---
# <a name="upload-a-csv-file-of-users-to-a-customers-account"></a>Upload en .csv fil med användare till en kunds konto

**Lämpliga roller:** Global administratör

Lägg till flera användare till en kunds konto samtidigt genom att ladda upp en datafil i filformatet med kommaavgränsade värden (.csv) till Partnercenter. 

## <a name="create-the-file-of-customer-users-and-upload-to-customer-account"></a>Skapa filen med kundanvändare och ladda upp till kundkontot

> [!NOTE]
> Mer information om gränssnittet för arbetsytor finns i [Getting around Partner Center (Ta sig runt i Partnercenter).](get-around-partner-center.md#turn-workspaces-on-and-off)

#### <a name="workspaces-view"></a>[Vyn Arbetsytor](#tab/workspaces-view)

1. Skapa en datafil med kommaavgränsade värden (.csv) med de data som beskrivs ovan. Spara filen så att du kan bläddra till den i ett senare steg. Se [Fält för .csv för att importera flera användare för ett kundkonto.](file-customer-users.md)

2. Logga in på instrumentpanelen i [Partnercenter](https://partner.microsoft.com/dashboard) och välj **panelen** Kunder.

3. Välj en kund i listan Kund.

4. Välj kundens flik **Användare och licenser och** välj sedan Upload **användare**.

5. Under **Upload användarinformation** väljer du **Bläddra**.

6. I filväljaren väljer du din datafil och sedan **Öppna**.

7. Välj **Verifiera**.

    De flesta fel vid skapande av konton orsakas av problem med datafilen, inklusive information som saknas, felaktiga eller duplicerade e-postadresser eller för många poster i filen.

8. När Partnercenter har verifierat filen väljer du den geografiska **platsen för** de nya användarna.

9. Välj **Spara**.

10. Ladda ned tillfällig lösenordsinformation för användarna.

    > [!IMPORTANT]
    > Se till att ladda ned filen med de tillfälliga lösenorden nu eftersom du inte kan göra det senare. Nya användare måste logga in på sitt nya konto med det tillfälliga lösenordet för sina nya konton.

11. Nya användare tilldelas automatiskt behörigheter för **Can use licenses and services (Kan använda licenser och tjänster).**

#### <a name="current-view"></a>[Aktuell vy](#tab/current-view)

1. Skapa en datafil med kommaavgränsade värden (.csv) med de data som beskrivs ovan. Spara filen så att du kan bläddra till den i ett senare steg. Se [Fält för .csv för att importera flera användare för ett kundkonto.](file-customer-users.md) 

2. Logga in i Partnercenter och gå till [instrumentpanelen](https://partner.microsoft.com/dashboard).

3. I menyn i Partnercenter väljer **du Kunder** och sedan en kund i listan Kund.

4. Välj kundens flik **Användare och licenser och** välj sedan Upload **användare**.

5. Under **Upload användarinformation** väljer du **Bläddra**.

6. I filväljaren väljer du din datafil och sedan **Öppna**.

7. Välj **Verifiera**.

    De flesta fel vid skapande av konton orsakas av problem med datafilen, inklusive information som saknas, felaktiga eller duplicerade e-postadresser eller för många poster i filen.

8. När Partnercenter har verifierat filen väljer du den geografiska **platsen för** de nya användarna.

9. Välj **Spara**.

10. Ladda ned tillfällig lösenordsinformation för användarna.

    > [!IMPORTANT]
    > Se till att ladda ned filen med de tillfälliga lösenorden nu eftersom du inte kan göra det senare. Nya användare måste logga in på sitt nya konto med det tillfälliga lösenordet för sina nya konton.

11. Nya användare tilldelas automatiskt behörigheter för **Can use licenses and services (Kan använda licenser och tjänster).**

* * *

## <a name="next-steps"></a>Nästa steg

- [Ge kunderna behörighet i Partnercenter att köpa egna produkter eller tjänster](give-customers-permission.md)
