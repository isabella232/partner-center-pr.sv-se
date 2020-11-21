---
title: Hantera ditt Partnercenter-konto
ms.topic: conceptual
ms.date: 11/20/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Lär dig hur du hanterar företagets profil, bank och skatte information och mer i Partner Center.
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 4cdaa7f8a2a6c8643b86f3e34569c2140ecd7450
ms.sourcegitcommit: 1aa43438ad181278052788f15e017f9ae7777943
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 11/21/2020
ms.locfileid: "95007065"
---
# <a name="manage-your-partner-center-account---company-profile-bank-information-roles-permissions-and-more"></a>Hantera ditt partner Center-konto – företags profil, bank information, roller, behörigheter med mera

**Lämpliga roller**

- global administratör
- MPN-administratör

Det konto som du skapar i partner centret när du registrerar dig är ditt e-post och din företags information. När du har skapat ett konto slutför du konfigurationen av företagets fullständiga profil, inklusive support information, fil skatte undantag om det behövs och primär kontakt information. Ditt företags konto innehåller också användar konton för alla som kommer att använda partner centret för att lägga till eller hantera kunder, Sälj prenumerationer, arbeta med fakturering och fakturering, skapa affärs profiler, hantera hänvisningar, arbeta med incitaments program och tillhandahålla support.

Se även 

- [Bjud in anställda att delta i Partner Center](guide-to-migration.md)

- [Lägg till en ny användare](create-user-accounts-and-set-permissions.md)

>[!NOTE]
>Menyn konto inställningar ändras beroende på vilka program som du har registrerat i. Om du till exempel är partner i Cloud Solution Provider-programmet (CSP) kan du hantera dina Azure-delade tjänster från konto inställningar.

## <a name="account-management"></a>Kontohantering

