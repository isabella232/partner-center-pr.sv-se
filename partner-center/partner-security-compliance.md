---
title: Status för partner säkerhets krav
ms.date: 05/26/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Lär dig mer om de nya kraven för att öka säkerheten för rådgivare, på kontroll panelen och partner i programmet för moln lösnings leverantörer.
author: isaiahwilliams
ms.author: iswillia
ms.localizationpriority: high
ms.topic: conceptual
ms.custom: SEOMAY.20
ms.openlocfilehash: 1b6c2d56a0747ddf2bd1a821886e371ed698a4a1
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/22/2020
ms.locfileid: "92531592"
---
# <a name="partner-security-requirements-status---get-answers-and-check-reports-about-current-status"></a>Status för partner säkerhets krav – Hämta svar och kontrol lera rapporter om aktuell status

**Gäller för**

- Alla partner i Cloud Solution Provider-programmet
  - Direkt fakturering
  - Indirekt Provider
  - Indirekt åter försäljare
- Alla leverantörer på kontroll panelen
- Alla rådgivare

**Lämpliga användare**
- Alla aktiverade användare, inklusive gäst användare

Större Sekretess skydd och säkerhet är bland våra främsta prioriteringar. Vi vet att det bästa skyddet är förebyggande och att vi bara är lika starka som vår svagaste länk. Därför behöver vi alla i vårt eko system för att agera och se till att de har lämpliga säkerhets skydd på plats. För att hjälpa till att skydda partner och kunder presenterar vi en uppsättning obligatoriska säkerhets krav för rådgivare, kontroll panels leverantörer och partner som ingår i Cloud Solution Provider-programmet.

Från och med 1 augusti 2019 krävs alla partner för att genomdriva Multi-Factor Authentication för alla användare, inklusive tjänst konton, i sin partner klient. Mer detaljerad information om de nya säkerhets principerna finns i [säkerhets kraven för partner](partner-security-requirements.md).

Vi vill se till att varje användare har en MFA-utmaning för varje enskild autentisering. Den här upplevelsen kan åstadkommas på något av följande sätt:

- Implementera Azure AD Premium för att säkerställa att MFA upprätthålls för varje användare
- Implementera [standardinställningar för Azure AD-säkerhet](/azure/active-directory/conditional-access/concept-conditional-access-security-defaults)
- Implementera en lösning från tredje part för att se till att MFA upprätthålls för varje användare

## <a name="partner-security-requirements-status"></a>Status för partner säkerhets krav

Den här rapporten kan hjälpa dig att kontrol lera säkerhets kravets status genom att tillhandahålla ett sätt att se var du kan vara kort. Spårningen uppdateras regelbundet.

>[!NOTE]
>Status rapporten för partner säkerhets krav stöds bara i Partner Center. Den är inte tillgänglig i Microsoft Cloud för amerikanska myndigheter eller Microsoft Cloud Tyskland. Vi rekommenderar starkt att alla partner som agerar genom ett suveränt moln (21Vianet, amerikanska myndigheter och Tyskland) inför dessa nya säkerhets krav direkt. Dessa partners behöver dock inte uppfylla de nya säkerhets kraven från den 1 augusti 2019. Microsoft tillhandahåller ytterligare information om verk ställandet av dessa säkerhets krav för suveräna moln i framtiden.

## <a name="multi-factor-authentication-mfa-report"></a>Multi-Factor Authentication-rapport ("MFA")

Rapporten Partner Center MFA ger insikter om MFA-implementering av partner genom att tillhandahålla två typer av mått baserat på MFA-konfiguration och partner Center-aktiviteter för CSP-klienten: 

### <a name="mfa-configuration-on-a-csp-tenant"></a>MFA-konfiguration på en CSP-klient

Detta mått är relaterat till MFA-konfigurationen på en CSP-klient som har registrerats och rapporter ATS per dag. Det mäter procent andelen aktiverade användar konton med MFA som tvingas med något av dessa [MFA-alternativ](/azure/active-directory/fundamentals/concept-fundamentals-mfa-get-started). Exempel:

- Contoso är en CSP-partner med 110 användar konton i klienten, 10 av dessa användar konton är inaktiverade. 
- Från resten av 100-användar kontona tillämpas MFA med de tillhandahållna [MFA-alternativen](/azure/active-directory/fundamentals/concept-fundamentals-mfa-get-started)i 90. Måttet visar därför 90%. 

### <a name="partner-center-activities-with-mfa"></a>Partner Center-aktiviteter med MFA

