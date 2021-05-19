---
title: Vanliga frågor och svar om utbetalningar och skatteprofiler
description: Få svar på vanliga frågor om utbetalnings- och skatteinformation i Partnercenter. Innehåller svar om varför dina intäkter skiljer sig från vad du förväntade dig.
ms.service: marketplace
ms.subservice: partnercenter-marketplace-publisher
ms.topic: article
author: eunjkim520
ms.author: eunjkim
ms.date: 05/06/2021
ms.openlocfilehash: 7f5cf168a87c25f3afe0767769ce8dcc77d07f04
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 05/19/2021
ms.locfileid: "110145838"
---
# <a name="common-questions-about-payouts-and-taxes"></a>Vanliga frågor om utbetalning och skatter

**Lämpliga roller:** Kontoadministratörsroller | Globala | Incitamentsadministratör

Den här artikeln besvarar vanliga frågor om utbetalnings- och skatteinformation i Partnercenter. Ämnen som omfattas omfattar tidsinställning av betalningar, kontroll av din intäktsberättigande och vikten av att konfigurera dina utbetalnings- och skatteprofiler på rätt sätt.

## <a name="profile-management"></a>Profilhantering

#### <a name="why-do-i-need-to-provide-or-update-my-payout-andor-tax-details"></a>Varför måste jag ange eller uppdatera min utbetalnings- och/eller skatteinformation?

Alla partner som registrerar sig i ett nytt program måste ange giltig utbetalnings- och skatteinformation för att slutföra registreringen och ta emot betalningar. En registrering anses vara fullständig först när Microsoft har verifierat din utbetalnings- och skatteprofil.

Du kan också behöva uppdatera din information om reglerna för ditt program ändras eller om aspekter av din profil upphör att gälla eller blir inaktuella. Om detta inträffar visas statusen Åtgärd krävs på **översiktssidan – Uppdateringsbank och/eller skatteprofil.**

#### <a name="how-do-i-find-set-up-or-update-payout-and-tax-details"></a>Hur gör jag för att hitta, konfigurera eller uppdatera utbetalnings- och skatteinformation?

Detaljerad information om hur du uppdaterar betalnings- och skatteinformation i Partnercenter finns i [Konfigurera ditt utbetalningskonto och skatteformulär.](set-up-your-payout-account.md)

#### <a name="why-dont-i-see-my-enrollments-when-i-go-to-assign-my-payout-and-tax-profile"></a>Varför visas inte mina registreringar när jag ska tilldela min utbetalnings- och avgiftsprofil?

Det kan vara så att du inte har rätt behörigheter eller att du är inloggad med ett konto som inte har dessa behörigheter. Till exempel kan endast incitamentadministratörer för din MPN-plats skapa eller hantera utbetalnings- och skatteprofiler. Kontakta din organisationsadministratör för hjälp med bank- och skatterelaterade behörigheter.

#### <a name="im-only-able-to-sign-in-with-my-onmicrosoftcom-domain-what-should-i-do"></a>Jag kan bara logga in med min @onmicrosoft.com domän. Vad ska jag göra?

Kontakta kontoadministratören om du vill lägga till fler domäner i AAD-kontot.
 
#### <a name="my-organization-is-participating-in-multiple-programs-do-i-need-to-provide-my-payment-and-tax-profile-multiple-times"></a>Min organisation deltar i flera program. Måste jag ange min betalnings- och skatteprofil flera gånger?

Det beror på organisationens behov. Betalningsprofiler skapas på organisationsnivå, vilket gör att samma bankprofil kan tilldelas över flera MPN-ID:n och program inom en organisation. I de flesta fall kan du antingen återanvända en befintlig profil eller skapa en ny.

Det kan dock finnas undantag när du använder din bankprofil för olika länder eller regioner eftersom lokala bank- eller skatteregler kan gälla.

Skatteprofiler som skapats för en MPN-plats återanvänds och fylls i automatiskt när samma MPN-plats deltar i ett annat program. Men det kan finnas undantag. Utbetalningsreglerna för ett nytt incitamentprogram kan till exempel kräva ytterligare information om skatteprofilen.

#### <a name="can-i-use-the-same-bank-and-tax-details-for-all-incentive-programs-at-microsoft"></a>Kan jag använda samma bank- och skatteinformation för alla incitamentprogram på Microsoft?

Om ditt företag bjuds in för flera program kan du använda samma betalningskonto för alla dina program eller välja att ha olika betalningskonton för de olika programmen.


#### <a name="how-does-microsoft-ensure-that-the-bank-information-is-indeed-that-of-the-company-and-not-a-personal-bank-account-for-an-employee"></a>Hur säkerställer Microsoft att bankinformationen verkligen är företagets och inte ett personligt bankkonto för en anställd?

