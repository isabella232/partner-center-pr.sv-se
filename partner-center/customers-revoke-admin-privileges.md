---
title: Skaffa en kunds administratörsbehörighet
ms.topic: how-to
ms.date: 12/02/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-customers
description: Skaffa de behörigheter som du behöver för att hantera en kunds tjänst eller prenumeration för kundens räkning. Lär dig hur behörigheter beviljas, återkallas och hanteras.
author: BillLinzbach
ms.author: BillLi
ms.custom: SEOAPR.20
ms.localizationpriority: high
ms.openlocfilehash: fafd9e2c13abb1f4b9b12e5839662b27c4852452
ms.sourcegitcommit: 1161d5bcb345e368348c535a7211f0d353c5a471
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/09/2021
ms.locfileid: "123960713"
---
# <a name="obtain-permissions-to-manage-a-customers-service-or-subscription"></a>Få behörighet att hantera en kunds tjänst eller prenumeration

**Lämpliga roller:** Administratörsagent | Försäljningsagent

För att kunna hantera en kunds tjänst eller prenumeration för kundens räkning måste kunden ge dig administratörsbehörighet för den tjänsten. Om du vill få administratörsbehörighet från en kund skickar du en begäran om återförsäljarrelation via e-post. När kunden har godkänt din begäran kan du logga in på tjänstens administratörsportal och hantera tjänsten för kundens räkning. 

## <a name="invite-a-customer-to-establish-a-reseller-relationship-with-you"></a>Bjud in en kund att upprätta en återförsäljarrelation med dig

1.  Välj **Kunder** och välj sedan **Begär en återförsäljarrelation.**

2.  På nästa sida granskar du utkastet till e-postmeddelandet. Du kan öppna utkastet i ditt vanliga e-postprogram, eller så kan du kopiera meddelandet till Urklipp och klistra in det i ett e-postmeddelande. 

    >[!IMPORTANT]
    >Du kan redigera texten i e-postmeddelandet, men se till att ta med länken eftersom den är anpassad för att länka kunden direkt till ditt konto. 
    
3.  Välj **Klar** när du har slutfört det här steget.

4.  Skicka e-postmeddelandet till kunden.

5.  När kunden har accepterat din inbjudan visas  de på sidan Kunder och du kommer att kunna etablera och hantera tjänsten för kunden därifrån.

6.  Om du vill hantera kundens konto, tjänster, användare och licenser expanderar du kundens post genom att välja nedåtpilen nära kundens namn och sedan välja administratörsportalen för den tjänst som du vill hantera.

>[!IMPORTANT]  
>Kunder kan tilldela om eller ta bort administratörsbehörigheter i en tjänsts administratörsportal. Du måste dock informera kunden om att borttagningen av dina administratörsbehörigheter innebär att du inte längre kan öppna en tjänstbegäran till Microsoft för deras räkning. Du kommer inte att kunna öppna dessa typer av tjänstbegäranden för kundens räkning förrän du omförhandling av ditt avtal med kunden.

Dina kunder kan ta reda på vilka av deras partner som har administratörsbehörighet för sin klientorganisation från Office 365 administrationsportalen. Gör så här:

1. Kunden måste logga in på Office 365-administratörsportalen som global administratör.

2. Välj **Inställningar**  >  **Partnerrelationer**.

3. På sidan **Partnerrelationer** ser kunden en lista över de partner som de arbetar med och de som har beviljats delegerade administratörsbehörigheter till sin klientorganisation.

## <a name="customers-can-manage-a-partners-delegated-admin-privileges"></a>Kunder kan hantera en partners delegerade administratörsbehörighet 

Kunden kan välja att ta bort dina delegerade administratörsbehörigheter från sin klientorganisation men behålla relationen med dig i prenumerations- och licensförnyelsesyften. Kunder hanterar rättigheter och behörigheter till sina Office 365-konton på **sidan Partnerrelationer** i Office 365 administrationscenter. På den här sidan kan kunder:

- Se vilka partner de har en relation med och vilka partner som har delegerad administratörsbehörighet

- Ta bort en partners delegerade administrationsbehörigheter från klientorganisationen

Så här tar du bort delegerade administrationsbehörigheter från en partner:

