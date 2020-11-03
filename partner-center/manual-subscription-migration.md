---
title: Migrera kvalificerade Dynamics 365-prenumerationer
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Lär dig hur du migrerar från kvalificerade, grundläggande Dynamics 365-prenumerationer till en ny prenumeration innan befintliga prenumerationer upphör att gälla.
author: Brentserbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 8575d87ab3c4c7970135a87b7ef7564c4fe06232
ms.sourcegitcommit: 7153f0b8c67efd35f58695ca2a7e00e70da1c5e9
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 07/17/2020
ms.locfileid: "92531008"
---
# <a name="migrate-dynamics-365-and-customer-engagement-plan-from-basic-qualified-offers-to-newer-versions"></a>Migrera Dynamics 365 och en plan för kundengagemang från Basic (kvalificerade erbjudanden) till nyare versioner

**Gäller för**

-  Partnercenter

**Lämpliga roller**
-   Global administratör
-   Användaradministratör
-   Administratörs agent
-   Försäljnings agent

Från och med den 1 januari 2019 kan kunder med Dynamics 365 för försäljnings-/kund engagemang avtal från Basic-prenumerationer (kvalificerade erbjudanden) inte längre förnya de här äldre erbjudandena. befintliga prenumerationer förnyas inte automatiskt när de upphör att gälla. På prenumerationens informations sida ändras prenumerations statusen till "upphör att gälla [datum]" från "Auto Regener på [Date]". 

För att säkerställa kontinuitet för kunderna bör du gå över de med förfallna prenumerationer på ett alternativ som stöds. Vi rekommenderar att du flyttar kunder till nya prenumerationer före prenumerationens årliga slutdatum för att undvika eventuella avbrott i tjänsten för kunderna.

Om du använder API: et (topp-eller partner Center) kan du hitta förfallna prenumerationer genom att utvärdera slutdatumet för prenumerationen tillsammans med egenskapen Auto renew = false. Prenumerationerna i fråga kommer att ställas in på automatisk förnyelse = falskt den 1 januari 2019. Du kan när som helst flytta kunder till en ny plan. 

### <a name="the-dynamics-365-offers-being-retired"></a>Dynamics 365-erbjudanden som dras tillbaka

- Dynamics 365 for Sales Enterprise Edition CRMOL Basic (kvalificerat erbjudande)
- Dynamics 365 for Sales Enterprise Edition CRMOL Basic (kvalificerat erbjudande) för lärare
- Dynamics 365 for Sales Enterprise Edition CRMOL Basic (kvalificerat erbjudande) för studenter
- Dynamics 365 for Sales Enterprise Edition (myndighets prissättning) CRMOL Basic (kvalificerat erbjudande)
- Dynamics 365 för Sales Enterprise Edition från SA för CRM Basic (kvalificerat erbjudande)
- Dynamics 365 för Sales Enterprise Edition från SA för CRM Basic (kvalificerat erbjudande) för lärare
- Dynamics 365 för Sales Enterprise Edition från SA för CRM Basic (kvalificerat erbjudande) för studenter
- Dynamics 365 for Sales Enterprise Edition (myndighets priser) från SA för CRM Basic (kvalificerat erbjudande)
- Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (kvalificerat erbjudande)
- Dynamics 365 for Sales Enterprise Edition Add-On för CRM Basic (kvalificerat erbjudande) för lärare
- Dynamics 365 for Sales Enterprise Edition Add-On för CRM Basic (kvalificerat erbjudande) för studenter
- Dynamics 365 for Sales Enterprise Edition (myndighets prissättning) Add-On för CRM Basic (kvalificerat erbjudande)
- Dynamics 365 Customer Engagement plan Enterprise Edition CRMOL Basic (kvalificerat erbjudande)
- Dynamics 365 Customer Engagement plan Enterprise Edition (myndighets priser) CRMOL Basic (kvalificerat erbjudande)
- Dynamics 365 Customer Engagement plan Enterprise Edition CRMOL Basic (kvalificerat erbjudande) för studenter
- Dynamics 365 Customer Engagement plan Enterprise Edition CRMOL Basic (kvalificerat erbjudande) för lärare
- Dynamics 365 kund engagemang plan Enterprise Edition från SA för CRM Basic (kvalificerat erbjudande)
- Dynamics 365 Customer Engagement plan Enterprise Edition (prissättning för myndigheter) från SA för CRM Basic (kvalificerat erbjudande)
- Dynamics 365 Customer Engagement plan Enterprise Edition från SA för CRM Basic (kvalificerat erbjudande) för studenter
- Dynamics 365 Customer Engagement plan Enterprise Edition från SA för CRM Basic (kvalificerade erbjudanden) för lärare
- Dynamics 365 Customer Engagement plan Enterprise Edition Add-On for CRM Basic (kvalificerat erbjudande)
- Dynamics 365 Customer Engagement plan Enterprise Edition (myndighets prissättning) Add-On för CRM Basic (kvalificerat erbjudande)
- Dynamics 365 Customer Engagement plan Enterprise Edition Add-On for CRM Basic (kvalificerat erbjudande) för studenter
- Dynamics 365 Customer Engagement plan Enterprise Edition Add-On for CRM Basic (kvalificerade erbjudanden) för lärare



