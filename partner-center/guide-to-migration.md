---
title: Migrera från PMC till Partnercenter
ms.topic: article
ms.date: 10/02/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Lär dig hur du migrerar ditt företag från Partner Membership Center (PMC) till Partnercenter, inklusive de steg du behöver följa.
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 511612042f7da5e43d045d2991fa7d5251612726
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 05/19/2021
ms.locfileid: "110150751"
---
# <a name="guide-to-migrating-from-pmc-to-partner-center"></a>Guide för att flytta från PMC till Partnercenter

**Lämpliga roller:** Global administratör

Microsofts partnerwebbplats på partner.microsoft.com är en enhetlig digital upplevelse för partner. Från partnerwebbplatsen kommer du att kunna utforska dina möjligheter och delta i guidade upplevelser som hjälper ditt företag att bygga och sälja dina appar och tjänster med Microsoft. Med hjälp av länken Instrumentpanel som är tillgänglig på partnerwebbplatsen kan medlemmar i Microsoft Partner Network logga in på partnercentret där du hanterar din relation med Microsoft, registrerar dig för program och registrerar dig för erbjudanden.

Partner Membership Center (PMC) inaktiveras. Ditt företag har bjudits in att övergå Microsoft Partner Network för medlemskapshantering till Partnercenter. Den här guiden förbereder dig för vad du kan förvänta dig när du flyttar från PMC till Partnercenter.

>[!NOTE]
>Även om ditt företag har fler än ett konto eller en plats börjar flytten till Partnercenter genom att flytta ett (ditt första) konto till Partnercenter.

## <a name="get-started"></a>Kom igång

Flytten börjar i PMC. Den globala administratören får en inbjudan att påbörja flytten.

### <a name="prepare-in-pmc"></a>Förbereda i PMC

- Verifiera företagets information
- Verifiera den primära programkontakten
- Verifiera företagsplatser
- Uppdatera dina godkända användare

### <a name="when-youre-ready"></a>När du är klar

Välj **Kom igång** med din inbjudan. Du kommer till inloggningssidan i Partnercenter.

:::image type="content" source="images/migration/getstarted.jpg" alt-text="Komma igång":::

## <a name="start-with-your-work-email"></a>Börja med din e-postadress för arbetet

Om ditt företag inte har någon e-postadress till arbetet och AAD-klientorganisationen kan vi hjälpa dig att konfigurera en under inloggningsprocessen i Partnercenter. När du försöker logga in med ett e-postkonto som inte är en e-postadress för arbetet, till exempel ditt personliga konto, kommer du att dirigeras att ange information om ditt företag så att vi kan konfigurera en AAD-klientorganisation och e-post för arbetet. Den här företagsinformation används för att slutföra ditt konto i Partnercenter, så se till att de är korrekta.

>[!NOTE]
>Om du är en partner i Kina och har registrerats i både Microsoft Partner Network- och Molnlösningsleverantör-programmet (CSP) har du en separat klientorganisation för varje konto. Ditt konto med Molnlösningsleverantör Program hanteras i det nationella molnet och ditt Microsoft Partner Network-konto hanteras i det globala molnet. De två kontona kan inte länkas.

:::image type="content" source="images/migration/newtellusabout.png" alt-text="Berätta om ditt företag":::

När du har verifierat eller uppdaterat informationen väljer du **Acceptera och fortsätter**.
Villkoren på den här sidan är **exakt desamma som de** avtal som ditt företag redan har loggat in på PMC.  
Det här steget initierar skapandet av din Azure AD-klientorganisation och ger dig arbetskontot.

Om **du väljer Acceptera och** fortsätta så gör även följande:

- Migrerar ditt konto tillsammans med ALLA dess platser till Partnercenter

- Migrerar eventuella kompetenser eller MAPs som du kanske har köpt i PMC

- Migrerar alla marknadsföringsresurser, erbjudanden och program (MAPs, Silver, Gold) som du hade i PMC

## <a name="invite-employees-to-join-you"></a>Bjud in anställda att ansluta till dig

När din nya Azure AD-klient har skapats kan du bjuda in dina anställda att logga in på Partnercenter.

