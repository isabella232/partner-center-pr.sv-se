---
title: Säkerhets krav för partner
ms.topic: article
ms.date: 10/30/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Introducerar säkerhets krav för partner för att aktivera Multi-Factor Authentication (MFA) och anta ramverket för säker program modell.
author: vijvala
ms.author: vijvala
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 351d0715645b6e43607279393cdc376d898a7f54
ms.sourcegitcommit: 98f5eebe7d08ba214ed5a078f1ac770439e41eb7
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 10/31/2020
ms.locfileid: "93133002"
---
# <a name="security-requirements-for-using-partner-center-or-partner-center-apis"></a>Säkerhets krav för att använda API: er för partner Center eller partner Center

**Gäller för**

- Alla partner i Cloud Solution Provider-programmet
- Alla leverantörer på kontroll panelen
- Alla rådgivare

**Lämpliga användare**

- Alla aktiverade användare, inklusive gäst användare

Den här artikeln beskriver de obligatoriska säkerhets kraven för rådgivare, kontroll panels leverantörer och partner som ingår i Cloud Solution Provider-programmet, samt autentiseringsalternativ och andra säkerhets aspekter. Integritets skydd och säkerhet är bland våra främsta prioriteringar. Vi vet att det bästa skyddet är förebyggande och att vi bara är lika starka som vår svagaste länk. Därför behöver vi alla i vårt eko system för att agera och se till att lämpliga säkerhets skydd är på plats.

## <a name="mandatory-security-requirements"></a>Obligatoriska säkerhets krav

Partner som inte implementerar de obligatoriska säkerhets kraven kommer inte att kunna använda Transact i Cloud Solution Provider-programmet eller hantera kund klienter som utnyttjar delegerade administratörs rättigheter. Dessutom kan partner som inte implementerar säkerhets kraven ge sitt deltagande i program i risk zonen. Villkoren som är kopplade till partner säkerhets kraven har lagts till i Microsoft partner Agreement. När det gäller rådgivare är samma avtals krav på plats.

För att skydda dig och dina kunder, kräver vi partner att vidta följande åtgärder omedelbart:  

1. **Aktivera Multi-Factor Authentication (MFA) för alla användar konton i din partner klient** . Du måste tillämpa MFA på alla användar konton i din partner klient (er). Användarna måste ha en utmaning när de loggar in på Microsofts kommersiella moln tjänster eller när de använder sig av Transact i Cloud Solution Provider-programmet via partner Center eller via API: er.

2. **Anta ramverket för säker program modell** . Alla partners som integreras med API: er för partner Center måste anta modell program för [säker program modell](/partner-center/develop/enable-secure-app-model) för appar och program för användarautentisering.

    > [!IMPORTANT]
    > Vi rekommenderar starkt att partners implementerar den säkra program modellen för integrering med ett Microsoft API, till exempel Azure Resource Manager eller Microsoft Graph eller när du använder automatisering, till exempel PowerShell med hjälp av användarautentiseringsuppgifter, för att undvika störningar när MFA tillämpas.

Dessa säkerhets krav hjälper till att skydda din infrastruktur och skydda dina kunders data från potentiella säkerhets risker, till exempel att identifiera stölder eller andra bedrägeri incidenter.  

## <a name="implementing-multi-factor-authentication"></a>Implementera Multi-Factor Authentication

För att uppfylla partner säkerhets kraven måste du implementera och verkställa MFA för varje användar konto i din partner klient. Det kan du göra på något av följande sätt:

