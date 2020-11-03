---
title: Säkerhets krav för partner
ms.topic: article
ms.date: 10/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Introducerar partner kraven för att aktivera Multi-Factor Authentication (MFA) och anta modell ramverket för säker program.
author: vijvala
ms.author: vijvala
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 361a36adf40af67769a9a24ba1c485f2ad95b98c
ms.sourcegitcommit: 8a4a3de728532533276a88b1fd40c82b7a4ebb15
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 10/06/2020
ms.locfileid: "92531832"
---
# <a name="partner-security-requirements-for-partners-using-partner-center-or-partner-center-apis"></a>Partner säkerhets krav för partner som använder Partner Center-eller partner Center-API: er

**Gäller för**

- Alla partner i Cloud Solution Provider-programmet
  - Direkt fakturering
  - Indirekt Provider
  - Indirekt åter försäljare
- Alla leverantörer på kontroll panelen
- Alla rådgivare

**Lämpliga användare**

- Alla aktiverade användare, inklusive gäst användare

Större Sekretess skydd och säkerhet är bland våra främsta prioriteringar. Vi vet att det bästa skyddet är förebyggande och att vi bara är lika starka som vår svagaste länk. Därför behöver vi alla i vårt eko system för att agera och se till att lämpliga säkerhets skydd är på plats. För att hjälpa till att skydda partner och kunder, introducerar vi en uppsättning obligatoriska säkerhets krav för rådgivare, kontroll panels leverantörer och partner som ingår i Cloud Solution Provider-programmet.

## <a name="overview"></a>Översikt

Partner krävs för att tillämpa Multi-Factor Authentication för alla användar konton i sin partner klient. Villkoren som är kopplade till partner säkerhets kraven har lagts till i Microsoft partner Agreement. När det gäller rådgivare är samma avtals krav på plats.

Partner som inte implementerar de obligatoriska säkerhets kraven kommer inte att kunna använda Transact i Cloud Solution Provider-programmet eller hantera kund klienter som utnyttjar delegerade administratörs rättigheter, när dessa krav tillämpas. Dessutom kan partner som inte implementerar säkerhets kraven ge sitt deltagande i program i risk zonen.  

För att skydda dig och dina kunder, kräver vi partner att vidta följande åtgärder omedelbart:  

1. **Aktivera Multi-Factor Authentication (MFA) för alla användar konton i din partner klient** . Alla användar konton i din partner klient organisation (er) måste anropas av Multi-Factor Authentication (MFA) när de loggar in på Microsofts kommersiella moln tjänster eller när de är Transact i Cloud Solution Provider-programmet via partner Center eller via API: er.

2. **Anta ramverket för säker program modell** . Anta ramverket för säker program modell. Alla partners som integreras med API för partner Center måste anta modell program för säker program modell för appar och program för autentisering av appar och användar-pool.

    > [!IMPORTANT]
    > Vi rekommenderar starkt att partners implementerar den säkra program modellen för integrering med ett Microsoft API, till exempel Azure Resource Manager, Microsoft Graph eller utnyttjar automatisering, till exempel PowerShell som använder användar uppgifter, för att undvika avbrott när MFA tillämpas.

Aktivering av Multi-Factor Authentication (MFA) och införandet av ramverket för säkra program modeller hjälper till att skydda din infrastruktur och skydda kundens data från potentiella säkerhets risker, till exempel att identifiera stölder eller andra bedrägeriers incidenter.  

## <a name="actions-that-you-need-to-take"></a>Åtgärder som du behöver vidta

För att uppfylla kraven på partner säkerheten måste du tvinga Multi-Factor Authentication för varje användar konto i din partner klient. Det kan du göra på något av följande sätt:

- Implementera [standardinställningar för Azure AD-säkerhet](/azure/active-directory/conditional-access/concept-conditional-access-security-defaults).

- Köpa Azure Active Directory Premium för varje användar konto. Mer information finns i [Planera en molnbaserad Azure Multi-Factor Authentication-distribution](/azure/active-directory/authentication/howto-mfa-getstarted).

