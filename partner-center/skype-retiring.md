---
title: Migrera vissa Skype för företag-prenumerationer
description: Lär dig hur och när du ska migrera vissa kunder med att gå ut prenumerationer på Skype för företag Online abonnemang 1 till nya Office 365-versioner.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 06/03/2020
ms.openlocfilehash: 67c1689136892443937748b6cc9e31e4f0ac9983
ms.sourcegitcommit: ec33c2352a9dd3e5a941f0f42ff1e8d256bb2399
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/24/2021
ms.locfileid: "105028425"
---
# <a name="migrate-skype-for-business-online-plan-1-subscriptions-to-newer-office-365-versions"></a>Migrera Skype för företag – Online, plan 1-prenumerationer till senare Office 365-versioner

Abonnemang 1 för Skype för företag – Online kommer att dras tillbaka den 1 augusti 2018. Efter det datumet kan kunder inte längre köpa nya prenumerationer på Skype för företag, och befintliga prenumerationer förnyas inte automatiskt när de går ut och kommer inte att tillhandahålla ett förnyelse alternativ. På prenumerationens informations sida har prenumerations statusen för Skype för Business Online abonnemang 1 ändrats till "upphör att gälla [datum]" från "Auto renyheterna på [Date]".  

För att säkerställa kontinuitet för kunderna bör du gå över till kunder med att gå ut för prenumerationer på Skype för företag Online abonnemang 1 till ett SKU-alternativ som stöds, som anges nedan. Vi rekommenderar att du flyttar kunder till nya prenumerationer före prenumerationens årliga slutdatum för att undvika eventuella avbrott i tjänsten för kunderna. 

>[!NOTE]
>Både Skype for Business Online abonnemang 1 är kommersiellt och myndighets SKU: er dras tillbaka.

Om du använder API: et (topp-eller partner Center) hittar du prenumerationer som upphör att gälla genom att utvärdera slutdatumet för prenumerationen tillsammans med egenskapen Auto renew = false. Prenumeration 1 på Skype för företag – Online abonnemang 1 kommer att ställas in på automatisk förnyelse = falskt den 1 september 2018. Du kan när som helst flytta kunder till en ny plan. 

## <a name="skype-for-business-online-plan-1-replacement-plans"></a>Ersättnings planer för Skype för företag – Online abonnemang 1

Med de nya planerna kan dina kunder dra nytta av nya funktioner och funktioner i Office 365. Pris information finns i matrisen pris lista och erbjudande lista i Partner Center. 

- Alternativ 1: Office 365 Enterprise F1
- Alternativ 2: Microsoft 365 Enterprise F1
- Alternativ 3: andra Office 365-planer

|**Funktion**    |**Alternativ 1**   |**Alternativ 2**   |**Alternativ 3**   |
|:-----------------|:-----------------|:-------------|:------------|
|Hämta alla funktioner som ingår i Skype för företag – Online abonnemang 1|Ja   |Ja   |Ja   |
|Snabb meddelanden och närvaro |Ja   |Ja   |Ja   |
|Peer-to-peer-ljud och video över IP|Ja   |Ja   |Ja   
|Anslut till möten som en autentiserad användare| Ja   |Ja   |Ja   |

## <a name="transition-customers-to-new-product-plans"></a>Överföra kunder till nya produkt planer

Microsoft erbjuder kontinuerligt nya produkter och tjänster till våra partner. I dessa fall kan du behöva uppgradera kunder till nya tjänster eller migrera sina prenumerationer från SKU: er som slutligen kommer att stängas av. Migrering av kunder från tillbakadragna SKU: er till nyare kräver följande steg:

- Köp den nya prenumerationen
- Tilldela om aktuella användar licenser
- Avbryt gammal prenumeration

### <a name="migrate-your-customers-to-new-plans"></a>Migrera dina kunder till nya planer

1. Om du vill köpa den nya prenumerationen väljer du **kunder** från **menyn Partner Center** och väljer kunden som du vill flytta. Välj sedan **Lägg till prenumerationer**.

2. Välj den prenumeration som du vill köpa från katalogen (i det här fallet ett av alternativen ovan), ange antalet licenser och välj sedan **Skicka**. 

Kunden bör nu ha både gamla och nya prenumerationer, den gamla prenumerationen på Skype för företag – Online abonnemang 1 och den nya mål prenumerationen, till exempel alternativ 1 – Office 365 Enterprise F1.

3. Om du vill tilldela om kundens användares licenser går du till menyn **partner Center** och väljer **kunder**, väljer kunden som du flyttar och väljer sedan **användare och licenser**. Sidan kund användare och licenser öppnas.

4. Om du vill omtilldela användar licensen väljer du den användare som ska omtilldelas och väljer sedan **Hantera licenser.**

5. På sidan **Hantera licenser** avmarkerar du kryss rutan licens för Skype för företag – Online abonnemang 1 och väljer en ny service plan för den prenumeration som kunden flyttar till.

6. Välj **Skicka**. En bekräftelse sida listar de nya licens tilldelningarna. Fortsätt med samma process för andra användare som behöver licens tilldelningar.

När du har flyttat användar licensen till den nya tjänsten kan du på ett säkert sätt avbryta den tillbakadragna prenumerationen på kund nivå.

7. Från menyn **partner Center** väljer du **kunder**. Välj den kund vars prenumeration du vill avbryta.

8. På sidan prenumerations information ställer du in prenumerationen på **pausad**.

9. Välj **Skicka.**

Den gamla prenumerationen har pausats och den nya prenumerationen är aktiv. Den inaktiverade prenumerationen kommer att avetableras automatiskt efter 120 dagar. Kunden debiteras inga ytterligare kostnader för den gamla prenumerationen.

