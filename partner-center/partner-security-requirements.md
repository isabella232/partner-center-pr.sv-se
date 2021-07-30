---
title: Säkerhetskrav för partner
ms.topic: article
ms.date: 10/30/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-enroll
description: Introducerar partnersäkerhetskrav för att aktivera multifaktorautentisering (MFA) och införa Modell för säkra program ramverket.
author: vijvala
ms.author: vijvala
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 73d508b8a8dabacaf65037c905fd31929a0f2522
ms.sourcegitcommit: ad1af627f5ee6b6e3a70655f90927e932cf4c985
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 07/29/2021
ms.locfileid: "114837347"
---
# <a name="security-requirements-for-using-partner-center-or-partner-center-apis"></a>Säkerhetskrav för att använda PARTNER Center- eller Partner Center-API:er

**Lämpliga roller:** Alla Partner Center-användare

Den här artikeln förklarar de obligatoriska säkerhetskraven för rådgivare, Kontrollpanelen-leverantörer och partner som deltar i Molnlösningsleverantör-programmet, samt autentiseringsalternativ och andra säkerhetsöverväganden. Sekretessskydd och säkerhet är bland våra högsta prioriteter. Vi vet att det bästa skydd är att förebygga och att vi bara är lika starka som vår svagaste länk. Därför behöver vi att alla i vårt ekosystem agerar och ser till att rätt säkerhetsskydd finns på plats.

## <a name="mandatory-security-requirements"></a>Obligatoriska säkerhetskrav

Partner som inte implementerar de obligatoriska säkerhetskraven kommer inte att kunna genomföra transaktioner i Molnlösningsleverantör-programmet eller hantera kundklienter med delegerade administratörsrättigheter. Dessutom kan partner som inte implementerar säkerhetskraven riskera deras deltagande i program. De termer som är associerade med partnersäkerhetskraven har lagts till i Microsoft-partneravtal. När det gäller rådgivare gäller samma avtalskrav.

För att skydda dig och dina kunder kräver vi att partner omedelbart vidta följande åtgärder:  

1. **Aktivera multifaktorautentisering (MFA) för alla användarkonton i din partnerklientorganisation.** Du måste tillämpa MFA på alla användarkonton i dina partnerklienter. Användare måste uppmanas av MFA när de loggar in på Microsofts kommersiella molntjänster eller när de gör en överträdelse i Molnlösningsleverantör-programmet via Partnercenter eller via API:er.

2. **Anta Modell för säkra program ramverket**. Alla partner som integrerar med Partner Center-API:er [måste Modell för säkra program ramverket](/partner-center/develop/enable-secure-app-model) för alla program för app- och användarauth-modeller.

    > [!IMPORTANT]
    > Vi rekommenderar starkt att partner implementerar Modell för säkra program för integrering med ett Microsoft API, till exempel Azure Resource Manager eller Microsoft Graph, eller när du använder automatisering som PowerShell med hjälp av användarautentiseringsuppgifter för att undvika eventuella avbrott när MFA tillämpas.

Dessa säkerhetskrav hjälper till att skydda din infrastruktur och dina kunders data mot potentiella säkerhetsrisker, till exempel stöld eller andra bedrägeriincidenter.  

## <a name="implementing-multi-factor-authentication"></a>Implementera multifaktorautentisering

För att uppfylla partnersäkerhetskraven måste du implementera och framtvinga MFA för varje användarkonto i din partnerklientorganisation. Du kan göra detta på något av följande sätt:

