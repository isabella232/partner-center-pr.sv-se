---
title: Hantera användare och användar licenser för kund konton
ms.topic: how-to
ms.date: 05/13/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Lär dig hur du hanterar användare för dina kunder i Partner Center, till exempel skapa användar konton, lägga till eller ta bort användar licenser, återställa användar lösen ord och ta bort eller återställa användar konton.
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: fb7906b006540ef939e443a21855488e9d2c36f9
ms.sourcegitcommit: 4043c791402f0acebee6ede160a135e87fe92493
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 12/01/2020
ms.locfileid: "96474078"
---
# <a name="manage-users-and-user-licenses-for-customer-accounts"></a>Hantera användare och användar licenser för kund konton

**Lämpliga roller**

- Global administratör
- Administratör för användar hantering
- Administratörs agent


Du kan skapa och ta bort nya användare i ett kund konto. Du kan också återställa ett eller flera användar konton som du tidigare tog bort inom 30 dagar från borttagningen. Användarens tidigare prenumerations tilldelningar återställs också (förutsatt att deras tidigare allokeringar är tillgängliga).

När du köper nya prenumerationer för en kund bör kunden ge dig en lista över alla användare som behöver konton, deras användar behörigheter och vilka tjänster varje användare behöver.  

Du kan [tilldela prenumerationer till flera användare](bulk-license-provisioning-for-multiple-users.md) i taget genom att importera namnen med en [Excel-kompatibel. csv-kalkylbladsfilen](adding-multiple-users-to-a-customer-account.md).

<a href="" id="createuseraccounts"></a>

## <a name="create-user-accounts-for-a-customer"></a>Skapa användar konton för en kund

1. Logga in på [instrument panelen](https://partner.microsoft.com/dashboard)för partner Center.

2. Från menyn Partner Center väljer du **kunder** och väljer sedan en kund i listan.

3. I menyn kund väljer **du användare och licenser**.

4. För varje användare som du lägger till väljer du **Lägg till prenumeration** och fyller sedan i informationen, inklusive behörigheter och licenser. **Spara** ändringarna.

5. Se till att du registrerar användar namnet och det tillfälliga lösen ordet för att skicka till användaren.

6. Om du lägger till flera användare en i taget använder du **Lägg till en annan användare**.

7. Du kan också lägga till flera användare samtidigt genom att [Importera en Excel-kompatibel. csv-kalkylbladsfilen](adding-multiple-users-to-a-customer-account.md). Du kan vänta tills du är klar med hela uppsättningen innan du skickar eller skriver ut namn och lösen ord från bekräftelse skärmen.

<a href="" id="userlicensing"></a>

## <a name="add-or-remove-user-licenses-for-a-customer"></a>Lägga till eller ta bort användar licenser för en kund

Följande steg gäller för att lägga till eller ta bort användar licenser för Microsoft-produkter. Om du vill lägga till eller ta bort användar licenser för licensbaserade SaaS-prenumerationer på den kommersiella Marketplace, se [lägga till eller ta bort licenser för en SaaS-prenumeration](csp-commercial-marketplace-manage.md#add-or-remove-licenses-for-a-saas-subscription).

1. Logga in på [instrument panelen](https://partner.microsoft.com/dashboard)för partner Center.

2. Från menyn Partner Center väljer du **kunder** och väljer sedan en kund i listan.

3. I menyn kund väljer **du användare och licenser**.

4. Välj en eller flera användare i listan. Om kunden till exempel precis har köpt nya licenser och du vill tilldela dem till personer som inte har dem än kan du använda alternativet **filtrera användare efter...** för att hitta rätt grupp.

5. Välj **Hantera licenser**. Gör dina ändringar och **Spara** sedan.

> [!NOTE]
> För [Azure Marketplace-produkter](csp-commercial-marketplace-manage.md#assign-licenses-and-activate-a-subscription-on-behalf-of-a-customer)hanteras licens tilldelning och aktivering via den oberoende program varu leverantör (ISV) som publicerade produkten.

<a href="" id="resetpassword"></a>

## <a name="reset-a-users-password-for-a-customer"></a>Återställa en användares lösen ord för en kund

1. Logga in på [instrument panelen](https://partner.microsoft.com/dashboard)för partner Center.

2. Från menyn Partner Center väljer du **kunder** och väljer sedan en kund i listan.

3.  I menyn kund väljer **du användare och licenser**. Välj användaren i listan.

4.  Längst ned på skärmen väljer du **Återställ lösen ord**. 

5.  Skicka det nya tillfälliga lösen ordet till användaren.

<a href="" id="deleteuseraccounts"></a>

## <a name="delete-user-accounts-for-a-customer"></a>Ta bort användar konton för en kund

1.  Från menyn **partner Center** väljer du **kunder**. Välj kund i listan.

2.  I menyn kund väljer **du användare och licenser**. Välj användaren i listan.

3.  Längst ned på skärmen väljer du **ta bort användar konto**.

Om du behöver återställa det här kontot kan du hitta det på fliken **borttagna användare** i listan kund **användare och licenser** . Du har 30 dagar på dig att återställa en borttagen användare.

<a href="" id="restoreuseraccounts"></a>

## <a name="restore-deleted-user-accounts"></a>Återställa borttagna användar konton

1.  Från menyn **partner Center** väljer du **kunder** och väljer sedan kunden i listan.

2.  Välj **användare och licenser**.

3.  Välj fliken **borttagna användare ()** . Den bör läsa **(1)** eller större när det finns borttagna användare som kan återställas.

4.  Välj en eller flera av kryss rutorna för borttagna användare och välj sedan **Återställ**.

    Alla valda användar konton kommer att visas på sidan **användare och licenser** .

## <a name="related-topics"></a>Relaterade ämnen


[Tilldela eller återkalla licenser till flera användare](bulk-license-provisioning-for-multiple-users.md)

[Skapa flera användare för ett kund konto](adding-multiple-users-to-a-customer-account.md)