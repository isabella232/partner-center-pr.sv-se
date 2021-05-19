---
title: Vanliga frågor och svar om säkerhetskrav för partner
ms.topic: article
ms.date: 05/26/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Vanliga frågor och svar om partnersäkerhetskraven – vad de är, hur partner bör implementera dem och hur du vet om du har uppfyllt dem.
author: isaiahwilliams
ms.author: iswillia
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 174c56ce9bb5fb3d9d92c1ef18af73479619f4bb
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 05/19/2021
ms.locfileid: "110145889"
---
# <a name="common-questions-about-partner-security-requirements"></a>Vanliga frågor om partnersäkerhetskrav

**Lämpliga roller:** Alla Partner Center-användare

I den här artikeln får du svar på några vanliga [frågor om partnersäkerhetskraven.](partner-security-requirements.md)

### <a name="what-are-the-partner-security-requirements-and-why-should-partners-implement-them"></a>Vilka är partnersäkerhetskraven och varför ska partner implementera dem?

Större och kontinuerliga skyddsmekanismer för säkerhet och sekretess är bland våra högsta prioriteter och vi fortsätter att hjälpa partner att skydda sina kunder och klienter. Vi fortsätter att se ett mer avancerat och ökande antal säkerhetsattacker, främst relaterade till identitetskomprometteringsincidenter. Eftersom förebyggande kontroller spelar en viktig roll i en övergripande försvarsstrategi för att förhindra säkerhetsattacker införde vi obligatoriska säkerhetskrav under 2019. [](partner-security-requirements.md) Alla partner som deltar i Molnlösningsleverantör(CSP)-programmet, Kontrollpanelen-leverantörer och rådgivare måste implementera kraven för att vara kompatibla.

### <a name="what-are-the-key-timelines-and-milestones"></a>Vilka är de viktigaste tidslinjerna och milstolparna?

De villkor som är associerade med dessa säkerhetskrav, inklusive tidslinjer och milstolpar, ingår i [Microsoft-partneravtal](microsoft-partner-agreement.md). Du måste implementera dessa säkerhetskrav så snart som möjligt för att efterleva ditt deltagande i CSP-programmet.

### <a name="what-will-happen-if-i-dont-implement-these-partner-security-requirements"></a>Vad händer om jag inte implementerar dessa partnersäkerhetskrav?

Den Microsoft-partneravtal kräver att du tillämpar multifaktorautentisering för användarkonton och inför den säkra programmodellen för att interagera med Partner Center-API:et. 

Partner som inte följer dessa säkerhetsmetoder kan förlora sin möjlighet att göra transaktioner i CSP-programmet eller hantera kundklienter med hjälp av delegerade administratörsrättigheter.

### <a name="do-the-security-requirements-apply-to-all-geographies"></a>Gäller säkerhetskraven för alla geografiska områden?

Ja, säkerhetskraven gäller för alla geografiska områden. Vi rekommenderar starkt att alla partner som agerar via ett suveränt moln (amerikanska myndigheter och Tyskland) agerar och inför dessa nya säkerhetskrav omedelbart. Dessa partner är dock för närvarande inte nödvändiga för att uppfylla säkerhetskraven. Microsoft kommer att tillhandahålla ytterligare information om tillämpningen av dessa säkerhetskrav för nationella moln i framtiden.

### <a name="is-it-possible-to-get-an-exclusion-for-an-account"></a>Går det att få ett undantag för ett konto?

Nej, det går inte att undanta användarkonton från kravet på att multifaktorautentisering (MFA) ska tillämpas. Eftersom det är mycket privilegierat att vara en partner kräver Microsoft-partneravtal att multifaktorautentisering tillämpas för varje användarkonto i din partnerklientorganisation.

### <a name="how-do-i-know-if-i-have-met-the-partner-security-requirements"></a>Hur gör jag för att om jag uppfyller partnersäkerhetskraven?

Slutför följande steg:

- Du måste uppfylla alla krav som beskrivs i [partnersäkerhetskraven.](partner-security-requirements.md)
- Du måste se till att alla användarkonton i din partnerklientorganisation har multifaktorautentisering framtvingad.

