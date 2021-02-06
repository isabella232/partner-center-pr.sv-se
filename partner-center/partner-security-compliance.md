---
title: Status rapport för säkerhets krav
ms.date: 10/30/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Lär dig att kontrol lera efterlevnaden av säkerhets kraven i rapporten säkerhets krav status och MFA-rapport för partner Center
author: isaiahwilliams
ms.author: iswillia
ms.localizationpriority: high
ms.topic: conceptual
ms.custom: SEOMAY.20
ms.openlocfilehash: 3f521e05fbf0b3a6c209a84ed9ab53d2502960a5
ms.sourcegitcommit: d37a3f353426e52dfbbac577b7576f9c3f6d2ddf
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 02/06/2021
ms.locfileid: "99624161"
---
# <a name="security-requirements-status-report"></a>Status rapport för säkerhets krav

**Lämpliga roller**
- Leverantörer på kontroll panelen
- Globala administratörer

I den här artikeln beskrivs status rapporten säkerhets krav i Partner Center. Den här rapporten ger Mät värden som följer [kraven på partner säkerhet](partner-security-requirements.md) för Multi-Factor Authentication (MFA) för användare i din partner klient.

Om du vill få åtkomst till den här rapporten i [partner Center](https://partner.microsoft.com/dashboard)går du till **Inställningar**  >  **konto inställningar**  >  **säkerhets krav status**. Rapporten uppdateras dagligen och visar inloggnings data från de senaste sju dagarna.

>[!NOTE]
>Status rapporten för säkerhets krav stöds bara i Partner Center. Den är inte tillgänglig i Microsoft Cloud för amerikanska myndigheter eller Microsoft Cloud Tyskland. Vi rekommenderar starkt att alla partner som agerar genom ett suveränt moln (amerikanska myndigheter och Tyskland) inför dessa nya säkerhets krav direkt. Dessa partner krävs dock för närvarande inte för att uppfylla de nya säkerhets kraven. Microsoft tillhandahåller ytterligare information om verk ställandet av dessa säkerhets krav för suveräna moln i framtiden.

## <a name="security-status-metrics"></a>Mått för säkerhets status

Status rapporten säkerhets krav ger insikter om MFA-implementering av partner och tillhandahåller mått på MFA-konfiguration och partners Center aktiviteter på partner klienter. I följande avsnitt beskrivs dessa mått i detalj.

### <a name="mfa-configuration-on-a-partner-tenant"></a>MFA-konfiguration på en partner klient

Mått **procent andelen aktiverade användar konton med MFA som framtvingas med alternativ som anges här:** visar procent andelen aktiverade användar konton på din partner klient som har MFA-tvång. Du kan använda något av dessa [MFA-alternativ](/azure/active-directory/fundamentals/concept-fundamentals-mfa-get-started) för att uppnå efterlevnad. Dessa data samlas in och rapporteras dagligen. Exempel:

- Contoso är en CSP-partner med 110 användar konton i klienten, 10 av dessa användar konton är inaktiverade. 
- Från resten av 100-användar kontona tillämpas MFA med de tillhandahållna [MFA-alternativen](/azure/active-directory/fundamentals/concept-fundamentals-mfa-get-started)i 90. Måttet visar därför 90%. 

### <a name="partner-center-requests-with-mfa"></a>Partner Center-begäranden med MFA

Varje gång dina anställda loggar in på Partner Center för att arbeta eller, via API: er, hämta eller skicka data via partner Center, har deras säkerhets status och spårats. I säkerhets status spårning ingår även program och alla program på kontroll panelen. Dessa data visas i mått under **procent av begär anden till Partner Center med MFA** och de senaste sju dagarna.

#### <a name="dashboard-mfa-verification"></a>Instrument panel MFA-verifiering

Måttet **via partner Center-portalen** är relaterat till aktiviteter i Partner Center-instrumentpanelen. Det mäter procent andelen åtgärder som utförs av användare som har slutfört MFA-verifieringen. Exempel:

- Contoso är en CSP-partner med två administratörs agenter, Jane och John.
- Den första dagen är Jane inloggad på instrument panelen i Partner Center utan MFA-verifiering och gjort tre åtgärder.
- Den andra dagen är John inloggad på instrument panelen i Partner Center utan MFA-verifiering och gjort fem åtgärder.
- Den tredje dagen är Jane inloggad på instrument panelen i Partner Center med MFA-verifiering och gjort två åtgärder.
- Inga åtgärder har gjorts av någon av agenterna under de återstående fyra dagarna.
- Med de 10 åtgärder som gjorts i 7-dagars perioden har två gjorts av användaren med MFA-verifiering. Måttet visar därför 20%.

Använd fil **Portal förfrågningar utan MFA** för att förstå vilken användare som är inloggad på Partner Center-instrumentpanelen utan att ha MFA-verifiering och tid för senaste besök i rapporterings fönstret.

#### <a name="appuser-mfa-verification"></a>App + MFA-verifiering av användare

Måttet **via API eller SDK** är relaterat till app + User Authentication via API-begäranden i Partner Center. Den mäter procent andelen API-begäranden som gjorts med hjälp av en åtkomsttoken med MFA-anspråk. Exempel:

- Fabrikam är en CSP-partner och har ett CSP-program som använder en blandning av autentiseringsmetoder för App + användare och appar.
- Den första dagen gjorde programmet tre API-begäranden som har säkerhetskopierats av en åtkomsttoken som erhållits via app + User Authentication-metoden utan MFA-verifiering.
- Den andra dagen gjorde programmet fem API-begäranden som har säkerhetskopierats av en åtkomsttoken som hämtades med endast app-autentisering.
- På den tredje dagen gjorde programmet två API-begäranden som har säkerhetskopierats av en åtkomsttoken som erhållits med hjälp av MFA-verifieringen app + User.
- Inga åtgärder har gjorts av någon av agenterna under de återstående fyra dagarna.
- De fem API-begärandena den andra dagen, som har säkerhetskopierats av en åtkomsttoken som hämtats via endast app-autentisering, utelämnas från måttet eftersom den inte använder användarautentiseringsuppgifter. Två av de återstående fem åtgärderna har säkerhetskopierats med en åtkomsttoken som erhållits med MFA-verifiering. Måttet visar därför 40%.

Om du vill veta vilka app + User-aktiviteter som resulterar i en icke-100% på det här måttet använder du filer:

- **Översikt över API-begäranden** för att förstå den övergripande MFA-statusen per program.
- **Alla API-begäranden** för att förstå detaljerna i varje API-begäranden som görs av användare av din klient, resultatet är begränsat till maximalt 10 000 senaste begär Anden för bättre nedladdning.

## <a name="actions-for-mfa-status-below-100"></a>Åtgärder för MFA-status under 100%

Vissa partner som har implementerat MFA kan se rapport måtten under 100%. Här följer några faktorer att ta reda på varför.

> [!NOTE]
> Du måste arbeta med någon från din organisation som är bekant med identitets hantering och MFA-implementering för din partner klient.

### <a name="implemented-mfa-for-your-partner-tenant"></a>Implementera MFA för din partner klient

Du måste implementera MFA för att din partner klient ska kunna uppnå efterlevnad. Mer information om hur du implementerar MFA finns i [säkerhets krav för att använda API: er för partner Center eller partner Center](partner-security-requirements.md).

>[!NOTE]
> MFA-mått beräknas dagligen och tar hänsyn till de åtgärder som utförts under de senaste sju dagarna. Om du bara har slutfört MFA-implementeringen för din partner klient kanske måtten ännu inte visar 100%.

### <a name="verify-mfa-on-all-user-accounts"></a>Verifiera MFA på alla användar konton

Ta reda på om din aktuella MFA-implementering omfattar alla användar konton eller bara vissa. Vissa MFA-lösningar är principbaserad och stöder användar undantag, medan andra kan kräva att du uttryckligen aktiverar MFA för varje användare. Kontrol lera att du inte har uteslutit någon användare från din aktuella MFA-implementering. Alla användar konton som undantas och loggar in på Partner Center för att utföra alla CSP-, CPV-eller Advisor-relaterade aktiviteter kan orsaka att måtten inte är 100%.

### <a name="review-your-mfa-conditions"></a>Granska dina MFA-villkor

Ta reda på om den aktuella implementeringen endast tillämpar MFA under vissa villkor. Vissa MFA-lösningar ger flexibilitet att endast genomdriva MFA när vissa villkor är uppfyllda. Till exempel kan användaren komma åt från okänd enhet eller okänd plats. En användare, som är aktive rad för MFA men inte krävs för att slutföra MFA-verifiering vid åtkomst till Partner Center, kan orsaka att måtten inte är 100%.

>[!NOTE]
>För partner som har implementerat MFA med hjälp av Azure AD Security-standardvärden är det viktigt att Observera att Multi-Factor Authentication för icke-administratörskonton kommer att tvingas utifrån risk. Användare tillfrågas endast om MFA under riskfyllda inloggnings försök (till exempel att användaren loggar in från en annan plats). Dessutom har användarna upp till 14 dagar på sig att registrera sig för MFA. Användare som inte har slutfört MFA-registrering kommer inte att begära MFA-verifiering under 14-dagars perioden. Därför förväntas vi att måtten inte får vara 100% för partner som har implementerat MFA med hjälp av standardinställningar för Azure AD-säkerhet.

### <a name="review-third-party-mfa-configurations"></a>Granska konfigurationer från tredje part MFA

Om du använder MFA-lösningen från tredje part kan du identifiera hur du integrerar den med Azure AD. I allmänhet finns det två metoder, inklusive Federation och anpassade kontroller:

* **Identitets Federation** – när Azure AD tar emot en autentiseringsbegäran omdirigerar Azure AD användaren till den federerade identitets leverantören för autentisering. Vid lyckad autentisering omdirigerar den federerade identitets leverantören användaren tillbaka till Azure AD tillsammans med en SAML-token. För att Azure AD ska kunna identifiera att användaren har slutfört MFA-verifiering vid autentisering till den federerade identitets leverantören, måste SAML-token innehålla *authenticationmethodsreferences* -anspråket (med värdet *multipleauthn*). Kontrol lera om den federerade identitets leverantören stöder utfärdande av ett sådant anspråk. Om så är fallet kontrollerar du om den federerade identitets leverantören har kon figurer ATS att göra det. Om anspråket saknas vet inte Azure AD (och därför Partner Center) att användaren har slutfört MFA-verifieringen och att det saknas ett anspråk kan orsaka att måttet inte är 100%.

* **Anpassad kontroll** – det går inte att använda anpassad kontroll för Azure AD för att identifiera om en användare har SLUTFÖRt MFA-verifiering via en MFA-lösning från tredje part. Därför kommer alla användare som har slutfört MFA-verifiering via en anpassad kontroll alltid att visas i Azure AD (och i sin tur Partner Center) som att de inte har slutfört MFA-verifiering. Där det är möjligt rekommenderar vi att du växlar till att använda identitets Federation i stället för anpassad kontroll vid integrering med Azure AD.

### <a name="identify-which-users-have-signed-in-to-partner-center-without-mfa"></a>Identifiera vilka användare som har loggat in på Partner Center utan MFA

Det kan vara bra att identifiera vilka användare som loggar in på Partner Center utan MFA-verifiering och verifiera dem mot din aktuella MFA-implementering. Du kan använda [Azure AD-inloggnings rapporten](/azure/active-directory/reports-monitoring/concept-sign-ins) för att ta reda på om en användare har SLUTFÖRt MFA-verifiering eller inte. Azure AD-inloggnings rapporten är för närvarande bara tillgänglig för partner som prenumererar på Azure AD Premium eller en O365-SKU, som innehåller Azure AD Premium (till exempel EMS).

## <a name="next-steps"></a>Nästa steg

- [Community för säkerhets vägledning för partner Center](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance)
- [Säkerhetskrav för Partnercenter](partner-security-requirements.md)
- [Vanliga frågor och svar om säkerhets krav för partner Center](partner-security-requirements-faq.md)
