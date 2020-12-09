---
title: Meddelanden december 2020
description: Meddelanden i december 2020 för Microsoft Partner Center, inklusive nya funktioner, kampanjer, erbjudanden, marknader eller ändringar av befintliga erbjudanden.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: brentserbus
ms.author: brserbus
ms.custom: announcement
ms.localizationpriority: high
ms.date: 12/02/2020
ms.openlocfilehash: 1341e60fd9914f421fd59335a8f037f3d915b72f
ms.sourcegitcommit: bc44a6e0c5ef048cda6e882fdb543c13c5b64912
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 12/08/2020
ms.locfileid: "96869307"
---
# <a name="december-2020-announcements"></a>Meddelanden december 2020

Den här sidan innehåller information om Microsoft Partner Center-meddelanden för november 2020.

2020-meddelanden: [april](2020-april.md)  |  [maj](2020-may.md)den  |  [juni](2020-june.md)  |  [juli](2020-july.md)  |  [August](2020-august.md)  |  [September](2020-september.md)  |  [October](2020-October.md)  |  [November](2020-november.md) | Utgången

______________

## <a name="sdk-release-on-net-standard-v1163"></a><a name="4"></a>SDK-version på .NET standard (v 1.16.3)

### <a name="categories"></a>Kategorier

- Datum: 2020-12-8
- Funktioner

### <a name="impacted-audience"></a>Förverkad mål grupp

Direkta fakturerings partner och indirekta leverantörer som deltar i CSP-programmet som använder Partner Center .NET SDK.

### <a name="details"></a>Information

