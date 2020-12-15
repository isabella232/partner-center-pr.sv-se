---
title: Visa information om stimulans och program
ms.topic: article
ms.date: 11/01/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
description: Använd dessa sidor för att visa och hantera status för incitaments program
author: mseamons
ms.author: mseamons
ms.localizationpriority: medium
ms.custom: SEOJULY.20
ms.openlocfilehash: 4bf1c7a2abceffc812666456ddae252fca70d8f1
ms.sourcegitcommit: 4e36d1a4ca2f074b55f9b9a08e300734eae1f06d
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 12/15/2020
ms.locfileid: "97492729"
---
# <a name="view-your-incentives-program-details"></a>Visa information om stimulans programmet

**Gäller för**

- Partnercenter

**Lämpliga roller**

- Stimulans administratör
- Stimulans användare
- Incitament skrivskyddad visning
- Global administratör
- MPN-partner administratör

Den här artikeln beskriver hur du kommer åt sidan **Mina incitament-översikter** som visar övergripande status för dina stimulans program, samt status för varje program på varje plats. Den ger också de olika registrerings statusarna. 

>[!NOTE]
>Mer information om stimulans-och stimulans funktioner i Partner Center finns i [partner investeringar och incitament](https://partner.microsoft.com/membership/partner-incentives) (inloggning krävs).

## <a name="access-the-incentives-overview-page"></a>Öppna sidan incitaments översikt

1. Logga in på [partner Center-instrumentpanelen](https://partner.microsoft.com/dashboard).
1. Välj **incitament** och sedan **Översikt** på menyn.
1. Du ser en sammanfattning av dina intäkter och betalningar längst upp på sidan och ytterligare information i tabellen nedtill. Du kan också sortera, gruppera och expandera den tillhör ande tabellen:

   - Markera kolumn namnet om du vill sortera efter kolumn.
   - Om du vill gruppera efter program väljer du fliken **efter program** ovanför tabellen.
   - Om du vill gruppera efter plats väljer du fliken **efter plats** ovanför tabellen.
   - Om du vill visa mer information om registreringar i en specifik grupp väljer du symbolen för» i slutet av en rad. Den här ikonen expanderar vyn.
1. Om du behöver göra något mer för att registrera dig i ett program visas den här informationen i kolumnen **Status**. I så fall kan du välja symbolen » för att läsa mer om vad du behöver göra.

## <a name="enrollment-status"></a>Registreringsstatus

I följande tabell förklaras de olika registrerings tillstånd som visas i kolumnen **status** .

| **Status**         | **Visas när** |
|:------------------------------------|:------------------|
| Åtgärd som krävs  | Partnern har godkänt en inbjudan att registrera sig i ett incitaments program men kan behöva uppdatera bank-eller skatte information. Se kolumnen **åtgärder som krävs** för nästa steg eller Länkar för att uppdatera bank-eller skatte informationen i Partner Center. |
| Utgångna  | Det angivna stimulans programmet erbjuds inte längre i stimulans systemet. |
| Registrerad  | All moms-och bank information har verifierats. Ingen ytterligare registrerings åtgärd krävs av partnern. |
| Registrerar  | Användaren är inte en stimulans administratör och registreringen är i **åtgärd krävs** eller **verifierar registrerings** tillstånd.|
| Inaktiv/inberättigande | Stimulans programmet kanske inte är öppet för registrering vid denna tidpunkt eller så uppfyller partnern inte den aktuella behörigheten för registrering eller registrering. <br><br> Om **statusen är ogiltig** uppfyller partnern inte de aktuella kraven för berättigande för programmet. Om du väljer länken **Se krav för berättigande** under registrerings statusen visas kraven för berättigande och vilka krav som är uppfyllda. <br><br> Du kan också se **inaktiv** status för virtuell organisation (VORG) eller pga-registreringar (partner global Account) som inte längre är aktiva i stimulans programmet.  |
| Inbjud  | En ny inbjudan till stimulans program registrering har skickats till partnern men partnern har ännu inte startat registrerings processen. I kolumnen bredvid **obligatoriska åtgärder** visas nästa steg och relaterade länkar.  |
| Verifierar registrering  | Partnern har redan slutfört eller uppdaterat bank-och skatte information för en ny eller befintlig registrering och väntar på att Microsoft ska verifiera denna information. Under validerings processen kan **valideringen av registreringen** visas i upp till 48 timmar.  |

## <a name="see-your-payment-information"></a>Se din betalnings information

Välj utbetalnings ikonen i det övre högra hörnet på skärmen för att få åtkomst till dessa olika sammanfattningar:

- Transaktions historik
- Betalningar
- Exportera data

:::image type="content" source="images/payouts/payout-overview.png" alt-text="Visar utbetalnings ikonen i det övre högra hörnet på Partner Center-portalen":::

I den här informationen ingår totala incitamentsintäkter och betalningar sedan du registrerade dig i incitamentsprogrammet. På den här sidan ser du även intäkter och betalningar efter plats eller program samt eventuella ytterligare åtgärder du kan behöva utföra för att registrera dig i ett program på en viss plats. 

Du kan också använda [API: et för partner utbetalning](https://apidocs.microsoft.com/services/partnerpayouts) för att ansluta och hämta utbetalnings transaktion och betalnings data direkt. Mer information finns i [utbetalnings instruktioner](payout-statement.md) .

## <a name="next-steps"></a>Nästa steg
- [Utbetalningsinstruktioner](payout-statement.md)
