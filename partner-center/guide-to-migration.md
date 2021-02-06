---
title: Migrera från PMC till Partner Center
ms.topic: article
ms.date: 10/02/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Lär dig hur du migrerar ditt företag från partner Membership Center (PMC) till Partner Center, inklusive de steg som du måste följa.
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: dd566a6d9ef60747eb7fd515b4d63d87d991da2a
ms.sourcegitcommit: d37a3f353426e52dfbbac577b7576f9c3f6d2ddf
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 02/06/2021
ms.locfileid: "99624195"
---
# <a name="guide-to-migrating-from-pmc-to-partner-center"></a>Guide för att flytta från PMC till Partnercenter

**Lämpliga roller**

- Global administratör

Microsofts partner webbplats på partner.microsoft.com är en enhetlig digital upplevelse för partner. Från partner webbplatsen kan du utforska dina affärs möjligheter och delta i guidade upplevelser som hjälper företaget att bygga och sälja dina appar och tjänster med Microsoft. Med hjälp av den instrument panels länk som är tillgänglig på partner webbplatsen kan medlemmar i Microsoft Partner Network logga in på Partner Center där du hanterar din relation med Microsoft, registrera dig i program och registrera dig för erbjudanden.

Partner medlemskaps Center (PMC) tas ur bruk. Ditt företag har bjudits in för att överföra din Microsoft Partner Network medlemskaps hantering till Partner Center. Den här guiden förbereder dig för vad du kan förväntar dig när du gör flytten från PMC till Partner Center.

>[!NOTE]
>Även om ditt företag har fler än ett konto eller en plats, börjar flytten till Partner Center genom att flytta ett (ditt första) konto till Partner Center.

## <a name="get-started"></a>Kom igång

Flytten börjar i PMC. Din globala administratör får en inbjudan att påbörja flytten.

### <a name="prepare-in-pmc"></a>Förbered i PMC

- Verifiera företagets information
- Verifiera primär program kontakt
- Verifiera företags platser
- Uppdatera dina godkända användare

### <a name="when-youre-ready"></a>När du är klar

Välj **Kom igång** i din inbjudan. Du kommer till inloggnings sidan för partner Center.

:::image type="content" source="images/migration/getstarted.jpg" alt-text="Komma igång":::

## <a name="start-with-your-work-email"></a>Börja med din e-postadress för arbetet

Om ditt företag inte har en e-postklient för arbete och AAD, kan vi hjälpa dig att konfigurera ett steg under inloggnings processen för partner Center. När du försöker logga in med ett e-postkonto som inte är ett e-postkonto för arbetet, till exempel ditt personliga konto, kommer du att omdirigeras till att ge information om ditt företag så att vi kan konfigurera en AAD-klient och ett e-postmeddelande för arbetet. Företags informationen kommer att användas för att slutföra ditt konto i Partner Center, så se till att de är korrekta.

>[!NOTE]
>Om du är en partner i Kina och registrerat i både Microsoft Partner Network-och Cloud Solution Provider (CSP)-programmet har du en separat klient för varje konto. Ditt konto med Cloud Solution Provider-programmet hanteras i det nationella molnet och ditt Microsoft Partner Networks konto hanteras i det globala molnet. De två kontona kan inte länkas.

:::image type="content" source="images/migration/newtellusabout.png" alt-text="Berätta för oss om ditt företag":::

När du har verifierat eller uppdaterat informationen väljer du **Godkänn och fortsätt**.
Villkoren på den här sidan är **exakt samma** som det avtal som ditt företag redan har loggat in på PMC.  
Det här steget startar skapandet av din Azure AD-klient och ger ditt arbets konto.

När du väljer **Godkänn och fortsätt** görs även följande:

- Migrerar ditt konto och alla dess platser till Partner Center

- Migrerar alla kompetenser eller MAPs som du kanske har köpt i PMC

- Migrerar eventuella marknadsförings resurser, erbjudanden och program (kartor, silver, guld) som du hade i PMC

## <a name="invite-employees-to-join-you"></a>Bjud in medarbetare att delta

