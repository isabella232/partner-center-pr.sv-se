---
title: Använda multifaktorautentisering (MFA) för din partnerklientorganisation
ms.topic: article
ms.date: 10/29/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-account
description: Lär dig hur du kan skydda din åtkomst till kundresurser genom att använda MFA för dina partnerklienter. Innehåller exempelscenarier.
author: isaiahwilliams
ms.author: iswillia
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 7224edb3d0cf04161739a31e537f4c9649cee375112a532b0a53503841c4add7
ms.sourcegitcommit: 121f1b9cbd88faeba60dc9b475f9c0647cdc933c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/06/2021
ms.locfileid: "115694529"
---
# <a name="mandating-multi-factor-authentication-mfa-for-your-partner-tenant"></a>Använda multifaktorautentisering (MFA) för din partnerklientorganisation

**Lämpliga roller:** Administratörsagent | Försäljningsagent | Supportagent för | Faktureringsadministratörskonto | Global administratör

Den här artikeln innehåller detaljerade exempel och vägledning för att använda multifaktorautentisering (MFA) i Partnercenter. Syftet med den här funktionen är att hjälpa partner att skydda sin åtkomst till kundresurser mot kompromettering av autentiseringsuppgifter. Partner måste framtvinga MFA för alla användarkonton i partnerklientorganisationen, inklusive gästanvändare. Användare måste slutföra MFA-verifieringen inom följande områden:

- [Instrumentpanel i Partnercenter](#partner-center-dashboard)
- [Partner Center-API](#partner-center-api)
- [Delegerad partneradministration](#partner-delegated-administration)

Större och pågående skyddsmekanismer för säkerhet och sekretess är bland våra högsta prioriteter och vi fortsätter att hjälpa partner att skydda sina kunder och klienter. Alla partner som deltar i Molnlösningsleverantör-programmet (CSP), Kontrollpanelen-leverantörer (CPV) och rådgivare bör implementera [partnersäkerhetskraven](partner-security-requirements.md) för att efterleva kraven.

För att hjälpa partner att skydda sina företag och kunder från identitetsstöld och obehörig åtkomst har vi aktiverat ytterligare säkerhetsskydd för partnerklienter som behöver och verifiera MFA. 

## <a name="partner-center-dashboard"></a>Instrumentpanel i Partnercenter

Vissa sidor i instrumentpanelen i Partnercenter kommer att vara MFA-skyddade, inklusive:

- Alla sidor under **fliken** Kunder, t.ex. alla sidor som kan nås via följande URL: https://partner.microsoft.com/commerce/*
- Alla sidor under **fliken > Kundförfrågningar,** t.ex. sidan som nås under https://partner.microsoft.com/dashboard/support/csp/customers/*
- Faktureringssida

I följande tabell visas vilka användartyper som har behörighet att komma åt dessa MFA-skyddade sidor (och därför påverkas av den här funktionen).


| MFA-skyddad sida       | Administratörsagenter      |  Försäljningsagenter     |   Supportagenter     | Global administratör      |  Faktureringsadministratör     | 
|---    |---    |---    |---    |---    |---    |
| Alla sidor under fliken Kunder      |   x    |    x   |  x     |       |       |
| Alla sidor under fliken Support > Kundförfrågningar     | x      |       |    x   |       |       |
| Faktureringssida     |   x    |       |       |    x   |   x    |

Om du försöker komma åt någon av dessa sidor och inte har slutfört MFA-verifieringen tidigare måste du göra det. Andra sidor i Partnercenter, till exempel sidan Översikt, Service Health för statuskontroll kräver inte MFA.

## <a name="verification-examples"></a>Verifieringsexempel

För att illustrera hur verifiering fungerar på instrumentpanelen i Partnercenter kan du titta på följande exempel.

### <a name="example-1-partner-has-implemented-azure-ad-mfa"></a>Exempel 1: Partnern har implementerat Azure AD MFA

1. Jane arbetar för CSP Contoso. Contoso har implementerat MFA för alla sina användare under Contosos partnerklientorganisation med hjälp Azure Active Directory MFA (Azure AD).

2. Jane startar en ny webbläsarsession och går till översiktssidan för Partnercenter-instrumentpanelen (som inte är MFA-skyddad). Partner Center omdirigerar Jane till Azure AD för att logga in.

3. På grund av contosos befintliga Azure AD MFA-konfiguration krävs Jane för att slutföra MFA-verifieringen. Vid lyckad inloggning och MFA-verifiering omdirigeras Jane tillbaka till översiktssidan för instrumentpanelen i Partnercenter.

4. Jane försöker komma åt en av de MFA-skyddade sidorna i Partnercenter. Eftersom Jane redan har slutfört MFA-verifieringen under inloggningen tidigare kan Jane komma åt sidan MFA-skyddad utan att behöva gå igenom MFA-verifieringen igen.

### <a name="example-2-partner-has-implemented-third-party-mfa-using-identity-federation"></a>Exempel 2: Partnern har implementerat MFA från tredje part med hjälp av identitetsfederation

1. Wingtip arbetar för CSP Wingtip. Wingtip har implementerat MFA för alla sina användare under Wingtip-partnerklientorganisationen med hjälp av MFA från tredje part, som är integrerat med Azure AD via identitetsfederation.

2. Page startar en ny webbläsarsession och navigerar till översiktssidan för Partnercenter-instrumentpanelen (som inte är MFA-skyddad). Partner Center omdirigerar Arnold till Azure AD för att logga in.

3. Eftersom Wingtip har ställt in identitetsfederation omdirigerar Azure AD Arnold till den federerade identitetsprovidern för att slutföra inloggningen och MFA-verifieringen. Vid lyckad inloggning och MFA-verifiering omdirigeras Arnold tillbaka till Azure AD och sedan till översiktssidan för instrumentpanelen i Partnercenter.

4. Provar att komma åt en av de MFA-skyddade sidorna i Partnercenter. Eftersom Arnold redan har slutfört MFA-verifieringen under inloggningen tidigare, kan Arnold komma åt den MFA-skyddade sidan utan att behöva gå igenom MFA-verifieringen igen.

### <a name="example-3-partner-hasnt-implemented-mfa"></a>Exempel 3: Partnern har inte implementerat MFA

1. John arbetar för CSP Fabrikam. Fabrikam har inte implementerat MFA för någon användare under Fabrikam-partnerklientorganisationen.

2. John startar en ny webbläsarsession och går till översiktssidan för Partnercenter-instrumentpanelen (som inte är MFA-skyddad). Partner Center omdirigerar John till Azure AD för att logga in.

3. Eftersom Fabrikam inte har implementerat MFA behöver John inte slutföra MFA-verifieringen. Vid lyckad inloggning omdirigeras John tillbaka till översiktssidan för instrumentpanelen i Partnercenter.

4. John försöker komma åt en av de MFA-skyddade sidorna i Partnercenter. Eftersom John inte har slutfört MFA-verifieringen omdirigerar Partner Center John till Azure AD för att slutföra MFA-verifieringen. Eftersom det är första gången John måste slutföra MFA, begärs även John att registrera [sig för MFA](#mfa-registration-experience). Vid lyckad MFA-registrering och MFA-verifiering kan John nu komma åt sidan MFA-skyddad.

5. En annan dag innan Fabrikam implementerar MFA för någon användare startar John en ny webbläsarsession och går till översiktssidan för Partnercenter-instrumentpanelen (som inte är MFA-skyddad). Partner Center omdirigerar John till Azure AD för att logga in utan MFA-prompt. 

6. John försöker komma åt en av de MFA-skyddade sidorna i Partnercenter. Eftersom John inte har slutfört MFA-verifieringen omdirigerar Partner Center John till Azure AD för att slutföra MFA-verifieringen. Eftersom John har registrerat MFA ombeds han bara att slutföra MFA-verifieringen den här gången.

> [!NOTE]
>Åtgärd: Företagsadministratörer har [tre alternativ för](partner-security-requirements.md#implementing-multi-factor-authentication) att implementera MFA.

## <a name="partner-center-api"></a>Partner Center-API

Partnercenter-API:et stöder både appautentisering och app-/användarautentisering. 

När App+User-autentisering används kräver Partnercenter MFA-verifiering. Mer specifikt, när ett partnerprogram vill skicka en API-begäran till Partnercenter, måste det innehålla en åtkomsttoken i auktoriseringshuvudet för begäran. 

> [!NOTE]
>Det [Modell för säkra program ramverket](/partner-center/develop/enable-secure-app-model) är ett skalbart ramverk för autentisering av CSP-partner och CPV:er via MFA Microsoft Azure arkitekturen vid anrop till Partner Center-API:er. Du måste implementera det här ramverket innan du aktiverar MFA på din klientorganisation. 

När Partnercenter tar emot en API-begäran med en åtkomsttoken som erhållits med hjälp av app- och användarautentisering söker Partnercenter-API:et efter förekomsten av *MFA-värdet* i *AMR-anspråket (Authentication Method Reference).* Du kan använda en JWT-avkodare för att verifiera om en åtkomsttoken innehåller det förväntade AMR-värdet (Authentication Method Reference) eller inte:

``` csharp
{
  "aud": "https://api.partnercenter.microsoft.com",
  "iss": "https://sts.windows.net/df845f1a-7b35-40a2-ba78-6481de91f8ae/",
  "iat": 1549088552,
  "nbf": 1549088552,
  "exp": 1549092452,
  "acr": "1",
  "amr": [
    "pwd",
    "mfa"
  ],
  "appid": "23ec45a3-5127-4185-9eff-c8887839e6ab",
  "appidacr": "0",
  "family_name": "Adminagent",
  "given_name": "CSP",
  "ipaddr": "127.0.0.1",
  "name": "Adminagent CSP",
  "oid": "4988e250-5aee-482a-9136-6d269cb755c0",
  "scp": "user_impersonation",
  "tenant_region_scope": "NA",
  "tid": "df845f1a-7b35-40a2-ba78-6481de91f8ae",
  "unique_name": "Adminagent.csp@testtestpartner.onmicrosoft.com",
  "upn": "Adminagent.csp@testtestpartner.onmicrosoft.com",
  "ver": "1.0"
}
```

Om värdet finns drar Partnercenter slutsatsen att MFA-verifieringen har slutförts och bearbetar API-begäran. Om värdet inte finns avvisar Partner Center-API:et begäran med följande svar:

``` csharp
HTTP/1.1 401 Unauthorized - MFA required
Transfer-Encoding: chunked
Request-Context: appId=cid-v1:03ce8ca8-8373-4021-8f25-d5dd45c7b12f
WWW-Authenticate: Bearer error="invalid_token"
Date: Thu, 14 Feb 2019 21:54:58 GMT
```

När App-Only autentisering används kommer API:erna som stöder App-Only autentisering att fungera kontinuerligt utan att MFA krävs.

## <a name="partner-delegated-administration"></a>Delegerad partneradministration

Partnerkonton, inklusive administratörsagenter och supportagenter, kan använda sina partner-delegerade administratörsbehörigheter för att hantera kundresurser via Microsoft Online Services-portaler, kommandoradsgränssnitt (CLI) och API:er (med app- och användarautentisering).

### <a name="using-service-portals"></a>Använda tjänstportaler

Vid åtkomst till Microsoft Online Services-portaler med hjälp av partner-delegerade administratörsbehörigheter (Admin-On-Behalf-Of) för att hantera kundresurser kräver många av dessa portaler att partnerkontot autentiserar interaktivt, med kundens Azure AD-klientorganisation inställd som autentiseringskontext – partnerkontot krävs för att logga in på kundens klientorganisation.

När Azure AD tar emot sådana autentiseringsförfrågningar kräver det att partnerkontot slutför MFA-verifieringen. Det finns två möjliga användarupplevelser, beroende på om partnerkontot är en hanterad eller federerad identitet:

- Om partnerkontot är en **hanterad** identitet uppmanar Azure AD användaren att slutföra MFA-verifieringen direkt. Om partnerkontot inte har registrerats för MFA med Azure AD tidigare uppmanas användaren att [slutföra MFA-registreringen](#mfa-registration-experience) först.

- Om partnerkontot är en **federerad** identitet beror upplevelsen på hur partneradministratören har konfigurerat federation i Azure AD. När du ställer in federation i Azure AD kan partneradministratören ange för Azure AD om den federerade identitetsprovidern stöder MFA eller inte. I så fall omdirigerar Azure AD användaren till den federerade identitetsprovidern för att slutföra MFA-verifieringen. Annars uppmanar Azure AD användaren att slutföra MFA-verifieringen direkt. Om partnerkontot inte har registrerats för MFA med Azure AD tidigare uppmanas användaren att [slutföra MFA-registreringen](#mfa-registration-experience) först.

Den övergripande upplevelsen liknar scenariot där en slutanvändares klientorganisation har implementerat MFA för sina administratörer. Kundklientorganisationen har till exempel aktiverat Standardinställningar för Azure AD-säkerhet, vilket kräver att alla konton med administrativ behörighet loggar in på kundens klientorganisation med MFA-verifiering, inklusive [administratörsagenter](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)och supportagenter. I testsyfte kan partner aktivera [Standardinställningar](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) för Azure AD-säkerhet i kundklientorganisationen och sedan försöka använda partnerdelegier för att få åtkomst till kundklientorganisationen.

> [!NOTE]
> Alla Microsoft Online-tjänstportaler kräver inte partnerkonton för att logga in på kundklientorganisationen vid åtkomst till kundresurser med partnerdelegier. I stället kräver de bara partnerkonton för att logga in på partnerklientorganisationen. Ett exempel är Exchange Administrationscenter. Med tiden förväntar vi oss att dessa portaler kräver partnerkonton för att logga in på kundklientorganisationen när du använder delegerade administratörsbehörigheter för partner.

### <a name="using-service-apis"></a>Använda tjänst-API:er

Vissa API:er för Microsoft Online Services (till exempel Azure Resource Manager, Azure AD Graph, Microsoft Graph osv.) stöder partner som använder delegerade administratörsbehörigheter för partner för att programmatiskt hantera kundresurser. Om du vill använda partner-delegerade administratörsbehörigheter med dessa API:er måste partnerprogrammet inkludera en åtkomsttoken i auktoriseringshuvudet för API-begäran, där åtkomsttoken hämtas genom att ha ett partneranvändarkonto för autentisering med Azure AD, med kundens Azure AD inställt som autentiseringskontext. Partnerprogrammet måste ha ett partneranvändarkonto för att logga in på kundens klientorganisation.

När Azure AD tar emot till exempel en autentiseringsbegäran kräver Azure AD partneranvändarkontot för att slutföra MFA-verifieringen. Om partneranvändarkontot inte har registrerats för MFA tidigare uppmanas användarkontot att slutföra MFA-registreringen först.

Alla partnerprogram som är integrerade med dessa API:er med partnerdelegerade administratörsbehörigheter påverkas av den här funktionen. För att säkerställa att partnerprogram kan fortsätta att fungera med dessa API:er utan avbrott:

- Partnern måste undvika att använda icke-interaktiv användarautentiseringsmetod med Azure AD för att hämta åtkomsttoken. När du använder en icke-interaktiv användarautentiseringsmetod som lösenord [Flow](https://github.com/AzureAD/azure-activedirectory-library-for-dotnet/wiki/Acquiring-tokens-with-username-and-password)kan Azure AD inte uppmana användaren att slutföra MFA-verifieringen. Partnern måste växla till en interaktiv användarautentiseringsmetod, till exempel [OpenID Anslut flöde i](/azure/active-directory/develop/v1-protocols-openid-connect-code) stället.

- Under autentiseringsmetoden för interaktiv användare bör partnern använda ett partneranvändarkonto som redan är aktiverat för MFA. Alternativt kan partnern slutföra MFA-registreringen och MFA-verifieringen under inloggningen när du uppmanas av Azure AD.

- Detta liknar scenariot där en slutanvändares klientorganisation har implementerat MFA för sina administratörer. Kundklientorganisationen har till exempel aktiverat Standardinställningar för Azure AD-säkerhet, vilket kräver att alla användarkonton med [administratörsbehörighet](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)loggar in på kundens klientorganisation med MFA-verifiering, inklusive administratörsagenter och supportagenter. I testsyfte kan partner aktivera [Standardinställningar](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) för Azure AD-säkerhet i kundklientorganisationen och sedan försöka använda partnerdelegier för att programmatiskt komma åt kundens klientorganisation.

### <a name="mfa-registration-experience"></a>Registreringsupplevelse för MFA

Om partnerkontot inte har registrerats för MFA tidigare under MFA-verifieringen uppmanar Azure AD användaren att slutföra MFA-registreringen först:

:::image type="content" source="images/MfaRegistration1.png" alt-text="Registreringssteg 1 för MFA.":::

När användaren **klickar** på Nästa uppmanas han eller hon att välja från en lista över verifieringsmetoder.

:::image type="content" source="images/MfaRegistration2.png" alt-text="MFA-registrering steg 2.":::

Vid lyckad registrering måste användaren slutföra MFA-verifieringen baserat på den verifiering som valts av användaren.
 
## <a name="list-of-common-issues"></a>Lista över vanliga problem

Innan du söker [efter tekniska undantag](#how-to-submit-a-request-for-technical-exception) från MFA-kravet granskar du listan över vanliga problem som rapporterats av andra partner för att förstå om din begäran är giltig.

#### <a name="issue-1-partner-needs-more-time-to-implement-mfa-for-their-partner-agents"></a>Problem 1: Partnern behöver mer tid för att implementera MFA för sina partneragenter
En partner har inte startat eller håller fortfarande på att implementera MFA för sina partneragenter som behöver åtkomst till Microsoft Online Services-portaler med partnerdelegier för att hantera kundresurser. Partnern behöver mer tid för att slutföra MFA-implementeringen. Är det här problemet en giltig orsak till det tekniska undantaget?

**Svar:** Nej. Partnern måste göra planer för att implementera MFA för sina användare för att undvika störningar.

> [!NOTE]
> Även om partnern inte har implementerat MFA för sina partneragenter kan partneragenterna fortfarande komma åt Microsoft Online Services-portaler med partnerdelegerade administratörsbehörigheter förutsatt att de kan slutföra MFA-registrering och MFA-verifiering när de uppmanas att logga in på kundens klientorganisation. Om du slutför MFA-registreringen aktiveras inte användaren automatiskt för MFA.

##### <a name="issue-2-partner-has-not-implemented-mfa-for-user-accounts-not-using-delegated-admin-privileges"></a>Problem 2: Partnern har inte implementerat MFA för användarkonton som inte använder delegerade administratörsbehörigheter
En partner har vissa användare i sina partnerklienter som inte behöver åtkomst till Microsoft Online Services-portaler för att hantera kundresurser med hjälp av partnerdelegier för administration. Partnern är i full gång med att implementera MFA för dessa användare och behöver mer tid att slutföra. Är det här problemet en giltig orsak till det tekniska undantaget?

**Svar:** Nej. Eftersom dessa användarkonton inte använder delegerad administratörsbehörighet för partner för att hantera kundresurser behöver de inte logga in på kundens klientorganisation. De påverkas inte av att Azure AD kräver MFA-verifiering vid inloggning till kundens klientorganisation.

##### <a name="issue-3-partner-has-not-implemented-mfa-for-user-service-accounts"></a>Problem 3: Partnern har inte implementerat MFA för användarkonton
En partner har vissa användarkonton i sina partnerklienter, som används av enheter som tjänstkonton. Det här är konton med låg behörighet som inte kräver åtkomst till Partnercenter eller Microsoft Online Services-portaler för att hantera kundresurser med partnerdelegerade administratörsbehörigheter. Är det här problemet en giltig orsak till det tekniska undantaget?

**Svar:** Nej. Eftersom dessa användarkonton inte använder delegerad administratörsbehörighet för partner för att hantera kundresurser behöver de inte logga in på kundens klientorganisation. De påverkas inte av att Azure AD kräver MFA-verifiering vid inloggning till kundens klientorganisation.

##### <a name="issue-4-partner-cannot-implement-mfa-using-ms-authenticator-app"></a>Problem 4: Partnern kan inte implementera MFA med ms Authenticator appen
En partner har principen "clean desk" (rent skrivbord) som inte tillåter anställda att ta med sina personliga mobila enheter till sitt arbetsområde. Utan åtkomst till sina personliga mobila enheter kan de anställda inte installera MS Authenticator App, vilket är den enda MFA-verifiering som stöds av Azure AD-säkerhetsstandarder. Är det här problemet en giltig orsak till det tekniska undantaget?

**Svar:** Nej, det här är inte en giltig orsak till det tekniska undantaget. Partnern bör överväga följande alternativ, så att deras anställda fortfarande kan slutföra MFA-verifiering vid åtkomst till Partnercenter:
- Partner kan också registrera sig för Azure AD Premium MFA-lösningar från tredje part (kompatibla med Azure AD) som kan tillhandahålla ytterligare verifieringsmetoder.

##### <a name="issue-5-partner-cannot-implement-mfa-due-to-the-use-of-legacy-authentication-protocols"></a>Problem 5: Partnern kan inte implementera MFA på grund av användningen av äldre autentiseringsprotokoll
En partner har vissa partneragenter som fortfarande använder äldre autentiseringsprotokoll, som inte är MFA-kompatibla. Till exempel använder användarna fortfarande Outlook 2010, som baseras på äldre autentiseringsprotokoll. Om du aktiverar MFA för dessa partneragenter störs användningen av äldre autentiseringsprotokoll.

**Svar:** Nej, det här är inte en giltig orsak till det tekniska undantaget. Partner rekommenderas starkt att gå bort från användningen av äldre autentiseringsprotokoll på grund av potentiella säkerhetskonsekvenser eftersom dessa protokoll inte kan skyddas med MFA-verifiering och är mycket mer sårbara för kompromettering av autentiseringsuppgifter. Om det inte är ett alternativ att flytta från användningen av äldre autentiseringsprotokoll bör partner överväga att registrera sig för Azure AD Premium, som stöder användning av programlösenord. Programlösenord är systemgenererade lösenord en gång och är vanligtvis starkare än lösenord som genereras av människor. Genom att använda programlösenord kan partner implementera MFA för sina användare, samtidigt som de går tillbaka till programlösenord endast för äldre autentiseringsprotokoll.

Läs inlägget om [Basic-autentisering](https://techcommunity.microsoft.com/t5/exchange-team-blog/basic-auth-and-exchange-online-february-2020-update/ba-p/1191282) och Exchange Online för att förstå den senaste planen för stöd av äldre autentisering för Outlook och följ [Exchange teambloggen](https://techcommunity.microsoft.com/t5/exchange-team-blog/bg-p/Exchange) för att få de kommande nyheterna. 

> [!NOTE]
> Även om partnern inte har implementerat MFA för sina partneragenter kan partneragenterna fortfarande komma åt Microsoft Online Services-portaler med partnerdelegerade administratörsbehörigheter förutsatt att de kan slutföra MFA-registrering och MFA-verifiering när de uppmanas att logga in på kundens klientorganisation. Om du slutför MFA-registreringen aktiveras inte användaren automatiskt för MFA.

##### <a name="issue-6-partner-has-implemented-third-party-mfa-that-isnt-recognized-by-azure-ad"></a>Problem 6: Partnern har implementerat MFA från tredje part som inte känns igen av Azure AD
En partner har implementerat MFA för sina användare med hjälp av en MFA-lösning från tredje part. Partnern kan dock inte konfigurera MFA-lösningen från tredje part för att vidarebefordra till Azure AD att MFA-verifieringen har slutförts under användarautentisering. Är detta en giltig orsak till det tekniska undantaget?

**Svar:** Ja, det här problemet kan betraktas som en giltig orsak till tekniska undantag. Innan du skickar en begäran om tekniskt undantag ska du bekräfta med tredjepartsprovidern för MFA att MFA-lösningen inte kan konfigureras för att flöda *anspråket authenticationmethodsreferences* (med värdet *multipleauthn*) till Azure AD för att indikera att MFA-verifieringen har slutförts under användarautentisering. När du skickar en begäran om tekniskt undantag måste du ange information om den MFA-lösning från tredje part som används och ange integreringsmetod (till exempel via identitetsfederation eller användning av Azure AD Custom Control) och ange följande information i den tekniska undantagsbegäran som kompletterande dokument:

- MFA-konfigurationer från tredje part.

- Resultatet av Testa [partnersäkerhetskraven som körs](/powershell/partnercenter/test-partner-security-requirements) av det MFA-aktiverade kontot från tredje part.

- Inköpsordern för den MFA-lösning från tredje part som du använder eller som du planerar att använda.

## <a name="how-to-submit-a-request-for-technical-exception"></a>Så här skickar du en begäran om tekniskt undantag

Partner kan ansöka om tekniska undantag för att förhindra MFA-verifiering om de stöter på tekniska problem med Microsoft Online Services och det inte finns någon möjlig lösning eller lösning. Granska listan över vanliga [problem i föregående avsnitt innan du](#list-of-common-issues) gör det.

Så här skickar du en begäran om tekniskt undantag:

1. Logga in på Partnercenter som global administratör eller administratörsagent.

2. Skapa en ny partnertjänstbegäran genom att gå till  >  **Supportpartner supportbegäranden** och välja **Ny begäran.**

3. Sök efter **MFA – Begäran om** undantag i sökrutan. eller välj **CSP** från Kategori, välj **konton, registrering,** åtkomst från ämne, välj **sedan MFA –** begäran om undantag från underavsnittet och välj **sedan nästa steg.**

4. Ange information som begärs för att skicka en tjänstbegäran för tekniskt undantag och välj **Skicka**.

Microsoft kan ta upp till tre arbetsdagar för att ge ett svar på en begäran om tekniskt undantag.

## <a name="next-steps"></a>Nästa steg

 - [Status för partnersäkerhetskrav](partner-security-compliance.md)