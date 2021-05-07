---
title: Meddelanden mars 2021
description: Mars 2021-meddelanden för Microsoft Partner Center, inklusive nya funktioner, kampanjer, erbjudanden, marknader eller ändringar i befintliga erbjudanden.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: brentserbus
ms.author: brserbus
ms.custom: announcement
ms.localizationpriority: high
ms.date: 04/02/2021
ms.openlocfilehash: 3d91eb26f98005b92a48c6f242ea4439e42cde05
ms.sourcegitcommit: 22e257d5b334ca8d3fc072f59010a508e1022694
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 05/06/2021
ms.locfileid: "108702883"
---
# <a name="march-2021-announcements"></a>Meddelanden mars 2021

Den här sidan innehåller meddelanden för Microsoft Partner Center för mars 2021.

## <a name="readiness-changes-to-the-cloud-solution-provider-csp-customer-address-validation-api-going-live-in-june-testing-capability-now-available"></a><a name="18"></a>Beredskap: Ändringar i CSP Molnlösningsleverantör-API:et för kundadressvalidering går live i juni. nu tillgänglig testfunktion

### <a name="categories"></a>Kategorier

- Datum: 2021-03-30
- Beredskap

### <a name="summary"></a>Sammanfattning

För att hjälpa partner och kunder att driva sin verksamhet baserat på förtroende kommer vi att bjuda in partner att testa ändringar i API:et validate address för alla länder över hela världen.

### <a name="impacted-audience"></a>Målgrupp som påverkas

CSP-direktfaktureringspartner och indirekta leverantörer som skapar nya eller uppdaterar befintliga kunders adressinformation.

### <a name="details"></a>Information

Microsoft körs med förtroende. Vi strävar efter att tillhandahålla en kompatibel, säker och säker metod för validering av kundadresser för att kunna hantera kundprenumerationer i CSP-programmet. Från och med den 31 mars 2021 har vi infört ändringar i API:et Validate Address som vi bjudit in partner att testa innan vi går live med ändringarna i juni 2021.

Ändringarna påverkar endast API:et validate address. API:er för att skapa kund och uppdatera faktureringsprofil påverkas inte.

Svaret returnerar något av följande statusmeddelanden:

| Status     | Beskrivning |    Antal föreslagna adresser som returneras |
|-------|---------------|-------------------|
|Verifierad leverans | Adressen är verifierad och kan skickas till. | Enkel |
|Verifierat | Adressen är verifierad. | Enkel |
|Interaktion krävs | Den föreslagna adressen har ändrats avsevärt och kräver användarbekräftelse. | Enkel |
|Gatuadress – partiell | Den angivna gatuadressen är delvis och behöver mer information. | Flera – högst tre |
|Delvis lokal | De angivna lokalerna (byggnummer, svitnummer och annat) är ofullständiga och behöver mer information. | Flera – högst tre |
|Flera | Det finns flera fält som är partiella i adressen (eventuellt även delvis gatuadress och delvis lokal). | Flera – högst tre |
|Inget | Adressen är felaktig. | Inget |
|Inte validerat | Adressen kunde inte skickas via valideringsprocessen. | Inget |

Amerikanska postkoder returnerar ytterligare 4 siffror + bindestreck , till exempel 12345-6789.

När en adress har skickats för validering via API:et validate address returneras följande svarsschema:

```csharp

// <summary>
/// Object represents the address validation response.
/// </summary>

public class AddressValidationResponse
{
   /// <summary>
   /// Gets or sets the original address
   /// </summary>
   /// <value>
   /// Original Address
   /// </value>
   public Address OriginalAddress { get; set; }

   /// <summary>
   /// Gets or sets the suggested addresses
   /// </summary>
   /// <value>
   /// Suggested Addresses
   /// </value>
   public List<Address> SuggestedAddresses { get; set; }

   /// <summary>
   /// Gets or sets the validation status
   /// </summary>
   /// <value>
   /// Status
   /// </value>
   public string Status { get; set; }

   /// <summary>
   /// Gets or sets the validation message
   /// </summary>
   /// <value>
   /// Validation Message
   /// </value>
   public string ValidationMessage { get; set; }
   ```

Ta en titt på det här exempelsvaret. Observera att för USA returnerar svaret ytterligare ett fyrsiffrigt suffix för postnummerraden om du bara anger fem siffror för postnumret.

```csharp

"suggested_address": {
              "Country": "US",
              "region": "WA",
              "city": "Redmond",
              "address_line1": "1 Microsoft Way",
              "postal_Code": "98052-8300"
},
"original_address": {
              "Country": "US",
              "region": "WA",
              "city": "Redmond",
              "address_line1": "1 Micro Way",
              "postal_Code": "98052"
},
"status":  "InteractionRequired",
"validation_message": "Address field invalid for property: ‘Street’"
}
```

### <a name="next-steps"></a>Nästa steg

- Dela ditt klientorganisations-ID för sandbox-miljön med ämnesexperten (AliJektki) som ska ingå i testresan, så att du kan börja förbereda dig för uppdateringen.

- Om du använder en CPV-lösning (Kontrollpanelens leverantör) kan du kontakta din CPV.

### <a name="questions"></a>Har du några frågor?

Om du behöver support för din verksamhet med Microsoft kan du kontakta yammer-gruppen som din partner har stöd för.

### <a name="change-log"></a>Ändringslogg:

- 31 mars 2020: Ursprunglig publikation

- 30 april 2021: Uppdateringar för exempelsvar och postnummerinformation

________________
## <a name="new-exchange-admin-center-eac-experience"></a><a name="17"></a>Ny upplevelse för Administrationscenter för Exchange (EAC)

### <a name="categories"></a>Kategorier

- Datum: 2021-03-29
- Funktioner

### <a name="summary"></a>Sammanfattning

Från och med 27 april 2021 kommer Administrationscenter för Exchange (EAC) att distribuera en ny upplevelse som förbättrar den dagliga effektiviteten för användarna.

### <a name="impacted-audience"></a>Målgrupp som påverkas

Delegerade administratörer som har åtkomst till Exchange via Partnercenter

### <a name="details"></a>Information

Från och med 27 april 2021 omdirigeras partner som navigerar till Exchange via Partnercenter till den nya EAC:en.

