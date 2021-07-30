---
title: Ge användarna multifaktorautentisering
ms.topic: how-to
ms.date: 12/15/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-enroll
description: Lär dig hur du ställer in dina anställda med MFA
author: vijvala
ms.author: vijvala
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: ee457193a23de0601b60b2291cdee985aceaaeb8
ms.sourcegitcommit: ad1af627f5ee6b6e3a70655f90927e932cf4c985
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 07/29/2021
ms.locfileid: "114846119"
---
# <a name="set-up-your-users-with-multi-factor-authentication"></a>Ge användarna multifaktorautentisering

**Lämpliga roller:** Global administratör

Större sekretessskydd och säkerhet är bland våra högsta prioriteter. Vi vet att det bästa försvaret är att förebygga och att vi bara är lika starka som vår svagaste länk. Därför behöver vi att alla i vårt ekosystem agerar och ser till att rätt säkerhetsskydd finns på plats. Vi rekommenderar starkt att alla partner aktiverar multifaktorautentisering (MFA) för sina användare i partnerklientorganisationen. 

## <a name="add-multi-factor-authentication-for-your-users"></a>Lägga till multifaktorautentisering för dina användare

Du måste vara global administratör för ditt företag för att slutföra den här uppgiften.

Det är enklast att aktivera MFA för dina användare när du lägger till dem i din Azure AD-klientorganisation.

1. Logga in [på Azure Portal](https://portal.azure.com) och gå sedan till **Användarhantering.**
1. Välj **Multi-Factor Authentication**.
1. Välj den användare som du vill aktivera och välj sedan **Aktivera.**

Detta aktiverar MFA för den här användaren. Aktiverat innebär att användaren uppmanas att konfigurera sin MFA-verifiering när de loggar in för första gången. Därefter uppmanas de vid inloggningen att ange en kod som skickas till dem antingen via e-post eller SMS (beroende på vilket de har ställt in).  

:::image type="content" source="images/multi-factor-authentication/security-verification.png" alt-text="Ange hur du ska verifiera.":::

>[!NOTE]
>Du kan **tvinga** användarna att använda MFA genom att följa samma steg som ovan och välja **Framtvinga.** Mer information finns i [Aktivera Azure Multi-Factor Authentication per användare för att skydda inloggningshändelser.](/azure/active-directory/authentication/howto-mfa-userstates) 

Alla användare börjar med **Inaktiverad**. När du registrerar användare i per användare Azure Active Directory Multi-Factor Authentication ändras deras tillstånd till **Aktiverad.** När aktiverad användare loggar in och slutför registreringen ändras deras tillstånd till **Framtvingad**. 

## <a name="next-steps"></a>Nästa steg

- [Tilldela roller och behörigheter till användare](permissions-overview.md)