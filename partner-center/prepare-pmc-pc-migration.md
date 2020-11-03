---
title: Flytta från partner medlemskaps Center
ms.topic: article
ms.date: 06/01/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Läs igenom användbar information och vanliga frågor och svar innan du flyttar ditt företag från partner medlemskaps Center till Partner Center.
author: parthpandyamsft
ms.author: parthp
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: be4250864bd07e555b0eb2079c28f3dfb4920805
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/22/2020
ms.locfileid: "92531600"
---
# <a name="prepare-for-your-move-from-partner-membership-center-pmc-to-partner-center"></a>Förbered dig för flytt från Partner medlemskap Center (PMC) till Partner Center

**Lämpliga roller**
- Global administratör
- Användaradministratör
- Försäljnings agent
- Administratörs agent

Vi flyttar medlemskaps hantering från partner medlemskaps Center (PMC) till Partner Center – det enda målet att hantera affärs relationer med Microsoft. Vi vill att din flytt till Partner Center ska vara så effektiv och enkel som möjligt. Vi har identifierat vissa områden där partner centret skiljer sig från PMC, och vi tror att du kommer att vilja förstå och förbereda dig innan du gör flytten.

## <a name="account-and-identity-setup"></a>Konfiguration av konto och identitet

Se nedan för svar på vanliga frågor om konto-och identitets konfiguration.

### <a name="what-is-an-azure-active-directory-azure-ad-work-account"></a>Vad är ett Azure Active Directory (Azure AD)-arbets konto?

Ett Azure-arbetskonto är en dedikerad och isolerad virtuell representation av ditt företag i det offentliga Azure-molnet som skapas åt dig när du prenumererar på en moln tjänst från Microsoft, till exempel Azure, Microsoft Intune eller Office 365.

Ditt arbets konto är värd för Azure AD-användare och information om dem – e-post, lösen ord, profil data, behörigheter och så vidare. Arbets kontot innehåller också grupper, program och annan information som rör ett företag och dess säkerhet. 

