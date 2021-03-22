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
ms.openlocfilehash: 7d80651c4e5e4afb476dada388f23c118e0bdf25
ms.sourcegitcommit: 35fe0fdc41886f6f5af71ec74e4a4ebd245dfe1d
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/22/2021
ms.locfileid: "104768711"
---
# <a name="troubleshoot-account-setup-or-mpn-renewal-issues"></a>Felsöka konto inställningar eller problem med MPN förnyelse


**Lämpliga roller**

- Global administratör
- MPN-partner administratör 
 
Här följer några förslag på hur du felsöker vanliga problem som uppstår när du konfigurerar ditt partner Center-konto.

## <a name="what-happens-if-you-are-migrating-from-partner-membership-center-and-you-cant-edit-any-company-information-fields"></a>Vad händer om du migrerar från partner medlemskaps Center och du inte kan redigera företags informations fält

I de fall där företaget redan har en närvaro i Partner Center (till exempel ett CSP-konto) – visas en skrivskyddad skärm. Den här skärmen visar all information om ditt företag som finns i Partner Center.

Du kan inte ändra informationen på den här skärmen. Detta är avsiktligt och inte ett fel.

Välj **Godkänn** och **Fortsätt** för att fortsätta.


### <a name="if-the-it-department-has-turned-off-sign-up-for-partner-center"></a>Om IT-avdelningen har inaktiverat **registrering för partner Center**

Du ser det här meddelandet eftersom virusbaserade användare är inaktiverade, eller om du har inaktiverat virus registrering på Azure AD-klienten. Den globala administratören för ditt Azure AD-konto kan aktivera nödvändiga funktioner genom att köra följande PowerShell-kommando:

**Set-MsolCompanySettings-AllowEmailVerifiedUsers $true-AllowAdHocSubscriptions $true**

Mer information finns i självbetjänings [registrering](/azure/active-directory/users-groups-roles/directory-self-service-signup).

## <a name="you-forgot-your-password"></a>Du har glömt ditt lösen ord

Om du har glömt ditt lösen ord väljer du länken **kan inte komma åt ditt konto?** på inloggnings sidan. Med det här alternativet kan du återställa ditt lösen ord eller be den globala administratören att tilldela nya autentiseringsuppgifter.

## <a name="on-the-tell-us-about-your-company-screen-you-receive-a-something-went-wrong-error"></a>På skärmen "berätta för oss om ditt företag" visas fel meddelandet "något gick fel"

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
