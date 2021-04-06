---
title: Skaffa en kunds administratörs behörighet
ms.topic: how-to
ms.date: 12/02/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Få de behörigheter du behöver för att hantera en kunds tjänst eller prenumeration åt dig. Lär dig hur behörigheter beviljas, återkallas och hanteras.
author: BillLinzbach
ms.author: BillLi
ms.custom: SEOAPR.20
ms.localizationpriority: high
ms.openlocfilehash: 624b66c7912af1f0109b6aadeffb67c5d4e9ea4b
ms.sourcegitcommit: 3d7d5064c5e021079ed7e6f93f03869cbf425a32
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/06/2021
ms.locfileid: "106502505"
---
# <a name="obtain-permissions-to-manage-a-customers-service-or-subscription"></a>Få behörighet att hantera en kunds tjänst eller prenumeration

**Lämpliga roller**

- Administratörs agent
- Försäljnings agent

Kunden måste bevilja administratörs behörighet för tjänsten för att kunna hantera en kunds tjänst eller prenumeration. Om du vill få administratörs behörighet från en kund skickar du ett e-postmeddelande till en åter försäljare Relations förfrågan. När Kunden godkänner din begäran kan du logga in på tjänstens administrations Portal och hantera tjänsten för kundens räkning. 

## <a name="invite-a-customer-to-establish-a-reseller-relationship-with-you"></a>Bjud in en kund för att upprätta en åter försäljares relation med dig

1.  Välj **kunder** och välj sedan **begär en åter försäljares relation**.

2.  På nästa sida granskar du utkastet till e-postmeddelandet. Du kan öppna utkastet i ditt vanliga e-postprogram, eller så kan du kopiera meddelandet till Urklipp och klistra in det i ett e-postmeddelande. 

    >[!IMPORTANT]
    >Du kan redigera texten i e-postmeddelandet, men se till att ta med länken eftersom den är anpassad för att länka kunden direkt till ditt konto. 
    
3.  Välj **klar** när du har slutfört det här steget.

4.  Skicka e-postmeddelandet till din kund.

5.  När kunden har accepterat din inbjudan visas den på sidan **kunder** och du kan etablera och hantera tjänsten för kunden därifrån.

6.  Om du vill hantera kundens konto, tjänster, användare och licenser expanderar du kundens post genom att välja nedåtpilen nära deras namn och välj sedan administrations portalen för den tjänst som du vill hantera.

>[!IMPORTANT]  
>Kunder kan omtilldela eller ta bort administratörs behörighet på en tjänsts administrations Portal. Men du måste meddela kunden att borttagning av administratörs behörighet innebär att du inte längre kan öppna en tjänstbegäran till Microsoft för deras räkning. Du kommer inte att kunna öppna de här typerna av tjänst begär Anden på kundens ställe förrän du omförhandlar ditt avtal med kunden.

Dina kunder kan ta reda på vilken av sina partners som har administratörs behörighet för deras klient organisation i administrations portalen för Office 365. Gör så här:

1. Kunden måste logga in på administrations portalen för Office 365 som global administratör.

2. Välj **Inställningar**  >  **partner relationer**.

3. På sidan **partner relationer** kommer kunden att se en lista över de partner som de arbetar med och de som har beviljats delegerade administrations behörigheter till klienten.

## <a name="customers-can-manage-a-partners-delegated-admin-privileges"></a>Kunder kan hantera en partners delegerade administratörs behörighet 

Kunden kan välja att ta bort dina delegerade administratörs behörigheter från sin klient, men samtidigt behålla relationen med dig för prenumerations-och licens förnyelse. Kunderna hanterar rättigheter och behörigheter till sina Office 365-konton på sidan **partner relationer** i administrations centret för Office 365. På den här sidan kan kunder:

- Se vilka partner som de har en relation till och vilka partner har delegerad administratörs behörighet

- Ta bort en partners delegerade administrations behörigheter från klienten

Så här tar du bort delegerade administrations behörigheter från en partner:

1. På sidan **partner relationer** väljer du intresse partner.
2. I informations fönstret väljer du **ta bort delegerad administratör**.
3. I bekräftelse fönstret väljer du **ta bort**.

>[!IMPORTANT]  
>Azure AD-roll tilldelningar till partnern är implicita. Om du försöker visa medlemmar i Azure AD-rollerna med Azure AD Portal/PowerShell/Graph returneras inte partnern. Om du vill ta reda på om partner tilldelas till Azure AD-roller måste du referera till sidan partner relationer i administrations portalen för Office 365 för att ta reda på om delegerad administrations behörighet har beviljats till partnern eller inte.

## <a name="delegated-admin-privileges-in-azure-ad"></a>Delegerade administratörs privilegier i Azure AD 

Det finns två säkerhets grupper, administratörs agenter och supportavdelningen i partnerns Azure AD-klient som används för delegerad administration. När en kund ger delegerad administrations behörighet till en partner:

- Administratörs Agent gruppen tilldelas rollen som global administratör i kundens Azure AD-klient.

- Agent gruppen för supportavdelningen tilldelas rollen support administratör i kundens Azure AD-klient.

Utifrån de katalog roller som tilldelats kan medlemmar i båda grupperna logga in på kundens Azure AD-klient och O365-tjänster med sina partner uppgifter och administratörer för kundens räkning.

Om din kund tar bort delegerade administratörs privilegier tas roll tilldelningarna för Azure AD bort och du kommer inte längre att kunna hantera kundens Azure AD-klient.

### <a name="azure-subscriptions-and-resource-management"></a>Azure-prenumerationer och resurs hantering

Varje Azure-prenumeration har en egen uppsättning resurs hanterings roller. Innan en CSP-partner kan hantera en kunds Azure-prenumeration måste partnern tilldelas en eller flera roller under Azure-prenumerationen. Specifikt:

- När en kund accepterar en inbjudan till åter försäljaren och beviljar behörighet för delegerad administration till en partner får partnern inte automatiskt åtkomst till befintliga Azure-prenumerationer under kund innehavaren.

- När CSP-partner etablerar en ny Azure-prenumeration för kunden, tilldelas gruppen admin agenter under CSP-partnerns klient organisation automatiskt ägar rollen under prenumerationen. Utifrån den här roll tilldelningen kan medlemmar i gruppen komma åt och hantera resurser under prenumerationen.

- När en kund tar bort delegerade administrations behörigheter från en partner med hjälp av Office 365-portalen kan partnern fortfarande hantera kundens Azure-prenumeration så länge partnern fortfarande är tilldelad till en eller flera roller under prenumerationen. Kunden måste ta bort roll tilldelningen för att stoppa partnern från att hantera Azure-prenumerationen.

## <a name="windows-autopilot"></a>Windows Autopilot

Från Partner Center kan CSP-partner hantera autopilot-profiler för sina kunder utan delegerad administratörs behörighet under följande omständigheter: 

- Om en kund tar bort delegerade administrations behörigheter men behåller en åter försäljares relation med dig, kan du fortsätta att hantera autopilot-profiler för dem.

- Du kan hantera kund enheter som du eller en annan partner har lagt till. 

- Du kan inte hantera enheter som kunden har lagt till via Microsoft Store för företag, Microsoft Store för utbildning eller Microsoft Intune Portal.

Mer information om autopilot finns i [förenkla enhets installationen med Windows autopilot](autopilot.md).

>[!IMPORTANT]  
>Den aktuella funktionen för autopilot-hantering i Partner Center kan fortsätta att ändra. När den här artikeln publicerades beaktas följande ändringar:

- Partner måste beviljas delegerad administrations behörighet av kunden innan partnern kan lägga till/uppdatera/ta bort profiler och tillämpa/ta bort profil från alla enheter i kund klienten.

- Partner måste beviljas delegerad administrations behörighet av kunden innan partnern kan ta bort enheter som lagts till av andra partner eller av kunden i kund klienten. Annars kan partnern bara ta bort enheter som lagts till tidigare av samma partner.
