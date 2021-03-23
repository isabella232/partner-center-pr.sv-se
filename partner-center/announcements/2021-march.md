---
title: Meddelanden i mars 2021
description: Mars 2021-meddelanden för Microsoft Partner Center, inklusive nya funktioner, kampanjer, erbjudanden, marknader eller ändringar av befintliga erbjudanden.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: brentserbus
ms.author: brserbus
ms.custom: announcement
ms.localizationpriority: high
ms.date: 03/22/2021
ms.openlocfilehash: a3172b78d41a966b52a824703a7f15f163467d63
ms.sourcegitcommit: 715368e56fe669d29c7981906e08bc8d7d5d62a4
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/23/2021
ms.locfileid: "104880743"
---
# <a name="march-2021-announcements"></a>Meddelanden i mars 2021

Den här sidan innehåller meddelandena för Microsoft Partner Center för mars 2021.

________________
## <a name="corrections-made-to-march-1-2021-perpetual-software-price-list"></a><a name="14"></a>Korrigeringar gjorda till den 1 mars 2021-pris listan för beständig program vara

### <a name="categories"></a>Kategorier

- Datum: 2021-03-23
- Erbjudanden/marknader

### <a name="impacted-audience"></a>Förverkad mål grupp

Indirekta leverantörer och direkta fakturerings partner som agerar med beständig program vara i Cloud Solution Provider-programmet 

### <a name="details"></a>Information

Pris listan för beständig program vara som publicerades den 1 mars 2021 ingår marknader som inte borde ha funnits där. Pris listan för beständig program vara uppdaterades den 17 mars 2021 med korrigeringarna. Dessa korrigeringar gäller endast:

- Produkt-ID: DF77X4D43RKT 
- Produkt namn: Windows 10 Home till Pro-uppgradering för Microsoft 365 Business
- Borttagna eller ej stödda marknader: AE, AF, AL, AM, AO, BA, BB, BD, BH, BM, BN, BO, BR, BS, BW, BZ, CI, CL, CM, CO, CR, FV, DZ, EG, tex, ET, FJ, FO, GE, Last, GT, HN, IL, i, SWEETIQ, JM, Eva, KE, KG, KN, KW, KY, KZ, LB, LK, LY, MA, MC, MD, MN, MO, MK, NA , NI, NP, OM, PA, PE, PH, PK, PR, PY, FRÅGOR OCH SVAR, RS, RU, RW, TG, SN, SA, TH, TJ, TM, TN, TT, TZ, UA, ΜG, UY, UZ, VE, VN, JULEN, ZM, ZW

Dessa ändringar gäller endast för produkten ovan. Andra produkter hade inga ändringar. 

### <a name="next-steps-and-resources"></a>Nästa steg och resurser