:::image type="content" source="images/migration/invite.png" alt-text="Bjud in anställda":::

Om du har loggat in med en befintlig AAD-klientorganisation kommer dina anställda att ha flyttat med dig. I det här fallet tilldelar du dina anställda roller för att hantera vad de kan göra i Partnercenter. 

>[!NOTE] 
>Roller i Partnercenter skiljer sig från roller i PMC. Mer information finns i [Moving from PMC to Partner Center (Flytta från PMC till Partnercenter).](move-pmc-pc-map.md)

## <a name="verify-your-domain-and-become-a-global-admin"></a>Verifiera din domän och bli global administratör  

Om din AAD-klientorganisation är ny tilldelas ingen rollen som global administratör. För att bli global administratör måste du verifiera ditt domänägarskap. Du kan behöva domänadministratören för att hjälpa dig med detta.

Du kan använda erbjudanden som du redan har köpt, men du kommer inte att kunna köpa några nya erbjudanden förrän du har slutfört steget med att tilldela en global administratör.

:::image type="content" source="images/migration/takecontrol.png" alt-text="Ta kontroll":::

När du väljer Kom igång visas följande skärm:

:::image type="content" source="images/migration/verifytxt.png" alt-text="Verifiera domänägarskap":::

Domänregistratorn är redan ifylld åt dig. Endast domänägaren kan uppdatera DNS-filen, så genom att kopiera och lägga till textfilen i DNS-posten kan vi kontrollera att du är ägaren. Det tar några minuter för uppdateringen att ske. Du måste logga ut från Partnercenter och sedan logga in igen. Din roll har ändrats till global administratör.

## <a name="get-acquainted-with-your-dashboard-and-partner-center"></a>Bekanta dig med din instrumentpanel och Partnercenter

Ta rundturen på instrumentpanelen. Här kan du hantera ditt medlemskap, lägga till en företagsprofil för hänvisningar, registrera dig i Molnlösningsleverantör-programmet och se meddelanden och erbjudanden som är relevanta för ditt företag när som helst genom att välja **Instrumentpanel.** Du kan också hantera incitament, köpa på marketplace, registrera dig för marknadstjänster med mera.  

:::image type="content" source="images/migration/fre.png" alt-text="Ta rundturen":::

## <a name="sign-the-microsoft-partner-agreement"></a>Signera Microsoft-partneravtal

Om du är en indirekt återförsäljare när du har ställt in ditt Partnercenter-konto måste du fortfarande registrera dig officiellt i Molnlösningsleverantör-programmet. Om du vill kontrollera medlemskapsstatusen går du [till din juridiska profil](https://partner.microsoft.com/pcv/accountsettings/partnerprofile) och bekräftar kontotypen. Registrera dig sedan i CSP som en [indirekt återförsäljare.](enrolling-in-the-csp-program.md)

 När du har registrerat dig som indirekt återförsäljare godkänner du [CSP-relationsbegäran hos din indirekta leverantör.](indirect-reseller-tasks-in-partner-center.md)

Godkänn sedan autentiseringsuppgifterna Microsoft-partneravtal i instrumentpanelen [i](https://partner.microsoft.com/pvc/dashboard) Partnercenter med hjälp av autentiseringsuppgifter för global administratör. Bekräfta att du har signerat Microsoft-partneravtal i avsnittet Programinformation i Partnerprofil. Dessutom visas ett bekräftelsemeddelande på översiktssidan för CSP. 

## <a name="next-steps"></a>Nästa steg

- [Hitta din globala administratör](become-global-admin.md)

- [Microsoft-partneravtal](microsoft-partner-agreement.md)

- [Skapa användarkonton](create-user-accounts-and-set-permissions.md)

- [Tilldela användarroller och behörigheter](permissions-overview.md)

- [Hantera dina medlemskapsprogram](renew-mpn-offers.md)

- [Skapa företagets företagsprofil](create-a-marketing-profile.md)

- [Ansluta till kunder via hänvisningar](manage-leads.md)

- [Guide för att migrera flera företag från PMC till Partnercenter](move-multiple-companies.md)
