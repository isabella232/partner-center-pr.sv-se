---
title: Begära en relation med en kund
ms.topic: how-to
ms.date: 06/17/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Begär en relation med en kund för scenarier med flera partner, flera kanaler eller om dina delegerade administratörsbehörigheter för en kund måste återställas.
author: dineshvu
ms.author: dineshvu
ms.localizationpriority: medium
ms.openlocfilehash: 55f86e6e48b0b897410826e22564e2d27e25258b
ms.sourcegitcommit: efd711b0e65c55f24ce5b9636abd7b5a8cc719fe
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/27/2021
ms.locfileid: "108018143"
---
# <a name="how-to-request-a-reseller-relationship-from-a-customer-in-partner-center"></a>Så här begär du en återförsäljarrelation från en kund i Partnercenter

**Lämpliga roller**

- Administratörsagent
- Global administratör

Om du vill hantera en kunds tjänst eller prenumeration för kundens räkning måste kunden ge dig administratörsbehörighet för den tjänsten eller prenumerationen och signera Microsoft-kundavtal.

Om du vill upprätta en återförsäljarrelation med en kund och endast hantera de Azure-prenumerationer som du etablerar behöver du inte skaffa administratörsbehörigheter.

>[!NOTE] 
>Alternativet att inte begära behörigheter är inte tillgängligt för partner som arbetar i Microsoft Cloud for US Government eller Microsoft Cloud Tyskland. Mer information finns i [Kunder delegerar administratörsbehörigheter till partner.](customers-revoke-admin-privileges.md)

## <a name="invite-a-customer-to-establish-a-reseller-relationship-with-you"></a>Bjud in en kund att upprätta en återförsäljarrelation med dig

Du kan begära en återförsäljarrelation med en kund från ditt land eller i samma region.

1. Välj **Kunder** på menyn **i Partnercenter** och välj sedan **Begär en återförsäljarrelation.**

2. Om du vill begära administratörsbehörighet från den här kunden väljer du **Inkludera delegerade administrationsbehörigheter för Azure Active Directory och Office 365.** Avmarkera det här alternativet om du vill upprätta relationen utan att begära administratörsbehörighet.

3. På nästa sida granskar du utkastet till e-postmeddelandet. Du kan öppna utkastet i ditt vanliga e-postprogram, eller så kan du kopiera meddelandet till Urklipp och klistra in det i ett e-postmeddelande.

   Du kan redigera texten i e-postmeddelandet, men se till att ta med länken eftersom den är anpassad för att länka kunden direkt till ditt konto. Välj **Klar** när du har slutfört det här steget.

4. Skicka e-postmeddelandet till kunden.

5. När kunden har accepterat din inbjudan visas den på sidan **Kunder** och kan etablera och hantera tjänsten för kunden därifrån.

   > [!NOTE]
   > Om kunden inte redan har accepterat Microsoft-kundavtal uppmanas de att göra det när de godkänner din inbjudan. Kunden måste vara global administratör för att acceptera inbjudan.

6. Om du vill hantera kundens konto, tjänster, användare och licenser expanderar du kundens post genom att välja nedåtpilen nära namnet.

> [!IMPORTANT]  
> Kunder kan tilldela om eller ta bort administratörsbehörigheter i en tjänsts administratörsportal. Men såvida inte och tills du omförhandling av ditt avtal med kunden fortsätter du att vara ansvarig för att tillhandahålla kundsupport och följa villkoren i Microsoft-partneravtal, även efter att en kund omtilldelar eller tar bort administratörsbehörigheter. I så fall kan du, om kunden behöver hjälp, ringa Microsoft-supporten för att öppna en tjänstbegäran för kundens räkning.

## <a name="changes-to-the-customer-invitation-experience"></a>Ändringar i kundinbjudan

Kundupplevelsen för att acceptera en återförsäljarrelationsinbjudan från en Molnlösningsleverantör partner finns i olika kundriktade portaler. Portalplatsen beror på om en kund finns i ett offentligt Microsoft-moln eller ett nationellt moln:

|Typer av molnkunder  | Var accepterar en kund en återförsäljarrelationsinbjudan? |
|---------|---------
| Kunder i offentligt moln | Microsoft 365 Administrationscenter |
| Kunder i Partnercenter för Microsoft Cloud Tyskland | Microsoft Office administratörsportalen |
| Kunder i Partnercenter för Microsoft Cloud for US Government | Microsoft Office administratörsportalen |
|

## <a name="next-steps"></a>Nästa steg

- [Tilldela supportkontakter](assign-support-contacts.md)

- [Ta bort en relation med en kund](remove-a-relationship.md)
