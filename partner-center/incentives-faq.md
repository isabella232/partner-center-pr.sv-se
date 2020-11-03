---
title: Vanliga frågor och svar
ms.topic: how-to
ms.date: 10/22/2020
description: Vanliga frågor och svar om Microsofts incitament. Den här artikeln innehåller frågor om användar roller, hur du registrerar dig eller vad du kan göra om fel meddelanden.
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
author: mseamons
ms.author: mseamons
ms.localizationpriority: medium
ms.openlocfilehash: 468ad99771aabfd42960e43e0a711e10eddc62f0
ms.sourcegitcommit: 4a88db7e9e90b4fbb2ba82af38d7f77b016977f3
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 10/24/2020
ms.locfileid: "92532236"
---
# <a name="frequently-asked-questions-on-incentives"></a>Vanliga frågor och svar om incitament

**Gäller för:**

- Partnercenter

**Lämpliga roller:**

- Incitaments administratör

- Incitaments användare

## <a name="do-i-need-to-be-the-global-admin-to-enroll-in-incentives"></a>Måste jag vara global administratör för att kunna registrera sig på incitament?

Det är inte nödvändigt att vara global administratör. MPN-administratören kan bjuda in andra användare att registrera sig om det behövs för att bli incitaments administratör, medan den globala administratören kan skapa nya användar konton. Du behöver inte vara global administratör för att kunna hantera ditt företags incitament genom verktyget. Mer information om roller och behörigheter finns i [Översikt över behörigheter](permissions-overview.md).

## <a name="what-do-i-need-to-do-if-i-find-my-company-is-already-a-member-of-the-microsoft-partner-network"></a>Vad behöver jag göra om jag har hittat mitt företag redan är medlem i Microsoft Partner Network?

Om du försöker ansluta till MPN och ditt företag redan är medlem känner den igen domänen och kopplar dig till det befintliga kontot redan. Detta kan vara samma företag eller ett relaterat företag som använder samma e-postdomän, eller samma Azure Activity Directory (Azure AD) för att hantera flera domäner.

Du kan identifiera den primära kontakten från sidan partner profil. Om din plats är MPNHQ-platsen behöver du bara konfigurera med de behörigheter som krävs för att hantera incitament. Mer information om roller och behörigheter finns i [Översikt över behörigheter](permissions-overview.md).

Om du inte befinner dig i samma land som MPNHQ-platsen läser du [instruktionerna för flera nationella konton](https://support.microsoft.com/help/4515619/special-considerations-for-multi-national-partners-joining-the-microso) för mer information om det här scenariot.

## <a name="what-user-roles-are-available"></a>Vilka användar roller är tillgängliga?

Den person som ansluter företaget till MPN blir den primära kontakt-och MPN-administratören som standard. Administratören kan bjuda in och hantera användare på portalen. Mer information om roller och behörigheter finns i [Översikt över behörigheter](permissions-overview.md).

Viktiga roller för incitament är att uppmuntra administratörer och stimulera användare. Stimulans administratören hanterar bank information för partnern. Stimulans användaren kan visa rapporter i verktyget för att se vad som har betalats och fördelningen av varje betalning, men inte Visa eller redigera bank uppgifter. Mer information om roller och behörigheter för stimulans administratören och stimulans användare finns i [Översikt över behörigheter](permissions-overview.md). Obs! de här rollerna är inte tillgängliga för val förrän partnern inbjuds att registrera sig för incitament. Båda rollerna kan tillämpas på alla platser under HQ.

## <a name="how-can-i-find-out-who-has-admin-rights-for-my-company"></a>Hur kan jag ta reda på vem som har administratörs behörighet för mitt företag?

Du kan ta reda på vem som har rollen som global administratör eller MPN konto administratör i företaget. Mer information finns i [hitta din roll](/partner-center/find-your-role.md).  

## <a name="i-cant-access-incentives-using-my-credentials"></a>Jag kan inte komma åt incitament med mina autentiseringsuppgifter.

Den mest sannolika orsaken till bristande åtkomst är att dina behörigheter inte konfigureras korrekt i Partner Center. Använd följande procedur för att se åtgärda detta.

1. Logga in på [instrument panelen för partner Center](https://partner.microsoft.com/dashboard/) med dina autentiseringsuppgifter för Azure AD-klienten (dina autentiseringsuppgifter för arbetet). Om du inte kan logga in kontaktar du företagets globala administratör.

2. Om du uppmanas att välja från ditt **arbets konto** eller **personliga konto** när du loggar in väljer du **arbets konto** .

3. På menyn Partner Center väljer du **incitament** och väljer sedan **Översikt** . Om du inte har behörighet som incitaments administratör visas kontakt information för alla globala administratörer och konto administratörer för ditt företag. Kontakta en av de här administratörerna för att få stimulans rollen för nödvändiga MPN-ID: n och incitaments program.

4. Om du redan har en roll för stimulans administration visas registreringar för ditt företag för de MPN-ID: n och de incitaments program som du har åtkomst till.
 
## <a name="some-enrollments-are-missing-from-the-incentives-overview-page"></a>Vissa registreringar saknas på sidan incitaments översikt.

Om du ser färre registreringar än vad du förväntat dig på sidan incitaments **Översikt** kan du göra följande.

1. Logga in på [instrumentpanelen i Partnercenter](https://partner.microsoft.com/dashboard/).

2. Under **Inställningar** väljer du [användar hantering](https://partner.microsoft.com/pcv/users).

3. Välj ditt namn om du vill se dina behörigheter. 

Om du behöver ändra din roll eller behörighet, se företagets globala eller konto administratör.

Observera att den här sidan endast visar registreringar som är associerade med det globala partner kontot (PGA) som är associerat med Azure AD-klienten. Om ditt företag har fler än en PGA måste du ha olika autentiseringsuppgifter för var och en.

## <a name="who-should-i-contact-if-i-get-an-error-message-or-need-help-during-the-enrollment-process"></a>Vem ska jag kontakta om jag får ett fel meddelande eller behöver hjälp under registrerings processen?

Det finns en support tjänst online om du stöter på problem i avsnittet incitament på instrument panelen – se support alternativet (? Ikonen) längst upp till höger.

## <a name="next-steps"></a>Nästa steg

- [Kom igång med incitament](incentives-get-started-intro.md)
