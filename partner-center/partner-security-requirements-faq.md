---
title: Vanliga frågor och svar om partner säkerhets krav
ms.topic: article
ms.date: 05/26/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Vanliga frågor och svar om partnerns säkerhets krav – vad de är, hur partners implementerar dem och hur du vet om du har uppnått dem.
author: isaiahwilliams
ms.author: iswillia
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: f2bf6823fdd976632fb8ad9c8f11ce99835d76a5
ms.sourcegitcommit: 10765386b2df0d4c2e8da9b302a692f452e1090d
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/31/2021
ms.locfileid: "106087084"
---
# <a name="common-questions-about-partner-security-requirements"></a>Vanliga frågor om säkerhets krav för partner

**Lämpliga roller**

- Alla partner Center-användare

I den här artikeln besvaras några vanliga frågor om [partnerns säkerhets krav](partner-security-requirements.md).

### <a name="what-are-the-partner-security-requirements-and-why-should-partners-implement-them"></a>Vilka är partnerns säkerhets krav och varför ska partner implementera dem?

Större och fort löp ande säkerhets-och integritets skydd är bland våra främsta prioriteringar och vi fortsätter att hjälpa våra partner att skydda sina kunder och klienter. Vi fortsätter att se mer avancerade, ökande antal säkerhets attacker, främst relaterade till incidenter med identitets kompromisser. Som förebyggande kontroller spelar en viktig roll i en övergripande skydds strategi för att avvärjer säkerhets attacker. vi introducerade de [nödvändiga säkerhets kraven](partner-security-requirements.md) i 2019. Alla partner som deltar i CSP-programmet (Cloud Solution Provider), på kontroll panelens leverantörer och rådgivare måste implementera kraven för att vara kompatibla.

### <a name="what-are-the-key-timelines-and-milestones"></a>Vilka är de viktigaste tids linjerna och mil stolparna?

Villkoren som är associerade med dessa säkerhets krav, inklusive tids linjer och mil stolpar, ingår i [Microsoft partner Agreement](microsoft-partner-agreement.md). Du måste implementera dessa säkerhets krav så snart som möjligt för att vara kompatibla med ditt deltagande i CSP-programmet.

### <a name="what-will-happen-if-i-dont-implement-these-partner-security-requirements"></a>Vad händer om jag inte implementerar de här partner säkerhets kraven?

Microsoft partner Agreement kräver att du tillämpar Multi-Factor Authentication för användar konton och använder den säkra program modellen för att interagera med API: et för partner Center. 

Partner som inte följer dessa säkerhets metoder kan förlora sin möjlighet att använda Transact i CSP-programmet eller hantera kund klienter med hjälp av ombuds administratörs rättigheter.

### <a name="do-the-security-requirements-apply-to-all-geographies"></a>Gäller säkerhets kraven för alla geografiska områden?

Ja, säkerhets kraven gäller för alla geografiska områden. Vi rekommenderar starkt att alla partner som agerar genom ett suveränt moln (amerikanska myndigheter och Tyskland) agerar och antar dessa nya säkerhets krav direkt. Dessa partners krävs dock inte för närvarande för att uppfylla säkerhets kraven. Microsoft tillhandahåller ytterligare information om verk ställandet av dessa säkerhets krav för suveräna moln i framtiden.

### <a name="is-it-possible-to-get-an-exclusion-for-an-account"></a>Är det möjligt att få ett undantag för ett konto?

Nej, det går inte att undanta något användar konto från kravet på att använda Multi-Factor Authentication (MFA). Med tanke på den starkt privilegier som är en partner, kräver Microsoft partner avtalet att Multi-Factor Authentication upprätthålls för varje användar konto i din partner klient.

### <a name="how-do-i-know-if-i-have-met-the-partner-security-requirements"></a>Hur gör jag för att veta om jag har uppfyllt kraven för partner säkerhet?

Slutför följande steg:

- Du måste uppfylla alla krav som beskrivs i [partner säkerhets kraven](partner-security-requirements.md).
- Du måste se till att alla användar konton i din partner klient har Multi-Factor Authentication.