Om du vill komma åt konto hantering i Partner Center för alla partner, kommersiell och utvecklare loggar du in på Partner Center- [instrumentpanelen](https://partner.microsoft.com/dashboard)och väljer sedan alternativet **Inställningar** (kugg hjuls ikonen) i det övre högra hörnet på skärmen. Du behöver inte längre välja mellan partner och utvecklare eftersom alla profiler och inställningar nu kombineras.

:::image type="content" source="images/accountsettings/opening.png" alt-text="inställnings ikon":::


:::image type="content" source="images/accountsettings/accountsettingssv.png" alt-text="Kontoinställningar":::

### <a name="locate-your-mpn-id"></a>Hitta ditt MPN-ID

Oavsett om du är partner eller en utvecklare, måste du använda ditt MPN-ID för sådana saker som att logga support biljetter. Ditt MPN-ID finns på sidan med **juridisk** information. Du kan också hitta den i **identitets profilen**.

## <a name="organization-profile"></a>Organisations profil

Du hanterar din juridiska företags profil, din partner profil och företagets platser på sidan **organisations profil** . På den här sidan kan du se information på den översta nivån om ditt företag. Du kan öka detalj nivån och redigera varje region. Välj den flik som motsvarar det aktuella programmet som du är intresse rad av (MPN, CSP eller kommersiell marknads plats) för att se information och först konsumentsajter status.
 
:::image type="content" source="images/accountsettings/accountsettingsnew.png" alt-text="juridisk information":::
 
### <a name="legal-information"></a>Juridisk information

När du först ansluter till Partner Center går företaget igenom en verifierings process med Microsoft. Du kan spåra status för verifieringen på den **juridiska profilen**. Den primära kontakten, personen som Microsoft kontaktar för partner frågor, samt den primära juridiska kontakten, den person som hanterar din juridiska information och status finns på sidan **juridisk profil** . Alla företagets företags platser finns här och du kan lägga till ytterligare företags platser här.  

Läs mer om [verifiering och din konto information](verification-responses.md).

### <a name="tenants-profile"></a>Klient organisations profil

All information om dina Azure AD-klienter, kommersiella och utvecklare, spåras på **klient profil** sidan. Den här profilen är den globala administratören som kan associera nya klienter till det globala partner kontot.

### <a name="identifiers"></a>Identifierare 

Avsnittet **identifierare** innehåller Partner Center identiteter för ditt företag – dina MPN-ID, ditt utgivar-ID, ditt Windows Publisher-ID med mera. Varje område kan expanderas och redige ras så att till exempel den primära kontakten för din publicerings verksamhet är lätt att hitta.

### <a name="company-profile"></a>Företags profil

**Företags profilen** identifierar vilken typ av partnerskap du har med Microsoft, till exempel oberoende program varu leverantör eller CSP-programpartner. Du kan se en ögonblicks bild av antalet kunder som du arbetar med, din årliga intäkt, företagets aktuella storlek. Du kan också expandera företags information på sidan företags information. På den här sidan kan du också tala om för Microsoft vilken typ av arbete du vill göra med Microsoft, till exempel skapa program, sälja Microsoft-program från tredje part eller vara en system integrerare. Du kan också definiera var du för närvarande gör affärer och de lokala där du vill utöka verksamheten i framtiden.

### <a name="account-merge-profile"></a>Konto sammanslagnings profil

När du bjuder in ett företag som har ett aktivt konto i Partner Center att slå samman sitt konto med ditt, hanteras informationen på sidan **koppla konto** . Leta upp MPN-ID: t för företaget som du vill bjuda in till att koppla ihop med dina, Visa aktuella fusioner och skicka inbjudningar till företag. Här kan du också acceptera eller avvisa en inbjudan att slå samman ditt företags konto till ett annat företags konto. Detaljerad information om hur du kopplar konton finns i [koppla ditt partner konto till ett annat partner konto](merge-accounts.md).

### <a name="payout-and-tax"></a>Utbetalning och skatt 

**Utbetalningen och skatten** innehåller din utbetalnings-och skatte information, inklusive **faktura till** information och **P.O.-nummer**. Skatte-ID: t för ditt företag är även på den här sidan, inklusive ditt moms-ID-nummer om du har en och den valuta som du använder.


## <a name="user-roles-and-permissions"></a>Användar roller och behörigheter

Hur ditt arbete i Partner Center och de områden som du kan uppdatera eller se beror på din roll och de behörigheter som är kopplade till den rollen. Om du till exempel inte är en incitaments administratör kan du inte ändra något på sidan incitament, men du kanske kan visa data. 

### <a name="update-preferred-email"></a>Uppdatera prioriterad e-post

Så här uppdaterar du önskat e-postmeddelande för att ta emot Partner Center-meddelanden: 

1. Logga in på [instrument panelen för partner Center](https://partner.microsoft.com/dashboard).
1. Gå till [**Inställningar för engagemang**](https://partner.microsoft.com/dashboard/engagement/preference), Välj länken **ändra** , uppdatera e-postadressen och klicka på **Spara**.

### <a name="find-your-user-role"></a>Hitta din användar roll

1. Gå till **Inställningar** och välj **min profil**.
 
1. På sidan **information** visas din personliga information som den gäller för ditt arbete och din utbildning, dina examina och certifierings data.
 
1. Välj fliken **roller och behörigheter** . Här visas alla roller som du har tilldelats och de behörigheter som dessa roller tillhandahåller.

## <a name="programs-in-which-you-are-enrolled"></a>Program som du har registrerat i

Mycket av det arbete som du hanterar ditt partner Center-konto relaterar till de program som du har registrerat i och de användar roller och behörigheter som du har tilldelats i partner centret.

Se vilka program som du har åtkomst till i Partner Center:

1. Logga in på [instrument panelen](https://partner.microsoft.com/dashboard)för partner Center.

2. Den vänstra navigerings menyn visar de program som du har registrerat i och kommer att visa tillgängliga alternativ för varje program.

Här är ett exempel. Låt oss anta att en användare har åtkomst till tre program på Partner Center-instrumentpanelen: **MPN** -programmet, programmet för **hänvisning** och programmet för **kommersiella marknads platser** . När de loggar in på Partner Center-instrumentpanelen visas dessa tre program till vänster på skärmen.

:::image type="content" source="images/accountsettings/programs-enrolled-left-nav.png" alt-text="program registrerad meny":::

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
