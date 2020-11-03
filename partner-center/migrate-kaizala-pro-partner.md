---
title: Migrera Kaizala Pro-prenumerationer till Microsoft365
description: Lär dig hur du migrerar Kaizala Pro-prenumerationer till Microsoft365-eller Office 365-versioner. Läs den här artikeln om du vill ha mer information om att överföra dina kunder.
ms.topic: article
ms.service: partner-dashboard
ms.author: sukumart
author: sukumart
ms.date: 06/01/2020
localization_priority: Normal
ms.openlocfilehash: 0807931ae95b5c7d76f4ad33708cc8014412f55f
ms.sourcegitcommit: 3c45a181ef86b3a4866e97fb50efeae8714ab3f7
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 10/19/2020
ms.locfileid: "92532032"
---
# <a name="migrate-kaizala-pro-standalone-subscriptions-to-microsoft365-or-office-365-versions"></a>Migrera Kaizala Pro fristående prenumerationer till Microsoft365-eller Office 365-versioner

Från och med den 1 juli 2020 avslutas Microsoft Sales of Kaizala Pro standalone service. Kunder kommer inte längre att kunna köpa nya Kaizala Pro-prenumerationer efter det här datumet och befintliga Kaizala Pro-prenumerationer förnyas inte automatiskt när de upphör att gälla.

För att säkerställa kontinuitet för kunderna bör du gå över till kunder med att förfalla Kaizala Pro fristående prenumerationer till ett SKU-alternativ som stöds, som anges nedan. Vi rekommenderar att du flyttar kunder till nya prenumerationer före prenumerationens årliga slutdatum för att undvika eventuella avbrott i tjänsten för kunderna.

Om du använder API: et (topp eller partner Center) kan du identifiera prenumerationer som upphör att gälla genom att utvärdera slutdatumet för prenumerationen tillsammans med egenskapen för automatisk förnyelse inställd på falskt: `auto renew = False` .

E4-prenumerationerna sätts till `auto renew=False` den 1 juli 2020. Du kan när som helst flytta kunder till en ny plan.

## <a name="kaizala-pro-standalone-replacement-plans"></a>Kaizala Pro fristående ersättnings planer

Med de nya planerna kan dina kunder dra nytta av nya funktioner och funktioner i Microsoft 365. Pris information finns i matrisen pris lista och erbjudande lista i Partner Center.

- [**Microsoft 365 för företag**](https://www.microsoft.com/microsoft-365/compare-all-microsoft-365-products?&activetab=tab:primaryr2), inklusive:  
   - Microsoft 365 Business Basic
   - Microsoft 365 Business Standard
   - Microsoft 365 Business Premium
    
- [**Microsoft 365 för Frontline**](https://www.microsoft.com/microsoft-365/microsoft-365-enterprise-f3?activetab=pivot:overviewtab), inklusive:
   - Microsoft 365 F3 (tidigare Microsoft 365 F1) och Office 365 F3
    
- [**Microsoft 365 för företag**](https://www.microsoft.com/microsoft-365/compare-microsoft-365-enterprise-plans), inklusive: 
   - Office 365 E1
   - Microsoft 365 E3 och Office 365 E3
   - Microsoft 365 E5 och Office 365 E5

- [**Microsoft 365 för utbildning**](https://www.microsoft.com/education/buy-license/microsoft365), inklusive: 
    - Microsoft 365 a1 och Office 365 a1
    - Microsoft 365 a3 och Office 365 a3
    - Microsoft 365 A5 och Office 365 A5

## <a name="transition-customers-to-new-product-plans"></a>Överföra kunder till nya produkt planer

Microsoft erbjuder kontinuerligt nya produkter och tjänster till våra partner. I dessa fall kan du behöva uppgradera kunder till nya tjänster eller migrera sina prenumerationer från SKU: er som slutligen kommer att stängas av. Migrering av kunder från tillbakadragna SKU: er till nyare kräver följande steg:

A. Köp den nya prenumerationen

B. Tilldela om aktuella användar licenser

C. Avbryt gammal prenumeration


## <a name="migrate-your-customers-to-new-plans"></a>Migrera dina kunder till nya planer

### <a name="a-purchase-the-new-subscription"></a>A. Köp den nya prenumerationen

1. Om du vill köpa den nya prenumerationen väljer du **kunder** från menyn **partner Center** och väljer kunden som du vill flytta. Välj sedan **Lägg till prenumerationer** .

2. Välj den prenumeration som du vill köpa från katalogen (i det här fallet ett av alternativen ovan), ange antalet licenser och välj sedan **Skicka** .

Kunden bör nu ha både gamla och nya prenumerationer, den gamla fristående Kaizala Pro-prenumerationen och den nya mål prenumerationen, till exempel alternativ 1 – Office 365 Enterprise F1.

### <a name="b-reassign-current-user-licenses"></a>B. Tilldela om aktuella användar licenser

1. Om du vill tilldela om kundens användares licenser går du till menyn **partner Center** och väljer **kunder** , väljer kunden som du flyttar och väljer sedan **användare och licenser** . Sidan kund användare och licenser öppnas.

2. Om du vill omtilldela användar licensen väljer du den användare som ska omtilldelas och väljer sedan **Hantera licenser** .

3. På sidan **Hantera licenser** avmarkerar du kryss rutan Kaizala Pro standalone License och väljer en ny service plan för den prenumeration som kunden flyttar till.

4.  Välj **Skicka** . En bekräftelse sida listar de nya licens tilldelningarna. Fortsätt med samma process för andra användare som behöver licens tilldelningar.

### <a name="c-cancel-old-subscription"></a>C. Avbryt gammal prenumeration

När du har flyttat användar licensen till den nya tjänsten kan du på ett säkert sätt avbryta den tillbakadragna prenumerationen på kund nivå.

1.  Från menyn **partner Center** väljer du **kunder** . Välj den kund vars prenumeration du vill avbryta.

2.  På sidan prenumerations information ställer du in prenumerationen på **pausad** .

3.  Välj **Skicka** .

Den gamla prenumerationen har pausats och den nya prenumerationen är aktiv. Den inaktiverade prenumerationen kommer att avetableras automatiskt efter 120 dagar. Kunden debiteras inga ytterligare kostnader för den gamla prenumerationen.
