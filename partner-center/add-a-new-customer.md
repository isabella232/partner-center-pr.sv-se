---
title: Så här lägger du till en ny kundpost
ms.topic: how-to
ms.date: 09/27/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-customers
description: Lär dig hur du lägger till en ny kundpost i Partnercenter. Sedan kan du sälja kundprenumerationer, hantera fakturering eller tillhandahålla kundsupport.
author: parthp
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOAPR.20
ms.openlocfilehash: 0d3b7787cf0f41a04f0a662450040802d74e9ef7
ms.sourcegitcommit: 1e616b52d55eff41d67a081ba3f4a8370a49e027
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/29/2021
ms.locfileid: "129191450"
---
# <a name="how-to-add-a-new-customer-record-in-partner-center"></a>Så här lägger du till en ny kundpost i Partnercenter

**Lämpliga roller:** Globala | Administratörsbehörighet för | Administratörsagent | Försäljningsagent

I den här artikeln beskrivs hur du lägger till en ny kund i Partnercenter. De här stegen krävs innan du kan sälja prenumerationer, hantera fakturering eller ge support till en kund.

## <a name="considerations"></a>Överväganden

När du lägger till en ny kundpost i Partnercenter:

- **Använd rätt registrerings-ID:** När du anger ditt företagsregistrerings-ID måste du använda ditt företags skatte-ID och inte kundens personliga ID.

