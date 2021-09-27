---
title: Incitamentsregistrering
ms.topic: how-to
ms.date: 09/27/2021
description: Registrera dig i incitamentsprogrammet och tilldela de roller som krävs för användarhantering. I den här artikeln beskrivs registreringsprocessen.
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
author: mseamons
ms.author: mseamons
ms.localizationpriority: medium
ms.openlocfilehash: c9a7dbae07ece38668a0b59b31c6e3e70e2280df
ms.sourcegitcommit: d731813da1d31519dc2dc583d17899e5cf4ec1b2
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/27/2021
ms.locfileid: "129074908"
---
# <a name="enrollment-and-user-management-in-the-incentives-program"></a>Registrering och användarhantering i incitamentsprogrammet

**Lämpliga roller:** Incitamentsadministratör

>[!NOTE]
>Innan du kan registrera dig i incitamentsprogrammet måste du ha slutfört migreringen Partner Membership Center [partnercenter.](./partner-membership-center-retirement-faq.md)

Registreringsprocessen består av två steg.

**Steg 1. Användarhantering: Det** här steget handlar om att upprätta incitamentsadministratören i Partnercenter.

**Steg 2. Registrering:** Microsoft skickar dig en inbjudan att registrera dig i ditt incitamentprogram.

## <a name="user-management"></a>Användarhantering

För att kunna registrera sig i ett Incitamentprogram i Partnercenter måste Global administratör eller kontoadministratören konfigurera företagets användare som incitamentadministratörer. Information om partnerkonton, roller och behörigheter finns i [Hantera ditt Partnercenter-konto.](partner-center-account-setup.md) Den Global administratör kan också konfigurera företagets användare via Azure Active Directory (Azure AD).

>[!NOTE]
>Endast incitamentadministratören kan registrera sig i incitamentprogram. Om det inte finns någon incitamentadministratör för din plats Global administratör kontoadministratören tilldela en. Incitamentadministratören måste tilldelas för platsens MPN-IP-nummer. Administratören Global administratör eller kontoadministratören kan också tilldelas som incitamentadministratör. Mer information om olika roller finns i [Hantera incitament.](permissions-overview.md#manage-incentives)

## <a name="enrollment-process"></a>Registreringsprocess

När din organisation är berättigad till incitament skickar Microsoft en inbjudan till incitamentadministratören för det berättigade MPNLocationID för att påbörja registreringsprocessen. Det här e-postmeddelandet skickas **från Microsoft Partner Center** och har ämnesinbjudan för **partnerinbjudan för incitamentregistrering.** Öppna inbjudan och välj **Kom igång**.

Du ser också en inbjudan på startsidan för Partnercenter. När du har valt meddelandet kan du inte se det igen. Incitamentadministratören kan dock fortfarande slutföra processen genom att logga in på [instrumentpanelen i Partnercenter](https://partner.microsoft.com/dashboard/) och välja **panelen Incitament.** Välj **Registrera** och slutför sedan utbetalnings- och skatteprofilen för programmet.

**Om** du redan har en standardinställning för bankprofilen för en MPN-plats och du försöker registrera dig för samma MPN-plats i ett incitamentprogram visas standardbankprofilen när du väljer Registrera och godkänner inbjudan. Du kommer också att se alla tillgängliga skatteprofiler om du har skapat den för den MPN-platsen. Om Microsoft har alla bank- och skatteprofilinformation som krävs uppmanas du att välja **Skicka för** att slutföra registreringen. Se [Konfigurera en standardbankprofil.](incentives-create-and-manage-your-payout-and-tax-profiles.md#set-up-a-default-bank-profile)

Du kan också välja en annan bankprofil än standardbankprofilen. Om Microsoft kräver ytterligare information för betalnings- eller skatteprofilerna  eller valutan uppmanas  du att fortsätta och omdirigeras till sidan betalnings- och skatteprofil för att ange den information som saknas. 

En registrering anses vara fullständig endast när utbetalnings- och skatteprofilen som du anger för registreringen verifieras av Microsoft.

Vissa incitamentprogram har inga behörighetskriterier och är öppna för alla partner. Incitamentadministratören ser inbjudningar för dessa program på översiktssidan för incitament, förutsatt att de har behörighet för relevant incitamentprogram och MPN. Microsoft skickar inte e-postinbjudningar för dessa program.

Om du vill ha mer information om registreringsprocessen laddar du [ned registreringsguiden för incitament](https://partner.microsoft.com/resources/detail/partner-center-incentives-enrollment-pdf) (inloggning krävs).

## <a name="expiration-and-renewal"></a>Förfallotid och förnyelse

Incitamentsregistreringen upphör att gälla i slutet av räkenskapsåret. Så länge du är en berättigad partner med ett aktivt avtal kommer Microsoft dock att vidarebefordra din incitamentsregistrering till nästa räkenskapsår. Du behöver inte vidta några åtgärder, så länge utbetalnings- och skatteinformationen som krävs för incitamentprogrammet är slutförd enligt reglerna för incitamentprogrammet.

## <a name="next-steps"></a>Nästa steg

- [Fastställa behörighet för program](incentives-determined-your-program-eligibility.md)
- [Skapa och hantera dina utbetalnings- och skatteprofiler](incentives-create-and-manage-your-payout-and-tax-profiles.md)