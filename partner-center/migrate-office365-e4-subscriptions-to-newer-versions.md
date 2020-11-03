---
title: Migrera Office 365 E4-prenumerationer
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Microsoft Office 365 Enterprise E4 Edition dras tillbaka den 7 april 2017. Lär dig hur du migrerar kund prenumerationer till nyare versioner av Office 365.
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: bbd2aceac62a7e726ed81a78305ea23213c94156
ms.sourcegitcommit: 36a60f672c1c3d6b63fd225d04c5ffa917694ae0
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 07/03/2020
ms.locfileid: "92529179"
---
# <a name="migrate-office-365-e4-subscriptions-to-newer-office-365-versions"></a>Migrera Office 365 E4-prenumerationer till senare Office 365-versioner

**Gäller för**

-  Partnercenter

**Lämpliga roller**
-   Global administratör
-   Användaradministratör
-   Administratörs agent
-   Försäljnings agent

Office 365 Enterprise E4 plan dras tillbaka, från och med 7 april 2017. Du kan inte längre köpa nya Office 365 E4-prenumerationer efter det här datumet och befintliga E4-prenumerationer kommer inte att förnyas automatiskt när de upphör att gälla.

När E4-prenumerationer slutar, kommer de att avbrytas. För att säkerställa kontinuitet för kunderna bör du överföra kunder med att förfalla E4-prenumerationer till ett SKU-alternativ som stöds, som anges nedan. Vi rekommenderar att du flyttar kunder till nya prenumerationer före prenumerationens årliga slutdatum för att undvika eventuella avbrott i tjänsten för kunderna. 

> [!NOTE]  
> Både Office 365 Enterprise E4-kommersiella och offentliga SKU: er dras tillbaka.
 
På prenumerationens informations sida har status för E4-prenumerationen ändrats till "upphör att gälla [datum]" från "Auto News på [Date]". 

Om du använder API: et (topp eller partner Center) kan du identifiera prenumerationer som upphör att gälla genom att utvärdera slutdatumet för prenumerationen tillsammans med egenskapen Auto renew = false. 

E4-prenumerationerna ställs in på automatisk förnyelse = falskt i den 7 april 2017. Du kan när som helst flytta kunder till en ny plan. 

## <a name="office-365-enterprise-e4-edition-replacement-plans"></a>Ersättnings planer för Office 365 Enterprise E4 Edition

Du kan välja att behålla samma funktioner med E4 eller låta dina kunder dra nytta av nya funktioner i Office 365 och Skype för företag – online. Pris information finns i matrisen pris lista och erbjudande lista i Partner Center. Säker produkt Enterprise E3 eller Secure produktiv Enterprise E5 kan ersättas med följande alternativ för Office 365 Enterprise E3 eller Office 365 Enterprise E5.

- Alternativ 1: Office 365 Enterprise E5

- Alternativ 2: Office 365 Enterprise E3 + Skype för företag Cloud PBX

- Alternativ 3: Office 365 Enterprise E3 + Skype för företag Plus CAL (pris-och funktions paritet med E4)

- Alternativ 4: Office 365 Enterprise E3


| Funktion | Alternativ 1 | Alternativ 2 | Alternativ 3 | Alternativ 4 |
| :---    | :------: |   :---:  |   :---:  |   :---:  |
| Hämta alla funktioner som ingår i Office 365 Enterprise E4? | Ja | Ja | Ja | Nej |
| Telefonnummer som hanteras i Office 365? | Ja | Ja | Nej | Nej |
| De telefonnummer som hanteras både lokalt och i Office 365 (hybrid distribution)? | Ja | Ja | Nej | Nej |
| Alternativ för att lägga till en PSTN-röst samtals plan? | Ja | Ja | Nej | Nej |
| PSTN-konferens? | Ja | Nej | Nej | Nej |
| Avancerade verktyg för samarbete, analys och säkerhet? | Ja | Nej | Nej | Nej |
| Interaktiva rapporter, instrument paneler och data visualiseringar? | Ja | Nej | Nej | Nej | 
| Mer kontroll över data säkerhet och efterlevnad med inbyggda sekretess-, genomskinlighets-och raffinerade användar kontroller? | Ja | Nej | Nej | Nej | 

## <a name="transition-customers-to-new-product-plans"></a>Överföra kunder till nya produkt planer

Microsoft erbjuder kontinuerligt nya produkter och tjänster till våra partner. I dessa fall kan du behöva uppgradera kunder till nya tjänster eller migrera sina prenumerationer från SKU: er som slutligen kommer att stängas av. Migrering av kunder från tillbakadragna SKU: er till nyare kräver följande steg:

-   Köp den nya prenumerationen
-   Tilldela om aktuella användar licenser
-   Avbryt den gamla prenumerationen

Följ dessa steg om du vill migrera en kunds Office 365 Enterprise E4-prenumeration till något av alternativen i tabellen ovan.

### <a name="step-1---purchase-the-new-subscription"></a>Steg 1 – Köp den nya prenumerationen

1. Från menyn **partner Center** väljer du **kunder** , väljer kunden som du vill flytta och väljer sedan **Lägg till prenumerationer** .

2. Välj den prenumeration som du vill köpa från katalogen (i det här fallet ett av alternativen ovan), ange antalet licenser och välj sedan **Skicka** .

   Kunden bör nu ha både gamla och nya prenumerationer, den gamla Office 365 Enterprise E4-prenumerationen och den nya mål prenumerationen, till exempel alternativ 1-Office 365 Enterprise E5.

### <a name="step-2---reassign-the-customers-users-licenses"></a>Steg 2 – tilldela om kundens användares licenser

1. Från menyn **partner Center** väljer du **kunder** , väljer kunden som du vill flytta och väljer sedan **användare och licenser** . Sidan kund användare och licenser öppnas.

2. Om du vill tilldela användar licenser igen väljer du den användare som ska omtilldelas och väljer sedan **Hantera licenser** .

3. På sidan **Hantera licenser** avmarkerar du kryss rutan **Office 365 Enterprise E4** -licens och väljer en ny service plan för den prenumeration som kunden flyttar till.

4. Välj **Skicka** . En bekräftelse sida listar de nya licens tilldelningarna.

5. Fortsätt på samma sätt med andra kund användare som behöver omtilldela licenser.

När du har flyttat användar licenserna till den nya tjänsten kan du på ett säkert sätt avbryta den tillbakadragna prenumerationen på den översta kund nivån.

### <a name="step-3---cancel-the-old-subscription"></a>Steg 3 – Avbryt den gamla prenumerationen

1. Från menyn **partner Center** väljer du **kunder** . Välj den kund som du vill flytta och välj den prenumeration som du vill avbryta.

2. På sidan prenumerations information anger du prenumerations statusen **pausad** .

3. Välj **Skicka** .

Den gamla prenumerationen har pausats och den nya prenumerationen är aktiv. Den inaktiverade prenumerationen kommer att avetableras automatiskt efter 120 dagar. Kunden debiteras inga ytterligare kostnader för den gamla prenumerationen.



 



