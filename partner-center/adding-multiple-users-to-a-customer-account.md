---
title: Lägg till flera användare för ett kund konto
ms.topic: how-to
ms.date: 08/01/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Om du vill lägga till flera användare till ett kund konto laddar du upp en datafil till Partner Center med fil formatet kommaavgränsad (. csv).
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 0a9b2ed89b10e43c31d00777054839f3208e5c16
ms.sourcegitcommit: 32516c30e90ee78415e5537d2b8ccf467f56a82d
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/03/2020
ms.locfileid: "92531172"
---
# <a name="upload-a-csv-file-of-users-to-a-customers-account"></a>Ladda upp en. csv-fil för användare till ett kund konto


**Gäller för**

- Partnercenter

**Lämpliga roller**

- Global administratör

Lägg till flera användare till ett kund konto samtidigt, genom att ladda upp en datafil i det kommaavgränsade värde fil formatet (. csv) till Partner Center. 

## <a name="create-the-file-of-customer-users-and-upload-to-customer-account"></a>Skapa filen med kund användare och överför till kund konto

1. Skapa en datafil med kommaavgränsade värden (. csv) med de data som beskrivs ovan. Spara filen så att du kan bläddra till den i ett senare steg. Se [fält för. csv-filen om du vill importera flera användare för ett kund konto](file-customer-users.md). 

2. Logga in på [instrument panelen](https://partner.microsoft.com/dashboard)för partner Center.

3. Från menyn Partner Center väljer du **kunder** och väljer sedan en kund i listan.

4. Välj fliken **användare och licenser** för kunden och välj sedan **överför användare** .

5. Under **överför användar information** väljer du **Bläddra** .

6. Välj data fil i fil väljaren och välj sedan **Öppna** .

7. Välj **Verifiera** .

    **Obs!**    De flesta fel uppstår på grund av problem med att skapa filer, inklusive information om saknade data, felaktiga eller dubbla e-postadresser eller för många poster i filen.

8. När Partner Center har verifierat filen väljer du den geografiska **platsen** för de nya användarna.
9. Välj **Spara** .
10. Ladda ned den tillfälliga lösen ords informationen för användarna.

    >[!IMPORTANT]
    > Se till att ladda ned filen med de tillfälliga lösen orden nu eftersom du inte kommer att kunna göra detta senare. Nya användare måste logga in på sitt nya konto med det tillfälliga lösen ordet för sina nya konton.

11. Nya användare tilldelas automatiskt behörigheter för **kan använda licenser och tjänster** . 

## <a name="next-steps"></a>Nästa steg

- [Ge kunderna tillstånd i Partner Center att köpa sina egna produkter eller tjänster](give-customers-permission.md)