För att hjälpa till att identifiera de viktiga områden där du kan vidta åtgärder tillhandahåller vi [status rapporten säkerhets krav](https://partner.microsoft.com/commerce/security/compliance) som är tillgänglig via partner Center.

Mer information om status rapporten finns i status för [partner säkerhets krav](partner-security-compliance.md).

## <a name="required-actions"></a>Nödvändiga åtgärder

### <a name="what-are-the-key-actions-i-need-to-take-to-meet-the-requirements"></a>Vilka är de viktigaste åtgärderna jag behöver utföra för att uppfylla kraven?

Alla partner i CSP-programmet (direkta fakturor, indirekta providers och indirekta åter försäljare), rådgivare och kontroll panels leverantörer måste uppfylla kraven.

1. **Tillämpa MFA för alla användare**

    Alla partner i CSP-programmet, Advisor-och kontroll panelen-leverantörer krävs för att genomdriva MFA för alla användare i sin partner klient.

    Fler saker att ha i åtanke:

    - Indirekta leverantörer behöver arbeta med indirekta åter försäljare för att publicera till Partner Center om de inte redan har gjort det, och uppmuntrar deras åter försäljare att uppfylla kraven.
    - Azure MFA görs tillgängligt för alla användare i partner innehavaren utan kostnad genom Azure AD Security-standardvärden med den enda verifierings metoden för ett Authenticator-program som har stöd för tidsbaserad en tid lösen ord (TOTP mobilapp).
    - Ytterligare verifierings metoder är tillgängliga via [Azure Active Directory Premium](/azure/active-directory/fundamentals/active-directory-get-started-premium) SKU: er, om andra metoder som ett telefonsamtal eller SMS krävs.
    - Partner kan också använda en MFA-lösning från tredje part för varje konto vid åtkomst till Microsofts kommersiella moln tjänster.

2. **Anta ramverket för säker program modell**

    Alla partner som har utvecklat anpassad integrering med hjälp av API: er (till exempel Azure Resource Manager, Microsoft Graph, Partner Center API osv.) eller implementerad anpassad automatisering med verktyg som denna PowerShell måste använda verktyg för [säker program modell](/partner-center/develop/enable-secure-app-model) för att integrera med Microsofts moln tjänster. Om du inte gör det kan det leda till ett avbrott på grund av MFA-distribution. Följande resurser ger en översikt och vägledning om hur du antar modellen.

    - [Översikt över säker program modell](/partner-center/develop/enable-secure-app-model)
    - [Partner Center: guiden för säker program modell](https://assetsprod.microsoft.com/secure-application-model-guide.pdf)
    - [Partner i CSP-program: .NET-exempel kod för att aktivera säker program modell](/samples/microsoft/partner-center-dotnet-samples/secure-app-model/)
    - [Partner i CSP-program: Java-exempel kod för att aktivera säker program modell](/samples/microsoft/partner-center-java-samples/secure-app-model/)
    - [Dokument för partner Center-autentisering](/partner-center/develop/partner-center-authentication)
    - [Partner Center PowerShell Multi-Factor Authentication-dokument (MFA)](/powershell/partnercenter/multi-factor-auth)

    Kontakta leverantören om du använder en kontroll panel för att införa säkra program modell ramverk.

    Kontroll panels leverantörer krävs för att [publicera](enroll-as-cpv.md) till Partner Center som leverantör av kontroll panelen och börja implementera det här kravet direkt. Se [partner Center: säker program modell ramverk](https://assetsprod.microsoft.com/secure-application-model-guide.pdf). Kontroll panels leverantörer måste acceptera och hantera CSP-partners medgivande i stället för autentiseringsuppgifter och rensa alla befintliga CSP-partners autentiseringsuppgifter.

## <a name="multi-factor-authentication"></a>Multifaktorautentisering

### <a name="what-is-multi-factor-authentication-mfa"></a>Vad är Multi-Factor Authentication (MFA)?

MFA är en säkerhetsmekanism för att autentisera individer genom mer än en nödvändig säkerhets-och validerings procedur. Det fungerar genom att kräva två eller fler av följande autentiseringsmetoder:

- Något som du känner till (vanligt vis ett lösen ord)
- Något du har (en betrodd enhet som inte enkelt dupliceras, till exempel en telefon)
- Något som du är (biometrik)

### <a name="what-is-the-cost-of-enabling-mfa"></a>Vad kostar det att aktivera MFA?

Microsoft tillhandahåller MFA utan kostnad genom implementering av säkerhets inställningar i Azure AD. Det enda verifierings alternativ som är tillgängligt med den här versionen av MFA är ett Authenticator-program. Om ett telefonsamtal eller SMS-meddelande krävs måste du köpa en [Azure Active Directory Premium](/azure/active-directory/fundamentals/active-directory-get-started-premium) -licens. Du kan också använda en lösning från tredje part för att tillhandahålla MFA för varje användare i din partner klient – i det här fallet är det ditt ansvar att se till att din MFA-lösning upprätthålls och att du är kompatibel.

### <a name="what-actions-do-i-need-to-take-if-i-already-have-an-mfa-solution"></a>Vilka åtgärder måste jag vidta om jag redan har en MFA-lösning?

Genom de här säkerhets kraven måste användare i en partner klient autentiseras med MFA vid åtkomst till Microsofts kommersiella moln tjänster. Lösningar från tredje part kan användas för att uppfylla dessa krav. Microsoft tillhandahåller inte längre verifierings testning till oberoende identitets leverantörer för kompatibilitet med Azure Active Directory. Om du vill testa din produkt för interoperabilitet, se dessa [rikt linjer](https://www.microsoft.com/download/details.aspx?id=56843).

> [!IMPORTANT]
> När du använder en lösning från tredje part är det viktigt att kontrol lera att lösningen utfärdar AMR-anspråk (Authentication Method Reference) som innehåller MFA-värdet. Se [testa säkerhets kraven för partner](/powershell/partnercenter/test-partner-security-requirements) för information om hur du verifierar att en lösning från tredje part utfärdar det förväntade anspråket.

### <a name="i-use-multiple-partner-tenants-to-transact-do-i-need-to-implement-mfa-on-them-all"></a>Jag använder flera partner klienter i Transact. Måste jag implementera MFA på alla?

Ja, du måste använda MFA för varje Azure Active Directory klient som är associerad med CSP-programmet eller Advisor-programmet. Om du vill köpa en Azure Active Directory Premium licens måste du köpa en Azure Active Directory licens för användarna i varje Azure Active Directory klient organisation. 

### <a name="does-each-user-account-in-my-partner-tenant-need-to-have-mfa-enforced"></a>Behöver varje användar konto i min partner klient ha MFA-tvång?

Ja, varje användare måste ha MFA-tvång. Men om du använder Azure AD-standardvärden krävs ingen ytterligare åtgärd eftersom funktionen tillämpar MFA för alla användar konton. Att aktivera säkerhets inställningar är ett kostnads fritt och enkelt sätt att se till att dina användar konton är MFA-kompatibla och inte påverkas när MFA tillämpas.

### <a name="i-am-a-direct-bill-partner-with-microsoft-what-do-i-need-to-do"></a>Jag är en direkt fakturerings partner med Microsoft. Vad behöver jag göra?

Leverantörer av direkta leverantörer av leverantörs leverantörer måste använda MFA för varje användare i sin partner klient.

### <a name="i-am-an-indirect-reseller-and-only-transact-though-a-distributor-do-i-still-have-to-do-enable-mfa"></a>Jag är en indirekt åter försäljare och endast Transact som en distributör. Behöver jag fortfarande aktivera MFA?

Alla indirekta åter försäljare krävs för att genomdriva MFA för varje användare i partner klient organisationen. Den indirekta åter försäljaren måste aktivera MFA.

### <a name="i-dont-use-the-partner-center-api-do-i-still-need-to-implement-mfa"></a>Jag använder inte API: t för partner Center. Behöver jag fortfarande implementera MFA?

Ja, det här säkerhets kravet gäller alla användare, inklusive användare av partner administratörer och slutanvändare i en partner klient.

### <a name="which-third-party-vendors-provide-mfa-solutions-compatible-with-azure-active-directory"></a>Vilka tredjepartsleverantörer tillhandahåller MFA-lösningar som är kompatibla med Azure Active Directory?

När du ska granska MFA-leverantörer och-lösningar måste partnern se till att den lösning som de väljer är kompatibel med Azure Active Directory.

Microsoft tillhandahåller inte längre verifierings testning till oberoende identitets leverantörer för kompatibilitet med Azure Active Directory. Om du vill testa din produkt för interoperabilitet, se dessa [rikt linjer](https://www.microsoft.com/download/details.aspx?id=56843).

Mer information finns i [listan över kompatibla Azure AD-federationar](/azure/active-directory/hybrid/how-to-connect-fed-compatibility).

### <a name="how-can-i-test-mfa-in-our-integration-sandbox"></a>Hur kan jag testa MFA i vårt integrations läge?

Funktionen standardinställningar för Azure AD-säkerhet ska vara aktive rad eller också kan du använda en lösning från tredje part som använder Federation.

### <a name="will-enabling-mfa-affect-how-i-interact-with-my-customers-tenant"></a>Kommer det att aktivera MFA att påverka hur jag interagerar med kundens klient?

Nej. Att uppfylla dessa säkerhets krav påverkar inte hur du hanterar dina kunder. Din möjlighet att utföra delegerade administrativa åtgärder avbryts inte.

### <a name="are-my-customers-subject-to-the-partner-security-requirements"></a>Omfattas mina kunder av partner säkerhets kraven?

Nej, du behöver inte använda MFA för varje användare i kundens Azure AD-klienter. Vi rekommenderar dock att du arbetar med varje kund för att fastställa hur du bäst skyddar användarna.

### <a name="can-any-user-be-excluded-from-the-mfa-requirement"></a>Kan alla användare uteslutas från MFA-kravet?

Nej, varje användare, inklusive tjänst konton, krävs i din partner klient för att autentisera med MFA.

### <a name="do-the-partner-security-requirements-apply-to-the-integration-sandbox"></a>Gäller partner säkerhets kraven för integration sandbox?

Ja, partnerns säkerhets krav gäller för integration sandbox. Det innebär att du måste implementera en lämplig MFA-lösning för användare i klient organisationen för integration sandbox. Vi rekommenderar att du implementerar standardvärden för Azure AD-säkerhet för att tillhandahålla MFA.

### <a name="how-do-i-configure-an-emergency-access-break-glass-account"></a>Hur gör jag för att konfigurerar du ett konto för nöd åtkomst (Break glas)?

Vi rekommenderar att du skapar ett eller två nödfalls åtkomst konton för att förhindra oavsiktligt utelåst av din Azure AD-klient. Med avseende på partner säkerhets kraven krävs att varje användare autentiseras med MFA. Detta krav innebär att du måste ändra definitionen för ett konto för nöd åtkomst. Det kan vara ett konto som använder en lösning från tredje part för MFA.

### <a name="is-active-directory-federation-service-adfs-required-if-i-am-using-a-third-party-solution"></a>Krävs Active Directory Federationstjänst (ADFS) om jag använder en lösning från tredje part?

Nej, det är inte nödvändigt att ha Active Directory Federationstjänst (ADFS) om du använder en lösning från tredje part. Vi rekommenderar att du arbetar med leverantören av lösningen avgör vilka krav som gäller för lösningen.

### <a name="is-it-a-requirement-to-enable-azure-ad-security-defaults"></a>Är det ett krav att aktivera standardinställningar för Azure AD-säkerhet?

Nej, det krävs inte att du aktiverar standardinställningar för Azure AD-säkerhet.

### <a name="can-conditional-access-be-used-to-meet-the-mfa-requirement"></a>Kan villkorlig åtkomst användas för att uppfylla MFA-kravet?

Ja, du kan använda villkorlig åtkomst för att verkställa MFA för varje användare, inklusive tjänst konton, i din partner klient. Men med tanke på den mycket privilegierade typen av partner behöver vi se till att varje användare har en MFA-utmaning för varje enskild autentisering. Det innebär att du inte kan använda funktionen för villkorlig åtkomst som kringgår kravet för MFA.

### <a name="will-the-service-account-used-by-azure-ad-connect-be-impacted-by-the-partner-security-requirements"></a>Kommer det tjänst konto som används av Azure AD Connect påverkas av partner säkerhets kraven?

Nej, det tjänst konto som används av Azure AD Connect påverkas inte av partnerns säkerhets krav. Om du får problem med Azure AD Connect som resultat av att använda MFA, kan du öppna en teknisk supportbegäran med Microsoft support.

## <a name="secure-application-model"></a>Säker program modell

### <a name="who-should-adopt-the-secure-application-model-to-meet-the-requirements"></a>Vem bör använda den säkra program modellen för att uppfylla kraven?

Microsoft presenterar ett säkert, skalbart ramverk för autentisering av CSP-partner (Cloud Solution Provider) och på kontroll panelens leverantörer (CPV) som använder Multi-Factor Authentication. Mer information finns i den [säkra program modell guiden](https://assetsprod.microsoft.com/secure-application-model-guide.pdf). Alla partner som har utvecklat anpassad integrering med hjälp av API: er (till exempel Azure Resource Manager, Microsoft Graph, Partner Center API osv.) eller implementerad anpassad automatisering med verktyg som denna PowerShell måste använda verktyg för [säker program modell](/partner-center/develop/enable-secure-app-model) för att integrera med Microsofts moln tjänster.

### <a name="what-is-the-secure-application-model"></a>Vad är en säker program modell?

Microsoft presenterar ett säkert, skalbart ramverk för att autentisera leverantörer av moln lösningar (CSP) och kontroll panels leverantörer (CPV) som utnyttjar Multi-Factor Authentication. Mer information finns i [guiden för säker program modell](https://assetsprod.microsoft.com/secure-application-model-guide.pdf) .  

### <a name="how-do-i-implement-the-secure-application-model"></a>Hur gör jag för att implementera den säkra program modellen?

Alla partner som har utvecklat anpassad integrering med hjälp av API: er (till exempel Azure Resource Manager, Microsoft Graph, Partner Center API osv.) eller implementerad anpassad automatisering med verktyg som denna PowerShell måste använda verktyg för [säker program modell](/partner-center/develop/enable-secure-app-model) för att integrera med Microsofts moln tjänster. Om du inte gör det kan det leda till ett avbrott på grund av MFA-distribution. Följande resurser ger en översikt och vägledning om hur du antar modellen.

- [Översikt över säker program modell](/partner-center/develop/enable-secure-app-model)
- [Partner Center: guiden för säker program modell](https://assetsprod.microsoft.com/secure-application-model-guide.pdf)
- [Partner i CSP-program: .NET-exempel kod för att aktivera säker program modell](/samples/microsoft/partner-center-dotnet-samples/secure-app-model/)
- [Partner i CSP-program: Java-exempel kod för att aktivera säker program modell](/samples/microsoft/partner-center-java-samples/secure-app-model/)
- [Dokument för partner Center-autentisering](/partner-center/develop/partner-center-authentication)
- [Partner Center PowerShell Multi-Factor Authentication-dokument (MFA)](/powershell/partnercenter/multi-factor-auth)

Om du använder en kontroll panel måste du kontakta leverantören angående införandet av ramverket för säker program modell.

Kontroll panels leverantörer krävs för att [publicera](enroll-as-cpv.md) till Partner Center som leverantör av kontroll panelen och börja implementera det här kravet direkt. Se [partner Center: säker program modell ramverk](https://assetsprod.microsoft.com/secure-application-model-guide.pdf). Kontroll panels leverantörer måste acceptera och hantera CSP-partners medgivande i stället för autentiseringsuppgifter och rensa alla befintliga CSP-partners autentiseringsuppgifter.

### <a name="does-the-secure-application-model-need-to-be-implemented-for-the-partner-center-apisdk-only"></a>Behöver den säkra program modellen implementeras enbart för partner Center API/SDK?

Genom att tvinga Multi-Factor Authentication för alla användar konton kommer all automatisering eller integrering som är avsedd att köras icke-interaktivt att påverkas. Även om säkerhets kraven för partner kräver att du aktiverar den säkra program modellen för partner Center API, kan den användas för att åtgärda behovet av en andra faktor för autentisering med automatisering och integrering.

>[!Note] 
>Resurser som används måste ha stöd för åtkomst till tokenbaserad autentisering.

### <a name="i-am-using-automation-tools-such-as-powershell-how-do-i-implement-the-secure-application-model"></a>Jag använder Automation-verktyg som PowerShell. Hur gör jag för att implementera den säkra program modellen?

Du måste implementera den säkra program modellen om din automatisering är avsedd att köras icke-interaktivt och förlitar sig på användarautentiseringsuppgifter för autentisering. Se [säker program modell | Partner Center PowerShell](/powershell/partnercenter/multi-factor-auth) för vägledning om hur du implementerar det här ramverket.  

>[!Note] 
>Alla Automation-verktyg ger inte möjlighet att autentisera med hjälp av åtkomsttoken. Publicera ett meddelande i gruppen för [säkerhets vägledning om Partner Center](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance) om du behöver hjälp med att förstå vilka ändringar som behöver göras. 

### <a name="what-user-credentials-should-the-application-administrator-provide-when-performing-the-consent-process"></a>Vilka användarautentiseringsuppgifter ska program administratören tillhandahålla när de genomför medgivande processen?

Vi rekommenderar att du använder ett tjänst konto som har tilldelats minst privilegierade behörigheter. Med avseende på Partner Center API bör du använda ett konto som antingen har tilldelats rollen Sälj agent eller administratörs agent.

### <a name="why-should-the-application-administrator-not-provide-global-admin-user-credentials-when-performing-the-consent-process"></a>Varför bör program administratören inte uppge autentiseringsuppgifter för global administratör när godkännande processen genomförs?

Vi rekommenderar att du använder lägsta privilegierade identiteter.  Detta minskar risken. Vi rekommenderar inte att du använder ett konto som har globala administratörs behörigheter eftersom det skulle ge fler behörigheter än vad som krävs.

### <a name="i-am-a-csp-partner-how-do-i-know-if-my-control-panel-vendor-cpv-is-working-on-implementing-the-solution-or-not"></a>Jag är en CSP-partner. Hur gör jag för att vet du om min kontroll panels leverantör (CPV) arbetar med att implementera lösningen eller inte?

För partner som använder en lösning för kontroll panelens tillverkare (CPV) till Transact i Cloud Solution Provider (CSP)-programmet, är det ditt ansvar att kontakta din CPV.

### <a name="who-is-a-control-panel-vendor-cpv"></a>Vem är en kontroll panels leverantör (CPV)?

En kontroll panel leverantör är en oberoende program varu leverantör som utvecklar appar för användning av CSP-partners för att integrera med API: er för partner Center. En kontroll panel leverantör är ingen CSP-partner med direkt åtkomst till instrument panelen eller API: er för partner Center. En detaljerad beskrivning finns i [guiden Partner Center: säker program modell](https://assetsprod.microsoft.com/secure-application-model-guide.pdf).

### <a name="i-am-a-cpv-how-do-i-enroll"></a>Jag är en CPV. Hur gör jag för att registrera dig?

Följ de rikt linjer som anges [här](enroll-as-cpv.md)om du vill registrera dig som en-leverantör av kontroll panelen (CPV).

CPVs måste kontaktas [CPVHelp@microsoft.com](mailto:CPVHelp@microsoft.com) för att ta emot registrerings länken och tillhandahålla en Microsoft personal sponsor som har en affärs relation med CPV eller känner sig för deras verksamhet. Till exempel en partner Development Manager (PDM).

När du har registrerat dig i Partner Center och registrerat dina program har du till gång till API: er för partner Center. Du får din sandbox-information via ett meddelande om att du är en ny CPV. När du har slutfört registreringen som Microsoft CPV och godkänt CPV-avtalet kan du:

1. Hantera program med flera innehavare (Lägg till program i Azure Portal och registrera och avregistrera program i Partner Center).

   >[!Note]
   >CPVs måste registrera sina program i Partner Center för att få behörighet för API: er för partner Center. Att lägga till program till enbart Azure Portal tillåter inte CPV-program för API: er för partner Center.

1. Visa och hantera din CPV-profil.

1. Visa och hantera dina användare som behöver åtkomst till CPV-funktioner. En CPV kan bara ha rollen global administratör.

### <a name="i-am-using-the-partner-center-sdk-will-sdk-automatically-adopt-the-secure-application-model"></a>Jag använder SDK för partner Center. Kommer SDK automatiskt att införa den säkra program modellen?

Nej, du måste följa rikt linjerna i [guiden för säker program modell](https://assetsprod.microsoft.com/secure-application-model-guide.pdf).

### <a name="can-i-generate-a-refresh-token-for-the-secure-application-model-with-accounts-that-dont-have-mfa-enabled"></a>Kan jag skapa en uppdateringstoken för säker program modell med konton som inte har MFA aktiverat?

Ja, en uppdateringstoken kan genereras med hjälp av ett konto som inte har MFA-tvång. Detta bör dock undvikas. Token som genereras med ett konto som inte har MFA-funktioner kan inte komma åt resurser på grund av kraven för MFA.

### <a name="how-should-my-application-obtain-an-access-token-if-we-enable-mfa"></a>Hur ska mitt program hämta en åtkomsttoken om vi aktiverar MFA?

Du måste följa den [säkra program modell guiden](https://assetsprod.microsoft.com/secure-application-model-guide.pdf) som innehåller information om hur du gör det samtidigt som du följer de nya säkerhets kraven. Du hittar .NET-exempel koden [här](http://github.com/microsoft/Partner-Center-DotNet-Samples/tree/master/secure-app-model) och Java-exempel koden [här](http://github.com/microsoft/Partner-Center-Java-Samples/tree/master/secure-app-model).

### <a name="as-a-cpv-do-i-create-an-azure-ad-application-in-our-cpv-tenant-or-the-tenant-of-the-csp-partner"></a>Som CPV skapar jag ett Azure AD-program i vår CPV-klient eller klient organisation för CSP-partner?

CPV måste skapa Azure Active Directory programmet i den klient som är associerad med registreringen som en CPV.

### <a name="i-am-a-csp-that-is-using-app-only-authentication-do-i-need-to-make-any-changes"></a>Jag är en CSP som endast använder autentisering med appar. Behöver jag göra några ändringar?

Endast appens autentisering påverkas inte eftersom användarautentiseringsuppgifter inte används för att begära en åtkomsttoken. Om autentiseringsuppgifter delas måste CPVs (Control panels Vendors) använda det [säkra program modell ramverket](https://assetsprod.microsoft.com/secure-application-model-guide.pdf) och ta bort eventuella befintliga partner autentiseringsuppgifter.

### <a name="as-a-cpv-can-i-leverage-the-app-only-authentication-style-to-get-access-tokens"></a>Som ett CPV kan jag använda formatet endast appens autentisering för att få åtkomst till tokens?

Nej, på kontroll panelen kan leverantörs partner inte använda formatet endast appens autentisering för att begära åtkomst-token för partnerns räkning. De bör implementera den säkra program modellen, som använder appens och användarens format för autentisering.

## <a name="technical-enforcement"></a>Teknisk tillämpning

### <a name="what-is-the-activation-of-security-safeguards"></a>Vad är aktivering av säkerhets åtgärder?

Alla partner som deltar i CSP-programmet (Cloud Solution Provider), på kontroll panelens leverantörer (CPVs) och rådgivare bör implementera de nödvändiga säkerhets kraven för att vara kompatibla.

Microsoft började med att skydda sina klienter och deras kunder genom att kräva Multi-Factor Authentication (MFA) för att förhindra obehörig åtkomst för att ge ytterligare skydd.  

Aktiveringen av ADMINISTRATE-funktioner (admin on-of-of) har slutförts för alla partner klienter. För att ytterligare hjälpa till att skydda partner och kunder, rikta in på Q2-CY2020, kommer vi att påbörja aktiveringen av Partner Center-transaktioner i CSP, vilket hjälper samarbets partners att skydda sina företag och kunder från problem med identitets stölder.

Mer information finns på [kräva Multi-Factor Authentication (MFA) för partner klient](partner-security-requirements-mandating-mfa.md) sidan.

### <a name="i-am-using-a-third-party-mfa-solution-and-i-am-being-blocked-what-should-i-do"></a>Jag använder en MFA-lösning från tredje part och jag är blockerad, vad ska jag göra?

För att verifiera att kontot som har åtkomst till resurser har anropats för Multi-Factor Authentication kontrollerar vi referens kravet för [autentiseringsmetoden](https://tools.ietf.org/html/rfc8176) för att se om MFA visas. Vissa lösningar från tredje part utfärdar inte detta anspråk eller inkluderar inte MFA-värdet. Om anspråket saknas, eller om MFA-värdet inte finns i listan, finns det inget sätt att avgöra om det autentiserade kontot har anropats för Multi-Factor Authentication. Du måste arbeta med leverantören för din lösning från tredje part för att fastställa vilka åtgärder som måste vidtas, så att lösningen utfärdar referens kravet för autentiseringsmetoden.

Se [testa säkerhets kraven för partner](/powershell/partnercenter/test-partner-security-requirements) om du är osäker på om din lösning från tredje part utfärdar det förväntade anspråket eller inte.

### <a name="mfa-is-blocking-me-from-supporting-my-customer-using-aobo-what-should-i-do"></a>MFA hindrar mig från att stödja min kund med ADMINISTRATE, vad ska jag göra?

Den tekniska tillämpningen av partner säkerhets kraven kontrol leras om det autentiserade kontot har anropats för Multi-Factor Authentication. Om kontot inte har varit omdirigeras du till inloggnings sidan och uppmanas att autentisera igen. Läs ytterligare erfarenhet och vägledning i den här [kräva Multi-Factor Authentication (MFA) för din partner klient](partner-security-requirements-mandating-mfa.md#partner-delegated-administration) dokumentation. I scenariot där domänen inte är federerad uppmanas du att konfigurera Multi-Factor Authentication efter att autentiseringen har autentiserats. När den är klar kan du hantera dina kunder med ADMINISTRATE. I scenariot där din domän är federerad måste du se till att kontot anropas för Multi-Factor Authentication.

## <a name="security-defaults-transition"></a>Säkerhets Standards över gång

### <a name="how-can-i-transition-from-baseline-policies-to-security-defaults-or-other-mfa-solutions"></a>Hur kan jag övergå från bas linje principer till säkerhets standarder eller andra MFA-lösningar?

Azure Active Directory (Azure AD) ["baseline"-principer tas bort och ersätts](/azure/active-directory/fundamentals/whats-new#replacement-of-baseline-policies-with-security-defaults) med "säkerhets standarder", en mer omfattande uppsättning skydds principer för dig och dina kunder. [Standardvärden för säkerhet](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) kan hjälpa till att skydda din organisation mot säkerhets attacker med identitets stöld.

Multi-Factor Authentication (MFA)-implementeringen tas bort på grund av den ursprungliga bas linjen om du inte har gått över från bas linje principerna till säkerhets standard principen eller [andra MFA-implementerings alternativ](partner-security-requirements.md#implementing-multi-factor-authentication). Alla användare i din partner klienter som utför MFA-skyddade åtgärder uppmanas att slutföra MFA-verifieringen. Läs mer detaljerade anvisningar [här](partner-security-requirements-mandating-mfa.md).
Gör något av följande för att vara kompatibel och minimera störningar:

- Över gång till säkerhets inställningar
    - Säkerhets standard princip är ett av de alternativ som partners kan välja för att implementera MFA. Den erbjuder en grundläggande säkerhets nivå som är aktive rad utan extra kostnad.
    - Lär dig hur du aktiverar MFA för din organisation med Azure AD och se [viktiga överväganden för säkerhets inställningar](partner-security-requirements.md#security-defaults).
    - Aktivera säkerhets principer om den uppfyller dina affärs behov.
- Över gång till villkorlig åtkomst
    - Aktivera villkorlig åtkomst om principen för säkerhets inställningar inte uppfyller dina behov. Mer information finns i dokumentationen för villkorlig åtkomst för Azure AD.

## <a name="key-resources"></a>Viktiga resurser

### <a name="how-to-get-started"></a>Så här kommer du igång

- [Säkerhets krav för partner: steg-för-steg-guide](partner-security-requirements.md).
- Dirigera dina frågor och synpunkter till den här [gruppen med säkerhets vägledning för partner Center](https://aka.ms/MPCSecurityGuidance).
- Delta i kommande partner kontors tider och webb seminarier. Kontrol lera det [detaljerade schemat och resurserna här](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance).

### <a name="resources-for-adopting-secure-application-model"></a>Resurser för att införa säker program modell

- [Översikt över säker program modell](/partner-center/develop/enable-secure-app-model)
- [Partner Center: guiden för säker program modell](https://assetsprod.microsoft.com/secure-application-model-guide.pdf)
- [Partner i CSP-program: .NET-exempel kod för att aktivera säker program modell](/samples/microsoft/partner-center-dotnet-samples/secure-app-model/)
- [Partner i CSP-program: Java-exempel kod för att aktivera säker program modell](/samples/microsoft/partner-center-java-samples/secure-app-model/)
- [Dokument för partner Center-autentisering](/partner-center/develop/partner-center-authentication)
- [Partner Center PowerShell Multi-Factor Authentication-dokument (MFA)](/powershell/partnercenter/multi-factor-auth)

## <a name="support"></a>Support

### <a name="where-can-i-get-support"></a>Var kan jag få support?

Om du har ASfP (Advanced support for Partners) kontaktar du tjänst konto hanteraren för support resurser för att uppfylla säkerhets kraven. för Premier Support för partner avtal (PSfP) kontaktar du Service Account Manager och Technical Account Manager.

### <a name="how-do-i-get-technical-information-and-support-to-help-me-adopt-secure-application-model-framework"></a>Hur gör jag för att få teknisk information och support som hjälper mig att införa säkra program modell ramverk?

Support alternativ för teknisk produkt för Azure Active Directory är tillgängliga via dina MPN-förmåner. Partner med åtkomst till en aktiv ASfP-eller PSfP-prenumeration kan arbeta med sin associerade konto hanterare (SAM/TAM) för att bäst förstå de tillgängliga alternativen.

### <a name="how-do-i-contact-support-if-ive-lost-access-to-partner-center"></a>Hur gör jag för att kontakta supporten om jag har förlorat åtkomst till Partner Center?

Om du förlorar åtkomst på grund av ett MFA-problem kontaktar du den globala administratören för din klient organisation. Din interna IT-avdelning kommer att kunna berätta vem din globala administratör är. 

Om du har glömt ditt lösen ord kan du [inte logga in](unable-to-sign-in.md) om du vill ha hjälp.

### <a name="where-can-i-find-more-information-about-common-technical-issues"></a>Var hittar jag mer information om vanliga tekniska problem?

Information om vanliga tekniska problem finns i [partner säkerhets krav för partner med partner Center-eller partner Center-API: er](partner-security-requirements.md)