Den här nya upplevelsen är för närvarande tillgänglig som en förhandsversion, och administratörer kan aktivera den här funktionen genom att välja växlingsknappen i det övre högra hörnet i den klassiska EAC. De kan också navigera till den nya EAC genom att välja banderollen "Prova nu" som visas på alla sidor.

Fördelarna med den nya EAC:en är:

- Lade till insikter, rapporter och aviseringsmekanismer för e-postflödesrelaterade problem. 

- Anpassade instrumentpaneler för att öka produktiviteten.

Videor som hjälper dig att navigera i den nya upplevelsen finns i avsnittet **Utbildningsguide & den** nya EAC-upplevelsen. Dessa ger dig en översikt över hur du bäst kan använda den nya portalen.

>[!NOTE]
>Med den här ändringen kommer den klassiska EAC-upplevelsen inte att bli inaktuell. Du meddelas i god tid innan någon ändring implementeras.

### <a name="next-steps"></a>Nästa steg

- Kolla in resurserna [om det här avsnittet,](https://partner.microsoft.com/resources/collection/new-exchange-admin-center-experience#/)där du kan visa skärmbilder av den nya upplevelsen.

- Dela den här informationen med lämpliga intressenter i din organisation. 

### <a name="questions"></a>Har du några frågor?

Om du har frågor om dessa ändringar kan du kontrollera dina relevanta Yammer-communities.

________________
## <a name="microsoft-operations-introducing-the-product-launch-calendar"></a><a name="16"></a>Microsoft Operations: Introduktion till kalendern för produktlansering

### <a name="categories"></a>Kategorier

- Datum: 2021-03-25
- Erbjudanden | Modern arbetsplats

### <a name="summary"></a>Sammanfattning

Som svar på partnerfeedback effektiviserar Microsoft Operations kommunikationen för produktlanseringar.

### <a name="impacted-audience"></a>Påverkad målgrupp

Molnlösningsleverantör (CSP)-partner

### <a name="details"></a>Information

Microsoft strävar efter att kontinuerligt förbättra partnerupplevelserna. Vi har fått feedback från dig om att du har fått för många meddelanden från Microsoft, inklusive dubbla meddelanden om produktlanseringar.

Som svar på din feedback har Microsoft effektiviserat beredskapsupplevelsen för produktlanseringar för nya och befintliga erbjudanden.

Vi ger dig nu en enda månatlig vy över produktlanseringar som publicerats i resursgalleriet för driftberedskap. Den här [månatliga kalendervyn för produktlansering](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) ersätter enskilda meddelanden om produktlansering i resursgalleriet för driftberedskap och i Partnercenter-meddelanden.

Du kan också komma åt den [här produktlanseringskalendern](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) från [communitysamlingar,](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) [kalendervyer](https://partner.microsoft.com/resources/assets#/?type=collection&search=Calendar&sort=updated)och [CSP-nyhetsbrev.](https://partner.microsoft.com/resources/collection/csp-monthly-update#/) Vi meddelar dig när vi publicerar varje månads kalender för produktlansering med ett meddelande i resursgalleriet för driftberedskap.

Du hittar fortfarande information om nya och befintliga erbjudanden i förhandsgransknings- och prislistans ändringsloggar, samt i produktbloggar, licensieringsguider och marknadsföringssidor.

Ändringen gäller för lanseringar för följande produkter:

- Lokal Dynamics
- Microsoft 365
- Microsoft Dynamics 365
- Windows
- Server  
- Verktyg
- Teams och Telco

Vi fortsätter att skicka specifika meddelanden om produktlanseringar som kräver information om driftberedskap.

### <a name="next-steps"></a>Nästa steg

Granska resurserna om det här avsnittet och dela den här informationen med lämpliga intressenter i din organisation.

### <a name="questions"></a>Har du några frågor?

Om du har fler frågor om dessa erbjudanden kan du läsa dina relevanta Yammer-communities.

________________
## <a name="changes-to-csp-customer-onboarding-requirements"></a><a name="15"></a>Ändringar av CSP-krav för kund-onboarding

### <a name="categories"></a>Kategorier

- Datum: 2021-03-25
- Funktioner

### <a name="summary"></a>Sammanfattning

Som en del av vårt åtagande att hjälpa partner och kunder att driva sin verksamhet baserat på förtroende begär vi ytterligare kundinformation från och med den 25 mars 2021.

### <a name="impacted-audience"></a>Målgrupp som påverkas

Molnlösningsleverantör direktfaktureringspartner och indirekta leverantörer som har nya eller befintliga kunder i de länder som anges i nästa avsnitt

### <a name="details"></a>Information

Microsoft körs med förtroende. Vi strävar efter att tillhandahålla en kompatibel, säker och säker metod för kundvalidering för att kunna göra kundprenumerationer i CSP-programmet. Den 25 mars 2021 introducerar vi förbättringar av Partner Center API och användargränssnitt som påverkar partner som uppfyller båda följande kriterier:

1. Partnern har en direkt faktureringsrelation med Microsoft (vilket innebär att partnern antingen är en partner för direktfakturering eller en indirekt leverantör).

2. Partnern gör affärer med nya eller befintliga kunder i följande länder:

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

Partner som uppfyller villkoren måste skicka in en kunds företagsregistrerings-ID (kallas även  kundens **organisation INN)** och telefonnummer när de registrera nya kunder eller ändra befintlig kundinformation.  Dessa partner kan också ange ett **mellannamn** för kunden (valfritt).

Observera att när du lägger till ditt företagsregistrerings-ID bör du använda ditt företagsskatte-ID och inte kundens personliga ID.

Partner som gör affärer med nya eller befintliga kunder i följande länder har redan fått en tidigare version i november 2020.

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

Partner med kunder i resten av världen kan den 25 mars 2021 ange företagets  **registrerings-ID,** telefonnummer och mellannamn för kunder som valfri information.

### <a name="next-steps"></a>Nästa steg

- Mer detaljerad vägledning finns i den tekniska dokumentationen och vanliga frågor [och svar i](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/) den dedikerade partnersamlingen.

- Förbered för att införliva ändringarna med partnercenter-API:et och webbanvändarupplevelsen. API/SDK:er kommer att vara tillgängliga för testning.

- Se till att skicka in ytterligare data när du registrera nya kunder eller ändrar befintlig kundinformation.

- Om du använder en CPV-lösning (Kontrollpanelens leverantör) kan du kontakta din CPV.

### <a name="questions"></a>Har du några frågor?

Kontakta skatterådgivaren eller det lokala skattekontoret om du har frågor om den juridiska identifieraren (kallas även INN eller TIN). Microsoft kan inte ge vägledning om skattefrågor.

Om du behöver support för din verksamhet med Microsoft öppnar [du en tjänstbegäran.](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=aa679372-d996-73df-e244-cb28bbbf28e8)

________________
## <a name="corrections-made-to-march-1-2021-perpetual-software-price-list"></a><a name="14"></a>Korrigeringar som gjorts för 1 mars 2021 permanent programvaruprislista

### <a name="categories"></a>Kategorier

- Datum: 2021-03-23
- Erbjudanden/marknader

### <a name="impacted-audience"></a>Påverkad målgrupp

Indirekta leverantörer och direktfaktureringspartner som använder permanent programvara i Molnlösningsleverantör program 

### <a name="details"></a>Information

Prislistan för permanent programvara som publicerades den 1 mars 2021 innehöll marknader som inte borde ha funnits där. Den permanenta programvaruprislistan uppdaterades den 17 mars 2021 med korrigeringarna. De här korrigeringarna gäller endast för:

- Produkt-ID: DF77X4D43RKT 
- Produktnamn: Windows 10 Home pro-uppgradering för Microsoft 365 företag
- Borttagna eller icke-stödda marknader: AE, AF, AL, AM, AO, BA, BB, BD, BM, BN, BO, BR, BS, BW, BY, BZ, CI, CL, CM, CO, CR, CW, DO, DZ, EC, EG, ET, FJ, FO, GE, GH, GT, HN, IL, IN, IQ, JM, JO, KE, KG, KN, CR, KY, KZ, LB, LK, LY, MA, MC, MD, ME, MN, MO, MU, NA, NG , NI, NP, OM, PA, PE, PH, PK, PR, PY, QA, RS, RU, RW, SG, SN, SV, TH, TJ, TM, TN, TT, TZ, UA, UG, UY, CUS, VE, VN, YE, ZM, ZW

Dessa ändringar gäller endast för ovanstående produkt. Andra produkter hade inga korrigeringar. 

### <a name="next-steps-and-resources"></a>Nästa steg och resurser

- Partner som överlappar permanent programvara bör ladda ned den senaste permanenta programvaruprislistan.
- Se [landskoderna för regionen för](https://docs.microsoft.com/azure/marketplace/commercial-marketplace-co-sell-countries) en användarvänlig mappning av förkortningen på två bokstäver till länder.
________________
## <a name="sdk-release-on-net-standard-v1170"></a><a name="13"></a> SDK-version på .NET Standard (v1.17.0)

### <a name="categories"></a>Kategorier

- Datum: 2021-03-23

- Funktioner
 
### <a name="impacted-audience"></a>Målgrupp som påverkas

Direktfaktureringspartner och indirekta leverantörer som deltar i CSP-programmet som använder Partner Center .NET SDK.

### <a name="details"></a>Information

Från och med 23 mars 2020 kan partner börja ladda ned versionen av [MicrosoftPartnerCenter.NETSDK (NuGet-| Microsoft.Store.PartnerCenter 1.17.0)](https://www.nuget.org/packages/Microsoft.Store.PartnerCenter/1.17.0), tillsammans med uppdaterade offentliga Partnercenter-SDK [GitHub-exempel](https://github.com/Microsoft/Partner-Center-DotNet-Samples). Den här versionen innehåller uppdateringar av följande metoder:

#### <a name="audit-updated-new-operation-types"></a>Granska uppdaterad: Nya åtgärdstyper

Nya [åtgärdstyper har lagts](https://docs.microsoft.com/partner-center/develop/auditing-resources) till för att veta när kunden godkänt och avslutat DAP.

- DapAdminRelationshipApproved

- DapAdminRelationshipTerminated

#### <a name="audit-updated-new-resource-and-operation-types"></a>Granska uppdaterad: Nya resurs- och åtgärdstyper

Nya [resurs- och åtgärdstyper har lagts](https://docs.microsoft.com/partner-center/develop/auditing-resources) till för att stödja scenariot med kundkatalogrollen.

- Ny resurstyp: "CustomerDirectoryRole"

- Åtgärdstyperna "AddUserMember" och "RemoveUserMember"

#### <a name="sdk-updates-to-customer-accounts"></a>SDK-uppdateringar till kundkonton

- Stöd för GET /customers/{customer-tenant-id}/directSignedMicrosoftCustomerAgreementStatus

- GET /customers/{customer-tenant-id}/kvalificering

- POST /customers/{customer_id}/qualifications?code={validationCode}

#### <a name="additional-changes"></a>Ytterligare ändringar

Följande ändringar introduceras som en del av New Commerce och är för närvarande endast tillgängliga genom inbjudan till partner som ingår i den tekniska förhandsversionen av den nya M365/D365-upplevelsen. Partner som inte är en del av den tekniska förhandsversionen av Ny handel bör inte märka påverkan och bör vara bakåtkompatibla.

- Katalogändringar:

  - GET /products/{product-id}/skus/{sku-id}

- Köp och hantera:
  - GET /customers/{customerId}/subscriptions
  - GET /customers/{customerId}/subscriptions/{subscriptionId}
  - PATCH /customers/{customerId}/subscriptions/{subscriptionId}
  - GET /customers/{customerId}/subscriptions/{subscriptionId}/transitioneligibilities
  - GET /customers/{customerId}/subscriptions/{subscriptionId}/transitions
  - POST /customers/{customerId}/subscriptions/{subscriptionId}/transitions

### <a name="next-steps"></a>Nästa steg

- Ladda ned den senaste [versionen av MicrosoftPartnerCenter.NETSDK (NuGet-| Microsoft.Store.PartnerCenter 1.17.0)](https://www.nuget.org/packages/Microsoft.Store.PartnerCenter/1.17.0)
- Ladda ned och granska [GitHub-exemplen](https://github.com/Microsoft/Partner-Center-DotNet-Samples)

________________
## <a name="csp-commercial-marketplace-offer-and-fy21-csp-incentives-for-eligible-offers"></a><a name="12"></a>CSP Commercial Marketplace-erbjudande och FY21 CSP-incitament för berättigade erbjudanden

### <a name="categories"></a>Kategorier

- Datum: 2021-03-18
- Funktioner

### <a name="impacted-audience"></a>Påverkad målgrupp

Indirekta leverantörer och direktfaktureringspartner i Molnlösningsleverantör program 

### <a name="details"></a>Information

Indirekta leverantörer och direktfaktureringspartner i Molnlösningsleverantör-programmet kan sälja erbjudanden från tredje part och få incitament för varje kvalificerande tredjepartserbjudande som erbjuds i Partnercenter eller Azure Portal. Incitamentet är i form av en kontakt med fakturerad försäljning för de berättigade erbjudandena och är tillgängligt fram till **den 30 juni 2021.**  

Fortsätt lära dig mer om denna CSP Commercial Marketplace-erbjudande nedan och kontakta dina kunder idag för att identifiera rätt erbjudanden för att möjliggöra fortsatt framgång och digital omvandling.

Vi samarbetar med oberoende programvaruleverantörer (ISV: er) för att få de senaste IaaS- och SaaS-lösningarna till marknaden för Microsoft-kunder. ISV-utgivare har möjlighet att aktivera försäljning av sina erbjudanden via Microsofts partnerkanal. Våra incitamentberättigade erbjudanden är indela i två kategorier:

- Välj SaaS- och IaaS-erbjudanden från tredje part med incentiviserad status för sälj- och säljförsäljning i Azure IP. 

- SaaS-program som är integrerade med Teams eller minst två Microsoft 365 produktivitetsappar, till exempel PowerPoint, Word, Excel, Outlook eller SharePoint.

### <a name="next-steps-and-resources"></a>Nästa steg och resurser

- Lär dig mer om att [tjäna partnerincitament](https://partner.microsoft.com/membership/partner-incentives) för att sälja berättigade Marketplace-appar för berättigade incitamentappar. Nya erbjudanden läggs till varje månad.  
- [Molnlösningsleverantör direktfakturering av partnerincitamentresurser](https://partner.microsoft.com/asset/collection/cloud-solution-provider-direct-partner-incentive-resources#/)
- [Molnlösningsleverantör incitamentresurser för indirekta leverantörer](https://partner.microsoft.com/asset/collection/cloud-solution-provider-indirect-provider-incentive-resources#/)
- Läs den här [presentationen](https://partner.microsoft.com/resources/detail/partner-center-cm-for-csp-overview-pdf) om du vill veta mer om att sälja appar på den kommersiella marknadsplatsen. Kolla in ytterligare resurser [här.](https://partner.microsoft.com/resources/collection/partner-center-cm-for-csp-collection#/) 
- Utforska katalogen för den kommersiella marknadsplatsen [i Partnercenter](https://docs.microsoft.com/partner-center/csp-commercial-marketplace-discover) [eller Azure Portal](https://ms.portal.azure.com/#home)
- Använda [API:er](https://docs.microsoft.com/partner-center/develop/create-subscription-azure-marketplace-products#get-a-list-of-offers-for-a-market) för att integrera appar på företagets marknadsplats
- Kontakta ISV:er som du är intresserad av att göra affärer med
- Indirekta leverantörer måste integrera med hjälp av API:er och vägleda återförsäljare om vilka appar som ska säljas

### <a name="questions"></a>Har du några frågor?  

I den [här artikeln](https://docs.microsoft.com/partner-center/csp-commercial-marketplace-overview) finns en översikt över den kommersiella marknadsplatsen i Partnercenter.

Om du behöver ytterligare hjälp kan du skapa en supportbegäran i Partnercenter. Läs mer på [https://aka.ms/IncentivesSupport](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=1) .

________________
## <a name="power-bi-premium-offer-naming-and-prerequisite-update"></a><a name="11"></a>Power BI Premium för namn och kravuppdatering

### <a name="categories"></a>Kategorier

- Datum: 2021-03-18
- Funktioner

### <a name="summary"></a>Sammanfattning

Den slutliga prislistan för den 1 april 2021 uppdateras för att förtydliga namngivnings- och/eller kravinformationen för erbjudanden Power BI Premium per användare.

### <a name="impacted-audience"></a>Påverkad målgrupp

Molnlösningsleverantör (CSP) direkta och indirekta partner

### <a name="details"></a>Information

Den slutliga prislistan för den 1 april 2021 uppdateras för att förtydliga namngivnings- och/eller kravinformationen för de Power BI Premium per användare.

Tills den slutliga prislistan har uppdaterats använder du informationen i det här avsnittet för att säkerställa att rätt produkt har beställts.

Följande information visar den berörda SKU:n och kravinformation.

| Erbjudandevisningsnamn den 1 mars – förhandsversion av prislista |  Uppdaterad erbjudandevisningsnamn den 1 april slutprislista| Erbjudande-ID |
| ------ | ----------- | ----------- |
| Power BI Premium per användare Add-On (prissättning för ideell personal)  |  Power BI Premium per Add-On **(Office)** (prissättning för ideell personal)   | 31c03289-47ab-4ab0-8df1-03742c127ac6   |

Kunder måste ha något av följande förhandskrav för att köpa det här erbjudandet:

| Erbjudandets visningsnamn | Erbjudande-ID |
| ------ | ----------- |
| Microsoft 365 E5 (prissättning för ideell personal)  |  31bedf01-9e57-4ece-a53a-d3656a563931   |
|   Microsoft 365 E5 utan ljudkonferens (prissättning för ideell personal)|  b456810a-c414-4e07-98fc-ef74e8175a09|
|   Office 365 E5 (prissättning för ideell personal)| ce139fe5-8bd5-47ed-a5be-07c286f8b9e    |
|   Utvärderingsversion av Office 365 E5 (prissättning för ideell personal)|  2f192efe-608a-4c9c-9d19-2b0b70b0962e|
|   Office 365 E5 utan ljudkonferens (prissättning för ideell personal)|  c3897426-9f49-4eaf-9b4d-7d9a1c72aef7|

Följande erbjudande Power BI Premium ett förhandskrav för inköp:

| Erbjudandets visningsnamn | Erbjudande-ID |
| ------ | ----------- |
|   Power BI Premium per Add-On (prissättning för ideell personal)|  ef0b895b-681b-4026-a5b1-dda182a57d40 |

Kunder måste ha detta förhandskrav för att kunna köpa det här erbjudandet:

| Erbjudandets visningsnamn | Erbjudande-ID |
| ------ |----------|
| Power BI Pro (prissättning för ideell personal)  |   cabdfc93-5786-4224-bfd3-35d58f833b35 |

### <a name="next-steps"></a>Nästa steg

Granska resurserna om det här avsnittet och dela den här informationen med lämpliga intressenter i din organisation.  

### <a name="questions"></a>Har du några frågor?

Om du har frågor om dessa erbjudanden kan du kontrollera dina relevanta Yammer-communities. 

## <a name="march-price-updates-for-microsoft-365-f3"></a><a name="10"></a> Prisuppdateringar mars för Microsoft 365 F3

### <a name="categories"></a>Kategorier

- Datum: 2021-03-16
- Erbjudanden/marknader

### <a name="summary"></a>Sammanfattning

Felaktig prissättning för mars 2021 har korrigerats för Microsoft 365 F3 British Pound (GBP) och EURO (EUR).

### <a name="impacted-audience"></a>Målgrupp som påverkas

Partner som köper Microsoft 365 F3 i Gbit/s eller EUR mellan 1 mars och 17 mars 2021 via programmet Molnlösningsleverantör (CSP).

### <a name="details"></a>Information

Microsoft har löst felaktig prissättning för Microsoft 365 F3. De felaktiga priserna var för GBP och EUR och endast för erbjudanden som köpts mellan 1 mars och 17 mars 2021. De erbjudanden och valutor som påverkas visas nedan. 

| Erbjudandets namn | Valuta | Erbjudande-ID | Material-ID |
| ------ |----------- |----------- |----------- |
| Microsoft 365 F3 (Fc) | GBP | 57b722c2-c435-4bfb-9bc8-80509213a13a | AAD-11626 |
| Microsoft 365 F3 (kommersiell) | EUR| 3451a3b0-8cda-44a7-bad7-c30be81c4aaa | AAA-89898 |
 
Prislistorna för licensbas för mars och april uppdaterades 16 mars 17:00 Pacific Standard Time.

### <a name="next-steps"></a>Nästa steg

- Partner bör ladda ned de aktuella licensbaserade prislistorna på nytt, både mars och aprilförhandsvisningen, med dessa priskorrigeringar om tillämpligt.  
- Microsoft kommer att kontakta berörda partner under de kommande veckorna via e-post för att informera dem om nästa steg som rör korrigering av berörda transaktioner.

### <a name="questions"></a>Har du några frågor?

Om du har fler frågor kan du kontrollera dina relevanta CSP Yammer-communities.

________________

## <a name="update-a-legal-company-name-through-partner-center"></a><a name="9"></a> Uppdatera ett juridiskt företagsnamn via Partnercenter

### <a name="categories"></a>Kategorier

- Datum: 2021-03-16
- Skala för & effektivitet

### <a name="summary"></a>Sammanfattning

Från och med mars 2021 kan Microsoft Partner Network-partner (MPN) och indirekta Molnlösningsleverantör CSP-återförsäljare (CSP) uppdatera sina juridiska företagsnamn via Partnercenter.

### <a name="impacted-audience"></a>Påverkad målgrupp

MPN-partner och indirekta CSP-återförsäljare (gäller inte CSP-direktfaktureringspartner)

### <a name="details"></a>Information

Från och med mars 2021 kan MPN-partner och indirekta CSP-återförsäljare uppdatera sitt juridiska företagsnamn via Partnercenter på ett kompatibelt sätt med självbetjäning. Med den här nya funktionen behöver partner inte längre skicka en supportbiljett till Partnercenter för att uppdatera företagets namn. Detta sparar mycket tid för partner när de utför dessa aktiviteter. 

Mer information finns i [Uppdatera din juridiska företagsprofil.](../update-your-partner-profile.md#update-your-legal-business-profile)

>[!NOTE]
>Se till att företagets namn i din juridiska företagsprofil inte innehåller stavfel och förkortningar och exakt matchar företagets formella registreringsposter för företag. Mer information om hur du uppdaterar din organisationsprofil finns i [Verifiera din organisationsprofil.](../update-your-partner-profile.md#update-your-legal-business-profile)

### <a name="next-steps"></a>Nästa steg

Dela den här informationen i din organisation så att rätt team kan granska och uppdatera sina processer.

### <a name="questions"></a>Har du några frågor?

Om du har fler frågor kan du kontrollera dina relevanta CSP Yammer-communities.

________________
## <a name="update-to-cloud-solution-provider-csp-program-evolution-and-open-license-program-changes"></a><a name="8"></a> Uppdatera till Molnlösningsleverantör programutveckling (CSP) och ändringar i Open License-programmet

### <a name="categories"></a>Kategorier

- Datum: 2021-03-15
- Funktioner

### <a name="summary"></a>Sammanfattning

Nya kommersiella och offentliga programvaruerbjudanden kommer till CSP-programmet (Molnlösningsleverantör) tillsammans med ändringar i Open Licensing-programmet.

### <a name="impacted-audience"></a>Målgrupp som påverkas

Kommersiella distributörer och hanterade återförsäljare som säljer via Open License-programmet, samt alla CSP-partner som handlar permanent programvara

### <a name="details"></a>Information

I september 2020 presenterade [Microsoft](https://blogs.partner.microsoft.com/mpn/expanding-opportunities-for-partners-in-the-cloud-solution-provider-program/) en serie steg i vår digitala omvandlingsresa för att utöka möjligheterna till partner i CSP-programmet, inklusive tillgängligheten för lokal programvara för partner. Dessa ändringar gör det möjligt för partner att utöka sin verksamhet och sin räckvidd genom att utnyttja programvarulicenser i CSP och positionera dem för framgång i dagens molnbaserade värld. De ger också kundernas övergångar till molnet och ger partner den flexibilitet som krävs för kundernas hybridmolnmiljöer.

I fortsättningen på den här digitala omvandlingen presenterar vi följande ändringar:

- 1 juli 2021: Inga nya SKU:er, produkter eller kampanjer kommer att läggas till i prislistan för Open License-programmet.

- 7 juli 2021: Två kommersiella erbjudanden, Get Genuine Windows och Visual Studio Professional, och erbjudanden inom den offentliga sektorn (myndigheter, utbildning och ideella organisationer – se [meddelande)](./2020-december.md#9)kommer att läggas till i CSP:s löpande prislista för programvara.  Prislistan finns i avsnittet Programvara på sidan [Säljpriser >](https://partnercenter.microsoft.com/pcv/sales) & i Partnercenter och publiceras på nytt det här datumet.

Fullständig information om CSP-programutvecklingen och ändringar i Open License-programmet finns i **Nästa steg** nedan.

### <a name="next-steps"></a>Nästa steg:

- Utveckling av CSP-program: Granska den beständiga [programvaran i Molnlösningsleverantör för programberedskap.](https://partner.microsoft.com/resources/collection/software-in-csp#/) Använd [beredskapskartan](https://partner.microsoft.com/resources/detail/software-in-csp-readiness-map-pdf) för att snabbt hitta rätt information för din roll.

- Öppna Ändringar av licensprogram: Granska [CSP-programutvecklingen och Ändra](https://partner.microsoft.com/resources/collection/csp-open-evolution-to-a-better-experience#/) beredskapsmaterial för Open License Program. Använd [beredskapskartan](https://partner.microsoft.com/resources/detail/csp-open-evolution-to-a-better-experience-readiness-map-pdf) för att snabbt hitta rätt information för din roll.

### <a name="questions"></a>Frågor

Om du har fler frågor kan du kontrollera dina relevanta CSP Yammer-communities.

_______________
## <a name="update-to-a-previous-announcement-premium-assessments-an-add-on-to-compliance-manager"></a><a name="7"></a>Uppdatera till ett tidigare meddelande: Premium Assessments, ett tillägg till Compliance Manager

### <a name="categories"></a>Kategorier

- Datum: 2021-03-15
- Utveckla verksamheten

### <a name="summary"></a>Sammanfattning

Utvärderingserbjudandena bör inte ha listats i prislistan och tas bort.

### <a name="impacted-audience"></a>Målgrupp som påverkas

Partner som gör en Molnlösningsleverantör

### <a name="details"></a>Information

Utvärderingserbjudandena bör inte ha inkluderats i prislistan. Dessa tas bort från prislistan 1 maj 2021.

Det ursprungliga meddelandet finns [här.](./2021-february.md#4)

### <a name="additional-resources"></a>Ytterligare resurser

- [Microsoft 365 säkerhet och efterlevnad för E5](https://www.microsoft.com/licensing/product-licensing/microsoft-365-enterprise?activetab=m365-enterprise:primaryr5)

- [Skapa och hantera utvärderingar i Microsoft Compliance Manager – Microsoft 365 efterlevnad](/microsoft-365/compliance/compliance-manager-assessments)

### <a name="next-steps"></a>Nästa steg

Granska resurserna om det här avsnittet och dela den här informationen med lämpliga intressenter i din organisation.

### <a name="questions"></a>Har du några frågor?

Frågor om dessa erbjudanden finns i dina relevanta Yammer-communities.

________________
## <a name="migrate-your-solutions-from-one-commercial-partner-ocp-go-to-market-gtm-to-the-microsoft-commercial-marketplace"></a><a name="6"></a> Migrera dina lösningar från EN kommersiell partner (OCP) till Microsofts kommersiella marknadsplats

### <a name="categories"></a>Kategorier

- Datum: 2021-03-12
- Funktioner

### <a name="summary"></a>Sammanfattning

Från och med 29 mars 2021 kommer du att få begränsade FUNKTIONER för EN kommersiell partner (OCP) på marknaden (GTM). Vi rekommenderar att du migrerar dina lösningar till den kommersiella marknadsplatsen i Partnercenter.

### <a name="impacted-audience"></a>Påverkad målgrupp

Organisationer som samarbetar med lösningar i OCP GTM

### <a name="details"></a>Information

I december 2020 påbörjade vi vår resa från Verktyget Microsoft OCP GTM till Microsofts kommersiella marknadsplats i Partnercenter. Den här övergången utökar funktionerna på den kommersiella marknadsplatsen där du kan demonstrera dina lösningar för miljontals kunder, dela affärsmöjligheter med andra Microsoft- och partnerförsäljningar och gemensamt sälja innovativa lösningar.

Nästa milstolpe i övergången sker den 29 mars 2021. Det är då du börjar uppleva begränsade OCP GTM-funktioner, där vissa fält blir skrivskyddade. Om du för närvarande samarbetar med lösningar i OCP GTM rekommenderar vi att du migrerar dina lösningar till den kommersiella marknadsplatsen för att dra nytta av dess funktioner och förenkla din publiceringsupplevelse. 

Att flytta till den kommersiella marknadsplatsen gör Partner Center till det primära målet för publiceringen av säljförsäljning. Det är här du kan fortsätta att utveckla din verksamhet genom att ansluta dina lösningar till våra delade kunder via samma kanaler och produktupplevelser som vi använder för Microsoft-produkter. [Läs mer om den kommersiella marknadsplatsen](https://blogs.partner.microsoft.com/mpn/getting-started-with-the-microsoft-commercial-marketplace/).

### <a name="next-steps"></a>Nästa steg

- Om du ännu inte har flyttat dina lösningar [](/azure/marketplace/co-sell-solution-migration) följer du anvisningarna i övergångsguiden eller visar den stegvisa videokursen för att slutföra alla [migreringsaktiviteter](https://partner.microsoft.com/asset/detail/ocp-gtm-to-the-microsoft-commercial-marketplace-mp4) och börja publicera dina lösningar på den kommersiella marknadsplatsen.

- Om du har frågor om den begränsade kapacitetsupplevelsen i OCP GTM kan du se krav på säljförsäljning för publicering på Microsofts kommersiella marknadsplats – vanliga [frågor och svar.](https://partner.microsoft.com/resources/detail/co-sell-requirements-publish-commercial-marketplace-faq-pdf) (Se avsnittet "OCP GTM-begränsade funktioner från och med 29 mars 2021.")

### <a name="questions"></a>Har du några frågor?

Kontakta [supporten](https://partner.microsoft.com/support/?stage=1) om du har frågor eller behöver mer information.

________________
## <a name="expanding-the-new-commerce-experience-in-the-cloud-solution-provider-csp-program-for-azure-to-russia"></a><a name="5"></a>Utöka den nya handelsupplevelsen i programmet Molnlösningsleverantör (CSP) för Azure till Ryssland

### <a name="categories"></a>Kategorier

- Datum: 2021-03-10
- Funktioner

### <a name="impacted-audience"></a>Målgrupp som påverkas

Alla partner i Ryssland går igenom programmet Molnlösningsleverantör (CSP).

### <a name="details"></a>Information

Från och med 10 mars 2021 är vi glada över att kunna presentera tillgängligheten för den nya handelsupplevelsen i **CSP för Azure i Ryssland.** Den här upplevelsen effektiviserar och förbättrar kundernas sätt att köpa och använda Azure-tjänster. Det ger även partner i CSP-programmet en konsekvent vy över Azure-priser över försäljningsork, USD-priser för global konsekvens, anpassning av faktureringsdatum och åtkomst till Azure Cost Management.

### <a name="next-steps"></a>Nästa steg

Det finns flera tillgängliga resurser som introducerar den nya Azure-handelsupplevelsen och ger ytterligare information. Hitta de senaste vanliga frågor och svar, decks, video och mer i [CSP Program Updates Resource Gallery](https://partner.microsoft.com/resources/collection/new-azure-experience-in-csp#/).

________________
## <a name="partner-center-software-license-key-and-download-fulfillment"></a><a name="4"></a>Partnercenter– programvarulicensnyckel och hämtningsuppfyllelse

### <a name="categories"></a>Kategorier

- Datum: 2021-03-04
- Funktioner

### <a name="summary"></a>Sammanfattning

Funktionen för nedladdning av programvara och licens för nyckeluppfyllelse i Partnercenter har återställts.

### <a name="impacted-audience"></a>Målgrupp som påverkas

Alla Molnlösningsleverantör (CSP) som gör permanenta programvarubeställningar och programvarubeställningar för serverprenumeration via Partnercenter

### <a name="details"></a>Information

Som svar på feedback från partnern omvärder vi funktionen för att uppfylla Partnercenter för att hämta programvaru- och licensnycklar för beständiga programvarubeställningar och programvaruordrar för serverprenumeration. Den återställs till sitt tidigare tillstånd innan den tas bort den 19 januari 2021. (Se [tillkännagivandet](2020-september.md#17).)

Observera att nycklar för programvarulicens och nedladdningslänkar är värdefulla och eftersökta immateriella tillgångar. Om de läcks kan de snabbt få slut på sina aktiveringsgränser och orsaka en negativ kund- och partnerupplevelse.

### <a name="next-steps"></a>Nästa steg

Granska följande resurser för användningsanvisningar och viktig vägledning om distribution av programvarunyckel:

- [Sälja lokal programvara via CSP-programmet](../csp-on-premise-software.md)
- [Partner Center New Commerce Operations Guide](https://partner.microsoft.com/resources/detail/partner-center-new-commerce-operations-guide-pdf) (se avsnittet Vägledning om distribution av **programvarunyckel.)**

### <a name="questions"></a>Har du några frågor?

Om du har ytterligare frågor om det här meddelandet kan du kontrollera dina relevanta Yammer-communities.

________________
## <a name="migrate-your-deals-from-partner-sales-connect-psc-to-partner-center"></a><a name="3"></a>Migrera dina avtal från Partner Sales Connect (PSC) till Partnercenter

### <a name="categories"></a>Kategorier

- Datum: 2021-03-04
- Funktioner

### <a name="summary"></a>Sammanfattning

Partner Sales Connect (PSC) kommer att gå över till skrivskyddade åtkomst från och med 31 mars 2021, så vi hoppas att du ska börja migrera dina avtal från PSC till PartnerCenter.

### <a name="impacted-audience"></a>Påverkad målgrupp

Partner med avtal i PSC

### <a name="details"></a>Information

Som en del av vårt delade engagemang för tillväxt är samförsäljning med **Microsoft** den väg som du kan använda för att bli **upptäckt,** leverera din expertis och utöka ditt kundfotavtryck för positiva kundresultat. Med ett genomsnittligt avtal som är **3,5** gånger snabbare än normalt kan du hantera din säljupplevelse i Partnercenter för att sälja direkt till kunder, partner och Microsoft-försäljningskanaler och hantera hela din hänvisningspipeline på en och samma plats.

**PSC** kommer  att gå över till skrivskyddade åtkomst från och med **31 mars 2021,** så vi hoppas att du börjar flytta till Partnercenter och få åtkomst till dessa kapacitetsförbättringar: 

- **Mer exakt routning** av de avtal som du delar med Microsoft till rätt säljare, baserat på vilken typ av hjälp du behöver.
- **Validering av berättigande för** förskottsberättigade avtal för incitamentberättigade lösningar och för att uppfylla kriterierna för ISV Connect-programmet, vilket förenklar godkännandeprocessen och POE-attestation (final proof of execution).
- **Smidig användarupplevelse** för att hantera alla dina möjligheter till säljförsäljning och säljkvalificerade leads på ett och samma ställe.

Vi har också nyligen lagt till nya funktioner i Partnercenter för att underlätta flytten:

- [Massåtgärder för möjligheter till säljförsäljning](../bulk-operations.md)
- [Avtalsmigreringsfunktionen](../psc-to-pc.md) (se **avsnittet om PSC-avtalsmigrering.)**

Med hjälp av säljupplevelsen i Partnercenter får säljteamen mer tid att fokusera på att hjälpa leads och affärsmöjligheter, stänga avtal och skapa varaktiga kundrelationer.

### <a name="next-steps"></a>Nästa steg

Använd [partnercenterövergångsguiden för](../psc-to-pc.md) att gå igenom stegen för att migrera dina avtal från PSC till Partnercenter.

### <a name="questions"></a>Har du några frågor?

Kontakta supporten för ytterligare [frågor.](https://partner.microsoft.com/support/?stage=1)

________________
## <a name="new-microsoft-dynamics-365-products-and-offers-available-on-april-1-2021"></a><a name="2"></a>Nya Microsoft Dynamics 365-produkter och -erbjudanden är tillgängliga den 1 april 2021

### <a name="categories"></a>Kategorier

- Datum: 2021-03-04
- Funktioner

### <a name="summary"></a>Sammanfattning

Den 1 april 2021 lanserar Microsoft flera nya produkter och erbjudanden för programmet Molnlösningsleverantör (CSP).

### <a name="impacted-audience"></a>Målgrupp som påverkas

Alla partner som gör en Molnlösningsleverantör (CSP)

### <a name="details"></a>Information

Den 1 april 2021 lanserar Microsoft följande nya produkter och erbjudanden:

- Power BI Premium per användare
- Usl-geo- och segmentexpansion för Customer Voice and Marketing

**Power BI Premium per användare**

Microsoft introducerar de första erbjudandena per användare Power BI Premium erbjudanden. Power BI Premium säljs för närvarande endast i en kapacitetskonstruktion. Power BI Premium per användare ger åtkomst till business intelligence (BI) och analysfunktioner. Dess flexibla individuella klientlicensiering riktar sig till små och medelstora företag.

Läs informationen [Power BI om du](/power-platform-release-plan/2020wave2/power-bi/planned-features) vill veta mer om det här erbjudandet.


**Erbjudandeinformation**

Observera att erbjudandets namn skiljer sig något från förhandsversionen av prislistan.

| Erbjudandets namn | Erbjudande-ID |
| ------ |----------- |
| Power BI Premium per användare | 9c810018-9356-4903-95ab-eeb956289290 | 
| Power BI Premium per användare för lärare och lärare | 3affc44f-f372-4ad5-8657-aadd9574fce0 | 
| Power BI Premium per användare för studenter | 657eea87-d0b0-4c89-8c8e-9b04395bd940 | 
| Power BI Premium per användare (prissättning för ideell personal) | 7a0a856c-059f-45dd-9d26-ae27992e706a | 
| Power BI Premium per användare Add-On | 244ff87e-5925-44a0-bf31-cea189719b58 | 
| Power BI Premium per Add-On för lärare och lärare | 5da849bd-b8f7-4340-b4f4-3a9eaeb8987e | 
| Power BI Premium per användare Add-On för studenter | cf62d70d-5af5-422a-bda8-97936402ac8e | 
| Power BI Premium per användare Add-On (prissättning för ideell personal) | 31c03289-47ab-4ab0-8df1-03742c127ac6 | 

**Customer Voice and Marketing USL geo and segmentexpansion**

Som en uppföljning till lanseringen i december 2020 har USL-erbjudanden för Dynamics 365 Customer Voice and Marketing ändrats för att lägga till nya länder och fler ideella organisationer och utbildnings-SKU:er.

| Erbjudandets namn | Erbjudande-ID |
| ------ |----------- |
| Dynamics 365 Customer Voice USL (prissättning för ideell personal) | 7a8642a5-481e-4906-a642-b56dbeeb62a0 |
| Dynamics 365 Customer Voice USL för lärare | 85162d70-9676-4cf6-a4bc-a0d6672f2657 |

Besök följande sidor om du vill veta mer om dessa erbjudanden:

- [Startsida för Dynamics 365 Customer Service Voice](https://dynamics.microsoft.com/customer-voice/overview/)
- [Startsida för Dynamics 365 Marketing](https://dynamics.microsoft.com/customer-voice/overview/)

### <a name="next-steps"></a>Nästa steg

Granska resurserna i det här avsnittet och dela den här informationen med lämpliga intressenter i din organisation.  

### <a name="questions"></a>Har du några frågor?

Om du har frågor om dessa erbjudanden kan du kontrollera dina relevanta Yammer-communities. 

________________
## <a name="microsoft-universal-print-now-available-in-some-suites"></a><a name="1"></a> Microsoft Universell utskrift nu tillgängligt i vissa paket

### <a name="categories"></a>Kategorier

- Datum: 2021-03-03
- Funktioner

### <a name="summary"></a>Sammanfattning

Microsoft Universell utskrift kommer att vara tillgängligt för att handla inom utvalda Microsoft 365-paket och som ett fristående tillägg från den 1 mars 2021.

### <a name="impacted-audience"></a>Påverkad målgrupp

Alla partner som gör en Molnlösningsleverantör via CSP-programmet

### <a name="details"></a>Information

[Universell utskrift](https://aka.ms/universalprint) är en Microsoft 365 utskriftstjänst som tar bort behovet av lokala utskriftsservrar och gör det möjligt för Windows-enheter att skriva ut till Azure-registrerade skrivare. Den kommer att vara tillgänglig för transact från den 1 mars 2021.

Arbetare drar nytta av drivrutinslöst utskrift, strömlinjeformad platsbaserad skrivaridentifiering och en intuitiv utskriftsupplevelse utan inlärningskurva. Enheter som är anslutna till Azure Active Directory (Azure AD) använder befintliga Azure AD-autentiseringsuppgifter för att skriva ut på ett säkert sätt. Administratörer hanterar utskrift med hjälp av Azure Portal och kan enkelt ansluta skrivare med inbyggt stöd för Universell utskrift. Universell utskrift kan distribueras med icke-kompatibla skrivare med hjälp av Anslutning för Universell utskrift programvara.

Universell utskrift återfylls vid start till Windows E3, A3, E5 och A5 och Microsoft 365 BP, F3, E3, A3, E5 och A5.  

**Erbjudandeinformation**

Observera att erbjudandets namn skiljer sig något från förhandsversionen av prislistan.

| Erbjudandets namn | Erbjudande-ID | Material-ID |
| ------ |----------- |----------- |  
| Universell utskrift volymökning (500 jobb) – Microsoft 365  | cb131356-45ee-4ae2-8537-873b706c8e75     | 9BI-00004   |
| Universell utskrift volymökning (500 jobb) för lärare och lärare – Microsoft 365   | 477 tb81-9872-43d6-91d3-c72390bfcf49   | 9BK-00004   |
| Universell utskrift volymökning (500 jobb) – Windows    | d3ddc493-5741-4e0d-a02d-07edbb0bb72e   | 9BI-00002   |
| Universell utskrift volym tillägg (500 jobb) för lärare – Windows   |  d0862f05-80f5-4fd4-8432-fe72dd893cc7  | 9BK-00002   |

### <a name="next-steps"></a>Nästa steg

Bekanta dig med prislistan och Universell utskrift [översikt](/universal-print/fundamentals/universal-print-whatis). Dela den här informationen med alla lämpliga kontakter i din organisation.

### <a name="questions"></a>Har du några frågor?

Om du har frågor om dessa erbjudanden kan du kontrollera dina relevanta Yammer-communities.