Ditt arbets-e-postmeddelande ingår i din Azure Active Directory-klient. Om du vill ha ett konto i Partner Center måste du ha en AAD-klient. Mer information om Azure Active Directory finns [i skapa din katalog i Azure AD](/azure/active-directory/fundamentals/add-custom-domain#create-your-directory-in-azure-ad).

I Partner Center använder du din e-postadress för arbetet för att logga in på ditt konto, inte din personliga e-postadress.

- Ditt arbets konto: john@contoso.com
- Ditt personliga konto: John@outlook.com

### <a name="what-account-should-you-sign-into-partner-center-with-if-you-have-an-aad-tenant-with-microsoft-for-office-365-for-example-and-you-also-have-a-tenant-for-your-csp-business"></a>Vilket konto ska du logga in på Partner Center med om du har en AAD-klient med Microsoft (för Office 365 till exempel) och du också har en klient för din CSP-verksamhet?

Du kan logga in på Partner Center med antingen CSP-kontot eller ditt MPN Work-e-postkonto. Om du väljer att logga in med din e-postadress för din e-post visas den vänstra navigeringen på instrument panelen både MPN och CSP-programinformation. Om du loggar in med din MPN Azure AD-klient för e-post visas bara din MPN-programinformation. 

### <a name="if-you-dont-want-to-use-your-existing-office-365-azure-ad-tenant-for-partner-center-you-can-create-a-new-tenant-prior-to-migrating-from-pmc"></a>Om du inte vill använda din befintliga Office 365 Azure AD-klient för partner Center kan du skapa en ny klient organisation innan du migrerar från PMC.

Det kan finnas många orsaker till att du inte vill använda en befintlig Azure AD-klient för att konfigurera ditt partner Center-konto. Innan du börjar migrera till Partner Center går du till [Azure Portal](https://ms.portal.azure.com/#home) för att skapa en ny Azure AD-klient. Följ anvisningarna i [skapa en ny klient i Azure Active Directory](/azure/active-directory/develop/quickstart-create-new-tenant). Använd den nya AAD-klienten för att konfigurera ditt partner Center-konto. Du måste vara global administratör för att skapa klienten. 

### <a name="user-roles-including-guest-user-roles-in-partner-center"></a>Användar roller inklusive gäst användar roller i Partner Center

Partner Center har olika typer av roller beroende på vilka typer av arbete som måste utföras. Det finns roller som globala administratörer som är Azure AD-roller. Några av rollerna är olika för program som moln tjänst leverantörens program eller incitament, och det finns roller som är speciella för MPN. Läs [Tilldela användar roller och behörigheter](permissions-overview.md)för att ta reda på vad alla partner Center-roller är.

### <a name="what-happens-to-my-users-roles-when-they-move-from-pmc-to-partner-center"></a>Vad händer med mina användares roller när de flyttas från PMC till Partner Center?

Förutom för MPN globala administratörs-eller primär program kontakt som utför migreringen förlorar alla användare i PMC sina administratörs roller. Den person som Slutför migreringen måste tilldela roller i Partner Center. Rollerna i partner centret skiljer sig från rollerna i PMC. Läs [tilldela användare roller och behörigheter] (behörigheter-overview.md och [flytta från PMC till Partner Center](move-pmc-pc-map.md#user-roles) för mer information om användar roller i Partner Center.

### <a name="whats-the-difference-between-my-company-profile-and-my-business-profile"></a>Vad är skillnaden mellan min företags profil och min företags profil?

Företags profilen är information om ditt företag som innehåller adress, platser, primär kontakt, bank och skatte information.

Din företags profil är hur du visar dig själv för kunderna och är en marknadsförings sida som visar din logo typ, information om ditt företags fokus, dina expert kunskaper osv.

### <a name="what-does-account-consolidation-mean-for-my-account"></a>Vad betyder konto konsolidering för mitt konto?

Om du använder samma Azure AD-klient för att migrera flera MPN-konton till Partner Center, känner systemet automatiskt igen det och ber dig att konsolidera dina konton. Detta gäller även om du har flera domäner kopplade till samma Azure AD-klient. 

Du kan fortfarande välja att migrera till Partner Center med hjälp av separata AAD-klienter, men Observera att detta ger en isolerad utvärdering av dina kompetenser och extra inköps kostnader. Mer information om konto konsolidering finns [i konsolidera företags konton](consolidate-accounts.md)

### <a name="if-i-have-multiple-aad-tenants-and-a-single-mpn-account-is-it-possible-to-link-them-in-partner-center"></a>Om jag har flera AAD-klienter och ett enda MPN-konto, är det möjligt att länka dem i Partner Center?

Ja, i Partner Center kan du länka flera Azure AD-klienter till ett enda partner Center-konto.
Mer information om konto konsolidering finns [i konsolidera företags konton](consolidate-accounts.md)

### <a name="are-there-restrictions-to-adding-multiple-azure-ad-tenants-to-a-single-partner-center-account"></a>Finns det några begränsningar för att lägga till flera Azure AD-klienter till ett enda partner Center-konto?

Om Azure AD-klienten redan är kopplad till ett befintligt Partner Center-konto kan det inte kopplas till nya partner Center-konton med hjälp av funktionen för flera innehavare. Ett annat sätt att tänka på det är att en Azure AD-klient bara kan kopplas till ett partner Center-konto, men ett partner Center-konto kan ha flera kopplade klienter.

## <a name="microsoft-partner-network-mpn-membership-migration"></a>Microsoft Partner Network (MPN) medlemskaps-migrering 

Se följande svar på vanliga frågor om migrering av MPN-medlemskap.

### <a name="who-can-perform-the-move-from-pmc-to-partner-center"></a>Vem kan utföra flytten från PMC till Partner Center?

Företaget MPN global admin eller den primära program kontakten (dessa två roller brukar innehas av samma person) kan initiera och utföra flytten.

### <a name="will-the-person-completing-the-migration-become-the-primary-contact-on-the-company-legal-profile-in-partner-center"></a>Blir personen som Slutför migreringen den primära kontakten i företagets juridiska profil i Partner Center?

Den primära kontakten behöver dock inte nödvändigt vis vara någon som har behörighet att signera avtal.

### <a name="can-microsoft-migrate-my-mpn-membership-for-me"></a>Kan Microsoft migrera mitt MPN-medlemskap åt mig?

Nej. Microsoft kan inte hjälpa dig att flytta ditt medlemskaps konto till Partner Center. Du måste flytta ditt konto genom att logga in på PMC med ditt arbets konto (inloggnings uppgifter) för att starta migreringsprocessen. När du har slutfört stegen för att flytta ditt konto kan du börja hantera ditt medlemskap och tilldela användar roller och behörigheter till ditt team så att de kan komma åt förmåner och hantera medlemskapet. 

Microsoft kommer automatiskt att migrera aktuella kompetenser, förmåner, plats information, bank-och skatte information för incitament och MCP-associationer, inklusive partner University Access.

### <a name="how-will-the-renewal-policy-change"></a>Hur ändras förnyelse principen?

I Partner Center är förnyelse perioden från ditt jubileums datum under följande 30 dagar.

### <a name="will-our-competencies-remain-unchanged-after-we-move-to-partner-center"></a>Är våra kompetenser oförändrade när vi flyttar till Partner Center?

Ja, kompetenser påverkas inte av flytten till Partner Center. Kontakta [supporten](https://partner.microsoft.com/support)om du märker avvikelser.

### <a name="will-my-benefits-including-cloud-benefits-technical-support-software-benefits-visual-studio-change-after-we-move"></a>Kommer mina förmåner (inklusive fördelar med molnet, teknisk support, program varu förmåner, Visual Studio) att ändras när vi flyttar?

Dina berättigade förmåner kommer inte att ändras. Kontakta [supporten](https://partner.microsoft.com/support)om du märker avvikelser.

### <a name="will-our-microsoft-accounts-that-have-visual-studio-benefits-allocations-be-honored"></a>Kommer våra Microsoft-konton som har förmåns tilldelningar för Visual Studio att behållas?

Ja. Visual Studio-förmåner som tilldelas till MSA: er kommer att behållas och behållas. De kommer också att bevaras efter förnyelse i Partner Center. Men om du tar bort en MSA-allokering när du har migrerat i Partner Center kan du inte lägga till den i Partner Center igen.

I Partner Center kan en partner lägga till arbets konton och gäst användar konton, som är MSA från samma klient organisation där partnern är MPN-administratör i Azure AD-klienten. Om partnern är global administratör i flera Azure AD-klienter och alla dessa klienter är kopplade till samma Partner Center-konto, tillåts partnern att lägga till användare över alla dessa klienter i Visual Studio-förmånerna och Azure Usage-baserade allokeringar.

Gäst användare kan tilldelas användnings prenumerationer av Visual Studio av MPN-administratören eller den globala administratören, men gäst användare kan inte logga in på Partner Center med hjälp av deras MSA. Gäst användare kan dock logga in på Azure och Visual Studio för att validera och använda sina tilldelade förmåner.

### <a name="how-should-we-manage-our-mcp-associations-and-our-partner-university-access"></a>Hur ska vi hantera våra MCP-associationer och vår partner University-åtkomst?

Det finns inga ändringar i MCP-associationerna som flyttas från PMC. Alla nya nya medarbetare efter att du har flyttat till Partner Center måste dock vara kopplade till Partner Center. Alla dina partner University-behörigheter för befintliga användare är kvar men eventuella nya medarbetare bör gå till [utbildnings centret](https://partner.microsoft.com/training) för information om hur du får åtkomst till partner University.

### <a name="how-do-i-view-mcp-information-once-i-move-to-partner-center"></a>Hur gör jag för att Visa MCP-information när jag flyttar till Partner Center?

Välj **kompetenser** i det vänstra navigerings fältet på instrument panelen. På sidan **kompetenser** kan du hämta kunskaps rapporten. Kunskaps rapporten visar en lista över de användare som har fått de kunskaper som är relevanta för kompetens och program i Partner Center. Om dina användare har fått kunskaper men dessa kunskaper inte är relevanta för de kompetenser som du arbetar mot, visas de inte i rapporten.

### <a name="are-customer-references-used-in-partner-center"></a>Används kund referenser i Partner Center?

Nej, du behöver inte kund referenser för att uppfylla kompetens kraven i Partner Center.

### <a name="will-partner-of-record-associations-move-to-partner-center"></a>Kommer partner av post kopplingar att flyttas till Partner Center?

Ja, det finns ingen ändring i partnern av posten. Lär dig mer om [att länka ditt partner-ID till dina kunder](/azure/billing/billing-partner-admin-link-started).

### <a name="is-there-an-impact-to-incentives-because-of-the-move-to-partner-center"></a>Finns det en inverkan på att uppmuntras på grund av flytten till Partner Center?

Nej, det finns ingen inverkan på att incitament om du har flyttat ditt konto utan att konsolidera platser. Om ditt företag har flera konton i PMC och, när du flyttar till Partner Center, som du bestämmer för att konsolidera till ett globalt konto, går det ingen förlust att incitament, men det kan uppstå en fördröjning i incitaments utbetalning. 

Om du inte flyttar alla dina PMC-konton som har varit involverade i stimulans program, kan du slippa incitament som är kopplade till dessa konton.

### <a name="what-are-the-incentive-roles-in-partner-center"></a>Vilka är stimulans rollerna i Partner Center?

Stimulans roller i Partner Center är platsbaserade och inkluderar incitaments administratör och incitaments användare. Mer information om vad dessa roller kan göra finns i [Tilldela användar roller och behörigheter](permissions-overview.md).

### <a name="can-incentives-admins-be-assigned-at-the-global-and-location-level"></a>Kan uppmuntra administratörer tilldelas på global nivå och på plats nivå?

Ja. Du kan tilldela en incitaments administratör som incitaments administratör för alla platser eller varje plats kan ha en egen incitaments administratör.

### <a name="can-incentives-be-paid-at-the-global-or-location-level"></a>Kan incitament betalas på global nivå eller på plats nivå?

Incitament betalas endast på plats nivå.

### <a name="regarding-referrals-how-many-business-profiles-can-we-create"></a>Vad gäller hänvisningar, hur många affärs profiler kan vi skapa?

Företaget kan skapa så många affärs profiler som du behöver för att helt kunna representera företagets intressen. I varje affärs profil kan du lista upp till fem platser, en plats per land. Var och en av affärs profilerna kan ta emot hänvisningar för var och en av dess platser.

### <a name="how-will-referrals-be-assigned-what-changes-can-i-expect-for-example-if-i-have-a-global-company-in-one-market-and-locations-in-other-markets-how-will-referrals-be-assigned"></a>Hur kommer hänvisningarna att tilldelas, vilka ändringar kan jag förväntar mig? Om jag till exempel har ett globalt företag på en marknad och platser på andra marknader, hur kommer hänvisningarna att tilldelas?

Hänvisningar tilldelas baserat på de Sök parametrar som kunden definierar. Oavsett om du har en plats eller många, och om kunderna anger en önskad plats och du har ett företag där de uppfyller de andra parametrarna, kommer hänvisningen att gå till den platsen.

### <a name="i-am-migrating-to-partner-center-from-within-russia-i-get-an-error-message-about-web-direct-how-do-i-continue-with-the-migration"></a>Jag migrerar till Partner Center i Ryssland. Jag får ett fel meddelande om webb Direct. Hur gör jag för att fortsätta med migreringen?

Om du får ett fel meddelande eftersom du deltar i webb direkt programmet bör du göra följande:

1. Logga in på portalen. Azure.com och skapa en ny Azure AD-klient. Mer information finns i [skapa en ny Azure AD-klient](/azure/active-directory/fundamentals/active-directory-access-create-new-tenant).

2. När du har skapat den nya Azure AD-klienten kan du använda den för att migrera från Partner medlemskap Center till Partner Center eller för att registrera sig som en ny nätverks partner i Partner Center.