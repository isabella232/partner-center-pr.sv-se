---
title: Visa information om incitament och program
ms.topic: article
ms.date: 11/01/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
description: Använd dessa sidor för att visa och hantera Incitamentsprogram status
author: mseamons
ms.author: mseamons
ms.localizationpriority: medium
ms.custom: SEOJULY.20
ms.openlocfilehash: 33ec3befdc4b2bab2f31d25d210679594debbbf1
ms.sourcegitcommit: 1161d5bcb345e368348c535a7211f0d353c5a471
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/09/2021
ms.locfileid: "123960573"
---
# <a name="view-your-incentives-program-details"></a>Visa information om incitamentsprogrammet

**Lämpliga roller:** Incitamentsadministratörsroller | Incitament för | Globala | MPN-partneradministratör

Den här artikeln förklarar **översiktssidan Mina** incitament, som visar övergripande status för dina incitamentsprogram, samt status för varje program på varje plats. Den ger även de olika registreringsstatusarna.

>[!NOTE]
>Mer information om incitament och incitamentsfunktioner i Partnercenter finns i [Partnerinvesteringar och incitament](https://partner.microsoft.com/membership/partner-incentives) (inloggning krävs).

## <a name="access-the-incentives-overview-page"></a>Få åtkomst till sidan med incitamentsöversikten

1. Logga in på [instrumentpanelen i Partnercenter](https://partner.microsoft.com/dashboard).
1. Välj **Incitament** och **sedan Översikt** på menyn.
1. Du ser en sammanfattning av dina intäkter och betalningar längst upp på sidan och ytterligare information i tabellen nedtill. Du kan också sortera, gruppera och expandera den tillhörande tabellen:

   - Om du vill sortera efter kolumn väljer du kolumnnamnet.
   - Om du vill gruppera efter program väljer **du fliken** Efter program ovanför tabellen.
   - Om du vill gruppera efter plats väljer **du fliken** Efter plats ovanför tabellen.
   - Om du vill visa mer information om registreringar inom en viss grupp väljer du sparrsymbolen i slutet av en viss rad. Den här sparren expanderar vyn.
1. Om du behöver göra något mer för att registrera dig i ett program visas den här informationen i kolumnen **Status**. I så fall kan du välja symbolen » för att läsa mer om vad du behöver göra.

## <a name="enrollment-status"></a>Registreringsstatus

I följande tabell beskrivs de olika registreringstillstånd som visas i **kolumnen** Status.

| **Status**         | **Visas när** |
|:------------------------------------|:------------------|
| Åtgärd som krävs  | Partnern har accepterat en inbjudan att registrera sig i ett incitamentprogram, men kan behöva uppdatera bank- eller skatteinformation. Se kolumnen **Åtgärder som krävs** för eventuella nästa steg eller länkar för att uppdatera din bank- eller skatteinformation i Partnercenter. |
| Avvecklade  | Det specifika incitamentprogrammet erbjuds inte längre i incitamentssystemet. |
| Registrerad  | All skatte- och bankinformation har verifierats. Ingen ytterligare registreringsåtgärd krävs av partnern. |
| Registrerar  | Användaren är inte incitamentadministratör och registreringen är i den åtgärd som **krävs eller** **verifierar registrerings tillstånd.**|
| Inaktiv/ej tillgänglig | Incitamentprogrammet kanske inte är öppet för registrering just nu eller så uppfyller inte partnern aktuell behörighet för registrering eller omregistrering. <br><br> Om statusen **är Ej berättigad uppfyller** partnern inte de aktuella behörighetskraven för programmet. Om du **väljer länken Se behörighetskrav** under registreringsstatusen visas behörighetskraven och vilka av dessa krav som har uppfyllts. <br><br> Du kan också se **en inaktiv** status för registreringar av virtuella organisationer (VORG) eller PARTNER Global Account (PGA) som inte längre är aktiva i incitamentprogrammet.  |
| Inbjuden  | En ny inbjudan till registrering av incitamentprogram har skickats till partnern, men partnern har ännu inte startat registreringsprocessen. I den intilliggande **kolumnen Åtgärder** krävs visas nästa steg och eventuella relaterade länkar.  |
| Verifiera registrering  | Partnern har redan slutfört eller uppdaterat bank- och skatteinformation för en ny eller befintlig registrering och väntar på att Microsoft ska verifiera den här informationen. Under valideringsprocessen kan **Verifiering av registrering visas** i upp till 48 timmar.  |

## <a name="see-your-payment-information"></a>Visa din betalningsinformation

Välj utbetalningsikonen i det övre högra hörnet på skärmen för att få åtkomst till dessa olika sammanfattningar:

- Transaktionshistorik
- Betalningar
- Exportera data

:::image type="content" source="images/payouts/payout-overview.png" alt-text="Visar utbetalningsikonen i det övre högra hörnet i Partnercenter-portalen.":::

I den här informationen ingår totala incitamentsintäkter och betalningar sedan du registrerade dig i incitamentsprogrammet. På den här sidan ser du även intäkter och betalningar efter plats eller program samt eventuella ytterligare åtgärder du kan behöva utföra för att registrera dig i ett program på en viss plats. 

Du kan också använda [partnerns utbetalnings-API för](https://apidocs.microsoft.com/services/partnerpayouts) att ansluta och hämta utbetalningstransaktioner och betalningsdata direkt. Mer [information finns i Utbetalningsutdrag.](payout-statement.md)

## <a name="next-steps"></a>Nästa steg

- [Utbetalningsinstruktioner](payout-statement.md)
