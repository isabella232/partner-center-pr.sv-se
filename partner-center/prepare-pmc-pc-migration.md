---
title: Flytta från Partner Membership Center
ms.topic: article
ms.date: 06/01/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Granska användbar information och vanliga frågor innan du flyttar din verksamhet från Partner Membership Center till Partnercenter.
author: parthpandyamsft
ms.author: parthp
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 7f533240d5236f03fe277d4c6dfa02ed1c58b63c
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 05/13/2021
ms.locfileid: "109855020"
---
# <a name="prepare-for-your-move-from-partner-membership-center-pmc-to-partner-center"></a>Förbered för flytten från Partner Membership Center (PMC) till Partnercenter

**Lämpliga roller:** Globala | Administratörsbehörighet för | Försäljningsagent | Administratörsagent

Vi flyttar medlemskapshanteringen från Partner Membership Center (PMC) till Partnercenter – det enda målet för att hantera din affärsrelation med Microsoft. Vi vill att din flytt till Partnercenter ska vara så effektiv och enkel som möjligt. Vi har identifierat några områden där Partnercenter skiljer sig från PMC och vi tror att du bör förstå och förbereda dig för dem innan du flyttar.

## <a name="account-and-identity-setup"></a>Konto- och identitetskonfiguration

Nedan finns svar på vanliga frågor om konto- och identitetskonfiguration.

### <a name="what-is-an-azure-active-directory-azure-ad-work-account"></a>Vad är ett Azure Active Directory(Azure AD)-arbetskonto?

Ett Azure-arbetskonto är en dedikerad och isolerad virtuell representation av ditt företag i det offentliga Azure-molnet, som skapas åt dig när du prenumererar på en Microsoft-molntjänst som Azure, Microsoft Intune eller Office 365.

Ditt arbetskonto är värd för dina Azure AD-användare och informationen om dem – deras e-post, lösenord, profildata, behörigheter och så vidare. Arbetskontot innehåller också grupper, program och annan information som rör ett företag och dess säkerhet. 

