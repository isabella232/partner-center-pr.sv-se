---
title: Felsöka problem med att konfigurera ditt Partnercenter-konto eller MPN-förnyelse
ms.topic: how-to
ms.date: 08/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Felsöka problem när du försöker registrera i Partnercenter. Svar på problem med betalningsmetoder, att glömma lösenord och mycket annat.
author: ArpithaKanuganti
ms.author: v-arkanu
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: f34adc57e668caecb69af37afc72b5153f667335
ms.sourcegitcommit: 08a175c06ff4c6a2b12713f081adfa489e16e7a1
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 05/10/2021
ms.locfileid: "109686270"
---
# <a name="troubleshoot-account-setup-or-mpn-renewal-issues"></a>Felsöka problem med kontokonfiguration eller MPN-förnyelse


**Lämpliga roller**

- Global administratör
- MPN-partneradministratör
 
Här är några förslag på felsökning av vanliga problem som uppstår när du ställer in ditt Partnercenter-konto.

## <a name="what-happens-if-you-are-migrating-from-partner-membership-center-and-you-cant-edit-any-company-information-fields"></a>Vad händer om du migrerar från Partner Membership Center och du inte kan redigera fält för företagsinformation

Om ditt företag redan finns i Partnercenter (till exempel ett CSP-konto) visas en skrivskyddad skärm. På den här skärmen visas all information om ditt företag när det finns i Partnercenter.

Du kan inte ändra informationen på den här skärmen. Detta är design och inte ett fel.

Välj **Acceptera** och **Fortsätt för att** fortsätta.


### <a name="if-the-it-department-has-turned-off-sign-up-for-partner-center"></a>Om IT-avdelningen har inaktiverat **Registrering för Partnercenter**

Du ser det här meddelandet eftersom virala användare är inaktiverade eller eftersom viral registrering är inaktiverat i Azure AD-klientorganisationen. Den globala administratören för ditt Azure AD-konto kan aktivera nödvändiga funktioner genom att köra följande PowerShell-kommando:

**Set-MsolCompanySettings -AllowEmailVerifiedUsers $true -AllowAdHocSubscriptions $true**

Mer information finns i [Registrera dig för självbetjäning.](/azure/active-directory/users-groups-roles/directory-self-service-signup)

## <a name="you-forgot-your-password"></a>Du har glömt ditt lösenord

Om du har glömt ditt lösenord väljer du länken Kan du inte komma åt ditt **konto?** på inloggningssidan. Med det här alternativet kan du återställa lösenordet eller be din globala administratör att tilldela dig nya autentiseringsuppgifter.

## <a name="on-the-tell-us-about-your-company-screen-you-receive-a-something-went-wrong-error"></a>På skärmen "Berätta om ditt företag" visas felet "Något gick fel"

Det här felmeddelandet visas vanligtvis om du oavsiktligt använder specialtecken, blanksteg eller landskod i företagets telefonnummer. Värdet som anges i fältet Telefonnummer får bara innehålla högst 10 tecken.


### <a name="your-credit-card-purchase-is-receiving-an-error-message-stating-that-your-order-was-declined-please-verify-your-information"></a>Ditt kreditkortsköp får ett felmeddelande om att din beställning nekades. Verifiera din information"


Använd alltid den adress som motsvarar ditt kreditkort i stället för din juridiska person. Kontrollera också att postnumret är korrekt och motsvarar den adress som du använder.

## <a name="you-want-to-switch-from-offline-payment-to-online-payment-method"></a>Du vill växla från offlinebetalning till onlinebetalningsmetod 

Du måste avbryta den ursprungliga beställningen och göra ett återköp med den önskade betalningsmetoden.

Så här avbryter du en beställning:

1. Välj **fliken Medlemskapserbjudanden** på instrumentpanelen.

2. Välj **Avbryt beställning**

3. Ett bekräftelsefönster visas och du måste bekräfta för att kunna avbryta den första beställningen.

## <a name="next-steps"></a>Nästa steg

- [Hantera ditt Partnercenter-konto](partner-center-account-setup.md)
- [Läsa fakturan och rekognoseringsfilen](read-your-bill.md)