Varje gång dina anställda loggar in på Partner Center för att arbeta eller, via API: er, hämta eller skicka data via partner Center, har deras säkerhets status och spårats. De ingår också i säkerhets status spårning, är dina program och alla program på kontroll panelen. Statusen som visas är under de senaste sju dagarna.

#### <a name="mfa-verification-completed-by-users"></a>MFA-verifiering slutförd av användare

Detta mått är relaterat till aktiviteter i Partner Center-instrumentpanelen. Det mäter procent andelen åtgärder som utförs av användare som har slutfört MFA-verifieringen. Exempel:

- Contoso är en CSP-partner med två administratörs agenter, Jane och John.
- Den första dagen är Jane inloggad på instrument panelen i Partner Center utan MFA-verifiering och gjort tre åtgärder.
- Den andra dagen är John inloggad på instrument panelen i Partner Center utan MFA-verifiering och gjort fem åtgärder.
- Den tredje dagen är Jane inloggad på instrument panelen i Partner Center med MFA-verifiering och gjort två åtgärder.
- Inga åtgärder har gjorts av någon av agenterna under de återstående fyra dagarna.
- Med de 10 åtgärder som gjorts i 7-dagars perioden har två gjorts av användaren med MFA-verifiering. Måttet visar därför 20%.

Använd fil **Portal förfrågningar utan MFA** för att förstå vilken användare som är inloggad på Partner Center-instrumentpanelen utan att ha MFA-verifiering och tid för senaste besök i rapporterings fönstret.

#### <a name="appuser-authentication"></a>App + användarautentisering

Det här måttet är relaterat till användningen av API-begäranden för partner Center som görs med app + User Authentication. Den mäter procent andelen API-begäranden som gjorts med hjälp av en åtkomsttoken med MFA-anspråk. Exempel:

- Fabrikam är en CSP-partner och har ett CSP-program som använder en blandning av autentiseringsmetoder för App + användare och appar.
- Den första dagen gjorde programmet tre API-begäranden som har säkerhetskopierats av en åtkomsttoken som erhållits via app + User Authentication-metoden utan MFA-verifiering.
- Den andra dagen gjorde programmet fem API-begäranden som har säkerhetskopierats av en åtkomsttoken som hämtades med endast app-autentisering.
- På den tredje dagen gjorde programmet två API-begäranden som har säkerhetskopierats av en åtkomsttoken som erhållits med hjälp av MFA-verifieringen app + User.
- Inga åtgärder har gjorts av någon av agenterna under de återstående fyra dagarna.
- De fem API-begärandena den andra dagen, som har säkerhetskopierats av en åtkomsttoken som hämtats via endast app-autentisering, utelämnas från måttet eftersom den inte använder användarautentiseringsuppgifter. Två av de återstående fem åtgärderna har säkerhetskopierats med en åtkomsttoken som erhållits med MFA-verifiering. Måttet visar därför 40%.

Om du vill veta vilka app + User-aktiviteter som resulterar i en icke-100% på det här måttet använder du filer:

- **Översikt över API-begäranden** för att förstå den övergripande MFA-statusen per program.
- **Alla API-begäranden** för att förstå detaljerna i varje API-begäranden som görs av användare av din klient, resultatet är begränsat till maximalt 10 000 senaste begär Anden för bättre nedladdning.

## <a name="what-should-i-do-if-the-metrics-under-mfa-report-arent-100"></a>Vad ska jag göra om måtten i MFA-rapporten inte är 100%

Det är möjligt att måtten under rapporten Partner Center MFA inte kan vara 100% för partner som har implementerat MFA. Här följer några faktorer att ta reda på varför.

> [!NOTE]
> Du måste arbeta med någon från din organisation som är bekant med identitets hantering och MFA-implementering för din partner klient.

### <a name="have-you-implemented-mfa-for-your-partner-tenant"></a>Har du implementerat MFA för din partner klient?

Om inte, måste du implementera MFA för din partner klient organisation först. Mer information om hur du implementerar MFA finns i [säkerhets krav](partner-security-requirements.md)för artikel partner.

### <a name="have-you-only-recently-completed-mfa-implementation"></a>Har du bara genomfört MFA-implementering nyligen?

Måtten beräknas per dag och tar hänsyn till de åtgärder som utförts under de senaste sju dagarna. Om du bara har slutfört MFA-implementeringen för din partner klient får måtten inte vara 100%.

### <a name="have-some-user-accounts-been-excluded-from-mfa-implementation"></a>Har vissa användar konton uteslutits från MFA-implementeringen?

