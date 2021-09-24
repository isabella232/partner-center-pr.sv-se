---
title: Massexport och import av möjligheter till säljförsäljning via Excel-/CSV-filer i referenser
description: Lär dig hur du laddar ned, skapar eller uppdaterar möjligheter till säljförsäljning med hjälp Excel (CSV)-filer i Partnercenter
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-referrals
author: vikramb
ms.author: vikramb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 09/08/2021
ms.openlocfilehash: a87b44bb2730faf87bfaaf25b5e051b0ce4f6f30
ms.sourcegitcommit: fceaca54b0ec695cf214209c09b4516e1b40866a
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/23/2021
ms.locfileid: "128326426"
---
# <a name="bulk-operations-for-co-sell-opportunities-using-comma-separated-value-csv-files"></a>Massåtgärder för möjligheter till säljförsäljning med hjälp av csv-filer (kommaavgränsade värden)

**Lämpliga roller:** Referensadministratörsroller | Referensanvändare

Med hjälp av massåtgärder i Partnercenter kan ditt företag exportera och importera data för säljsamarbetesmöjligheter. Gå till sidan **möjligheter till säljförsäljning för** att hitta **import-** och **exportlänkarna** längst upp till höger på banderollen för sidrubriken. Användare med behörighet som både **referensadministratör** och **referensanvändare** kan använda den här funktionen.

> [!IMPORTANT]
> Åtgärderna för att skapa/uppdatera som utförs via massimport kan inte ångras. Var försiktig när du ändrar eller skapar ett stort antal poster. Endast en delmängd av fälten kan ändras när du har skapat ett avtal. **Inga åtgärder tillåts när ett avtal når ett slutgiltigt tillstånd som Nekat/Upphört/Vunnet/Förlorat.**

## <a name="export-co-sell-opportunities"></a>Exportera möjligheter till säljsamarbete

Följande information beskriver exportfunktionen:

- Du kan exportera högst **5 000 poster genom** att klicka på **exportknappen.**
- De avtal som laddas ned baseras på dina åtkomstnivåer. Referensadministratörer och hänvisningsanvändare kan få olika resultat baserat på deras omfattning och inkludering som teammedlemmar i avtal. Läs mer om [referensbehörigheter.](permissions-overview.md#manage-referrals)
- Exportfunktionen tar hänsyn till den aktuella fliken på sidan möjligheter till säljförsäljning och de filter som har tillämpats.
- En CSV-fil med alla data baserat på tillämpade filter genereras.
- Det kan ta upp till en minut att ladda ned posterna.
- Du behöver inte vänta tills nedladdningsåtgärden har slutförts. Även om du navigerar till andra sidor i Partnercenter hämtas filen så fort exportfunktionen har slutförts.
- Du kan återanvända den nedladdade filen för att ändra avtalsinformationen och ladda upp för att uppdatera eventuella poster.

## <a name="import-co-sell-opportunities"></a>Importera möjligheter till säljsamarbete

- Du kan skapa eller uppdatera **högst 1 000 poster med** hjälp av importfunktionen.
- Du kan skapa mallen från grunden genom att ladda ned mallen från sidan Importera i Partnercenter.
- Du kan också använda funktionen Exportera för att ladda ned befintliga poster och uppdatera dem.
- Om filen har fler än 1 000 poster kan den inte bearbetas.
- När filen har bearbetats visas en sammanfattning med antalet referenser som har skapats, uppdaterats och inte bearbetats i det senaste processfilkortet.
- Du kan ladda ned information om bearbetade poster, åtgärda eventuella fel och ladda upp samma fil för att skapa eller uppdatera posterna som misslyckades i föregående körning. **Ta bort alla lyckade poster från filen innan du överför de korrigerade posterna som misslyckades i föregående körning.**
- Om du vill lägga till fler lösningar lägger du till extra kolumner bredvid lösning 1 och använder kolumnnamnet som Lösning X, där X representerar antalet lösningen i avtalet. Till exempel Lösning 2, Lösning 3.
- Du kan lägga till upp till 50 lösningar i ett avtal.
- Om du vill lägga till fler teammedlemmar lägger du till extra kolumner bredvid Teammedlem 1 och använder kolumnnamnet som Teammedlem X, där X representerar antalet teammedlemmen i avtalet. Till exempel Teammedlem 2, Teammedlem 3.
- Du kan lägga till upp till 50 teammedlemmar i ett avtal.

> [!NOTE]
> Du behöver inte vänta på att bearbetningen ska slutföras. Information om den senast bearbetade filen är tillgänglig för nedladdning när bearbetningen är klar. **Det kan ta upp till 10 minuter om du laddar upp filer med 1 000 poster.**

> [!IMPORTANT]
> Läs alla instruktioner noggrant och kontrollera formatet för varje kolumn i tabellen nedan innan du skapar eller uppdaterar avtal med CSV-filer i Partnercenter.

Alla fält i mallen kan inte redigeras. Det finns fält som alltid är skrivskyddade, vissa ändras till skrivskyddade status när hänvisningen har skapats och vissa ändras till skrivskyddade när du har ändrat dem till ett visst värde.

### <a name="fields-that-are-always-read-only"></a>Fält som alltid är skrivskyddade

- Fel
- Engagemangs-ID
- Hänvisningskod
- Microsoft-hänvisningsstatus
- Microsoft MSX-ID
- Migrerat PSC-avtals-ID
- Microsoft-teammedlem

### <a name="fields-that-will-become-read-only-after-you-create-the-referral"></a>Fält som blir skrivskyddade när du har skapat referensen

- Kundnamn
- Kundadressrad 1
- Kundadress rad 2
- Kundstad
- Kundtillstånd
- Kundpostnummer
- Kundland
- Kundens D-U-N-S-ID
- Samtycka till att dela kund-/partnerkontakt
- MPN-ID

### <a name="fields-that-will-become-read-only-after-you-first-share-them"></a>Fält som blir skrivskyddade när du delar dem första gången

- **Förnamnet på kundkontakten** blir skrivskyddade när du har skickat in information om hur du skapar eller uppgraderar en hänvisning till säljförsäljning
- **Kundens kontakts efternamn** blir skrivskyddade när du har skickat in information om hur du skapar eller uppgraderar en referens för säljförsäljning
- **Kundkontaktens Telefon blir** skrivskyddade när du har skickat in information om hur du skapar eller uppgraderar en hänvisning till säljförsäljning
- **E-postadressen för kundkontakt** blir skrivskyddat när du har skickat in information för att skapa eller uppgradera en hänvisning till säljförsäljning
- **Microsoft-hjälp krävs?** blir skrivskyddade när du har markerar den som Ja
- **Vilken specifik hjälp från Microsoft?** blir skrivskyddade när du har angett ett tal i det angivna formatet
- **Dela med Microsofts säljteam** blir skrivskyddade när du har markerar det som Ja
- **Anteckningar till Microsoft** blir skrivskyddade när du har skickat in anteckningar för att skapa eller uppgradera en hänvisning till säljförsäljning

Information om alla kolumner med deras information och exempelvärden finns i tabellen nedan.

|**Kolumnnamn**|**Är obligatoriskt?**|**Beskrivning**|**Exempelvärden**|
|-----|:-----|:---------|:---|
Fel|Inga|Fel om några relaterade till create/update-åtgärderna w.r.t till hänvisningarna inkluderas i den här kolumnen. Om det finns flera fel visas alla med semikolon.|Obligatoriskt fält Lösning 1 saknas|
Engagemangs-ID|Ja|Engagemangs-ID:t genereras av Microsoft Partner Center-referenssystemet. Krävs inte för att skapa en ny referens. Du kan använda det befintliga engagemangs-ID:t om du uppdaterar en post.|f7eaae47-0b84-4ac4-b4ea-5b2587d42cee
Hänvisningskod|Ja|Hänvisnings-ID genereras av referenssystemet för Microsoft Partner Center. Krävs inte för att skapa en ny referens. Fyll i det med referens-ID:t om du uppdaterar en befintlig post.|ebacdkdc-0b84-4ac4-b4ea-5b2587d42cee
Avtalsnamn|Ja|Det egna namnet för avtalet för din referens.|Storbritannien, våravtal
Kundnamn|Ja|Namnet på kundföretaget. Använd organisationens juridiska namn för snabb matchning på Microsoft-sidan.|Contoso Corporation
Kundadressrad 1|Ja|Adressrad 1 i kundföretaget. |One Contoso Way
Kundadress rad 2|Inga|Adressrad 2 på kundföretaget.|NE 148 street
Kundens stad|Ja|Ort där kundorganisationen finns.|Redmond
Kundtillstånd|Inga|Ange var kundorganisationen finns.|Washington
Kundens postnummer|Inga|Postnummer i den region där kundorganisationen finns.|98052
Kundland|Ja|Land/region där kundorganisationen finns. Använd *alfa-2-koden med två bokstäver i* den här listan med [landskoder.](https://en.wikipedia.org/wiki/List_of_ISO_3166_country_codes)|USA
Kundens D-U-N-S-ID|Inga|Försök att hämta KUNDORGANISATIONENS DUNS-ID. Detta hjälper till med snabbare matchning av kundorganisationen på Microsoft-sidan, vilket hjälper till att få snabbare säljtilldelning. Du kan hämta DUNS-ID kostnadsfritt från sidan [D-U-N-S Number Lookup (Antal uppslag i D-U-N-S).](https://www.dnb.com/duns-number/lookup.html)|81466849
Kundens kontakts förnamn|Beror|Förnamn är bara obligatoriskt om du behöver Microsoft-hjälp. Förnamnet på den primära kontakten från kundorganisationen som arbetar med detta avtal.|John
Kundens kontakts efternamn|Beror|Efternamn är bara obligatoriskt om du behöver Microsoft-hjälp. Efternamnet på den primära kontakten från kundorganisationen som arbetar med detta avtal.|Kund
Kundkontaktens Telefon nummer|Beror|Telefon är bara obligatoriskt om du behöver Microsoft-hjälp. Telefon antalet primära kontakter från kundorganisationen som arbetar med det här avtalet.|9999999999
E-postadress till kundkontakt|Beror|E-postadressen är bara obligatorisk om du behöver Microsoft-hjälp. E-postadressen till den primära kontakten från kundorganisationen som arbetar med detta avtal.|john.customer@contoso.com
Referensstatus för partner|Ja|Visar status för avtalet från företagets perspektiv. Krävs om du försöker skapa eller ändra en referens. Använd **Ny** om du försöker skapa ett nytt avtal. Värden som du kan använda visas i [Hänvisningsresurser.](/partner/develop/referral-resources#referralstatus)|Aktiv
Understatus för partnerreferens|Ja|Anger den exakta statusen för avtalet. Använd **Accepterad** om du försöker skapa ett nytt avtal. Det krävs även om du ändrar en befintlig referens. Värden som du kan använda visas i [Hänvisningsresurser.](/partner/develop/referral-resources#referralsubstatus)|Har godkänts
Microsoft-hänvisningsstatus|Beror|Visar status för den begäran om säljförsäljning som du har skickat till Microsoft och som behöver hjälp. Det här är ett skrivskyddade fält. Ändringar som görs i det här fältet när du importerar data ignoreras.| Väntar
Nekad/förlorad orsak|Beror| Du behöver bara ange den här informationen om du ändrar understatusen för fältet till antingen Nekad eller Förlorad. Annars kan du ignorera den här kolumnen. <br/> **Ange ett tal baserat på alternativen nedan** <br/><br/> **1**– Project budget inte är tillräcklig  <br/> **2**– Kunden svarade inte  <br/> **3**– Kunden valde en annan leverantör  <br/> **4** – Kundkravet uppfylls inte  <br/> **5** – Inte en kund <br/> **6**– Den föreslagna tidsraden var för kort <br/> **7** – Rapportera som missbruk, skräppost eller nätfiske <br/> **8** – Andra |6|
Försäljningsstadie|Inga|Det här är fältet för att ange den detaljerade försäljningsfasen för hänvisningen. Läs mer om försäljningsstadier [i Hantera möjligheter till säljförsäljning i Partnercenter](./manage-co-sell-opportunities.md)|40
Beräknat avtalsvärde|Ja|Avtalets värde baseras på de första konversationerna med kunden. Detta kan ändras tills avtalet når ett av de terminal-tillstånd som **vunnits eller** **förlorats.**|12563
Valuta|Ja|Valutan som avtalsvärdet anges i. Valutakoderna finns på [Wikipedia-sidan ISO 4217.](https://en.wikipedia.org/wiki/ISO_4217)|USD
Beräknat stängningsdatum|Ja|Beräknat slutdatum för avtalet baserat på de första konversationerna med kunden i formatet MM/DD/ÅYYY. <br/> **Datumet ska vara i UTC-tidszonen. Alla datum som visas i partnercentrets användargränssnitt baseras på lokaliserade tidszoner. Det kan finnas +/- en dag i Användargränssnittet i Partnercenter om du tittar på den referens som du angav datumet för i UTC-tidszonen.**|1/30/2020
CRM-ID|Inga|Identifierare för den här specifika hänvisningen i ditt CRM-system om det finns någon. Det här är ett fält för fritextinmatning.|34234324-sdfsdf-345345-sfd
Marknadsföringskampanj-ID|Inga|Det här fältet anger marknadsföringskampanjen, som resulterade i den här specifika hänvisningen. Används vanligtvis för ROI-beräkning|BingSummer2020
Kommentarer|Inga|Detaljerad information som anger uppdateringarna som rör referensen|Det här är ett exempel på en anteckning
Microsoft-hjälp krävs?|Ja|Detta är för att ange om du vill att Microsoft ska hjälpa dig att göra denna begäran om säljförsäljning|Ja
Vilken specifik hjälp från Microsoft?|Beror|Ett av de sex olika sätt som Microsoft kan hjälpa dig på. Detta gäller bara om du väljer Ja för frågan "Microsoft-hjälp krävs? " <br/> **Ange ett tal baserat på alternativen nedan** <br/><br/> **1**– Arbetsbelastning – specifikt värdeförslag  <br/> **2**– Kundens tekniska arkitektur  <br/> **3**– Konceptbevis /Demo  <br/> **4**– Offerter och licensiering  <br/> **5**– Post – kundframgång för försäljning  <br/> **6**– Allmänt eller annat|1|
Dela med Microsofts säljteam|Ja|Detta är för att ange om du vill dela information om avtalet med Microsofts säljteam eller inte. Detta gäller endast om du väljer Nej för frågan "Microsoft-hjälp krävs? "|Ja
Kommentarer till Microsoft|Inga|Eventuella specifika kommentarer till Microsoft om du behöver hjälp från Microsoft|Behöver hjälp med en POC för Contoso-kund
Samtycka till att dela kund-/partnerkontakt|Ja|Samtycka till att dela kundens kontaktuppgifter och dina anställdas kontaktuppgifter som arbetar med avtalet. **Avtal skapas eller uppdateras inte om du väljer Nej för den här kolumnen.** |Ja
CLA-nummer|Beror|CLA-nummer krävs inte när du skapar eller uppdaterar ett IOT-avtal. Det blir obligatoriskt när du går över till designsteget för vinst.
Enhetskategori|Inga|Lista över alla IoT-enhetskategorier. Välj en kategori bland alternativen nedan <br>Consumer Gaming Device <br> ATM <br> Transportsystem & fordonstrafik <br> Azure Sphere tavla<br> Azure Sphere-komponent <br> Azure Sphere Guardian<br> Azure Sphere-modul <br> Skapa automation<br> Gaming-enhet <br> Kommunikationsenheter<br> Konsumentens Internetenhet <br> Konsumentförslitningsbar<br> Digital bildram <br> Digital Signage <br> Gateway <br> HHT/Mobile<br> Branschautomatiseringsenhet<br> Bransch surfplatta (icke-POS) <br> Helskärmsläge<br> Media Player<br> Medieenhet <br> Mobil POS <br> Navigeringsenhet<br> Nätverksprojektor<br> Övrigt<br> Annan bankenhet<br> Annan elektronisk konsumentenhet<br> Annan enhet<br> Annan företagsenhet<br>  Annan sensor/nod <br> Försäljningsenhet<br> Utskriftsenhet <br> Säkerhet/övervakning <br>  Server<br> Set-Top Box<br> Smart TV <br> Test- och mätningsenhet<br> Tunn klientenhet <br/>
Silicon Type|Inga|Ange information om kretsuppsättningsmodellen genom att välja ett alternativ i listan nedan <br> AMD – A10 <br> AMD – A4 <br> AMD – A6 <br> AMD – A8 <br> AMD – E2 <br> AMD – FX 7500 <br> AMD – FX 7600P <br> AMD – FX 9370 <br> AMD – FX 9590 <br> AMD – G-serien <br> AMD – Andra <br> AMD – R-serien <br> AMD – resten av FX-modeller <br> Intel – Atom <br> Intel –Selleron – N1900 <br> Intel –Selleron – N2807 <br> Intel –Selleron – N2930 <br> Intel –Selleron – N3060 <br> Intel –Selleron – N3160 <br> Intel – Core i3 <br> Intel – Core i5 <br> Intel – Core i7 <br> Intel – Core M <br> Intel – Andra <br> Intel – Pentium <br> Intel – resten avSelleron <br> Intel – XEON <br> MediaTek MT3620 <br> NXP 8ULP-CS <br> Andra <br/>
Azure-certifierad enhet|Inga|Detta är för att ange om Azure-kompatibilitetscertifieringen har uppnåtts för enheten
Bifoga tjänster|Inga|Detta är för att ange om Azure-tjänsterna ska paketeras med IoT-lösningen vid distribution
Microsoft MSX-ID|Inga|ID för ett avtal i Microsoft MSX-systemet, endast tillgängligt för möjligheter till säljförsäljning
Migrerat PSC-avtals-ID|Inga|PSC-avtals-ID, endast tillgängligt för ett avtal som migrerats från PSC till PC
MPN-ID|Inga|MPN-ID för den organisation som säljarna skapas för
Lösning 1|Ja|Lösnings-ID (krävs), valutan (valfritt) där avtalsvärdet anges. Du hittar [valutakoderna](https://en.wikipedia.org/wiki/ISO_4217), Pris för SKU:n (valfritt) och Antal för SKU:n (valfritt)  |SOL-1234-PQRS, USD, 10, 100
Teammedlem 1|Ja|Förnamn, Efternamn, mobilnummer och e-post-ID för respektive teammedlem.| Bob, Partner, 999999, Bob.partner@Contoso.com
Microsoft-teammedlem 1|Inga|Förnamn, Efternamn, mobilnummer och e-post-ID för respektive Microsoft-teammedlem som arbetar med säljförsäljningsmöjligheten.| Sam, Seller, 999999, Sam.seller@Microsoft.com

## <a name="next-steps"></a>Nästa steg

Du kan använda dessa partnercenteranslutningsappar för säljförsäljning för att samförsäljninga med Microsoft inifrån dina CRM-system.

- [Anslutningsapp för säljförsäljning för Dynamics 365 CRM – översikt](connector-dynamics.md)
- [Anslutningsapp för säljförsäljning för Salesforce CRM – översikt](connector-salesforce.md)
