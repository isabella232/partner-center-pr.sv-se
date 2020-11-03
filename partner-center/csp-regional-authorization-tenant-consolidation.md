---
title: CSP regional auktorisering av klient konsolidering
ms.topic: how-to
ms.date: 07/15/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Använd de här anvisningarna för att konsolidera klienter för olika länder/regioner. Detta inkluderar steg för att migrera kund konton och kund prenumerationer.
author: billLinzbach
ms.author: billLi
ms.localizationpriority: medium
robots: noindex,nofollow
ms.custom: SEOMAY.20
ms.openlocfilehash: 0ae107c005eaf6b8ff8a6d99a91075ebc560cf81
ms.sourcegitcommit: 940dad4527f51781f6f966e196b3aa08389613a2
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 10/13/2020
ms.locfileid: "92531853"
---
# <a name="instructions-for-csp-regional-authorization-tenant-consolidation"></a>Instruktioner för CSP regional auktorisering av klient organisations konsolidering

**Gäller för**

-  Partnercenter
-  Partner Center för Microsoft Cloud för amerikanska myndigheter

**Lämpliga roller**

- Global administratör
- Administratörs agent

\[Viss information relaterar till en för hands fri produkt som kan ändras avsevärt innan den släpps kommersiellt. Microsoft lämnar inga garantier, uttryckliga eller underförstådda, avseende informationen som visas här.\]

Du kan konsolidera klienter för ditt företag. Använd de här anvisningarna för att konsolidera klienter för olika länder/regioner.

>[!NOTE]  
>Du måste vara medveten om alla etablerade prenumerationer och licens antal för var och en av dina kunder i kontot som du övergår från. Du kommer att etablera om samma exakta prenumerationer med samma licens antal under det nya centrala CSP-kontot som en del av migreringsprocessen. Använd funktionen Exportera lista för att skapa en lista över kunder att gå över till den centraliserade klienten.  När konsolideringen är klar kan du inte återgå till det tidigare klient organisations läget. Det kan också krävas en kund åtgärd.

## <a name="prepare-for-migration"></a>Förbereda för migrering

- Logga in på **partner Center**  med hjälp av kontot för **över gång** (det som du kommer att övergå till det nya kontot) och granska alla kunder och alla tjänster som tillhandahålls för dessa kunder.

- Logga ut från det här kontot.

## <a name="migrate-customer-accounts"></a>Migrera kund konton

1. Logga in på **partner Center** **med det nya kontot (det** som du använder för att överföra kunder till).

2. Välj **Kunder** .

3. Klicka på **begär en åter försäljare relation** . Du får ett e-postmeddelande som standard för att skicka till dina kunder. Det här meddelandet innehåller en URL med det org-ID som är unikt för ditt nya partner Center-konto.

4. **Kund åtgärd:** Se till att alla aktiva kunder som du vill migrera besöker den här URL: en. När du öppnar webb adressen uppmanas kunden att logga in på Office 365-portalen. Kunden loggar in med samma organisations-ID som de använder för att få åtkomst till Azure-och Office 365-administrations portalerna.

5. När du har loggat in uppmanas den globala administratören för **kund kontot** att skicka ett avtal som ger delegerad administratörs behörighet till det nya CSP-kontot. Om de samtycker väljer kunden kryss rutan och accepterar att auktorisera relationen.

Kunderna kommer att visas i partnerns kund lista när de har skickat in avtalet, ett i taget.

## <a name="migrating-office-365-and-non-azure-usage-based-subscriptions"></a>Migrera Office 365 och användnings prenumerationer som inte använder Azure

1. När din kund har undertecknat avtalet kan du återskapa deras prenumerationer under din centraliserade partner klient.

2. Välj **kunder** från **partner Center** .

3. Öppna företags namnet för den kund som du vill migrera.

4. Välj **Lägg till prenumeration** .

5. Lägg till rätt prenumerationer och licens antal från katalogen. Kontrol lera med den information som finns i **över gången från** partner konton.

   :::image type="content" source="images/regionalcustomer2.png" alt-text="kund lista":::

6. Klicka på **Skicka.**

   Tjänsterna tillhandahålls nu till kunden från **över gången till** partner kontot.

7. Upprepa de här stegen för att migrera prenumerationer för alla ytterligare kunder.

Innan du fortsätter till nästa avsnitt bör du se till att alla kund prenumerationer som finns under **över gången från** partner konton etableras på nytt under **över gången till** partner kontot.

> [!NOTE]
> Partners måste pausa prenumerationer på **över gången från** partner klient kontot i Partner Center samma dag som prenumerationerna övergår till och konfigureras under **över gången till** partner klient kontot i partner centret för att säkerställa att dubbel fakturering inte sker. Support förfrågningar kommer att nekas för krediter på grund av eventuella överlappningar i faktureringen som sker från att inte inaktivera **över gången från** prenumerationer.

