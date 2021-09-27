---
title: CSP regional auktorisering klientkonsolidering
ms.topic: how-to
ms.date: 09/27/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-membership
description: Använd de här instruktionerna för att konsolidera klienter för olika länder/regioner. Detta omfattar steg för att migrera kundkonton och kundprenumerationer.
author: billLinzbach
ms.author: billLi
ms.localizationpriority: medium
robots: noindex,nofollow
ms.custom: SEOMAY.20
ms.openlocfilehash: 1500525e49fd2585cd97cd4cf7999cba63ac9f30
ms.sourcegitcommit: d731813da1d31519dc2dc583d17899e5cf4ec1b2
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/27/2021
ms.locfileid: "129072337"
---
# <a name="instructions-for-csp-regional-authorization-tenant-consolidation"></a>Instruktioner för CSP-auktorisering för konsolidering av klientorganisationer

**Gäller för**: Partner Center-| Partnercenter för Microsoft Cloud for US Government

**Lämpliga roller:** Global | Administratörsagent

\[En del information gäller för frisläppt produkt som kan ändras avsevärt innan den släpps kommersiellt. Microsoft lämnar inga garantier, uttryckliga eller underförstådda, avseende informationen som visas här.\]

Du kan konsolidera klienter för din verksamhet. Använd de här instruktionerna för att konsolidera klienter för olika länder/regioner.

>[!NOTE]  
>Du måste vara medveten om alla etablerade prenumerationer och licensantal för var och en av dina kunder i det konto som du övergår från. Du kommer att ometablering av samma exakta prenumerationer med samma licensantal under det nya centrala CSP-kontot som en del av migreringsprocessen. Använd exportlistefunktionen för att skapa en lista över kunder som ska flyttas över till den centraliserade klientorganisationen.  När konsolideringen är klar kan du inte återgå till det tidigare klienttillståndet. Kundåtgärd kan också krävas.

## <a name="prepare-for-migration"></a>Förbereda för migrering

- Logga in på **Partnercenter** med övergångskontot (det som du kommer att övergå till det nya kontot) och granska alla kunder och alla tjänster som etablerats för dessa kunder. 

- Logga ut från det här kontot.

## <a name="migrate-customer-accounts"></a>Migrera kundkonton

1. Logga in på **Partnercenter**  med **övergångskontot** (nytt) (det som du övergår kunder till).

2. Välj **panelen** Kunder.

3. Välj **Begär en återförsäljarrelation**. Du får ett standardmeddelande som du kan skicka till dina kunder. Det här meddelandet innehåller en URL med organisations-ID:t som är unikt för ditt nya Partnercenter-konto.

4. **Kundåtgärd:** Se till att var och en av de aktiva kunder som du vill migrera besöker denna URL. När du öppnar URL:en uppmanas kunden att logga in på Office 365 portalen. Kunden loggar in med samma organisations-ID som de använder för att komma åt Azure och Office 365-administratörsportalerna.

5. När du har loggat  in uppmanas den globala administratören för kundkontot att skicka ett avtal som ger delegerade administratörsbehörigheter till det nya CSP-kontot. Om kunden accepterar markerar kunden kryssrutan och godkänner att relationen godkänns.

Kunderna visas i partnerns kundlista när de har skickat avtalet, en i rad.

## <a name="migrating-office-365-and-non-azure-usage-based-subscriptions"></a>Migrera Office 365 och icke-Azure-användningsbaserade prenumerationer

1. När kunden har signerat avtalet kan du återskapa deras prenumerationer under din centraliserade partnerklientorganisation.

2. Från **Partnercenter** väljer du **Kunder.**

3. Öppna företagsnamnet för den kund som du vill migrera.

4. Välj **Lägg till prenumeration.**

5. Lägg till rätt prenumerationer och licensantal från katalogen. Kontrollera med informationen som anges i **Övergång från** partnerkonton.

   :::image type="content" source="images/regionalcustomer2.png" alt-text="kundlista.":::

6. Välj **Skicka.**

   Tjänsterna tillhandahålls nu till kunden från **övergångskontot till** partnerkontot.

7. Upprepa dessa steg för att migrera prenumerationer för alla ytterligare kunder.

Innan du fortsätter till nästa avsnitt ser du till att alla kundprenumerationer som finns under Övergångs från **partnerkonton** etableras på nytt under **övergångskontot till** partnerkontot.

> [!NOTE]
> Partner måste inaktivera  prenumerationer på kontot för övergång från partnerklientorganisation i Partnercenter samma dag som prenumerationerna övergår och konfigureras under kontot för övergång till **partnerklientorganisation** i Partnercenter för att säkerställa att dubbel fakturering inte sker. Supportbegäranden nekas för krediter på grund av eventuell överlappning i faktureringen som inträffar när övergången från prenumerationer **inaktiveras** korrekt.

