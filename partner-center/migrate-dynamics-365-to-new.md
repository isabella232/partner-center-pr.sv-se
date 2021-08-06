---
title: Migrera Dynamics 365 Business Edition
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
description: Lär dig hur du migrerar kvalificerade Dynamics 365 Business Edition-erbjudanden till nyare versioner innan de upphör att gälla.
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 40be8c8a338f5bbcbc8a10ccd9343f7ef52817902cdf7a5a54e8631a2d2c8b4b
ms.sourcegitcommit: 121f1b9cbd88faeba60dc9b475f9c0647cdc933c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/06/2021
ms.locfileid: "115681543"
---
# <a name="migrate-dynamics-365-business-edition-offers-to-newer-versions"></a>Migrera Dynamics 365 Business Edition-erbjudanden till nyare versioner

**Lämpliga roller:** Global | Administratörsbehörighet för användarhantering | Administratörsagent | Försäljningsagent

Från och med 1 januari 2019 kan kunder med Dynamics 365 Business Edition-prenumerationer inte längre förnya till dessa äldre erbjudanden. befintliga prenumerationer förnyas inte automatiskt när de upphör att gälla. På prenumerationens informationssida ändras prenumerationsstatusen till "Upphör att gälla [datum]" från "Förnyas automatiskt [datum]".

För att säkerställa kontinuitet för kunder bör du föra över dem med utgående prenumerationer till ett alternativ som stöds, som anges nedan. Vi rekommenderar att du flyttar kunder till nya prenumerationer före prenumerationens årliga slutdatum för att undvika eventuella tjänstavbrott för kunder.

Om du använder API:et (antingen KANT eller Partnercenter) kan du hitta prenumerationer som går ut genom att utvärdera slutdatumet för prenumerationen tillsammans med egenskapen för automatisk förnyelse = Falskt. Prenumerationerna i fråga ställs in på förnya automatiskt = Falskt den 1 januari 2019. Du kan när som helst flytta kunder till en ny plan. 

## <a name="the-dynamics-365-business-editions-being-retired"></a>Dynamics 365 Business Editions dras tillbaka

- Dynamics 365 for Finance and Operations, Business Edition
- Dynamics 365 for Team Members, Business Edition

## <a name="dynamics-business-central---the-dynamics-365-business-edition-new-offers"></a>Dynamics Business Central – nya erbjudanden för Dynamics 365 Business Edition

Med de nya Dynamics Business Central-erbjudandena kan dina kunder ansluta sina ekonomi-, försäljnings-, tjänst- och driftsprocesser för att effektivisera affärsprocesser, förbättra kundinteraktioner och fatta bättre beslut. Dynamics 365 Business Central är molnbaserad och endast tillgängligt via Molnlösningsleverantör (CSP) programpartner.
Dynamics 365 Business Edition-kunder är berättigade till rabatterade övergångspriser för de nya Business Central-erbjudandena fram till den 30 juni 2020.

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
2. På sidan med prenumerationsdetaljer ställer du in den gamla prenumerationen på **Pausad** och väljer **Skicka**.

Den gamla prenumerationen har nu inaktiverats och den nya prenumerationen är aktiv. Den pausade prenumerationen avetableeras automatiskt efter 120 dagar. Kunden medför inga ytterligare kostnader för den gamla prenumerationen.
