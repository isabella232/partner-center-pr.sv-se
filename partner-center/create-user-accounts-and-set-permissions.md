---
title: Skapa användar konton och tilldela roller
description: Varje medarbetare måste tilldelas en roll innan de kan komma åt Partner Center. Lär dig hur du skapar användar konton, tilldelar roller och anger behörigheter.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
ms.custom: contperf-fy21q2
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.date: 10/12/2020
ms.openlocfilehash: c8fad4432f9aabba69877d80038ec9e2665c639d
ms.sourcegitcommit: 4e36d1a4ca2f074b55f9b9a08e300734eae1f06d
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 12/15/2020
ms.locfileid: "97492542"
---
# <a name="create-user-accounts"></a>Skapa användarkonton  

**Lämpliga roller**

- Kontoadministratör
- Global administratör
- Administratör för användar hantering

Skapa användar konton för medarbetare som behöver åtkomst till Partner Center. Dessa uppgifter måste utföras av administratör för användar hantering, konto administratör eller global administratör. Användaren som utför dessa uppgifter måste också tilldelas Azure Active Directory-roller (AAD) för användar administratör eller global administratör. Mer information om AAD-roller finns [i administratörs roll behörigheter i Azure Active Directory](/azure/active-directory/users-groups-roles/directory-assign-admin-roles).

## <a name="add-a-new-user"></a>Lägga till en ny användare

1. Från **inställnings** ikonen längst upp till höger i Partner Center väljer du **konto inställningar** och väljer sedan **användar hantering**.

2. Välj **Lägg till användare**.

3. Ange användarens fullständiga namn och unika e-postadress.

4. Välj typ av agent och/eller vilken typ av administratör som du vill tilldela till användaren. Åtkomst till Partner Center är rollbaserad, så du kan tilldela behörigheter för att anpassa användarens vy så att bara de funktioner som användaren behöver för att slutföra vissa uppgifter visas.  Om användarna vill ha en roll tilldelning kan de hitta globala administratörer att kontakta genom att gå till **användar hantering** och filtrering på global administratör.

5. Välj **Lägg till** när du vill skapa användarkontot. Bekräfta användarens information på nästa sida.

> [!IMPORTANT]  
> Anteckna den nya användarens inloggnings information som visas på den här sidan. Se till att kopiera och skicka den här informationen till den nya användaren eftersom du inte kommer att kunna komma åt den igen senare. 

Användaren måste logga in på Partner Center med sitt användar namn och tillfälliga lösen ord. När användaren loggar in på Partner Center för första gången uppmanas de att ändra sina lösen ord.

## <a name="assign-user-roles"></a>Tilldela användar roller

Du måste ha en tilldelad roll för att kunna arbeta i Partner Center.  För närvarande inkluderar roller Azure Active Directory klient roller, CSP-roller (Cloud Solution Provider) och företags roller som inte är AAD-AAD. Ett enskilt företag kan ha behov av alla dessa roller.

>[!Important]
>Individer måste anges i din klient organisation för att få åtkomst till Partner Center. Roll tilldelningar ger ytterligare åtkomst.

## <a name="next-steps"></a>Nästa steg

- [Tilldela användar roller och behörigheter för medarbetare som behöver arbeta i Partner Center](permissions-overview.md)