Från och med december 08 2020 kan partners börja hämta versionen av [MicrosoftPartnerCenter. NETSDK (NuGet Galleri | Microsoft. Store. PartnerCenter 1.16.3)](https://www.nuget.org/packages/Microsoft.Store.PartnerCenter/1.16.3)tillsammans med uppdaterade offentliga partners Center SDK [GitHub-exempel](https://github.com/Microsoft/Partner-Center-DotNet-Samples). Den här versionen innehåller uppdateringar av följande:
 
**SelfServePolicies – nya funktioner har lagts till**

- [GetSelfServePolicies](/partner-center/develop/get-a-self-serve-policy-by-id.md)
- [GetListOfSelfServicePolicies](/partner-center/develop/get-a-list-of-self-serve-policies.md)
- [CreateSelfServePolicies](/partner-center/develop/create-a-self-serve-policy.md)
- [UpdateSelfServePolicies](/partner-center/develop/update-a-self-serve-policy.md)
- [DeleteSelfServePolicies](/partner-center/develop/delete-a-self-serve-policy.md)
 
**Kund företags profil**

- Lade till [OrganizationRegistrationNumber](/partner-center/develop/create-a-customer.md)
 
**CustomerBillingProfile.DefaultAddress**

- Lade till MiddleName
 
### <a name="next-steps"></a>Nästa steg

- Ladda ned den senaste versionen [MicrosoftPartnerCenter. NETSDK (NuGet Gallery | Microsoft. Store. PartnerCenter 1.16.3)](https://www.nuget.org/packages/Microsoft.Store.PartnerCenter/1.16.3)
- Hämta och granska [GitHub-exemplen](https://github.com/Microsoft/Partner-Center-DotNet-Samples)

______________

## <a name="december-2020-license-based-price-list-release-notes"></a><a name="3"></a>Versions information om licensbaserade pris listor i december 2020

### <a name="categories"></a>Kategorier

- Datum: 2020-12-8
- Erbjudanden/marknader

### <a name="summary"></a>Sammanfattning 

Licens-och erbjudande listan i december 2020 har några problem.

### <a name="impacted-audience"></a>Förverkad mål grupp 

Alla partner som går via program varan för Cloud Solution Provider (CSP)

### <a name="details"></a>Information

De licensbaserade licens listorna och erbjudande listan i december innehåller några avvikelser. De här problemen är relaterade till licensbaserade licensfiler och bör korrigeras i januari 2021-uppdateringarna.

#### <a name="incorrect-offers-in-the-license-based-price-list"></a>Felaktiga erbjudanden i den licensierade pris listan

De licensbaserade pris listorna för december innehåller följande erbjudanden som inte ska ingå i pris listorna. Dessa erbjudanden har tidigare inkluderats i pris listorna och bör inte ha publicerats. Det finns inget schema när det kan vara tillgängligt. Om de läggs till i framtiden visas de som tillägg i kommande pris listor för för hands versioner.

   |**Erbjudandets namn**|**Erbjudande-ID**|
   |-------------------|:------|
   |Dynamics 365-personalavdelningen (priser för icke-täckning)|1596fa61-7da1-4263-98f8-b27dfa4cfbb5|
   |Dynamics 365-personal som är anslutna till att kvalificera Dynamics 365-bas erbjudandet (priser för icke-täckning)|8bf0b826-e05b-45aa-9cd1-9a9f742f7731|
   |Dynamics 365-personal som är anslutna till att kvalificera Dynamics 365-bas erbjudandet (priser för icke-täckning) (kvalificerat erbjudande)|f906435d-9dc9-42ba-bea6-2a2b08ca60db|
   |Dynamics 365-sand Box (priser för icke-täckning)|079ec5ba-d726-4384-95af-62d135c210d2|
   |Dynamics 365 självbetjäning för Human Resources (priser för icke-täckning)|931acecc-34c3-4f83-913e-c7fdbfd7e2a1|
   |Dynamics 365-åtgärder – order rader (priser för icke-täckning)|7dd6b78a-3d53-47f8-8a64-bd84609a9a70|
   
#### <a name="incorrect-offers-in-the-offer-list-matrix"></a>Felaktiga erbjudanden i listan över erbjudande listor
   
Under erbjudanden finns i matrisen med listan över erbjudanden som fel. De är inte tillgängliga, det finns inget mål datum ännu för tillgänglighet. Partner bör ignorera dessa.

   |**Erbjudandets namn**|**Erbjudande-ID**|
   |-------------------|:------|
   |Dynamics 365-åtgärder – databas kapacitet (priser för icke-täckning)|1d3f4d81-89b9-419e-a880-31b2c50b8d66|
   |Dynamics 365-åtgärder – fil kapacitet (priser för icke-täckning)|dc173a86-285b-444c-881e-3ece531f67da|

#### <a name="powerapps-offer"></a>PowerApps-erbjudande

Det här erbjudandet ingår i listan över erbjudande listor, men inte i pris listan för december. Erbjudandet är tillgängligt och priser finns i den föregående Månadens pris lista november-fil. Det här erbjudandet ska läggas till i pris listan i januari.

   |**Erbjudandets namn**|**Erbjudande-ID**|
   |-------------------|:------|
   |Power Apps per app-plan|5e1087b6-246b-4503-b88a-b60bdf0b3840|

### <a name="next-steps"></a>Nästa steg

Kontrol lera versions anteckningar ofta när andra problem är påslagna kommer de att läggas till i det här meddelandet.

### <a name="last-updated"></a>Senast uppdaterad

8 december 2020

______________

## <a name="an-update-of-the-us-microsoft-365-business-voice-with-calling-plan-offer-is-coming-soon"></a><a name="2"></a>En uppdatering av US Microsoft 365 Business röst med erbjudandet om samtals plan kommer snart

### <a name="categories"></a>Kategorier

- Datum: 2020-12-3
- Erbjudanden/marknader

### <a name="summary"></a>Sammanfattning 

Den 1 januari 2021 kommer Microsoft att börja överföra våra partner och kunder till en ny Microsoft 365 Business röst med erbjudandet om samtals plan. Ingen partner åtgärd krävs.

### <a name="impacted-audience"></a>Förverkad mål grupp 

Alla partner som går via program varan för Cloud Solution Provider (CSP)

### <a name="details"></a>Information

Microsoft kommer att ersätta den befintliga affärs rösten med erbjudandet om samtals plan i USA med ett nytt erbjudande för att stödja interna krav för Telco-produkter. Det nya erbjudandet kommer att ha samma funktions uppsättning och priser. Erbjudande ändringarna är interna för Microsoft och bör inte påverka sättet som CSP-partner marknad, säljer eller stöder affärs rösten med erbjudandet om samtals plan. Ändringen gäller bara för det här erbjudandet.

För ny försäljning använder du det nya erbjudandet från den 1 januari 2021. Det gamla erbjudandet kommer att ersättas med det nya erbjudandet för pris listan.

Befintliga kunder överförs automatiskt till det nya erbjudandet vid förnyelse datumet. Ingen åtgärd krävs från partner och kunder som förnyas.


* * Ny erbjudande information
 
   |**Erbjudandets namn**|**Erbjudande-ID**|**Material-ID**|
   |-------------------|:------|:------|
   |Microsoft 365 Business röst (US)|86713ec1-ad33-42cf-a1ce-8397d4d875fe|PZW-00023|
   
* * Gammal erbjudande information

   |**Erbjudandets namn**|**Erbjudande-ID**|**Material-ID**|
   |-------------------|:------|:------|
   |Microsoft 365 Business röst (US)|9f9f2c7b-c961-402b-9421-8e3c9207eeb3|PZW-00009|

### <a name="next-steps"></a>Nästa steg

Bekanta dig med pris listan och dela den här informationen med alla lämpliga kontakter i din organisation.

______________

## <a name="now-live-partner-center-api-updates-and-user-interface-enhancements-for-the-education-customer-validation-process"></a><a name="1"></a>Nu är Live: API-uppdateringar för partner Center och användar gränssnitts förbättringar för kund validerings processen för utbildning

### <a name="categories"></a>Kategorier

- Datum: 2020-12-3
- Funktioner

### <a name="impacted-audience"></a>Förverkad mål grupp 

Partner som säljer akademiska erbjudanden via Cloud Solution Provider-programmet

### <a name="summary"></a>Sammanfattning 

Microsoft körs med förtroende. Vi strävar efter att tillhandahålla en kompatibel, säker och säker metod för kund validering för att kunna agera akademiska erbjudanden i Cloud Solution Provider-programmet. Som en del av detta åtagande introducerar vi API: er för API: er och användar gränssnitts förbättringar som ger klarhet och insyn i kundens först konsumentsajter-process samt möjligheten att mata in mer exakta data som kommer att ge bättre kund först konsumentsajter. 

**Förbättringar i Partner Center** 

- Nya API: er för att hämta och publicera kompetenser som stöd för korrekt data inmatning och förbättra kund validerings processen för utbildning av Microsoft. 

- Förbättringar av användar gränssnittet för att stödja korrekt data inmatning och förbättra kund validerings processen för utbildning av Microsoft. 

**Utfasning av befintliga API: er för att hämta och skicka kvalificering** 

De befintliga API: erna GET och tag kommer att tas ur bruk **före slutet av februari 2021**. Vid detta tillfälle måste du ha övergått till de nya API: erna GET och POST Partner Center för att kunna köpa utbildnings erbjudanden.  

**Test** 

För att få en bättre förståelse för de API: er och data som krävs för lyckad kund validering kan partners testa dessa förbättringar. Partner som vill delta i testningen bör hämta [partner Center-utbildningen för kund testning](https://partner.microsoft.com/resources/detail/partner-center-edu-testing-guide-pdf) för instruktioner om hur du förbereder, registrerar dig och för information om vad som ska förväntas under test fasen.

**Biblioteks-och Museum-kunder** 

Förutom de ovanstående förbättringarna är vi glada att kunna meddela att vi kommer att möjliggöra pris värda erbjudanden för biblioteks-och Museum-kunder, vilket utökar de utbildnings kunder som du kan använda för att få till exempel på Transact CSP-erbjudanden. 

Microsoft förbehåller sig rätten att granska statusen för alla kunder eller föreslagna kunder som en kvalificerad utbildnings användare. Mer information finns i de [akademiska användar kraven för utbildning](https://www.microsoftvolumelicensing.com/DocumentSearch.aspx?Mode=3&DocumentTypeId=7) . 

### <a name="next-stepsadditional-resources"></a>Nästa steg/ytterligare resurser

- Granska det nya användar gränssnittet för partner Center, API-ändringar och vägledning i åtgärds beredskaps resurserna:  [partner Center utbildning av kund validerings](https://partner.microsoft.com/resources/collection/partner-center-edu-validation-enhancements#/) process 

- Se till att din organisation är bekant med de [akademiska användar kraven för utbildning](https://www.microsoftvolumelicensing.com/DocumentSearch.aspx?Mode=3&DocumentTypeId=7). 

- Dela den här informationen med lämpliga team i din organisation och med dina åter försäljare för att hjälpa dem att förbereda för dessa ändringar. 

### <a name="change-log"></a>Ändrings logg 

_ Den 31 augusti 2020: ursprunglig publikation 

- 25 september 2020: uppdatering av test fönster har lagts till 

- 4 oktober 2020: påminnelse om att registrera sig för testning 

- 10 november 2020: påminnelse om att registrera sig för testning 

- 3 december 2020: API-uppdateringar Live 
