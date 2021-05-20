---
title: Meddelanden april 2021
description: April 2021-meddelanden för Microsoft Partner Center, inklusive nya funktioner, kampanjer, erbjudanden, marknader eller ändringar i befintliga erbjudanden.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: brentserbus
ms.author: brserbus
ms.custom:
- announcement
- references_regions
ms.localizationpriority: high
ms.date: 04/29/2021
ms.openlocfilehash: 13b8ec9ddd82b38a265606809b8c39c07436e548
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 05/19/2021
ms.locfileid: "110150139"
---
# <a name="april-2021-announcements"></a>Meddelanden april 2021

Den här sidan innehåller meddelanden för Microsoft Partner Center för april 2021.

## <a name="readiness-updated-csp-customer-address-validation-api-going-live-in-june-testing-capability-now-available"></a><a name="10"></a>Beredskap: Uppdaterade VALIDERINGs-API:et för CSP-kundadresser live i juni; nu tillgänglig testfunktion

### <a name="categories"></a>Kategorier

- Datum: 2021-04-30
- Beredskap

### <a name="summary"></a>Sammanfattning

För att hjälpa partner och kunder att driva sin verksamhet baserat på förtroende kommer vi att bjuda in partner att testa ändringar i API:et validate address för alla länder över hela världen.

### <a name="impacted-audience"></a>Målgrupp som påverkas

CSP-direktfaktureringspartner och indirekta leverantörer som skapar nya eller uppdaterar befintliga kunders adressinformation

### <a name="details"></a>Information

Microsoft körs med förtroende. Vi strävar efter att tillhandahålla en kompatibel, säker och säker metod för validering av kundadresser för att kunna hantera kundprenumerationer i CSP-programmet. Från och med 31 mars 2021 har vi infört ändringar i API:et för valideringsadress. Vi bjuder in partner att testa API:et före livesändningen i slutet av juni 2021. 

Observera att dessa ändringar endast påverkar API:et för valideringsadress. API:er för att skapa kund och uppdatera faktureringsprofil påverkas inte. Även om den föreslagna adressen för närvarande inte behöver användas med API:et för att skapa kund rekommenderas det starkt.

Svaret returnerar något av följande statusmeddelanden:

| Status     | Beskrivning |    Antal föreslagna adresser som returneras |
|-------|---------------|-------------------|
|Verifierad leverans | Adressen är verifierad och kan skickas till. | Enkel |
|Verifierat | Adressen är verifierad. | Enkel |
|Interaktion krävs | Den föreslagna adressen har ändrats avsevärt och kräver användarbekräftelse. | Enkel |
|Gatuadress delvis | Den angivna gatuadressen är delvis och behöver mer information. | Multipel – högst tre |
|Delvis lokal | De angivna lokalerna (byggnummer, svitnummer och annat) är ofullständiga och behöver mer information. | Multipel – högst tre |
|Flera | Det finns flera fält som är partiella i adressen (inklusive delvis gatuadress och delvis lokal). | Multipel – högst tre |
|Ingen | Adressen är felaktig. | Ingen |
|Inte validerat | Adressen kunde inte skickas via valideringsprocessen. | Ingen |

Amerikanska postkoder returnerar ytterligare fyra siffror + bindestreck, till exempel 12345-6789.

### <a name="next-steps"></a>Nästa steg

- Mer detaljerad vägledning finns i den tekniska dokumentationen och vanliga frågor och svar [i](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/) den dedikerade partnersamlingen.
- Förbered för att införliva ändringarna med partnercenter-API:et och webbanvändarupplevelsen. 
- Dela ditt klient-ID för sandbox-miljön med ämnesexperten (Ali Firmwareki) som ska ingå i testresan, så att du kan börja förbereda dig för uppdateringen. 
- Om du använder en CPV-lösning (Kontrollpanelens leverantör) kan du kontakta din CPV.

### <a name="questions"></a>Har du några frågor?

Om du behöver support för din verksamhet med Microsoft kan du kontakta din partnersupport i Yammer-gruppen eller öppna en [tjänstbegäran.](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=aa679372-d996-73df-e244-cb28bbbf28e8)

