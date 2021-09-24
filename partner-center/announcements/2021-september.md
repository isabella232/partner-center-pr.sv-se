---
title: Meddelanden september 2021
description: September 2021-meddelanden för Microsoft Partner Center, inklusive nya funktioner, kampanjer, erbjudanden, marknader eller ändringar i befintliga erbjudanden.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-announcements
author: brentserbus
ms.author: brserbus
ms.custom:
- announcement
- references_regions
ms.localizationpriority: high
ms.date: 09/20/2021
ms.openlocfilehash: 51706ec685519ea297e851cb4f2b862b96db3da1
ms.sourcegitcommit: fceaca54b0ec695cf214209c09b4516e1b40866a
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/24/2021
ms.locfileid: "128373429"
---
# <a name="september-2021-announcements"></a>Meddelanden september 2021

Den här sidan innehåller meddelanden för Microsoft Partner Center för september 2021.

________________

## <a name="product-keys-available-for-business-central-for-dual-use-rights"></a><a name="13"></a> Produktnycklar som är tillgängliga för Business Central för dubbla användningsrättigheter

### <a name="categories"></a>Kategorier

- Datum: 2021-09-23
- Funktioner

### <a name="summary"></a>Sammanfattning

Från och med 23 september 2021 kommer produktnycklar för den lokala versionen av Business Central för dubbla användningsrättigheter att vara tillgängliga för kunder via Administrationscenter för Microsoft 365.

### <a name="impacted-audience"></a>Målgrupp som påverkas

CSP-partner

### <a name="details"></a>Information

Från och med 23 september 2021 kommer produktnycklar för den lokala versionen av Business Central för dubbel användning att vara tillgängliga i Partner Source Business Center (PSBC). Kunder kan själv betjäna organisationens produktnycklar via Administrationscenter för Microsoft 365.

Det finns inga ändringar i orderprocessen eller processen för att uppfylla ändringar i landskoden.

### <a name="next-steps"></a>Nästa steg