- Partner som har en Transact-beständig program vara bör ladda ned den senaste pris listan för beständig program vara.
- Se [lands koderna för regioner](https://docs.microsoft.com/azure/marketplace/commercial-marketplace-co-sell-countries) för en egen mappning av den två bokstavs förkortningen till länder.
________________
## <a name="sdk-release-on-net-standard-v1170"></a><a name="13"></a> SDK-version på .NET standard (v 1.17.0)

### <a name="categories"></a>Kategorier

- Datum: 2021-03-23

- Funktioner
 
### <a name="impacted-audience"></a>Förverkad mål grupp

Direkta fakturerings partner och indirekta leverantörer som deltar i CSP-programmet som använder Partner Center .NET SDK.

### <a name="details"></a>Information

Från och med mars 23 2020 kan partners börja hämta versionen av [MicrosoftPartnerCenter. NETSDK (NuGet Galleri | Microsoft. Store. PartnerCenter 1.17.0)](https://www.nuget.org/packages/Microsoft.Store.PartnerCenter/1.17.0)tillsammans med uppdaterade offentliga partners Center SDK [GitHub-exempel](https://github.com/Microsoft/Partner-Center-DotNet-Samples). Den här versionen innehåller uppdateringar av följande metoder:

#### <a name="audit-updated-new-operation-types"></a>Granskning uppdaterad: nya åtgärds typer

Nya [Åtgärds typer](https://docs.microsoft.com/partner-center/develop/auditing-resources) har lagts till för att veta när kunden godkände och avslutade DAP.

- DapAdminRelationshipApproved

- DapAdminRelationshipTerminated

#### <a name="audit-updated-new-resource-and-operation-types"></a>Granskning uppdaterad: nya resurs-och åtgärds typer

Nya [resurs-och åtgärds typer](https://docs.microsoft.com/partner-center/develop/auditing-resources) har lagts till för att stödja scenariot för kund katalog roller.

- Ny resurs typ "CustomerDirectoryRole"

- Åtgärds typer "AddUserMember" och "RemoveUserMember"

#### <a name="sdk-updates-to-customer-accounts"></a>SDK-uppdateringar till kund konton

- Stöd för GET/customers/{customer-tenant-id}/directSignedMicrosoftCustomerAgreementStatus

- Hämta/Customers/{Customer-Tenant-ID}/Qualifications

- PUBLICERA/Customers/{customer_id}/Qualifications? Code = {validationCode}

#### <a name="additional-changes"></a>Ytterligare ändringar

Följande ändringar införs som en del av New Commerce och är för närvarande endast tillgängliga genom inbjudan till partner som är en del av M365/D365 nya Commerce Experience Technical Preview. Partner som inte ingår i den nya Commerce Technical Preview bör inte märkas och bör vara bakåtkompatibla.

- Katalog ändringar:

  - Hämta/Products/{Product-ID}/SKUs/{SKU-ID}

- Köp och hantera:
  - Hämta/customers/{customerId}/subscriptions
  - Hämta/customers/{customerId}/subscriptions/{subscriptionId}
  - KORRIGERINGs/customers/{customerId}/subscriptions/{subscriptionId}
  - Hämta/customers/{customerId}/subscriptions/{subscriptionId}/transitioneligibilities
  - Hämta/customers/{customerId}/subscriptions/{subscriptionId}/transitions
  - PUBLICERA/customers/{customerId}/subscriptions/{subscriptionId}/transitions

### <a name="next-steps"></a>Nästa steg

- Ladda ned den senaste versionen [MicrosoftPartnerCenter. NETSDK (NuGet Gallery | Microsoft. Store. PartnerCenter 1.17.0)](https://www.nuget.org/packages/Microsoft.Store.PartnerCenter/1.17.0)
- Hämta och granska [GitHub-exemplen](https://github.com/Microsoft/Partner-Center-DotNet-Samples)

________________
## <a name="csp-commercial-marketplace-offer-and-fy21-csp-incentives-for-eligible-offers"></a><a name="12"></a>Erbjudande om kommersiella Marketplace-erbjudanden och FY21 för berättigade erbjudanden

### <a name="categories"></a>Kategorier

- Datum: 2021-03-18
- Funktioner

### <a name="impacted-audience"></a>Förverkad mål grupp

Indirekta leverantörer och direkta fakturerings partner i Cloud Solution Provider-programmet 

### <a name="details"></a>Information

Indirekta leverantörer och direkta fakturerings partner i Cloud Solution Provider-programmet kan sälja tredje parts erbjudanden och få rabatt incitament för varje berättigad tredje parts erbjudande i Partner Center eller Azure Portal. Stimulans beloppet är i form av en rabatt på fakturerad försäljning för berättigade erbjudanden och är **tillgänglig fram till den 30 juni 2021**.  

Fortsätt att lära dig det här erbjudandet om erbjudandet om marknads plats erbjudande nedan och kontakta kunderna idag för att identifiera de rätta erbjudandena för att möjliggöra fortsatt lyckad och digital omvandling.

Vi samarbetar med oberoende program varu leverantörer (ISV) för att få de senaste IaaS-och SaaS-lösningarna till marknaden för Microsoft-kunder. ISV-utgivare kan välja att aktivera försäljning av sina erbjudanden via Microsoft Partner Channel. Våra incitaments berättigade erbjudanden delas in i två kategorier:

- Välj SaaS-och IaaS-erbjudanden från tredje part med Azure IP Co-Sälj motiverade status. 

- SaaS-program som är integrerade med team eller minst två Microsoft 365 produktivitets appar, till exempel PowerPoint, Word, Excel, Outlook eller SharePoint.

### <a name="next-steps-and-resources"></a>Nästa steg och resurser

- Lär dig om bidrags [partner incitament](https://partner.microsoft.com/membership/partner-incentives) för att sälja berättigade Marketplace-appar till de incitament som är berättigade till appar. Nya erbjudanden läggs till varje månad.  
- [Vår leverantör av moln lösningar direkt fakturerings partner stimulans resurser](https://partner.microsoft.com/asset/collection/cloud-solution-provider-direct-partner-incentive-resources#/)
- [Moln lösnings leverantörs tjänst för indirekt leverantörs stimulans](https://partner.microsoft.com/asset/collection/cloud-solution-provider-indirect-provider-incentive-resources#/)
- Läs igenom den här [presentationen](https://partner.microsoft.com/resources/detail/partner-center-cm-for-csp-overview-pdf) om du vill veta mer om hur du säljer kommersiella Marketplace-appar. Kolla in ytterligare resurser [här](https://partner.microsoft.com/resources/collection/partner-center-cm-for-csp-collection#/). 
- Utforska den kommersiella Marketplace-katalogen i [partner Center](https://docs.microsoft.com/partner-center/csp-commercial-marketplace-discover) eller [Azure Portal](https://ms.portal.azure.com/#home)
- Använd [API: er](https://docs.microsoft.com/partner-center/develop/create-subscription-azure-marketplace-products#get-a-list-of-offers-for-a-market) för att integrera appar i ditt företags marknads plats
- Kontakta ISV: er som du är intresse rad av att göra affärer med
- Indirekta leverantörer måste integreras med API: er och guide åter försäljare där appar kan säljas

### <a name="questions"></a>Har du några frågor?  

I [den här artikeln](https://docs.microsoft.com/partner-center/csp-commercial-marketplace-overview) hittar du en översikt över den kommersiella marknads platsen i Partner Center.

Om du behöver ytterligare hjälp kan du skapa en supportbegäran i Partner Center. Läs mer på [https://aka.ms/IncentivesSupport](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=1) .

________________
## <a name="power-bi-premium-offer-naming-and-prerequisite-update"></a><a name="11"></a>Power BI Premium erbjuder namngivning och nödvändig uppdatering

### <a name="categories"></a>Kategorier

- Datum: 2021-03-18
- Funktioner

### <a name="summary"></a>Sammanfattning

Den slutgiltiga pris listan 1 april 2021 kommer att uppdateras för att lägga till klarhet i namngivnings-och/eller nödvändig information för Power BI Premium per användare-erbjudanden.

### <a name="impacted-audience"></a>Förverkad mål grupp

Leverantörer av moln lösningar (CSP), direkta och indirekta partner

### <a name="details"></a>Information

Den slutgiltiga pris listan 1 april 2021 kommer att uppdateras för att lägga till klarhet i namngivnings-och/eller nödvändig information för Power BI Premium per användare-erbjudanden.

Innan den slutgiltiga pris listan har uppdaterats kan du använda informationen i det här avsnittet för att se till att rätt produkt beställs.

Följande information visar den berörda SKU: n och nödvändig information.

| Visnings namn för erbjudande 1 mars för hands version av pris lista |  Uppdaterat erbjudandets visnings namn den 1 april, slutgiltiga pris listan| Erbjudande-ID |
| ------ | ----------- | ----------- |
| Power BI Premium per användare Add-On (prissättning i ideell personal)  |  Power BI Premium per användare Add-On **(Office)** (prissättning i ideell personal)   | 31c03289-47ab-4ab0-8df1-03742c127ac6   |

Kunder måste ha något av följande krav för att köpa erbjudandet:

| Erbjudandets visnings namn | Erbjudande-ID |
| ------ | ----------- |
| Microsoft 365 E5 (pris för ideell personal)  |  31bedf01-9e57-4ece-a53a-d3656a563931   |
|   Microsoft 365 E5 utan ljud konferens (pris för ideell personal)|  b456810a-c414-4e07-98fc-ef74e8175a09|
|   Office 365 E5-pris (ideell personal)| ce139fe5-8bd5-47ed-a5be-07c286f8b9e    |
|   Utvärderings version av Office 365 E5 (ideell personal)|  2f192efe-608a-4c9c-9d19-2b0b70b0962e|
|   Office 365 E5 utan ljud konferens (pris för ideell personal)|  c3897426-9f49-4eaf-9b4d-7d9a1c72aef7|

Följande Power BI Premiums erbjudande måste ha ett krav för köp:

| Erbjudandets visnings namn | Erbjudande-ID |
| ------ | ----------- |
|   Power BI Premium per användare Add-On (prissättning i ideell personal)|  ef0b895b-681B-4026-a5b1-dda182a57d40 |

Kunder måste ha denna förutsättning för att kunna köpa detta erbjudande:

| Erbjudandets visnings namn | Erbjudande-ID |
| ------ |----------|
| Power BI Pro (pris för ideell personal)  |   cabdfc93-5786-4224-bfd3-35d58f833b35 |

### <a name="next-steps"></a>Nästa steg

Granska resurserna om det här avsnittet och dela den här informationen med lämpliga intressenter i din organisation.  

### <a name="questions"></a>Har du några frågor?

Om du har frågor om dessa erbjudanden kan du kontrol lera dina relevanta Yammer-communities. 

## <a name="march-price-updates-for-microsoft-365-f3"></a><a name="10"></a> Pris uppdateringar i mars för Microsoft 365 F3

### <a name="categories"></a>Kategorier

- Datum: 2021-03-16
- Erbjudanden/marknader

### <a name="summary"></a>Sammanfattning

Felaktigt mars 2021-pris har korrigerats för Microsoft 365 F3 Storbritannien (GBP) och euro (EUR).

### <a name="impacted-audience"></a>Förverkad mål grupp

Partner köper Microsoft 365 F3 i GBP eller EUR mellan 1 mars och 17 mars 2021 med hjälp av CSP-programmet (Cloud Solution Provider).

### <a name="details"></a>Information

Microsoft har löst felaktig prissättning för Microsoft 365 F3. De felaktiga priserna var för GBP och EUR och endast för erbjudanden som köpts mellan 1 mars och 17 mars 2021. De påverkade erbjudandena och valutorna visas nedan. 

| Erbjudandets namn | Valuta | Erbjudande-ID | Material-ID |
| ------ |----------- |----------- |----------- |
| Microsoft 365 F3 (välgörenhet) | GBP | 57b722c2-c435-4bfb-9bc8-80509213a13a | AAD-11626 |
| Microsoft 365 F3 (kommersiell) | EUR| 3451a3b0-8cda-44a7-bad7-c30be81c4aaa | AAA-89898 |
 
Licensen för för hands versionen av mars och april har uppdaterats 16 mars, 17 Pacific, normal tid.

### <a name="next-steps"></a>Nästa steg

- Partner bör hämta de aktuella licensbaserade pris listorna, både mars och för hands versionen av april, med dessa pris korrigeringar om det är tillämpligt.  
- Microsoft kontaktar berörda partner i kommande veckor via e-post för att informera dem om nästa steg som rör korrigering av berörda transaktioner.

### <a name="questions"></a>Har du några frågor?

Om du behöver fler frågor kontrollerar du dina relevanta CSP-communities.

________________

## <a name="update-a-legal-company-name-through-partner-center"></a><a name="9"></a> Uppdatera ett juridiskt företags namn via partner Center

### <a name="categories"></a>Kategorier

- Datum: 2021-03-16
- & skala för enhets effektivitet

### <a name="summary"></a>Sammanfattning

Från och med 2021 mars, Microsoft Partner Network (MPN) partner och indirekt åter försäljare av moln lösnings leverantör kan uppdatera sitt juridiska företags namn via partner Center.

### <a name="impacted-audience"></a>Förverkad mål grupp

MPN-partner och indirekta CSP-åter försäljare (gäller inte för CSP direkt fakturerings partner)

### <a name="details"></a>Information

Från och med 2021 mars kan MPN-partner och indirekta CSP-återförsäljare uppdatera sitt juridiska företags namn via partner Center på ett kompatibelt och självständigt sätt. Med den här nya funktionen behöver partners inte längre skicka ett support ärende för partner Center för att uppdatera företagets namn. Detta sparar en betydande del av tiden för partner när du utför dessa aktiviteter. 

Mer information finns i [Uppdatera din juridiska företags profil](../update-your-partner-profile.md#update-your-legal-business-profile).

>[!NOTE]
>Se till att företags namnet i din juridiska företags profil är fritt från stavfel och förkortningar, och exakt matchar dina formella företags registrerings poster. Mer information om hur du uppdaterar din organisations profil finns i [Verifiera din organisations profil](../update-your-partner-profile.md#update-your-legal-business-profile).

### <a name="next-steps"></a>Nästa steg

Dela den här informationen i din organisation så att rätt team kan granska och uppdatera sina processer.

### <a name="questions"></a>Har du några frågor?

Om du behöver fler frågor kontrollerar du dina relevanta CSP-communities.

________________
## <a name="update-to-cloud-solution-provider-csp-program-evolution-and-open-license-program-changes"></a><a name="8"></a> Uppdatera till program utveckling i Cloud Solution Provider (CSP) och öppna licens programs ändringar

### <a name="categories"></a>Kategorier

- Datum: 2021-03-15
- Funktioner

### <a name="summary"></a>Sammanfattning

Nya program varor från kommersiell och offentlig sektor kommer till program vara från Cloud Solution Provider (CSP) tillsammans med ändringar i Open License-programmet.

### <a name="impacted-audience"></a>Förverkad mål grupp

Kommersiella åter försäljare och hanterade åter försäljare som säljer genom Open License-programmet, samt alla CSP-partner som agerar beständig program vara

### <a name="details"></a>Information

I september 2020 [presenterade](https://blogs.partner.microsoft.com/mpn/expanding-opportunities-for-partners-in-the-cloud-solution-provider-program/) Microsoft en serie steg i vår digitala omvandlings resa för att utöka möjligheterna till partner i CSP-programmet, inklusive tillgängligheten för lokala program för partner. De här ändringarna gör det möjligt för partner att växa sin verksamhet och utöka sin räckvidd genom att använda program varu licenser i CSP och placera dem på framgång i dagens moln – första världen. De ger också kunderna till gång till molnet och ger partner den flexibilitet som krävs för kundernas hybrid moln miljöer.

Vi presenterar följande ändringar i fortsättningen på den här digitala omvandlingen:

- 1 juli 2021: inga nya SKU: er, produkter eller kampanjer läggs till i pris listan öppna licens program.

- 7 juli 2021: två kommersiella erbjudanden, få äkta Windows-och Visual Studio Professional-erbjudanden och offentliga sektor erbjudanden (myndigheter, utbildning och icke-vinst – se [meddelande](./2020-december.md#9)) läggs till i listan med program varu pris listan med kryptografiprovider.  Pris listan finns i avsnittet program vara på sidan [sälj > priser för pris &](https://partnercenter.microsoft.com/pcv/sales) i Partner Center och kommer att publiceras på detta datum igen.

Fullständig information om hur du kan utveckla CSP-program och öppna licens program ändringar finns i **Nästa steg** nedan.

### <a name="next-steps"></a>Nästa steg:

- Utveckling av CSP-program: granska den ständiga [program varan i Cloud solution providers program](https://partner.microsoft.com/resources/collection/software-in-csp#/) beredskap material. Använd den här [beredskaps kartan](https://partner.microsoft.com/resources/detail/software-in-csp-readiness-map-pdf) för att snabbt hitta rätt information för din roll.

- Öppna licens program ändringar: granska [CSP-programmets utveckling och öppna licens programmet ändrar](https://partner.microsoft.com/resources/collection/csp-open-evolution-to-a-better-experience#/) beredskaps material. Använd den här [beredskaps kartan](https://partner.microsoft.com/resources/detail/csp-open-evolution-to-a-better-experience-readiness-map-pdf) för att snabbt hitta rätt information för din roll.

### <a name="questions"></a>Frågor

Om du behöver fler frågor kontrollerar du dina relevanta CSP-communities.

_______________
## <a name="update-to-a-previous-announcement-premium-assessments-an-add-on-to-compliance-manager"></a><a name="7"></a>Uppdatera till ett tidigare meddelande: Premium-utvärderingar, ett tillägg till Compliance Manager

### <a name="categories"></a>Kategorier

- Datum: 2021-03-15
- Utveckla verksamheten

### <a name="summary"></a>Sammanfattning

Utvärderings versionen har inte listats i pris listan och kommer att tas bort.

### <a name="impacted-audience"></a>Förverkad mål grupp

Partner som agerar via Cloud Solution Provider

### <a name="details"></a>Information

Utvärderings versionen får inte ha inkluderats i pris listan. De kommer att tas bort från pris listan 1 maj 2021.

Det ursprungliga meddelandet är [här](./2021-february.md#4).

### <a name="additional-resources"></a>Ytterligare resurser

- [Microsoft 365 E5-säkerhet och efterlevnad](https://www.microsoft.com/licensing/product-licensing/microsoft-365-enterprise?activetab=m365-enterprise:primaryr5)

- [Bygga och hantera utvärderingar i Microsoft Compliance Manager – Microsoft 365 efterlevnad](/microsoft-365/compliance/compliance-manager-assessments)

### <a name="next-steps"></a>Nästa steg

Granska resurserna om det här avsnittet och dela den här informationen med lämpliga intressenter i din organisation.

### <a name="questions"></a>Har du några frågor?

Om du har frågor om dessa erbjudanden kan du kontrol lera dina relevanta Yammer-communities.

________________
## <a name="migrate-your-solutions-from-one-commercial-partner-ocp-go-to-market-gtm-to-the-microsoft-commercial-marketplace"></a><a name="6"></a> Migrera dina lösningar från en kommersiell partner (OCP) go-to-Marketing (GTM) till Microsofts kommersiella marknads plats

### <a name="categories"></a>Kategorier

- Datum: 2021-03-12
- Funktioner

### <a name="summary"></a>Sammanfattning

Från och med den 29 mars 2021 kommer du att börja uppleva begränsade en OCP-funktion (kommersiell partner) (GTM). Vi rekommenderar att du migrerar dina lösningar till den kommersiella marknads platsen i Partner Center.

### <a name="impacted-audience"></a>Förverkad mål grupp

Organisationer som samsäljs med lösningar i OCP-GTM

### <a name="details"></a>Information

I december 2020 startade vi vår resa från Microsoft OCP GTM-verktyget till Microsofts kommersiella marknads plats i Partner Center. Den här över gången utökar funktionerna i den kommersiella marknads platsen där du kan presentera dina lösningar på miljon tals kunder, som dubbelriktat delar affärs möjligheter med andra Microsoft-och partner-säljare, och gemensamt säljer innovativa lösningar.

Nästa mil stolpe i över gången kommer att ske den 29 mars 2021. Det är när du börjar uppleva begränsade OCP GTM-funktioner, och vissa fält blir skrivskyddade. Om du för närvarande samverkar med lösningar i OCP GTM, rekommenderar vi att du migrerar dina lösningar till den kommersiella marknaden för att dra nytta av dess funktioner och förenkla publicerings upplevelsen. 

Om du flyttar till den kommersiella marknads platsen blir partner Center det främsta målet för publicerings upplevelsen i Co-försäljningen. Det är här du kan fortsätta att växa din verksamhet genom att ansluta dina lösningar till våra delade kunder via samma kanaler och produkt upplevelser som vi använder för Microsoft-produkter. [Läs mer om den kommersiella marknads platsen](https://blogs.partner.microsoft.com/mpn/getting-started-with-the-microsoft-commercial-marketplace/).

### <a name="next-steps"></a>Nästa steg

- Om du inte har flyttat dina lösningar än följer du instruktionerna som beskrivs i [över gångs guiden](/azure/marketplace/co-sell-solution-migration) eller visar [själv studie kursen](https://partner.microsoft.com/asset/detail/ocp-gtm-to-the-microsoft-commercial-marketplace-mp4) för att slutföra alla migreringsåtgärder och börja publicera dina lösningar på den kommersiella Marketplace.

- Om du har frågor om den begränsade kapacitets upplevelsen i OCP-GTM kan du Visa [samförsäljnings kraven för att publicera på vanliga frågor och svar om Microsoft kommersiella Marketplace](https://partner.microsoft.com/resources/detail/co-sell-requirements-publish-commercial-marketplace-faq-pdf). (Mer information finns i avsnittet "OCP GTM Limited capabilitity Started 29 mars 2021.")

### <a name="questions"></a>Har du några frågor?

Kontakta [supporten](https://partner.microsoft.com/support/?stage=1) om du har några frågor eller behöver mer information.

________________
## <a name="expanding-the-new-commerce-experience-in-the-cloud-solution-provider-csp-program-for-azure-to-russia"></a><a name="5"></a>Expandera den nya Commerce-upplevelsen i Cloud Solution Provider (CSP)-programmet för Azure till Ryssland

### <a name="categories"></a>Kategorier

- Datum: 2021-03-10
- Funktioner

### <a name="impacted-audience"></a>Förverkad mål grupp

Alla partner i Ryssland går igenom programmet för Cloud Solution Provider (CSP).

### <a name="details"></a>Information

Från och med den 10 2021 mars är vi glada att kunna meddela att den **nya Commerce-upplevelsen i CSP för Azure i Ryssland** är tillgänglig. Den här upplevelsen kommer att effektivisera och förbättra hur kunderna köper och använder Azure-tjänster. Det ger också partner i CSP-programmet en konsekvent vy över Azures priser i Sälj rörelserna, priset USD för global konsekvens, justering av fakturerings datum och åtkomst till Azure Cost Management.

### <a name="next-steps"></a>Nästa steg

Det finns flera tillgängliga resurser som introducerar den nya Azure Commerce-upplevelsen och ger ytterligare information. Hitta de senaste frågorna, kortlek, video och mycket mer i [CSP-programmet uppdateringar resurs Galleri](https://partner.microsoft.com/resources/collection/new-azure-experience-in-csp#/).

________________
## <a name="partner-center-software-license-key-and-download-fulfillment"></a><a name="4"></a>Partner Center licens nyckel för program vara och hämtnings klara

### <a name="categories"></a>Kategorier

- Datum: 2021-03-04
- Funktioner

### <a name="summary"></a>Sammanfattning

Hämtningen av Partner Center-program varan och licens nyckelns uppfyllelse funktion har återställts.

### <a name="impacted-audience"></a>Förverkad mål grupp

Alla leverantörer av moln lösnings leverantörer (CSP) samverkar med program varu beställningar för beständig och Server prenumeration via partner Center

### <a name="details"></a>Information

Som svar på feedback från partnern är vi återinför för att få program vara och licens nycklar för program varu beställningar med beständig och Server prenumeration. Det kommer att återställas till sitt tidigare tillstånd innan det tas bort den 19 januari 2021. (Se [meddelandet](2020-september.md#17).)

Observera att program licens nycklar och nedladdnings länkar är värdefulla och har sökts efter efter immateriella till gångar. Om de läcker ut kan de snabbt bli uttömda sina aktiverings gränser och orsaka en negativ kund-och partner upplevelse.

### <a name="next-steps"></a>Nästa steg

Läs följande resurser för användnings instruktioner och viktig vägledning om program varu nyckel distribution:

- [Sälja lokal program vara via CSP-programmet](../csp-on-premise-software.md)
- [Partner Center New Commerce Operations Guide](https://partner.microsoft.com/resources/detail/partner-center-new-commerce-operations-guide-pdf) (se avsnittet **vägledning om distribution av program varu nycklar** ).

### <a name="questions"></a>Har du några frågor?

Om du har ytterligare frågor om det här meddelandet kan du kontrol lera dina relevanta Yammer-communities.

________________
## <a name="migrate-your-deals-from-partner-sales-connect-psc-to-partner-center"></a><a name="3"></a>Migrera dina avtal från partner Sales Connect (PSC) till Partner Center

### <a name="categories"></a>Kategorier

- Datum: 2021-03-04
- Funktioner

### <a name="summary"></a>Sammanfattning

Partner Sales Connect (PSC) flyttas till skrivskyddad åtkomst från den 31 mars 2021, så vi uppmanar dig att börja migrera dina avtal från PSC till Partner Center.

### <a name="impacted-audience"></a>Förverkad mål grupp

Partner med avtal i PSC

### <a name="details"></a>Information

Som en del av vårt gemensamma åtagande att växa, är **samförsäljning med Microsoft** att du kan **identifiera, leverera dina kunskaper och utöka dina kunders** behov av positiva kund resultat. Med ett genomsnittligt avtal som är **3,5 gånger snabbare** än vanligt, kan du med hantera din samkunds upplevelse i Partner Center sälja över den direkta kunden, partnern och Microsofts försäljnings kanaler och hantera hela din Hänvisnings pipeline på en plats.

**PSC** kommer att flyttas till **skrivskyddad åtkomst** från den **31 mars 2021**, så vi uppmanar dig att påbörja din flytt till Partner Center och få till gång till dessa förbättringar: 

- **Mer exakt routning** av de avtal som du delar med Microsoft till den högra säljaren, baserat på vilken typ av hjälp du behöver.
- Krav **verifiering för direkt** behandling för incitaments berättigade lösningar och för att uppfylla kraven på ISV Connect-program, vilket fören klar godkännande processen och det slutliga Poe-attesteringen (proof of Execution).
- **Smidig användar upplevelse** för att hantera alla dina samförsäljnings möjligheter och Sälj kvalificerade leads på ett och samma ställe.

Vi har också nyligen lagt till nya funktioner i Partner Center som hjälper dig att flytta:

- [Mass åtgärder för samförsäljnings möjligheter](../bulk-operations.md)
- [Funktionen](../psc-to-pc.md) för att migrera en funktion (se avsnittet **PSC-migrering** .)

Med hjälp av co-Sales-upplevelsen i Partner Center får Sälj teamen mer tid på att fokusera på Nurturing-leads och affärs möjligheter, avsluta avtal och skapa långsiktiga kund relationer.

### <a name="next-steps"></a>Nästa steg

Använd [över gångs guiden](../psc-to-pc.md) för partner Center för att gå igenom stegen för att migrera dina avtal från PSC till Partner Center.

### <a name="questions"></a>Har du några frågor?

Kontakta [supporten](https://partner.microsoft.com/support/?stage=1)om du vill ha fler frågor.

________________
## <a name="new-microsoft-dynamics-365-products-and-offers-available-on-april-1-2021"></a><a name="2"></a>Nya Microsoft Dynamics 365-produkter och erbjudanden som är tillgängliga den 1 april 2021

### <a name="categories"></a>Kategorier

- Datum: 2021-03-04
- Funktioner

### <a name="summary"></a>Sammanfattning

Den 1 april 2021 kommer Microsoft att lansera flera nya produkter och erbjudanden för Cloud Solution Provider (CSP)-programmet.

### <a name="impacted-audience"></a>Förverkad mål grupp

Alla partner som går via program varan för Cloud Solution Provider (CSP)

### <a name="details"></a>Information

Den 1 april 2021 kommer Microsoft att lansera följande nya produkter och erbjudanden:

- Power BI Premium per användare
- Kund röst och marknadsföring dem Geo-och segment expansion

**Power BI Premium per användare**

Microsoft kommer att introducera de första Power BI Premium erbjudandena per användare. Power BI Premium säljs för närvarande endast i en kapacitets konstruktion. Power BI Premium per användare ger till gång till Enterprise-Business Intelligence (BI) och analys funktioner. Den flexibla enskilda klient licensieringen tillgodoser små och medel stora företag.

Läs mer om det här erbjudandet i [Power BI versions informationen](/power-platform-release-plan/2020wave2/power-bi/planned-features) .


**Erbjudande information**

Observera att namnet på erbjudandet skiljer sig något från för hands versionen av pris listan.

| Erbjudandets namn | Erbjudande-ID |
| ------ |----------- |
| Power BI Premium per användare | 9c810018-9356-4903-95ab-eeb956289290 | 
| Power BI Premium per användare för lärare | 3affc44f-f372-4ad5-8657-aadd9574fce0 | 
| Power BI Premium per användare för studenter | 657eea87-d0b0-4c89-8c8e-9b04395bd940 | 
| Power BI Premium per användare (prissättning i ideell personal) | 7a0a856c-059f-45dd-9d26-ae27992e706a | 
| Power BI Premium per användare Add-On | 244ff87e-5925-44a0-bf31-cea189719b58 | 
| Power BI Premium per användare Add-On för lärare | 5da849bd-b8f7-4340-b4f4-3a9eaeb8987e | 
| Power BI Premium per användare Add-On för studenter | cf62d70d-5af5-422a-bda8-97936402ac8e | 
| Power BI Premium per användare Add-On (prissättning i ideell personal) | 31c03289-47ab-4ab0-8df1-03742c127ac6 | 

**Kund röst och marknadsföring dem Geo-och segment expansion**

Som en uppföljning till lanseringen av december 2020 har Dynamics 365 Customer Voice och Marketing dem-erbjudanden ändrats för att lägga till nya länder och fler ideella och utbildnings-SKU: er.

| Erbjudandets namn | Erbjudande-ID |
| ------ |----------- |
| Dynamics 365 Customer Voice-dem (pris för ideell personal) | 7a8642a5-481e-4906-a642-b56dbeeb62a0 |
| Dynamics 365 Customer Voice-dem för lärare | 85162d70-9676-4cf6-a4bc-a0d6672f2657 |

Besök följande sidor för att få mer information om dessa erbjudanden:

- [Dynamics 365-röstens start sida för kund service](https://dynamics.microsoft.com/customer-voice/overview/)
- [Start sida för Dynamics 365-marknadsföring](https://dynamics.microsoft.com/customer-voice/overview/)

### <a name="next-steps"></a>Nästa steg

Granska resurserna i det här avsnittet och dela den här informationen med lämpliga intressenter i din organisation.  

### <a name="questions"></a>Har du några frågor?

Om du har frågor om dessa erbjudanden kan du kontrol lera dina relevanta Yammer-communities. 

________________
## <a name="microsoft-universal-print-now-available-in-some-suites"></a><a name="1"></a> Microsoft Universal Print finns nu i vissa paket

### <a name="categories"></a>Kategorier

- Datum: 2021-03-33
- Funktioner

### <a name="summary"></a>Sammanfattning

Microsoft Universal Print är tillgängligt för Transact i SELECT Microsoft 365 Suites och som ett fristående tillägg från den 1 mars 2021.

### <a name="impacted-audience"></a>Förverkad mål grupp

Alla partner som går via program varan för Cloud Solution Provider (CSP)

### <a name="details"></a>Information

[Universal Print](https://aka.ms/universalprint) är en Microsoft 365 utskrifts tjänst som tar bort behovet av lokala utskrifts servrar och gör det möjligt för Windows-enheter att skriva ut till Azure-registrerade skrivare. Den kommer att vara tillgänglig för Transact från den 1 mars 2021.

Arbets tagarna har nytta av driv rutins utskrift, strömlinjeformad plats-baserad skrivar identifiering och en intuitiv utskrifts upplevelse utan inlärnings kurva. Enheter som är anslutna till Azure Active Directory (Azure AD) använder befintliga Azure AD-autentiseringsuppgifter för att skriva ut på ett säkert sätt. Administratörer hanterar utskriften med hjälp av Azure Portal och kan enkelt ansluta skrivare med inbyggt stöd för universell utskrift. Universell utskrift kan distribueras med icke-kompatibla skrivare med hjälp av Universal Print Connector-programvara.

Universal Print kommer att fyllas i vid lanseringen till Windows E3, A3, E5 och A5 och Microsoft 365 BP, F3, E3, A3, E5 och A5.  

**Erbjudande information**

Observera att namnet på erbjudandet skiljer sig något från för hands versionen av pris listan.

| Erbjudandets namn | Erbjudande-ID | Material-ID |
| ------ |----------- |----------- |  
| Tillägg för universell utskrifts volym (500 jobb) – Microsoft 365  | cb131356-45ee-4ae2-8537-873b706c8e75     | 9BI-00004   |
| Tillägg för universell utskrifts volym (500 jobb) för lärare – Microsoft 365   | 477bee81-9872-43d6-91d3-c72390bfcf49   | 9BK-00004   |
| Tillägg för universell utskrifts volym (500 jobb) – Windows    | d3ddc493-5741-4e0d-a02d-07edbb0bb72e   | 9BI-00002   |
| Tillägg för universell utskrifts volym (500 jobb) för lärare – Windows   |  d0862f05-80f5-4fd4-8432-fe72dd893cc7  | 9BK-00002   |

### <a name="next-steps"></a>Nästa steg

Bekanta dig med pris listan och [Översikt över universell utskrift](/universal-print/fundamentals/universal-print-whatis). Dela den här informationen med alla lämpliga kontakter i din organisation.

### <a name="questions"></a>Har du några frågor?

Om du har frågor om dessa erbjudanden kan du kontrol lera dina relevanta Yammer-communities.