## <a name="dynamics-365-for-sales-customer-engagement-plan-from-basic-qualified-offers-replacement-plans"></a>Dynamics 365 för sälj-/kund engagemang-plan från Basic (kvalificerade erbjudanden) ersättnings planer

**Återkallade erbjudanden**   

- Dynamics 365 för försäljning från CRM Basic eller CRMOL Basic (kvalificerat erbjudande)
- Dynamics 365 kund engagemang plan från CRM Basic eller CRMOL Basic (kvalificerat erbjudande)

**Ersättnings alternativ**
- Dynamics 365 for Sales Professional (ny)
- Dynamics 365 for Sales Professional (ny)
- Dynamics 365 for Customer Service
- Dynamics 365 kund engagemang plan eller
- Dynamics 365-team medlemmar



## <a name="transition-customers-to-new-product-plans"></a>Överföra kunder till nya produkt planer

Att flytta kunder från tillbakadragna SKU: er till nyare kräver följande steg i den här ordningen:

- Köp den nya prenumerationen
- Tilldela om aktuella användar licenser
- Avbryt gammal prenumeration

## <a name="purchase-the-new-plan-for-your-customer"></a>Köp det nya avtalet för kunden

1. Välj **kunder** i det vänstra navigerings fältet och välj sedan den kund som du vill flytta till den nya prenumerationen.
2. Välj **Lägg till prenumeration** .
3. Välj den prenumeration som du vill köpa från katalogen (i det här fallet ett av alternativen ovan), ange antalet licenser och välj sedan **Skicka** . 

Din kund kommer nu att ha både den gamla och den nya prenumerationen. Nästa steg är att omtilldela licenser till kundens användare.

1. Välj **kunder** i det vänstra navigerings fältet och välj sedan den kund som du flyttar.
2. Välj **användare och licenser** .
3. Om du vill tilldela en licens till en användare igen väljer du användaren och väljer sedan **Hantera licenser** . 
4. På sidan **Hantera licenser** avmarkerar du kryss rutan Dynamics 365 för sälj-/kund engagemang från Basic-licens (kvalificerad erbjudande) och väljer en ny service plan för den prenumeration som kunden flyttar till. 
5. Välj **Skicka** . Du kommer att göra detta för varje användare som behöver den nya licensen. 

När du har flyttat licenserna till den nya prenumerationen kan du avbryta den gamla prenumerationen. 

1. Välj **kunder** i det vänstra navigerings fältet och välj sedan den kund som du flyttar.
2. På sidan prenumerations information anger du att den gamla prenumerationen har **pausats** och väljer **Skicka** .

Den gamla prenumerationen är nu inaktive rad och den nya prenumerationen är aktiv. Den inaktiverade prenumerationen kommer att avetableras automatiskt efter 120 dagar. Kunden debiteras inga ytterligare kostnader för den gamla prenumerationen.
 

 