- Granska resurserna om det här ämnet och dela med lämpliga intressenter i din organisation.  
- Se till att din organisation och dina kundorganisationer är bekanta med den här ändringen.
- Om du inte är bekant med hur du laddar ned produktnycklar kan du läsa [Ladda ned permanent programvara och produktlicensnycklar.](/microsoft-365/admin/setup/download-software-licenses-csp?view=o365-worldwide)
- Granska den uppdaterade processen för att uppfylla licenser för dubbel användning för Dynamics [i samlingen Dynamics 365 Business Central Dual Use Rights Resources](https://partner.microsoft.com/resources/collection/dynamics-365-business-central-dual-use-rights-resources#/).

### <a name="questions"></a>Har du några frågor?

Om du har frågor om dessa erbjudanden kan du kontrollera dina Yammer communityn.

________________

## <a name="reminder-introducing-api-throttling-to-partners-calling-partner-center-apis"></a><a name="12"></a>Påminnelse: Introduktion till API-begränsning för partner som anropar Partner Center-API:er

### <a name="summary"></a>Sammanfattning

Från och med oktober 2021 implementerar Microsoft API-begränsning för partner som anropar Partner Center-API:er.

### <a name="categories"></a>Kategorier

- Datum: 2021-09-21
- Funktioner

### <a name="impacted-audience"></a>Målgrupp som påverkas

Partner som gör en Molnlösningsleverantör program  

### <a name="details"></a>Information

Från oktober 2021 implementerar Microsoft API-begränsning för en mer konsekvent prestanda inom ett tidsintervall för partner som anropar Partner Center-API:erna.För att förhindra överanvändning av resurser begränsar begränsningen antalet begäranden till en tjänst under ett tidsintervall.När ett tröskelvärde för begränsning överskrids begränsar PartnerCenter eventuella ytterligare begäranden från klienten under en viss tidsperiod.
  
#### <a name="partner-benefits"></a>Partnerförmåner

Partnercenter är utformat för att hantera ett stort antal begäranden, men om ett överväldigande antal begäranden inträffar hjälper begränsningen till att upprätthålla optimala prestanda och tillförlitlighet för alla partner.

Här är några av fördelarna:

- Begränsning säkerställer minimal avbrottstid.
- Genom att minska begäranden med stora volymer kan vi säkerställa konsekventa prestanda för alla partner.  

#### <a name="apis-to-be-throttled"></a>API:er som ska begränsas

| Åtgärd | Dokumentation för Partnercenter |
| ----------- | ---------------------- |
| Hämta v1/customers/{customer_id}/users/{user_id}/licenses | [Hämta licenser tilldelade till en användare](/partner-center/develop/check-which-licenses-are-assigned-to-a-user) |
| Hämta /v1/customers/{customer_id}/subscribedskus | [Hämta en lista över tillgängliga licenser](/partner-center/develop/get-a-list-of-available-licenses) |
| Hämta /v1/customers/{customer_id}/berättiganden | [Hämta en samling berättiganden](/partner-center/develop/get-a-collection-of-entitlements) |
| Hämta /v1/customers/{customer_id}/artifacts/{artifact_type}<br>/groups/{group_id}/lineItems/{lineitem_id}<br>/resource/{resource_id} | [Hämta en samling berättiganden](/partner-center/develop/get-a-collection-of-entitlements#retrieve-reservation-details-from-an-entitlement-by-using-sdk-v19) |
| Hämta /v1/customers/{customer_id}/users/{use<br>r_id}/directoryroles | [Hämta användarroller för en kund](/partner-center/develop/get-user-roles-for-a-customer) |

Vi rekommenderar att du överväger att använda aktivitetslogg-API:et för att öka effektiviteten och undvika begränsningar. Mer information om den här funktionen finns i informationen [här.](/partner-center/develop/api-throttling-guidance)  

### <a name="next-steps"></a>Nästa steg

Granska resurserna [för](/partner-center/develop/api-throttling-guidance) det här avsnittet och vidta nödvändiga åtgärder.

### <a name="change-log"></a>Ändringslogg

- 21 september: Påminnelse om kommande ändringar
- 19 juli: Ursprungligt meddelande

________________

## <a name="coming-soon-delegated-administrative-privileges-monitoring-and-self-service-removal"></a><a name="11"></a> Kommer snart: Övervakning av delegerade administrativa privilegier och borttagning av självbetjäning

### <a name="categories"></a>Kategorier

- Datum: 2021-14-10
- Funktioner

### <a name="summary"></a>Sammanfattning

Microsoft lanserar nya rapporteringsverktyg som visar DAP-anslutningar (active delegated administrative privileges) så att partner kan inaktivera oanvända DAP-anslutningar.

### <a name="impacted-audience"></a>Målgrupp som påverkas

Direktfaktureringspartner, indirekta leverantörer och indirekta återförsäljare som gör transaktioner via Molnlösningsleverantör program

### <a name="details"></a>Information

Partner kan använda delegerade administratörsbehörigheter (DAP) för att hantera och stödja sina kunders tjänster.

För att förbättra säkerheten i partner- och kundekosystemet rekommenderar Microsoft att du inaktiverar DAP när det inte används.

Från och med slutet av oktober lanserar Microsoft nya rapporteringsverktyg så att partneradministrationsagenter kan granska DAP-anslutningar med sina kunder. Den här rapporteringen visar hur partneragenter kommer åt kundklienter i alla klienter via DAP. Partner kan sedan granska och ta bort DAP-anslutningar som inte används.

Om du vill veta mer om den här nya rapporteringsfunktionen har vi skapat en [guide](https://partner.microsoft.com/resources/detail/dap-monitoring-and-self-serve-removal-pdf) som dokumenterar de olika filter och fält som är tillgängliga i rapporten.

#### <a name="key-considerations"></a>Viktiga överväganden

- Om du inaktiverar DAP-åtkomst för en kund inaktiveras partnerns administratörsbehörighet för att hantera funktioner i kundens klientorganisation.  
- Transacting-partner kan fortsätta att göra beställningar åt sina kunder.
- Partneragenter kan inte längre skapa en supportbiljett för sina kunder till Microsoft.  
- Att inaktivera DAP påverkar inte aktuella rollbaserade åtkomstkontrollroller i en prenumeration och påverkar inte partner-intjänade krediter.

### <a name="next-steps"></a>Nästa steg

Granska resurserna [om](https://partner.microsoft.com/resources/collection/delegated-administrative-privileges-dap#/) det här avsnittet och dela med lämpliga intressenter i din organisation.

## <a name="september-cloud-solution-provider-community-update-and-reminders"></a><a name="10"></a>Uppdatering Molnlösningsleverantör community och påminnelser i september

### <a name="categories"></a>Kategorier

- Datum: 2021-9-10
- Community-| Kapacitet

### <a name="summary"></a>Sammanfattning

Det [Molnlösningsleverantör månadsuppdateringsbrevet (CSP)](https://partner.microsoft.com/resources/detail/csp-monthly-update-september-2021-global) är nu tillgängligt, tillsammans med ytterligare [CSP-communityresurser](https://partner.microsoft.com/resources/collection/september-2021-csp-partner-community-content#/) som ger dig viktiga programuppdateringar.

### <a name="impacted-audience"></a>Målgrupp som påverkas

CSP-direktfaktureringspartner och indirekta leverantörer

### <a name="details"></a>Information

Den här månadens resurser täcker följande ämnen:

#### <a name="launches"></a>Lanserar

- [Microsoft Dynamics 365, Microsoft 365, Microsoft Power Platform och Windows 365 i den nya handelsupplevelsen i CSP](https://partner.microsoft.com/resources/detail/d365-m365-power-platform-w365-in-the-new-commerce-experience-in-csp-pdf)

#### <a name="clinics"></a>Kliniker

- [Introduktion till licensieringsstöd för partner](https://partner.microsoft.com/resources/detail/introduction-to-licensing-support-for-partners-pdf)
- [Guide till webbplatsen för produktvillkor för partner](https://partner.microsoft.com/resources/detail/product-terms-site-guide-for-partners-pdf)
- [Så här rapporterar du ett supportbedrägeri](https://partner.microsoft.com/resources/detail/how-to-report-a-support-scam-pdf)
- [Ändring av programattribut för Microsoft 365-applikationer för företag](https://partner.microsoft.com/resources/detail/program-attribute-change-for-microsoft-365-apps-for-enterprise-pdf)

#### <a name="csp-community-qa-reminder"></a>CSP Community Q&A reminder

Den månatliga CSP-communityn Q&A-session ger dig möjlighet att lära dig mer och ställa frågor om ändringar som påverkar programmet. Den här månadens anrop fokuserar på ämnena som anges i föregående avsnitt och mycket mer.

[Registrera dig här för att ansluta till anropet](https://globalpbocomm.eventbuilder.com/GlobalCSP).

#### <a name="always-availablelaunch-content-on-demand"></a>Alltid tillgängligt – Starta innehåll på begäran

I den månatliga [CSP-communitysamlingen](https://partner.microsoft.com/resources/collection/september-2021-csp-partner-community-content#/)hittar du:

- Det nedladdningsbara [nyhetsbrevet CSP Monthly Update](https://partner.microsoft.com/resources/detail/csp-monthly-update-september-2021-global) som sammanställer de senaste CSP-meddelandena, uppdateringarna, händelserna och påminnelserna i ett lättläst dokument.
- [CSP-meddelande kalender som](https://partner.microsoft.com/resources/detail/csp-announcement-calendar-september-2021-pdf) ger en tidslinje för kommande ändringar som påverkar programmet.
- Den **nya** [kalendern för produktlansering](https://partner.microsoft.com/resources/detail/product-launch-calendar-september-pdf) där du kan se kommande produktlanseringar och erbjudanden.
- Guiden [för global kampanjberedskap](https://partner.microsoft.com/resources/collection/global-promo-readiness-guide-collection#/) som samlar de senaste och kommande kampanjerna som är tillgängliga för partner och kunder.
- [CSP startar uppdateringsresurser](https://partner.microsoft.com/resources/collection/csp-launch-topics-collection#/) med lätt att använda innehåll om viktiga operativa ändringar.
- [Uppdaterare och påminnelser om](https://partner.microsoft.com/resources/detail/csp-september-2021-refreshers-and-reminders-pdf) viktiga CSP-ämnen som tar emot intresse och frågor.

Behöver du licensberedskap? [Webbseminor om månatliga CSP-spotlight-webbseminor](https://commercial_licensing.eventbuilder.com/YearToDate_ALL) täcker den senaste CSP-licensieringsinformationen som är tillgänglig för alla partner.

### <a name="next-steps"></a>Nästa steg

Granska community-resurserna och registrera dig för Q&A community-anropet.

### <a name="questions"></a>Har du några frågor?

Det månatliga CSP-communityn Q&A-anrop är den bästa platsen för att ställa frågor om driftsförändringar i CSP-programmet. Du kan [skicka en fråga](https://forms.office.com/Pages/ResponsePage.aspx?id=v4j5cvGGr0GRqy180BHbRzrhg6eBq-tPjJzqc4xPoxdUQU1WQklGNDZBNVJaRkMxUDVJVUxHSkNXWS4u) upp till 48 timmar före samtalet. Alla startrelaterade frågor besvaras i anropet och/eller i Q&A-dokumentet som publicerats efter anropet. Du kan besöka förra månadens [communitysamling och](https://partner.microsoft.com/resources/collection/august-2021-csp-partner-community-content#/) granska Q&A-dokumentet som publicerades efter augustihändelsen.

Har du frågor om något annat CSP-ämne? Besök [supportsidan för Partnercenter.](https://partner.microsoft.com/support/?stage=1)

_____________

## <a name="september-co-sell-with-microsoft-qa-community-call-reminder"></a><a name="9"></a> Påminnelse om att samarbeta med Microsoft Q&ett community-samtal i september

### <a name="categories"></a>Kategorier

- Datum: 2021-09-09
- Community-| Inbjudningar och påminnelser

### <a name="summary"></a>Sammanfattning

[Registrera dig](https://globalpbocomm.eventbuilder.com/GlobalCoSell) nu för communitysessionen i september, som visar de senaste lanseringarna och förbättringarna av den kommersiella marknadsplatsen och referensmodulerna i Partnercenter.

### <a name="impacted-audience"></a>Påverkad målgrupp

Den här sessionen är dedikerad till PartnerCenter-specifika användarroller som hanterar:

- Commercial Marketplace-modul för publiceringshantering av erbjudanden.
- Hänvisningsmodul för hantering av leads och delning av möjligheter till säljförsäljning.

Alla andra Partner Center-användare kan komma åt innehåll på begäran i [resursgalleriet för driftberedskap.](https://partner.microsoft.com/resources/cloud-solution-provider-program)

### <a name="details"></a>Information

Viktiga artiklar för den här månaden är:

#### <a name="commercial-marketplace"></a>Kommersiell marknadsplats

- [Lösnings finder är nu integrerad i AppSource](https://appsource.microsoft.com/blogs/now-live-on-microsoft-appsource-tap-into-the-unrivaled-microsoft-partner-ecosystem-to-accelerate-your-digital-transformation)
- [Vägledning och behörigheter som krävs för att publicera ett erbjudande på den kommersiella marknadsplatsen (nedladdningar PowerPoint presentation)](https://assetsprod.microsoft.com/mpn/guidance-and-permissions-needed-to-publish-an-offer-and-co-sell-with-ms.pptm)

#### <a name="referral"></a>Remiss

- [Konfigurera samförsäljning för ett erbjudande på den kommersiella marknadsplatsen](/azure/marketplace/co-sell-configure)
- [Skapa och hantera routningsregler för inkommande affärsmöjligheter: Partnercenter](../routing-rules.md)
- [Hantera möjligheter till säljförsäljning: Partnercenter](../manage-co-sell-opportunities.md#accepted-stage)
- [Avtalsregistreringsdata är nu tillgängliga för export i hänvisnings-Insights](./2021-july.md#17)

#### <a name="refresh"></a>Uppdatera

- [Erfarenhet av säljförsäljning i Partnercenter](/azure/marketplace/co-sell-configure#enter-your-contacts)
- [Referenshantering i Partnercenter](https://partner.microsoft.com/resources/detail/referral-management-in-partner-center-pptx)
- [Dela säljavtal i stor skala med hjälp av funktionen för massåtgärder i Partnercenter](./2021-february.md#13)
- [Ökad flexibilitet med partnerledda samförsäljningserbjudanden](./2021-february.md#11)
- [Hämta hänvisnings-Insights i Partnercenter](../referral-insights.md)

### <a name="next-steps"></a>Nästa steg

Granska [communityresurserna och](https://partner.microsoft.com/resources/collection/september-2021-co-sell-partner-community-content#/)registrera dig för Q&A community-anropet.

### <a name="questions"></a>Har du några frågor?

Q&A community call är den bästa platsen för att ställa frågor om operativa ändringar. Du kan [skicka en fråga](https://forms.office.com/Pages/ResponsePage.aspx?id=v4j5cvGGr0GRqy180BHbRzrhg6eBq-tPjJzqc4xPoxdUQU1WQklGNDZBNVJaRkMxUDVJVUxHSkNXWS4u) upp till 48 timmar före anropet. Alla startrelaterade frågor besvaras i anropet och/eller i Q&A-dokumentet som publicerats efter anropet.  

Om du har frågor om andra ämnen kan du gå till [supportsidan för Partnercenter.](https://partner.microsoft.com/support/?stage=1)

_____________

## <a name="new-validation-rules-for-company-name-and-email-address-on-september-22"></a><a name="8"></a>Nya verifieringsregler för företagets namn och e-postadress den 22 september

### <a name="categories"></a>Kategorier

- Datum: 2021-09-07
- Beredskap

### <a name="summary"></a>Sammanfattning

För att hjälpa partner och kunder att driva sin verksamhet baserat på förtroende uppdaterar vi valideringsreglerna för en kunds företagsnamn och e-postadress. Detta gäller både ny och befintlig kundinformation. Det krävs inga API-ändringar.

### <a name="impacted-audience"></a>Påverkad målgrupp

CSP-direktfaktureringspartner och indirekta leverantörer

### <a name="details"></a>Information

Microsoft körs med förtroende. Vi strävar efter att tillhandahålla en kompatibel, säker och säker metod för att verifiera kundens företagsnamn och e-postadressinformation. Från och med den 22 september 2021 kommer vi att uppdatera e-post- och företagsnamnsverifieringar. Mer information finns i Så [här lägger du till en ny kundpost.](../add-a-new-customer.md)

#### <a name="new-rules-for-company-name-and-email-address"></a>Nya regler för företagsnamn och e-postadress

Från och med den 22 september 2021 gäller följande nya valideringsregler.

När du anger ett företagsnamn tillåts inte följande:

- Använd bara ett tecken.
- Använd endast specialtecken, till exempel &$^# (se [tabell](../add-a-new-customer.md#table-of-special-characters)).
- Endast blanksteg och/eller tabbar.
- Använda fristående förkortningar från den begränsade listan, till exempel LLC, Inc osv. (se [tabell](../add-a-new-customer.md#table-of-abbreviations)).
- Använda namn med TDL-tillägg (Internet Top-Level Domain), till exempel ".com", ".org", ".edu", ".club", osv. (se [tabell](../add-a-new-customer.md#table-of-top-level-domain-extensions)).
- Använd samma tecken som upprepas tre eller flera gånger utan andra tecken, till exempel 999.
- Använda blanksteg och/eller tabbar blandat med enskilda tecken, till exempel 1 2 3.

När du anger en kunds e-postadress tillåts inte följande:
- E-postadressen får inte innehålla @microsoft.com .
- Kundens e-postadress får inte innehålla samma domännamn som partnern. En partner som heter ABC kan till exempel inte skapa ett e-postmeddelande för kunden med @abc.com .

Mer information finns under EAP-webbsemin:
- Däck: [https://www.yammer.com/cloudpartnercommunity/#/files/1094484746240](https://www.yammer.com/cloudpartnercommunity/#/files/1094484746240)

- Inspelning: [https://www.yammer.com/cloudpartnercommunity/#/files/1094484361216](https://www.yammer.com/cloudpartnercommunity/#/files/1094484361216)
 
#### <a name="partner-and-customer-impact"></a>Påverkan på partner och kund

Partner kommer inte att kunna skapa kunder om de inte följer ovanstående regler från den 22 september.

_____________

## <a name="readiness-dual-mode-attestation-and-additional-reseller-declaration"></a><a name="7"></a>Beredskap: Atterstation med dubbla lägen och ytterligare återförsäljardeklaration

### <a name="summary"></a>Sammanfattning

För att hjälpa partner och kunder att driva sin verksamhet baserat på förtroende kräver vi att partnern ska intyga att de fungerar som direkta eller indirekta partner när de använder samma klientorganisations-ID per transaktion.

Vi begär också att alla partner som gör transaktioner i EU-/EFTA-länder deklarerar ytterligare återförsäljare (upp till 5) som är inblandade i transaktionen.

### <a name="categories"></a>Kategorier

- Datum: 2021-09-07
- Pilotberedskap för WW-uppskjutning sker i december

### <a name="impacted-audience"></a>Målgrupp som påverkas

Indirekta CSP-leverantörer som är både direkta och indirekta partner

Indirekta partner som gör överträdelser i EU/EFTA-länder

### <a name="details"></a>Information

Microsoft körs med förtroende. Vi strävar efter att tillhandahålla en kompatibel, säker och säker metod för att göra kundprenumerationer i CSP-programmet.

Från och med den 7 september 2021 kommer vi att öppna ett pilottest för partner för att få möjlighet att testa mot nya attesteringskrav och ytterligare återförsäljare (endast EU/EFTA) ändringar som inträffar i API:erna Skapa kundvagn, Uppdatera kundvagn och Skapa beställning. Observera att dessa ändringar kommer att bryta befintliga upplevelser för dessa API:er. Därför rekommenderar vi starkt att partner tar tillfället i akt att delta i pilottestet innan den fullständiga uppskjutningen i december.

#### <a name="partner-and-customer-impact"></a>Partner- och kundpåverkan

- NY ÄNDRING: Indirekta partner kommer inte att kunna slutföra köp utan att först ha intyg om att de fungerar som direkta eller indirekta partner
- EU-/EFTA-partner följer inte EU-regler om de inte deklarerar och inkluderar ytterligare återförsäljare som är inblandade i transaktionen
- Mer information finns under EAP-webbsemin: 
- Däck: [https://www.yammer.com/cloudpartnercommunity/#/files/1094484746240](https://www.yammer.com/cloudpartnercommunity/#/files/1094484746240)
- Inspelning: [https://www.yammer.com/cloudpartnercommunity/#/files/1094484361216](https://www.yammer.com/cloudpartnercommunity/#/files/1094484361216)

Följande API:er påverkas och informationen har delats och uppdaterats därefter:

- [Skapa en kundorder – partnercenterapputvecklare](/partner-center/develop/create-an-order)
- [Skapa en kundvagn – partnercenterapputvecklare](/partner-center/develop/create-a-cart)
- [Uppdatera en kundvagn – partnercenterapputvecklare](/partner-center/develop/update-a-cart)

De ytterligare återförsäljarna påverkar partner som gör transaktioner i följande EU-/EFTA-länder:

| EU-/EFTA-länder | &nbsp; | &nbsp; |
| --- | --- | --- |
| Andorra<br>Österrike<br>Belgien<br>Bouvetön<br>Bulgarien<br>Kroatien<br>Cypern<br>Tjeckien<br>Danmark<br>Estland<br>Färöarna<br>Finland<br>Frankrike<br>Tyskland<br>Gibraltar | Grekland<br>Grönland<br>Guernsey<br>See (covers Vatikan city)<br>Ungern<br>Island<br>Irland<br>Isle of Man<br>Italien<br>Jersey<br>Lettland<br>Liechtenstein<br>Litauen<br>Luxemburg<br>Malta | Monaco<br>Nederländerna<br>Norge<br>Polen<br>Portugal<br>Rumänien<br>San Marino<br>Slovakien<br>Slovenien<br>Spanien<br>Svalbard och Jan Mayen<br>Sverige<br>Schweiz<br>Storbritannien: TBD |
|

Om du vill delta i piloten ska du kontakta ämnesexperten (AliCertifikatki) och ange partnerns klientorganisations-ID så att de kan läggas till i flygresan.

_____________

## <a name="perpetual-software-and-software-subscriptions-price-lists-republished-to-fix-price-increases-in-russia"></a><a name="6"></a>Löpande prislistor för programvaru- och programvaruprenumerationer publiceras på nytt för att åtgärda prisökningar i Ryssland

### <a name="categories"></a>Kategorier

- Datum: 2021-09-03
- Erbjudanden/marknader

### <a name="summary"></a>Sammanfattning

Prislistorna för permanent programvara och programvaruprenumerationer som publicerades den 1 september 2021 återpublicerades den 3 september för att åtgärda ett prisproblem i Ryssland.

### <a name="impacted-audience"></a>Målgrupp som påverkas

Indirekta leverantörer och direktfaktureringspartner som överför permanenta programvaru- och programvaruprenumerationer i Molnlösningsleverantör i Ryssland.

### <a name="details"></a>Information

De permanenta prislistorna för programvaru- och programvaruprenumerationer som publicerades den 1 september hade en felaktig prisökning på 15,2 % som angavs för alla produkter.

Prisökningen på ~15,2 % börjar gälla den 1 oktober **2021**, inte i september. Prislistorna har publicerats på nytt med rätt prisinformation.

Partner som har köpt produkter mellan 1 september och 3 september debiteras enligt de korrigerade priserna som visas i de senaste prislistorna.

### <a name="next-steps"></a>Nästa steg

- Partner som använder permanent programvara och programvaruprenumerationer i Ryssland bör ladda ned den senaste prislistan för att se de korrigerade priserna.
- Information om prisökningarna som kommer i oktober finns i artikeln [Microsoft justerar licensieringsprogrammet för kommersiella kunder i Ryssland.](https://news.microsoft.com/ru-ru/licensing-changes-at-microsoft-russia-2021/)

_____________

## <a name="corrections-to-september-license-based-services-price-list-and-october-preview-for-microsoft-365-business-basic-usd"></a><a name="5"></a>Korrigeringar av prislistan för septemberlicensbaserade tjänster och oktoberförhandsvisningen för Microsoft 365 Business Basic (USD)

### <a name="summary"></a>Sammanfattning

Septemberprislistan och oktoberförhandsvisningen hade ett felaktigt listpris för Microsoft 365 Business Basic i USD.

### <a name="categories"></a>Kategorier

- Datum: 2021-09-02
- Erbjudanden/marknader

### <a name="impacted-audience"></a>Målgrupp som påverkas

Indirekta leverantörer och direktfaktureringspartner som överför licensbaserade tjänster i Molnlösningsleverantör program.

### <a name="details"></a>Information

Prislistan för september och förhandsversionen av licensbaserade tjänster som publicerades den 1 september 2021 hade ett felaktigt listpris för Microsoft 365 Business Basic. Korrigerade prislistor publicerades den 2 september 2021. Detta påverkar endast USD.

Det påverkade erbjudandet omfattar:

- Erbjudandenamn: Microsoft 365 Business Basic
- Erbjudande-ID: bd938f12-058f-4927-bba3-ae36b1d2501c
- Före: Listpris = 2
- Efter: Listpris = 4

### <a name="next-steps"></a>Nästa steg

Partner som överlappar licensierade tjänster i USD bör ladda ned den senaste prislistan för att se det korrigerade priset.

________________
## <a name="nigeria-and-thailand-are-now-microsoft-managed-countries"></a><a name="4-5"></a>Now Microsoft-hanterade länder

### <a name="categories"></a>Kategorier

- Datum: 2021-09-01
- Funktioner

### <a name="summary"></a>Sammanfattning

Både Kina och Kina är nu Microsoft-hanterade länder.

### <a name="impacted-audience"></a>Påverkad målgrupp

Partner som gör en transacting iRanska ochNdee.

### <a name="details"></a>Information

Se [Skatteinformation för kommersiella marknadsplatsutgivare.](../tax-details-marketplace.md)

### <a name="questions"></a>Frågor

Om du har fler frågor om dessa erbjudanden kan du läsa dina Yammer communityn.

________________
## <a name="announcing-intune-per-device-for-enterprise-for-csp-partners"></a><a name="4"></a>Meddelande om Intune per enhet för Enterprise för CSP-partner

### <a name="categories"></a>Kategorier

- Datum: 2021-09-02
- Funktioner

### <a name="summary"></a>Sammanfattning

Vi presenterar ett nytt erbjudande för Intune per enhet, som är tillgängligt från och med den 1 september.

### <a name="impacted-audience"></a>Påverkad målgrupp

Partner som gör en transacting Molnlösningsleverantör (CSP)-programmet.

### <a name="details"></a>Information

Microsoft Intune är den mest omfattande enhetliga plattformen för slutpunktshantering för att hantera och skydda både fysiska och virtuella slutpunkter i din organisation. Vi presenterar ett nytt Erbjudande för Intune per enhet som hjälper företagsorganisationer att hantera enheter som har tilldelats till en autentiserad användare (d.v.s. inte används av flera autentiserade användare).

Det här erbjudandet, som är tillgängligt 1 september 2021, utnyttjar Intune per enhet och lägger till Azure Active Directory (Azure AD). Det är en helt funktionell färdig upplevelse och innehåller följande tjänstplaner:

- Exchange Foundation
- Microsoft Intune
- Azure Active Directory for Education.

Baserat på feedback från våra Microsoft-partner har Intune per enhet för Enterprise skapats för att ingå i en försäljning per enhet (enhet + Windows + Intune) som ett femårigt erbjudande som sträcker sig över enhetens livslängd. Det här nya erbjudandet hjälper CSP:er att förenkla avtalsstrukturer och erbjuda sina kunder ett mer konkurrenskraftigt avtal.

Information om det nya Intune-erbjudandet per enhet:

- Det är ett SaaS Enterprise-erbjudande och är inte utformat för SMB-kunder (Small & Medium Business).
- Den är endast tillgänglig för CP:er och är inte tillgänglig i Volymlicensiering eller Web Direct.
- Kostnaden är 150 USD (USD/ERP) för en femårsprenumeration.
- Erbjudande-ID: 5170ccfb-e95b-49a4-b7f3-31f631a356ba
- Det fungerar som det ska för alla Windows till en enda autentiserad användare.
- Erbjudandet omfattar inte enhetsbaserad villkorlig åtkomst.  

### <a name="questions"></a>Frågor

Om du har fler frågor om dessa erbjudanden kan du läsa dina Yammer communityn.

_____________

## <a name="key-updates-for-the-new-commerce-experience-for-cloud-solution-provider-csp-seat-based-offers"></a><a name="3"></a>Viktiga uppdateringar för den nya handelsupplevelsen för Molnlösningsleverantör(CSP)-baserade erbjudanden

### <a name="summary"></a>Sammanfattning

Som en uppföljning till avslöjandet den 19 augusti 2021 har Microsoft viktiga uppdateringar för den nya handelsupplevelsen för CSP-platsbaserade erbjudanden.

### <a name="categories"></a>Kategorier

- Datum: 2021-09-01
- Funktioner

### <a name="impacted-audience"></a>Påverkad målgrupp

CSP:s direktfaktureringspartner och indirekta leverantörer och återförsäljare via deras indirekta leverantörer

### <a name="details"></a>Information

Den 19 augusti 2021 presenterade [Microsoft](https://partner.microsoft.com/resources/detail/new-commerce-for-csp-seat-based-offers-pdf) den nya handelsupplevelsen för Microsoft 365, Dynamics 365, Power Platform och Windows 365-baserade erbjudanden för bredd rörelse som kommer i oktober 2021. Som en uppföljning till det här meddelandet har vi följande viktiga uppdateringar som hjälper din organisation att förbereda för den här omvandlingen:

- Lansering av de platsbaserade erbjudandena för integrerad sandbox-testning
- Påminnelse för kommande CSP Q&A-anrop i september
- Incitamentprogram för Microsoft Commerce

#### <a name="launch-of-seat-based-offers-for-integrated-sandbox-testing"></a>Lansering av platsbaserade erbjudanden för integrerad sandbox-testning

Från och med den 1 september 2021 har Microsoft aktiverat [](https://partner.microsoft.com/resources/detail/new-commerce-for-csp-seat-based-offers-pdf) platsbaserade erbjudanden för integrerad [sandbox-testning](/partner-center/develop/test-and-debug) i den nya handelsupplevelsen för CSP-programmet.

Tillägget av Microsoft 365, Dynamics 365, Power Platform och Windows 365-erbjudanden i CSP till den nya handelsupplevelsen är en annan viktig milstolpe i vår nya handelsresa. Microsoft investerar i produktinnovationer, bättre verktyg och tillgång till nya affärsmöjligheter som gör det möjligt för partner att öka sina CSP-intäkter och ge fler alternativ till kunder. Vi utvecklar vår handelsplattform och effektiviserar order- och prenumerationshanteringsprocesserna för att hjälpa partner och kunder att lyckas med den digitala omvandlingen.

Partner som deltar i sandbox-testmiljön får tidig insyn i den nya handelsupplevelsen för platsbaserade erbjudanden, vilket möjliggör avancerad planering, operationalisering och teknisk integrering för dessa erbjudanden.

Genom att delta i sandbox-miljön kan din organisation:

- Utföra API-integrering i en testmiljö innan du distribuerar i produktion
- Ha tillräckligt med tid för att operationalisera den nya handelsupplevelsen innan du startar

Tabellen innehåller en sammanfattning av de viktigaste funktionerna som är tillgängliga i den integrerade sandbox-testmiljön:

| Konfigurera administratörsbehörigheter för partner/kunddelegier | Partiell underuppgradering – fullständig funktion |
| ----------- | ---------------|
| Modeller på 1 nivå, 2 nivåer | Partiell prenumerationsuppgradering via support |
| Identifiering sida vid sida av aktuell och ny upplevelse | Schemalagda ändringar vid förnyelse  |
| Identifiera och köpa Modern (välj produkter) | Pausa/återuppta (via support) |
| Hantera prenumeration (automatisk förnyelse, lägg till platser, avbryt rörelse) | Kostnadsfria utvärderingsversioner (endast MAC-presentment) |
| Oberoende tillägg  | Partnervaluta |
| Faktureringsplaner | Pristransparens  |
| Livscykelhantering för prenumeration (respitperiod) | Årliga faktureringsplaner för erbjudanden under flera år  |
| Begränsningar för ägarskap | Pausa/återuppta (via självbetjäning)  |
| Faktura-/rekognoseringsfiler | Omtilldeling av automatisk plats för fullständiga SKU-övergångar |
| SKU-uppgraderingar med medeltidsmängd | Kostnadsfri utvärderingsversion (med fullständig present) |
| Framtvingande av annulleringsprincip: 30 dagars blockavbokning efter 30 dagar (ändras med allmän tillgänglighet till 72 timmar) |  |
|

#### <a name="reminder-for-upcoming-csp-qa-calls-in-september"></a>Påminnelse för kommande CSP Q&A-anrop i september

Registrera dig för kommande [CSP Q&A Community Calls](https://globalpbocomm.eventbuilder.com/GlobalCSP) den 15 september och 16 september för att lära dig och ställa frågor om den nya handelsupplevelsen för Microsoft 365, Dynamics 365, Power Platform och Windows 365 seat-based offers for breadth motion som kommer i oktober 2021. CSP Community Q&A-anrop är dedikerade för att hjälpa CSP-direktfakturering och indirekta partner med frågor som rör CSP-uppskjutningar och kommande ändringar. För att underlätta för dig görs communitysamlingar tillgängliga i förväg i [galleriet med partnerberedskap,](https://partner.microsoft.com/resources/assets/#/?prog=CSP%7CCSP-Direct%7CCSP-Indirect-Partner&type=collection&search=community%20collection%202021&sort=updated) där du kan granska material som diskuteras i Q&A call (Frågor och svar-anrop).

Om du vill delta i och/eller hitta tidigare inspelningar av CSP Fundamentals-anrop kan du gå till [registrering av grunderna för CSP.](https://globalpbocomm.eventbuilder.com/CSPFundamentals)

#### <a name="microsoft-commerce-incentive-program"></a>Incitamentprogram för Microsoft Commerce

Den 1 september 2021 har Microsoft informerat partner om nästa steg i utvecklingen av sitt partnerincitamentprogram så att det blir tillgängligt i oktober. De två primära komponenterna i den här kommunikationen är FY22-incitamentsguiderna och information om den förbättrade incitamentsupplevelse som utvecklas i Partnercenter.

- **Förbättrad partnerupplevelse**  I början av oktober som mål för partnerns tillgänglighet investerar Microsoft i en enda engagemangs- och aktivitetsplattform i Partnercenter som är ett centraliserat mål för partner för att få incitament genom köpsteg och faser i kundens livscykel.

- **Ny metod för incitament**  Nya incitaments- och investeringserbjudanden kommer att fortsätta att läggas till i Microsoft Commerce Incentives program. I enlighet med arbetet med att förenkla partnerupplevelsen konsoliderar Microsoft incitamentprogramguiderna till ett enda dokument som finns i Partnercenter.

### <a name="next-steps"></a>Nästa steg

#### <a name="launch-of-seat-based-offers-for-integrated-sandbox-testing"></a>Lansering av platsbaserade erbjudanden för integrerad sandbox-testning

- Ingen åtgärd krävs om din organisation har etablerat en integrerad sandbox-miljö. Om din organisation inte har en integrerad sandbox-miljö följer du dessa steg [för](/partner-center/develop/indirect-provider-sandbox-capabilities) att skapa en.
- Läs [CSP-handboken](https://partner.microsoft.com/resources/detail/operating-guide-new-commerce-experience-for-csp-seat-based-offers-pdf) för Microsoft 365, Dynamics 365, Power Platform och Windows 365 i den nya handelsupplevelsen för att lära dig mer om funktioner, affärsregler och stegvisa instruktioner för versionen. Kontrollera regelbundet handboken eftersom den uppdateras regelbundet.
- Granska resurserna som beskrivs i [beredskapskartan](https://partner.microsoft.com/resources/detail/readiness-map-new-commerce-experienceseat-based-offers-pdf).
- Läs [API-dokumentationsmappen](https://partner.microsoft.com/resources/collection/api-documentation#/).
- Om du behöver support loggar du en supportbegäran eller gör ett inlägg i konversationerna i [Partnercenter-SDK-](https://www.yammer.com/cloudpartnercommunity/#/threads/inGroup?type=in_group&feedId=6589502)och API Yammer-gruppen , där presentationer och inspelningar av funktionsinlägg publiceras under september månad.

#### <a name="reminder-for-upcoming-csp-qa-calls-in-september"></a>Påminnelse om kommande CSP Q&A-anrop i september

- Registrera dig för kommande [CSP Q&A Community Calls](https://globalpbocomm.eventbuilder.com/GlobalCSP) den 15 september eller 16 september.
- Läs den nya handelsupplevelsen för CSP-platsbaserade erbjudanden [för den](https://partner.microsoft.com/resources/collection/new-commerce-experience-for-csp-seat-based-offers#/) här lanseringen.
- Delta i CSP Q&A Community Call och ställ frågor som din organisation har angående den nya handelsupplevelsen för Microsoft 365, Dynamics 365, Power Platform och Windows 365-platsbaserad för bredd rörelse.

#### <a name="microsoft-commerce-incentive-program"></a>Microsoft Commerce Incitamentprogram

- Granska kommunikationen i den kommande förbättrade partnerupplevelsen i Microsoft Commerce Incentives [resurssamlingen](https://partner.microsoft.com/asset/collection/microsoft-commerce-incentive-resources#/).
- Granska de uppdaterade FY22-partnerincitamentguiderna på [partnerincitamentportalen.](https://microsoft.sharepoint.com/teams/PartnerIncentivesPortal)

### <a name="questions"></a>Har du några frågor?

Om du har fler frågor om dessa erbjudanden kan du läsa dina Yammer communityn.

_____________

## <a name="view-this-months-product-launches-and-offers"></a><a name="2"></a>Visa den här månadens produktlanseringar och erbjudanden

### <a name="summary"></a>Sammanfattning

Produktlanserings kalender för september 2021 publiceras nu.

### <a name="categories"></a>Kategorier

- Datum: 2021-09-01
- Utveckla din verksamhet

### <a name="impacted-audience"></a>Målgrupp som påverkas

Alla partner som gör en Molnlösningsleverantör (CSP)

### <a name="details"></a>Information

Kalendern för produktlansering september 2021 [](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) är nu tillgänglig i resursgalleriet för driftberedskap. Visa kommande produktlanseringar och erbjudanden här.

### <a name="next-steps"></a>Nästa steg

Granska kalendern [för produktlansering](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/)och dela informationen med lämpliga intressenter i din organisation.  

### <a name="questions"></a>Har du några frågor?

Om du har fler frågor om dessa erbjudanden kan du läsa dina Yammer communityn.

_____________

## <a name="software-in-microsoft-china-cloud-solution-provider-program-mccl-csp-to-start-transactions-from-august-12"></a><a name="1"></a>Programvara i Microsoft China Molnlösningsleverantör-program (MCCL CSP) för att starta transaktioner från och med 12 augusti

### <a name="summary"></a>Sammanfattning

Som en uppföljning till vår uppdatering från den 3 augusti startar programvara i MCCL CSP transaktioner från den 12 augusti 2021.

### <a name="categories"></a>Kategorier

- Datum: 2021-09-01
- Utveckla din verksamhet

### <a name="impacted-audience"></a>Målgrupp som påverkas

MCCL CSP-programpartner

### <a name="details"></a>Information

#### <a name="mccl-csp-transaction-start"></a>Start av MCCL CSP-transaktion

- Den 12 augusti 2021 startar MCCL CSP transaktioner för kinesiska kunder.

- Kunder kan fortsätta att köpa programvarulicenser med hjälp av en partner i Open License-programmet fram till den 31 december 2021. Beständiga licenser kommer att vara tillgängliga i både MCCL CSP och Open License-programmen fram till utfasningen av Open License-programmet.

#### <a name="open-license-program-deprecation"></a>Utfasning av licensprogram

- Från och med 1 januari 2022 kan kunder inte längre köpa eller förnya programvarulicenser via Microsoft Open License-programmet.

- Kunder kan fortsätta att ha fullständiga rättigheter och åtkomst till alla permanenta programvarulicenser som köpts via Open License-programmet även efter utfasningen. De kan också fortfarande komma åt Volume Licensing Service Center för att hantera dessa licenser och tjänster.

#### <a name="software-assurance-sa-purchases"></a>Software Assurance köp (SA)

- SA-erbjudanden med Open License (L&SA) fortsätter att vara tillgängliga i Open Value (OV) och Open Value Subscription (OVS). Men varken SA eller L&SA är tillgängliga i MCCL CSP-programmet eftersom det inte finns någon plan för att erbjuda detta i MCCL CSP.

- SA-förmånerna fortsätter tills SA-perioden upphör att gälla, även om den upphör att gälla efter den 1 januari 2022.

- Microsoft OV-programmet rekommenderas för framtida inköp som inkluderar SA.

>[!NOTE]
>Det finns inga planer på att ändra OV- och OVS-programmen.

#### <a name="partner-change-management"></a>Partnerändringshantering

- Befintliga Microsoft Open-distributörer har publicerats som indirekta MCCL-leverantörer.

- Indirekta leverantörer och utvalda indirekta återförsäljare bjuds in att genomföra testning av produktionsmiljön i augusti för att säkerställa transaktionsfunktionen.

- Beredskapsworkshops för indirekta partner startade i juli och fortsätter till december 2021.

### <a name="next-steps"></a>Nästa steg

Gör dig redo för den här ändringen med hjälp av följande resurser:

- [Vad är ny handel?](https://partner.microsoft.com/resources/detail/new-commerce-experience-introduction)
- [Spelbok om indirekt MCCL CSP-leverantör](https://microsoftapc.sharepoint.com/:b:/t/ChinaLicensingHome/EeWi5axiZ_RCkTbxa-brE-sBGYdLJ5idpnZvFt2MFiTLWw?e=6itfqY)
- [Spelbok om indirekt MCCL-återförsäljare](https://microsoftapc.sharepoint.com/:b:/t/ChinaLicensingHome/EY-csVS7lFdKpwkRqeJJ4hkBPGWv4qkfINictqVrwKVLxQ?e=9G6ZY1)

Observera att dessa ändringar endast gäller för MCCL CSP och inte påverkar 21 Vianet CSP.

### <a name="questions"></a>Har du några frågor?

Om du har ytterligare frågor kan du prata med din lokala partnerutvecklingschef.
