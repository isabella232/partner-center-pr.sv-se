---
title: Registrera i CSP-programmet
titleSuffix: Microsoft Cloud for US Government - Partner Center
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Läs om krav för CSP-program för partner som vill registrera sig i Cloud Solution Provider-programmet för Microsoft Cloud för amerikanska myndigheter.
author: mowrim
ms.author: mowrim
ms.localizationpriority: medium
ms.custom: SEOJUNE.20
ms.date: 10/05/2020
ms.openlocfilehash: 8fb6d3ec54b2cbcbc23a09cf122da0129afb7fbb
ms.sourcegitcommit: 8a4a3de728532533276a88b1fd40c82b7a4ebb15
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 10/06/2020
ms.locfileid: "92531829"
---
# <a name="enroll-in-the-cloud-solution-provider-program-for-microsoft-cloud-for-us-government"></a>Registrera dig i Cloud Solution Provider-programmet för Microsoft Cloud för amerikanska myndigheter

**Gäller för**

- Partner Center för Microsoft Cloud för amerikanska myndigheter

**Lämpliga roller**

- Global administratör

Microsoft-partner kan nu sälja Microsofts moln lösningar och tjänster till amerikanska federala, statliga, lokala och stambaserad entiteter via Cloud Solution Provider program (CSP) för Microsoft Cloud för amerikanska myndigheter.

Microsoft Cloud för amerikanska myndigheter tillhandahåller en privat, dedikerad och isolerad instans av Microsoft Azure som uppfyller de amerikanska myndigheternas krav på data säkerhet, sekretess och efterlevnad. Ditt företag måste uppfylla Microsofts krav på behörighet att delta i CSP-programmet för Microsoft Cloud för amerikanska myndigheter. Mer information finns i [partner Center för Microsoft Cloud för amerikanska myndigheter](partner-center-for-microsoft-us-govt-cloud.md).

## <a name="before-you-begin"></a>Innan du börjar

Innan du kan registrera dig i CSP-programmet för Microsoft Cloud för amerikanska myndigheter, måste vi kontrol lera att ditt företag uppfyller kraven för att sälja till amerikanska myndighets organisationer. Innan du startar registrerings processen ska du fylla i [formuläret för moln validering i Microsoft-myndigheter](https://azuregov.microsoft.com/csp) så att vi kan verifiera ditt företags berättigande. När vi har verifierat ditt företags berättigande ger vi dig en Azure Active Directory (Azure AD)-klient som är speciell för Microsoft Cloud för amerikanska myndigheter.  

Om du vill skapa ett partner Center-konto och registrera dig i CSP för Microsoft Cloud för amerikanska myndigheter måste du ange följande information (du kanske vill samla in den här informationen innan du startar registrerings processen):

- Autentiseringsuppgifter för global administratör för din organisations nya Azure AD-klient för Microsoft Cloud för amerikanska myndigheter
- Organisationens Microsoft Partner Network-ID (MPN)
- En företags adress i USA

> [!IMPORTANT]  
> Om du har ett befintligt konto i Partner Center och vill registrera dig i CSP för Microsoft Cloud för amerikanska myndigheter, måste du skapa ett nytt, separat konto som är specifikt för den amerikanska myndighets marknaden.

## <a name="how-to-enroll"></a>Så här registrerar du

### <a name="step-1---create-a-partner-center-account-for-microsoft-cloud-for-us-government"></a>Steg 1 – Skapa ett partner Center-konto för Microsoft Cloud för amerikanska myndigheter

1. Starta registreringen [här](https://partnercenter.microsoft.com/register/resellerusgjoinnow).

2. Logga in med autentiseringsuppgifter för global administratör för din organisations Azure AD-klient för Microsoft Cloud för amerikanska myndigheter. Om din organisation inte har något konto för den här portalen kan du begära en genom att fylla i [formuläret för moln validering från Microsoft-myndigheter](https://azuregov.microsoft.com/csp).

### <a name="step-2---apply-to-participate-in-the-cloud-solution-provider-program-for-microsoft-cloud-for-us-government"></a>Steg 2 – tillämpa på delta i Cloud Solution Provider-programmet för Microsoft Cloud för amerikanska myndigheter

1. Fyll i information som saknas i registrerings formuläret, inklusive ditt Microsoft Partner Network-ID och din organisations kund information.

2. Välj **Godkänn och fortsätt** . Det kan ta flera dagar att granska ditt program. Vi skickar e-post när vi har slutfört vår granskning.

   > [!IMPORTANT]
   > Genom att välja **Godkänn och fortsätt** , bekräftar du att du har behörighet att agera för din organisations räkning och att du godkänner att Microsoft kan köra en kontroll av en bakgrund i bakgrunden innan du granskar organisationens program för moln lösnings leverantör.

### <a name="step-3---sign-the-reseller-agreement-for-microsoft-cloud-for-us-government"></a>Steg 3 – signera åter försäljar avtalet för Microsoft Cloud för amerikanska myndigheter

1. Logga in på Partner Center för Microsoft Cloud för amerikanska myndigheter med hjälp av länken i e-postmeddelandet om program godkännande.

2. På sidan **avtal** läser du villkoren, och om du samtycker till det väljer du **Godkänn och fortsätter** att signera åter försäljarens avtal digitalt för Microsoft Cloud för amerikanska myndigheter. Det kan ta flera timmar att skapa ditt konto. Du kan logga ut från Partner Center för Microsoft Cloud för amerikanska myndigheter och sedan logga in igen senare.

### <a name="step-4---assign-users-to-the-admin-agent-role-in-the-microsoft-azure-admin-portal-for-microsoft-cloud-for-us-government"></a>Steg 4 – tilldela användare rollen admin agent i Microsoft Azure admin-portalen för Microsoft Cloud för amerikanska myndigheter

Microsoft Cloud för amerikanska myndigheter tillhandahåller en separat instans av Microsoft Azure som uppfyller myndigheternas krav på efterlevnad, säkerhet och sekretess. För att administratörer ska kunna hantera användare och licenser i Microsoft Azure-portalen måste du tilldela rollen som administratörs agent manuellt.

> [!NOTE]
> När du har tilldelat användare rollen som administratörs agent kommer de att kunna komma åt kund listan på sidan **kunder** och [lägga till nya kunder](add-a-new-customer.md).

1. Logga in på Microsoft Azure Admin Portal på [https://portal.azure.us/](https://portal.azure.us/) .

2. Tilldela rollen admin agent till lämpliga användare i din organisation. För att göra detta måste du lägga till dessa användare i den inbyggda **AdminAgent** -gruppen. Mer information om hur du gör detta finns [i Hantera medlemmar för en grupp i Azure Active Directory](/azure/active-directory/active-directory-groups-members-azure-portal) .

## <a name="connect-with-us"></a>Anslut till oss

- Har du några frågor? Skicka e-post till oss azgovcsp@microsoft.com

- Delta i [Yammer](https://www.yammer.com/cloudpartnercommunity/#/threads/inGroup?type=in_group&feedId=11509777)

## <a name="next-steps"></a>Nästa steg

- [Partner Center för Microsoft Cloud för amerikanska myndigheter](partner-center-for-microsoft-us-govt-cloud.md)

- [Hantering av användare och licenser i Partner Center för Microsoft Cloud för amerikanska myndigheter](user-management-in-partner-center-for-microsoft-us-govt-cloud.md)