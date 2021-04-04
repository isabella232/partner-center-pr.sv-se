---
title: Kräva Multi-Factor Authentication (MFA) för din partner klient
ms.topic: article
ms.date: 10/29/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Lär dig hur kräva MFA för dina partner klienter kan skydda din åtkomst till kund resurser. Innehåller exempel scenarier.
author: isaiahwilliams
ms.author: iswillia
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 21e0ebd58835be34f9cc161072ff3690b30abf57
ms.sourcegitcommit: 10765386b2df0d4c2e8da9b302a692f452e1090d
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/31/2021
ms.locfileid: "106086370"
---
# <a name="mandating-multi-factor-authentication-mfa-for-your-partner-tenant"></a>Kräva Multi-Factor Authentication (MFA) för din partner klient

**Lämpliga roller**

- Administratörs agent
- Försäljnings agent
- Support agent
- Faktureringsadministratör
- Global administratör

Den här artikeln innehåller detaljerade exempel och rikt linjer för kräva Multi-Factor Authentication (MFA) i Partner Center. Syftet med den här funktionen är att hjälpa partners att skydda sin åtkomst till kund resurser mot autentiseringsuppgifter som komprometteras. Partner krävs för att genomdriva MFA för alla användar konton i sin partner klient, inklusive gäst användare. Användare kommer att tilldelas fullständig MFA-verifiering för följande områden:

