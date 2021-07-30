---
title: Felsöka problem med betalningar och intäkter
ms.topic: article
ms.date: 02/05/2021
description: Lär dig hur du löser problem som saknade eller felaktiga intäkter, berättigandeproblem och hur du stämma av dina incitamentsintäkter.
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
author: Karthic83
ms.author: kashanum
ms.localizationpriority: medium
ms.openlocfilehash: 7e3f3e206c851fbcc68ecd47f6027a2d5856478e
ms.sourcegitcommit: ad1af627f5ee6b6e3a70655f90927e932cf4c985
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 07/29/2021
ms.locfileid: "114844783"
---
# <a name="troubleshooting-missing-payments-incorrect-earnings-and-other-issues"></a>Felsöka uteblivna betalningar, felaktiga intäkter och andra problem

**Lämpliga roller:** Incitamentsadministratör

Den här artikeln hjälper dig att lösa eventuella problem med intäkter eller betalningar i ditt incitamentsprogram. Ämnen som omfattas omfattar tidsinställning för betalningar, kontroll av berättigande till intäkter och vikten av att konfigurera utbetalnings- och skatteprofiler på rätt sätt.

## <a name="who-can-create-or-update-payout-and-tax-profiles-for-my-organization"></a>Vem kan skapa eller uppdatera utbetalnings- och skatteprofiler för min organisation?

Användare som har rollen som incitamentadministratör i Partnercenter för relevant incitamentprogram och MPN-plats kan uppdatera och se utbetalnings- och skatteprofiler för organisationen.

## <a name="how-long-does-it-take-for-microsoft-to-approve-my-pending-payout-andor-tax-profiles"></a>Hur lång tid tar det för Microsoft att godkänna mina väntande utbetalningar och/eller skatteprofiler?

Det kan ta upp till 48 timmar innan godkännandet går igenom. Under den här tiden visas din profil på sidan Översikt med statusen Verifierar registrering. När processen är klar visas statusen  antingen som Registrerad om åtgärden lyckades eller Åtgärd krävs – Uppdatera betalnings- **och/eller skatteinformation** om det behövs.

## <a name="how-do-i-know-if-i-have-completed-my-payout-and-tax-profile-correctly"></a>Hur vet jag om jag har fyllt i uppgifterna för min utbetalnings- och skatteprofil korrekt?

Statusen för din registrering visas på översiktssidan. När du har skapat dina profiler är statusen **Verifierar registreringen**. När vi har verifierat din information ändras statusen **till Registrerad.** Den här statusen anger att din utbetalnings- och skatteprofil och din registrering har slutförts.

## <a name="why-do-i-need-to-update-my-tax-profile-to-use-it-with-a-new-incentive-program"></a>Varför måste jag uppdatera min skatteprofil för att använda den med ett nytt incitamentprogram?

Vi betalar incitament från olika platser beroende på typ av incitament. Dessa olika platser kan kräva ytterligare skatteinformation, beroende på reglerna för incitamentprogrammet.

## <a name="how-can-i-delete-a-payment-andor-tax-profile"></a>Hur kan jag ta bort en betalnings- och/eller skatteprofil?

För närvarande går det inte att ta bort befintliga utbetalnings- och skatteprofiler.

## <a name="my-payment-is-missing-or-incorrect"></a>Min betalning saknas eller är felaktig

Om en betalning saknas eller är fel, så beror det ofta på något av följande:

- **Du kanske inte är berättigad.**  Intäkter är endast tillgängliga om du uppfyller behörighetskraven, det vill säga att du har registrerat dig för respektive programs intäktsperiod.
- **Du kanske inte uppfyller kraven.**  Kontrollera att du uppfyller behörighetskraven och intäktsreglerna för det aktuella incitamentet.

  **Så här kontrollerar du berättigandet**

  1. Logga in på [Partnerincitament](https://partner.microsoft.com/membership/partner-incentives).

  2. Rulla ned till dokumenten för ditt program.
  
  3. Välj den dokumentlänk som du vill använda och granska sedan avsnitten 

**Partnerberättigande och** **intäktsregler för berättigade partner.**

- **Din betalningsprofil kan vara ofullständig.** Startdatumet för dina incitamentintäkter är den första dagen i månaden då du uppfyllde alla behörighetskrav, inklusive registrering av utbetalnings- och skatteuppgifter. Intäkter är inte tillgängliga under månaderna innan utbetalnings- och skatteuppgifterna registrerats. Om du till exempel uppfyller alla krav under april 2020 blir startdatumet för intäkter 1 april 2020.
- **Du kan ha en utestående åtgärd**.  Dina incitament kanske inte behandlas eftersom det finns en väntande åtgärd som du behöver utföra.

  **Så här visar du dina utestående åtgärder**

  1. Logga in på [Partnerincitament](https://partner.microsoft.com/membership/partner-incentives).
  2. Öppna sidan **Transaktionshistorik.** Granska fälten på den här sidan för eventuella utestående åtgärder som ska slutföras, till exempel väntande skatteprofil, väntande betalningsprofil **eller** **väntande momsfaktura.**

Om de här åtgärderna inte hjälper och dina betalningar fortfarande saknas eller är felaktiga kontaktar du [supporten.](https://partner.microsoft.com/dashboard/support/incentives/servicerequests?category=incentives)

## <a name="how-can-i-reconcile-my-adjustments"></a>Hur kan jag stämma av mina justeringar?

Du kan hitta och stämma av dina justeringar genom att ladda ned information om dina intjäningar och transaktioner.

1. Logga in på [instrumentpanelen i Partnercenter](https://partner.microsoft.com/dashboard/).
2. I det övre navigeringsfältet väljer du valutaikonen och sedan **Transaktionshistorik.**
3. Använd lämpliga filter. (Se **viktig information** nedan.)
4. När du har filtrerat dina data väljer du **Starta nedladdning** och sedan **Exportera data.** Dina data öppnas i en CSV-fil.
5. I CSV-filen går du till Kolumn P, **typ av intjäning.**
6. Filtrera den här kolumnen **för Adjustment-Beser .** Du kan se månaden för varje justering i Kolumn S.

>[!IMPORTANT]
>Justeringar som tillämpas på tidigare intäktsperioder visas inte i intäkterna för den månad då justeringen tillämpades. Justeringarna återspeglas alltid i intäktsrapporten för den månad då justeringen tillämpades.
>
>En justering för januari 2019-intäkter som bearbetades i september 2019 återspeglar till exempel inte intäktsbeloppet för september 2019. Men när betalningen för september 2019 tas emot inkluderar den justeringen för januari 2019 som tillämpades i september. I det här scenariot måste du ladda ned transaktionsinformationen för januari 2019 för att se den justering som tillämpades.
>
>Tänk på detta när du anger datumfilter. Som nämnts ovan visas justeringar för tidigare perioder endast under den månad då justeringen tillämpades. Kontrollera att det valda datumintervallet motsvarar månaden för justeringen som du försöker hitta. Du kan behöva välja **Rensa alla för** att ta bort dina filter och sedan använda nya.

## <a name="why-are-my-co-op-claim-payments-made-in-two-different-currencies"></a>Varför görs mina betalningar på gemensamma anspråk i två olika valutor?

När gemensamma medel intjänas från olika Microsoft-enheter görs betalningar i den lokala valutan för varje enhet.  

## <a name="why-was-i-paid-in-a-currency-other-than-my-co-op-claim-currency"></a>Varför har jag betalats i en annan valuta än min valuta för gemensamma anspråk?

Varje incitamentsprogram har en bankprofil som har skapats vid installationen. Den valuta som anges i profilen är den valuta du får betalt i.

## <a name="i-dont-see-earnings-for-a-certain-period"></a>Jag ser inte intäkter under en viss period

När du inte ser intäkter under en period då de förväntas beror det vanligtvis på något av följande problem:

- **Du kanske inte är berättigad.**  Intäkter är endast tillgängliga om du uppfyller behörighetskraven, det vill säga att du har registrerat dig för respektive programs intäktsperiod.

- **Din betalningsprofil kan vara ofullständig.**  Startdatumet för dina incitamentintäkter är den första dagen i månaden då du uppfyllde alla behörighetskrav, inklusive registrering av utbetalnings- och skatteuppgifter. Intäkter är inte tillgängliga under månaderna innan utbetalnings- och skatteuppgifterna registrerats. Om du till exempel uppfyller alla krav under april 2020 blir startdatumet för intäkter 1 april 2020.

Om du har slutfört behörighetskraven, inklusive registrering med utbetalnings- och skatteinformation i tid och intäkter fortfarande saknas, kontaktar du [supporten.](https://partner.microsoft.com/dashboard/support/incentives/servicerequests?category=incentives)

## <a name="my-earnings-are-missing-or-incorrect"></a>Mina intäkter saknas eller är felaktiga

Intäkter som saknas eller inte stämmer kan bero på något av följande problem:

- **Du kanske inte uppfyller kraven.**  Kontrollera att du uppfyller [behörighetskraven](#my-payment-is-missing-or-incorrect) och intäktsreglerna för det aktuella incitamentet.

- **Det kan förekomma någon avvikelse.**  Om du uppfyller både [](incentives-confirm-your-earnings-eligibility.md) [behörighetskraven för program](incentives-determined-your-program-eligibility.md) och intäkter och dina intäkter fortfarande verkar vara felaktiga kan följande information hjälpa dig att hämta dina data.

Intäkter visas både på sidan **Transaktionshistorik** och **på sidan** Betalningar. Du kan komma åt båda sidorna genom att **välja utbetalningsikonen** i navigeringsfältet i Partnercenter.

:::image type="content" source="images/incentives/paymenticon.png" alt-text="Transaktionsinformation.":::

Månatliga intäktsbelopp i vyn Transaktionshistorik överensstämmer kanske inte med betalningsbeloppet som tagits emot under en viss månad. Detta beror på omberäkningar och justeringar för tidigare intjäningsperioder som tillämpas på framtida betalningar.

Till exempel återspeglas inte en justering för intäkter för januari 2019 som bearbetades i september 2019 i intäktsbeloppet för september 2019. Men när betalningen för september 2019 tas emot inkluderar den justeringen för januari 2019 som tillämpades i september.

I det här scenariot behöver du ladda ned transaktionsinformationen för att få en fullständig vy över alla intäkter som ingår i betalningen.  Dessutom kan du gå till vyn Betalningar för att ladda ned transaktioner för varje betalning.

### <a name="transaction-history"></a>Transaktionshistorik

Den här vyn visar intäkts- och betalningstrender per månad, intäkter efter status och transaktionsinformation samt betalningsstatus för varje transaktion. Data visas bara för de program och MPN-ID:er som du är incitamentanvändare eller administratör för.

### <a name="payments"></a>Betalningar

I den här vyn kan du visa betalningar för alla program och MPN-ID:er. Data visas bara för de program och MPN-ID:er som du är incitamentanvändare eller administratör för. Från den här vyn kan du ladda ned banköverföring eller visa transaktionsinformation efter betalning.

| Gör så här: | Gå hit |
| ------ | :----------- | 
| Visa din betalningsinformation per rad, inklusive intjäning och betalningsbelopp i lokal valuta  | Se **fältet Lista över** betalningar   |
| Ladda ned en betalningsbokstav   |  Välj **Betalningsöverföring**  |
| Visa transaktionsnivåinformation för en specifik betalning |  Välj **Visa**  |
| Exportera transaktionsinformation till Excel  |  Välj **Börja ladda** ned och välj sedan Exportera **data.** Alla valda filter tillämpas på exporterade data. När statusen har ändrats till Slutförd väljer **du Ladda** ned och följer anvisningarna för att exportera den detaljerade transaktionsrapporten. Uppdatera sidan om statusen inte uppdateras inom fem minuter.  |

### <a name="missing-or-incorrect-earnings-and-payments"></a>Intäkter och betalningar som saknas eller är felaktiga

Om du inte kan hitta någon betalnings- eller transaktionsinformation kontrollerar du om du har tillämpat rätt filter. Eftersom vissa programnamn har ändrats (till exempel att CSP 1T Direct Partner nu CSP Direct Bill Partner) kan du behöva använda flera val.

Om du fortfarande inte kan hitta dina intäkter eller om du tror att intäkterna som visas är felaktiga kontaktar du [supporten.](https://partner.microsoft.com/dashboard/support/incentives/servicerequests?category=incentives)

## <a name="how-do-i-reconcile-my-earnings"></a>Hur gör jag för att mina intäkter?

Gör följande om dina intäkter inte stämmer:

1. **Kontrollera att du är berättigad till intäkter.**  Intäkter är bara tillgängliga om du uppfyller både [programberättigandet och](incentives-determined-your-program-eligibility.md) [intäktsberättigandet.](incentives-confirm-your-earnings-eligibility.md)

2. **Kontrollera att din betalningsprofil har slutförts.**  Startdatumet för dina incitamentintäkter är den första dagen i månaden då du uppfyllde alla behörighetskrav, inklusive registrering av utbetalnings- och skatteuppgifter. Intäkter är inte tillgängliga under månaderna innan utbetalnings- och skatteuppgifterna registrerats. Om du till exempel uppfyller alla krav under april 2020 blir startdatumet för intäkter 1 april 2020. 

3. **Kontrollera att du har uppfyllt kraven.**  Kontrollera om du har uppfyllt behörighets- [och](#my-payment-is-missing-or-incorrect) intäktsreglerna för ditt incitamentprogram.

Om de här åtgärderna inte hjälper och dina intäkter fortfarande inte har stämts av kontaktar du [supporten.](https://partner.microsoft.com/dashboard/support/incentives/servicerequests?category=incentives)

## <a name="where-can-i-find-my-rates"></a>Var hittar jag mina priser?

1. Logga in på [Partnerincitament](https://partner.microsoft.com/membership/partner-incentives).

2. Rulla ned för att få åtkomst till dokumenten för ditt program.

3. Välj dokumentlänken för respektive program.

4. I dokumentet går du till avsnittet **Programstruktur och Priser**.

## <a name="next-steps"></a>Nästa steg

- [Hantera säljsamarbetsanspråk](incentives-managing-co-op-claims.md)