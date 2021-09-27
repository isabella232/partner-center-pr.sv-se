---
title: Hantera användare för kundkonton
ms.topic: how-to
ms.date: 09/27/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-customers
description: Hantera användare för dina kunder i Partnercenter – skapa användarkonton, lägga till eller ta bort användarlicenser, återställa lösenord och ta bort eller återställa användarkonton.
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: dca930586fd17e9c70e80455802cf3f587170a42
ms.sourcegitcommit: d731813da1d31519dc2dc583d17899e5cf4ec1b2
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/27/2021
ms.locfileid: "129070490"
---
# <a name="manage-users-and-user-licenses-for-customer-accounts"></a>Hantera användare och användarlicenser för kundkonton 

**Lämpliga roller:** Globala | Administratörsbehörighet för | Administratörsagent

Du kan skapa och ta bort nya användare i en kunds konto. Du kan också återställa ett eller flera användarkonton som du tidigare har tagit bort inom 30 dagar efter borttagningen. Användarens tidigare prenumerationstilldelningar återställs också (förutsatt att deras tidigare allokeringar är tillgängliga).

När du köper nya prenumerationer för en kund bör kunden ge dig en lista över alla användare som behöver konton, deras användarbehörigheter och vilka tjänster varje användare behöver.

> [!NOTE]
> Avsnittet **Användare och**  licenser på fliken Kund visar alla användare som skapats i en specifik kunds klientorganisation, inklusive användare som har köpt licenser från en annan CSP-partner eller från en annan inköpskanal.

Du kan [tilldela prenumerationer till flera användare](bulk-license-provisioning-for-multiple-users.md) samtidigt genom att importera namnen med hjälp Excel en .csv [kalkylbladsfil](adding-multiple-users-to-a-customer-account.md).

<a href="" id="createuseraccounts"></a>

## <a name="create-user-accounts-for-a-customer"></a>Skapa användarkonton för en kund

