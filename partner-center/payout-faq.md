---
title: Vanliga frågor och svar om betalning och skatte profil
description: Få svar på vanliga frågor om utbetalningar och skatte information i Partner Center. Innehåller svar om varför din vinst är annorlunda än förväntat.
ms.service: marketplace
ms.subservice: partnercenter-marketplace-publisher
ms.topic: article
author: eunjkim520
ms.author: eunjkim
ms.date: 11/25/2020
ms.openlocfilehash: 3b09f0a08cd974f88afe5c5708df307830491f3f
ms.sourcegitcommit: 4e36d1a4ca2f074b55f9b9a08e300734eae1f06d
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 12/15/2020
ms.locfileid: "97492593"
---
# <a name="common-questions-about-payouts-and-taxes"></a>Vanliga frågor om utbetalningar och skatter

**Lämpliga roller**:

- Kontoadministratör
- Global administratör
- Incitaments administratör

I den här artikeln besvaras vanliga frågor om utbetalningar och skatte information i Partner Center. ämnen som omfattas är betalnings sätt, kontrollerar kompensations berättigande och vikten av att ställa in dina utbetalningar och skatte profiler korrekt.

## <a name="profile-management"></a>Profil hantering

#### <a name="why-do-i-need-to-provide-or-update-my-payout-andor-tax-details"></a>Varför måste jag ange eller uppdatera mina utbetalnings-och/eller skatte uppgifter?

Alla partner som registrerar sig i ett nytt program måste ange giltiga utbetalnings-och skatte information för att slutföra registreringen och ta emot betalningar. En registrering betraktas som slutförd först efter att Microsoft har verifierat din utbetalnings-och skatte profil.

Du kan också behöva uppdatera din information om reglerna för ditt program ändras, eller om delar av profilen går ut eller blir inaktuella. Om detta händer visar sidan Översikt en status som **krävs – uppdatera bank och/eller skatte profil**.

#### <a name="how-do-i-find-set-up-or-update-payout-and-tax-details"></a>Hur gör jag för att hittar, ställer du in eller uppdaterar du utbetalnings-och skatte information?

Detaljerad information om hur du uppdaterar betalnings-och skatte information i Partner Center finns i [Konfigurera ditt utbetalnings konto och skatte formulär](set-up-your-payout-account.md).

#### <a name="why-dont-i-see-my-enrollments-when-i-go-to-assign-my-payout-and-tax-profile"></a>Varför visas inte mina registreringar när jag ska tilldela min utbetalnings- och avgiftsprofil?

Det kan vara att du inte har rätt behörighet eller att du är inloggad med ett konto som inte har dessa behörigheter. Till exempel kan endast incitaments administratörer för din MPN-plats skapa eller hantera utbetalnings-och skatte profiler. Kontakta din organisationsadministratör för hjälp med bank- och skatterelaterade behörigheter.

#### <a name="im-only-able-to-sign-in-with-my-onmicrosoftcom-domain-what-should-i-do"></a>Jag kan bara logga in med min @onmicrosoft.com domän. Vad ska jag göra?

Kontakta kontoadministratören om du vill lägga till fler domäner till AAD-kontot.
 
#### <a name="my-organization-is-participating-in-multiple-programs-do-i-need-to-provide-my-payment-and-tax-profile-multiple-times"></a>Min organisation deltar i flera program. Måste jag ange min betalnings-och skatte profil flera gånger?

Det beror på organisationens behov. Betalnings profiler skapas på en organisations nivå, vilket gör att samma bank profil kan tilldelas över flera MPN-ID: n och program inom en organisation. I de flesta fall kan du antingen återanvända en befintlig profil eller skapa en ny.

Det kan dock finnas undantag när du använder din bankprofil för olika länder eller regioner eftersom lokala bank- eller skatteregler kan gälla.

Skatte profiler som skapats för en MPN plats får återanvändas och fylls i automatiskt när samma MPN-plats ingår i ett annat program. Men det kan finnas undantag. Utbetalningsreglerna för ett nytt incitamentprogram kan till exempel kräva ytterligare information om skatteprofilen.

#### <a name="can-i-use-the-same-bank-and-tax-details-for-all-incentive-programs-at-microsoft"></a>Kan jag använda samma bank-och skatte information för alla stimulans program på Microsoft?

Om ditt företag är inbjudet till flera program kan du använda samma betalnings konto för alla dina program, eller så kan du välja att ha olika betalnings konton för olika program.


#### <a name="how-does-microsoft-ensure-that-the-bank-information-is-indeed-that-of-the-company-and-not-a-personal-bank-account-for-an-employee"></a>Hur ser Microsoft till att bank informationen verkligen är företagets och inte ett personligt bank konto för en medarbetare?