För att identifiera viktiga områden där du kan vidta åtgärder tillhandahåller vi statusrapporten för säkerhetskrav [som](https://partner.microsoft.com/commerce/security/compliance) är tillgänglig via Partnercenter.

Mer information om statusrapporten finns i [status för partnersäkerhetskrav.](partner-security-compliance.md)

## <a name="required-actions"></a>Nödvändiga åtgärder

### <a name="what-are-the-key-actions-i-need-to-take-to-meet-the-requirements"></a>Vilka är de viktigaste åtgärderna jag behöver vidta för att uppfylla kraven?

Alla partner i CSP-programmet (direktfakturering, indirekt leverantör och indirekt återförsäljare), rådgivare Kontrollpanelen leverantörer måste uppfylla kraven.

1. **Framtvinga MFA för alla användare**

    Alla partner i CSP-programmet, Advisors och Kontrollpanelen Vendors måste framtvinga MFA för alla användare i sin partnerklientorganisation.

    Fler saker att ha i åtanke:

    - Indirekta leverantörer måste samarbeta med indirekta återförsäljare för att kunna registrera sig på Partner Center om de inte redan har gjort det och uppmuntra sina återförsäljare att uppfylla kraven.
    - Azure MFA görs tillgängligt för alla användare i partnerklientorganisationen utan kostnad via Standardinställningar för Azure AD-säkerhet med den enda verifieringsmetoden för ett autentiseringsprogram som stöder tidsbaserade engångslösenord (TOTP).
    - Ytterligare verifieringsmetoder är tillgängliga via [Azure Active Directory Premium](/azure/active-directory/fundamentals/active-directory-get-started-premium) SKU:er, om andra metoder, till exempel ett telefonsamtal eller SMS, krävs.
    - Partner kan också använda en MFA-lösning från tredje part för varje konto vid åtkomst till Microsofts kommersiella molntjänster.

2. **Anta Modell för säkra program ramverket**

    Alla partner som har utvecklat anpassad integrering med hjälp av API:er (till exempel Azure Resource Manager, Microsoft Graph, Partner Center API osv.) eller implementerat anpassad automatisering med hjälp av verktyg som PowerShell måste implementera [Modell för säkra program-ramverket](/partner-center/develop/enable-secure-app-model) för integrering med Microsofts molntjänster. Om du inte gör det kan det leda till avbrott på grund av MFA-distributionen. Följande resurser ger en översikt och vägledning om hur du inför modellen.

    - [Modell för säkra program översikt](/partner-center/develop/enable-secure-app-model)
    - [Partnercenter: Modell för säkra program guide](https://assetsprod.microsoft.com/secure-application-model-guide.pdf)
    - [Partner i CSP-program: .NET-exempelkod för att Modell för säkra program](/samples/microsoft/partner-center-dotnet-samples/secure-app-model/)
    - [Partner i CSP-program: Java-exempelkod för att aktivera Modell för säkra program](/samples/microsoft/partner-center-java-samples/secure-app-model/)
    - [Partnercenter – autentiseringsdokument](/partner-center/develop/partner-center-authentication)
    - [Dokument om Partnercenter PowerShell Multi-Factor Authentication (MFA)](/powershell/partnercenter/multi-factor-auth)

    Kontakta leverantören om du använder en kontrollpanel för att införa Modell för säkra program ramverket.

    Kontrollpanelens leverantörer måste registrera [till](enroll-as-cpv.md) Partner Center som kontrollpanelsleverantör och börja implementera det här kravet omedelbart. Se [Partnercenter: Modell för säkra program ramverket](https://assetsprod.microsoft.com/secure-application-model-guide.pdf). Kontrollpanelens leverantörer måste godkänna och hantera CSP-partners medgivande i stället för autentiseringsuppgifter och rensa alla befintliga CSP-partners autentiseringsuppgifter.

## <a name="multi-factor-authentication"></a>Multifaktorautentisering

### <a name="what-is-multi-factor-authentication-mfa"></a>Vad är multifaktorautentisering (MFA)?

MFA är en säkerhetsmekanism för att autentisera individer via mer än en nödvändig säkerhets- och valideringsprocedur. Det fungerar genom att kräva två eller flera av följande autentiseringsmetoder:

- Något du känner till (vanligtvis ett lösenord)
- Något du har (en betrodd enhet som inte är enkel att duplicera, t.ex. en telefon)
- Något du är (biometrik)

### <a name="what-is-the-cost-of-enabling-mfa"></a>Vad är kostnaden för att aktivera MFA?

Microsoft tillhandahåller MFA utan kostnad via implementeringen av Standardinställningar för Azure AD-säkerhet. Det enda verifieringsalternativ som är tillgängligt med den här versionen av MFA är ett autentiseringsprogram. Om ett telefonsamtal eller SMS krävs måste en [Azure Active Directory Premium](/azure/active-directory/fundamentals/active-directory-get-started-premium) licens köpas. Du kan också använda en lösning från tredje part för att tillhandahålla MFA för varje användare i din partnerklientorganisation – i det här fallet är det ditt ansvar att se till att din MFA-lösning tillämpas och att du är kompatibel.

### <a name="what-actions-do-i-need-to-take-if-i-already-have-an-mfa-solution"></a>Vilka åtgärder måste jag vidta om jag redan har en MFA-lösning?

Genom dessa säkerhetskrav måste användare i en partnerklientorganisation autentiseras med hjälp av MFA vid åtkomst till Microsofts kommersiella molntjänster. Tredjepartslösningar kan användas för att uppfylla dessa krav. Microsoft tillhandahåller inte längre valideringstestning till oberoende identitetsproviders för kompatibilitet med Azure Active Directory. Om du vill testa din produkt för samverkan kan du följa dessa [riktlinjer.](https://www.microsoft.com/download/details.aspx?id=56843)

> [!IMPORTANT]
> När du använder en lösning från tredje part är det viktigt att kontrollera att lösningen som utfärdar autentiseringsmetodreferensanspråk (AMR) som innehåller MFA-värdet. Se [Testa partnersäkerhetskraven för](/powershell/partnercenter/test-partner-security-requirements) mer information om hur du verifierar din lösning från tredje part som utfärdar det förväntade anspråket.

### <a name="i-use-multiple-partner-tenants-to-transact-do-i-need-to-implement-mfa-on-them-all"></a>Jag använder flera partnerklienter för transaktioner. Måste jag implementera MFA på alla?

Ja, du måste framtvinga MFA för varje Azure Active Directory som är associerad med CSP-programmet eller Advisor-programmet. Om du vill Azure Active Directory Premium en licens måste du köpa en Azure Active Directory-licens för användarna i varje Azure Active Directory klientorganisation. 

### <a name="does-each-user-account-in-my-partner-tenant-need-to-have-mfa-enforced"></a>Måste varje användarkonto i min partnerklientorganisation ha MFA framtvingat?

Ja, varje användare måste ha MFA framtvingat. Men om du använder standardvärden för Azure AD-säkerhet krävs ingen ytterligare åtgärd eftersom den funktionen tillämpar MFA för alla användarkonton. Att aktivera standardinställningar för säkerhet är ett kostnadsfritt och enkelt sätt att se till att dina användarkonton är MFA-kompatibla och inte påverkas när MFA tillämpas.

### <a name="i-am-a-direct-bill-partner-with-microsoft-what-do-i-need-to-do"></a>Jag är direktfaktureringspartner hos Microsoft. Vad behöver jag göra?

Direktfakturering Molnlösningsleverantör partner måste tillämpa MFA för varje användare i sin partnerklientorganisation.

### <a name="i-am-an-indirect-reseller-and-only-transact-though-a-distributor-do-i-still-have-to-do-enable-mfa"></a>Jag är en indirekt återförsäljare och gör bara en transact-åtgärd via en distributör. Måste jag fortfarande aktivera MFA?

Alla indirekta återförsäljare måste framtvinga MFA för varje användare i partnerklientorganisationen. Den indirekta återförsäljaren måste aktivera MFA.

### <a name="i-dont-use-the-partner-center-api-do-i-still-need-to-implement-mfa"></a>Jag använder inte Partner Center-API:et. Behöver jag fortfarande implementera MFA?

Ja, det här säkerhetskravet gäller för alla användare, inklusive partneradministratörsanvändare och slutanvändare i en partnerklientorganisation.

### <a name="which-third-party-vendors-provide-mfa-solutions-compatible-with-azure-active-directory"></a>Vilka tredjepartsleverantörer tillhandahåller MFA-lösningar som är kompatibla med Azure Active Directory?

När du granskar MFA-leverantörer och -lösningar måste partner se till att den lösning de väljer är kompatibel med Azure Active Directory.

Microsoft tillhandahåller inte längre valideringstestning till oberoende identitetsproviders för kompatibilitet med Azure Active Directory. Om du vill testa din produkt för samverkan kan du följa dessa [riktlinjer.](https://www.microsoft.com/download/details.aspx?id=56843)

Mer information finns i [kompatibilitetslistan för Azure AD-federation.](/azure/active-directory/hybrid/how-to-connect-fed-compatibility)

### <a name="how-can-i-test-mfa-in-our-integration-sandbox"></a>Hur testar jag MFA i vår sandbox-miljö för integrering?

Standardfunktionen för Azure AD-säkerhet ska vara aktiverad eller så kan du använda en lösning från tredje part som använder federation.

### <a name="will-enabling-mfa-affect-how-i-interact-with-my-customers-tenant"></a>Påverkar aktiveringen av MFA hur jag interagerar med min kunds klientorganisation?

Nej. Hur dessa säkerhetskrav uppfylls påverkar inte hur du hanterar dina kunder. Din möjlighet att utföra delegerade administrativa åtgärder avbryts inte.

### <a name="are-my-customers-subject-to-the-partner-security-requirements"></a>Omfattas mina kunder av partnersäkerhetskraven?

Nej, det krävs inte att du tillämpar MFA för varje användare i kundens Azure AD-klienter. Vi rekommenderar dock att du samarbetar med varje kund för att avgöra hur användarna ska skyddas på bästa sätt.

### <a name="can-any-user-be-excluded-from-the-mfa-requirement"></a>Kan någon användare undantas från MFA-kravet?

Nej, varje användare, inklusive tjänstkonton, i din partnerklientorganisation måste autentiseras med hjälp av MFA.

### <a name="do-the-partner-security-requirements-apply-to-the-integration-sandbox"></a>Gäller partnersäkerhetskraven för sandbox-miljön för integrering?

Ja, partnersäkerhetskraven gäller för sandbox-miljön för integrering. Det innebär att du måste implementera lämplig MFA-lösning för användare i sandbox-klientorganisationen för integrering. Vi rekommenderar att du implementerar Standardinställningar för Azure AD-säkerhet för att tillhandahålla MFA.

### <a name="how-do-i-configure-an-emergency-access-break-glass-account"></a>Hur gör jag för att konfigurera ett nödkonto för åtkomst (nödfall)?

Det anses vara bästa praxis att skapa ett eller två konton för åtkomst vid akutfall för att förhindra att du oavsiktligt blir utelåst från Din Azure AD-klientorganisation. När det gäller partnersäkerhetskraven måste varje användare autentiseras med hjälp av MFA. Det här kravet innebär att du måste ändra definitionen av ett konto för åtkomst vid akutfall. Det kan vara ett konto som använder en tredjepartslösning för MFA.

### <a name="is-active-directory-federation-service-adfs-required-if-i-am-using-a-third-party-solution"></a>Krävs Active Directory Federationstjänst (ADFS) om jag använder en lösning från tredje part?

Nej, du behöver inte ha Active Directory Federationstjänst (ADFS) om du använder en lösning från tredje part. Vi rekommenderar att du arbetar med leverantören av lösningen för att avgöra vilka kraven för deras lösning är.

### <a name="is-it-a-requirement-to-enable-azure-ad-security-defaults"></a>Är det ett krav att aktivera Standardinställningar för Azure AD-säkerhet?

Nej, du måste inte aktivera standardinställningarna för Azure AD-säkerhet.

### <a name="can-conditional-access-be-used-to-meet-the-mfa-requirement"></a>Kan villkorlig åtkomst användas för att uppfylla MFA-kravet?

Ja, du kan använda villkorlig åtkomst för att tillämpa MFA för varje användare, inklusive tjänstkonton, i din partnerklientorganisation. Men eftersom det är mycket privilegierat att vara en partner måste vi se till att varje användare har en MFA-utmaning för varje enskild autentisering. Det innebär att du inte kan använda funktionen för villkorsstyrd åtkomst som kringgår kravet på MFA.

### <a name="will-the-service-account-used-by-azure-ad-connect-be-impacted-by-the-partner-security-requirements"></a>Kommer tjänstkontot som används Azure AD Connect påverkas av partnersäkerhetskraven?

Nej, tjänstkontot som används av Azure AD Connect påverkas inte av partnersäkerhetskraven. Om du får problem med Azure AD Connect på grund av tvingande MFA öppnar du en teknisk supportbegäran hos Microsoft-supporten.

## <a name="secure-application-model"></a>Modell för säkra program

### <a name="who-should-adopt-the-secure-application-model-to-meet-the-requirements"></a>Vem bör införa den säkra programmodellen för att uppfylla kraven?

Microsoft introducerar ett säkert, skalbart ramverk för Molnlösningsleverantör-partner (CSP) och Kontrollpanelen Vendors (CPV) som använder Multi-Factor Authentication. Mer information finns i [Modell för säkra program guiden](https://assetsprod.microsoft.com/secure-application-model-guide.pdf). Alla partner som har utvecklat anpassad integrering med hjälp av API:er (till exempel Azure Resource Manager, Microsoft Graph, Partner Center API osv.) eller implementerat anpassad automatisering med hjälp av verktyg som PowerShell måste implementera [Modell för säkra program-ramverket](/partner-center/develop/enable-secure-app-model) för integrering med Microsofts molntjänster.

### <a name="what-is-the-secure-application-model"></a>Vad är Modell för säkra program?

Microsoft introducerar ett säkert, skalbart ramverk för autentisering av Molnlösningsleverantör-partner (CSP) och Kontrollpanelen-leverantörer (CPV) som använder Multi-Factor Authentication. Mer [information Modell för säkra program guiden](https://assetsprod.microsoft.com/secure-application-model-guide.pdf) finns i guiden.  

### <a name="how-do-i-implement-the-secure-application-model"></a>Hur gör jag för att implementerar du Modell för säkra program?

Alla partner som har utvecklat anpassad integrering med hjälp av api:er (till exempel Azure Resource Manager, Microsoft Graph, Partner Center API osv.) eller [](/partner-center/develop/enable-secure-app-model) implementerat anpassad automatisering med hjälp av verktyg som PowerShell, måste implementera Modell för säkra program-ramverket för att integrera med Microsofts molntjänster. Om du inte gör det kan det leda till avbrott på grund av MFA-distributionen. Följande resurser ger en översikt och vägledning om hur du inför modellen.

- [Modell för säkra program översikt](/partner-center/develop/enable-secure-app-model)
- [Partnercenter: Modell för säkra program guide](https://assetsprod.microsoft.com/secure-application-model-guide.pdf)
- [Partner i CSP-program: .NET-exempelkod för att Modell för säkra program](/samples/microsoft/partner-center-dotnet-samples/secure-app-model/)
- [Partner i CSP-program: Java-exempelkod för att aktivera Modell för säkra program](/samples/microsoft/partner-center-java-samples/secure-app-model/)
- [Partnercenter – autentiseringsdokument](/partner-center/develop/partner-center-authentication)
- [Dokument om PartnerCenter PowerShell Multi-Factor Authentication (MFA)](/powershell/partnercenter/multi-factor-auth)

Om du använder en kontrollpanel måste du kontakta leverantören angående implementeringen av Modell för säkra program ramverket.

Kontrollpanelens leverantörer måste [](enroll-as-cpv.md) publicera till Partnercenter som kontrollpanelsleverantör och börja implementera det här kravet omedelbart. Se [Partnercenter: Modell för säkra program ramverket](https://assetsprod.microsoft.com/secure-application-model-guide.pdf). Kontrollpanelens leverantörer måste godkänna och hantera CSP-partners medgivande i stället för autentiseringsuppgifter och rensa alla befintliga CSP-partners autentiseringsuppgifter.

### <a name="does-the-secure-application-model-need-to-be-implemented-for-the-partner-center-apisdk-only"></a>Måste Modell för säkra program implementeras endast för Partner Center API/SDK?

Genom att framtvinga multifaktorautentisering för alla användarkonton påverkas all automatisering eller integrering som är avsedd att köras icke-interaktivt. Partnersäkerhetskraven kräver att du aktiverar den säkra programmodellen för Partner Center-API:et, men det kan användas för att hantera behovet av en andra faktor för autentisering med automatisering och integrering.

>[!Note] 
>Resurser som används måste ha stöd för åtkomsttokenbaserad autentisering.

### <a name="i-am-using-automation-tools-such-as-powershell-how-do-i-implement-the-secure-application-model"></a>Jag använder automatiseringsverktyg som PowerShell. Hur gör jag för att implementerar du Modell för säkra program?

Du måste implementera Modell för säkra program om automatiseringen är avsedd att köras icke-interaktivt och förlitar sig på användarautentiseringsuppgifter för autentisering. Se [Modell för säkra program | Partner Center PowerShell för](/powershell/partnercenter/multi-factor-auth) vägledning om hur du implementerar det här ramverket.  

>[!Note] 
>Alla automatiseringsverktyg ger inte möjlighet att autentisera med hjälp av åtkomsttoken. Publicera ett meddelande i [gruppen Säkerhetsvägledning i Partnercenter](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance) om du behöver hjälp med att förstå vilka ändringar som behöver göras. 

### <a name="what-user-credentials-should-the-application-administrator-provide-when-performing-the-consent-process"></a>Vilka användarautentiseringsuppgifter ska programadministratören ange när medgivandeprocessen utfördes?

Vi rekommenderar att du använder ett tjänstkonto som har tilldelats minst privilegierade behörigheter. När det gäller Partnercenter-API:et bör du använda ett konto som antingen har tilldelats rollen Försäljningsagent eller Administratörsagenter.

### <a name="why-should-the-application-administrator-not-provide-global-admin-user-credentials-when-performing-the-consent-process"></a>Varför ska programadministratören inte ange autentiseringsuppgifter för global administratör när medgivandeprocessen utfördes?

Det är bästa praxis att använda lägsta möjliga identitet.  Detta minskar risken. Vi rekommenderar inte att du använder ett konto som har globala administratörsbehörigheter eftersom det ger fler behörigheter än vad som krävs.

### <a name="i-am-a-csp-partner-how-do-i-know-if-my-control-panel-vendor-cpv-is-working-on-implementing-the-solution-or-not"></a>Jag är CSP-partner. Hur gör jag för att om min Kontrollpanelen leverantör (CPV) arbetar med att implementera lösningen eller inte?

För partner som använder en Kontrollpanelen Vendor-lösning (CPV) för att göra en transact i Molnlösningsleverantör-programmet (CSP) är det ditt ansvar att rådgöra med din CPV.

### <a name="who-is-a-control-panel-vendor-cpv"></a>Vem är Kontrollpanelen leverantör (CPV)?

En Kontrollpanelen leverantör är en oberoende programvaruleverantör som utvecklar appar för användning av CSP-partner för att integrera med Partner Center-API:er. En Kontrollpanelen leverantör är inte en CSP-partner med direkt åtkomst till Partner Center-instrumentpanelen eller API:er. En detaljerad beskrivning finns i guiden [PartnerCenter: Secure Applications Model](https://assetsprod.microsoft.com/secure-application-model-guide.pdf).

### <a name="i-am-a-cpv-how-do-i-enroll"></a>Jag är en CPV. Hur gör jag för att registrera?

Om du vill registrera dig som en kontrollpanelsleverantör (CPV) följer du riktlinjerna [här](enroll-as-cpv.md).

CPV:er måste kontaktas för att få registreringslänken och tillhandahålla en Microsoft-medarbetares sponsring som har en affärsrelation med [CPVHelp@microsoft.com](mailto:CPVHelp@microsoft.com) CPV:n eller känner till deras verksamhet. Till exempel en Partner Development Manager (PDM).

När du har registrerat dig i Partnercenter och registrerat dina program har du åtkomst till Partner Center-API:er. Du får din sandbox-information via ett Partnercenter-meddelande om du är en ny CPV. När du har slutfört registreringen som microsoft-CPV och godkänt CPV-avtalet kan du:

1. Hantera program för flera innehavare (lägg till program Azure Portal program och registrera och avregistrera program i Partnercenter).

   >[!Note]
   >CPV:er måste registrera sina program i Partnercenter för att auktoriseras för Partner Center-API:er. Att lägga till program i Azure Portal auktoriserar inte CPV-program för Partner Center-API:er.

1. Visa och hantera din CPV-profil.

1. Visa och hantera användare som behöver åtkomst till CPV-funktioner. En CPV kan bara ha rollen Global administratör.

### <a name="i-am-using-the-partner-center-sdk-will-sdk-automatically-adopt-the-secure-application-model"></a>Jag använder Partnercenter-SDK. Kommer SDK automatiskt att införa Modell för säkra program?

Nej, du måste följa riktlinjerna i guiden för Modell för säkra program [.](https://assetsprod.microsoft.com/secure-application-model-guide.pdf)

### <a name="can-i-generate-a-refresh-token-for-the-secure-application-model-with-accounts-that-dont-have-mfa-enabled"></a>Kan jag generera en uppdateringstoken för den säkra programmodellen med konton som inte har MFA aktiverat?

Ja, en uppdateringstoken kan genereras med ett konto som inte har MFA framtvingat. Detta bör dock undvikas. Alla token som genereras med ett konto som inte har MFA aktiverat kan inte komma åt resurser på grund av kravet på MFA.

### <a name="how-should-my-application-obtain-an-access-token-if-we-enable-mfa"></a>Hur ska mitt program hämta en åtkomsttoken om vi aktiverar MFA?

Du måste följa den Modell för säkra program [som](https://assetsprod.microsoft.com/secure-application-model-guide.pdf) innehåller information om hur du gör detta samtidigt som du uppfyller de nya säkerhetskraven. Du hittar .NET-exempelkod [här och](http://github.com/microsoft/Partner-Center-DotNet-Samples/tree/master/secure-app-model) Java-exempelkod [här.](http://github.com/microsoft/Partner-Center-Java-Samples/tree/master/secure-app-model)

### <a name="as-a-cpv-do-i-create-an-azure-ad-application-in-our-cpv-tenant-or-the-tenant-of-the-csp-partner"></a>Skapar jag som CPV ett Azure AD-program i vår CPV-klient eller klientorganisationen för CSP-partnern?

CPV:en måste skapa programmet Azure Active Directory klientorganisationen som är associerad med registreringen som en CPV.

### <a name="i-am-a-csp-that-is-using-app-only-authentication-do-i-need-to-make-any-changes"></a>Jag är en CSP som endast använder appautentisering. Behöver jag göra några ändringar?

Appautentisering påverkas inte eftersom användarautentiseringsuppgifter inte används för att begära en åtkomsttoken. Om användarautentiseringsuppgifter delas måste kontrollpanelens leverantörer (CPV: er) använda Modell för säkra program [ramverket](https://assetsprod.microsoft.com/secure-application-model-guide.pdf) och rensa eventuella befintliga partnerautentiseringsuppgifter.

### <a name="as-a-cpv-can-i-leverage-the-app-only-authentication-style-to-get-access-tokens"></a>Kan jag som CPV använda appens enda autentiseringsstil för att hämta åtkomsttoken?

Nej, Kontrollpanelen leverantörspartner kan inte använda appens enda autentiseringsstil för att begära åtkomsttoken för partnerns räkning. De bör implementera den säkra programmodellen, som använder autentiseringsstilen app + användare.

## <a name="technical-enforcement"></a>Teknisk tillämpning

### <a name="what-is-the-activation-of-security-safeguards"></a>Vad är aktiveringen av säkerhetsskyddsmekanismer?

Alla partner som deltar i Molnlösningsleverantör(CSP)-programmet, Kontrollpanelen-leverantörer (CPV:er) och rådgivare bör implementera de obligatoriska säkerhetskraven för att vara kompatibla.

För att ge ytterligare skydd började Microsoft aktiveringen av säkerhetsskydd som hjälper partner att skydda sina klienter och sina kunder genom att använda multifaktorautentisering (MFA) för att förhindra obehörig åtkomst.  

Aktiveringen för AOBO-funktioner (admin-on-behalf-of) har slutförts för alla partnerklienter. För att ytterligare hjälpa till att skydda partner och kunder, som riktar in sig på kvartal 2 CY2020, påbörjar vi aktiveringen av Partner Center-transaktioner i CSP, vilket hjälper partner att skydda sina företag och kunder mot identitetsstöldrelaterade incidenter.

Mer information finns på [sidan om multifaktorautentisering (MFA) för din partnerklientorganisation.](partner-security-requirements-mandating-mfa.md)

### <a name="i-am-using-a-third-party-mfa-solution-and-i-am-being-blocked-what-should-i-do"></a>Jag använder en MFA-lösning från tredje part och blockeras. Vad ska jag göra?

För att verifiera att kontot som har åtkomst till resurser har [](https://tools.ietf.org/html/rfc8176) utmanats för multifaktorautentisering kontrollerar vi autentiseringsmetodens referensanspråk för att se om MFA visas. Vissa lösningar från tredje part utfärdar inte det här anspråket eller inkluderar inte MFA-värdet. Om anspråket saknas, eller om MFA-värdet inte visas, går det inte att avgöra om det autentiserade kontot har utmanats för multifaktorautentisering. Du måste samarbeta med leverantören för din lösning från tredje part för att avgöra vilka åtgärder som behöver vidtas så att lösningen utfärdar autentiseringsmetodens referensanspråk.

Se [Testa partnersäkerhetskraven](/powershell/partnercenter/test-partner-security-requirements) om du är osäker på om din lösning från tredje part utfärdar det förväntade anspråket eller inte.

### <a name="mfa-is-blocking-me-from-supporting-my-customer-using-aobo-what-should-i-do"></a>MFA hindrar mig från att stödja min kund med hjälp av AOBO, vad ska jag göra?

Det tekniska framtvingandet för partnersäkerhetskraven kontrolleras om det autentiserade kontot har utmanats för multifaktorautentisering. Om kontot inte har gjort det omdirigeras du till inloggningssidan och uppmanas att autentisera dig igen. Läs mer om upplevelsen och vägledningen [i den här MFA-dokumentationen (Multi-Factor Authentication)](partner-security-requirements-mandating-mfa.md#partner-delegated-administration) för din partnerklientorganisation. I scenariot där din domän inte är federerad uppmanas du att konfigurera multifaktorautentisering när autentiseringen är klar. När det är klart kan du hantera dina kunder med hjälp av AOBO. I scenariot där din domän är federerad måste du se till att kontot måste använda multifaktorautentisering.

## <a name="security-defaults-transition"></a>Övergång till standardvärden för säkerhet

### <a name="how-can-i-transition-from-baseline-policies-to-security-defaults-or-other-mfa-solutions"></a>Hur övergår jag från baslinjeprinciper till standardinställningar för säkerhet eller andra MFA-lösningar?

Azure Active Directory (Azure AD) ["baslinjeprinciper"](/azure/active-directory/fundamentals/whats-new#replacement-of-baseline-policies-with-security-defaults) tas bort och ersätts med "standardinställningar för säkerhet", en mer omfattande uppsättning skyddsprinciper för dig och dina kunder. [Standardvärden för säkerhet](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) kan hjälpa till att skydda din organisation från identitetsstöldsrelaterade säkerhetsattacker.

Implementeringen av multifaktorautentisering (MFA) tas bort på grund av att baslinjeprinciperna tas ur spel om du inte har övergåt från baslinjeprinciper till säkerhetstandardprincipen eller andra implementeringsalternativ för [MFA.](partner-security-requirements.md#implementing-multi-factor-authentication) Alla användare i dina partnerklienter som utför MFA-skyddade åtgärder uppmanas att slutföra MFA-verifieringen. Granska mer detaljerad vägledning [här.](partner-security-requirements-mandating-mfa.md)
Vidta någon av följande åtgärder för att hålla dig kompatibel och minimera störningar:

- Övergång till standardinställningar för säkerhet
    - Standardprinciper för säkerhet är ett av de alternativ som partner kan välja att implementera MFA. Den erbjuder en grundläggande säkerhetsnivå som är aktiverad utan extra kostnad.
    - Lär dig hur du aktiverar MFA för din organisation med Azure AD och granskar viktiga överväganden [för säkerhetsstandarder.](partner-security-requirements.md#security-defaults)
    - Aktivera standardprinciper för säkerhet om den uppfyller dina affärsbehov.
- Övergång till villkorlig åtkomst
    - Om standardprincipen för säkerhet inte tillgodoser dina behov aktiverar du villkorlig åtkomst. Mer information finns i dokumentationen om villkorsstyrd åtkomst i Azure AD.

## <a name="key-resources"></a>Viktiga resurser

### <a name="how-to-get-started"></a>Så här kommer du igång

- [Säkerhetskrav för partner: stegvis guide.](partner-security-requirements.md)
- Skicka dina frågor och feedback till den här [säkerhetsvägledningsgruppen i Partnercenter.](https://aka.ms/MPCSecurityGuidance)
- Delta i kommande kontorstider för partner och webbseminor. Kontrollera det [detaljerade schemat och resurserna här.](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance)

### <a name="resources-for-adopting-secure-application-model"></a>Resurser för att införa en säker programmodell

- [Modell för säkra program översikt](/partner-center/develop/enable-secure-app-model)
- [Partnercenter: Modell för säkra program guide](https://assetsprod.microsoft.com/secure-application-model-guide.pdf)
- [Partner i CSP-program: .NET-exempelkod för att Modell för säkra program](/samples/microsoft/partner-center-dotnet-samples/secure-app-model/)
- [Partner i CSP-program: Java-exempelkod för att aktivera Modell för säkra program](/samples/microsoft/partner-center-java-samples/secure-app-model/)
- [Partnercenter – autentiseringsdokument](/partner-center/develop/partner-center-authentication)
- [Dokument om PartnerCenter PowerShell Multi-Factor Authentication (MFA)](/powershell/partnercenter/multi-factor-auth)

## <a name="support"></a>Support

### <a name="where-can-i-get-support"></a>Var kan jag få support?

Om du har avancerad support för partner (ASfP) för supportresurser som uppfyller säkerhetskraven kontaktar du din tjänstkontohanterare. för Premier Support för partneravtal (PSfP) kontaktar du din tjänstkontohanterare och teknisk kontohanterare.

### <a name="how-do-i-get-technical-information-and-support-to-help-me-adopt-secure-application-model-framework"></a>Hur gör jag för att få teknisk information och support för att hjälpa mig att införa ett säkert ramverk för programmodeller?

Alternativ för teknisk produktsupport för Azure Active Directory är tillgängliga via dina MPN-förmåner. Partner med åtkomst till en aktiv ASfP- eller PSfP-prenumeration kan arbeta med sin associerade kontohanterare (SAM/TAM) för att bättre förstå vilka alternativ som är tillgängliga för dem.

### <a name="how-do-i-contact-support-if-ive-lost-access-to-partner-center"></a>Hur gör jag för att kontakta supporten om jag har förlorat åtkomsten till Partnercenter?

Om du förlorar åtkomsten på grund av ett MFA-problem kontaktar du den globala administratören för din klientorganisation. Din interna IT-avdelning kan berätta vem din globala administratör är. 

Om du har glömt lösenordet läser du [Det går inte att logga in](unable-to-sign-in.md) för att få hjälp.

### <a name="where-can-i-find-more-information-about-common-technical-issues"></a>Var hittar jag mer information om vanliga tekniska problem?

Information om vanliga tekniska problem finns i Partnersäkerhetskrav [för partner som använder Api:er för Partner Center eller Partner Center](partner-security-requirements.md)