Ta reda på om din aktuella MFA-implementering omfattar alla användar konton eller bara vissa. Vissa MFA-lösningar är principbaserad och stöder användar undantag, medan andra kan kräva att du uttryckligen aktiverar MFA för varje användare. Kontrol lera att du inte har uteslutit någon användare från din aktuella MFA-implementering. Alla användar konton som undantas och loggar in på Partner Center för att utföra en CSP-relaterad aktivitet kan orsaka att måtten inte är 100%.

### <a name="is-mfa-only-required-when-certain-conditions-are-met"></a>Krävs MFA bara när vissa villkor uppfylls?

Ta reda på om den aktuella implementeringen endast tillämpar MFA under vissa villkor. Vissa MFA-lösningar ger flexibilitet att endast genomdriva MFA när vissa villkor är uppfyllda. Till exempel kan användaren komma åt från okänd enhet eller okänd plats. En användare, som är aktive rad för MFA men inte krävs för att slutföra MFA-verifiering vid åtkomst till Partner Center, kan orsaka att måtten inte är 100%.

>[!NOTE]
>För partner som har implementerat MFA med hjälp av Azure AD Security-standardvärden är det viktigt att Observera att Multi-Factor Authentication för icke-administratörskonton kommer att tvingas utifrån risk. Användare tillfrågas endast om MFA under riskfyllda inloggnings försök (till exempel att användaren loggar in från en annan plats). Dessutom har användarna upp till 14 dagar på sig att registrera sig för MFA. Användare som inte har slutfört MFA-registrering kommer inte att begära MFA-verifiering under 14-dagars perioden. Därför förväntas vi att måtten inte får vara 100% för partner som har implementerat MFA med hjälp av standardinställningar för Azure AD-säkerhet.

### <a name="are-you-using-third-party-mfa-solution"></a>Använder du MFA-lösningen från tredje part?

Om du använder MFA-lösningen från tredje part kan du identifiera hur du integrerar den med Azure AD. I allmänhet finns det två metoder, inklusive Federation och anpassade kontroller:

* **Identitets Federation** – när Azure AD tar emot en autentiseringsbegäran omdirigerar Azure AD användaren till den federerade identitets leverantören för autentisering. Vid lyckad autentisering omdirigerar den federerade identitets leverantören användaren tillbaka till Azure AD tillsammans med en SAML-token. För att Azure AD ska kunna identifiera att användaren har slutfört MFA-verifiering vid autentisering till den federerade identitets leverantören, måste SAML-token innehålla *authenticationmethodsreferences* -anspråket (med värdet *multipleauthn* ). Kontrol lera om den federerade identitets leverantören stöder utfärdande av ett sådant anspråk. Om så är fallet kontrollerar du om den federerade identitets leverantören har kon figurer ATS att göra det. Om anspråket saknas vet inte Azure AD (och därför Partner Center) att användaren har slutfört MFA-verifieringen och att det saknas ett anspråk kan orsaka att måttet inte är 100%.

* **Anpassad kontroll** – det går inte att använda anpassad kontroll för Azure AD för att identifiera om en användare har SLUTFÖRt MFA-verifiering via en MFA-lösning från tredje part. Därför kommer alla användare som har slutfört MFA-verifiering via en anpassad kontroll alltid att visas i Azure AD (och i sin tur Partner Center) som att de inte har slutfört MFA-verifiering. Där det är möjligt rekommenderar vi att du växlar till att använda identitets Federation i stället för anpassad kontroll vid integrering med Azure AD.

### <a name="identify-which-users-have-logged-into-partner-center-without-mfa"></a>Identifiera vilka användare som har loggat in på Partner Center utan MFA

Det kan vara bra att identifiera vilka användare som loggar in på Partner Center utan MFA-verifiering och verifiera dem mot din aktuella MFA-implementering. Du kan använda [Azure AD-inloggnings rapporten](/azure/active-directory/reports-monitoring/concept-sign-ins) för att ta reda på om en användare har SLUTFÖRt MFA-verifiering eller inte. Azure AD-inloggnings rapporten är för närvarande bara tillgänglig för partner som prenumererar på Azure AD Premium eller en O365-SKU, som innehåller Azure AD Premium (till exempel EMS).

## <a name="next-steps"></a>Nästa steg

- [Community för säkerhets vägledning för partner Center](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance)
- [Säkerhets krav för partner Center](partner-security-requirements.md)
- [Vanliga frågor och svar om säkerhets krav för partner Center](partner-security-requirements-faq.md)