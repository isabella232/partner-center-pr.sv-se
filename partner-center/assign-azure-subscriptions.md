---
title: Tilldela Azure-prenumerationer till kunder
ms.topic: how-to
ms.date: 05/13/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Lär dig hur du tilldelar Azure-prenumerationer till dina kunder i Partner Center och hur du kan göra det möjligt för kunder att hantera sina egna prenumerationer.
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 8cac2a6edc9199befeae940ed271c3236440c260
ms.sourcegitcommit: 4043c791402f0acebee6ede160a135e87fe92493
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 12/01/2020
ms.locfileid: "96473959"
---
# <a name="assigning-azure-subscriptions-to-customers-in-partner-center"></a>Tilldela Azure-prenumerationer till kunder i Partner Center

**Lämpliga roller**

- Global administratör
- Försäljnings agent

## <a name="assign-azure-subscriptions-to-your-customers"></a>Tilldela Azure-prenumerationer till dina kunder

1. Välj **kunder** från menyn **partner Center** och leta upp den kund som du vill hantera.

2. Välj nedåtpilen i slutet av raden för att expandera kundens post och välj sedan **Microsoft Azure-hanteringsportal**. Du dirigeras till [Azure Portal](https://portal.azure.com/) där du kan hantera kundens prenumerationer.

3. Välj **prenumerationer** från Azure Portal.

4. Välj den prenumeration som du vill tilldela och välj **Access Control**.

5. Välj **Lägg till** för att lägga till en användare i prenumerationen. 

6. När du har lagt till användaren i prenumerationen kan du tilldela användaren en roll och det angivna kontot som användaren kommer att ha åtkomst till.

## <a name="enable-customers-to-manage-their-azure-subscriptions"></a>Gör det möjligt för kunder att hantera sina Azure-prenumerationer

När du har skapat en Microsoft Azure-prenumeration för en kund kan du göra det möjligt för dem att hantera prenumerationen. För att göra detta måste du logga in på kundens Microsoft Azure hanterings Portal. 

1. Öppna kundens Azure Portal genom att antingen expandera kundens lista i din kund lista eller Välj kundens namn och välj sedan **Microsoft Azure-hanteringsportal**.

   > [!NOTE]  
   > Om du uppmanas att logga in på Azure Portal kanske du inte har delegerad administratörs behörighet. Välj **begär en relation** för att bjuda in kunden att identifiera dig som sin partner av posten. När kunden har accepterat din inbjudan beviljas du automatiskt delegerad administratörs behörighet.

2. I Azure Portal öppnar du kund prenumerations listan och väljer kundens Azure-prenumeration.

3. Tilldela en roll till någon av kundens användare så att de kan skapa och hantera resurser under prenumerationen.

## <a name="next-steps"></a>Nästa steg

- [Hur CSP-partner kan sälja prenumerationer till kunder](customer-subscriptions.md)

- [Så här hämtar du behörigheter för att hantera en kunds tjänst eller prenumerationer](customers-revoke-admin-privileges.md)
