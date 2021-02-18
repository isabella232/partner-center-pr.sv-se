---
title: Mass åtgärder via Excel-filer i hänvisningar
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Lär dig hur du hämtar, skapar eller uppdaterar samförsäljnings möjligheter med Excel-filer
author: vikramb
ms.author: vikramb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 02/03/2021
ms.openlocfilehash: 16975e78c10aeb73bf141c1a1d0a215ac885039c
ms.sourcegitcommit: 64243caed029ffe40e2bbc369f4ee96f4f0ca26f
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 02/18/2021
ms.locfileid: "100645647"
---
# <a name="bulk-operations-for-co-sell-opportunities-using-comma-separated-valuecsv-files"></a>Mass åtgärder för samförsäljnings möjligheter med hjälp av CSV-filer (kommaavgränsade värden)

**Lämpliga roller**

- Referens administratör
- Referent användare

Mass åtgärder i Partner Center hjälper företaget att exportera och importera affärs möjlighets data. Gå till sidan affärs möjligheter för samförsäljning för att hitta import-och export länkarna längst upp till höger i banderollen för sid rubriken. Användare med både **referral admin** och **referral User** -behörigheter kan använda den här funktionen.

> [!IMPORTANT]
> Det går inte att ångra åtgärderna för att skapa/uppdatera som görs via Mass import. Var försiktig när du ändrar eller skapar ett stort antal poster. Endast en delmängd av fälten kan ändras efter att du har skapat ett avtal. **Inga åtgärder tillåts när något avtal når ett Terminal-tillstånd som nekad/upphört/uppnådd/förlorad/förlorad.**

## <a name="exporting-co-sell-opportunities"></a>Exportera samförsäljnings möjligheter

Nedan visas information om export funktionen