> [!NOTE]
> Förhandsversionsgränssnittet i Partnercenter ger en mer effektiv och produktiv användarupplevelse via logiskt grupperade arbetsytor. Mer information om gränssnittet för arbetsytor och hur du aktiverar det finns i [Getting around Partner Center (Ta sig runt i Partnercenter).](get-around-partner-center.md#turn-workspaces-on-and-off)

#### <a name="workspaces-view"></a>[Vyn Arbetsytor](#tab/workspaces-view)

1. På [instrumentpanelen i Partnercenter](https://partner.microsoft.com/dashboard)väljer **du panelen** Kunder och sedan kunden i listan Kund.

2. I kundmenyn väljer du **Användare och licenser.**

3. För varje användare som du lägger till **väljer du Lägg till** prenumeration och fyller sedan i informationen, inklusive behörigheter och licenser. **Spara** ändringarna.

4. Se till att registrera användarnamnet och det tillfälliga lösenordet som ska skickas till användaren.

5. Om du lägger till flera användare en i taget använder du Lägg **till en annan användare.**

6. Du kan också lägga till flera användare samtidigt genom [att importera en Excel-kompatibel .csv kalkylbladsfil](adding-multiple-users-to-a-customer-account.md). Du kan vänta tills du är klar med hela uppsättningen innan du skickar e-post eller skriver ut namn och lösenord från bekräftelseskärmen.

#### <a name="current-view"></a>[Aktuell vy](#tab/current-view)

1. På [instrumentpanelen i Partnercenter](https://partner.microsoft.com/dashboard) **väljer du** Kunder och sedan kunden i listan Kund.

2. I kundmenyn väljer du **Användare och licenser.**

3. För varje användare som du lägger till **väljer du Lägg till** prenumeration och fyller sedan i informationen, inklusive behörigheter och licenser. **Spara** ändringarna.

4. Se till att registrera användarnamnet och det tillfälliga lösenordet som ska skickas till användaren.

5. Om du lägger till flera användare en i taget använder du Lägg **till en annan användare.**

6. Du kan också lägga till flera användare samtidigt genom [att importera en Excel-kompatibel .csv kalkylbladsfil](adding-multiple-users-to-a-customer-account.md). Du kan vänta tills du är klar med hela uppsättningen innan du skickar e-post eller skriver ut namn och lösenord från bekräftelseskärmen.

* * *

<a href="" id="userlicensing"></a>

## <a name="add-or-remove-user-licenses-for-a-customer"></a>Lägga till eller ta bort användarlicenser för en kund

Följande steg gäller för att lägga till eller ta bort användarlicenser för Microsoft-produkter. Om du vill lägga till eller ta bort användarlicenser för licensbaserade SaaS-prenumerationer på den kommersiella marknadsplatsen kan du läsa Lägga till eller ta bort licenser för [en SaaS-prenumeration.](csp-commercial-marketplace-manage.md#add-or-remove-licenses-for-a-saas-subscription)

> [!NOTE]
> Förhandsversionsgränssnittet i Partnercenter ger en mer effektiv och produktiv användarupplevelse via logiskt grupperade arbetsytor. Mer information om gränssnittet för arbetsytor och hur du aktiverar det finns i [Getting around Partner Center (Ta sig runt i Partnercenter).](get-around-partner-center.md#turn-workspaces-on-and-off)

#### <a name="workspaces-view"></a>[Vyn Arbetsytor](#tab/workspaces-view)

1. På [instrumentpanelen i Partnercenter](https://partner.microsoft.com/dashboard)väljer **du panelen** Kunder och sedan kunden i listan Kund.

2. I kundmenyn väljer du **Användare och licenser.**

3. Välj en eller flera användare i listan. Om kunden till exempel precis har köpt nya licenser och du vill tilldela dem till personer som inte har dem ännu, kan du använda alternativet **Filtrera användare efter...** för att hitta rätt grupp.

4. Välj **Hantera licenser**. Gör dina ändringar och spara **sedan**.

> [!NOTE]
> För [Azure Marketplace produkter](csp-commercial-marketplace-manage.md#assign-licenses-and-activate-a-subscription-on-behalf-of-a-customer)hanteras licenstilldelning och aktivering via isv:n (Independent Software Vendor) som publicerade produkten.

#### <a name="current-view"></a>[Aktuell vy](#tab/current-view)

1. På [instrumentpanelen i Partnercenter](https://partner.microsoft.com/dashboard) **väljer du** Kunder och sedan kunden i listan Kund.

2. I kundmenyn väljer du **Användare och licenser.**

3. Välj en eller flera användare i listan. Om kunden till exempel precis har köpt nya licenser och du vill tilldela dem till personer som inte har dem ännu, kan du använda alternativet **Filtrera användare efter...** för att hitta rätt grupp.

4. Välj **Hantera licenser**. Gör dina ändringar och spara **sedan**.

> [!NOTE]
> För [Azure Marketplace produkter](csp-commercial-marketplace-manage.md#assign-licenses-and-activate-a-subscription-on-behalf-of-a-customer)hanteras licenstilldelning och aktivering via isv:n (Independent Software Vendor) som publicerade produkten.

* * *

<a href="" id="resetpassword"></a>

## <a name="reset-a-users-password-for-a-customer"></a>Återställa en användares lösenord för en kund

> [!NOTE]
> Förhandsversionsgränssnittet i Partnercenter ger en mer effektiv och produktiv användarupplevelse via logiskt grupperade arbetsytor. Mer information om gränssnittet för arbetsytor och hur du aktiverar det finns i [Getting around Partner Center (Ta sig runt i Partnercenter).](get-around-partner-center.md#turn-workspaces-on-and-off)

#### <a name="workspaces-view"></a>[Vyn Arbetsytor](#tab/workspaces-view)

1. Logga in på [instrumentpanelen i Partnercenter,](https://partner.microsoft.com/dashboard) **välj** panelen Kunder och välj sedan kunden i listan Kund.

2. I kundmenyn väljer du **Användare och licenser.** Välj användaren i listan.

3. Längst ned på skärmen väljer du **Återställ lösenord.**

4. Skicka det nya tillfälliga lösenordet till användaren.

#### <a name="current-view"></a>[Aktuell vy](#tab/current-view)

1. Logga in på [instrumentpanelen i Partnercenter,](https://partner.microsoft.com/dashboard)välj Kunder och välj sedan kunden i listan Kund. 

2. I kundmenyn väljer du **Användare och licenser.** Välj användaren i listan.

3. Längst ned på skärmen väljer du **Återställ lösenord.**

4. Skicka det nya tillfälliga lösenordet till användaren.

* * *

<a href="" id="deleteuseraccounts"></a>

## <a name="delete-user-accounts-for-a-customer"></a>Ta bort användarkonton för en kund

> [!NOTE]
> Förhandsversionsgränssnittet i Partnercenter ger en mer effektiv och produktiv användarupplevelse via logiskt grupperade arbetsytor. Mer information om gränssnittet för arbetsytor och hur du aktiverar det finns i [Getting around Partner Center (Ta sig runt i Partnercenter).](get-around-partner-center.md#turn-workspaces-on-and-off)

#### <a name="workspaces-view"></a>[Vyn Arbetsytor](#tab/workspaces-view)

1. På [instrumentpanelen i Partnercenter](https://partner.microsoft.com/dashboard)väljer **du panelen** Kunder och sedan kunden i listan Kund.

2. I kundmenyn väljer du **Användare och licenser.** Välj användaren i listan.

3. Längst ned på skärmen väljer du **Ta bort användarkonto.**

Om du behöver återställa det här kontot  hittar du det på fliken Borttagna användare i listan Kundens **användare och** licenser. Du har 30 dagar på dig att återställa en borttagna användare.

#### <a name="current-view"></a>[Aktuell vy](#tab/current-view)

1. På [instrumentpanelen i Partnercenter](https://partner.microsoft.com/dashboard) **väljer du** Kunder och sedan kunden i listan Kund.

2. I kundmenyn väljer du **Användare och licenser.** Välj användaren i listan.

3. Längst ned på skärmen väljer du **Ta bort användarkonto.**

Om du behöver återställa det här kontot  hittar du det på fliken Borttagna användare i listan Kundens **användare och** licenser. Du har 30 dagar på dig att återställa en borttagna användare.

* * *

<a href="" id="restoreuseraccounts"></a>

## <a name="restore-deleted-user-accounts"></a>Återställa borttagna användarkonton

> [!NOTE]
> Förhandsversionsgränssnittet i Partnercenter ger en mer effektiv och produktiv användarupplevelse via logiskt grupperade arbetsytor. Mer information om gränssnittet för arbetsytor och hur du aktiverar det finns i [Getting around Partner Center (Ta sig runt i Partnercenter).](get-around-partner-center.md#turn-workspaces-on-and-off)

#### <a name="workspaces-view"></a>[Vyn Arbetsytor](#tab/workspaces-view)

1. På [instrumentpanelen i Partnercenter](https://partner.microsoft.com/dashboard)väljer **du panelen** Kunder och sedan kunden i listan Kund.

2. Välj **Användare och licenser.**

3. Välj **fliken Borttagna** användare ( ). Den bör läsa **(1)** eller högre när det finns borttagna användare som kan återställas.

4. Markera en eller flera av de borttagna användarnas kryssrutor och välj sedan **Återställ**.

    Alla valda användarkonton visas igen på sidan **Användare och** licenser.

#### <a name="current-view"></a>[Aktuell vy](#tab/current-view)

1. På [instrumentpanelen i Partnercenter](https://partner.microsoft.com/dashboard) **väljer du** Kunder och sedan kunden i listan Kund.

2. Välj **Användare och licenser.**

3. Välj **fliken Borttagna** användare ( ). Den bör läsa **(1)** eller högre när det finns borttagna användare som kan återställas.

4. Markera en eller flera av de borttagna användarnas kryssrutor och välj sedan **Återställ**.

    Alla valda användarkonton visas igen på sidan **Användare och** licenser.

* * *

## <a name="next-steps"></a>Nästa steg

- [Tilldela eller återkalla licenser till flera användare](bulk-license-provisioning-for-multiple-users.md)

- [Skapa flera användare för ett kundkonto](adding-multiple-users-to-a-customer-account.md)