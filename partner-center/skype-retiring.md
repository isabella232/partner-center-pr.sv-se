---
title: Migrera Skype för företag-prenumerationer
description: Lär dig hur och när du ska migrera vissa kunder med utgående Skype för företag – Online, abonnemang 1 till nya Office 365-versioner.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 06/03/2020
ms.openlocfilehash: a8de5b824a24b07607b5365848ec1027ca0d08e8
ms.sourcegitcommit: 8dc9f28f15d9760a8363826513b4470b76b40ff3
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/23/2021
ms.locfileid: "112551545"
---
# <a name="migrate-skype-for-business-online-plan-1-subscriptions-to-newer-office-365-versions"></a>Migrera Skype för företag – Online, plan 1-prenumerationer till senare Office 365-versioner

**Lämpliga roller:** Försäljningsagent

Skype för företag – Online, abonnemang 1 dras tillbaka från och med 1 augusti 2018. Efter det datumet kan kunder inte längre köpa nya Skype för företag Abonnemang 1-prenumerationer, och befintliga prenumerationer förnyas inte automatiskt när de upphör att gälla och kommer inte att tillhandahålla ett förnyelsealternativ. På prenumerationens informationssida har prenumerationsstatusen för Skype för företag – Online, abonnemang 1 ändrats till "Upphör [datum]" från "Förnyas automatiskt [datum]".  

För att säkerställa kontinuitet för kunder bör du föra över kunder med utgående Prenumerationer på Skype för företag – Online, abonnemang 1 till ett SKU-alternativ som stöds, som anges nedan. Vi rekommenderar att du flyttar kunder till nya prenumerationer före prenumerationens årliga slutdatum för att undvika eventuella tjänstavbrott för kunder. 

>[!NOTE]
>Både kommersiella SKU:er och myndighets-SKU:er för Skype för företag – Online, abonnemang 1 dras tillbaka.

Om du använder API:et (antingen Commerce REST (NINGS REST) eller Partnercenter) kan du hitta utgångna prenumerationer genom att utvärdera slutdatumet för prenumerationen tillsammans med egenskapen för automatisk förnyelse = Falskt. Prenumerationen på Skype för företag – Online, abonnemang 1 ställs in på förnya automatiskt = Falskt den 1 september 2018. Du kan när som helst flytta kunder till en ny plan. 

## <a name="skype-for-business-online-plan-1-replacement-plans"></a>Ersättningsplaner för Skype för företag – Online, plan 1

Med de nya planerna kan dina kunder dra nytta av nyare funktioner och funktioner i Office 365. Prisinformation finns i prislistan och erbjudandelistan i Partnercenter. 

- Alternativ 1: Office 365 Enterprise F1
- Alternativ 2: Microsoft 365 Enterprise F1
- Alternativ 3: Andra Office 365-planer

|**Funktion**    |**Alternativ 1**   |**Alternativ 2**   |**Alternativ 3**   |
|:-----------------|:-----------------|:-------------|:------------|
|Hämta alla funktioner som ingår i Skype för företag – Online, abonnemang 1|Ja   |Ja   |Ja   |
|Snabbmeddelanden och närvaro |Ja   |Ja   |Ja   |
|Peer-to-peer-ljud och video över IP|Ja   |Ja   |Ja   
|Ansluta till möten som en autentiserad användare| Ja   |Ja   |Ja   |

## <a name="transition-customers-to-new-product-plans"></a>Övergå kunder till nya produktplaner

Microsoft erbjuder kontinuerligt nya produkter och tjänster till våra partner. I dessa fall kan du behöva uppgradera kunder till nya tjänster eller migrera sina prenumerationer från SKU:er som så småningom kommer att stängas av. Migrering av kunder från tillbakadragna SKU:er till nyare kräver följande steg:

- Köpa den nya prenumerationen
- Tilldela om aktuella användarlicenser
- Avbryta gammal prenumeration

### <a name="migrate-your-customers-to-new-plans"></a>Migrera dina kunder till nya planer

1. Om du vill köpa den nya prenumerationen går du till **Menyn i Partnercenter** och väljer **Kunder,** väljer den kund som du vill flytta och väljer sedan **Lägg till prenumerationer.**

2. Välj den prenumeration som du vill köpa från katalogen (i det här fallet något av alternativen ovan), ange antalet licenser och välj sedan **Skicka.** 

Kunden bör nu ha både gamla och nya prenumerationer, den gamla Prenumerationen på Skype för företag – Online, abonnemang 1 och den nya målprenumerationen, till exempel Alternativ 1 – Office 365 Enterprise F1.

3. Om du vill tilldela om kundens användarlicenser går du till **Menyn i Partnercenter,** väljer **Kunder,** väljer den kund som du flyttar och väljer sedan **Användare och licenser.** Kundens sida Användare och licenser öppnas.

4. Om du vill tilldela om användarlicensen väljer du den användare som ska tilldelas om och väljer sedan **Hantera licenser.**

5. På sidan **Hantera licenser** avmarkerar du kryssrutan Skype för företag – Online, abonnemang 1 och väljer en ny tjänstplan för prenumerationen som kunden flyttar till.

6. Välj **Skicka**. En bekräftelsesida visar de nya licenstilldelningarna. Fortsätt samma process för andra användare som behöver licenstilldelningar.

När du har flyttat användarlicensen till den nya tjänsten kan du på ett säkert sätt avbryta den tillbakadragna prenumerationen på kundnivå.

7. I **menyn i Partnercenter** väljer du **Kunder.** Välj den kund vars prenumeration du avbryter.

8. På sidan med prenumerationsdetaljer ställer du in prenumerationen på **Pausad**.

9. Välj **Skicka.**

Den gamla prenumerationen pausas och den nya prenumerationen är aktiv. Den pausade prenumerationen avetableeras automatiskt efter 120 dagar. Kunden medför inga ytterligare kostnader för den gamla prenumerationen.

## <a name="next-steps"></a>Nästa steg

- [Rådgivare: Skapa och skicka en utvärderingsinbjudan för klienter att testa Office 365](advisors-create-a-trial-invitation.md)
- [Rådgivare: Skapa din klientbas med Office 365-utvärderingsinbjudningar och inköpserbjudanden](advisors-build-your-business.md)
- [Rådgivare: Skapa ett inköpserbjudande](advisor-create-a-purchase-offer.md)
