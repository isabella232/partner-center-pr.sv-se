---
title: Vanliga frågor och svar om incitament
ms.topic: how-to
ms.date: 02/05/2021
description: Vanliga frågor och svar om Microsoft-incitament. Den här artikeln innehåller frågor om användarroller, hur du registrerar eller vad du kan göra med felmeddelanden.
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
author: mseamons
ms.author: mseamons
ms.localizationpriority: medium
ms.openlocfilehash: a917f3648447ac273fae839d32a4b4d3ce80ae35
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 05/19/2021
ms.locfileid: "110152026"
---
# <a name="frequently-asked-questions-on-incentives"></a>Vanliga frågor och svar om incitament

**Lämpliga roller:** Incitamentsadministratörsroller | Incitamentsanvändare

## <a name="do-i-need-to-be-the-global-admin-to-enroll-in-incentives"></a>Måste jag vara global administratör för att registrera mig för incitament?

Nej. Både den globala administratören och kontoadministratören kan tilldela användare som incitamentsadministratörer. Incitamentsadministratörer hanterar företagets incitamentsprogram via Partnercenter. Mer information finns i Översikt [över behörigheter.](permissions-overview.md)

## <a name="what-do-i-need-to-do-if-i-find-my-company-is-already-a-member-of-the-microsoft-partner-network-mpn"></a>Vad behöver jag göra om jag upptäcker att mitt företag redan är medlem i Microsoft Partner Network (MPN)?

Om du försöker ansluta till MPN och ditt företag redan är medlem känner MPN igen domänen och kopplar dig till det befintliga kontot. Det befintliga kontot kan vara samma företag eller ett relaterat företag som använder samma e-postdomän, eller samma Azure Activity Directory (Azure AD) för att hantera flera domäner.

Du kan identifiera den primära kontakten på sidan Juridisk profil. Om din plats är MPNHQ-platsen behöver du bara konfigureras med de behörigheter som krävs för att hantera incitament. Mer information om roller och behörigheter finns i Översikt [över behörigheter.](permissions-overview.md)

Om du inte befinner dig i samma land som [MPNHQ-platsen](https://support.microsoft.com/help/4515619/special-considerations-for-multi-national-partners-joining-the-microso) kan du läsa mer om det här scenariot i Instruktioner för konton med flera nationella konton.

## <a name="what-user-roles-are-available"></a>Vilka användarroller är tillgängliga?

Den person som registrerar företaget i Partnercenter blir som standard primär kontakt och global administratör. Administratören kan bjuda in och hantera användare på portalen.

De viktigaste rollerna för incitament är Incitamentsadministratör och Incitamentsanvändare. Incitamentsadministratören kan registrera sig i incitamentprogram och hantera bank- och skatteinformation för partnern. Incitamentsanvändaren kan visa rapporter i verktyget för att se vad som betalats och uppdelningen av varje betalning, men kan inte visa eller redigera bankinformation. Båda rollerna kan tillämpas på alla platser under det globala partnerkontot.

Mer information finns i Översikt [över behörigheter.](permissions-overview.md)

## <a name="how-can-i-find-out-who-has-global-or-account-admin-rights-for-my-company"></a>Hur tar jag reda på vem som har behörighet som global administratör eller kontoadministratör för mitt företag?

Så här hittar du en global administratör eller kontoadministratör som kan göra rolländringar eller tilldela roller till en ny användare:

1. Från ikonen Kontoinställningar längst upp till höger i Partnercenter väljer du **Användarhantering.**
2. Filtrera på **antingen Global administratör** eller **Kontoadministratör.**
3. Du kan också gå **till Min profil,** välja **Roller** och behörigheter och se en lista över de olika administratörer som kan hjälpa dig att höja dina behörigheter.
 
Mer information finns i [Hitta din roll.](find-your-role.md)  

## <a name="i-cant-access-incentives-using-my-credentials"></a>Jag kan inte komma åt incitament med mina autentiseringsuppgifter.

Den troliga anledningen till att du inte kan se incitament är att du inte har rätt behörigheter. Använd följande procedur för att åtgärda detta.

1. Logga in på [instrumentpanelen i Partnercenter med](https://partner.microsoft.com/dashboard/) dina autentiseringsuppgifter för Azure AD-klientorganisationen (dina autentiseringsuppgifter för arbetet). Om du inte kan logga in kontaktar du företagets globala administratör.

2. Om du uppmanas att välja från ditt arbetskonto eller personliga konto när du **loggar** in **väljer** du **Arbetskonto**.

3. På menyn i Partnercenter väljer **du Incitament** och sedan **Översikt.** Om du inte har behörighet som incitamentsadministratör eller incitament visas kontaktinformationen för alla globala administratörer och kontoadministratörer i ditt företag. Kontakta någon av dessa administratörer för att få incitamentrollen för de MPN-ID:er och incitamentprogram som krävs.

4. Om du redan har rollen incitamentsadministratör visas registreringarna för ditt företag för DE MPN-ID:er och incitamentprogram som du har åtkomst till.

## <a name="some-enrollments-are-missing-from-the-incentives-overview-page"></a>Vissa registreringar saknas på översiktssidan för incitament.

Om du antingen har fått en inbjudan från eller har registrerat dig i ett incitamentprogram som inte längre visas på instrumentpanelen bör du kontrollera att du har rätt åtkomst. Endast användare med rollen Incitamentanvändare eller Incitamentadministratör kan se programmet. Se [Hitta din roll.](./find-your-role.md)

Om du behöver ändra din roll eller behörighet kontaktar du företagets globala administratör eller kontoadministratör. Om du vill veta vilka dessa personer är kan du [läsa Hitta din globala administratör.](./find-your-role.md#find-your-global-admin)

På sidan Översikt visas endast registreringar som är associerade med det globala partnerkontot (PGA) som är associerat med Azure AD-klientorganisationen. Om ditt företag har fler än en PGA måste du ha olika autentiseringsuppgifter för var och en.

## <a name="who-should-i-contact-if-i-get-an-error-message-or-need-help-during-the-enrollment-process"></a>Vem ska jag kontakta om jag får ett felmeddelande eller behöver hjälp under registreringsprocessen?

Det finns en onlinesupporttjänst om du stöter på problem i avsnittet Incitament på instrumentpanelen – se supportalternativet (? Ikon) längst upp till höger.

## <a name="next-steps"></a>Nästa steg

- [Komma igång med incitament](incentives-get-started-intro.md)