- Du kan exportera **högst 5000 poster** genom att klicka på knappen Exportera.
- De avtal som hämtas kommer att baseras på dina åtkomst nivåer. Hänvisnings administratörer och hänvisnings användare kan få olika resultat baserat på deras omfattning och inkluderas som grupp medlemmar i avtalen. Läs mer om [referens behörigheter](permissions-overview.md#manage-referrals).
- Funktionen export tar i att ta hänsyn till den aktuella fliken på sidan samförsäljnings möjligheter och de filter som har tillämpats.
- En CSV-fil med alla data som baseras på de filter som används skapas.
- Det kan ta upp till en minut att hämta posterna.
- Du behöver inte vänta på att nedladdnings åtgärden ska slutföras. Även om du navigerar till andra sidor i Partner Center hämtas filen så snart export funktionen har slutförts.
- Du kan återanvända den nedladdade filen för att ändra avtals informationen och ladda upp för att uppdatera alla poster.

## <a name="importing-co-sell-opportunities"></a>Importera affärs möjligheter för försäljning

- Du kan skapa eller uppdatera **högst 1000 poster** med hjälp av import funktionen.
- Du kan bygga mallen från grunden genom att hämta mallen från import sidan på Partner Center.
- Du kan också använda export funktionen för att hämta befintliga poster och uppdatera dem.
- Om filen har fler än 1000 poster kan den inte bearbetas.
- När filen har bearbetats visas en sammanfattning med antalet referenser som har skapats, uppdaterats och inte bearbetats i det senaste process fil kortet.
- Du kan hämta information om bearbetade poster, åtgärda eventuella fel och överföra samma fil för att skapa eller uppdatera de poster som misslyckades i föregående körning. **Ta bort alla lyckade poster från filen innan du överför de korrigerade poster som misslyckades i föregående körning.**
- För att lägga till fler lösningar lägger du till extra kolumner bredvid lösning 1 och använder kolumn namnet som lösning X, där X representerar numret för lösningen i affären. Till exempel lösning 2, lösning 3.
- Du kan lägga till upp till 50 lösningar i ett avtal.
- För att lägga till fler grupp medlemmar lägger du till extra kolumner bredvid team medlem 1 och använder kolumn namnet som grupp medlem X, där X representerar team medlemmens nummer i affären. Till exempel grupp medlem 2, grupp medlem 3.
- Du kan lägga till upp till 50 team medlemmar i ett avtal.

> [!NOTE]
> Du behöver inte vänta på att bearbetningen ska slutföras. Information om den senast bearbetade filen kommer att vara tillgänglig när bearbetningen är klar. **Det kan ta upp till 10 minuter att ladda upp filer med 1000 poster.**

> [!IMPORTANT]
> Läs igenom alla anvisningar noggrant och kontrol lera formatet för varje kolumn i tabellen nedan innan du skapar eller uppdaterar avtal med CSV-filer i Partner Center.

|**Kolumnnamn**|**Är obligatorisk?**|**Beskrivning**|**Exempel värde (n)**|
|-----|:-----|:---------|:---|
Fel|No|Fel om någon som är relaterad till åtgärderna skapa/uppdatera w. r. t till hänvisningarna ska tas med i den här kolumnen. Om det finns flera fel visas alla dessa med semikolon.|Obligatorisk fält lösning 1 saknas|
Förlovnings-ID|No|Åtagande-ID: t genereras av Microsoft Partner Center referral system. Krävs inte för att skapa en ny hänvisning. Du kan använda det befintliga åtagande-ID: t om du uppdaterar en post.|f7eaae47-0b84-4ac4-b4ea-5b2587d42cee
Hänvisningskod|No|Hänvisnings-ID genereras av Microsoft Partner Center referral system. Krävs inte för att skapa en ny hänvisning. Fyll i det med hänvisnings-ID: t om du uppdaterar en befintlig post.|ebacdkdc-0b84-4ac4-b4ea-5b2587d42cee
Avtals namn|Yes|Det egna namnet på erbjudandet för din referens.|BRITTISKA våren-erbjudandet
Kundnamn|Yes|Namnet på kund företaget. Använd organisationens juridiska namn för snabb matchning på Microsoft-sidan.|Contoso Corporation
Kund adress rad 1|Yes|Adress rad 1 för kund företaget. |Ett contoso-sätt
Kund adress rad 2|No|Adress rad 2 för kund företaget.|NE 148-gata
Kund ort|Yes|Ort där kund organisationen befinner sig.|Redmond
Kund tillstånd|No|Stat där kund organisationen befinner sig.|Washington
Kund post nummer|No|Post nummer för den region där kund organisationen finns.|98052
Kund land|Yes|Land/region där kund organisationen finns. Använd de två lands koderna för bokstäver som anges [här]( https://en.wikipedia.org/wiki/List_of_ISO_3166_country_codes).|USA
Customer D – U-N-S ID|No|Försök att hämta DUNS-ID: t för kund organisationen. Detta hjälper till att snabbare matcha kund organisationen på Microsoft-sidan, vilket underlättar säljarens tilldelning. Du kan hämta DUNS-ID kostnads fritt från den här [webbplatsen](https://www.dnb.com/duns-number/lookup.html).|81466849
Förnamn för kund kontakt|Väggen|Förnamn är bara obligatoriskt om du behöver Microsoft hjälp. Det första namnet på den primära kontakten från kund organisationen som arbetar med detta avtal.|John
Kundens kontakt efter namn|Väggen|Efter namn är bara obligatoriskt om du behöver Microsoft hjälp. Efter namnet på den primära kontakten från kund organisationen som arbetar på detta avtal.|Kund
Telefonnummer till kund kontakt|Väggen|Telefonnummer är bara obligatoriskt om du behöver Microsoft hjälp. Telefonnumret till den primära kontakten från kund organisationen som arbetar på detta avtal.|9999999999
E-postadress till kund kontakt|Väggen|E-postadress är bara obligatorisk om du behöver Microsoft hjälp. E-postadressen till den primära kontakten från kund organisationen som arbetar på detta avtal.|john.customer@contoso.com
Partner hänvisnings status|Yes|Anger status för affären från ditt företags perspektiv. Krävs om du försöker skapa eller ändra en referens. Använd **ny** om du försöker skapa ett nytt avtal. Godkända värden dokumenteras [här](https://docs.microsoft.com/partner/develop/referral-resources#referralstatus).|Aktiv
Under status för partner referral|Yes|Anger den exakta statusen för affären. Använd **accepterat** om du försöker skapa ett nytt avtal. Det krävs också om du ändrar en befintlig hänvisning. Godkända värden dokumenteras [här](https://docs.microsoft.com/partner/develop/referral-resources#referralsubstatus).|Har godkänts
Microsoft referral-status|Väggen|Anger statusen för den samförsäljnings förfrågan som du skickade till Microsoft som söker hjälp. Detta är ett skrivskyddat fält. Alla ändringar som görs i fältet när data importeras ignoreras.| Väntar
Nekad/förlorad orsak|Väggen| Du behöver bara ange den här informationen om du ändrar under status för fältet till antingen avböjt eller förlorat. Du kan ignorera den här kolumnen annars. <br/> **Ange ett tal baserat på alternativen nedan** <br/><br/> **1**– projekt budgeten är inte tillräcklig  <br/> **2**– kunden svarade inte  <br/> **3**– kunden valde en annan leverantör  <br/> **4** – kund krav har inte uppfyllts  <br/> **5** – inte en kund <br/> **6**-föreslagen tids linje var för kort <br/> **7** -rapportera som missbruk, skräp post eller nätfiske <br/> **8** – andra |6|
Försäljningsstadie|No|Det här är fältet för att ange det detaljerade försäljnings steget för hänvisningen. Läs mer om försäljnings faserna [här](https://aka.ms/salesStages)|40
Uppskattat avtals värde|Yes|"Värdet för affären baserat på de första samtalen med kunden. Detta kan ändras tills avtalet når ett av Terminal-tillstånden| vunnen eller förlorad. "|12563
Valuta|Yes|Den valuta i vilken det avtalade värdet anges. Du hittar valuta koderna [här](https://en.wikipedia.org/wiki/ISO_4217).|USD
Beräknat stängnings datum|Yes|Det beräknade stängnings datumet för affären baserat på de första samtalen med kunden i formatet MM/DD/ÅÅÅÅ. <br/> **Datumet bör vara i UTC-tidszonen. Alla datum som visas i Partner Center-ANVÄNDARGRÄNSSNITTET baseras på lokaliserade tids zoner. Det kan finnas en skillnad på +/-en dag i användar gränssnittet för partner Center om du tittar på den referens som du angav för datumet i UTC-tidszonen.**|1/30/2020
CRM-ID|No|Identifierare för den här aktuella hänvisningen i CRM-systemet om det finns någon. Det här är ett kostnads fritt text inmatnings fält.|34234324-sdfsdf-345345-SFD
ID för marknadsförings kampanj|No|I det här fältet anges marknadsförings kampanjen som resulterade i den här referensen. Används vanligt vis för ROI-beräkning|BingSummer2020
Kommentarer|No|Detaljerade kommentarer som visar vilka uppdateringar som är relaterade till hänvisningen|Detta är ett exempel på en anteckning
Krävs Microsoft-hjälp?|Yes|Detta är att ange om du vill att Microsoft ska hjälpa dig att göra den här samförsäljnings förfrågan|Yes
Vilken hjälp från Microsoft?|Väggen|Ett av sex olika sätt som Microsoft kan hjälpa dig med. Detta gäller endast om du väljer Nej för frågan "Microsoft-Hjälp krävs? " <br/> **Ange ett tal baserat på alternativen nedan** <br/><br/> **1**– eget värde för arbets belastning  <br/> **2**– teknisk arkitektur för kunder  <br/> **3**– proof of Concept/demo  <br/> **4**– offerter och licensiering  <br/> **5**– kund slutförd efter försäljning  <br/> **6**-allmänt eller annat|1|
Dela med Microsoft Sales-teamet|Yes|Detta är att ange om du vill dela information om erbjudandet med Microsoft Sales-teamet eller inte. Detta gäller endast om du väljer Nej för frågan "Microsoft-Hjälp krävs? "|Yes
Anteckningar till Microsoft|No|Alla speciella anteckningar till Microsoft om du behöver hjälp från Microsoft|Behöver hjälp med en POC för Contoso-kund
Medgivande för att dela kund-/partner kontakt|Yes|Medgivande för att dela kund kontakt uppgifter och företagets anställda kontakt uppgifter som arbetar med erbjudandet. **Det går inte att skapa eller uppdatera avtal om du väljer Nej för den här kolumnen.** |Yes
Lösning 1|Yes|Lösnings-ID (krävs), den valuta (valfritt) som det avtalade värdet anges i. Du hittar valuta koderna [här](https://en.wikipedia.org/wiki/ISO_4217), priset på SKU (valfritt) och antal för SKU (valfritt)  |SOL-1234-PQRS, USD, 10, 100
Team medlem 1|Yes|Förnamn, efter namn, mobiltelefon nummer och e-post-ID för respektive grupp medlem.| Bob, partner, 999999, Bob.partner@Contoso.com