## <a name="disabling-the-office-365-subscriptions-under-the-transitioning-from-partner-account"></a>Inaktivera Office 365 prenumerationer under övergångskontot från partner

Om du inaktiverar CSP-prenumerationen under **övergången från** partnerkonton stoppas eventuell framtida fakturering. Du behöver inte inaktivera Azure-prenumerationer manuellt eftersom Azure-prenumerationer inaktiveras automatiskt under migreringsprocessen.

1. Logga in på **Partnercenter med** **övergångskontot från** CSP och gå till kundlistan.

2. Öppna kunden med prenumerationer att inaktivera och välj sedan det första erbjudandet att inaktivera.

3. Ställ in prenumerationen **på pausad** och välj **sedan Skicka**.

   >[!Note]
   >Om du pausar prenumerationen säkerställer du att dubbel fakturering inte sker.

   Prenumerationen visas **som inaktiverad** i prenumerationslistan.

4. Upprepa dessa steg för alla prenumerationer under kunden. Kontrollera att alla visas som **pausade.**

5. Välj nästa kund i listan och upprepa processen för att inaktivera alla prenumerationer.

## <a name="migrating-azure-usage-based-subscriptions"></a>Migrera azure-användningsbaserade prenumerationer

Till skillnad Office 365 CSP-prenumerationer behöver azure-baserade CSP-prenumerationer inte migreras manuellt. Microsoft Azure Supporten migrerar Azure-prenumerationerna och alla  distribuerade tjänster eller resurser från övergångskontot från CSP-återförsäljare till kontot för övergång **till** CSP-återförsäljare. Det kommer inte att ske några avbrott i tjänsten för kunden under den här övergången.

1. Se till att de kundkonton som kommer att ha Azure-prenumerationer migrerade har godkänt avtalet för att associeras med det nya **övergångskontot till** CSP.

2. Du meddelar Microsoft vilka kundkonton som är redo att migreras och anger kundens företagsnamn.

3. Microsoft migrerar azure-användningsbaserade prenumerationer och meddelar dig när migreringen är klar.

4. Du måste bekräfta att Azure-prenumerationen under kontot för övergång  från  CSP-återförsäljare nu har markerats som inaktiverat i Partnercenter under avsnittet kundprenumerationer.

5. Bekräfta att Azure-prenumerationen under **kontot för övergång** till  CSP-återförsäljare nu visar statusen aktiv i Partnercenter under avsnittet kundprenumerationer.

   >[!Note]
   > Om du inaktiverar prenumerationerna under kunden ändras inte utseendet på kunden i kundlistan. Det finns för närvarande inget alternativ för att ta bort kunder från listan. Partner bör undvika att lägga till prenumerationer till dessa kunder från **övergången från** konto i framtiden.

6. Upprepa de här stegen för alla prenumerationer under alla dina kunder för att stoppa framtida avgifter för **övergång från** konto. Partnern får en slutlig faktura med en kredit för antalet oanvända dagar mellan annulleringsdagen och den sista dagen i faktureringsperioden. Inga framtida fakturor genereras efter den sista faktureringsperioden.

### <a name="additional-information"></a>Ytterligare information

- Om du inaktiverar prenumerationen från kontot för övergång från **CSP** påverkas inte slutanvändarens tjänst så länge tjänsten etablerades från övergångskontot till **CSP** innan prenumerationen inaktiverades.

- Prenumerationer kan inte användas av kunden och genererar inte avgifter när de pausas eller avbryts.

- Det finns för närvarande inget sätt att ta bort en kund helt från **kundlistan.**
- 
    >[!Note]
    > Partner måste inaktivera prenumerationer på kontot för övergång från **partnerklientorganisation** i Partnercenter samma  dag som prenumerationerna övergår till och konfigureras under övergångskontot för att säkerställa att dubbel fakturering inte sker. Microsoft kommer inte att stödja begäranden om krediter på grund av överlappande fakturering som inträffar från att inte korrekt ställa in övergången **från** prenumerationer till pausad.

### <a name="simplify-migration-using-export"></a>Förenkla migrering med export

Med hjälp **av exportfunktionen** kan du avbilda de prenumerationer som du behöver använda i din nya konsoliderade struktur:

1. Välj **Kunder** i Partnercenter för att se listan över kunder. 

2. Öppna önskat kundnamn.

3. På sidan **Prenumerationer väljer** du Exportera **prenumerationer för** att exportera information om prenumerationer till en Excel fil.

4. Använd den här listan för att återskapa prenumerationerna i din nya konsoliderade klientorganisation.

### <a name="api-registration"></a>API-registrering

Mer information om API-registrering finns i [Konfigurera API-åtkomst i Partnercenter.](/partner-center/develop/set-up-api-access-in-partner-center)

## <a name="next-steps"></a>Nästa steg

- [Molnlösningsleverantör program regionala marknader och valutor där du kan sälja CSP-erbjudanden](regional-authorization-overview.md)