- Implementera [Azure Active Directory (Azure AD)-säkerhet som standard.](/azure/active-directory/conditional-access/concept-conditional-access-security-defaults) Mer information finns i [nästa avsnitt.](#security-defaults)

- Köp Azure Active Directory Premium för varje användarkonto. Mer information finns i Planera [en Azure AD Multi-Factor Authentication-distribution.](/azure/active-directory/authentication/howto-mfa-getstarted)

- Använd en lösning från tredje part för att tillämpa MFA för varje användarkonto i din partnerklientorganisation. För att säkerställa att lösningen ger den förväntade lösningen kan [du se hur säkerhetskraven kommer att tillämpas.](#how-the-requirements-are-enforced)

> [!NOTE]
> Även om multifaktorautentisering inte krävs i avtal för ett suveränt moln (amerikanska myndigheter och Tyskland) rekommenderar vi starkt att du inför dessa säkerhetskrav.

### <a name="security-defaults"></a>Standardinställningar för säkerhet

Ett av alternativen som partner kan välja för att implementera MFA-krav är att aktivera standardinställningar för säkerhet i Azure AD. Standardinställningarna för säkerhet ger en grundläggande säkerhetsnivå utan extra kostnad. Läs om hur du aktiverar MFA för din organisation med Azure AD och de viktigaste övervägandena nedan innan du aktiverar standardinställningar för säkerhet.

- Partner som redan har infört baslinjeprinciper måste vidta åtgärder för att övergå till standardvärden för säkerhet.

- Standardinställningarna för säkerhet är allmän tillgänglighetsersättning av baslinjeprinciperna för förhandsversionen. När en partner aktiverar standardinställningarna för säkerhet kommer de inte längre att kunna aktivera baslinjeprinciper.

- Med standardinställningarna för säkerhet aktiveras alla principer samtidigt.

- För partner som använder [villkorlig åtkomst](/azure/active-directory/conditional-access/concept-conditional-access-policy-common) [är standardinställningarna för säkerhet inte tillgängliga.](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults#disabling-security-defaults)

- Vi blockerar inte äldre autentisering just nu. Men eftersom de flesta händelser som rör komprometterade identiteter kommer från inloggningsförsök med äldre autentisering, uppmuntras partner att flytta från dessa äldre protokoll.

- Azure AD Anslut synkroniseringskonto undantas från standardinställningarna för säkerhet.

Detaljerad information finns i [Översikt över Azure AD Multi-Factor Authentication för din organisation](/azure/active-directory/authentication/concept-mfa-get-started) och Vad är [standardinställningar för säkerhet?](/azure/active-directory/conditional-access/concept-conditional-access-security-defaults).

> [!NOTE]
> Standardvärden för Azure AD-säkerhet är utvecklingen av förenklade baslinjeskyddsprinciper. Om du redan har aktiverat baslinjeskyddsprinciperna rekommenderar vi starkt att du aktiverar [standardinställningarna för säkerhet.](/azure/active-directory/conditional-access/concept-conditional-access-security-defaults)

## <a name="implementation-considerations"></a>Att tänka på vid implementering

Eftersom dessa krav gäller för alla användarkonton i partnerklientorganisationen måste du tänka på flera saker för att säkerställa en smidig distribution. Du kan till exempel identifiera användarkonton i Azure AD som inte kan utföra MFA och program och enheter i din organisation som inte stöder modern autentisering.

Innan du utför någon åtgärd rekommenderar vi att du slutför följande verifieringar. 

#### <a name="do-you-have-an-application-or-device-that-does-not-support-the-use-of-modern-authentication"></a>Har du ett program eller en enhet som inte stöder användning av modern autentisering?

När du tillämpar MFA blockeras äldre autentiseringsprotokoll som IMAP, POP3, SMTP och andra eftersom de inte stöder MFA. Du kan åtgärda den här begränsningen [genom att använda funktionen för applösenord](/azure/active-directory/authentication/howto-mfa-mfasettings#app-passwords) för att säkerställa att programmet eller enheten fortfarande autentiseras. Granska [övervägandena för att använda applösenord](/azure/active-directory/authentication/howto-mfa-mfasettings#considerations-about-app-passwords) för att avgöra om de kan användas i din miljö.

#### <a name="do-you-have-office-365-users-with-licenses-associated-with-your-partner-tenant"></a>Har du Office 365 licenser som är associerade med din partnerklientorganisation?

Innan du implementerar en lösning rekommenderar vi att du bestämmer vilka versioner Microsoft Office användare i din partnerklientorganisation använder. Det finns en risk att användarna får anslutningsproblem med program som Outlook. Innan du framtvingar MFA är det viktigt att du använder Outlook 2013 SP1 eller senare och att din organisation har modern autentisering aktiverad. Mer information finns i [Aktivera modern autentisering i Exchange Online](/exchange/clients-and-mobile-in-exchange-online/enable-or-disable-modern-authentication-in-exchange-online). 

Om du vill aktivera modern autentisering för enheter Windows som Microsoft Office 2013 installerade måste du skapa två registernycklar. Se [Aktivera modern autentisering för Office 2013 på Windows enheter.](/office365/admin/security-and-compliance/enable-modern-authentication)

#### <a name="is-there-a-policy-preventing-any-of-your-users-from-using-their-mobile-devices-while-working"></a>Finns det en princip som förhindrar att någon av användarna använder sina mobila enheter när de arbetar?

Det är viktigt att identifiera alla företagspolicyer som förhindrar anställda från att använda mobila enheter när de arbetar, eftersom det påverkar vilken MFA-lösning du implementerar. Det finns lösningar, till exempel den som tillhandahålls via implementeringen av Standardinställningar för Azure AD-säkerhet, som endast tillåter användning av en [autentiseringsapp](/azure/active-directory/conditional-access/concept-conditional-access-security-defaults)för verifiering. Om din organisation har en princip som förhindrar användning av mobila enheter kan du överväga något av följande alternativ:

- Distribuera ett tidsbaserat TOTP-program (engångsbaslösenord) som kan köras på ett säkert system.

- Implementera en lösning från tredje part som tillämpar MFA för varje användarkonto i partnerklientorganisationen som ger det lämpligaste verifieringsalternativet.

- Köp [Azure Active Directory Premium](https://azure.microsoft.com/pricing/details/active-directory/) licenser för de berörda användarna.

#### <a name="what-automation-or-integration-do-you-have-to-leverage-user-credentials-for-authentication"></a>Vilken automatisering eller integrering behöver du för att utnyttja användarautentiseringsuppgifter för autentisering?

Eftersom vi tillämpar MFA för varje användare, inklusive tjänstkonton, i partnerkatalogen påverkar detta all automatisering eller integrering som använder autentiseringsuppgifter för autentisering. Det är därför viktigt att du identifierar vilka konton som används i dessa situationer. Se följande lista över exempelprogram eller tjänster att tänka på:

- Kontrollpanelen som används för att etablera resurser åt dina kunder

- Integrering med alla plattformar som används för fakturering (i enlighet med CSP-programmet) och stöd för dina kunder

- PowerShell-skript som använder Az, AzureRM, Azure AD, MS Online och andra moduler

Listan ovan är inte omfattande. Därför är det viktigt att du utför en fullständig utvärdering av alla program eller tjänster i din miljö som använder användarautentiseringsuppgifter för autentisering. För att uppfylla kravet på MFA bör du implementera vägledningen i det Modell för säkra program [ramverket](/partner-center/develop/enable-secure-app-model) där det är möjligt.

## <a name="accessing-your-environment"></a>Åtkomst till din miljö

För att bättre förstå vad eller vem som autentiserar utan att behöva använda MFA rekommenderar vi att du granskar inloggningsaktiviteten. Via Azure Active Directory Premium kan du använda inloggningsrapporten. Mer information om det här ämnet finns i [Inloggningsaktivitetsrapporter i Azure Active Directory portalen.](/azure/active-directory/reports-monitoring/concept-sign-ins) Om du inte har Azure Active Directory Premium, eller om du letar efter ett sätt att hämta den här inloggningsaktiviteten via PowerShell, måste du använda cmdleten [Get-PartnerUserSignActivity](/powershell/module/partnercenter/get-partnerusersigninactivity) från [Partner Center PowerShell-modulen.](https://www.powershellgallery.com/packages/PartnerCenter/)

## <a name="how-the-requirements-are-enforced"></a>Hur kraven tillämpas

Partnersäkerhetskraven tillämpas av Azure AD, och i sin tur Partnercenter, genom att söka efter förekomsten av MFA-anspråket för att identifiera att MFA-verifiering har skett. Från och med den 18 november 2019 aktiverade Microsoft ytterligare säkerhetsskydd (tidigare kallat "tekniskt framtvingande") för partnerklienter.

Vid aktiveringen uppmanas användare i partnerklientorganisationen att slutföra MFA-verifieringen när de utför en administratör för (AOBO)-åtgärder, kommer åt Partner Center-portalen eller anropar Partner Center-API:er. Mer information finns i [Flerfaktorautentisering (MFA) för din partnerklientorganisation.](partner-security-requirements-mandating-mfa.md) 

Partner som inte har uppfyllt kraven bör implementera dessa åtgärder så snart som möjligt för att undvika eventuella verksamhetsavbrott. Om du använder Azure Active Directory multifaktorautentisering eller Standardinställningar för Azure AD-säkerhet behöver du inte utföra några ytterligare åtgärder.

Om du använder en MFA-lösning från tredje part finns det en risk att MFA-anspråket inte utfärdas. Om det här anspråket saknas kan Azure AD inte avgöra om autentiseringsbegäran har begärts av MFA. Information om hur du verifierar din lösning som utfärdar det förväntade anspråket finns [i Testa partnersäkerhetskraven.](/powershell/partnercenter/test-partner-security-requirements) 

> [!IMPORTANT]
> Om din lösning från tredje part inte utfärdar det förväntade anspråket måste du kontakta leverantören som utvecklade lösningen för att avgöra vilka åtgärder som ska vidtas.

## <a name="resources-and-samples"></a>Resurser och exempel

Se följande resurser för support och exempelkod:

- [Communityn för säkerhetsvägledning i Partnercenter:](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance)Communityn för säkerhetsvägledning i Partnercenter är en online-community där du kan lära dig mer om kommande händelser och ställa frågor som du kan ha.
- [Partner Center .NET-exempel:](https://github.com/microsoft/partner-center-dotnet-samples)Den GitHub lagringsplatsen innehåller exempel som utvecklats med .NET och som visar hur du kan implementera Modell för säkra program ramverket.
- [Partner Center Java-exempel:](https://github.com/microsoft/partner-center-java-samples)Den GitHub lagringsplatsen innehåller exempel, utvecklade med Java, som visar hur du kan implementera Modell för säkra program ramverket.
- [Partner Center PowerShell – Multifaktorautentisering:](/powershell/partnercenter/multi-factor-auth)Den här artikeln om multifaktorautentisering innehåller information om hur du implementerar Modell för säkra program ramverket med PowerShell.

## <a name="next-steps"></a>Nästa steg

- [Använda multifaktorautentisering (MFA) för din partnerklientorganisation](partner-security-requirements-mandating-mfa.md)