Det är företagets ansvar att se till att rollen som incitaments administratör, som har behörighet att redigera den här informationen, endast får lämpliga anställda.

#### <a name="my-tax-profile-has-expired-how-do-i-fix-this"></a>Min moms profil har upphört att gälla. Hur gör jag för att åtgärda detta?

Använd stegen i [skapa eller uppdatera din moms profil](set-up-your-payout-account.md#create-or-update-your-tax-profile) för att uppdatera din avgifts profil. På sidan **skatte profil** kan du se profiler som har upphört att gälla eller som upphör att gälla i kolumnen **förfallo datum** . 

## <a name="earnings-incorrect-or-missing"></a>Inkomsten är felaktig eller saknas

#### <a name="why-are-my-earnings-missing"></a>Varför saknas min intäkt?

- Kundordern kanske inte är berättigad till utbetalning ännu. För icke-företagskunders beställningar måste Microsoft ta emot kundbetalningar innan utgivaren blir berättigad. För företagskunders beställningar är dina intäkter tillgängliga 1–2 dagar efter inköpsorderdatumet. Verifiera orderstatus i [orderrapporter](https://partner.microsoft.com/dashboard/commercial-marketplace/analytics/order).
- Intäkter från transaktioner före juli 2019 kanske inte visas i rapporten för transaktionshistorik. Läs tidigare utdrag i [Payout Download](https://partner.microsoft.com/dashboard/payouts/reports/incentiveexport) (Ladda ned utbetalning).
- Kontrol lera [tids ramen för utbetalnings cykeln](payment-thresholds-methods-timeframes.md) och förstå när dina intäkter bör visas i utbetalnings instruktionen.

#### <a name="why-is-my-earnings-amount-different-than-what-i-expected"></a>Varför är min intäkts mängd annorlunda än vad jag förväntade mig?

- Om ordern delvis betalades av din kund baseras ditt belopp på det delvis betalda beloppet efter avdrag av avgift och lämplig skatt.
- Kontrol lera ansvars skatte ansvars per land. I de länder där skatten är Microsoft-ansvarig samlar Microsoft in och drar av skatten från utgivarintäkterna. Transaktionsbeloppet som visas i utdraget är efter skattebeloppet. Se [Skatteinformation](tax-details-marketplace.md).
- SaaS och IaaS erbjuder en rabatt byrå avgift på 10% i stället för standard 20%, vilket lämnar en inkomst avgift på 90%. Erbjudandet gäller fram till den 30 juni 2021.

**Mer läsning**: [publicerings avtal för handels Marketplace](https://go.microsoft.com/fwlink/p/?LinkID=699560), [utbetalnings princip information](payout-policy-details.md), [betalnings tröskel, metod](payment-thresholds-methods-timeframes.md)och [](marketplace-get-paid.md)tidsram, betalning, [skatte information](tax-details-marketplace.md), [utbetalnings instruktioner](payout-statement.md)

## <a name="earnings-reconciliation"></a>Intäktsavstämning

### <a name="how-do-i-reconcile-payout-statements-to-order-or-usage-reports-in-analytics"></a>Hur gör jag för att stämma av utbetalningsutdrag till order- eller användningsrapporter i Analytics?
Använd AssetID, Ordernr och rad objekt-ID som visas i historik rapporten för utbetalnings transaktioner med analytiska beställningar och användnings rapporter. Använd den här mappningen:

- Transaktionshistorik för utbetalning. History.AssetID = order.OrderID
- Payout Transaction History.OrderID & LineItem = Usage.UsageReferenceID [OrderID:LineItemID]

### <a name="how-do-i-know-when-to-expect-payments-for-my-customer-orders"></a>Hur vet jag när jag ska förvänta mig betalning för mina kundbeställningar?
- Börja med att använda din assetID, kontrol lera kund order i [order rapporter](https://partner.microsoft.com/dashboard/commercial-marketplace/analytics/order).
- Kontrol lera kund kanalen för kund prenumerationen i [kunders rapport](https://partner.microsoft.com/dashboard/commercial-marketplace/analytics/customer).
- För företags kunder visas utgivar intäkterna i utdraget 1-2 dagar efter inköps order datumet.
- För icke-företags kunder visas utbetalningar i utdraget 1-2 dagar efter att kund betalningen mottagits.

**Mer läsning**: [utbetalnings instruktioner](payout-statement.md), [order instrument panel i kommersiell Marketplace-analys](/azure/marketplace/partner-center-portal/orders-dashboard)

## <a name="payments-and-adjustments"></a>Betalningar och justeringar

#### <a name="why-is-my-payment-missing"></a>Varför saknas min betalning?

- Se till att din utbetalnings status och skatte profils status visas som *giltig* på [översikts sidan](https://partner.microsoft.com/dashboard/commercial-marketplace/overview).
- Du kanske inte har uppnått minimitröskelvärdet för en betalning. Intäkterna måste vara minst $50 USD för att du ska få en betalning.


#### <a name="how-do-i-set-my-account-to-not-receive-payment"></a>Vill du Hur gör jag för att ange att mitt konto inte ska ta emot betalning?
Du kan lagra betalningar i [utbetalnings profil](https://partner.microsoft.com/dashboard/commercial-marketplace/overview). kontrol lera bara **Håll**. Microsoft kommer att betala till dig tills du släpper upp spärren.

#### <a name="why-do-i-receive-in-a-different-currency-than-the-purchase-currency"></a>Varför får jag betalningar i en annan valuta än inköpsvalutan?

Utbetalningsvalutan baseras på den valuta som du valde i utbetalningsprofilen. Inköpsvalutan baseras på den valuta som kunden betalade i.

#### <a name="how-do-i-reconcile-adjustments"></a>Hur gör jag för att stämma av justeringar?

Betalningsjusteringar är betalningskorrigeringar för att hantera kompensationsjusteringar, till exempel systemproblem. I utbetalningsutdraget anges orsaken till justeringen av ReasonCode. Dessa är inte avsedda för avstämning direkt till enskilda transaktioner.

**Mer läsning**: [publicerings avtal för handels Marketplace](https://go.microsoft.com/fwlink/p/?LinkID=699560), [utbetalnings princip information](payout-policy-details.md), [skatte information](tax-details-marketplace.md), [betalnings tröskel, metod och tidsram](payment-thresholds-methods-timeframes.md)

## <a name="taxes"></a>Skatter

#### <a name="how-do-we-identify-tax-remit-responsibility-between-microsoft-or-publisher-in-the-payout-statement"></a>Hur identifierar vi ansvaret för skatteinbetalning mellan Microsoft och utgivaren i utbetalningsutdraget?

Leta reda på kolumnen Skattemodell i den nedladdade transaktionshistoriken. Där står det MS Managed (Hanteras av MS) eller ISV Managed (Hanteras av ISV). Se de landsspecifika skattereglerna och utbetalningseffekter i [Skatteinformation](tax-details-marketplace.md).

#### <a name="how-do-i-download-service-fee-tax-forms"></a>Hur gör jag för att hämta skatteformulär för serviceavgifter?

Gå till sidan **Payout Payment** (Utbetalning) och sedan till avsnittet **List of Payment** (Lista över betalningar). En länk till skatteformuläret för serviceavgifter för en betalning som har serviceavgifter/skatt.

#### <a name="how-do-i-download-a-withholding-tax-form-in-pdf"></a>Hur gör jag för att ladda ned ett källskatteformulär i PDF-format?

Gå till sidan *Payout Payment* (Utbetalning) och sedan till avsnittet **List of Payment** (Lista över betalningar). En länk till ett källskatteformulär visas bredvid en betalning.

#### <a name="where-do-i-find-year-end-tax-forms"></a>Var hittar jag skatteblanketter för slutet av beskattningsåret?

Gå till [profilsidan](https://partner.microsoft.com/dashboard/payee/profiles/partner/manage) för att visa dina skatteblanketter för slutet av beskattningsåret.

#### <a name="how-do-i-find-withholding-tax-for-a-transaction"></a>Hur hittar jag källskatten för en transaktion?
Källskatt gäller för amerikanska utgivare som har skickat in ett W-9-formulär. Källskatt beräknas för en månatlig betalning.

**Mer läsning**: [publicerings avtal för handels Marketplace](https://go.microsoft.com/fwlink/p/?LinkID=699560), [utbetalnings princip information](payout-policy-details.md)

## <a name="payout-statement-access"></a>Åtkomst till utbetalnings instruktion

#### <a name="how-do-i-access-a-payout-statement"></a>Hur får jag åtkomst till ett utbetalningsutdrag?

1. Kontrollera dina roller. Du måste ha rollen *finansiell bidragsgivare* eller *kontoägare* för att få åtkomst till utbetalningsutdrag.
2. I det övre högra navigerings fönstret väljer du **utbetalnings** ikonen för att Visa utbetalnings instruktionen. Välj mellan **transaktions historik**, **betalning** och **hämtning**.

**Mer läsning**: [utbetalnings roller och behörigheter](payout-statement.md#roles-and-permissions), [utbetalnings instruktioner](payout-statement.md) 

## <a name="payout-statement-report"></a>Rapporten utbetalnings instruktion

#### <a name="what-does-each-field-in-the-transaction-download-mean"></a>Vad betyder varje fält i transaktionsnedladdningen?

Se [utbetalnings uttryck](payout-statement.md) för en detaljerad lista över attributen och deras betydelser.

#### <a name="what-is-earning-status"></a>Vad är intäktsstatus?

Detta visar dina intäkter som antingen obearbetade, behandlade eller skickade.

- **Obearbetad** – intäkterna är under en depositions period till förfallo datumet.
- **Bearbetad** – intäkterna har förberetts och är fördelade i en månads betalning. Betalningar frigörs med 15 i varje månad.
- **Skickat** – betalningen har frigjorts till din bank baserat på din utbetalnings profil.

#### <a name="how-do-i-download-service-fee-tax-forms"></a>Hur gör jag för att hämta skatteformulär för serviceavgifter?

Gå till sidan **Payout Payment** (Utbetalning) och sedan till avsnittet **List of Payment** (Lista över betalningar). En länk till skatteformuläret för serviceavgifter för en betalning som har serviceavgifter/skatt.

#### <a name="how-do-i-download-a-withholding-tax-form-in-pdf"></a>Hur gör jag för att ladda ned ett käll skatte formulär i PDF-filen?

Gå till sidan **Payout Payment** (Utbetalning) och sedan till avsnittet **List of Payment** (Lista över betalningar). En länk till ett källskatteformulär visas bredvid en betalning.

#### <a name="where-do-i-find-year-end-tax-forms"></a>Var hittar jag skatteblanketter för slutet av beskattningsåret?

Gå till [profilsidan](https://partner.microsoft.com/dashboard/payee/profiles/partner/manage) för att visa dina skatteblanketter för slutet av beskattningsåret.

**Mer läsning**: [utbetalnings instruktioner](payout-statement.md), [hämtning av transaktions historik](payout-statement.md#transaction-history-download)

## <a name="historical-statements"></a>Historiska instruktioner

#### <a name="how-do-i-view-historical-information"></a>Hur gör jag för att du Visa historisk information?

Historiskt utdrag visar en ögonblicksbild av utbetalningsdata från oktober 2019. Tyvärr uppdateras inte utbetalnings informationen här. För att få den senaste informationen skickar du ett support ärende för den senaste informationen.

**Mer läsning**: [utbetalnings instruktioner](payout-statement.md), [hämtning av transaktions historik](payout-statement.md#transaction-history-download)

## <a name="payout-export-api"></a>Export-API för inbetalning

#### <a name="how-do-i-download-payout-data"></a>Hur gör jag för att ladda ned utbetalningsdata?

Använd [API för partner utbetalning](https://apidocs.microsoft.com/services/partnerpayouts).

## <a name="commercial-marketplace-payout-policies"></a>Principer för utbetalning av kommersiella marknads platser

#### <a name="how-do-i-find-the-current-agency-fee-and-the-payout-rate"></a>Hur gör jag för att hitta aktuellt arvode och utbetalningsfrekvens?

- Kontrollera utgivaravtalet för kommersiell marknadsplats. Standardarvodet är 20 %. SaaS Co-Sell berättigade transaktioner har en rabatterad avgift på 10%. Sök efter meddelanden om arvoden för PR-byråer.
- I din utbetalnings instruktion anger kostnaden den faktiska utbetalnings takten för en specifik transaktion.

#### <a name="when-can-i-expect-a-payment-from-microsoft-once-earnings-appear-on-my-statement"></a>När kan jag vänta mig en betalning från Microsoft när intäkterna visas i mitt utdrag?
- När dina intäkter har status obearbetad kan du kontrollera förfallodatum för den månad då dina intäkter bearbetas för betalning. När din betalning har förberetts ändras din beställnings status till "bearbetad".  Microsoft släpper betalningar den 15:e i förfallomånaden.
- För beställningar som betalas av kredit kortet, innehåller Microsoft betalningar 30 dagar tills betalningen har förfallit.

 **Mer läsning**: [publicerings avtal för handels Marketplace](https://go.microsoft.com/fwlink/p/?LinkID=699560), [utbetalnings princip information](payout-policy-details.md), [skatte information](tax-details-marketplace.md), [betalnings tröskel, metod och tidsram](payment-thresholds-methods-timeframes.md)

## <a name="next-steps"></a>Nästa steg

- [Få betalt](marketplace-get-paid.md)
- [Konfigurera utbetalningskonto och deklarationsblanketter](set-up-your-payout-account.md)