- [Instrument panel för partner Center](#partner-center-dashboard)
- [Partner Center-API](#partner-center-api)
- [Partner delegerad administration](#partner-delegated-administration)

Större och fort löp ande säkerhets-och integritets skydd är bland våra främsta prioriteringar och vi fortsätter att hjälpa våra partner att skydda sina kunder och klienter. Alla partner som deltar i CSP-programmet (Cloud Solution Provider), på kontroll panelens leverantörer (CPVs) och rådgivare bör implementera [säkerhets kraven för partner](partner-security-requirements.md) för att vara kompatibla.

För att hjälpa våra partner att skydda sina företag och kunder från identitets stöld och obehörig åtkomst har vi aktiverat ytterligare säkerhets skydd för partner klienter som bestämmer sig för att verifiera MFA. 

## <a name="partner-center-dashboard"></a>Instrument panel för partner Center

Vissa sidor på instrument panelen i Partner Center är MFA-skyddade, inklusive:

- Alla sidor på fliken **kunder** , t. ex. alla sidor som kan nås via följande URL: https://partner.microsoft.com/commerce/*
- Alla sidor på fliken **Support > kund förfrågningar** , t. ex. sidan som nås under https://partner.microsoft.com/dashboard/support/csp/customers/*
- Faktureringssida

I följande tabell visas vilka användar typer som har behörighet att komma åt dessa MFA-skyddade sidor (och därför påverkas av den här funktionen).


| MFA-skyddad sida       | Administratörs agenter      |  Försäljnings agenter     |   Support agenter     | Global administratör      |  Faktureringsadministratör     | 
|---    |---    |---    |---    |---    |---    |
| Fliken alla sidor under kunder      |   x    |    x   |  x     |       |       |
| Fliken för alla sidor under support > kund förfrågningar     | x      |       |    x   |       |       |
| Faktureringssida     |   x    |       |       |    x   |   x    |

Om du försöker komma åt någon av dessa sidor och du inte har slutfört MFA-verifieringen tidigare, måste du göra det. Andra sidor på Partner Center som sidan Översikt, Service Health status kontroll sidan kräver inte MFA.

## <a name="verification-examples"></a>Verifierings exempel

Tänk på följande exempel för att illustrera hur verifiering fungerar i instrument panelen för partner Center.

### <a name="example-1-partner-has-implemented-azure-ad-mfa"></a>Exempel 1: partner har implementerat Azure AD MFA

1. Jane arbetar för CSP contoso. Contoso har implementerat MFA för alla användare under contoso partner klient organisation med hjälp av Azure Active Directory (Azure AD) MFA.

2. Jane startar en ny webbläsarsession och navigerar till översikts sidan för instrument panelen i Partner Center (som inte är MFA-skyddad). Partner Center omdirigerar Jane till Azure AD för att logga in.

3. På grund av den befintliga installationen av Azure AD MFA från contoso krävs Jane för att slutföra MFA-verifieringen. Vid lyckad inloggning och MFA-verifiering omdirigeras Jane tillbaka till översikts sidan för partner Center Dashboard.

4. Jane försöker komma åt en av MFA-skyddade sidor i Partner Center. Eftersom Jane redan har slutfört MFA-verifiering under inloggningen tidigare, kan Jane komma åt den MFA-skyddade sidan utan att behöva gå igenom MFA-verifieringen igen.

### <a name="example-2-partner-has-implemented-third-party-mfa-using-identity-federation"></a>Exempel 2: partner har implementerat MFA från tredje part med identitets Federation

1. Trent fungerar för CSP Wingtip. Wingtip har implementerat MFA för alla användare under en Wingtip partner klient med MFA från tredje part, som är integrerat med Azure AD via identitets Federation.

2. Trent startar en ny webbläsarsession och navigerar till översikts sidan för partner Center Dashboard (som inte är MFA-skyddad). Partner Center omdirigerar Trent till Azure AD för att logga in.

3. Eftersom Wingtip har konfigurerat identitets Federation omdirigerar Azure AD Trent till den federerade identitets leverantören för att slutföra inloggning och MFA-verifiering. Vid lyckad inloggning och MFA-verifiering omdirigeras Trent tillbaka till Azure AD och sedan till översikts sidan för partner Center Dashboard.

4. Trent försöker komma åt en av MFA-skyddade sidor i Partner Center. Eftersom Trent redan har slutfört MFA-verifiering under inloggningen tidigare, kan Trent komma åt den MFA-skyddade sidan utan att behöva gå igenom MFA-verifieringen igen.

### <a name="example-3-partner-hasnt-implemented-mfa"></a>Exempel 3: partnern har inte implementerat MFA

1. John arbetar för CSP fabrikam. Fabrikam har inte implementerat MFA för användare under Fabrikam partner klient organisation.

2. John startar en ny webbläsarsession och navigerar till översikts sidan för instrument panelen i Partner Center (som inte är MFA-skyddad). Partner Center omdirigerar John till Azure AD för att logga in.

3. Eftersom Fabrikam inte har implementerat MFA krävs inte John för att slutföra MFA-verifieringen. Vid lyckad inloggning omdirigeras John till översikts sidan för partner Center-instrumentpanelen.

4. John försöker komma åt en av MFA-skyddade sidor i Partner Center. Eftersom John inte har slutfört MFA-verifieringen omdirigerar Partner Center John till Azure AD för att slutföra MFA-verifieringen. Eftersom det är första gången John krävs för att slutföra MFA, så begär John även att [registrera sig för MFA](#mfa-registration-experience). Vid lyckad MFA-registrering och MFA-verifiering kan John nu komma åt den MFA-skyddade sidan.

5. En annan dag innan Fabrikam implementerar MFA för en användare startar John en ny webbläsarsession och navigerar till översikts sidan för partner Center Dashboard (som inte är MFA-skyddad). Partner Center omdirigerar John till Azure AD för att logga in utan MFA-prompt. 

6. John försöker komma åt en av MFA-skyddade sidor i Partner Center. Eftersom John inte har slutfört MFA-verifieringen omdirigerar Partner Center John till Azure AD för att slutföra MFA-verifieringen. Eftersom John har registrerat MFA, så den här gången uppmanas han/hon bara att slutföra MFA-verifieringen.

> [!NOTE]
>Åtgärd: företags administratörer har [tre alternativ](partner-security-requirements.md#implementing-multi-factor-authentication) för att implementera MFA.

## <a name="partner-center-api"></a>Partner Center-API

Partner Center API stöder både app-only-autentisering och app + användarautentisering. 

När app + User Authentication används kräver Partner Center MFA-verifiering. Mer specifikt, när ett partner program vill skicka en API-begäran till Partner Center, måste det innehålla en åtkomsttoken i begärans Authorization-huvud. 

> [!NOTE]
>[Ramverket för säkra program modeller](/partner-center/develop/enable-secure-app-model) är ett skalbart ramverk för autentisering av CSP-partner och CPVs via Microsoft Azure MFA-arkitektur vid anrop till API: er för partner Center. Du måste implementera det här ramverket innan du aktiverar MFA på din klient. 

När Partner Center får en API-begäran med en åtkomsttoken som hämtats med app + User Authentication, kommer Partner Center-API: et att söka efter värdet *MFA* i *AMR-anspråk (Authentication Method Reference)* . Du kan använda en JWT-avkodare för att kontrol lera om en åtkomsttoken innehåller det förväntade AMR-värdet (Authentication Method Reference) eller inte:

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

Om värdet finns, avslutar Partner Center att MFA-kontrollen har slutförts och bearbetar API-begäran. Om värdet inte finns, avvisar API: t för API: et begäran med följande svar:

``` csharp
HTTP/1.1 401 Unauthorized - MFA required
Transfer-Encoding: chunked
Request-Context: appId=cid-v1:03ce8ca8-8373-4021-8f25-d5dd45c7b12f
WWW-Authenticate: Bearer error="invalid_token"
Date: Thu, 14 Feb 2019 21:54:58 GMT
```

När App-Only autentisering används, kommer de API: er som stöder App-Only autentisering att fungera kontinuerligt utan att kräva MFA.

## <a name="partner-delegated-administration"></a>Partner delegerad administration

Partner konton, inklusive administratörs agenter och support agenter, kan använda sina partner delegerade administratörs behörigheter för att hantera kund resurser via Microsoft Online Services-portaler, kommando rads gränssnitt (CLI) och API: er (med hjälp av app + User Authentication).

### <a name="using-service-portals"></a>Använda service portaler

Vid åtkomst till Microsoft Online Services-portaler med administratörs behörigheten partner delegerad (admin-on-of) för att hantera kund resurser, kräver många av dessa portaler partner kontot för att autentisera interaktivt, med kund Azure AD-klienten inställd som autentiserings kontext – partner kontot krävs för att logga in på kund innehavaren.

När Azure AD tar emot sådana autentiseringsbegäranden kräver det partner kontot för att slutföra MFA-verifieringen. Det finns två möjliga användar upplevelser, beroende på om partner kontot är en hanterad eller federerad identitet:

- Om partner kontot är en **hanterad** identitet uppmanas användaren att slutföra MFA-verifieringen direkt i Azure AD. Om partner kontot inte har registrerats för MFA med Azure AD innan, uppmanas användaren att [slutföra MFA-registreringen](#mfa-registration-experience) först.

- Om partner kontot är en **federerad** identitet är upplevelsen beroende av hur partner administratören har konfigurerat Federation i Azure AD. När du konfigurerar Federation i Azure AD kan partner administratören ange för Azure AD om den federerade identitets leverantören stöder MFA eller inte. I så fall omdirigerar Azure AD användaren till den federerade identitets leverantören för att slutföra MFA-verifieringen. Annars uppmanas användaren av Azure AD direkt att slutföra MFA-verifieringen. Om partner kontot inte har registrerats för MFA med Azure AD innan, uppmanas användaren att [slutföra MFA-registreringen](#mfa-registration-experience) först.

Den övergripande upplevelsen liknar det scenario där en slutkunds klient har implementerat MFA för sina administratörer. Till exempel har kund innehavaren aktiverat [standardinställningar för Azure AD-säkerhet](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults), som kräver att alla konton med administratörs behörighet loggar in på kund innehavaren med MFA-verifiering, inklusive administratörs agenter och support agenter. I test syfte kan partners aktivera [Azure AD-säkerhetsvärden](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) i kund klienten och sedan försöka använda partner delegerade administrations privilegier för att få åtkomst till kund innehavaren.

> [!NOTE]
> Alla Microsoft Online Service portaler kräver inte att partner konton loggar in på kund innehavaren vid åtkomst till kund resurser med hjälp av partner delegerade administratörs privilegier. I stället behöver de bara partner kontona för att logga in på partner klient organisationen. Ett exempel är administrations centret för Exchange. Med tiden förväntar vi dessa portaler att kräva att partner konton loggar in på kund innehavaren när du använder partner delegerade administratörs privilegier.

### <a name="using-service-apis"></a>Använda tjänst-API: er

Vissa API: er för Microsoft Online Services (till exempel Azure Resource Manager, Azure AD graf, Microsoft Graph osv.) support partner som använder partner delegerade administratörs behörighet för att hantera kund resurser program mässigt. Om du vill använda en partner delegerad administratörs behörighet med dessa API: er måste partner programmet inkludera en åtkomsttoken i huvud för API-begäran, där åtkomsttoken erhålls genom att ha ett partner användar konto för autentisering med Azure AD, med kunden Azure AD inställd som autentiserings kontext. Partner programmet måste ha ett partner användar konto logga in på kund klienten.

När Azure AD tar emot, till exempel autentiseringsbegäran, kräver Azure AD partner användar kontot för att slutföra MFA-verifieringen. Om partner användar kontot inte har registrerats för MFA förut uppmanas användar kontot att slutföra MFA-registreringen först.

Alla partner program som är integrerade med dessa API: er med hjälp av partner delegerade administratörs behörigheter påverkas av den här funktionen. För att se till att partner program kan fortsätta att arbeta med dessa API: er utan avbrott:

- Partner måste undvika att använda en icke-interaktiv autentiseringsmetod för användare med Azure AD för att få åtkomst-token. När du använder en icke-interaktiv autentiseringsmetod för användare, till exempel [lösen ords flöde](https://github.com/AzureAD/azure-activedirectory-library-for-dotnet/wiki/Acquiring-tokens-with-username-and-password), kan inte Azure AD uppmana användaren att slutföra MFA-verifieringen. Partner måste växla till att använda interaktiv autentiseringsmetod för användare, till exempel [OpenID Connect-flöde](/azure/active-directory/develop/v1-protocols-openid-connect-code) i stället.

- Vid interaktiv användarautentisering bör partnern använda ett partner användar konto som redan har Aktiver ATS för MFA. När du tillfrågas av Azure AD kan partnern slutföra MFA-registrering och MFA-verifiering under inloggningen.

- Detta liknar det scenario där en slutkunds klient har implementerat MFA för sina administratörer. Till exempel har kund innehavaren aktiverat [standardinställningar för Azure AD-säkerhet](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults), som kräver att alla användar konton har administratörs behörighet för att logga in på kund innehavaren med MFA-verifiering, inklusive administratörs agenter och support agenter. I test syfte kan partners aktivera [Azure AD-säkerhetsvärden](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) i kund klienten och sedan försöka använda partner delegerade administrations behörigheter för att program mässigt få åtkomst till kund klienten.

### <a name="mfa-registration-experience"></a>MFA-registrerings upplevelse

Om partner kontot inte har registrerats för MFA innan kan du vid MFA-verifieringen uppmana användaren att slutföra MFA-registreringen först:

:::image type="content" source="images/MfaRegistration1.png" alt-text="MFA-registrering steg 1":::

När du klickar på **Nästa** uppmanas användaren att välja från en lista över verifierings metoder.

:::image type="content" source="images/MfaRegistration2.png" alt-text="MFA-registrering steg 2":::

Vid lyckad registrering måste användaren slutföra MFA-verifieringen baserat på den verifiering som användaren valt.
 
## <a name="list-of-common-issues"></a>Lista över vanliga problem

Innan du ansöker om [tekniskt undantag](#how-to-submit-a-request-for-technical-exception) från MFA-kravet kan du läsa listan över vanliga problem som har rapporter ATS av andra partner för att förstå om din begäran är giltig.

#### <a name="issue-1-partner-needs-more-time-to-implement-mfa-for-their-partner-agents"></a>Problem 1: partner behöver mer tid för att implementera MFA för sina partner agenter
En partner har inte startat eller håller fortfarande på att implementera MFA för sina partner agenter som behöver åtkomst till Microsoft Online Services-portaler med hjälp av partner delegerade administrations behörigheter för att hantera kund resurser. Partnern behöver mer tid för att slutföra MFA-implementeringen. Är det här problemet en giltig orsak till det tekniska undantaget?

**Svar**: Nej. Partner måste göra planer för att implementera MFA för sina användare för att undvika avbrott.

> [!NOTE]
> Även om partnern inte har implementerat MFA för sina partner agenter, kan partner agenterna fortfarande komma åt Microsoft Online Services portaler med delegerad administrations behörighet, förutsatt att de kan slutföra MFA-registrering och MFA-verifiering när de uppmanas att logga in på kund klienten. Att slutföra MFA-registreringen aktiverar inte användaren för MFA automatiskt.

##### <a name="issue-2-partner-has-not-implemented-mfa-for-user-accounts-not-using-delegated-admin-privileges"></a>Problem 2: partner har inte implementerat MFA för användar konton som inte använder delegerad administratörs behörighet
En partner har vissa användare i sina partner innehavare som inte behöver åtkomst till Microsoft Online Services-portaler för att hantera kund resurser med hjälp av partner delegerade administrations privilegier. Partnern håller på att implementera MFA för dessa användare och behöver mer tid för att slutföras. Är det här problemet en giltig orsak till det tekniska undantaget?

**Svar**: Nej. Eftersom dessa användar konton inte använder partner delegerade administrations behörigheter för att hantera kund resurser, behöver de inte logga in på kund klienten. De kommer inte att påverkas av Azure AD som kräver MFA-verifiering vid inloggning till kund innehavaren.

##### <a name="issue-3-partner-has-not-implemented-mfa-for-user-service-accounts"></a>Problem 3: partnern har inte implementerat MFA för användar tjänst konton
En partner har vissa användar konton i sina partner klienter, vilka används av enheter som tjänst konton. Detta är konton med låg behörighet som inte kräver åtkomst Partner Center eller Microsoft Online Services-portaler för att hantera kund resurser med hjälp av partner delegerade administrations privilegier. Är det här problemet en giltig orsak till det tekniska undantaget?

**Svar**: Nej. Eftersom dessa användar konton inte använder partner delegerade administrations behörigheter för att hantera kund resurser, behöver de inte logga in på kund klienten. De kommer inte att påverkas av Azure AD som kräver MFA-verifiering vid inloggning till kund innehavaren.

##### <a name="issue-4-partner-cannot-implement-mfa-using-ms-authenticator-app"></a>Problem 4: partner kan inte implementera MFA med MS Authenticator-appen
En partner har en princip för "städa skriv bord", som inte tillåter att anställda ansluter sina personliga enheter till sitt arbets utrymme. Utan åtkomst till sina personliga mobila enheter kan medarbetarna inte installera MS Authenticator-appen, vilket är den enda MFA-verifiering som stöds av standardinställningar för Azure AD-säkerhet. Är det här problemet en giltig orsak till det tekniska undantaget?

**Svar**: Nej, detta är inte en giltig orsak till det tekniska undantaget. Partnern bör överväga följande alternativ, så att deras anställda fortfarande kan slutföra MFA-verifieringen vid åtkomst till Partner Center:
- Partner kan också registrera sig för Azure AD Premium eller tredjeparts MFA-lösningar (som är kompatibla med Azure AD), vilket kan ge ytterligare verifierings metoder.

##### <a name="issue-5-partner-cannot-implement-mfa-due-to-the-use-of-legacy-authentication-protocols"></a>Problem 5: partner kan inte implementera MFA på grund av användning av bakåtkompatibla autentiseringsprotokoll
En partner har vissa partner agenter som fortfarande använder bakåtkompatibla autentiseringsprotokoll, som inte är MFA-kompatibla. Användarna använder till exempel fortfarande Outlook 2010, som baseras på bakåtkompatibla autentiseringsprotokoll. Om du aktiverar MFA för dessa partner agenter avbryts användningen av bakåtkompatibla autentiseringsprotokoll.

**Svar**: Nej, detta är inte en giltig orsak till det tekniska undantaget. Partner rekommenderar starkt att de flyttas bort från användningen av bakåtkompatibla autentiseringsprotokoll på grund av potentiella säkerhets konsekvenser eftersom dessa protokoll inte kan skyddas med MFA-verifiering och är mycket mer sårbara för komprometterande autentiseringsuppgifter. Om det inte finns något alternativ för att flytta bort från användningen av äldre autentiseringsprotokoll, bör partners överväga att registrera sig för Azure AD Premium, vilket stöder användning av program lösen ord. Program lösen ord är ett systemgenererat lösen ord som genereras av systemet och är vanligt vis starkare än de som genereras av det mänskliga lösen ordet. Genom att använda lösen ord för program kan partners implementera MFA för sina användare, och samtidigt återgå till program lösen ord för äldre autentiseringsprotokoll.

Läs artikeln om grundläggande autentisering [och Exchange Online](https://techcommunity.microsoft.com/t5/exchange-team-blog/basic-auth-and-exchange-online-february-2020-update/ba-p/1191282) för att förstå den senaste planen om stöd för äldre autentisering för Outlook, och följ [Exchange Team-bloggen](https://techcommunity.microsoft.com/t5/exchange-team-blog/bg-p/Exchange) för att få de kommande nyheterna. 

> [!NOTE]
> Även om partnern inte har implementerat MFA för sina partner agenter, kan partner agenterna fortfarande komma åt Microsoft Online Services portaler med delegerad administrations behörighet, förutsatt att de kan slutföra MFA-registrering och MFA-verifiering när de uppmanas att logga in på kund klienten. Att slutföra MFA-registreringen aktiverar inte användaren för MFA automatiskt.

##### <a name="issue-6-partner-has-implemented-third-party-mfa-that-isnt-recognized-by-azure-ad"></a>Problem 6: partner har implementerat MFA från tredje part som inte känns igen av Azure AD
En partner har implementerat MFA för sina användare med hjälp av en MFA-lösning från tredje part. Partnern kan dock inte korrekt konfigurera MFA-lösningen från tredje part som ska vidarebefordras till Azure AD om MFA-verifieringen har slutförts under användarautentisering. Är detta en giltig orsak till det tekniska undantaget?

**Svar**: Ja, det här problemet kan anses vara en giltig orsak till ett tekniskt undantag. Innan du skickar en begäran om tekniskt undantag bör du kontrol lera med leverantören av MFA-lösningen från tredje part att MFA-lösningen inte kan konfigureras för att flöda *authenticationmethodsreferences* -anspråket (med värdet *Multipleauthn*) till Azure AD för att indikera att MFA-verifieringen har slutförts under användarautentisering. När du skickar en begäran om tekniskt undantag måste du ange information om vilken MFA-lösning från tredje part som används och ange integrations metoden (till exempel via identitets Federation eller användning av anpassad Azure AD-kontroll) och ange följande information i den tekniska undantags förfrågan som stöd dokument:

- MFA-konfigurationer från tredje part.

- Resultatet av [testet av partner säkerhets kraven](/powershell/partnercenter/test-partner-security-requirements) som körs av MFA-aktiverade konto från tredje part.

- Inköps ordern för MFA-lösningen från tredje part som du använder eller som du planerar att använda.

## <a name="how-to-submit-a-request-for-technical-exception"></a>Så här skickar du en begäran om tekniskt undantag

Partner kan ansöka om tekniskt undantag för att förhindra MFA-verifiering om de stöter på tekniska problem med Microsoft Online Services och det inte finns någon genomförbar lösning eller lösning. Läs igenom [listan med vanliga problem](#list-of-common-issues) i föregående avsnitt innan du gör detta.

Så här skickar du en begäran om tekniskt undantag:

1. Logga in på Partner Center som global administratör eller administratörs agent.

2. Skapa en ny partner tjänst förfrågan genom att navigera till **support support**  >  **förfrågningar** och välja **ny begäran**.

3. Sök efter **MFA-begäran om undantag** i sökrutan. eller Välj **CSP** från kategori och välj sedan **konton, onboarding, åtkomst** från ämne och välj **MFA-Request för Exception** i underavsnittet och välj sedan **Nästa steg**.

4. Ange information som krävs för att skicka en tjänstbegäran för tekniskt undantag och välj **Skicka**.

Microsoft kan ta upp till tre arbets dagar för att tillhandahålla ett svar på en begäran om tekniskt undantag.

## <a name="next-steps"></a>Nästa steg

 - [Status för partner säkerhets krav](partner-security-compliance.md)