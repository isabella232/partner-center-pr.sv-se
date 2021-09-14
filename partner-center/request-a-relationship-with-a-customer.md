---
title: Göra en förfrågan om återförsäljarrelation med en kund
ms.topic: how-to
ms.date: 06/17/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-customers
description: Begär en relation med en kund för scenarier med flera partner, flera kanaler eller om dina delegerade administratörsbehörigheter för en kund måste återställas.
author: dineshvu
ms.author: dineshvu
ms.localizationpriority: medium
ms.openlocfilehash: 5b80cc15ade94a9003ec1b21293d86c3b5ac8ace
ms.sourcegitcommit: 37eac16c4339cb97831eb2a86d156c45bdf6a531
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/13/2021
ms.locfileid: "126249075"
---
# <a name="how-to-request-a-reseller-relationship-from-a-customer-in-partner-center"></a>Så här begär du en återförsäljarrelation från en kund i Partnercenter

**Lämpliga roller:** Administratörsagent | Global administratör

Om du vill hantera en kunds tjänst eller prenumeration för kundens räkning måste kunden ge dig administratörsbehörighet för den tjänsten eller prenumerationen och signera Microsoft-kundavtal.

Om du vill upprätta en återförsäljarrelation med en kund och endast hantera de Azure-prenumerationer som du etablerar behöver du inte skaffa administratörsbehörigheter.

>[!NOTE] 
>Alternativet att inte begära behörigheter är inte tillgängligt för partner som arbetar i Microsoft Cloud for US Government eller Microsoft Cloud Tyskland. Mer information finns i Kunder [delegerar administratörsbehörigheter till partner.](customers-revoke-admin-privileges.md)

## <a name="invite-a-customer-to-establish-a-reseller-relationship-with-you"></a>Bjud in en kund att upprätta en återförsäljarrelation med dig

Du kan begära en återförsäljarrelation med en kund från ditt land eller i samma region.

1. Välj **Kunder** på menyn **i Partnercenter** och välj sedan **Begär en återförsäljarrelation.**

2. Om du vill begära administratörsbehörighet från den här kunden **väljer du Inkludera delegerade administrationsbehörigheter för Azure Active Directory och Office 365**. Avmarkera det här alternativet om du vill upprätta relationen utan att begära administratörsbehörighet.

3. På nästa sida granskar du utkastet till e-postmeddelandet. Du kan öppna utkastet i ditt vanliga e-postprogram, eller så kan du kopiera meddelandet till Urklipp och klistra in det i ett e-postmeddelande.

   Du kan redigera texten i e-postmeddelandet, men se till att ta med länken eftersom den är anpassad för att länka kunden direkt till ditt konto. Välj **Klar** när du har slutfört det här steget.

4. Skicka e-postmeddelandet till kunden.

5. När kunden har accepterat din inbjudan visas den på sidan **Kunder** och kan etablera och hantera tjänsten för kunden därifrån.

   > [!NOTE]
   > Om kunden inte redan har accepterat Microsoft-kundavtal uppmanas de att göra det när de accepterar din inbjudan. Kunden måste vara global administratör för att acceptera inbjudan.

6. Om du vill hantera kundens konto, tjänster, användare och licenser expanderar du kundens post genom att välja nedåtpilen nära kundens namn.

> [!IMPORTANT]  
> Kunder kan tilldela om eller ta bort administratörsbehörigheter i en tjänsts administratörsportal. Men såvida inte och tills du omförhandling av ditt avtal med kunden fortsätter du att vara ansvarig för att tillhandahålla kundsupport och följa villkoren i Microsoft-partneravtal, även efter att en kund har tilldelat om eller tagit bort administratörsbehörigheter. I så fall kan du, om kunden behöver hjälp, ringa Microsoft-supporten för att öppna en tjänstbegäran för kundens räkning.

## <a name="changes-to-the-customer-invitation-experience"></a>Ändringar i kundinbjudan

Kundupplevelsen för att acceptera en återförsäljarrelationsinbjudan från en Molnlösningsleverantör-partner (CSP) finns i olika kundriktade portaler. Portalplatsen beror på om en kund finns i ett offentligt Microsoft-moln eller ett nationellt moln:

|Typer av molnkunder  | Var accepterar en kund en återförsäljarrelationsinbjudan? |
|---------|---------
| Kunder i offentligt moln | Microsoft 365 Admin Centrum |
| Kunder i Partnercenter för Microsoft Cloud Tyskland | Microsoft Office Administratörsportalen |
| Kunder i Partnercenter för Microsoft Cloud for US Government | Microsoft Office Administratörsportalen |
|

## <a name="next-steps"></a>Nästa steg

- [Tilldela supportkontakter](assign-support-contacts.md)

- [Ta bort en relation med en kund](remove-a-relationship.md)
