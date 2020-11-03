---
title: Felsöka konfiguration av ditt partner Center-konto eller problem med MPN-förnyelse
ms.topic: how-to
ms.date: 08/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Felsök problem när du försöker registrera dig i Partner Center. Svarar på utmaningar med betalnings metoder, Forgetting-lösenord och mycket annat.
author: ArpithaKanuganti
ms.author: v-arkanu
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: d990a2cb4dcb69dfc76e8a4f0d40fd4912b4f8a0
ms.sourcegitcommit: 3c45a181ef86b3a4866e97fb50efeae8714ab3f7
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 10/19/2020
ms.locfileid: "92531989"
---
# <a name="troubleshoot-account-setup-or-mpn-renewal-issues"></a>Felsöka konto inställningar eller problem med MPN förnyelse

**Gäller för**

- Partnercenter
 
**Lämpliga roller**

- Global administratör
- MPN-partner administratör 
 
Här följer några förslag på hur du felsöker vanliga problem som uppstår när du konfigurerar ditt partner Center-konto.

## <a name="what-happens-if-you-are-migrating-from-partner-membership-center-and-you-cant-edit-any-company-information-fields"></a>Vad händer om du migrerar från partner medlemskaps Center och du inte kan redigera företags informations fält

I de fall där ditt företag redan har en närvaro i Partner Center (säg CSP-konto) – visas en skrivskyddad skärm. Den här skärmen visar all information om ditt företag som finns i Partner Center.

Du kan inte ändra informationen på den här skärmen. Detta är avsiktligt och inte ett fel.

Välj **Godkänn** och **Fortsätt** för att fortsätta.


### <a name="if-the-it-department-has-turned-off-sign-up-for-partner-center"></a>Om IT-avdelningen har inaktiverat **registrering för partner Center** .

Du ser det här meddelandet eftersom virusbaserade användare är inaktiverade, eller om du har inaktiverat virus registrering på Azure AD-klienten. Den globala administratören för ditt Azure AD-konto kan aktivera nödvändiga funktioner genom att köra följande PowerShell-kommando:

**Set-MsolCompanySettings-AllowEmailVerifiedUsers $true-AllowAdHocSubscriptions $true**

Mer information finns i självbetjänings [registrering](/azure/active-directory/users-groups-roles/directory-self-service-signup)

## <a name="you-forgot-your-password"></a>Du har glömt ditt lösen ord

Om du har glömt ditt lösen ord väljer du länken **kan inte komma åt ditt konto?** på inloggnings sidan. Med det här alternativet kan du återställa ditt lösen ord eller be den globala administratören att tilldela nya autentiseringsuppgifter.

## <a name="on-the-tell-us-about-your-company-scree-you-receive-a-something-went-wrong-error"></a>I "berätta för oss om ditt företag"-Scree får du ett fel meddelande om att något har gått fel

Det här fel meddelandet visas vanligt vis om du oavsiktligt använder specialtecken, mellanslag eller landskod i företagets telefonnummer. Värdet som anges i fältet telefonnummer får bara innehålla högst 10 tecken.


### <a name="your-credit-card-purchase-is-receiving-an-error-message-stating-that-your-order-was-declined-please-verify-your-information"></a>Kredit korts köpet får ett fel meddelande om att "din beställning har avböjts. Verifiera din information.


Använd alltid adressen som motsvarar ditt kredit kort i stället för din juridiska person. Kontrol lera också att post numret är korrekt och motsvarar adressen som du använder.

## <a name="you-want-to-switch-from-offline-payment-to-online-payment-method"></a>Du vill växla från offline-betalning till betalnings metod online 

Du måste avbryta den ursprungliga ordern och köpa igen med hjälp av den prioriterade betalnings metoden.

Så här avbryter du en order:

1. Fliken Välj **medlemskaps erbjudanden** på instrument panelen.

2. Välj **Avbryt order**

3. Ett bekräftelse fönster visas och du måste bekräfta innan du kan avbryta den inledande ordningen.

## <a name="next-steps"></a>Nästa steg

- [Hantera ditt Partnercenter-konto](partner-center-account-setup.md)
- [Läsa din faktura-och rekognoseringar-fil](read-your-bill.md)