Det är företagets ansvar att se till att rollen som incitamentsadministratör – som har behörighet att redigera den här informationen – endast ges till lämpliga anställda.

#### <a name="my-tax-profile-has-expired-how-do-i-fix-update-it"></a>Min skatteprofil har upphört att gälla. Hur gör jag för att du uppdatera den?

Om en skatteprofil har upphört att gälla eller snart upphör att gälla, innebär det att skatteformuläret som du har angett till Microsoft måste uppdateras. Använd följande steg för att uppdatera din skatteprofil:

1. Logga in på instrumentpanelen [i Partnercenter](https://partner.microsoft.com/dashboard/home)och välj sedan kugghjulsikonen för att öppna **menyn** Inställningar.
2. Välj **Kontoinställningar,** expandera **avsnittet Utbetalning och** skatt och välj sedan **Utbetalnings- och skatteprofil.**
3. Välj **Skatteprofil**
4. Kontrollera kolumnen Förfallodatum **och gå** till skatteprofilen som har upphört att gälla eller snart upphör att gälla.
5. Välj **Redigera** för att starta redigeringsprocessen för skatteprofilen.
6. I avsnittet skatteformulär anger du den uppdaterade informationen.

## <a name="earnings-incorrect-or-missing"></a>Felaktiga eller saknade intäkter

#### <a name="why-are-my-earnings-missing"></a>Varför saknas min intäkt?

- Kundordern kanske inte är berättigad till utbetalning ännu. För icke-företagskunders beställningar måste Microsoft ta emot kundbetalningar innan utgivaren blir berättigad. För företagskunders beställningar är dina intäkter tillgängliga 1–2 dagar efter inköpsorderdatumet. Verifiera orderstatus i [orderrapporter](https://partner.microsoft.com/dashboard/commercial-marketplace/analytics/order).
- Intäkter från transaktioner före juli 2019 kanske inte visas i rapporten för transaktionshistorik. Läs tidigare utdrag i [Payout Download](https://partner.microsoft.com/dashboard/payouts/reports/incentiveexport) (Ladda ned utbetalning).
- Kontrollera [tidsramen för utbetalningscykeln och](payment-thresholds-methods-timeframes.md) se när dina intäkter ska visas i utbetalningsutdraget.

#### <a name="why-is-my-earnings-amount-different-than-what-i-expected"></a>Varför skiljer sig mina intäkter från det jag förväntade mig?

- Om ordern delvis har betalats av kunden baseras ditt intäktsbelopp på det delvis betalda beloppet efter att du har dra av avgiften och lämplig skatt.
- Kontrollera ansvaret för skatteincheckning efter land. I länder där skatt är Microsoft-ansvarig samlar Microsoft in och drar av skatt från utgivarintäkter. Transaktionsbeloppet som visas i utdraget är efter skattebeloppet. Se [Skatteinformation](tax-details-marketplace.md).
- SaaS- och IaaS-erbjudanden har en rabatterad myndighetsavgift på 10 % i stället för standard 20 %, vilket ger en intäktsfrekvens på 90 %. Det här är ett krav Co-Sell IP-adress. Erbjudandet gäller fram till den 30 juni 2021. 

**Mer information** finns [i : Utgivaravtal](/legal/marketplace/msft-publisher-agreement)för kommersiell [marknadsplats,](payout-policy-details.md)information om utbetalningsprincip, [betalningströskel,](payment-thresholds-methods-timeframes.md)metod och tidsram, få [betalt,](marketplace-get-paid.md) [skatteinformation,](tax-details-marketplace.md) [utbetalningsutdrag](payout-statement.md)

## <a name="earnings-reconciliation"></a>Intäktsavstämning

### <a name="how-do-i-reconcile-payout-statements-to-order-or-usage-reports-in-analytics"></a>Hur gör jag för att stämma av utbetalningsutdrag till order- eller användningsrapporter i Analytics?

Använd AssetID, orderID och radobjekt-ID som visas i rapporten för utbetalningstransaktionshistorik med analytiska beställningar och användningsrapporter. Använd den här mappningen:

- Transaktionshistorik för utbetalning. History.AssetID = order.OrderID
- Payout Transaction History.OrderID & LineItem = Usage.UsageReferenceID [OrderID:LineItemID]

### <a name="how-do-i-know-when-to-expect-payments-for-my-customer-orders"></a>Hur vet jag när jag ska förvänta mig betalning för mina kundbeställningar?

- Börja med att använda ditt assetID och kontrollera kundorder i [orderrapporterna.](https://partner.microsoft.com/dashboard/commercial-marketplace/analytics/order)
- Kontrollera kundkanalen för din kundprenumeration [i kundrapporten](https://partner.microsoft.com/dashboard/commercial-marketplace/analytics/customer).
- För företagskunder visas utgivares intäkter i utdraget 1–2 dagar efter inköpsorderdatumet.
- För icke-företagskunder visas utgivarintäkterna i utdraget 1–2 dagar efter att kundbetalningen har tagits emot.

**Mer information finns** i : [Utbetalningsutdrag,](payout-statement.md) [instrumentpanelen Beställningar på den kommersiella marknadsplatsen](/azure/marketplace/partner-center-portal/orders-dashboard)

## <a name="payments-and-adjustments"></a>Betalningar och justeringar

#### <a name="why-is-my-payment-missing"></a>Varför saknas min betalning?

- Kontrollera att din utbetalningsstatus och skatteprofilstatus visas *som giltiga* på [översiktssidan](https://partner.microsoft.com/dashboard/commercial-marketplace/overview).
- Du kanske inte har uppnått minimitröskelvärdet för en betalning. Intäkterna måste vara minst $50 USD för att du ska få en betalning.


#### <a name="how-do-i-set-my-account-to-not-receive-payment"></a>Hur gör jag för att ange att mitt konto inte ska ta emot betalningar?
Du kan hålla betalningar i [utbetalningsprofilen](https://partner.microsoft.com/dashboard/commercial-marketplace/overview). Om du vill göra detta markerar **du Hold (Håll)** så håller Microsoft betalningen till dig tills du frigör kvarten.

#### <a name="why-do-i-receive-in-a-different-currency-than-the-purchase-currency"></a>Varför får jag betalningar i en annan valuta än inköpsvalutan?

Utbetalningsvalutan baseras på den valuta som du valde i utbetalningsprofilen. Inköpsvalutan baseras på den valuta som kunden betalade i.

#### <a name="how-do-i-reconcile-adjustments"></a>Hur gör jag för att stämma av justeringar?

Betalningsjusteringar är betalningskorrigeringar för att hantera kompensationsjusteringar, till exempel systemproblem. I utbetalningsutdraget anger ReasonCode orsaken till justeringen. Dessa är inte avsedda att stämma av direkt till enskilda transaktioner.

**Mer information** finns [i: Commercial Marketplace Publisher Agreement,](/legal/marketplace/msft-publisher-agreement) [utbetalningsprincipinformation,](payout-policy-details.md) [](tax-details-marketplace.md)skatteinformation, [betalningströskel, metod och tidsram](payment-thresholds-methods-timeframes.md)

## <a name="taxes"></a>Skatter

#### <a name="how-do-we-identify-tax-remit-responsibility-between-microsoft-or-publisher-in-the-payout-statement"></a>Hur identifierar vi ansvaret för skatteinbetalning mellan Microsoft och utgivaren i utbetalningsutdraget?

Leta reda på kolumnen Skattemodell i den nedladdade transaktionshistoriken. Där står det MS Managed (Hanteras av MS) eller ISV Managed (Hanteras av ISV). Se de landsspecifika skattereglerna och utbetalningseffekter i [Skatteinformation](tax-details-marketplace.md).

#### <a name="how-do-i-download-service-fee-tax-forms"></a>Hur gör jag för att hämta skatteformulär för serviceavgifter?

Gå till sidan **Payout Payment** (Utbetalning) och sedan till avsnittet **List of Payment** (Lista över betalningar). En länk till skatteformuläret för serviceavgifter för en betalning som har serviceavgifter/skatt.

#### <a name="where-do-i-find-year-end-tax-forms"></a>Var hittar jag skatteblanketter för slutet av beskattningsåret?

Gå till [profilsidan](https://partner.microsoft.com/dashboard/payee/profiles/partner/manage) för att visa dina skatteblanketter för slutet av beskattningsåret.

#### <a name="how-do-i-find-withholding-tax-for-a-transaction"></a>Hur hittar jag källskatten för en transaktion?
Källskatt gäller för amerikanska utgivare som har skickat in ett W-9-formulär. Källskatt beräknas för en månatlig betalning.

**Mer information finns** i : [Utgivaravtal för](/legal/marketplace/msft-publisher-agreement)Commercial Marketplace , information om [utbetalningsprincip](payout-policy-details.md)

## <a name="payout-statement-access"></a>Åtkomst till utbetalningsutdrag

#### <a name="how-do-i-access-a-payout-statement"></a>Hur får jag åtkomst till ett utbetalningsutdrag?

1. Kontrollera dina roller. Du måste ha rollen *finansiell bidragsgivare* eller *kontoägare* för att få åtkomst till utbetalningsutdrag.
2. I det övre högra navigeringsfönstret väljer du **utbetalningsikonen** för att visa ditt utbetalningsutdrag. Välj mellan **Transaktionshistorik,** **Betalning** och **Ladda ned**.

**Mer information:** [Utbetalningsroller och behörigheter](payout-statement.md#roles-and-permissions), [Utbetalningsutdrag](payout-statement.md) 

## <a name="payout-statement-report"></a>Rapport för utbetalningsutdrag

#### <a name="what-does-each-field-in-the-transaction-download-mean"></a>Vad betyder varje fält i transaktionsnedladdningen?

Se [Utbetalningsutdrag](payout-statement.md) för en detaljerad lista över attributen och deras betydelser.

#### <a name="what-is-earning-status"></a>Vad är intäktsstatus?

Detta visar dina intäkter som antingen obearbetade, bearbetade eller skickade.

- **Obearbetad** – intäkterna är under en depositionsperiod fram till förfallodatumet.
- **Bearbetade** – intäkterna har mognat och förbereds till en månatlig betalning. Betalningar släpps den 15:e i varje månad.
- **Skickat** – Betalningen har publicerats till din bank baserat på din utbetalningsprofil.

#### <a name="how-do-i-download-service-fee-tax-forms"></a>Hur gör jag för att hämta skatteformulär för serviceavgifter?

Gå till sidan **Payout Payment** (Utbetalning) och sedan till avsnittet **List of Payment** (Lista över betalningar). En länk till skatteformuläret för serviceavgifter för en betalning som har serviceavgifter/skatt.

#### <a name="how-do-i-download-a-withholding-tax-form-in-pdf"></a>Hur gör jag för att du ladda ned ett källskatteformulär i PDF-format?

Gå till sidan **Payout Payment** (Utbetalning) och sedan till avsnittet **List of Payment** (Lista över betalningar). En länk till ett källskatteformulär visas bredvid en betalning. Ett källskatteformulär gäller endast för valda incitamentprogram, inte för utbetalning från den kommersiella marknadsplatsen.

#### <a name="where-do-i-find-year-end-tax-forms"></a>Var hittar jag skatteblanketter för slutet av beskattningsåret?

Gå till [profilsidan](https://partner.microsoft.com/dashboard/payee/profiles/partner/manage) för att visa dina skatteblanketter för slutet av beskattningsåret.

**Mer information:** [Utbetalningsutdrag](payout-statement.md), [nedladdning av transaktionshistorik](payout-statement.md#transaction-history-download)

## <a name="historical-statements"></a>Historiska uttryck

#### <a name="how-do-i-view-historical-information"></a>Hur gör jag för att du visa historisk information?

Historiskt utdrag visar en ögonblicksbild av utbetalningsdata från oktober 2019. Utbetalningsinformationen här uppdateras tyvärr inte. Om du vill få den senaste informationen skickar du en supportbiljett för den senaste informationen.

**Mer information:** [Utbetalningsutdrag,](payout-statement.md) [nedladdning av transaktionshistorik](payout-statement.md#transaction-history-download)

## <a name="payout-export-api"></a>API för utbetalningsexport

#### <a name="how-do-i-download-payout-data"></a>Hur gör jag för att ladda ned utbetalningsdata?

Använd [partnerns utbetalnings-API.](https://apidocs.microsoft.com/services/partnerpayouts)

## <a name="commercial-marketplace-payout-policies"></a>Utbetalningsprinciper för den kommersiella marknadsplatsen

#### <a name="how-do-i-find-the-current-agency-fee-and-the-payout-rate"></a>Hur gör jag för att hitta aktuellt arvode och utbetalningsfrekvens?

- Kontrollera utgivaravtalet för kommersiell marknadsplats. Standardarvodet är 20 %. SaaS-säljberättigade transaktioner har en rabatterad avgift på 10 %. Sök efter meddelanden om arvoden för PR-byråer.
- I ditt utbetalningsutdrag anger intjäningstakten den faktiska utbetalningsfrekvensen för en viss transaktion.

#### <a name="when-can-i-expect-a-payment-from-microsoft-once-earnings-appear-on-my-statement"></a>När kan jag vänta mig en betalning från Microsoft när intäkterna visas i mitt utdrag?
- När dina intäkter har status obearbetad kan du kontrollera förfallodatum för den månad då dina intäkter bearbetas för betalning. När din betalning har förberetts ändras din intäktsstatus till "bearbetad".  Microsoft släpper betalningar den 15:e i förfallomånaden.
- För beställningar som betalas med kreditkort håller Microsoft betalningar i 30 dagar tills intjäning har mognat.

 **Mer information** finns [i : Utgivaravtal](/legal/marketplace/msft-publisher-agreement)för kommersiell marknadsplats, information [om](payout-policy-details.md) [utbetalningsprincip,](tax-details-marketplace.md) [skatteinformation, betalningströskel, metod och tidsram](payment-thresholds-methods-timeframes.md)

## <a name="next-steps"></a>Nästa steg

- [Få betalt](marketplace-get-paid.md)
- [Konfigurera utbetalningskonto och deklarationsblanketter](set-up-your-payout-account.md)