- Använda en lösning från tredje part för att genomdriva Multi-Factor Authentication för varje användar konto i din partner klient. För att säkerställa att lösningen tillhandahåller den förväntade lösningen, se [Hur säkerhets kraven kommer att verkställas](#how-the-requirements-will-be-enforced).

> [!NOTE]
> Även om Multi-Factor Authentication inte enligt avtal krävs för ett suveränt moln (21Vianet, amerikanska myndigheter och Tyskland) är det mycket viktigt att du antar dessa säkerhets krav.

## <a name="security-defaults"></a>Standardinställningar för säkerhet

Säkerhets standard princip är ett av de [alternativ](#actions-that-you-need-to-take) som partners kan välja att implementera MFA för säkerhets kraven, beroende på deras affärs behov. Den erbjuder en grundläggande säkerhets nivå som är aktive rad utan extra kostnad. Läs om hur du aktiverar MFA för din organisation med Azure AD och viktiga överväganden nedan innan du aktiverar säkerhets inställningarna.

- Bas linje principerna kommer att stanna under de kommande månaderna och föråldrade mål i slutet av feb 2020.

- Partner som redan har infört bas linje principer måste vidta åtgärder för att gå över till säkerhets inställningarna.

- Säkerhets standarder är den allmänna tillgänglighets ersättningen för för hands versions bas linjerna. När en partner aktiverar säkerhets inställningarna kommer de inte längre att kunna aktivera bas linje principer.

- Med säkerhets inställningar aktive ras alla principer samtidigt.

- För partner som använder [villkorlig åtkomst](/azure/active-directory/conditional-access/concept-conditional-access-policy-common)är [säkerhets inställningar inte tillgängliga](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults#disabling-security-defaults).

- Det går inte att blockera äldre autentisering för partner för tillfället. Men eftersom de flesta händelser som rör komprometterade identiteter kommer från inloggnings försök med hjälp av äldre autentisering uppmuntras partner att gå vidare från dessa äldre protokoll.

- Azure AD Connect-synkroniseringsschemat är exkluderat från säkerhets inställningarna.

- Mer detaljerad information finns i [aktivera Multi-Factor Authentication för din organisation](/azure/active-directory/authentication/concept-mfa-get-started) och [Azure Active Directory säkerhets inställningar](/azure/active-directory/conditional-access/concept-conditional-access-security-defaults).

> [!NOTE]
> Standardvärden i Azure AD är utvecklingen av principer för grundläggande säkerhet. Om du redan har aktiverat principerna för bas linjen rekommenderas det starkt att du aktiverar säkerhets inställningarna.

Om du vill gå över från bas linje principerna till säkerhets inställningarna läser du [Vad är säkerhets inställningar?](/azure/active-directory/conditional-access/concept-conditional-access-security-defaults).

### <a name="consideration"></a>Att tänka på

Eftersom dessa krav gäller för alla användar konton i din partner klient måste du överväga flera saker för att säkerställa en smidig distribution, inklusive identifiera användar konton i Azure Active Directory som inte kan utföra Multi-Factor Authentication, samt program och enheter som används av din organisation som inte stöder modern autentisering.

Innan du utför någon åtgärd rekommenderar vi att du identifierar följande:

#### <a name="do-you-have-an-application-or-device-that-does-not-support-the-use-of-modern-authentication"></a>Har du ett program eller en enhet som inte stöder användning av modern autentisering?

När du upprätthåller Multi-Factor Authentication-autentisering använder du protokoll som IMAP, POP3, SMTP osv. kommer att blockeras eftersom de inte stöder Multi-Factor Authentication. För att åtgärda den här begränsningen kan en funktion som kallas [applösenord](/azure/active-directory/authentication/howto-mfa-mfasettings#app-passwords) användas för att säkerställa att programmet eller enheten fortfarande autentiseras. Du bör granska överväganden för att använda applösenord som dokumenteras [här](/azure/active-directory/authentication/howto-mfa-mfasettings#considerations-about-app-passwords) för att avgöra om de kan användas i din miljö.

#### <a name="do-you-have-users-using-office-365-provided-by-licenses-associated-with-your-partner-tenant"></a>Har du användare som använder Office 365 som tillhandahålls av licenser som är kopplade till din partner klient?

Innan du implementerar någon lösning rekommenderar vi att du fastställer vilken version av Microsoft Office som används av användare i din partner klient. Det finns en chans att användarna får problem med anslutningen till program som Outlook. Innan du framtvingar Multi-Factor Authentication är det viktigt att se till att Outlook 2013 SP1 eller senare används och att din organisation har modern autentisering aktive rad. Mer information finns i [Aktivera modern autentisering i Exchange Online](/exchange/clients-and-mobile-in-exchange-online/enable-or-disable-modern-authentication-in-exchange-online) .

Om du vill aktivera modern autentisering för alla enheter som kör Windows, som har Microsoft Office 2013 installerat, måste du skapa två register nycklar. Se [Aktivera modern autentisering för Office 2013 på Windows-enheter](/office365/admin/security-and-compliance/enable-modern-authentication).

#### <a name="is-there-a-policy-preventing-any-of-your-users-from-using-their-mobile-devices-while-working"></a>Finns det någon princip som hindrar användarna från att använda sina mobila enheter när de arbetar?

Det är viktigt att identifiera företags principer som förhindrar att anställda använder mobila enheter medan de arbetar eftersom det påverkar vilken Multi-Factor Authentication-lösning du implementerar. Det finns lösningar, till exempel den som tillhandahålls via implementeringen av [säkerhets inställningarna i Azure AD](/azure/active-directory/conditional-access/concept-conditional-access-security-defaults), som endast tillåter användning av en Authenticator-app för verifiering. Om din organisation har en princip som förhindrar användning av mobila enheter, bör du överväga något av följande alternativ:

- Distribuera ett tidsbaserat TOTP mobilapp-program (Base Password) som kan köras på ett säkert system

- Implementera en lösning från tredje part som upprätthåller Multi-Factor Authentication för varje användar konto i partner innehavaren som tillhandahåller det mest lämpliga verifierings alternativet

- Köp [Azure Active Directory Premium](https://azure.microsoft.com/pricing/details/active-directory/) licenser för berörda användare

#### <a name="what-automation-or-integration-do-you-have-to-leverage-user-credentials-for-authentication"></a>Vilken Automation eller integrering behöver du använda användarautentiseringsuppgifter för autentisering?

Eftersom kravet är att genomdriva MFA för varje användare, inklusive tjänst konton, i din partner katalog kommer all automatisering eller integrering som utnyttjar användarautentiseringsuppgifter för autentisering att påverkas. Det är därför viktigt att du identifierar vilka konton som används i dessa situationer. Se följande lista över exempel program eller tjänster som du bör tänka på:

- Kontroll panelen används för att etablera resurser för kundernas räkning

- Integrering med vilken plattform som helst som används för fakturering (som den är kopplad till CSP-programmet) och support för dina kunder

- PowerShell-skript som använder AZ, AzureRM, Azure AD, MS online osv.

Listan ovan är inte fullständig. Det är därför viktigt att du utför en fullständig utvärdering av alla program eller tjänster i din miljö som utnyttjar användarautentiseringsuppgifter för autentisering. För att tävla med kravet på Multi-Factor Authentication bör du implementera vägledningen i [ramverket för säker program modell](/partner-center/develop/enable-secure-app-model) där det är möjligt.

## <a name="accessing-your-environment"></a>Åtkomst till din miljö

Vi rekommenderar att du granskar inloggnings aktiviteten för att bättre förstå vad eller vem som autentiseras utan att behöva anropas för Multi-Factor Authentication. Med hjälp av Azure Active Directory Premium kan du utnyttja inloggnings rapporten. Mer information finns i [rapporter om inloggnings aktiviteter i Azure Active Directory portalen](/azure/active-directory/reports-monitoring/concept-sign-ins) . Om du inte har Azure Active Directory Premium, eller om du vill ha ett sätt att hämta detta via PowerShell, måste du använda cmdleten [Get-PartnerUserSignActivity](/powershell/module/partnercenter/get-partnerusersigninactivity)  från [partner centret PowerShell](https://www.powershellgallery.com/packages/PartnerCenter/) -modulen.

## <a name="how-the-requirements-will-be-enforced"></a>Hur kraven kommer att tillämpas

Säkerhets kraven för partnern kommer att verkställas av Azure Active Directory och i sin tur kan du söka efter MFA-anspråk för att identifiera att Multi-Factor Authentication-kontrollen har skett. Från och med 18 november 2019 kommer Microsoft att aktivera ytterligare säkerhets skydd (kallades tidigare "tekniskt tvång") till partner klienter. 

Vid aktivering begärs användare i partner klienten att slutföra autentisering med multifaktorautentisering (MFA) vid utförandet av en administratör på uppdrag av (ADMINISTRATE) åtgärder. Vi kommer att fortsätta att utöka omfattningen av säkerhets skyddet till ytterligare scenarier och användar roller, vilket ger partners i förväg meddelanden. Mer information finns i det här dokumentet, som kommer att uppdateras ofta. Partner som inte har uppfyllt kraven bör genomföra dessa åtgärder så snart som möjligt för att undvika eventuella affärs avbrott. 

Om du använder Azure Multi-Factor Authentication eller Azure AD Security-standardvärden finns det inga ytterligare åtgärder som du behöver vidta.

När du använder en Multi-Factor Authentication-lösning från tredje part, kan MFA-anspråk inte utfärdas. Om detta påstående saknas kan Azure Active Directory inte avgöra om autentiseringsbegäran har anropats av Multi-Factor Authentication. Information om hur du verifierar att lösningen utfärdar det förväntade anspråket finns [i testa säkerhets kraven för partner](/powershell/partnercenter/test-partner-security-requirements). 

> [!IMPORTANT]
> Om din lösning från tredje part inte utfärdar det förväntade anspråket måste du arbeta med leverantören som utvecklade lösningen för att fastställa vilka åtgärder som ska vidtas.

## <a name="resources-and-support"></a>Resurser och support

Se följande resurser för support och exempel kod:

- [Community för säkerhets guide för partner Center](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance): communityn för säkerhets vägledning för partner Center är en online-community där du kan lära dig om kommande händelser och ställa frågor som du kan ha.
- [Partner Center .net-exempel](https://github.com/microsoft/partner-center-dotnet-samples): den här GitHub-lagringsplatsen innehåller exempel som har utvecklats med .net, som visar hur du kan implementera säkra program modell ramverk.
- [Partner Center Java-exempel](https://github.com/microsoft/partner-center-java-samples): den här GitHub-lagringsplatsen innehåller exempel som har utvecklats med Java, som visar hur du kan implementera säkra program modell ramverk.
- [Partner Center PowerShell – Multi-Factor Authentication](/powershell/partnercenter/multi-factor-auth): den här Multi-Factor Authentication artikeln innehåller information om hur du implementerar den säkra program modell ramverket med PowerShell.