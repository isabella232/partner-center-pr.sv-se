---
title: Vanliga frågor och svar
ms.topic: how-to
ms.date: 02/05/2021
description: Vanliga frågor och svar om Microsofts incitament. Den här artikeln innehåller frågor om användar roller, hur du registrerar dig eller vad du kan göra om fel meddelanden.
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
author: mseamons
ms.author: mseamons
ms.localizationpriority: medium
ms.openlocfilehash: 1c3cafa6b5ea280a924a0142da78483d54a18ab9
ms.sourcegitcommit: 6498c57e75aa097861523b206dc142f789deeb36
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/02/2021
ms.locfileid: "106179504"
---
# <a name="frequently-asked-questions-on-incentives"></a>Vanliga frågor och svar om incitament

**Lämpliga roller**

- Incitaments administratör
- Incitaments användare

## <a name="do-i-need-to-be-the-global-admin-to-enroll-in-incentives"></a>Måste jag vara global administratör för att kunna registrera sig på incitament?

Nej. Både den globala administratören och konto administratören kan tilldela användare som incitaments administratörer. Incitaments Administratörer hanterar företagets incitaments program via partner Center. Mer information finns i [Översikt över behörigheter](permissions-overview.md).

## <a name="what-do-i-need-to-do-if-i-find-my-company-is-already-a-member-of-the-microsoft-partner-network-mpn"></a>Vad behöver jag göra om jag tycker att mitt företag redan är medlem i Microsoft Partner Network (MPN)?

Om du försöker ansluta till MPN och ditt företag redan är medlem kommer MPN att identifiera domänen och koppla dig till det befintliga kontot. Det befintliga kontot kan vara samma företag eller ett relaterat företag som använder samma e-postdomän, eller samma Azure Activity Directory (Azure AD) för att hantera flera domäner.

Du kan identifiera den primära kontakten från sidan juridisk profil. Om din plats är MPNHQ-platsen behöver du bara konfigurera med de behörigheter som krävs för att hantera incitament. Mer information om roller och behörigheter finns i [Översikt över behörigheter](permissions-overview.md).

Om du inte befinner dig i samma land som MPNHQ-platsen läser du [instruktionerna för flera nationella konton](https://support.microsoft.com/help/4515619/special-considerations-for-multi-national-partners-joining-the-microso) för mer information om det här scenariot.

## <a name="what-user-roles-are-available"></a>Vilka användar roller är tillgängliga?

Den person som registrerar företaget i Partner Center blir den primära kontakten och den globala administratören som standard. Administratören kan bjuda in och hantera användare på portalen.

Viktiga roller för incitament är att uppmuntra administratörer och stimulera användare. Incitaments administratören kan registrera sig för stimulans program och hantera bank-och skatte information för partnern. Stimulans användaren kan visa rapporter i verktyget för att se vad som har betalats och fördelningen av varje betalning, men inte Visa eller redigera bank uppgifter. Båda rollerna kan tillämpas på alla platser under partnerns globala konto.

Mer information finns i [Översikt över behörigheter](permissions-overview.md).

## <a name="how-can-i-find-out-who-has-global-or-account-admin-rights-for-my-company"></a>Hur kan jag ta reda på vem som har globala eller konto administratörs rättigheter för mitt företag?

Hitta en global administratör eller konto administratör som kan göra roll ändringar eller tilldela roller till en ny användare:

1. Välj **användar hantering** på ikonen konto inställningar längst upp till höger i Partner Center.
2. Filtrera på antingen **Global administratör** eller **konto administratör**.
3. Du kan också gå till **min profil**, välja **roller och behörigheter** och se en lista över de olika administratörer som kan hjälpa dig att öka dina behörigheter.
 
Mer information finns i [hitta din roll](find-your-role.md).  

## <a name="i-cant-access-incentives-using-my-credentials"></a>Jag kan inte komma åt incitament med mina autentiseringsuppgifter.

Den troliga orsaken till att du inte kan se incitament är att du inte har rätt behörighet. Använd följande procedur för att åtgärda detta.

1. Logga in på [instrument panelen för partner Center](https://partner.microsoft.com/dashboard/) med dina autentiseringsuppgifter för Azure AD-klienten (dina autentiseringsuppgifter för arbetet). Om du inte kan logga in kontaktar du företagets globala administratör.

2. Om du uppmanas att välja från ditt **arbets konto** eller **personliga konto** när du loggar in väljer du **arbets konto**.

3. På menyn Partner Center väljer du **incitament** och väljer sedan **Översikt**. Om du inte har någon incitaments administratör eller incitament över användar behörigheter visas kontakt information för alla globala administratörer och konto administratörer för ditt företag. Kontakta en av de här administratörerna för att få stimulans rollen för nödvändiga MPN-ID: n och incitaments program.

4. Om du redan har en roll för stimulans administration visas registreringar för ditt företag för de MPN-ID: n och de incitaments program som du har åtkomst till.

## <a name="some-enrollments-are-missing-from-the-incentives-overview-page"></a>Vissa registreringar saknas på sidan incitaments översikt.

Om du antingen har fått en inbjudan från, eller om du har registrerat dig i, ett incitaments program som inte längre visas i instrument panelen, bör du kontrol lera att du har rätt åtkomst. Endast användare med rollen stimulans användare eller incitaments administratör kan se programmet. Se [hitta din roll](./find-your-role.md).

Kontakta företagets globala eller konto administratör om du behöver ändra din roll eller behörighet. Läs [hitta din globala administratör](./find-your-role.md#find-your-global-admin)för att lära dig mer om vem dessa personer är.

Översikts sidan visar bara registreringar som är associerade med det globala partner kontot (PGA) som är associerat med Azure AD-klienten. Om ditt företag har fler än en PGA måste du ha olika autentiseringsuppgifter för var och en.

## <a name="who-should-i-contact-if-i-get-an-error-message-or-need-help-during-the-enrollment-process"></a>Vem ska jag kontakta om jag får ett fel meddelande eller behöver hjälp under registrerings processen?

Det finns en support tjänst online om du stöter på problem i avsnittet incitament på instrument panelen – se support alternativet (? Ikonen) längst upp till höger.

## <a name="next-steps"></a>Nästa steg

- [Komma igång med incitament](incentives-get-started-intro.md)