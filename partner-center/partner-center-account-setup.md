---
title: Hantera ditt Partnercenter-konto
ms.topic: conceptual
ms.date: 11/20/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Lär dig hur du använder Partner Center för att hantera företagets profil, bank och skatte information, roller, behörigheter med mera.
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 55046b21e70ad04f47bf4cd191736aa12335060e
ms.sourcegitcommit: 147813ba322653c989df5afe0b3bf0c252523a92
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 12/03/2020
ms.locfileid: "96556454"
---
# <a name="manage-your-partner-center-account---company-profile-bank-information-roles-permissions-and-more"></a>Hantera ditt partner Center-konto – företags profil, bank information, roller, behörigheter med mera

**Lämpliga roller** – global administratör, MPN-administratör

Det konto som du skapar i partner centret när du registrerar dig är ditt e-post och din företags information. När du har skapat ett konto slutför du konfigurationen av företagets fullständiga profil, inklusive support information, fil skatte undantag om det behövs och primär kontakt information. Ditt företags konto innehåller också användar konton för alla som kommer att använda Partner Center för att lägga till eller hantera kunder, Sälj prenumerationer, arbeta med fakturering och fakturering, skapa affärs profiler, hantera hänvisningar, arbeta med stimulans program och tillhandahålla support.

Se även artiklar [Bjud in anställda till Partner Center](guide-to-migration.md) och [lägga till en ny användare](create-user-accounts-and-set-permissions.md).

>[!NOTE]
>Menyn konto inställningar ändras beroende på vilka program som du har registrerat i. Om du till exempel är partner i Cloud Solution Provider-programmet (CSP) kan du hantera dina Azure-delade tjänster från konto inställningar.

## <a name="account-management"></a>Kontohantering

