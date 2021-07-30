---
title: Statusrapport för säkerhetskrav
ms.date: 10/30/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-enroll
description: Lär dig hur du kontrollerar dina säkerhetskravs kompatibilitet med statusrapporten för säkerhetskrav och MFA-rapporten i Partnercenter
author: isaiahwilliams
ms.author: iswillia
ms.localizationpriority: high
ms.topic: conceptual
ms.custom: SEOMAY.20
ms.openlocfilehash: db558062f5dab2a3f9ffbe99f7122a436f89d21f
ms.sourcegitcommit: ad1af627f5ee6b6e3a70655f90927e932cf4c985
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 07/29/2021
ms.locfileid: "114844555"
---
# <a name="security-requirements-status-report"></a>Statusrapport för säkerhetskrav

**Lämpliga roller:** CPV-| Global administratör

I den här artikeln förklaras statusrapporten för säkerhetskrav i Partnercenter. Den här rapporten ger mått om efterlevnad av [partnersäkerhetskrav för](partner-security-requirements.md) multifaktorautentisering (MFA) för användare i din partnerklientorganisation.

Om du vill komma åt den här rapporten i [Partnercenter](https://partner.microsoft.com/dashboard) **går Inställningar**  >  **till**  >  **Kontoinställningar Säkerhetskravstatus**. Rapporten uppdateras dagligen och visar inloggningsdata från de senaste sju dagarna.

>[!NOTE]
>Statusrapporten för säkerhetskrav stöds endast i Partnercenter. Den är inte tillgänglig i Microsoft Cloud for US Government Eller Microsoft Cloud Tyskland. Vi rekommenderar starkt att alla partner som gör en överträdelse via ett suveränt moln (amerikanska myndigheter och Tyskland) inför dessa nya säkerhetskrav omedelbart. Dessa partner behöver dock för närvarande inte uppfylla de nya säkerhetskraven. Microsoft tillhandahåller ytterligare information om tillämpningen av dessa säkerhetskrav för nationella moln i framtiden.

## <a name="security-status-metrics"></a>Mått för säkerhetsstatus

Statusrapporten för säkerhetskrav ger insikter om implementering av partner-MFA och innehåller mått om MFA-konfiguration och Partnercenter-aktiviteter på partnerklienter. I följande avsnitt förklaras dessa mått i detalj.

### <a name="mfa-configuration-on-a-partner-tenant"></a>MFA-konfiguration på en partnerklientorganisation

Måttet **Procentandel aktiverade användarkonton** med MFA framtvingat med hjälp av alternativen som anges här: visar procentandelen aktiverade användarkonton på din partnerklientorganisation som har MFA framtvingat. Du kan använda något av dessa [MFA-alternativ för](/azure/active-directory/fundamentals/concept-fundamentals-mfa-get-started) att uppnå efterlevnad. Dessa data samlas in och rapporteras dagligen. Till exempel:

- Contoso är en CSP-partner med 110 användarkonton i klientorganisationen och 10 av dessa användarkonton är inaktiverade. 
- Av resten av 100 användarkonton tillämpas 90 MFA med de tillhandahållna [MFA-alternativen](/azure/active-directory/fundamentals/concept-fundamentals-mfa-get-started). Därför visar måttet 90 %. 

### <a name="partner-center-requests-with-mfa"></a>Partner Center-begäranden med MFA

Varje gång dina anställda loggar in på Partnercenter för att arbeta eller, via API:er, hämta eller skicka data via Partnercenter, måste deras säkerhetsstatus utvärderas och spåras. Dina program och eventuella program från kontrollpanelen ingår även i spårning av säkerhetsstatus. Dessa data visas i mått under Procent **av begäranden till Partnercenter** med MFA och visar de senaste sju dagarna.

#### <a name="dashboard-mfa-verification"></a>MFA-verifiering på instrumentpanelen

Måttet **via Partnercenter-portalen** är relaterat till aktiviteter i instrumentpanelen i Partnercenter. Den mäter procentandelen åtgärder som utförs av användare som har slutfört MFA-verifieringen. Till exempel:

- Contoso är CSP-partner med två administratörsagenter, Jane och John.
- Den första dagen loggade Jane in på Partner Center-instrumentpanelen utan MFA-verifiering och gjorde tre åtgärder.
- Den andra dagen loggade John in på Partner Center-instrumentpanelen utan MFA-verifiering och gjorde fem åtgärder.
- Den tredje dagen loggade Jane in på instrumentpanelen i Partnercenter med MFA-verifiering och gjorde två åtgärder.
- Ingen av agenterna gjorde några åtgärder under de återstående fyra dagarna.
- Av de 10 åtgärderna som gjordes i sjudagarsfönstret gjordes två av användaren med MFA-verifiering. Därför visar måttet 20 %.

Använd **filportalbegäranden** utan MFA för att förstå vilken användare som loggade in på Partnercenter-instrumentpanelen utan att ha MFA-verifiering och tiden för senaste besök under rapportfönstret.

#### <a name="appuser-mfa-verification"></a>Verifiering av MFA för app+användare

Måttet **Via API eller SDK är relaterat** till app- och användarautentisering via Api-begäranden i Partnercenter. Den mäter procentandelen API-begäranden som görs med hjälp av en åtkomsttoken med MFA-anspråk. Till exempel:

- Fabrikam är en CSP-partner och har ett CSP-program som använder en blandning av app- och användarautentisering och appskyddade autentiseringsmetoder.
- Den första dagen gjorde programmet tre API-begäranden, som backades upp av en åtkomsttoken som erhölls via autentiseringsmetoden App+User utan MFA-verifiering.
- Den andra dagen gjorde programmet fem API-begäranden, som backades upp av en åtkomsttoken som erhölls med appbaserad autentisering.
- Den tredje dagen gjorde programmet två API-begäranden, som backades upp av en åtkomsttoken som erhölls med hjälp av autentiseringsmetoden App+Användare med MFA-verifiering.
- Ingen av agenterna gjorde några åtgärder under de återstående fyra dagarna.
- De fem API-begärandena den andra dagen, som backades upp av en åtkomsttoken som erhållits via appbaserad autentisering, utelämnas från måttet eftersom den inte använder autentiseringsuppgifter för användare. Av de återstående fem åtgärderna backades två av dem upp av en åtkomsttoken som erhölls med MFA-verifiering. Därför visar måttet 40 %.

Om du vill förstå vilka app- och användaraktiviteter som resulterar i icke-100 % för det här måttet använder du filer:

- **Sammanfattning av API-begäranden** för att förstå övergripande MFA-status per program.
- **Alla API-begäranden** för att förstå detaljerna i varje API-begäranden som görs av användare i din klientorganisation är resultatet begränsat till högst 10 000 senaste begäranden för bättre nedladdning.

## <a name="actions-for-mfa-status-below-100"></a>Åtgärder för MFA-status under 100 %

Vissa partner som har implementerat MFA kan se rapportmått under 100 %. Här är några faktorer att tänka på för att förstå varför.

> [!NOTE]
> Du måste arbeta med någon från din organisation som är bekant med identitetshantering och MFA-implementering för din partnerklientorganisation.

### <a name="implemented-mfa-for-your-partner-tenant"></a>Implementerat MFA för din partnerklientorganisation

Du måste implementera MFA för din partnerklientorganisation för att uppnå efterlevnad. Mer information om hur du implementerar MFA finns i [Säkerhetskrav för att använda Partner Center eller Partner Center-API:er.](partner-security-requirements.md)

>[!NOTE]
> MFA-mått beräknas dagligen och tar hänsyn till åtgärder som utförts under de senaste sju dagarna. Om du bara nyligen har slutfört MFA-implementeringen för din partnerklientorganisation kanske måtten ännu inte visar 100 %.

### <a name="verify-mfa-on-all-user-accounts"></a>Verifiera MFA för alla användarkonton

Förstå om din aktuella MFA-implementering omfattar alla användarkonton eller bara vissa. Vissa MFA-lösningar är principbaserade och stöder användar exkludering, medan andra kan kräva att du uttryckligen aktiverar MFA per användare. Kontrollera att du inte har exkluderat någon användare från din aktuella MFA-implementering. Alla användarkonton som undantas och loggar in på Partnercenter för att utföra aktiviteter relaterade till CSP, CPV eller Advisor kan orsaka att måtten inte är 100 %.

### <a name="review-your-mfa-conditions"></a>Granska dina MFA-villkor

Förstå om den aktuella implementeringen endast tillämpar MFA under specifika villkor. Vissa MFA-lösningar ger flexibilitet att endast framtvinga MFA när vissa villkor uppfylls. Användaren kan till exempel komma åt från en okänd enhet eller en okänd plats. En användare som är aktiverad för MFA men inte behöver slutföra MFA-verifiering vid åtkomst till Partnercenter kan orsaka att måtten inte är 100 %.

>[!NOTE]
>För partner som har implementerat MFA med standardvärden för Azure AD-säkerhet är det viktigt att observera att multifaktorautentisering för icke-administratörskonton tillämpas baserat på risker. Användarna uppmanas endast att ange MFA vid riskfyllda inloggningsförsök (till exempel om användaren loggar in från en annan plats). Dessutom har användarna upp till 14 dagar på sig att registrera sig för MFA. Användare som inte har slutfört MFA-registreringen kommer inte att behöva verifiera MFA under 14-dagarsperioden. Därför förväntas måtten inte vara 100 % för partner som har implementerat MFA med hjälp av Azure AD-säkerhetsstandarder.

### <a name="review-third-party-mfa-configurations"></a>Granska MFA-konfigurationer från tredje part

Om du använder en MFA-lösning från tredje part identifierar du hur du integrerar den med Azure AD. I allmänhet finns det två metoder, inklusive federationskontroller och anpassade kontroller:

* **Identitetsfederation** – När Azure AD tar emot en autentiseringsbegäran omdirigerar Azure AD användaren till den federerade identitetsprovidern för autentisering. Vid lyckad autentisering omdirigerar den federerade identitetsprovidern användaren tillbaka till Azure AD tillsammans med en SAML-token. För att Azure AD ska kunna identifiera att användaren har slutfört MFA-verifieringen vid autentisering till den federerade identitetsprovidern måste SAML-token innehålla *autentiseringsmethodsreferences-anspråket* (med värdet *multipleauthn*). Kontrollera om den federerade identitetsprovidern stöder utfärdande av ett sådant anspråk. I så fall kontrollerar du om den federerade identitetsprovidern har konfigurerats för att göra det. Om anspråket saknas vet Inte Azure AD (och därför Partnercenter) att användaren har slutfört MFA-verifieringen och att anspråket saknas kan göra att måttet inte är 100 %.

* **Anpassad kontroll** – Azure AD Custom Control kan inte användas för att identifiera om en användare har slutfört MFA-verifiering via en MFA-lösning från tredje part. Därför visas alla användare som har slutfört MFA-verifiering via en anpassad kontroll alltid för Azure AD (och i sin tur Partnercenter) som att de inte har slutfört MFA-verifieringen. Där det är möjligt rekommenderar vi att du växlar till att använda identitetsfederation i stället för anpassad kontroll vid integrering med Azure AD.

### <a name="identify-which-users-have-signed-in-to-partner-center-without-mfa"></a>Identifiera vilka användare som har loggat in på Partnercenter utan MFA

Det kan vara bra att identifiera vilka användare som loggar in på Partnercenter utan MFA-verifiering och verifiera dem mot din aktuella MFA-implementering. Du kan använda [Azure AD-inloggningsrapporten för att](/azure/active-directory/reports-monitoring/concept-sign-ins) ta reda på om en användare har slutfört MFA-verifieringen eller inte. Azure AD-inloggningsrapporten är för närvarande endast tillgänglig för partner som prenumererar på Azure AD Premium eller en O365-SKU, vilket omfattar Azure AD Premium (till exempel EMS).

## <a name="next-steps"></a>Nästa steg

- [Gruppgrupp för säkerhetsvägledning i Partnercenter](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance)
- [Säkerhetskrav för Partnercenter](partner-security-requirements.md)
- [Vanliga frågor och svar om säkerhetskrav för Partnercenter](partner-security-requirements-faq.yml)
