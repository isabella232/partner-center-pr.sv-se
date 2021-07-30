---
title: Migrera Office 365 E4-prenumerationer
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
description: Microsoft Office 365 Enterprise E4-utgåvan dras tillbaka den 7 april 2017. Lär dig hur du migrerar dina kundprenumerationer till nyare versioner av Office 365.
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: a1b47860f0af3427342d89945528e9118ecfc0aa
ms.sourcegitcommit: ad1af627f5ee6b6e3a70655f90927e932cf4c985
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 07/29/2021
ms.locfileid: "114843331"
---
# <a name="migrate-office-365-e4-subscriptions-to-newer-office-365-versions"></a>Migrera Office 365 E4-prenumerationer till senare Office 365-versioner

**Lämpliga roller:** Globala | Administratörsbehörighet för | Administratörsagent | Försäljningsagent

Den Office 365 Enterprise, E4 planen dras tillbaka från och med 7 april 2017. Du kan inte längre köpa nya Office 365 E4-prenumerationer efter detta datum, och befintliga E4-prenumerationer förnyas inte automatiskt när de upphör att gälla.

När E4-prenumerationer avslutas avbryts de. För att säkerställa kontinuitet för kunder bör du göra så att kunder med E4-prenumerationer upphör att gälla till ett SKU-alternativ som stöds, som anges nedan. Vi rekommenderar att du flyttar kunder till nya prenumerationer före prenumerationens årliga slutdatum för att undvika eventuella tjänstavbrott för kunder. 

> [!NOTE]  
> Både Office 365 Enterprise, E4 kommersiella SKU:er och myndighets-SKU:er dras tillbaka.
 
På prenumerationens informationssida har E4-prenumerationens status ändrats till "Upphör [datum]" från "Förnyas automatiskt [date]". 

Om du använder API:et (aNTINGEN ELLER Partnercenter) kan du identifiera utgående prenumerationer genom att utvärdera slutdatumet för prenumerationen tillsammans med egenskapen förnya automatiskt = Falskt. 

E4-prenumerationerna ställs in på förnya automatiskt = Falskt den 7 april 2017. Du kan när som helst flytta kunder till en ny plan. 

## <a name="office-365-enterprise-e4-edition-replacement-plans"></a>Office 365 Enterprise, E4- och versionsplaner

Du kan välja att behålla samma funktioner med E4 eller få dina kunder att dra nytta av nyare funktioner i Office 365 och Skype för företag Online. Prisinformation finns i matrisen för prislistan och erbjudandelistan i Partnercenter. Secure Product Enterprise E3 eller Secure Productive Enterprise E5 kan ersättas med följande alternativ för Office 365 Enterprise E3 eller Office 365 Enterprise E5.

- Alternativ 1: Office 365 Enterprise E5

- Alternativ 2: Office 365 Enterprise E3 + Skype för företag Cloud PBX

- Alternativ 3: Office 365 Enterprise E3 + Skype för företag Plus CAL (pris- och funktionsparitet med E4)

- Alternativ 4: Office 365 Enterprise E3


| Funktion | Alternativ 1 | Alternativ 2 | Alternativ 3 | Alternativ 4 |
| :---    | :------: |   :---:  |   :---:  |   :---:  |
| Får du alla funktioner som ingår i Office 365 Enterprise, E4? | Ja | Ja | Ja | Inga |
| Telefon tal som hanteras i Office 365? | Ja | Ja | Inga | Inga |
| Telefon tal som hanteras både lokalt och i Office 365 (hybriddistribution)? | Ja | Ja | Inga | Inga |
| Alternativ för att lägga till en pstn-plan för röstsamtal? | Ja | Ja | Inga | Inga |
| PSTN-konferens? | Ja | Inga | Inga | Inga |
| Avancerade verktyg för samarbete, analys och säkerhet? | Ja | Inga | Inga | Inga |
| Interaktiva rapporter, instrumentpaneler och datavisualiseringar? | Ja | Inga | Inga | Inga | 
| Mer kontroll över datasäkerhet och efterlevnad med inbyggd sekretess, transparens och förfinade användarkontroller? | Ja | Inga | Inga | Inga | 

## <a name="transition-customers-to-new-product-plans"></a>Övergå kunder till nya produktplaner

Microsoft erbjuder kontinuerligt nya produkter och tjänster till våra partner. I dessa fall kan du behöva uppgradera kunder till nya tjänster eller migrera sina prenumerationer från SKU:er som så småningom kommer att stängas av. Migrering av kunder från tillbakadragna SKU:er till nyare kräver följande steg:

-   Köpa den nya prenumerationen
-   Tilldela om aktuella användarlicenser
-   Avbryta den gamla prenumerationen

Följ de här stegen för att migrera en Office 365 Enterprise, E4 prenumeration till något av alternativen i tabellen ovan.

### <a name="step-1---purchase-the-new-subscription"></a>Steg 1 – Köp den nya prenumerationen

1. I **menyn i Partnercenter** väljer du **Kunder,** väljer den kund som du vill flytta och väljer sedan Lägg **till prenumerationer.**

2. Välj den prenumeration som du vill köpa från katalogen (i det här fallet något av alternativen ovan), ange antalet licenser och välj sedan **Skicka.**

   Kunden bör nu ha både gamla och nya prenumerationer, den gamla Office 365 Enterprise, E4-prenumerationen och den nya målprenumerationen, till exempel alternativ 1 – Office 365 Enterprise E5.

### <a name="step-2---reassign-the-customers-users-licenses"></a>Steg 2 – Tilldela om kundens användarlicenser

1. I **menyn i Partnercenter** väljer **du Kunder,** väljer den kund som du vill flytta och väljer **sedan Användare och licenser.** Kundens sida Användare och licenser öppnas.

2. Om du vill tilldela om användarlicenser väljer du den användare som du vill tilldela om och väljer sedan **Hantera licenser.**

3. På sidan **Hantera licenser** avmarkerar du **kryssrutan Office 365 Enterprise, E4** licens och väljer en ny tjänstplan för prenumerationen som kunden flyttar till.

4. Välj **Skicka**. En bekräftelsesida visar de nya licenstilldelningarna.

5. Fortsätt på samma sätt med andra kundanvändare som behöver licensomtilldeling.

När du har flyttat användarlicenserna till den nya tjänsten kan du på ett säkert sätt avbryta den tillbakadragna prenumerationen på den högsta kundnivån.

### <a name="step-3---cancel-the-old-subscription"></a>Steg 3 – Avbryt den gamla prenumerationen

1. I **menyn i Partnercenter** väljer du **Kunder.** Välj den kund som du vill flytta och välj den prenumeration som du vill avbryta.

2. På sidan prenumerationsinformation anger du prenumerationsstatusen Till **Pausad.**

3. Välj **Skicka**.

Den gamla prenumerationen pausas och den nya prenumerationen är aktiv. Den pausade prenumerationen avetableeras automatiskt efter 120 dagar. Kunden medför inga ytterligare kostnader för den gamla prenumerationen.



 



