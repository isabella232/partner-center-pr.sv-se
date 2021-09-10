---
title: Massexport och import av möjligheter till säljförsäljning via Excel-/CSV-filer i referenser
description: Lär dig hur du laddar ned, skapar eller uppdaterar möjligheter till säljförsäljning med hjälp av Excel (CSV)-filer i Partnercenter
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-referrals
author: vikramb
ms.author: vikramb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 02/03/2021
ms.openlocfilehash: 58443589d4a90b59783f84a12a920d725f74ffbc
ms.sourcegitcommit: 1161d5bcb345e368348c535a7211f0d353c5a471
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/09/2021
ms.locfileid: "123960273"
---
# <a name="bulk-operations-for-co-sell-opportunities-using-comma-separated-value-csv-files"></a>Massåtgärder för möjligheter till säljförsäljning med hjälp av filer med kommaavgränsade värden (CSV)

**Lämpliga roller:** Referensadministratörsroller | Referensanvändare

Med hjälp av massåtgärder i Partnercenter kan ditt företag exportera och importera data för säljsamarbetesmöjligheter. Gå till sidan för **säljsamarbete** för att hitta länkarna för **import** och **export** längst upp till höger på banderollen för sidrubriken. Användare med behörighet som både **referensadministratör** och **referensanvändare** kan använda den här funktionen.

> [!IMPORTANT]
> Åtgärderna för att skapa/uppdatera som utförs via massimport kan inte ångras. Var försiktig när du ändrar eller skapar ett stort antal poster. Endast en delmängd av fälten kan ändras när du har skapat ett avtal. **Inga åtgärder tillåts när ett avtal når ett slutgiltigt tillstånd som Nekat/Upphört/Vunnet/Förlorat.**

## <a name="export-co-sell-opportunities"></a>Exportera möjligheter till säljsamarbete

Följande information beskriver exportfunktionen:

- Du kan exportera högst **5 000 poster genom** att klicka på **exportknappen.**
- De avtal som laddas ned baseras på dina åtkomstnivåer. Referensadministratörer och hänvisningsanvändare kan få olika resultat baserat på deras omfattning och inkludering som gruppmedlemmar i avtal. Läs mer om [referensbehörigheter.](permissions-overview.md#manage-referrals)
- Exportfunktionen tar hänsyn till den aktuella fliken på sidan möjligheter till säljförsäljning och de filter som har tillämpats.
- En CSV-fil med alla data baserat på tillämpade filter genereras.
- Det kan ta upp till en minut att ladda ned posterna.
- Du behöver inte vänta tills nedladdningsåtgärden har slutförts. Även om du navigerar till andra sidor i Partnercenter hämtas filen så fort exportfunktionen har slutförts.
- Du kan återanvända den nedladdade filen för att ändra avtalsinformationen och ladda upp för att uppdatera alla poster.

## <a name="import-co-sell-opportunities"></a>Importera möjligheter till säljsamarbete

- Du kan skapa eller uppdatera högst **1 000 poster med** importfunktionen.
- Du kan skapa mallen från grunden genom att ladda ned mallen från sidan Importera i Partnercenter.
- Du kan också använda exportfunktionen för att ladda ned befintliga poster och uppdatera dem.
- Om filen har fler än 1 000 poster kan den inte bearbetas.
- När filen har bearbetats visas en sammanfattning med antalet referenser som har skapats, uppdaterats och inte bearbetats i det senaste processfilkortet.
- Du kan ladda ned information om bearbetade poster, åtgärda eventuella fel och ladda upp samma fil för att skapa eller uppdatera posterna som misslyckades i föregående körning. **Ta bort alla lyckade poster från filen innan du laddar upp de korrigerade posterna som misslyckades i föregående körning.**
- Om du vill lägga till fler lösningar lägger du till extra kolumner bredvid lösning 1 och använder kolumnnamnet som Lösning X, där X representerar numret på lösningen i avtalet. Till exempel Lösning 2, Lösning 3.
- Du kan lägga till upp till 50 lösningar i ett avtal.
- Om du vill lägga till fler gruppmedlemmar lägger du till extra kolumner bredvid Teammedlem 1 och använder kolumnnamnet som Teammedlem X, där X representerar antalet teammedlemmen i avtalet. Till exempel Teammedlem 2, Teammedlem 3.
- Du kan lägga till upp till 50 teammedlemmar i ett avtal.

> [!NOTE]
> Du behöver inte vänta tills bearbetningen har slutförts. Information om den senast bearbetade filen blir tillgänglig för nedladdning när bearbetningen är klar. **Det kan ta upp till 10 minuter om du laddar upp filer med 1 000 poster.**

> [!IMPORTANT]
> Läs alla instruktioner noggrant och kontrollera formatet för varje kolumn i tabellen nedan innan du skapar eller uppdaterar avtal med hjälp av CSV-filer i Partnercenter.

|**Kolumnnamn**|**Är obligatoriskt?**|**Beskrivning**|**Exempelvärden**|
|-----|:-----|:---------|:---|
Fel|No|Fel om några relaterade till åtgärderna för att skapa/uppdatera w.r.t till hänvisningarna tas med i den här kolumnen. Om det finns flera fel visas alla avgränsade med semikolon.|Obligatoriskt fält Lösning 1 saknas|
Engagemangs-ID|No|Engagemangs-ID:t genereras av referenssystemet för Microsoft Partner Center. Krävs inte för att skapa en ny referens. Du kan använda det befintliga engagemangs-ID:t om du uppdaterar en post.|f7eaae47-0b84-4ac4-b4ea-5b2587d42cee
Hänvisningskod|No|Hänvisnings-ID genereras av referenssystemet för Microsoft Partner Center. Krävs inte för att skapa en ny referens. Fyll i det med hänvisnings-ID:t om du uppdaterar en befintlig post.|ebacdkdc-0b84-4ac4-b4ea-5b2587d42cee
Avtalsnamn|Yes|Det egna namnet för avtalet för din referens.|Storbritanniens våravtal
Kundnamn|Yes|Namnet på kundföretaget. Använd organisationens juridiska namn för snabb matchning på Microsoft-sidan.|Contoso Corporation
Kundadressrad 1|Yes|Adressrad 1 i kundföretaget. |One Contoso Way
Kundadress rad 2|No|Adressrad 2 på kundföretaget.|NE 148 street
Kundens stad|Yes|Ort där kundorganisationen finns.|Redmond
Kundtillstånd|No|Ange var kundorganisationen finns.|Washington
Kundens postnummer|No|Postnummer i den region där kundorganisationen finns.|98052
Kundland|Yes|Land/region där kundorganisationen finns. Använd landskoderna med två bokstäver som anges [här.]( https://en.wikipedia.org/wiki/List_of_ISO_3166_country_codes)|USA
Kundens D-U-N-S-ID|No|Försök att hämta KUNDORGANISATIONENS DUNS-ID. Detta hjälper till med snabbare matchning av kundorganisationen på Microsoft-sidan, vilket hjälper till att få snabbare säljtilldelning. Du kan få DUNS-ID kostnadsfritt från den här [webbplatsen.](https://www.dnb.com/duns-number/lookup.html)|81466849
Kundens kontakts förnamn|Beror|Förnamn är bara obligatoriskt om du behöver Hjälp från Microsoft. Förnamnet på den primära kontakten från kundorganisationen som arbetar med det här avtalet.|John
Kundens kontakts efternamn|Beror|Efternamn är bara obligatoriskt om du behöver Microsoft-hjälp. Efternamn på den primära kontakten från kundorganisationen som arbetar med det här avtalet.|Kund
Kundkontaktens Telefon nummer|Beror|Telefon är bara obligatoriskt om du behöver Hjälp från Microsoft. Telefon den primära kontakten från kundorganisationen som arbetar med det här avtalet.|9999999999
E-postadress för kundkontakt|Beror|E-postadress är bara obligatoriskt om du behöver Microsoft-hjälp. E-postadressen till den primära kontakten från kundorganisationen som arbetar med det här avtalet.|john.customer@contoso.com
Partnerreferensstatus|Yes|Visar avtalets status ur företagets perspektiv. Krävs om du försöker skapa eller ändra en referens. Använd **Ny** om du försöker skapa ett nytt avtal. Godkända värden dokumenteras [här.](/partner/develop/referral-resources#referralstatus)|Aktiv
Understatus för partnerreferens|Yes|Anger den exakta statusen för avtalet. Använd **Accepterad** om du försöker skapa ett nytt avtal. Det krävs också om du ändrar en befintlig referens. Godkända värden dokumenteras [här.](/partner/develop/referral-resources#referralsubstatus)|Har godkänts
Microsoft-hänvisningsstatus|Beror|Visar statusen för den begäran om säljförsäljning som du har skickat till Microsoft och som behöver hjälp. Det här är ett skrivskyddade fält. Ändringar som görs i det här fältet när du importerar data ignoreras.| Väntar
Nekad/förlorad orsak|Beror| Du måste bara ange den här informationen om du ändrar understatusen för fältet till antingen Nekad eller Förlorad. Annars kan du ignorera den här kolumnen. <br/> **Ange ett tal baserat på alternativen nedan** <br/><br/> **1**– Project budget inte är tillräcklig  <br/> **2**– Kunden svarade inte  <br/> **3**– Kunden valde en annan leverantör  <br/> **4** – Kundkrav uppfylls inte  <br/> **5** – Inte en kund <br/> **6**– Den föreslagna tidsraden var för kort <br/> **7** – Rapportera som missbruk, skräppost eller nätfiske <br/> **8** – Andra |6|
Försäljningsstadie|No|Det här är fältet för att ange den detaljerade försäljningsfasen för hänvisningen. Läs mer om försäljningsstadier [här](./manage-co-sell-opportunities.md)|40
Beräknat avtalsvärde|Yes|Avtalets värde baseras på de första konversationerna med kunden. Detta kan ändras tills avtalet når ett av de terminalstater som **vunnits eller** **förlorats.**|12563
Valuta|Yes|Den valuta som avtalsvärdet anges i. Valutakoderna finns [här.](https://en.wikipedia.org/wiki/ISO_4217)|USD
Beräknat stängningsdatum|Yes|Avtalets uppskattade slutdatum baserat på de första konversationerna med kunden i formatet MM/DD/Å ÅYYY. <br/> **Datumet ska vara i UTC-tidszonen. Alla datum som visas i partnercentrets användargränssnitt baseras på lokaliserade tidszoner. Det kan finnas +/- en dag i partnercentergränssnittet om du tittar på den hänvisning som du angav datumet för i UTC-tidszonen.**|1/30/2020
CRM-ID|No|Identifierare för den här specifika hänvisningen i ditt CRM-system om det finns någon. Det här är ett fält för fritextinmatning.|34234324-sdfsdf-345345-sfd
Marknadsföringskampanj-ID|No|Det här fältet anger marknadsföringskampanjen, som resulterade i den här specifika hänvisningen. Används vanligtvis för ROI-beräkning|BingSummer2020
Kommentarer|No|Detaljerad information som anger uppdateringarna som rör hänvisningen|Det här är ett exempel på en anteckning
Microsoft-hjälp krävs?|Yes|Detta är för att ange om du vill att Microsoft ska hjälpa dig att göra denna begäran om säljförsäljning|Yes
Vilken specifik hjälp från Microsoft?|Beror|Ett av de sex olika sätt som Microsoft kan hjälpa dig. Detta gäller bara om du väljer Ja för frågan "Microsoft-hjälp krävs? " <br/> **Ange ett tal baserat på alternativen nedan** <br/><br/> **1**– Arbetsbelastning – specifikt värdeförslag  <br/> **2**– Kundens tekniska arkitektur  <br/> **3**– Konceptbevis /Demo  <br/> **4**– Offerter och licensiering  <br/> **5**– Post – kundframgång för försäljning  <br/> **6**– Allmänt eller annat|1|
Dela med Microsofts säljteam|Yes|Detta är för att ange om du vill dela information om avtalet med Microsofts säljteam eller inte. Detta gäller endast om du väljer Nej för frågan "Microsoft-hjälp krävs? "|Yes
Kommentarer till Microsoft|No|Eventuella specifika kommentarer till Microsoft om du behöver hjälp från Microsoft|Behöver hjälp med en POC för Contoso-kund
Samtycka till att dela kund-/partnerkontakt|Yes|Samtycka till att dela kundens kontaktuppgifter och dina anställdas kontaktuppgifter som arbetar med avtalet. **Avtal skapas eller uppdateras inte om du väljer Nej för den här kolumnen.** |Yes
Lösning 1|Yes|Lösnings-ID (krävs), valutan (valfritt) där avtalsvärdet anges. Du hittar valutakoderna [här,](https://en.wikipedia.org/wiki/ISO_4217)Pris för SKU:n (valfritt) och Antal för SKU:n (valfritt)  |SOL-1234-PQRS, USD, 10, 100
Teammedlem 1|Yes|Förnamn, Efternamn, mobilnummer och e-post-ID för respektive teammedlem.| Bob, Partner, 999999, Bob.partner@Contoso.com

## <a name="next-steps"></a>Nästa steg

Du kan använda dessa partnercenteranslutningsappar för säljförsäljning för att samarbeta med Microsoft i dina CRM-system.

- [Anslutningsapp för säljförsäljning för Dynamics 365 CRM – översikt](connector-dynamics.md)
- [Anslutningsapp för säljförsäljning för Salesforce CRM – översikt](connector-salesforce.md)
