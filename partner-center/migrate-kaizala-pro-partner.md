---
title: Migrera Kaizala Pro-prenumerationer till Microsoft 365
description: Lär dig hur du migrerar Kaizala Pro-prenumerationer till Microsoft 365 eller Office 365-versioner. Läs den här artikeln för mer information om hur du övergår till dina kunder.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
ms.author: sukumart
author: sukumart
ms.date: 06/01/2020
localization_priority: Normal
ms.openlocfilehash: e248657b9b4d4cf50cb7d38b2a0593ae6445bd28
ms.sourcegitcommit: ad1af627f5ee6b6e3a70655f90927e932cf4c985
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 07/29/2021
ms.locfileid: "114843144"
---
# <a name="migrate-kaizala-pro-standalone-subscriptions-to-microsoft-365-or-office-365-versions"></a>Migrera Kaizala Pro fristående prenumerationer till Microsoft 365 eller Office 365 versioner

**Lämpliga roller:** Försäljningsagent

Från och med 1 juli 2020 avslutar Microsoft försäljningen av Kaizala Pro fristående tjänsten. Kunder kommer inte längre att kunna köpa nya Kaizala Pro prenumerationer efter detta datum, och befintliga Kaizala Pro-prenumerationer förnyas inte automatiskt när de upphör att gälla.

För att säkerställa kontinuitet för kunder bör du göra så att kunderna upphör att Kaizala Pro fristående prenumerationer till ett SKU-alternativ som stöds, som anges nedan. Vi rekommenderar att du flyttar kunder till nya prenumerationer före prenumerationens årliga slutdatum för att undvika eventuella tjänstavbrott för kunder.

Om du använder API:et (antingen FALSE eller Partner Center) kan du identifiera utgående prenumerationer genom att utvärdera slutdatumet för prenumerationen tillsammans med egenskapen för automatisk förnyelse inställd på falskt: `auto renew = False` .

E4-prenumerationerna anges till `auto renew=False` den 1 juli 2020. Du kan när som helst flytta kunder till en ny plan.

## <a name="kaizala-pro-standalone-replacement-plans"></a>Kaizala Pro Fristående ersättningsplaner

Med de nya planerna kan dina kunder dra nytta av nyare funktioner i Microsoft 365. Prisinformation finns i prislistan och erbjudandelistan i Partnercenter.

- [**Microsoft 365 för företag**](https://www.microsoft.com/microsoft-365/compare-all-microsoft-365-products?&activetab=tab:primaryr2), inklusive:  
   - Microsoft 365 Business Basic
   - Microsoft 365 Business Standard
   - Microsoft 365 Business Premium
    
- [**Microsoft 365 för Frontline**](https://www.microsoft.com/microsoft-365/microsoft-365-enterprise-f3?activetab=pivot:overviewtab), inklusive:
   - Microsoft 365 F3 (tidigare Microsoft 365 F1) och Office 365 F3
    
- [**Microsoft 365 för Enterprise**](https://www.microsoft.com/microsoft-365/compare-microsoft-365-enterprise-plans), inklusive: 
   - Office 365 E1
   - Microsoft 365 E3 och Office 365 E3
   - Microsoft 365 E5 och Office 365 E5

- [**Microsoft 365 for Education**](https://www.microsoft.com/education/buy-license/microsoft365), inklusive: 
    - Microsoft 365 A1 och Office 365 A1
    - Microsoft 365 A3 och Office 365 A3
    - Microsoft 365 A5 och Office 365 A5

## <a name="transition-customers-to-new-product-plans"></a>Övergå kunder till nya produktplaner

Microsoft erbjuder kontinuerligt nya produkter och tjänster till våra partner. I dessa fall kan du behöva uppgradera kunder till nya tjänster eller migrera sina prenumerationer från SKU:er som så småningom kommer att stängas av. Migrering av kunder från tillbakadragna SKU:er till nyare kräver följande steg:

A. Köpa den nya prenumerationen

B. Tilldela om aktuella användarlicenser

C. Avbryta gammal prenumeration


## <a name="migrate-your-customers-to-new-plans"></a>Migrera dina kunder till nya planer

### <a name="a-purchase-the-new-subscription"></a>A. Köpa den nya prenumerationen

1. Om du vill köpa den nya prenumerationen går du till **Menyn i Partnercenter** och väljer **Kunder,** väljer den kund som du vill flytta och väljer sedan **Lägg till prenumerationer.**

2. Välj den prenumeration som du vill köpa från katalogen (i det här fallet något av alternativen ovan), ange antalet licenser och välj sedan **Skicka.**

Kunden bör nu ha både gamla och nya prenumerationer, den gamla fristående Kaizala Pro-prenumerationen och den nya målprenumerationen, till exempel alternativ 1 – Office 365 Enterprise F1.

### <a name="b-reassign-current-user-licenses"></a>B. Tilldela om aktuella användarlicenser

1. Om du vill tilldela om kundens användarlicenser går du till **Menyn i Partnercenter,** väljer **Kunder,** väljer den kund som du flyttar och väljer sedan **Användare och licenser.** Kundens sida Användare och licenser öppnas.

2. Om du vill tilldela om användarlicensen väljer du den användare som ska tilldelas om och väljer **sedan Hantera licenser.**

3. På sidan **Hantera licenser** avmarkerar du kryssrutan Kaizala Pro fristående licens och väljer en ny tjänstplan för prenumerationen som kunden flyttar till.

4.  Välj **Skicka**. En bekräftelsesida visar de nya licenstilldelningarna. Fortsätt samma process för andra användare som behöver licenstilldelningar.

### <a name="c-cancel-old-subscription"></a>C. Avbryta gammal prenumeration

När du har flyttat användarlicensen till den nya tjänsten kan du på ett säkert sätt avbryta den tillbakadragna prenumerationen på kundnivå.

1.  I **menyn i Partnercenter** väljer du **Kunder.** Välj den kund vars prenumeration du avbryter.

2.  På sidan med prenumerationsdetaljer ställer du in prenumerationen på **Pausad**.

3.  Välj **Skicka**.

Den gamla prenumerationen pausas och den nya prenumerationen är aktiv. Den pausade prenumerationen avetableeras automatiskt efter 120 dagar. Kunden medför inga ytterligare kostnader för den gamla prenumerationen.