Din e-postadress till arbetet är en del av din Azure Active Directory-klientorganisation. Om du vill ha ett konto i Partnercenter måste du ha en AAD-klientorganisation. Mer information om hur Azure Active Directory finns i [Skapa din katalog i Azure AD.](/azure/active-directory/fundamentals/add-custom-domain#create-your-directory-in-azure-ad)

I Partnercenter använder du din e-postadress för arbetet för att logga in på ditt konto, inte din personliga e-postadress.

- Ditt arbetskonto: john@contoso.com
- Ditt personliga konto: John@outlook.com

### <a name="what-account-should-you-sign-into-partner-center-with-if-you-have-an-aad-tenant-with-microsoft-for-office-365-for-example-and-you-also-have-a-tenant-for-your-csp-business"></a>Vilket konto ska du logga in på Partnercenter med om du har en AAD-klientorganisation med Microsoft (till exempel för Office 365) och du också har en klientorganisation för din CSP-verksamhet?

Du kan logga in på Partnercenter med Antingen CSP-kontot eller ditt MPN-arbets-e-postkonto. Om du väljer att logga in med CSP-arbetsmeddelandet visas information om både MPN- och CSP-program i det vänstra navigeringsfönstret på instrumentpanelen. Om du loggar in med din e-postadress för MPN Azure AD-klientorganisationens arbete visas endast din MPN-programinformation. 

### <a name="if-you-dont-want-to-use-your-existing-office-365-azure-ad-tenant-for-partner-center-you-can-create-a-new-tenant-prior-to-migrating-from-pmc"></a>Om du inte vill använda din befintliga Office 365 Azure AD-klient för Partnercenter kan du skapa en ny klient innan du migrerar från PMC.

Det kan finnas många orsaker till att du inte vill använda en befintlig Azure AD-klient för att konfigurera ditt Partnercenter-konto. Innan du börjar migrera till Partnercenter går du till Azure Portal för [att](https://ms.portal.azure.com/#home) skapa en ny Azure AD-klientorganisation. Följ riktlinjerna i Skapa [en ny klientorganisation i Azure Active Directory](/azure/active-directory/develop/quickstart-create-new-tenant). Använd den nya AAD-klienten för att konfigurera ditt Partnercenter-konto. Du måste vara global administratör för att skapa klientorganisationen. 

### <a name="user-roles-including-guest-user-roles-in-partner-center"></a>Användarroller, inklusive gästanvändarroller i Partnercenter

Partnercenter har olika typer av roller beroende på vilka typer av arbete som krävs. Det finns roller som global administratör som är Azure AD-roller. Vissa av rollerna är specifika för program som t.ex. molntjänstleverantörens program eller incitament, och det finns roller som är specifika för MPN. Om du vill ta reda på vad alla Partner Center-roller är kan du [läsa Tilldela användarroller och behörigheter](permissions-overview.md).

### <a name="what-happens-to-my-users-roles-when-they-move-from-pmc-to-partner-center"></a>Vad händer med mina användares roller när de flyttar från PMC till Partnercenter?

Förutom den globala MPN-administratör eller primära programkontakt som genomför migreringen förlorar alla användare i PMC sina administratörsroller. Den person som slutför migreringen måste tilldela roller i Partnercenter. Rollerna i Partnercenter skiljer sig från rollerna i PMC. Läs [Tilldela användarroller och behörigheter](permissions-overview.md och Flytta från PMC till [Partnercenter](move-pmc-pc-map.md#user-roles) för mer information om användarroller i Partnercenter.

### <a name="whats-the-difference-between-my-company-profile-and-my-business-profile"></a>Vad är skillnaden mellan min företagsprofil och min företagsprofil?

Din företagsprofil är information om ditt företag som innehåller adress, platser, primär kontakt, bank och skatteinformation.

Din företagsprofil visar dig själv för kunderna och är en marknadsföringssida som visar din logotyp, information om ditt affärsfokus, dina kunskaper osv.

### <a name="what-does-account-consolidation-mean-for-my-account"></a>Vad innebär kontokonsolidering för mitt konto?

Om du använder samma Azure AD-klientorganisation för att migrera flera MPN-konton till Partnercenter kommer systemet automatiskt att identifiera det och be dig konsolidera dina konton. Detta gäller även om du har flera domäner som är kopplade till samma Azure AD-klientorganisation. 

Du kan fortfarande välja att migrera till Partnercenter med separata AAD-klienter, men observera att detta resulterar i en isolerad utvärdering av dina kompetenser och extra inköpskostnader. Mer information om kontokonsolidering finns i [Konsolidera företagskonton](consolidate-accounts.md)

### <a name="if-i-have-multiple-aad-tenants-and-a-single-mpn-account-is-it-possible-to-link-them-in-partner-center"></a>Om jag har flera AAD-klienter och ett enda MPN-konto, går det att länka dem i Partnercenter?

Ja, i Partnercenter kan du länka flera Azure AD-klienter till ett enda Partnercenter-konto.
Mer information om kontokonsolidering finns i [Konsolidera företagskonton](consolidate-accounts.md)

### <a name="are-there-restrictions-to-adding-multiple-azure-ad-tenants-to-a-single-partner-center-account"></a>Finns det begränsningar för att lägga till flera Azure AD-klienter till ett enda Partnercenter-konto?

Om Azure AD-klienten redan är associerad med ett befintligt Partnercenter-konto kan den inte associeras till nya Partnercenter-konton med funktionen för flera innehavare. Ett annat sätt att tänka på det är att en Azure AD-klientorganisation bara kan associeras till ett Partnercenter-konto, men ett Partnercenter-konto kan ha flera klientorganisationsklienter kopplade till sig.

## <a name="microsoft-partner-network-mpn-membership-migration"></a>Microsoft Partner Network (MPN) medlemskapsmigrering 

Se följande svar på vanliga frågor om migrering av MPN-medlemskap.

### <a name="who-can-perform-the-move-from-pmc-to-partner-center"></a>Vem kan utföra flytten från PMC till Partnercenter?

Ditt företags globala MPN-administratör eller den primära programkontakten (dessa två roller innehas ofta av samma person) kan initiera och utföra flytten.

### <a name="will-the-person-completing-the-migration-become-the-primary-contact-on-the-company-legal-profile-in-partner-center"></a>Blir personen som slutför migreringen den primära kontakten i företagets juridiska profil i Partnercenter?

Men inte nödvändigtvis måste den primära kontakten vara någon som har behörighet att signera avtal.

### <a name="can-microsoft-migrate-my-mpn-membership-for-me"></a>Kan Microsoft migrera mitt MPN-medlemskap åt mig?

Nej. Microsoft kan inte hjälpa dig att flytta ditt medlemskapskonto till Partnercenter. Du måste flytta ditt konto genom att logga in på PMC med ditt arbetskonto (inloggningsuppgifter) för att påbörja migreringsprocessen. När du har slutfört stegen för att flytta ditt konto kan du börja hantera ditt medlemskap och tilldela användarroller och behörigheter till ditt team så att de kan komma åt förmåner och hantera medlemskapet. 

Microsoft migrerar automatiskt aktuella kompetenser, förmåner, platsinformation, bank-/skatteinformation för incitament och MCP-associationer, inklusive åtkomst till Partner University.

### <a name="how-will-the-renewal-policy-change"></a>Hur ändras förnyelseprincipen?

I Partnercenter är förnyelsefönstret från årsdagen till följande 30 dagar.

### <a name="will-our-competencies-remain-unchanged-after-we-move-to-partner-center"></a>Kommer våra kompetenser att vara oförändrade när vi har flyttat till Partnercenter?

Ja, kompetenser påverkas inte av flytten till Partnercenter. Kontakta supporten om du upptäcker [avvikelser.](https://partner.microsoft.com/support)

### <a name="will-my-benefits-including-cloud-benefits-technical-support-software-benefits-visual-studio-change-after-we-move"></a>Kommer mina fördelar (inklusive molnförmåner, teknisk support, programvaruförmåner Visual Studio) att ändras när vi har flyttat?

Dina berättigade förmåner ändras inte. Kontakta supporten om du upptäcker [avvikelser.](https://partner.microsoft.com/support)

### <a name="will-our-microsoft-accounts-that-have-visual-studio-benefits-allocations-be-honored"></a>Kommer våra Microsoft-konton som har Visual Studio-förmåner att respekteras?

Ja. Visual Studio fördelar som allokeras till MSA:er kommer att respekteras och behållas. De kommer också att bevaras efter förnyelsen i Partnercenter. Men om du tar bort en MSA-allokering när den har migrerats i Partnercenter kan den inte läggas till i Partnercenter igen.

I Partnercenter kan en partner lägga till arbetskonton och gästanvändarkonton, som är MSA från samma klientorganisation där partnern är MPN-administratör i Azure AD-klientorganisationen. Om partnern är global administratör i flera Azure AD-klienter och alla dessa klienter är associerade med samma Partnercenter-konto kan partnern lägga till användare över alla dessa klienter i Visual Studio-förmånerna och Användningsbaserade allokeringar för Azure.

Även om gästanvändare kan tilldelas användningsbaserade prenumerationer på Visual Studio av MPN-administratören eller global administratör, kan gästanvändare inte logga in på PartnerCenter med hjälp av deras MSA. Gästanvändare kan dock logga in på Azure och Visual Studio validera och använda sina tilldelade förmåner.

### <a name="how-should-we-manage-our-mcp-associations-and-our-partner-university-access"></a>Hur ska vi hantera våra MCP-associationer och vår Åtkomst till Partner University?

Det finns inga ändringar i MCP-associationer som flyttas från PMC. Alla nya medarbetare efter att du har flyttat till Partnercenter måste dock associeras i Partnercenter. Alla dina partner university-behörigheter för befintliga användare kommer [](https://partner.microsoft.com/training) att finnas kvar, men alla nya medarbetare bör gå till utbildningscentret för information om hur du får åtkomst till Partner University.

### <a name="how-do-i-view-mcp-information-once-i-move-to-partner-center"></a>Hur gör jag för att du visa MCP-information när jag har flyttat till Partnercenter?

Välj **Kompetenser** i det vänstra navigeringsfältet på instrumentpanelen. Från **sidan Kompetenser** kan du ladda ned kunskapsrapporten. I kompetensrapporten visas en lista över de användare som har skaffat sig kunskaper som är relevanta för kompetenser och program i Partnercenter. Om dina användare har fått kunskaper men dessa kunskaper inte är relevanta för de kompetenser som du arbetar mot, kommer de inte att visas i rapporten.

### <a name="are-customer-references-used-in-partner-center"></a>Används kundreferenser i Partnercenter?

Nej, du behöver inte kundreferenser för att uppfylla kompetenskraven i Partnercenter.

### <a name="will-partner-of-record-associations-move-to-partner-center"></a>Kommer partner för postassociationer att flyttas till Partnercenter?

Ja, det finns ingen ändring i Partner of Record. Läs mer om hur [du länkar ditt partner-ID till dina kunder.](/azure/billing/billing-partner-admin-link-started)

### <a name="is-there-an-impact-to-incentives-because-of-the-move-to-partner-center"></a>Påverkas incitamenten på grund av flytten till Partnercenter?

Nej, incitamenten påverkas inte om du har flyttat ditt konto utan att konsolidera platser. Om ditt företag har flera konton i PMC och du väljer att konsolidera till ett globalt konto när du flyttar till Partnercenter går det inte att förlora incitamenten, men det kan uppstå en fördröjning i incitamentutbetalningen. 

Om du inte flyttar alla dina PMC-konton som har varit inblandade i incitamentsprogram kan du sluta tjäna incitament som är knutna till dessa konton.

### <a name="what-are-the-incentive-roles-in-partner-center"></a>Vilka är incitamentrollerna i Partnercenter?

Incitamentroller i Partnercenter är platsbaserade och innehåller incitamentsadministratör och incitamentsanvändare. Mer information om vad dessa roller kan göra finns i [Tilldela användarroller och behörigheter.](permissions-overview.md)

### <a name="can-incentives-admins-be-assigned-at-the-global-and-location-level"></a>Kan incitamentsadministratörer tilldelas på global nivå och platsnivå?

Ja. Du kan tilldela en incitamentsadministratör som incitamentsadministratör för alla platser, eller så kan varje plats ha en egen incitamentsadministratör.

### <a name="can-incentives-be-paid-at-the-global-or-location-level"></a>Kan incitament betalas på global nivå eller platsnivå?

Incitament betalas endast på platsnivå.

### <a name="regarding-referrals-how-many-business-profiles-can-we-create"></a>Hur många företagsprofiler kan vi skapa när det gäller hänvisningar?

Ditt företag kan skapa så många företagsprofiler som du behöver för att fullständigt representera företagets intressen. I varje företagsprofil kan du visa upp till fem platser, en plats per land. Var och en av företagsprofilerna kan ta emot hänvisningar för var och en av sina platser.

### <a name="how-will-referrals-be-assigned-what-changes-can-i-expect-for-example-if-i-have-a-global-company-in-one-market-and-locations-in-other-markets-how-will-referrals-be-assigned"></a>Hur tilldelas hänvisningar, vilka ändringar kan jag förvänta mig? Hur kommer hänvisningar att tilldelas om jag till exempel har ett globalt företag på en marknad och på andra marknader?

Referenser tilldelas baserat på de sökparametrar som kunden definierar. Oavsett om du har en plats eller många, och om kunden anger en önskad plats och du har ett företag där som uppfyller de andra parametrarna så kommer hänvisningen att gå till den platsen.

### <a name="i-am-migrating-to-partner-center-from-within-russia-i-get-an-error-message-about-web-direct-how-do-i-continue-with-the-migration"></a>Jag migrerar till Partnercenter från Ryssland. Jag får ett felmeddelande om Web Direct. Hur gör jag för att fortsätta med migreringen?

Om du får ett felmeddelande eftersom du deltar i Web Direct-programmet bör du göra följande:

1. Logga in på portalen. Azure.com och skapa en ny Azure AD-klientorganisation. Mer information finns i [Skapa en ny Azure AD-klientorganisation.](/azure/active-directory/fundamentals/active-directory-access-create-new-tenant)

2. När du har skapat den nya Azure AD-klienten kan du använda den för att migrera från Partner Membership Center till Partnercenter eller för att registrera dig som en ny net i Partnercenter.