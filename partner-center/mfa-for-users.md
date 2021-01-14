---
title: Ge användarna multifaktorautentisering
ms.topic: how-to
ms.date: 12/15/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Lär dig hur du ställer in dina anställda med MFA
author: vijvala
ms.author: vijvala
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: f42c97be88a1a505f7e0ae9b8af0d4a9167d8447
ms.sourcegitcommit: 531151a5dbc999b8b7de478d72ea115e6d579ff1
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 01/13/2021
ms.locfileid: "98182383"
---
# <a name="set-up-your-users-with-multi-factor-authentication"></a>Ge användarna multifaktorautentisering

**Lämpliga roller**

- Global administratör

Större Sekretess skydd och säkerhet är bland våra främsta prioriteringar. Vi vet att det bästa skyddet är förebyggande och att vi bara är lika starka som vår svagaste länk. Därför behöver vi alla i vårt eko system för att agera och se till att lämpliga säkerhets skydd är på plats. Vi rekommenderar starkt att alla partners aktiverar Multi-Factor Authentication (MFA) för sina användare i sin partner klient organisation. 

## <a name="add-multi-factor-authentication-for-your-users"></a>Lägg till Multi-Factor Authentication för dina användare

Du måste vara den globala administratören för ditt företag för att slutföra den här uppgiften.

Det är enklast att aktivera MFA för dina användare när du lägger till dem i din Azure AD-klient.

1. Logga in på [Azure Portal](https://portal.azure.com) och gå sedan till **användar hantering**.
1. Välj **Multi-Factor Authentication**.
1. Välj den användare som du vill aktivera och välj sedan **Aktivera**.

Detta aktiverar MFA för den här användaren. Aktive rad innebär att användaren uppmanas att ställa in sin MFA-verifiering när de loggar in för första gången. Därefter uppmanas han eller hon att ange en kod som skickas till dem antingen via e-post eller SMS (beroende på vilka de har ställt in).  

:::image type="content" source="images/MFA/securityverification.png" alt-text="Ange hur du vill verifiera":::

>[!NOTE]
>Du kan **tvinga** dina användare att använda MFA genom att använda samma steg som ovan och välja **tvinga**. Läs mer i [Aktivera Azure-Multi-Factor Authentication per användare för att skydda inloggnings händelser](/azure/active-directory/authentication/howto-mfa-userstates). 

Alla användare börjar vara **inaktiverade**. När du registrerar användare i Azure-Multi-Factor Authentication per användare, ändras deras status till **aktive rad**. När aktiverade användare loggar in och slutför registrerings processen ändras deras status till **tvingande**. 

## <a name="next-steps"></a>Nästa steg

- [Tilldela roller och behörigheter till användare](permissions-overview.md)