Om du vill komma åt konto hantering i Partner Center för alla partner, kommersiell och utvecklare loggar du in på Partner Center- [instrumentpanelen](https://partner.microsoft.com/dashboard) och väljer **Inställningar** (kugg hjuls ikonen) i det övre högra hörnet på skärmen och sedan **konto inställningar**. Du behöver inte längre välja mellan inställningar för partner och utvecklare eftersom alla profiler och inställningar nu kombineras.

:::image type="content" source="images/accountsettings/opening.png" alt-text="inställnings ikon":::

Då visas sidan konto inställningar.

:::image type="content" source="images/accountsettings/account-settings-sv.png" alt-text="Menyn Inställningar.":::

### <a name="locate-your-mpn-id"></a>Hitta ditt MPN-ID

Oavsett om du är partner eller utvecklar kan du använda ditt MPN-ID för att logga support biljetter. Ditt MPN-ID finns på Thee-sidan för **juridisk information** . Du kan också hitta den i **identitets profilen**.

## <a name="organization-profile"></a>Organisations profil

Använd dessa sidor för att hantera sådana områden som juridisk företags profil, partner profil och företags platser. Välj flikar som **juridiska** eller **innehavare** (beskrivs i detalj nedan) om du vill redigera det här fältet. Välj fliken för det program som du är intresse rad av (MPN, CSP eller kommersiell marknads plats) för att se information och först konsumentsajter status.

:::image type="content" source="images/accountsettings/account-settings-new.png" alt-text="Meny för juridisk information.":::

### <a name="legal-info"></a>Juridisk information

När du först ansluter till Partner Center går företaget igenom en verifierings process med Microsoft. Du kan spåra status för verifieringen på sidan **juridisk information** . Den visar den primära kontakten (som Microsoft kommer att kontakta angående partner frågor) samt den primära juridiska kontakten (den person som hanterar din juridiska information och status). Alla företagets företags platser visas och du kan lägga till dem här.

Läs mer om [verifiering och din konto information](verification-responses.md).

### <a name="tenants-profile"></a>Klient organisations profil

Den här sidan innehåller all information om dina Azure AD-klienter, både kommersiella och utvecklare. Den här profilen är den globala administratören som kan associera nya klienter till det globala partner kontot.

### <a name="identifiers"></a>Identifierare

Den här sidan innehåller Partner Center identiteter för ditt företag: MPN-ID, Publisher-ID, Windows Publisher ID med mera.  Varje område kan expanderas och redige ras så att till exempel den primära kontakten för din publicerings verksamhet är lätt att hitta.

### <a name="company-profile"></a>Företags profil

På den här sidan identifieras den typ av partnerskap som du har med Microsoft, till exempel oberoende program varu leverantör eller CSP-programpartner. Det visar antalet kunder som du arbetar med, årlig intäkt och företagets aktuella storlek. Expandera företags information på sidan **företags information** för att berätta för Microsoft vilken typ av arbete du vill göra med Microsoft, t. ex. skapa program, sälja Microsoft och tredjepartsprogram eller vara en System Integrator. Du kan också definiera var du för närvarande gör affärer och de lokala där du vill utöka verksamheten i framtiden.

### <a name="account-merge-profile"></a>Konto sammanslagnings profil

När du bjuder in ett företag som har ett aktivt konto i Partner Center att slå samman sitt konto med ditt, hanteras informationen på sidan **koppla konto** . Leta upp MPN-ID: t för företaget som du vill bjuda in till att koppla ihop med dina, Visa aktuella fusioner och skicka inbjudningar till företag. Acceptera eller avvisa en inbjudan att slå samman ditt företags konto till ett annat företags konto här. Mer information finns i [koppla ditt partner konto till ett annat partner konto](merge-accounts.md).

## <a name="payout-and-tax"></a>Utbetalning och skatt

Den här sidan innehåller information om utbetalnings-och skatte information, inklusive **faktura till** information, **inköps order nummer**, skatte-ID för ditt företag, moms-ID-nummer om du har en och den valuta som du använder.

## <a name="user-management"></a>Användarhantering

Vad du arbetar med i Partner Center och vilka områden som du kan uppdatera eller se beror på din roll och de behörigheter som är kopplade till den rollen. Om du till exempel inte är en incitaments administratör kan du inte ändra något på sidan incitament, men du kanske kan visa data.

### <a name="update-preferred-email"></a>Uppdatera prioriterad e-post

Så här uppdaterar du önskat e-postmeddelande för att ta emot Partner Center-meddelanden:

1. Logga in på [instrument panelen för partner Center](https://partner.microsoft.com/dashboard).
1. Gå till [**Inställningar för engagemang**](https://partner.microsoft.com/dashboard/engagement/preference), Välj länken **ändra** , uppdatera e-postadressen och välj **Spara**.

### <a name="find-your-user-role"></a>Hitta din användar roll

1. Gå till **Inställningar** och välj **min profil**.

1. På sidan **information** visas din personliga information som den gäller för ditt arbete och din utbildning, dina tentor och certifierings data.

1. Välj fliken **roller och behörigheter** för att se alla roller som du har tilldelats och de behörigheter som dessa roller tillhandahåller.

## <a name="programs-in-which-you-are-enrolled"></a>Program som du har registrerat i

Det arbete som du hanterar ditt partner Center-konto relaterar till de program som du har registrerat i och de användar roller och behörigheter som du har tilldelats i Partner Center.

Se vilka program som du har åtkomst till:

1. Logga in på [instrument panelen](https://partner.microsoft.com/dashboard)för partner Center.

2. Den vänstra navigerings menyn visar de program som du har registrerat i och kommer att visa tillgängliga alternativ för varje program.

Här är ett exempel. Anta att en användare har åtkomst till tre program på Partner Center-instrumentpanelen: **MPN** -programmet, programmet för **hänvisning** och programmet för **kommersiella marknads platser** . När de loggar in på Partner Center-instrumentpanelen visas dessa tre program till vänster på skärmen.

:::image type="content" source="images/accountsettings/programs-enrolled-left-nav.png" alt-text="Program registrerade-menyn.":::

### <a name="enrolling-in-programs"></a>Registrera i program

Det finns många tillgängliga Partner Center-program. Varje program har olika krav som företaget behöver uppfylla innan det kan registreras i det programmet.

Information om hur du registrerar i vissa partner Center-program finns i följande ofullständiga lista:

- [Program för kommersiella marknads platser](https://docs.microsoft.com/azure/marketplace/partner-center-portal/create-account)
- [Microsoft Partner Network medlemskaps förmåner](mpn-overview.md)
- [CSP-program](https://docs.microsoft.com/partner-center/enrolling-in-the-csp-program)
- [Office Store](https://partner.microsoft.com/dashboard/account/v3/enrollment/introduction/office)

Mer information om hur du registrerar i Partner Center-program finns även i [partner nätverks resurser](https://partner.microsoft.com/).

## <a name="next-steps"></a>Nästa steg

- [Uppdatera din partnerprofil](update-your-partner-profile.md)
- [Skapa användar konton och ange behörigheter](create-user-accounts-and-set-permissions.md)
- [Tilldela användarroller och -behörigheter](permissions-overview.md)
- [Hantera ditt MPN-konto: platser](manage-locations.md)
- [Återställa ett användarlösenord](reset-a-user-password.md)
- [API: Hämta juridisk företags profil för partner](https://docs.microsoft.com/partner-center/develop/get-legal-business-profile.md)
- [Identifiera erbjudanden och priser i Partner Center handels Marketplace](csp-commercial-marketplace-discover.md)