_______________
## <a name="new-location-for-partner-center-api-swagger-documentation"></a><a name="9"></a>Ny plats för Swagger-dokumentation för Partner Center API

### <a name="categories"></a>Kategorier

- Datum: 2021-04-26
- Funktioner

### <a name="summary"></a>Sammanfattning

Partner Center API Swagger-dokument har migrerats från den [tidigare Webbplatsen för Swagger-dokumentation](https://apidocs.microsoft.com/services/partnercenter) till en [ny webbplats för Swagger-dokumentation.](/rest/api/partner-center-rest/)

### <a name="impacted-audience"></a>Målgrupp som påverkas

Direktfaktureringspartner och indirekta leverantörer som deltar i Molnlösningsleverantör-programmet (CSP) som använder Partner Center-API:er

### <a name="details"></a>Information

Från och med 26 april 2021 finns Partner Center API Swagger-dokumentationen, inklusive Rest API-innehåll, på en [ny webbplats.](/rest/api/partner-center-rest/) Den gamla platsen kommer inte att vara tillgänglig efter flera veckor.

### <a name="benefits"></a>Fördelar

Swagger-dokumentationen för Partnercenter-API:et innehåller **en Try It-funktion.** Om du vill använda den här funktionen måste du ha en bearer-token som du kan generera genom att följa stegen i [Partner Center-autentisering.](/partner-center/develop/partner-center-authentication#app--user-authentication)

### <a name="next-steps"></a>Nästa steg

Dela den här informationen i din organisation så att rätt team kan granska och uppdatera sina processer.

### <a name="questions"></a>Har du några frågor?

Frågor om dessa erbjudanden finns i dina relevanta Yammer-communities.

________________
## <a name="cloud-solution-provider-csp-software-return-period-policy-and-download-link-expiry-notice"></a><a name="8"></a>Molnlösningsleverantör princip för programvarureturperiod (CSP) och förfallomeddelande om nedladdningslänk

### <a name="categories"></a>Kategorier

- Datum: 2021-04-21
- Funktioner

### <a name="summary"></a>Sammanfattning

Det finns ändringar i CSP-principen för programvarureturperiod och nedladdningslänkens upphörande.

### <a name="impacted-audience"></a>Målgrupp som påverkas

Partner som gör en löpande programvaru- eller programvaruprenumeration i CSP

### <a name="details"></a>Information

Observera följande viktiga meddelanden om kontinuerliga programvaru- och programvaruprenumerationsköp via Partnercenter:

#### <a name="software-return-period-policy"></a>Princip för programvarureturperiod

Från och med 1 juni 2021 ändras returperioden för programvaruerbjudanden i CSP enligt vad som anges i Microsoft-partneravtal (MPA) från 60 dagar från orderdatumet till 30 dagar från orderdatumet.

När en order för ett programvaruerbjudande har skickats har partnern 30 dagar från orderdatumet för att skicka ändringar i en sådan order:

- Alla permanent programvarulicens som returneras inom 30-dagars returperiod får en fullständig kredit av det betalda inköpspriset.

- Alla produkter för programvaruprenumeration som returneras inom 30-dagars returperioden får en jämförd kredit på det betalda inköpspriset.

Det här meddelandet är en uppföljning av vår e-postkommunikation som skickades december 2020 och april 2021 till alla CSP-partner angående returperioden och andra uppdateringar av MPA. Se dessa meddelanden för fullständig information om ändringar som påverkar MPA.

#### <a name="software-download-link-expiry"></a>Länk för nedladdning av programvara upphör att gälla

Från och med 3 juni 2021 har nedladdningslänkarna för programvara för permanenta produktköp av programvara och programvaruprenumeration via Partnercenter ett förfallodatum på fem dagar från den första nedladdningen. Förfalloperioden gäller för alla inköp före 3 juni 2021, samt den 3 juni 2021 eller senare.

### <a name="next-steps"></a>Nästa steg

Granska [CSP-returperioden och vanliga frågor och](https://partner.microsoft.com/resources/detail/csp-software-return-period-download-expiry-faq-pdf)svar om att nedladdningslänken upphör att gälla och informera alla lämpliga team i din organisation om dessa ändringar:

### <a name="questions"></a>Har du några frågor?

Frågor om dessa erbjudanden finns i dina relevanta Yammer-communities.

________________
## <a name="open-licensing-program-transitioning-resellers-to-the-cloud-solution-provider-csp-program"></a><a name="7"></a>Open Licensing Program: Övergång av återförsäljare till Molnlösningsleverantör (CSP)

### <a name="categories"></a>Kategorier

- Datum: 2021-04-19
- Utveckla din verksamhet

### <a name="summary"></a>Sammanfattning

Den här kommunikationen beskriver hur du förbereder dig för de ändringar som snart kommer till Open Licensing-programmet.

### <a name="impacted-audience"></a>Påverkad målgrupp

CSP- och Open License-partner

### <a name="details"></a>Information

2020 meddelade [Microsoft](https://blogs.partner.microsoft.com/mpn/general-availability-of-perpetual-software-licenses-in-the-cloud-solution-provider-program/) att permanenta programvarulicenser kommer att vara allmänt tillgängliga för partner och kunder via programmet Molnlösningsleverantör (CSP). Den första milstolpen nåddes i januari 2021, när kommersiella permanenta programvaruerbjudanden blev tillgängliga. Nästa viktiga milstolpe sker i juli 2021 när erbjudanden [inom den offentliga sektorn](https://aka.ms/openlicensepublicsector) blir tillgängliga. Vi har [också](https://blogs.partner.microsoft.com/mpn/expanding-opportunities-for-partners-in-the-cloud-solution-provider-program/) meddelat att från och med den 1 januari 2022 kan inga nya köp eller förnyelser av Software Assurance eller onlinetjänster göras via Open License-programmet.

Övergången av permanent programvara till CSP-programmet i den nya handelsupplevelsen hjälper partner att utöka möjligheterna att erbjuda olika lösningar och hanterade tjänster. Detta påskyndar även kundernas övergång till molnet.  För att säkerställa en smidig övergång för både våra partner och kunder har vi gjort dessa justeringar och material för att påskynda den här digitala omvandlingen:

#### <a name="april-2021"></a>April 2021

[Nu tillgängligt:](https://partner.microsoft.com/resources/collection/reseller-open-license-to-csp-transition-materials#/)Open License-to-CSP transition materials for resellers (Öppna övergångsmaterial för licens till CSP för återförsäljare)

#### <a name="july-2021"></a>Juli 2021

##### <a name="csp"></a>CSP

- 1 juli: Beständiga programvarulicenser som är tillgängliga för kunder inom den offentliga sektorn

- 7 juli: Visual Studio Pro och Skaffa äkta Windows-avtal beständiga programvarulicenser som är tillgängliga för alla segment

##### <a name="open-value"></a>Öppet värde

- 1 juli: Ytterligare SKU:er är tillgängliga i Open Value-programmet för utbildning och ideell verksamhet, vilket ger liknande erbjudanden som Open License-programmet

##### <a name="open-license"></a>Öppna licens

- 1 juli: Microsoft kommer inte längre att lansera nya erbjudanden i Open License-programmet.

#### <a name="january-2022"></a>Januari 2022

- 1 januari: Inga nya köp eller förnyelser kan göras via Open License-programmet

### <a name="next-steps"></a>Nästa steg

#### <a name="csp-indirect-providers"></a>Indirekta CSP-leverantörer

Använd de kommande månaderna för att hjälpa Open License-återförsäljare att få en orientering i CSP-programmet genom att delta i partner-community-evenemang och använda övergångsmaterial för öppen licens till CSP för återförsäljare:

- [Öppna övergångsmaterial för licens-till-CSP](https://partner.microsoft.com/resources/collection/reseller-open-license-to-csp-transition-materials#/)för återförsäljare – anpassningsbar översiktspresentation, e-postmall, introduktionsguide för indirekt CSP-återförsäljare med mera som hjälper dig att införa dina återförsäljare i stor skala.

- [CSP Partner Community Events](https://globalpbocomm.eventbuilder.com/GlobalCSP) som värdar för Microsoft Business Operations.  Delta i de olika sessionerna för att lära dig grunderna i CSP (CSP Fundamentals) eller håll dig uppdaterad och ställ frågor om programvara i CSP (Q&A Sessions).

- (Kommer snart) Utbildningssession som fokuserar på indirekt CSP-återförsäljare som värd för Microsoft Business Operations.

#### <a name="open-license-resellers"></a>Öppna licensåterförsäljare

- Om din organisation inte är registrerad i CSP-programmet kontaktar du återförsäljaren för information om hur du kommer igång. Anslut med en indirekt leverantör [här.](https://partner.microsoft.com/membership/cloud-solution-provider/find-a-provider)

- Om din organisation redan har registrerats i CSP-programmet kan du läsa mer om permanent programvara i CSP [här.](https://partner.microsoft.com/resources/collection/software-in-csp)

### <a name="questions"></a>Har du några frågor?

Mer information om dessa erbjudanden finns i dina relevanta Yammer-communities.

________________
## <a name="now-live-global-promo-readiness-guide"></a><a name="6"></a>Nu live: Guide för global kampanjberedskap

### <a name="categories"></a>Kategorier

- Datum: 2021-04-16
- Funktioner

### <a name="summary"></a>Sammanfattning

Launch Readiness har publicerat en ny [global guide för kampanjberedskap](https://partner.microsoft.com/resources/detail/operations-promo-guide-pdf) i resursgalleriet för driftberedskap. Den här guiden innehåller en samlad vy över alla aktiva [globala kampanjer.](https://partner.microsoft.com/resources/collection/global-promo-readiness-guide-collection#/)

### <a name="impacted-audience"></a>Påverkad målgrupp

Alla partner för volymlicensiering (VL), Dynamics Price List (DPL) Molnlösningsleverantör (CSP)

### <a name="details"></a>Information

Microsoft-partner har delat med oss om behovet av att tillhandahålla en samlad vy över alla globala kampanjer med kompletterande information. Du ville ha den här konsoliderade guiden för att hjälpa dig att använda kampanjer med tillförsikt att all tillgänglig information är lättillgänglig på en central och praktisk plats.

Från och med april 2021 uppdaterar Microsoft den här guiden månadsvis, och den kommer att vara tillgänglig i en dedikerad samling global kampanjberedskapsguide i resursgalleriet för driftberedskap.

Länkar till den här guiden kommer också att ingå i följande samlingar:

- [Starta kalendersamlingen](https://partner.microsoft.com/resources/collection/csp-announcement-calendar#/), som ger en centraliserad vy över kommande ändringar och uppskjutningar.

- [Community-samlingar](https://partner.microsoft.com/resources/collection/april-2021-csp-partner-community-content#/), som innehåller stödmaterial för våra månatliga partnersamtal, med fokus på kommande ändringar och aktuella ämnen av drifts intresse.

- [Partnerns nyhetsbrev,](https://partner.microsoft.com/resources/collection/csp-monthly-update#/)till exempel månadsuppdatering för CSP

Som en månatlig påminnelse kommer vi också att publicera ett Partnercenter-meddelande med varje nytt ärende i guiden för global kampanjberedskap.

### <a name="next-steps"></a>Nästa steg

I början av varje månad hittar du den senaste guiden för global [kampanjberedskap](https://partner.microsoft.com/resources/detail/operations-promo-guide-pdf) i [resursgalleriet för driftberedskap.](https://partner.microsoft.com/resources)

Dela den här informationen med lämpliga kontakter i din organisation och berätta för oss hur användbar guiden är via "Var den här sidan användbar?" i slutet av varje sida.

________________
## <a name="april-cloud-solution-provider-csp-community-update-and-reminders"></a><a name="5"></a>Community-Molnlösningsleverantör för April Molnlösningsleverantör (CSP) och påminnelser

### <a name="categories"></a>Kategorier

- Datum: 2021-04-16
- Community-| Inbjudningar och påminnelser

### <a name="summary"></a>Sammanfattning

CSP-communityresurser är tillgängliga på begäran och uppdateras varje månad för att hålla dig informerad och förberedd för ändringar i CSP-programmet.

### <a name="impacted-audience"></a>Målgrupp som påverkas

CSP-direktfaktureringspartner och indirekta leverantörer

### <a name="details"></a>Information

Den här månaden innehåller resurserna följande viktiga ämnen:

- [Uppdatera till utveckling av CSP-program och ändringar i Open License-programmet](https://partner.microsoft.com/resources/collection/csp-open-evolution-to-a-better-experience#/)

- [Ändringar av CSP-kunders registreringskrav i vissa regioner](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/)

- [Nytt format för den nya PDF-fakturan för handel i CSP-programmet](https://partner.microsoft.com/resources/collection/introducing-new-format-for-the-new-commerce-invoice-in-csp#/)

I [CSP-communitysamlingen](https://partner.microsoft.com/resources/collection/april-2021-csp-partner-community-content#/)hittar du:

- Det nedladdningsbara [nyhetsbrevet CSP Monthly Update](https://partner.microsoft.com/resources/detail/csp-monthly-update-april-2021-global), som sammanställer de senaste CSP-meddelandena, uppdateringarna, händelserna och påminnelserna i ett lättläst dokument.

- [CSP-meddelande kalender](https://partner.microsoft.com/resources/detail/csp-announcement-calendar-april-2021), som ger en tidslinjevy över kommande ändringar som påverkar programmet.

- Den nya [kalendern för produktlansering,](https://partner.microsoft.com/resources/detail/product-launch-calendar-april-pdf)där du kan se kommande produktlanseringar och erbjudanden.

- [CSP startar uppdateringsresurser](https://partner.microsoft.com/resources/collection/april-2021-csp-launch-topics-collection#/) med lätt att använda innehåll om viktiga operativa ändringar.

- [Uppdaterare och påminnelser om](https://partner.microsoft.com/resources/detail/csp-april-2021-refreshers-and-reminders-pdf) viktiga CSP-ämnen som tar emot intresse och frågor.

#### <a name="csp-community-call-qas"></a>CSP Community Call Q&As

Community Call Q&As are available to help you with questions related to upcoming changes. Registrera dig nu för CSP Community Call Q&As som äger rum i april, maj och juni. Dessa fokuserar på de senaste uppskjutningar, viktiga uppdateringsuppdateringar och påminnelser.

[Registrera dig här.](https://globalpbocomm.eventbuilder.com/GlobalCSP)

### <a name="next-steps"></a>Nästa steg

Granska communityresurserna och registrera dig för Community Call Q&A.

För att säkerställa att du får ut mesta av Community Call Q&A granskar du communityinnehållet på begäran och skickar dina frågor upp till 48 timmar före samtalet.

### <a name="questions"></a>Har du några frågor?

Det månatliga CSP Community Call Q&A är den bästa platsen för frågor som rör ändringar i CSP-programmet. Granska materialet varje månad och skicka dina frågor i förväg så att vi kan ägna sessionen åt de ämnen som är viktigast för dig.

Kontakta supporten för [mer information.](https://partner.microsoft.com/dashboard/support/csp/servicerequests/create?category=csp)

________________
## <a name="final-reminder-deprecation-of-get-qualification-on-may-6-2021"></a><a name="4"></a>Sista påminnelse: Utfasning av GET-kvalificering den 6 maj 2021

### <a name="categories"></a>Kategorier

- Datum: 2021-05-04

- Funktioner

### <a name="impacted-audience"></a>Påverkad målgrupp

Partner som säljer erbjudanden för Academic, Nonprofit och Government Community Cloud (GCC) via Molnlösningsleverantör-programmet med partnercenter-API:et

### <a name="details"></a>Information

Det här meddelandet är en uppföljning av partnercenterförbättringarna [som släpptes i december](./2020-december.md#1). Som en del av den versionen distribuerades nya GET- och POST-kvalificerings-API:er och därför kommer den befintliga GET-kvalificeringen att dras tillbaka den 6 maj **2021.** Då måste du ha gått över till att använda de nya POST Partner Center-API:erna. Med de nya POST-API:erna kan du köpa Education-erbjudanden, medan de nya GET-API:erna gör att du kan köpa förkvalificerade erbjudanden för ideella organisationer och GCC.

### <a name="next-steps"></a>Nästa steg

- **Uppdatera till de nya API:erna** för en lyckad övergång i rätt tid.

- **Granska de nya partnercenter-API-ändringarna och guiden** i resurserna för driftberedskap: [Förbättringar av kundvalideringsprocessen i PartnerCenter Education.](https://partner.microsoft.com/resources/collection/partner-center-edu-validation-enhancements#/)

- Dela den här informationen med lämpliga team i din organisation och med dina återförsäljare för att hjälpa dem att förbereda sig för dessa ändringar.

### <a name="questions"></a>Har du några frågor?

Om du har frågor om det här meddelandet kontaktar du [supporten för Partnercenter.](https://partner.microsoft.com/dashboard/support/referrals/servicerequests?category=referrals)

### <a name="change-log"></a>Ändringslogg

- 4 maj 2021: Sista påminnelsen om kommande utfasning av GET-kvalificering

- 9 april 2021: Påminnelse om kommande utfasning av GET-kvalificering 

- Februari: Uppdaterade tidslinjer för utfasning av GET & PUT-kvalificeringar

- Januari: Påminnelse om kommande utfasningar av GET & PUT-kvalificeringar

________________
## <a name="new-format-for-the-new-commerce-pdf-invoice-in-csp"></a><a name="3"></a>Nytt format för den nya PDF-fakturan för handel i CSP

### <a name="categories"></a>Kategorier

- Datum: 2021-04-05
- Funktioner

### <a name="summary"></a>Sammanfattning

Microsoft introducerar ett nytt format för den nya PDF-fakturan för handel i programmet Molnlösningsleverantör (CSP) för att visa faktureringsinformation efter produktinformation i stället för SKU-beskrivning.

### <a name="impacted-audience"></a>Målgrupp som påverkas

Partner som gör en överträdelse via CSP-programmet

### <a name="details"></a>Information

Från och med maj 2021 introducerar Microsoft ett nytt format för den nya PDF-fakturan för handel i CSP-programmet för att visa faktureringsinformation efter produktinformation i stället för SKU-beskrivning. Med den här nya uppdateringen kommer vi att aggregera radobjekten efter produkttyp samtidigt som vi visar varje produkt på en enskild rad.

Partner kommer att märka att ändringen börjar gälla på fakturan för maj för faktureringsperioden mellan den 1 april 2021 och den 30 april 2021. De berörda erbjudandena är Microsoft Azure Reserverad instans, Azure-prenumerationer (Azure-plan) och Marketplace.

Eventuella begäranden om kreditrefakturering som görs efter att fakturaformatet har uppdaterats genereras i det nya formatet.

#### <a name="partner-benefits"></a>Partnerförmåner

Den här uppdateringen kommer att erbjuda följande förbättringar av faktureringsupplevelsen för partner:

- Minskad fakturastorlek samtidigt som kritiska data bevaras

- Anpassning av formatet till branschstandarderna för kompakta och användarvänliga fakturor 

Följande element påverkas inte:

- Sidan med faktureringssammanfattning i PDF-filen med faktura

- Befintliga fakturerings-API:er

- Avstämningsfiler (rekognoseringsfiler kan användas för att hämta detaljerade data.) 

- Fakturor för användnings- och licensbaserade avgifter

### <a name="next-steps"></a>Nästa steg

Granska informationen om det här avsnittet i [resursgalleriet för driftberedskap](https://partner.microsoft.com/resources/collection/introducing-new-format-for-the-new-commerce-invoice-in-csp#/) på Microsofts partnerwebbplats. Mer information om fakturerings- och skatteämnen som faktureringsresurser, fakturor, CSP-fakturering och skatter finns i [avsnittet Fakturering](../billing.md) i Partnercenter.

________________
## <a name="changes-to-the-cloud-solution-provider-csp-customer-onboarding-requirements"></a><a name="2"></a>Ändringar i CSP Molnlösningsleverantör-kundernas registreringskrav

### <a name="categories"></a>Kategorier

- Datum: 2021-04-02
- Erbjudanden/marknader

### <a name="summary"></a>Sammanfattning

Som en del av vårt åtagande att hjälpa partner och kunder att driva sin verksamhet baserat på förtroende begär vi ytterligare kundinformation från och med den 25 mars 2021.

### <a name="impacted-audience"></a>Påverkad målgrupp

CSP:s direktfaktureringspartner och indirekta leverantörer som har nya eller befintliga kunder i de länder som anges i nästa avsnitt

### <a name="details"></a>Information

Microsoft körs med förtroende. Vi strävar efter att tillhandahålla en kompatibel, säker och säker metod för kundvalidering för att omvandla kundprenumerationer i CSP-programmet. Den 25 mars 2021 introducerar vi förbättringar av Partner Center API och användargränssnitt som påverkar partner som uppfyller båda följande kriterier:

- Partnern har en direkt faktureringsrelation med Microsoft (vilket innebär att partnern antingen är en partner för direktfakturering eller en indirekt leverantör).

- Partnern gör affärer med nya eller befintliga kunder i följande länder:

    - Thailand
    - Vietnam
    - Turkiet
    - Polen
    - Sydafrika
    - Indien
    - Brasilien
    - Irak
    - Myanmar
    - Sydsudan
    - Saudiarabien
    - Förenade Arabemiraten
    - Venezuela

Partner som uppfyller villkoren måste skicka en kunds företagsregistrerings-ID (kallas även kundens organisation INN) och telefonnummer nästa gång de uppdaterar eller skapar en prenumeration för kunden. Dessa partner kan också ange ett mellannamn för kunden (valfritt).

Observera att när du lägger till ditt företagsregistrerings-ID bör du använda ditt företags skatte-ID och inte kundens personliga ID.

Partner som gör affärer med nya eller befintliga kunder i följande länder har redan introducerats med en tidigare version i november 2020.

- Armenien
- Azerbajdzjan
- Vitryssland
- Ungern
- Kazakstan
- Kirgizistan
- Moldavien
- Ryssland
- Tadzjikistan
- Ukraina
- Uzbekistan

Partner med kunder i resten av världen kommer att ha möjlighet i slutet av mars 2021 att ange företagets registrerings-ID, telefonnummer och mellannamn för kunder som valfri information.

### <a name="next-steps"></a>Nästa steg

- Mer detaljerad vägledning finns i den tekniska dokumentationen och vanliga frågor [och svar i](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/) den dedikerade partnersamlingen.
- Förbered för att införliva ändringarna med partnercenter-API:et och webbanvändarupplevelsen. API/SDK:er kommer att vara tillgängliga för testning.
- Se till att skicka in ytterligare data när du registrera nya kunder eller ändrar befintlig kundinformation.
- Om du använder en CPV-lösning (Kontrollpanelen) bör du kontakta din CPV.

### <a name="questions"></a>Har du några frågor?

Kontakta skatterådgivaren eller det lokala skattekontoret om du har frågor som rör id:t för företagsregistrering (kallas även INN eller TIN). Microsoft kan inte ge vägledning om skattefrågor.

Om du behöver support för dina åtgärder med Microsoft öppnar du en [tjänstbegäran.](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=aa679372-d996-73df-e244-cb28bbbf28e8)

## <a name="view-this-months-product-launches-and-offers"></a><a name="1"></a>Visa den här månadens produktlanseringar och erbjudanden

### <a name="categories"></a>Kategorier

- Datum: 2021-04-01
- Funktioner
 
### <a name="summary"></a>Sammanfattning

Produktlanserings kalender för april 2021 publiceras nu.

### <a name="impacted-audience"></a>Målgrupp som påverkas

Alla partner som gör en Molnlösningsleverantör (CSP)

### <a name="details"></a>Information

Kalendern för april [2021-produktlansering](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) är nu tillgänglig i resursgalleriet för driftberedskap. Visa kommande produktlanseringar och erbjudanden här.

### <a name="next-steps"></a>Nästa steg

Granska kalendern [för produktlansering](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/)och dela informationen med lämpliga intressenter i din organisation.  

### <a name="questions"></a>Har du några frågor?

Om du vill ha fler frågor om dessa erbjudanden kan du läsa dina relevanta Yammer-communities.