- Implementera [säkerhets inställningar för Azure Active Directory (Azure AD)](/azure/active-directory/conditional-access/concept-conditional-access-security-defaults). Mer information finns i [Nästa avsnitt](#security-defaults).

- Köp Azure Active Directory Premium för varje användar konto. Mer information finns i [Planera en Azure Multi-Factor Authentication-distribution](/azure/active-directory/authentication/howto-mfa-getstarted).

- Använd en lösning från tredje part för att genomdriva MFA för varje användar konto i din partner klient. För att säkerställa att lösningen tillhandahåller den förväntade lösningen, se [Hur säkerhets kraven kommer att verkställas](#how-the-requirements-are-enforced).

> [!NOTE]
> Även om Multi-Factor Authentication inte enligt avtal krävs för ett suveränt moln (amerikanska myndigheter och Tyskland) rekommenderar vi att du antar dessa säkerhets krav.

### <a name="security-defaults"></a>Standardinställningar för säkerhet

Ett av de alternativ som partner kan välja för att implementera MFA-krav är att aktivera säkerhets inställningar i Azure AD. Säkerhets standarder erbjuder en grundläggande säkerhets nivå utan extra kostnad. Läs om hur du aktiverar MFA för din organisation med Azure AD och viktiga överväganden nedan innan du aktiverar säkerhets inställningarna.

- Partner som redan har infört bas linje principer måste vidta åtgärder för att gå över till säkerhets inställningarna.

- Säkerhets standarder är den allmänna tillgänglighets ersättningen för för hands versions bas linjerna. När en partner aktiverar säkerhets inställningarna kommer de inte längre att kunna aktivera bas linje principer.

- Med säkerhets inställningar aktive ras alla principer samtidigt.

- För partner som använder [villkorlig åtkomst](/azure/active-directory/conditional-access/concept-conditional-access-policy-common)är [säkerhets inställningar inte tillgängliga](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults#disabling-security-defaults).

- Vi blockerar inte äldre autentisering för tillfället. Men eftersom de flesta händelser som rör komprometterade identiteter kommer från inloggnings försök med hjälp av äldre autentisering uppmuntras partner att gå vidare från dessa äldre protokoll.

- Azure AD Connect-synkroniseringsschemat är exkluderat från säkerhets inställningarna.

Mer detaljerad information finns [i Översikt över Azure Multi-Factor Authentication för din organisation](/azure/active-directory/authentication/concept-mfa-get-started) och [Vad är säkerhets inställningar?](/azure/active-directory/conditional-access/concept-conditional-access-security-defaults).

> [!NOTE]
> Standardvärden i Azure AD är utvecklingen av principer för grundläggande säkerhet. Om du redan har aktiverat principerna för bas linjen rekommenderas det starkt att du aktiverar [säkerhets inställningarna](/azure/active-directory/conditional-access/concept-conditional-access-security-defaults).

## <a name="implementation-considerations"></a>Att tänka på vid implementering

Eftersom dessa krav gäller för alla användar konton i din partner klient måste du överväga flera saker för att säkerställa en smidig distribution. Identifiera till exempel användar konton i Azure AD som inte kan utföra MFA, samt program och enheter i din organisation som inte stöder modern autentisering.

Innan du utför någon åtgärd rekommenderar vi att du utför följande verifieringar. 

#### <a name="do-you-have-an-application-or-device-that-does-not-support-the-use-of-modern-authentication"></a>Har du ett program eller en enhet som inte stöder användning av modern autentisering?

När du tillämpar MFA, använder äldre autentisering-protokoll som IMAP, POP3, SMTP osv. blockeras eftersom de inte stöder MFA. Om du vill åtgärda den här begränsningen använder du [appens lösen ord](/azure/active-directory/authentication/howto-mfa-mfasettings#app-passwords) för att se till att programmet eller enheten fortfarande kommer att autentiseras. Granska [överväganden för att använda applösenord](/azure/active-directory/authentication/howto-mfa-mfasettings#considerations-about-app-passwords) för att avgöra om de kan användas i din miljö.

#### <a name="do-you-have-office-365-users-with-licenses-associated-with-your-partner-tenant"></a>Har du Office 365-användare med licenser som är kopplade till din partner klient?

Innan du implementerar någon lösning rekommenderar vi att du fastställer vilken version av Microsoft Office användare i din partner klient organisation använder. Det finns en chans att användarna får problem med anslutningen till program som Outlook. Innan du framtvingar MFA är det viktigt att se till att du använder Outlook 2013 SP1 eller senare och att din organisation har modern autentisering aktive rad. Mer information finns i [Aktivera modern autentisering i Exchange Online](/exchange/clients-and-mobile-in-exchange-online/enable-or-disable-modern-authentication-in-exchange-online). 

Om du vill aktivera modern autentisering för enheter som kör Windows som har Microsoft Office 2013 installerat måste du skapa två register nycklar. Se [Aktivera modern autentisering för Office 2013 på Windows-enheter](/office365/admin/security-and-compliance/enable-modern-authentication).

#### <a name="is-there-a-policy-preventing-any-of-your-users-from-using-their-mobile-devices-while-working"></a>Finns det någon princip som hindrar användarna från att använda sina mobila enheter när de arbetar?

Det är viktigt att identifiera företags principer som hindrar anställda från att använda mobila enheter medan de arbetar eftersom det påverkar vilken MFA-lösning du implementerar. Det finns lösningar, till exempel den som tillhandahålls via implementeringen av [säkerhets inställningarna i Azure AD](/azure/active-directory/conditional-access/concept-conditional-access-security-defaults), som endast tillåter användning av en Authenticator-app för verifiering. Om din organisation har en princip som förhindrar användning av mobila enheter, bör du överväga något av följande alternativ:

- Distribuera ett tidsbaserat TOTP mobilapp-program (Base Password) som kan köras på ett säkert system.

- Implementera en lösning från tredje part som tillämpar MFA för varje användar konto i partner klienten som tillhandahåller det mest lämpliga verifierings alternativet.

- Köp [Azure Active Directory Premium](https://azure.microsoft.com/pricing/details/active-directory/) licenser för de påverkade användarna.

#### <a name="what-automation-or-integration-do-you-have-to-leverage-user-credentials-for-authentication"></a>Vilken Automation eller integrering behöver du använda användarautentiseringsuppgifter för autentisering?

Eftersom vi tillämpar MFA för varje användare, inklusive tjänst konton, i din partner katalog, kommer detta att påverka all automatisering eller integrering som utnyttjar användarautentiseringsuppgifter för autentisering. Det är därför viktigt att du identifierar vilka konton som används i dessa situationer. Se följande lista över exempel program eller tjänster som du bör tänka på:

- Kontroll panelen används för att etablera resurser för kundernas räkning

- Integrering med vilken plattform som helst som används för fakturering (som den är kopplad till CSP-programmet) och support för dina kunder

- PowerShell-skript som använder AZ, AzureRM, Azure AD, MS online osv.

Listan ovan är inte fullständig. Det är därför viktigt att du utför en fullständig utvärdering av alla program eller tjänster i din miljö som utnyttjar användarautentiseringsuppgifter för autentisering. Om du vill tävla med kravet för MFA bör du implementera rikt linjerna i [säkra program modell ramverk](/partner-center/develop/enable-secure-app-model) där det är möjligt.

## <a name="accessing-your-environment"></a>Åtkomst till din miljö

För att bättre förstå vad eller vem som autentiseras utan att bli tillfrågad för MFA, rekommenderar vi att du granskar inloggnings aktiviteten. Med hjälp av Azure Active Directory Premium kan du utnyttja inloggnings rapporten. Mer information om det här ämnet finns i [rapporter om inloggnings aktiviteter i Azure Active Directory-portalen](/azure/active-directory/reports-monitoring/concept-sign-ins). Om du inte har Azure Active Directory Premium, eller om du letar efter ett sätt att hämta denna inloggnings aktivitet via PowerShell, måste du använda cmdleten [Get-PartnerUserSignActivity](/powershell/module/partnercenter/get-partnerusersigninactivity) från [partner centret PowerShell](https://www.powershellgallery.com/packages/PartnerCenter/) -modulen.

## <a name="how-the-requirements-are-enforced"></a>Så här framtvingas kraven

Partner säkerhets krav upprätthålls av Azure AD och i sin tur i sin tur kan du söka efter MFA-anspråk för att identifiera att MFA-kontrollen har ägt rum. Från och med 18 november 2019 har Microsoft aktiverat ytterligare säkerhets skydd (kallades tidigare "tekniskt tvång") till partner klienter.

Vid aktivering begärs användare i partner innehavaren att slutföra MFA-verifiering när de utför en administratör på uppdrag av (ADMINISTRATE) åtgärder, åtkomst till Partner Center-portalen eller anropar API: er för partner Center. Mer information finns i [kräva Multi-Factor Authentication (MFA) för din partner klient](partner-security-requirements-mandating-mfa.md). 

Partner som inte har uppfyllt kraven bör genomföra dessa åtgärder så snart som möjligt för att undvika eventuella affärs avbrott. Om du använder Azure Multi-Factor Authentication eller Azure AD Security-standardvärden finns det inga ytterligare åtgärder som du behöver vidta.

Om du använder en MFA-lösning från tredje part, kan MFA-anspråk inte utfärdas. Om detta påstående saknas, kan inte Azure AD avgöra om autentiseringsbegäran har anropats av MFA. Information om hur du verifierar att lösningen utfärdar det förväntade anspråket finns [i testa säkerhets kraven för partner](/powershell/partnercenter/test-partner-security-requirements). 

> [!IMPORTANT]
> Om din lösning från tredje part inte utfärdar det förväntade anspråket måste du arbeta med leverantören som utvecklade lösningen för att fastställa vilka åtgärder som ska vidtas.

## <a name="resources-and-samples"></a>Resurser och exempel

Se följande resurser för support och exempel kod:

- [Community för säkerhets guide för partner Center](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance): communityn för säkerhets vägledning för partner Center är en online-community där du kan lära dig om kommande händelser och ställa frågor som du kan ha.
- [Partner Center .net-exempel](https://github.com/microsoft/partner-center-dotnet-samples): den här GitHub-lagringsplatsen innehåller exempel som har utvecklats med .net, som visar hur du kan implementera säkra program modell ramverk.
- [Partner Center Java-exempel](https://github.com/microsoft/partner-center-java-samples): den här GitHub-lagringsplatsen innehåller exempel som har utvecklats med Java, som visar hur du kan implementera säkra program modell ramverk.
- [Partner Center PowerShell – Multi-Factor Authentication](/powershell/partnercenter/multi-factor-auth): den här Multi-Factor Authentication artikeln innehåller information om hur du implementerar den säkra program modell ramverket med PowerShell.

## <a name="next-steps"></a>Nästa steg

- [Kräva Multi-Factor Authentication (MFA) för din partner klient](partner-security-requirements-mandating-mfa.md)