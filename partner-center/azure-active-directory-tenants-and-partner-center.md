---
title: Länka ditt arbetskonto för att få åtkomst till Partnercenter
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-account
description: Skapa ett arbetskonto som länkar ditt företag till ditt Partnercenter-konto. Detta gör att anställda på ditt företag kan komma åt Partnercenter.
author: vinayks
ms.author: vinayks
ms.custom: SEOAPR.20
ms.localizationpriority: high
ms.date: 6/17/2021
ms.openlocfilehash: 9632cc6fbf18a02526cb0df4699bbe0ffaee4bb26ded97b3cb8b186ed8cf556b
ms.sourcegitcommit: 121f1b9cbd88faeba60dc9b475f9c0647cdc933c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/06/2021
ms.locfileid: "115691435"
---
# <a name="create-a-work-account-that-links-your-company-to-your-partner-center-account"></a>Skapa ett arbetskonto som länkar ditt företag till ditt Partnercenter-konto

**Lämpliga roller:** Globala | Administratör för användarhantering

## <a name="why-you-need-a-work-account"></a>Varför du behöver ett arbetskonto

Microsoft kräver att du länkar ditt företags arbetskonto till ditt nya Partnercenter-konto. Med länken kan dina kontoanvändare logga in på Partnercenter med sina användarnamn och lösenord för arbetskontot.

## <a name="the-work-account-email-address"></a>Arbetskontots e-postadress

Ditt arbetskonto eller arbets-e-postadress är den e-postadress som ditt företag har angett. E-postadressen för ett arbetskonto har vanligtvis formatet `you@yourcompany.com` . Personliga e-postadresser som Hotmail, Gmail eller Yahoo fungerar inte som e-post och kan inte användas för ditt Partnercenter-konto.

Om du har mer än en giltig e-postadress till arbetet använder du den som är kopplad till företagets huvudkontor i stället för till den regionala avdelningen. Använd till exempel din e-postadress i stället för `contoso.com` `contoso.uk` adressen.

> [!NOTE]  
> Innan du använder ett befintligt arbetskonto bör du tänka på hur många användare i arbetskontot som behöver åtkomst till Partnercenter. Om du har användare i arbetskontot som inte behöver åtkomst till Partnercenter kan du överväga att skapa ett nytt konto för endast de användare som behöver åtkomst till Partnercenter.

## <a name="not-sure-if-your-company-already-has-a-work-account"></a>Är du osäker på om ditt företag redan har ett arbetskonto?

Om du inte är säker på om ditt företag har ett arbetskonto följer du dessa steg för att kontrollera. Om du har en aktiv prenumeration på Microsoft Azure eller Office 365 har du redan ett arbetskonto.

1. Logga in på [Azure-portalen](https://portal.azure.com).

2. Välj Azure Active Directory på navigeringsmenyn och välj **Custom Domain Namn.**

3. Om du redan har ett arbetskonto visas domännamnet.

Om ditt företag inte redan har ett arbetskonto kan du skapa ett under registreringsprocessen.

Diagrammet nedan innehåller steg för flera vanliga scenarier:

- avgöra om du har ett arbetskonto
- bestämma hur du ska logga in på ditt arbetskonto
- avgöra om du behöver skapa ett nytt arbetskonto

:::image type="content" source="images/onboardingAADFlow.png" lightbox="images/onboardingAADFlow.png" alt-text="Har du ett arbetskonto eller behöver du skapa ett?":::

Mer information om hur du lägger till domäner i Azure AD finns i [Lägga till eller associera en domän i Azure AD](/azure/active-directory/active-directory-add-domain)

## <a name="about-microsoft-azure"></a>Om Microsoft Azure

Microsoft Azure är en offentlig molnplattform som företag kan använda för att skapa, distribuera och hantera program i ett globalt nätverk med Microsoft-hanterade datacenter. Företag använder Azure för att skapa en virtuell IT-infrastruktur med virtuella funktioner, eller tjänster, i stället för fysiska datorer.

När du köper en Azure-prenumeration hyr du i princip ett dedikerat, skyddat utrymme i det offentliga Azure-molnet. Det skiljer sig inte så mycket från att hyra ett golv i en kontorsbyggnad för ditt företags fysiska verksamhet. Ditt företag är en klientorganisation för kontorsbyggnadens ägare.

Ett Azure-arbetskonto är en dedikerad och isolerad virtuell representation av ditt företag i det offentliga Azure-molnet som skapas åt dig när du prenumererar på en Microsoft-molntjänst som Azure, Microsoft Intune eller Office 365.

Ditt arbetskonto är värd för dina Azure AD-användare och informationen om dem – deras lösenord, profildata, behörigheter och så vidare. Arbetskontot innehåller också grupper, program och annan information som rör ett företag och dess säkerhet.

## <a name="next-steps"></a>Nästa steg

- [Hantera ditt Partnercenter-konto](partner-center-account-setup.md)
- [Spåra verifieringsstatus](verification-responses.md)
