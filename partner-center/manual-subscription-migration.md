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
ms.openlocfilehash: 5ba6992eff64031aed0dafeb5a5010983396ab63
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 05/19/2021
ms.locfileid: "110151652"
---
# <a name="migrate-dynamics-365-and-customer-engagement-plan-from-basic-qualified-offers-to-newer-versions"></a>Migrera Dynamics 365 och en plan för kundengagemang från Basic (kvalificerade erbjudanden) till nyare versioner

**Lämpliga roller:** Global | Administratörsbehörighet för användarhantering | Administratörsagent | Försäljningsagent

Från och med den 1 januari 2019 kan kunder med Prenumerationer på Dynamics 365 for Sales/Customer Engagement från Basic-prenumerationer (kvalificerade erbjudanden) inte längre förnya dessa äldre erbjudanden. befintliga prenumerationer förnyas inte automatiskt när de upphör att gälla. På prenumerationens informationssida ändras prenumerationsstatusen till "Upphör att gälla [datum]" från "Förnyas automatiskt [datum]". 

För att säkerställa kontinuitet för kunder bör du föra över dem med utgående prenumerationer till ett alternativ som stöds, som anges nedan. Vi rekommenderar att du flyttar kunder till nya prenumerationer före prenumerationens årliga slutdatum för att undvika eventuella tjänstavbrott för kunder.

Om du använder API:et (antingen KANT eller Partnercenter) kan du hitta prenumerationer som går ut genom att utvärdera slutdatumet för prenumerationen tillsammans med egenskapen för automatisk förnyelse = Falskt. Prenumerationerna i fråga ställs in på förnya automatiskt = Falskt den 1 januari 2019. Du kan när som helst flytta kunder till en ny plan. 

### <a name="the-dynamics-365-offers-being-retired"></a>Dynamics 365-erbjudanden som dras tillbaka

- Dynamics 365 for Sales Enterprise Edition CRMOL Basic (kvalificerat erbjudande)
- Dynamics 365 for Sales Enterprise Edition CRMOL Basic (kvalificerat erbjudande) för lärare och lärare
- Dynamics 365 for Sales Enterprise Edition CRMOL Basic (kvalificerat erbjudande) för studenter
- Dynamics 365 for Sales Enterprise Edition (Government Pricing) CRMOL Basic (kvalificerat erbjudande)
- Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (kvalificerat erbjudande)
- Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (kvalificerat erbjudande) för lärare och lärare
- Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (kvalificerat erbjudande) för studenter
- Dynamics 365 for Sales Enterprise Edition (Myndighetspriser) från SA för CRM Basic (kvalificerat erbjudande)
- Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (kvalificerat erbjudande)
- Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (kvalificerat erbjudande) för lärare och lärare
- Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (kvalificerat erbjudande) för studenter
- Dynamics 365 for Sales Enterprise Edition (Government Pricing) Add-On för CRM Basic (kvalificerat erbjudande)
- Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (kvalificerat erbjudande)
- Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) CRMOL Basic (kvalificerat erbjudande)
- Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (kvalificerat erbjudande) för studenter
- Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (kvalificerat erbjudande) för lärare och lärare
- Dynamics 365 Customer Engagement Plan Enterprise Edition från SA för CRM Basic (kvalificerat erbjudande)
- Dynamics 365 Customer Engagement Plan Enterprise Edition (Myndighetspriser) från SA för CRM Basic (kvalificerat erbjudande)
- Dynamics 365 Customer Engagement Plan Enterprise Edition från SA för CRM Basic (kvalificerat erbjudande) för studenter
- Dynamics 365 Customer Engagement Plan Enterprise Edition from SA for CRM Basic (kvalificerat erbjudande) för lärare och lärare
- Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (kvalificerat erbjudande)
- Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) Add-On för CRM Basic (kvalificerat erbjudande)
- Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (kvalificerat erbjudande) för studenter
- Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (kvalificerat erbjudande) för lärare och lärare



## <a name="dynamics-365-for-sales-customer-engagement-plan-from-basic-qualified-offers-replacement-plans"></a>Dynamics 365 for Sales/Customer Engagement-plan från grundläggande (kvalificerade erbjudanden) ersättningsplaner

**Tillbakadragna erbjudanden**   

- Dynamics 365 for Sales från CRM Basic eller CRMOL Basic (kvalificerat erbjudande)
- Dynamics 365 Customer Engagement-plan från CRM Basic eller CRMOL Basic (kvalificerat erbjudande)

**Ersättningsalternativ**
- Dynamics 365 for Sales Professional (NY)
- Dynamics 365 for Sales Professional (NY)
- Dynamics 365 for Customer Service
- Dynamics 365 Customer Engagement-plan eller
- Dynamics 365-teammedlemmar



## <a name="transition-customers-to-new-product-plans"></a>Övergå kunder till nya produktplaner

Att flytta kunder från tillbakadragna SKU:er till nyare kräver följande steg i den här ordningen:

- Köpa den nya prenumerationen
- Tilldela om aktuella användarlicenser
- Avbryta gammal prenumeration

## <a name="purchase-the-new-plan-for-your-customer"></a>Köp den nya planen för din kund

1. Välj **Kunder** i det vänstra navigeringsfältet och välj sedan den kund som du vill flytta till den nya prenumerationen.
2. Välj **Lägg till prenumeration.**
3. Välj den prenumeration som du vill köpa från katalogen (i det här fallet något av alternativen ovan), ange antalet licenser och välj sedan **Skicka.** 

Kunden kommer nu att ha både den gamla och den nya. Nästa steg är att omtilldela licenser till kundens användare.

1. Välj **Kunder** i det vänstra navigeringsfältet och välj sedan den kund som du flyttar.
2. Välj **Användare och licenser.**
3. Om du vill tilldela om en licens till en användare väljer du användaren och sedan **Hantera licenser.** 
4. På sidan **Hantera licenser** avmarkerar du kryssrutan Dynamics 365 for Sales/Customer Engagement Plan från Basic-licens (kvalificerat erbjudande) och väljer en ny tjänstplan för prenumerationen som kunden flyttar till. 
5. Välj **Skicka**. Du gör detta för varje användare som behöver den nya licensen. 

När du har flyttat över licenserna till den nya prenumerationen kan du avbryta den gamla prenumerationen. 

1. Välj **Kunder** i det vänstra navigeringsfältet och välj sedan den kund som du flyttar.
2. På sidan med prenumerationsdetaljer anger du den gamla prenumerationen till **Pausad** och väljer **Skicka**.

Den gamla prenumerationen har nu inaktiverats och den nya prenumerationen är aktiv. Den pausade prenumerationen avetableeras automatiskt efter 120 dagar. Kunden medför inga ytterligare kostnader för den gamla prenumerationen.
 

 



