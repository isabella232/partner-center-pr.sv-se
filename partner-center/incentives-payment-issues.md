---
title: Felsöka problem med betalningar och intäkter
ms.topic: article
ms.date: 02/05/2021
description: Lär dig hur du löser problem som saknade eller felaktiga intäkter, berättigande problem och hur du kan stämma av dina incitament.
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
author: Karthic83
ms.author: kashanum
ms.localizationpriority: medium
ms.openlocfilehash: c6ff8915384f8c7ab98fa058f2e45e3d0b4f7214
ms.sourcegitcommit: 6498c57e75aa097861523b206dc142f789deeb36
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/02/2021
ms.locfileid: "106179521"
---
# <a name="troubleshooting-missing-payments-incorrect-earnings-and-other-issues"></a>Felsöka saknade betalningar, felaktiga intäkter och andra problem

**Lämpliga roller**

- Incitaments administratör

Den här artikeln hjälper dig att lösa eventuella intäkter eller betalnings problem i stimulans programmet. Ämnen som omfattas inkluderar tids inställning för betalningar, kontroll av intäkts berättigande och betydelsen av att ställa in dina utbetalnings-och skatte profiler korrekt.

## <a name="who-can-create-or-update-payout-and-tax-profiles-for-my-organization"></a>Vem kan skapa eller uppdatera utbetalnings-och skatte profiler för min organisation?

Användare som har rollen incitaments administratör i Partner Center för det relevanta stimulans programmet och MPN-platsen kan uppdatera och se utbetalnings-och skatte profiler för organisationen.

## <a name="how-long-does-it-take-for-microsoft-to-approve-my-pending-payout-andor-tax-profiles"></a>Hur lång tid tar det för Microsoft att godkänna mina väntande utbetalningar och/eller skatteprofiler?

Det kan ta upp till 48 timmar innan godkännandet går igenom. Under den här tiden visas din profil på sidan Översikt med statusen Verifierar registrering. När processen har slutförts visas statusen antingen **registrerad** om lyckad eller **åtgärd krävs – uppdatera betalning och/eller skatte information** om det behövs.

## <a name="how-do-i-know-if-i-have-completed-my-payout-and-tax-profile-correctly"></a>Hur vet jag om jag har fyllt i uppgifterna för min utbetalnings- och skatteprofil korrekt?

Statusen för din registrering visas på översiktssidan. När du har skapat dina profiler kommer din status att **Verifiera registreringen**. När vi har verifierat din information ändras statusen till **registrerad**. Denna status anger att din utbetalnings-och skatte profil och registreringen har slutförts.

## <a name="why-do-i-need-to-update-my-tax-profile-to-use-it-with-a-new-incentive-program"></a>Varför måste jag uppdatera min skatteprofil för att använda den med ett nytt incitamentprogram?

Vi betalar incitament från olika platser beroende på typ av incitament. Dessa olika platser kan kräva ytterligare skatteinformation, beroende på reglerna för incitamentprogrammet.

## <a name="how-can-i-delete-a-payment-andor-tax-profile"></a>Hur kan jag ta bort en betalnings- och/eller skatteprofil?

För närvarande går det inte att ta bort befintliga utbetalnings- och skatteprofiler.

## <a name="my-payment-is-missing-or-incorrect"></a>Min betalning saknas eller är felaktig

Om en betalning saknas eller är fel, så beror det ofta på något av följande:

- **Du kanske inte är berättigad.**  Intäkter är endast tillgängliga om du uppfyller behörighetskraven, det vill säga att du har registrerat dig för respektive programs intäktsperiod.
- **Du kanske inte uppfyller kraven.**  Kontrollera att du uppfyller behörighetskraven och intäktsreglerna för det aktuella incitamentet.

  **Kontrol lera din behörighet**

  1. Logga in på [partner incitament](https://partner.microsoft.com/membership/partner-incentives).

  2. Rulla ned till dokumenten för ditt program.
  
  3. Välj den dokument länk som du vill använda och granska sedan avsnitten 

Regler för **partner berättigade** och **berättigade intäkter**.

- **Din betalnings profil kan vara ofullständig.** Startdatumet för dina incitamentintäkter är den första dagen i månaden då du uppfyllde alla behörighetskrav, inklusive registrering av utbetalnings- och skatteuppgifter. Intäkter är inte tillgängliga under månaderna innan utbetalnings- och skatteuppgifterna registrerats. Om du till exempel uppfyller alla krav under april 2020 blir startdatumet för intäkter 1 april 2020.
- **Du kan ha en utestående åtgärd**.  Dina incitament kanske inte behandlas eftersom det finns en väntande åtgärd som du behöver utföra.

  **Så här visar du dina utestående åtgärder**

  1. Logga in på [partner incitament](https://partner.microsoft.com/membership/partner-incentives).
  2. Öppna **transaktions historik** sidan. Granska fälten på den här sidan för eventuella utestående åtgärder som ska slutföras, till exempel **väntande skatte profil**, **väntande betalnings profil** eller **överföring av väntande moms faktura**.

Kontakta [supporten](https://partner.microsoft.com/dashboard/support/incentives/servicerequests?category=incentives)om dessa åtgärder inte hjälper och dina betalningar fortfarande saknas eller är felaktiga.

## <a name="how-can-i-reconcile-my-adjustments"></a>Hur kan jag synkronisera mina justeringar?

Du kan hitta och synkronisera dina justeringar genom att hämta information om dina uppgifter och transaktioner.

1. Logga in på [instrumentpanelen i Partnercenter](https://partner.microsoft.com/dashboard/).
2. Välj Money-ikonen i det övre navigerings fältet och välj sedan **transaktions historik**.
3. Tillämpa lämpliga filter. (Se den **viktiga** kommentaren nedan.)
4. När du har filtrerat dina data väljer du **Starta hämtning** och väljer **Exportera data**. Dina data kommer att öppnas i en CSV-fil.
5. I CSV-filen navigerar du till kolumn P, **typ av typ**.
6. Filtrera den här kolumnen för **justering – rabatt**. Du kan se månad för varje justering i kolumn S.

>[!IMPORTANT]
>Justeringar som tillämpas på föregående intäkts perioder visas inte i intäkterna för den månad då justeringen tillämpades. Justeringar kommer alltid att avspeglas i vinst rapporten för den månad då justeringen tillämpades.
>
>Till exempel kommer en justering för januari 2019-intäkter som bearbetades i september 2019 inte att avspeglas i intäkts beloppet för september 2019. Men när betalningen för september 2019 tas emot kommer det att ta med justeringen för januari 2019 som tillämpades i september. I det här scenariot måste du hämta transaktions informationen för januari 2019 för att se den justering som tillämpades.
>
>Tänk på detta när du anger dina datum filter. Som nämnts ovan visas justeringar för föregående perioder bara under den månad då justeringen tillämpades. Kontrol lera att det valda datum intervallet motsvarar månads justeringen som du försöker hitta. Du kan behöva välja **Rensa alla** för att ta bort dina filter och sedan använda nya.

## <a name="why-are-my-co-op-claim-payments-made-in-two-different-currencies"></a>Varför görs mina betalningar på gemensamma anspråk i två olika valutor?

När gemensamma medel intjänas från olika Microsoft-enheter görs betalningar i den lokala valutan för varje enhet.  

## <a name="why-was-i-paid-in-a-currency-other-than-my-co-op-claim-currency"></a>Varför har jag betalats i en annan valuta än min valuta för gemensamma anspråk?

Varje incitamentsprogram har en bankprofil som har skapats vid installationen. Den valuta som anges i profilen är den valuta du får betalt i.

## <a name="i-dont-see-earnings-for-a-certain-period"></a>Jag ser inga intäkter under en viss period

När du inte ser intäkter under en period som de förväntas vara, beror det vanligt vis på ett av följande problem:

- **Du kanske inte är berättigad.**  Intäkter är endast tillgängliga om du uppfyller behörighetskraven, det vill säga att du har registrerat dig för respektive programs intäktsperiod.

- **Din betalnings profil kan vara ofullständig.**  Startdatumet för dina incitamentintäkter är den första dagen i månaden då du uppfyllde alla behörighetskrav, inklusive registrering av utbetalnings- och skatteuppgifter. Intäkter är inte tillgängliga under månaderna innan utbetalnings- och skatteuppgifterna registrerats. Om du till exempel uppfyller alla krav under april 2020 blir startdatumet för intäkter 1 april 2020.

Om du har slutfört berättiganderegler, inklusive onboarding med utbetalnings-och skatte information i tid, och intäkterna fortfarande saknas, kontaktar du [supporten](https://partner.microsoft.com/dashboard/support/incentives/servicerequests?category=incentives).

## <a name="my-earnings-are-missing-or-incorrect"></a>Mina intäkter saknas eller är felaktiga

Intäkter som saknas eller inte stämmer kan bero på något av följande problem:

- **Du kanske inte uppfyller kraven.**  Kontrollera att du uppfyller [behörighetskraven](#my-payment-is-missing-or-incorrect) och intäktsreglerna för det aktuella incitamentet.

- **Det kan förekomma någon avvikelse.**  Om du uppfyller kraven för [program berättigande](incentives-determined-your-program-eligibility.md) och [intäkts](incentives-confirm-your-earnings-eligibility.md) krav och intäkterna fortfarande verkar vara felaktiga, kan följande information hjälpa dig att hämta dina data.

Intäkter visas både på sidan **transaktions historik** och på sidan **betalningar** . Du kan komma åt båda sidorna genom att välja **utbetalnings** ikonen i navigerings fältet i Partner Center.

:::image type="content" source="images/incentives/paymenticon.png" alt-text="Transaktionsinformation":::

Månads Visa belopp i vyn transaktions historik kanske inte överensstämmer med det betalnings belopp som har tagits emot för en angiven månad. Detta beror på omberäkningar och justeringar för tidigare arbets perioder som tillämpas på framtida betalningar.

Till exempel kommer en justering för januari 2019-intäkter som bearbetades i september 2019 inte att avspeglas i intäkts beloppet för september 2019. men när betalningen för september 2019 tas emot kommer det att ta med justeringen för januari 2019 som tillämpades i september.

I det här scenariot måste du hämta transaktions informationen för att få en fullständig vy över alla intäkter som ingår i din betalning.  Dessutom kan du gå till vyn betalningar för att ladda ned transaktioner för varje betalning.

### <a name="transaction-history"></a>Transaktions historik

I den här vyn visas vinst-och betalnings trender per månad, intäkter efter status och transaktions information tillsammans med betalnings status för varje transaktion. Data visas bara för de program och MPN-ID: n som du är stimulans användare eller administratör för.

### <a name="payments"></a>Betalningar

Med den här vyn kan du Visa betalningar för alla program och MPN-ID: n. Data visas bara för de program och MPN-ID: n som du är stimulans användare eller administratör för. I den här vyn kan du hämta remitteringen eller Visa transaktions information per betalning.

| Gör så här: | Gå hit |
| ------ | :----------- | 
| Visa betalnings information per rad, inklusive kostnader för betalning och betalning i lokal valuta  | Se **listan över betalnings** fält   |
| Ladda ned en remitterings bokstav   |  Välj **betalnings remittering**  |
| Visa information om transaktions nivå för en speciell betalning |  Välj **vy**  |
| Exportera transaktions information till Excel  |  Välj **starta nedladdning** och välj sedan **Exportera data**. Alla valda filter kommer att tillämpas på exporterade data. När statusen har ändrats till slutförd väljer du **Hämta** och följer anvisningarna för att exportera rapporten detaljerade transaktioner. Uppdatera sidan om statusen inte uppdateras inom fem minuter.  |

### <a name="missing-or-incorrect-earnings-and-payments"></a>Saknad eller felaktig vinst och betalning

Om du inte kan hitta någon betalnings-eller transaktions information kontrollerar du om du har tillämpat rätt filter. Eftersom vissa program namn har ändrats (t. ex. är CSP 1T Direct-partnern nu KRYPTOGRAFIPROVIDERns direkta fakturerings partner), kan du behöva använda flera val.

Om du fortfarande inte kan hitta dina intäkter eller om du anser att de intäkter som visas är felaktiga, kan du kontakta [supporten](https://partner.microsoft.com/dashboard/support/incentives/servicerequests?category=incentives).

## <a name="how-do-i-reconcile-my-earnings"></a>Hur gör jag för att stämma av min vinst?

Gör följande om dina intäkter inte stämmer:

1. **Kontrollera att du är berättigad till intäkter.**  Intäkter kommer bara att vara tillgängliga om du uppfyller både [program berättigande](incentives-determined-your-program-eligibility.md) och [intäkts berättigande](incentives-confirm-your-earnings-eligibility.md).

2. **Kontrollera att din betalningsprofil har slutförts.**  Startdatumet för dina incitamentintäkter är den första dagen i månaden då du uppfyllde alla behörighetskrav, inklusive registrering av utbetalnings- och skatteuppgifter. Intäkter är inte tillgängliga under månaderna innan utbetalnings- och skatteuppgifterna registrerats. Om du till exempel uppfyller alla krav under april 2020 blir startdatumet för intäkter 1 april 2020. 

3. **Kontrollera att du har uppfyllt kraven.**  Kontrol lera om du har uppfyllt reglerna som [berättigad](#my-payment-is-missing-or-incorrect) och berättigad inkomst för ditt incitaments program.

Kontakta [supporten](https://partner.microsoft.com/dashboard/support/incentives/servicerequests?category=incentives)om dessa åtgärder inte hjälper och dina intäkter fortfarande inte har stämts av.

## <a name="where-can-i-find-my-rates"></a>Var hittar jag mina priser?

1. Logga in på [partner incitament](https://partner.microsoft.com/membership/partner-incentives).

2. Rulla ned för att komma åt dokumenten för ditt program.

3. Välj dokument länken för respektive program.

4. I dokumentet refererar du till avsnittets **program struktur och priser**.

## <a name="next-steps"></a>Nästa steg

- [Hantera säljsamarbetsanspråk](incentives-managing-co-op-claims.md)