---
title: Vad ska jag göra om den enda administratören för ditt MPN-program har lämnat företaget?
ms.topic: how-to
ms.date: 09/08/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Lär dig vad du ska göra för att hitta en ny MPN-administratör eller få hjälp från företagets globala administratör. Lär dig också hur du lägger till en ny global administratör för partner Center.
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 3702ebd5a9421036a053a9a142a2f40d3e488137
ms.sourcegitcommit: 3c26a61982082787bbdaf5d1e92553b26f3a5076
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/06/2021
ms.locfileid: "106442007"
---
# <a name="what-to-do-if-the-only-admin-for-your-mpn-program-has-left-the-company"></a>Vad ska jag göra om den enda administratören för ditt MPN-program har lämnat företaget?

**Lämpliga roller**

- MPN-partner administratör
- Kontoadministratör
- Global administratör

I följande artikel får du stegvisa instruktioner om vad du kan göra om din MPN-administratör har lämnat företaget.

## <a name="scenario-1-mpn-partner-adminaccount-admin-has-left-the-company-but-there-are-still-global-admins-in-the-account"></a>Scenario 1: MPN-partner administratören/konto administratören har lämnat företaget men det finns fortfarande globala administratörer i kontot

I det här fallet kan en annan person i företaget tilldelas rollen som MPN-partner administratör. Tilldelas rollen som roll för en speciell MPN-partner admin/konto-administratör:

1. Logga in på ditt partner Center-konto med ditt arbets konto (till exempel tom@contoso.com ).
1. Från sid filtret för **användar hantering** på global administratör för att se vilka globala administratörer för ditt företag är. 
1. Kontakta en av de globala administratörerna och be dem att tilldela dig den MPN roll du behöver. 

## <a name="scenario-2-mpn-partner-adminaccount-admin-has-left-the-company-and-there-are-no-global-admins-in-the-account"></a>Scenario 2: MPN-partner administratören/konto administratören har lämnat företaget och det finns inga globala administratörer i kontot 

Om du går till sidan för **användar hantering** och filter för global administratör, men du ser att det inte finns någon global administratör i ditt företag som kan hjälpa dig att få den MPN rollen, följer du dessa steg:

1. Gå till [Portal.Azure.com](https://ms.portal.azure.com/)och logga in med ditt arbets konto (till exempel tom@contoso.com ). 
1. Välj alternativet **Hjälp + Support** i det vänstra meny navigerings fältet.
1. På nästa sida väljer du **ny supportbegäran** och **teknisk ärende** typ i list menyn, infogar ytterligare information och klickar på **Nästa: lösningar.**

:::image type="content" source="images/accountsettings/adminfinder.png" alt-text="Hitta administratör i Azure Portal":::

4. När du har granskat de rekommenderade lösningarna på nästa sida väljer du **Nästa: information** och fyller i de fält som behövs.
1. Granska och skapa support förfrågan.


## <a name="scenario-3-mpn-partner-adminaccount-adminglobal-admin-has-left-the-company-and-there-are-no-other-users-who-can-access-the-companys-azure-ad-this-is-a-complete-loss-of-access"></a>Scenario 3: MPN partner admin/konto admin/global admin har lämnat företaget och det finns inga andra användare som kan komma åt företagets Azure AD. Detta är en fullständig förlust av åtkomst.

Följ stegen i [Administratörs](/azure/active-directory/users-groups-roles/domains-admin-takeover#internal-admin-takeover) förskottet för att ta över en ohanterad katalog som Azure Active Directory administratör.

## <a name="not-sure-if-your-company-already-has-a-work-account"></a>Är du osäker på om ditt företag redan har ett arbets konto?

Om du inte är säker på om ditt företag har ett arbets konto följer du de här stegen för att kontrol lera.

1. Logga in på [Azure admin-portalen](https://ms.portal.azure.com).
2. Välj **Azure Active Directory** på menyn till vänster och välj sedan **domän namn**.
Om du redan har ett arbets konto visas ditt domän namn.

>[!Note]
>Om du har en aktiv prenumeration på Microsoft Azure eller Office 365 har du redan ett arbets konto och inloggnings uppgifterna ska vara samma som de som används för att få åtkomst till dessa tjänster.