1. Under sidan **Partnerrelationer** väljer du den partner du är intresserad av.
2. I informationsfönstret väljer du Ta **bort delegerad administratör.**
3. I bekräftelsefönstret väljer du Ta **bort**.

>[!IMPORTANT]  
>Azure AD-rolltilldelningar till partnern är implicita. Om du försöker lista medlemmarna i Azure AD-rollerna med hjälp av Azure AD-portalen/PowerShell/Graph, returneras inte partnern. Om du vill ta reda på om partner har tilldelats Till Azure AD-roller måste du gå till sidan Partnerrelationer i Office 365 Admin-portalen för att ta reda på om delegerad administratörsbehörighet har beviljats till partnern eller inte.

## <a name="delegated-admin-privileges-in-azure-ad"></a>Delegerade administratörsbehörigheter i Azure AD 

Det finns två säkerhetsgrupper, Administratörsagenter och Supportagenter, i partnerns Azure AD-klientorganisation som används för delegerad administration. När en kund ger delegerad administratörsbehörighet till en partner:

- Gruppen Administratörsagent tilldelas rollen Global administratör i kundens Azure AD-klientorganisation.

- Supportagentgruppen tilldelas rollen Supportadministratör i kundens Azure AD-klientorganisation.

Baserat på de katalogroller som tilldelats kan medlemmar i båda grupperna logga in på kundens Azure AD-klientorganisation och O365-tjänster med sina partnerautentiseringsuppgifter och administratör för kundens räkning.

Om kunden tar bort delegerade administratörsbehörigheter tas Azure AD-rolltilldelningarna bort och du kommer inte längre att kunna hantera kundens Azure AD-klientorganisation.

### <a name="azure-subscriptions-and-resource-management"></a>Azure-prenumerationer och resurshantering

Varje Azure-prenumeration har en egen uppsättning resurshanteringsroller. Innan en CSP-partner kan hantera en kunds Azure-prenumeration måste partnern tilldelas en eller flera roller under Azure-prenumerationen. Specifikt:

- När en kund accepterar en återförsäljarinbjudan och ger delegerad administratörsbehörighet till en partner får partnern inte automatiskt åtkomst till befintliga Azure-prenumerationer under kundens klientorganisation.

- När CSP-partnern tillhandahåller en ny Azure-prenumeration för kunden tilldelas gruppen Administratörsagenter under CSP-partnerns klientorganisation automatiskt rollen Ägare under prenumerationen. Baserat på den här rolltilldelningen kan medlemmar i gruppen komma åt och hantera resurser under prenumerationen.

- När en kund tar bort delegerade administrationsbehörigheter från en partner med hjälp av Office 365 Portal kan partnern fortfarande hantera kundens Azure-prenumeration så länge partnern fortfarande är tilldelad till en eller flera roller under prenumerationen. Om du vill hindra partnern från att hantera Azure-prenumerationen måste kunden ta bort rolltilldelningen.

## <a name="windows-autopilot"></a>Windows Autopilot

Från Partnercenter kan CSP-partner hantera Autopilot-profiler för sina kunder utan delegerad administratörsbehörighet under dessa omständigheter: 

- Om en kund tar bort delegerade administrationsbehörigheter men behåller en återförsäljarrelation med dig kan du fortsätta att hantera Autopilot-profiler för dem.

- Du kan hantera kundenheter som du eller en annan partner har lagt till. 

- Du kan inte hantera enheter som kunden har lagt till via Microsoft Store för företag, Microsoft Store för utbildning eller Microsoft Intune portalen.

Mer information om Autopilot finns i [Förenkla enhetskonfiguration med Windows Autopilot.](autopilot.md)

>[!IMPORTANT]  
>Den aktuella Autopilot-hanteringsupplevelsen i Partnercenter kan fortsätta att ändras. När den här artikeln publicerades övervägs följande ändringar:

- Partnern måste beviljas delegerad administratörsbehörighet av kunden innan partnern kan lägga till/uppdatera/ta bort profiler och tillämpa/ta bort profil från enheter i kundens klientorganisation.

- Partnern måste beviljas delegerad administratörsbehörighet av kunden innan partnern kan ta bort enheter som lagts till av andra partner eller av kunden i kundens klientorganisation. Annars kan partnern endast ta bort enheter som lagts till tidigare av samma partner.
