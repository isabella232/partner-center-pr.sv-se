---
title: Migrera Dynamics 365 Business Edition
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Lär dig hur du migrerar kvalificerade Dynamics 365 Business Edition-erbjudanden till nyare versioner innan de går ut.
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: e83c06c11638bdde508fd27904038bcb6d8c9e9c
ms.sourcegitcommit: f24089cd27b1de6ecf6ddbefb6cbb2d340e144de
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/01/2021
ms.locfileid: "106132646"
---
# <a name="migrate-dynamics-365-business-edition-offers-to-newer-versions"></a>Migrera Dynamics 365 Business Edition-erbjudanden till nyare versioner

**Lämpliga roller**

- Global administratör
- Administratör för användar hantering
- Administratörs agent
- Försäljnings agent

Från och med 1 januari 2019 kan kunder med Dynamics 365 Business Edition-prenumerationer inte längre förnyas till de här äldre erbjudandena. befintliga prenumerationer förnyas inte automatiskt när de upphör att gälla. På prenumerationens informations sida ändras prenumerations statusen till "upphör att gälla [datum]" från "Auto Regener på [Date]".

För att säkerställa kontinuitet för kunderna bör du gå över de med förfallna prenumerationer på ett alternativ som stöds. Vi rekommenderar att du flyttar kunder till nya prenumerationer före prenumerationens årliga slutdatum för att undvika eventuella avbrott i tjänsten för kunderna.

Om du använder API: et (topp-eller partner Center) kan du hitta förfallna prenumerationer genom att utvärdera slutdatumet för prenumerationen tillsammans med egenskapen Auto renew = false. Prenumerationerna i fråga kommer att ställas in på automatisk förnyelse = falskt den 1 januari 2019. Du kan när som helst flytta kunder till en ny plan. 

## <a name="the-dynamics-365-business-editions-being-retired"></a>Dynamics 365 Business-versionerna dras tillbaka

- Dynamics 365 för finanser och drift, Business Edition
- Dynamics 365 for Team Members, Business Edition

## <a name="dynamics-business-central---the-dynamics-365-business-edition-new-offers"></a>Dynamics Business Central – Dynamics 365 Business Edition nya erbjudanden

Med de nya Dynamics Business Central-erbjudandena kan dina kunder ansluta sina finanser, försäljning, tjänster och åtgärder för att effektivisera affärs processerna, förbättra kund interaktioner och fatta bättre beslut. Dynamics 365 Business Central är endast molnbaserad och tillgängligt via program partner för Cloud Solution Provider (CSP).
Dynamics 365 Business Edition-kunder är berättigade till rabatterad över gångs prissättning för de nya företags Central erbjudandena fram till den 30 juni 2020.

## <a name="transition-customers-to-new-product-plans"></a>Överföra kunder till nya produkt planer

 Att flytta kunder från tillbakadragna SKU: er till nyare kräver följande steg i den här ordningen:

- Köp den nya prenumerationen
- Tilldela om aktuella användar licenser
- Avbryt gammal prenumeration

## <a name="purchase-the-new-plan-for-your-customer"></a>Köp det nya avtalet för kunden

1. Välj **kunder** i det vänstra navigerings fältet och välj sedan den kund som du vill flytta till den nya prenumerationen.
2. Välj **Lägg till prenumeration**.
3. Välj den prenumeration som du vill köpa från katalogen (i det här fallet ett av alternativen ovan), ange antalet licenser och välj sedan **Skicka**. 

Din kund kommer nu att ha både den gamla och den nya prenumerationen. Nästa steg är att omtilldela licenser till kundens användare.

1. Välj **kunder** i det vänstra navigerings fältet och välj sedan den kund som du flyttar.
2. Välj **användare och licenser**.
3. Om du vill tilldela en licens till en användare igen väljer du användaren och väljer sedan **Hantera licenser**. 
4. På sidan **Hantera licenser** avmarkerar du kryss rutan Dynamics 365 för sälj-/kund engagemang från Basic-licens (kvalificerad erbjudande) och väljer en ny service plan för den prenumeration som kunden flyttar till. 
5. Välj **Skicka**. Du kommer att göra detta för varje användare som behöver den nya licensen. 

När du har flyttat licenserna till den nya prenumerationen kan du avbryta den gamla prenumerationen. 

1. Välj **kunder** i det vänstra navigerings fältet och välj sedan den kund som du flyttar.
2. På sidan prenumerations information anger du att den gamla prenumerationen har **pausats** och väljer **Skicka**.

Den gamla prenumerationen är nu inaktive rad och den nya prenumerationen är aktiv. Den inaktiverade prenumerationen kommer att avetableras automatiskt efter 120 dagar. Kunden debiteras inga ytterligare kostnader för den gamla prenumerationen.