När du har skapat din nya Azure AD-klient kan du bjuda in dina anställda att logga in på Partner Center.

:::image type="content" source="images/migration/invite.png" alt-text="Bjud in anställda":::

Om du har loggat in med en befintlig AAD-klient har dina anställda flyttat med dig. I det här fallet tilldelar du dina anställda roller som avgör vad de kan göra i Partner Center. 

>[!NOTE] 
>Roller i Partner Center skiljer sig från roller i PMC. Mer information finns i [flytta från PMC till Partner Center](move-pmc-pc-map.md).

## <a name="verify-your-domain-and-become-a-global-admin"></a>Verifiera din domän och bli global administratör  

Om din AAD-klient är ny, tilldelas ingen rollen global administratör. För att bli global administratör måste du verifiera din domän ägarskap. Du kan behöva domän administratören för att hjälpa dig med detta.

Även om du kan använda de erbjudanden du redan har köpt kommer du inte att kunna köpa några nya erbjudanden förrän du har slutfört steget med att tilldela en global administratör.

:::image type="content" source="images/migration/takecontrol.png" alt-text="Ta kontroll":::

När du väljer kom igång visas följande skärm bild:

:::image type="content" source="images/migration/verifytxt.png" alt-text="Verifiera domänägarskap":::

Din domän registrator är redan ifylld för dig. Det är bara domän ägaren som kan uppdatera DNS-filen, så genom att kopiera och lägga till text filen i din DNS-post kan vi verifiera att du är ägare. Det tar några minuter innan uppdateringen sker. Du måste logga ut från Partner Center och sedan logga in igen. Din roll kommer att ha ändrats till global administratör.

## <a name="get-acquainted-with-your-dashboard-and-partner-center"></a>Bekanta dig med instrument panelen och partner Center

Ta en rundtur på din instrument panel. Här kan du hantera ditt medlemskap, lägga till en affärs profil för hänvisningarna, registrera dig i Cloud Solution Provider-programmet och se meddelanden och erbjudanden som är relevanta för din verksamhet när som helst genom att välja **instrument panel**. Du kan också hantera incitament, köpa på Marketplace och registrera dig för go-to-Marketing-tjänster med mera.  

:::image type="content" source="images/migration/fre.png" alt-text="Ta en rundtur":::

## <a name="sign-the-microsoft-partner-agreement"></a>Signera Microsoft partner Agreement

Om du är en indirekt åter försäljare måste du fortfarande officiellt registrera dig i Cloud Solution Provider-programmet när du har konfigurerat ditt partner Center-konto. Kontrol lera medlemskapets status genom att gå till din [juridiska profil](https://partner.microsoft.com/pcv/accountsettings/partnerprofile) och bekräfta konto typen. Registrera sedan i CSP som en [indirekt åter försäljare](enrolling-in-the-csp-program.md).

 När du har registrerat dig som en indirekt åter försäljare accepterar du [begäran om CSP-relation med den indirekta providern](indirect-reseller-tasks-in-partner-center.md).

Godkänn sedan Microsoft partner Agreement i Översikt över [instrument panelen](https://partner.microsoft.com/pvc/dashboard) i Partner Center med hjälp av globala administratörsautentiseringsuppgifter. Bekräfta att du har undertecknat Microsoft partner Agreement i avsnittet program information i partner profilen. Dessutom visas ett meddelande om aviseringar på sidan CSP-översikt. 

## <a name="next-steps"></a>Nästa steg

- [Hitta din globala administratör](become-global-admin.md)

- [Microsoft-partneravtal](microsoft-partner-agreement.md)

- [Skapa användarkonton](create-user-accounts-and-set-permissions.md)

- [Tilldela användarroller och behörigheter](permissions-overview.md)

- [Hantera dina medlemskaps program](renew-mpn-offers.md)

- [Skapa företagets företags profil](create-a-marketing-profile.md)

- [Ansluta till kunder via hänvisningar](manage-leads.md)

- [Guide för att migrera flera företag från PMC till Partner Center](move-multiple-companies.md)
