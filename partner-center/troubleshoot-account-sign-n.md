---
title: Felsöka problem med att konfigurera ditt PartnerCenter-konto eller MPN-förnyelse
ms.topic: how-to
ms.date: 09/27/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-enroll
description: Felsöka problem när du försöker registrera i Partnercenter. Svar på problem med betalningsmetoder, att glömma lösenord med mera.
author: ParthP
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: d57cec763db2c22b08ec7cc5ae1b6f39c697811f
ms.sourcegitcommit: e1da62b36420d78bf44e3962358d0af65ebc3402
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/27/2021
ms.locfileid: "129088526"
---
# <a name="troubleshoot-account-setup-or-mpn-renewal-issues"></a>Felsöka problem med kontokonfiguration eller MPN-förnyelse

**Lämpliga roller:** Global | MPN-partneradministratör

Här är några förslag på felsökning av vanliga problem som uppstår när du ställer in ditt Partnercenter-konto.

## <a name="what-happens-if-you-are-migrating-from-partner-membership-center-and-you-cant-edit-any-company-information-fields"></a>Vad händer om du migrerar från Partner Membership Center och du inte kan redigera fält för företagsinformation

I fall där ditt företag redan finns i Partnercenter (till exempel ett Molnlösningsleverantör-konto (CSP) – visas en skrivskyddad skärm. Den här skärmen visar all information om ditt företag som det finns i Partnercenter.

Du kan inte ändra informationen på den här skärmen. Detta är enligt design och inte ett fel.

Fortsätt genom att **välja Acceptera** och sedan **Fortsätt.**

### <a name="if-the-it-department-has-turned-off-sign-up-for-partner-center"></a>Om IT-avdelningen har inaktiverat **Registrera dig för Partnercenter**

Du ser det här meddelandet eftersom virala användare är inaktiverade eller eftersom viral registrering har inaktiverats på Azure Active Directory klientorganisationen (AD). Den globala administratören för ditt Azure AD-konto kan aktivera nödvändiga funktioner genom att köra följande PowerShell-kommando:

**Set-MsolCompanySettings -AllowEmailVerifiedUsers $true -AllowAdHocSubscriptions $true**

Mer information finns i [Registrera dig för självbetjäning.](/azure/active-directory/users-groups-roles/directory-self-service-signup)

## <a name="you-forgot-your-password"></a>Du har glömt ditt lösenord

Om du har glömt ditt lösenord går du till inloggningssidan och väljer **Kan du inte komma åt ditt konto?**. Med det här alternativet kan du återställa lösenordet eller be din globala administratör att tilldela dig nya autentiseringsuppgifter.

## <a name="on-the-tell-us-about-your-company-screen-you-receive-a-something-went-wrong-error"></a>På skärmen "Berätta om ditt företag" visas felet "Något gick fel"

Det här felmeddelandet visas vanligtvis om du oavsiktligt använder specialtecken, blanksteg eller landskod i företagets telefonnummer. Det värde som anges Telefon fältet Antal får bara innehålla högst 10 tecken.

### <a name="your-credit-card-purchase-is-receiving-an-error-message-stating-that-your-order-was-declined-please-verify-your-information"></a>Ditt kreditkortsköp får ett felmeddelande om att din beställning nekades. Verifiera din information"

Använd alltid den adress som motsvarar ditt kreditkort i stället för din juridiska person. Kontrollera också att postnumret är korrekt och motsvarar den adress som du använder.

## <a name="you-want-to-switch-from-offline-payment-to-online-payment-method"></a>Du vill växla från offlinebetalning till onlinebetalningsmetod

Du måste avbryta den ursprungliga beställningen och göra ett återköp med den önskade betalningsmetoden.

Så här avbryter du en beställning:

> [!NOTE]
> Mer information om gränssnittet för arbetsytor finns i [Getting around Partner Center (Ta sig runt i Partnercenter).](get-around-partner-center.md#turn-workspaces-on-and-off)

#### <a name="workspaces-view"></a>[Vy över arbetsytor](#tab/workspaces-view)

1. På [instrumentpanelen i Partnercenter](https://partner.microsoft.com/dashboard)väljer du **panelen** Medlemskap.

2. Välj **Medlemskapserbjudanden** och sedan **Avbryt beställning.**

3. Ett bekräftelsefönster visas och du måste bekräfta för att kunna avbryta den första beställningen.

#### <a name="current-view"></a>[Aktuell vy](#tab/current-view)

1. På [instrumentpanelen i Partnercenter](https://partner.microsoft.com/dashboard)väljer du **fliken Medlemskapserbjudanden.**

2. Välj **Avbryt beställning.**

3. Ett bekräftelsefönster visas och du måste bekräfta för att kunna avbryta den första beställningen.

* * *

## <a name="next-steps"></a>Nästa steg

- [Hantera ditt Partnercenter-konto](partner-center-account-setup.md)
- [Läsa fakturan och rekognoseringsfilen](read-your-bill.md)
