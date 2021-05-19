---
title: Vad gör jag om den enda administratören för ditt MPN-program har lämnat företaget?
ms.topic: how-to
ms.date: 09/08/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Lär dig vad du kan göra för att hitta en ny MPN-administratör eller få hjälp från företagets globala administratör. Lär dig också hur du lägger till en ny global administratör i Partnercenter.
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 5efd157078acd72ca47418aaa9559a678fc5b129
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 05/19/2021
ms.locfileid: "110151176"
---
# <a name="what-to-do-if-the-only-admin-for-your-mpn-program-has-left-the-company"></a>Vad gör jag om den enda administratören för ditt MPN-program har lämnat företaget?

**Lämpliga roller:** MPN-partneradministratör | Kontoadministratörsbehörighet | Global administratör

I följande artikel går vi igenom tre vanliga scenarier för vad du kan göra om MPN-administratören har lämnat företaget.

## <a name="scenario-1-mpn-partner-adminaccount-admin-has-left-the-company-but-there-are-still-global-admins-in-the-account"></a>Scenario 1: MPN-partneradministratören/kontoadministratören har lämnat företaget men det finns fortfarande globala administratörer i kontot

I det här fallet kan en annan person på företaget tilldelas rollen som MPN-partneradministratör. Tilldelas rollen som specifik MPN-partneradministratör/kontoadministratörsroll:

1. Logga in på ditt Partnercenter-konto med ditt arbetskonto (till exempel tom@contoso.com ).
1. På sidan **Användarhantering** filtrerar du på Global administratör för att se vilka globala administratörer för ditt företag är. 
1. Kontakta en av de globala administratörerna och be dem tilldela dig den MPN-specifika roll som du behöver. 

## <a name="scenario-2-mpn-partner-adminaccount-admin-has-left-the-company-and-there-are-no-global-admins-in-the-account"></a>Scenario 2: MPN-partneradministratören/kontoadministratören har lämnat företaget och det finns inga globala administratörer i kontot 

Följ dessa steg  om du går till sidan Användarhantering och filtrerar på Global administratör men du upptäcker att det inte finns någon global administratör i företaget som kan hjälpa dig att få den MPN-specifika rollen:

1. Gå till [portal.azure.com](https://ms.portal.azure.com/), logga in med ditt arbetskonto (till exempel tom@contoso.com ). 
1. Välj alternativet **Hjälp + support** i navigeringsfältet till vänster.
1. På nästa sida väljer du **Nytt Supportbegäran** och Teknisk **problemtyp** i listrutan, infogar eventuell ytterligare information och klickar på **Nästa: Lösningar.**

:::image type="content" source="images/accountsettings/adminfinder.png" alt-text="Leta upp administratör i Azure Portal":::

4. När du har granskat de rekommenderade lösningarna på nästa sida väljer **du Nästa: Information** och fyller i de obligatoriska fälten.
1. Granska och skapa supportbegäran.


## <a name="scenario-3-mpn-partner-adminaccount-adminglobal-admin-has-left-the-company-and-there-are-no-other-users-who-can-access-the-companys-azure-ad-this-is-a-complete-loss-of-access"></a>Scenario 3: MPN-partneradministratör/kontoadministratör/global administratör har lämnat företaget och det finns inga andra användare som har åtkomst till företagets Azure AD. Det här är en fullständig förlust av åtkomst.

Följ stegen [för övertagande](/azure/active-directory/users-groups-roles/domains-admin-takeover#internal-admin-takeover) av administratör för att ta över en ohanterad katalog som Azure Active Directory administratör.

## <a name="not-sure-if-your-company-already-has-a-work-account"></a>Är du osäker på om ditt företag redan har ett arbetskonto?

Om du inte är säker på om ditt företag har ett arbetskonto följer du dessa steg för att kontrollera.

1. Logga in på [Azure-administratörsportalen.](https://ms.portal.azure.com)
2. Välj **Azure Active Directory** på den vänstra menyn och välj **sedan Domännamn**.
Om du redan har ett arbetskonto visas ditt domännamn.

>[!Note]
>Om du har en aktiv prenumeration på Microsoft Azure eller Office 365 har du redan ett arbetskonto och dina inloggningsuppgifter ska vara samma som de som används för att komma åt dessa tjänster.