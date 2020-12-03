---
title: Länka ditt arbets konto för att komma åt Partner Center
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Skapa ett arbets konto som länkar ditt företag till ditt partner Center-konto. Detta gör det möjligt för anställda i företaget att komma åt Partner Center.
author: vinayks
ms.author: vinayks
ms.custom: SEOAPR.20
ms.localizationpriority: high
ms.date: 11/25/2019
ms.openlocfilehash: bc837db5a9dbcf92fbfead54b552695a218ae675
ms.sourcegitcommit: 2d9aab15ddc20cb3d9537e68ace33d36f7d8a250
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 12/02/2020
ms.locfileid: "96534802"
---
# <a name="create-a-work-account-that-links-your-company-to-your-partner-center-account"></a>Skapa ett arbets konto som länkar ditt företag till ditt partner Center-konto

**Lämpliga roller**

- Global administratör
- Administratör för användar hantering

## <a name="why-you-need-a-work-account"></a>Varför du behöver ett arbets konto

Microsoft kräver att du länkar ditt företags arbets konto till ditt nya partner Center-konto. Länken gör att ditt konto användare kan logga in på Partner Center med sitt arbets konto användar namn och lösen ord.

## <a name="the-work-account-email-address"></a>E-postadress till arbets konto

Ditt arbets konto eller din e-postadress för arbetet är den e-postadress som du fått av ditt företag. Ett e-postmeddelande med arbets konto är vanligt vis i formatet `you@yourcompany.com` . Personliga e-postadresser som Hotmail, Gmail eller Yahoo fungerar inte med e-post och kan inte användas för ditt partner Center-konto.

Om du har fler än en giltig e-postadress för arbetet använder du den som är kopplad till företagets huvud kontor i stället för den regionala avdelningen, till exempel använder din `contoso.com` e-postadress i stället för `contoso.uk` adressen.

> [!NOTE]  
> Innan du bestämmer dig för att använda ett befintligt arbets konto bör du tänka på hur många användare i kontot som behöver arbeta i Partner Center. Om du har användare i kontot som inte behöver arbeta i Partner Center bör du överväga att skapa ett nytt konto för de användare som behöver arbeta i partner centret.

## <a name="not-sure-if-your-company-already-has-a-work-account"></a>Är du osäker på om ditt företag redan har ett arbets konto?

Om du inte är säker på om ditt företag har ett arbets konto följer du de här stegen för att kontrol lera. Om du har en aktiv prenumeration på Microsoft Azure eller Office 365 har du redan ett arbets konto.

1. Logga in på [Azure-portalen](https://portal.azure.com).

2. Välj Azure Active Directory på menyn och välj sedan domän namn.

3. Om du redan har ett arbets konto visas ditt domän namn.

Om ditt företag inte redan har ett arbets konto kan du skapa ett under registrerings processen.

Diagrammet nedan innehåller steg för flera typiska scenarier:

- ta reda på om du har ett arbets konto
- ta reda på hur du loggar in på ditt arbets konto
- avgöra om du behöver skapa ett nytt arbets konto

:::image type="content" source="images/onboardingAADFlow.png" lightbox="images/onboardingAADFlow.png" alt-text="Har du ett arbets konto eller behöver du skapa ett?":::

Mer information om hur du lägger till domäner i Azure AD finns i [lägga till eller associera en domän i Azure AD](/azure/active-directory/active-directory-add-domain)

## <a name="about-microsoft-azure"></a>Om Microsoft Azure

Microsoft Azure är en offentlig moln plattform som företag kan använda för att bygga, distribuera och hantera program i ett globalt nätverk av Microsoft-hanterade data Center. Företag använder Azure för att bygga en virtuell IT-infrastruktur med virtuella funktioner eller tjänster i stället för fysiska datorer.

När du köper en Azure-prenumeration hyr du i princip ett dedikerat, säkert utrymme i det offentliga Azure-molnet, så att det inte är för annat än att hyra ut en våning i en kontors byggnad för att dela ditt företags fysiska verksamhet. Ditt företag är en klient organisation för Office-byggnadens ägare.

Ett Azure-arbetskonto är en dedikerad och isolerad virtuell representation av ditt företag i det offentliga Azure-molnet som skapas åt dig när du prenumererar på en moln tjänst från Microsoft, till exempel Azure, Microsoft Intune eller Office 365.

Ditt arbets konto är värd för Azure AD-användare och information om dem – deras lösen ord, profil data, behörigheter och så vidare. Arbets kontot innehåller också grupper, program och annan information som rör ett företag och dess säkerhet.

## <a name="next-steps"></a>Nästa steg

- [Hantera ditt Partnercenter-konto](partner-center-account-setup.md)
- [Spåra verifierings status](verification-responses.md)