- **Ange ytterligare information för vissa länder:** Företagsregistrerings-ID och telefonnummer krävs för vissa länder om du är en partner för direktfakturering eller en indirekt leverantör [](#company-registration-id-and-phone-number-required-for-some-countries)

- **Bekräfta Microsoft-kundavtal:** Innan du kan göra en beställning åt en kund måste du bekräfta att kunden har godkänt [Microsoft-kundavtal](confirm-customer-agreement.md).

- **Använd olika  steg för** befintliga kunder: För befintliga kunder, inklusive de som redan har kundposter i Partnercenter via ett [scenario](multichannel.md) med flera kanaler eller [flera](multipartner.md) [partner,](request-a-relationship-with-a-customer.md)begär du en relation med dem i stället för att följa stegen här.

- **Ange detaljerad, korrekt kundinformation:** För att underlätta kundverifiering, se till att du:
  - Ange det exakta juridiska/officiella namnet som det visas i de officiella dokumenten.
  - Undvik att använda förkortningar eller korta formulär.
  - Använd inte testnamn.
  - Ange fullständig, exakt adressinformation (till exempel platsinformation, ort, delstat, land och postnummer).

## <a name="new-rules-for-company-name-and-email-address"></a>Nya regler för företagsnamn och e-postadress

Från och med den 22 september 2021 gäller följande nya valideringsregler.

När du anger ett företagsnamn tillåts inte följande:
- Använd bara ett tecken.
- Använd endast specialtecken, till exempel &$^# (se [tabellen](#table-of-special-characters) nedan).
- Endast blanksteg och/eller tabbar.
- Använda fristående förkortningar från listan över begränsade namn, till exempel LLC, Inc osv. (se [tabellen](#table-of-abbreviations) nedan).
- Använda namn med TDL-tillägg (Internet Top-Level Domain), till exempel ".com", ".org", ".edu", ".club" osv. (se [tabellen](#table-of-top-level-domain-extensions) nedan).

- Använda samma tecken som upprepas tre eller flera gånger utan andra tecken, till exempel 999.

- Använda blanksteg och/eller tabbar blandat med enskilda tecken, till exempel 1 2 3.

När du anger en kunds e-postadress tillåts inte följande:

- E-postadressen får inte innehålla @microsoft.com .
- Kundens e-postadress får inte innehålla samma domännamn som partnern. En partner som heter ABC kan till exempel inte skapa ett e-postmeddelande för kunder med @abc.com .

## <a name="to-add-a-new-customer-in-partner-center"></a>Så här lägger du till en ny kund i Partnercenter

> [!NOTE]
> Mer information om gränssnittet för arbetsytor finns i [Getting around Partner Center (Ta sig runt i Partnercenter).](get-around-partner-center.md#turn-workspaces-on-and-off)

#### <a name="workspaces-view"></a>[Vyn Arbetsytor](#tab/workspaces-view)

1. Logga in på [instrumentpanelen i Partnercenter,](https://partner.microsoft.com/dashboard)välj **panelen Kunder** och välj sedan Lägg **till kund.**

2. Om kunden är en utbildningsnämnd kan du se [hur du skapar en eduktionskund.](sell-to-education-customers.md)

3. På **sidan Kontoinformation** anger du kundens information och primär kontaktinformation.
   >[!IMPORTANT]
   >Partner måste intyga följande:
   >
   >Jag bekräftar att min organisation fungerar som en indirekt partner när jag väljer en återförsäljare och som direkt partner utan att välja en återförsäljare
   >
   >Jag bekräftar att jag inte säljer produkter som köpts i den här ordern till andra partner som är kopplade till min överordnade organisation

   >[!NOTE]
   >EU-/EFTA-lagar anger att partner som gör transaktioner i dessa länder måste deklarera ytterligare återförsäljare som är associerade med en transaktion. Följande regler gäller:
   >- En första återförsäljare måste väljas innan ytterligare återförsäljare
   >- Ytterligare återförsäljare har inte rätt till ytterligare incitament, erbjudanden osv.
   >- Ytterligare säljare som angetts verifieras för att säkerställa att rätt MPN-ID anges i förekommande fall och att återförsäljaren har signerat MPA.
   >- Upp till 5 ytterligare återförsäljare kan anges som en del av transaktionen

4. Om du är en indirekt leverantör väljer du den indirekta återförsäljare som du vill associera med kundens prenumerationer i listan.

5. Välj **Granska.**

6. Välj **Skicka**.

7. Om du vill lägga till prenumerationer väljer du **Lägg till produkter.**

8. När du är klar med att lägga till kundinformation och har köpt de prenumerationer som krävs väljer du **Klar.**

#### <a name="current-view"></a>[Aktuell vy](#tab/current-view)

1. Logga in på [instrumentpanelen i Partnercenter,](https://partner.microsoft.com/dashboard) **välj Kunder** och välj sedan Lägg **till kund.**

2. Om kunden är en utbildningsnämnd kan du se [hur du skapar en eduktionskund.](sell-to-education-customers.md)

3. På **sidan Kontoinformation** anger du kundens information och primär kontaktinformation.
   >[!IMPORTANT]
   >Partner måste intyga följande:
   >
   >Jag bekräftar att min organisation fungerar som en indirekt partner när jag väljer en återförsäljare och som direkt partner utan att välja en återförsäljare
   >
   >Jag bekräftar att jag inte säljer produkter som köpts i den här ordern till andra partner som är kopplade till min överordnade organisation

   >[!NOTE]
   >EU-/EFTA-lagar anger att partner som gör transaktioner i dessa länder måste deklarera ytterligare återförsäljare som är associerade med en transaktion. Följande regler gäller:
   >- En första återförsäljare måste väljas innan ytterligare återförsäljare
   >- Ytterligare återförsäljare har inte rätt till ytterligare incitament, erbjudanden osv.
   >- Ytterligare säljare som angetts verifieras för att säkerställa att rätt MPN-ID anges i förekommande fall och att återförsäljaren har signerat MPA.
   >- Upp till 5 ytterligare återförsäljare kan anges som en del av transaktionen 

4. Om du är en indirekt leverantör väljer du den indirekta återförsäljare som du vill associera med kundens prenumerationer i listan.

5. När du är klar med att ange den information som krävs väljer **du Nästa: Prenumerationer**.

6. På **sidan Prenumerationer** väljer du det eller de erbjudanden som kunden vill köpa från dig, anger antalet licenser och väljer sedan **Nästa: Granska.**

7. Kontrollera **att posterna** är korrekta på sidan Granska och välj sedan **Skicka**.

8. När du är klar med att lägga till kundinformation och har köpt de prenumerationer som krävs väljer du **Klar.**

* * *

## <a name="company-registration-id-and-phone-number-required-for-some-countries"></a>Företagsregistrerings-ID och telefonnummer som krävs för vissa länder

Partner för direktfakturering och indirekta leverantörer som lägger till poster för kunder i följande länder måste också ange företagets telefonnummer och registrerings-ID (kallas även organisationens INN):

IaA,JN, Brasilien, Judic, India,Arv,Jet, Kyrgyzstan,jiska,Jv,Jv, Ryssland, Sydafrika, Sydafrika, Sydkorea, Sydkorea, Sydkorea, Island, Förenade Arabemiraten, Bande, Bande och Vietnam

## <a name="company-name-and-email-characters-abbreviations-and-extensions"></a>Företagsnamn och e-posttecken, förkortningar och tillägg

Följande tabeller listar de objekt som anges i [avsnittet nya](#new-rules-for-company-name-and-email-address) regler ovan.

### <a name="table-of-special-characters"></a>Tabell med specialtecken

| Tecken. | Tecken. | Tecken. | Tecken. |
| ----- | ----- | -----| ----- |
| '~' | '-' |  '=' |  '_' |
|  '#' | '.' |  '%' |  '-' |
|  '+' |  ':' |  '^' |  '[' |
|  '$' |  '–' |  "&" |  ']' |
|  '@' |  '—' |  '*' |  '(' |
|  ',' |  ')' |  '”' |  '⟩' |
|  '`' |  "<" |  '!' |  '\\' |
|  '(' |  ">" |  '“' |  '/' |
|  ')' |  '{' |  '‘' |  '\|' |
|  '\' |  '}' |  '،' |  ':' |
|  ';' |  '⟨' |  '’' | '?' |
|  '”' |  '⟩' |  '\\' |  |


### <a name="table-of-abbreviations"></a>Tabell med förkortningar

| Abbr. | Abbr. | Abbr. | Abbr. |
| ----- | ----- | ----- | ----- |
|"c p a" | "pty" | "l. l. c." | "gmbh" |
| "c.p.a." | "pty ltd" | "l.l.c." | "mol" |
| "l.l.p." | "pte ltd" | " l l p" | "wll" |
| "c. p. a." | "privat begränsad" | "corp" | "lda" |
| "l. l. p." | "pvt" | "corporation" | "sarl" |
| " l l c" | "pvt ltd" | "inc" | "kft" |
| "corp." | "zrt" | "inkorporerat" | "ltd" |
| "llc." | "ooo" | "begränsad" | "ltd." |
| "llp." | "llp" | "llc" | "sdn vida"

### <a name="table-of-top-level-domain-extensions"></a>Tabell över toppnivådomäntillägg

| Ext.  | Ext.  | Ext.  | Ext. |
| ----- | ----- | ----- | ----- |
| .ac | .ba | .ca | .de |
| .ad | .bb | .cc | .js |
| .ae | .bd | .cd | .dk |
| .af | .be | .cf | .dm |
| .ag | .bf | .cg | .do |
| .ai | .bg | .ch | .dz |
| .al | .prost | .ci | .fm |
| .am | .bi | .ck | .fo |
| .an | .bj | .cl | .fr |
| .ao | .bl | .cm | .ga |
| .aq | .bm | .cn | .gb |
| .ar | .bn | .co | .ddr |
| .as | .bo | .cr | .ge |
| .at | .bq | .cu | .gf |
| .au | .br | .cv | .gg |
| .aw | .bs | .cw | .gh |
| .ax | .bt | .cx | .gi |
| .az | .fins | .cy | .gla |
| .ec | .bw | .mer | .gm |
| .ee | .by | .eu | .gn |
| .eg | .bz | .fi | .gp |
| .ye | .es | .fj | .gq |
| .er | .et | .fk | .gr |
| .gs | .gw | .hm | .ht |
| .gt | .mer | .hn | .hu |
| .gu | .hk | .hr | .id |
| .ie | .kz | .mo | .nz |
| .il | .la | .mp | .om |
| .im | .lb | .mq | .pa |
| .i | .lc | .mr | .pe |
| .io | .li | .ms | .pf |
| .iq | .lk | .mt | .pg |
| .ir | .lr | .mu | .ph |
| .is | .ls | .mv | .pk |
| .it | .lt | .megas | .pl |
| .je | .lu | .mx | .pm |
| .jm | .lv | .my | .pn |
| .jo | .ly | .mz | .pr |
| .jp | .ma | .na | .ps |
| .ke | .mc | .nc | .pt |
| .kg | .md | .ne | .pw |
| .kh | .me | .nf | .py |
| .ki | .mg | .ng | .qa |
| .km | .mg | .ni | .re |
| .kn | .mh | .nl | .ro |
| .kp | .mk | .no | .rs |
| .kr | .ml | .np | .ru |
| .kw | .mm | .nr | .rw |
| .ky | .mn | .nu | .sa |
| .sb | .tf | .vc | .中国 |
| .sc | .tg | .ve | .中國 |
| .sd | .th | .vg | .భారత్ |
| .se | .tj | .vi | .ලංකා |
| .sg | .tk | .vn | .ભારત |
| .sh | .tl | .vu | .भारतम् |
| .si | .tm | .wf | .भारत |
| .js | .tn | .ws | .भारोत |
| .sk | .to | .ಭಾರತ | .укр |
| .sl | .tp | .한국 | .香港 |
| .sm | .tr | .ଭାରତ | .台湾 |
| .sn | .tt | .ভাৰত | .台灣 |
| .so | .tv | .ভারত | .мон |
| .sr | .tw | .சிங்கப்பூர் | .tc |
| .ss | .tz | .sz | .td |
| .st | .ua | .বাংলা | .uz |
| .su | .ug | .қаз | .va |
| .sv | .uk | .срб | .мкд |
| .sx | .um | .бг | .ею |
| .sy | .us | .бел | Uy |
| .tc | .uz | .мкд |  |

## <a name="next-steps"></a>Nästa steg

- Mer information om vad du kan sälja till kunder via Molnlösningsleverantör-programmet finns [i Partnererbjudanden i Molnlösningsleverantör program](csp-offers.md).