## <a name="disabling-the-office-365-subscriptions-under-the-transitioning-from-partner-account"></a>Inaktiverar Office 365-prenumerationer under över gång från partner konto

Om du inaktiverar CSP-prenumerationen under **över gången från** partner konton avbryts eventuell framtida fakturering. Du behöver inte inaktivera Azure-prenumerationer manuellt, eftersom Azure-prenumerationer inaktive ras automatiskt under migreringsprocessen.

1. Logga in på **partner Center** med **över gång från** CSP-konto och navigera till kund listan.

2. Öppna kunden med prenumerationer som du vill inaktivera och välj sedan det första erbjudandet som ska inaktive ras.

3. Ställ in prenumerationen på **pausad** och klicka sedan på **Skicka** .

   >[!Note]
   >Om du avbryter prenumerationen säkerställs dubbel fakturering.

   Prenumerationen visar **inaktive** rad i prenumerations listan.

4. Upprepa de här stegen för alla prenumerationer under kunden. Kontrol lera att alla visas **inaktiverade.**

5. Välj nästa kund i listan och upprepa processen för att inaktivera alla prenumerationer.

## <a name="migrating-azure-usage-based-subscriptions"></a>Migrera Azure Usage-baserade prenumerationer

Till skillnad från Office 365 CSP-prenumerationer behöver Azure, användnings CSP-prenumerationer inte migreras manuellt. Microsoft Azure-support migrerar Azure-prenumerationerna samt alla distribuerade tjänster eller resurser från **över gången från** CSP: er åter försäljar konton till kontot för **över gång till** CSP-återförsäljare. Det sker ingen avbrott i tjänsten för kunden under över gången.

1. Se till att de kund konton som kommer att ha Azure-prenumerationer migrerats har godkänt att avtalet associeras med den nya **över gången till** CSP-kontot.

2. Du kommer att meddela Microsoft om vilka kund konton som är redo att migrera och ange kundens företags namn.

3. Microsoft migrerar Azure Usage-baserade prenumerationer och meddelar dig när migreringen är klar.

4. Du måste bekräfta att Azure-prenumerationen under **över gången från** CSP Reporting-kontot nu har marker ATS som **inaktive** rad i Partner Center i avsnittet kund prenumerationer.

5. Bekräfta att Azure-prenumerationen under **över gången till** CSP Reporting-kontot nu visar statusen **aktiv** i Partner Center i avsnittet kund prenumerationer.

   >[!Note]
   > Om du inaktiverar prenumerationerna under kunden ändras inte utseendet på kunden i listan kunder. Det finns för närvarande inget alternativ att ta bort kunder från listan. Partner bör undvika att lägga till prenumerationer till dessa kunder från deras **över gång från** konto i framtiden.

6. Upprepa de här stegen för alla prenumerationer under alla kunder för att stoppa framtida avgifter på **över gången från** konton. Partnern får en sista faktura med en kredit för antalet oanvända dagar mellan dagen för annullering och den sista dagen i fakturerings perioden. Inga framtida fakturor skapas efter den sista fakturerings perioden.

### <a name="additional-information"></a>Ytterligare information

- Inaktive ring av prenumerationen från **över gång från** CSP-konto påverkar inte den slutliga kundens tjänst så länge tjänsten etablerades från **över gången till** CSP-konto innan prenumerationen inaktiverades.

- Prenumerationer kan inte användas av kunden och genererar inga kostnader när de pausas eller avbryts.

- Det finns för närvarande inget sätt att ta bort en kund helt från listan **kunder** .
- 
    >[!Note]
    > Partners måste pausa prenumerationer på **över gången från** partner klient kontot i Partner Center samma dag som dessa prenumerationer överförs till och konfigureras under **över gången till** konto för att säkerställa dubbel fakturering. Microsoft stöder inte förfrågningar om krediter på grund av eventuella överlappningar i faktureringen som sker från att inte ställa in **över gången från** prenumerationer till pausad.

### <a name="simplify-migration-using-export"></a>Förenkla migreringen med hjälp av export

Med hjälp av **funktionen Exportera** kan du samla in de prenumerationer som du behöver använda i din nya konsoliderade struktur:

1. Klicka på **kunder** i Partner Center för att se listan över kunder. 

2. Öppna det önskade kund namnet.

3. På sidan **prenumerationer** klickar du på **Exportera prenumerationer** för att exportera information om prenumerationer till en Excel-fil.

4. Använd den här listan för att återskapa prenumerationerna i den nya konsoliderade klienten.

### <a name="api-registration"></a>API-registrering

Mer information om API-registrering finns i [Konfigurera API-åtkomst i Partner Center](/partner-center/develop/set-up-api-access-in-partner-center).

## <a name="next-steps"></a>Nästa steg

- [Cloud Solution Provider program regionala marknader och valutor där du kan sälja CSP-erbjudanden](regional-authorization-overview.md)
