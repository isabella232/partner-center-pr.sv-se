---
title: Skapa användarkonton och tilldela roller
description: Alla medarbetare måste tilldelas en roll innan de kan komma åt Partnercenter. Lär dig hur du skapar användarkonton, tilldelar roller och anger behörigheter.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-account
ms.custom: contperf-fy21q2
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.date: 10/12/2020
ms.openlocfilehash: 7aacaa04beb0aaa80ff40b1ba5bb2bb419c464904379e6737e55b387cce3bf3d
ms.sourcegitcommit: 121f1b9cbd88faeba60dc9b475f9c0647cdc933c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/06/2021
ms.locfileid: "115691097"
---
# <a name="create-user-accounts"></a>Skapa användarkonton  

**Lämpliga roller:** Kontoadministratörsroller | Global | Administratör för användarhantering

Skapa användarkonton för anställda som behöver åtkomst till Partnercenter. Dessa uppgifter måste utföras av användarhanteringsadministratören, kontoadministratören eller den globala administratören. Användaren som utför dessa uppgifter måste också tilldelas AAD Azure Active Directory rollerna (Användaradministratör) eller Global administratör. Mer information om AAD-roller finns i [Administratörsrollbehörigheter i Azure Active Directory](/azure/active-directory/users-groups-roles/directory-assign-admin-roles).

## <a name="add-a-new-user"></a>Lägga till en ny användare

1. Från ikonen **Inställningar** längst upp till höger i Partnercenter väljer du **Kontoinställningar** och sedan **Användarhantering.**

2. Välj **Lägg till användare**.

3. Ange användarens fullständiga namn och unika e-postadress.

4. Välj typ av agent och/eller den typ av administratör som du vill tilldela till användaren. Åtkomst till Partnercenter är rollbaserad, så du kan tilldela behörigheter för att anpassa användarens vy så att endast de funktioner som användaren behöver för att slutföra specifika uppgifter visas.  Om användarna vill ha en rolltilldelning kan de hitta globala administratörer att kontakta genom att gå till **Användarhantering och** filtrering på global administratör.

5. Välj **Lägg till** när du vill skapa användarkontot. Bekräfta användarens information på nästa sida.

> [!IMPORTANT]  
> Anteckna den nya användarens inloggningsinformation som visas på den här sidan. Se till att kopiera och skicka den här informationen till den nya användaren eftersom du inte kan komma åt den igen senare. 

Användaren måste logga in på Partnercenter med sitt användarnamn och tillfälliga lösenord. När användaren loggar in på Partnercenter för första gången uppmanas de att ändra sitt lösenord.

## <a name="assign-user-roles"></a>Tilldela användarroller

Om du vill arbeta i Partnercenter måste du ha en tilldelad roll.  För närvarande omfattar roller Azure Active Directory klientroller, Molnlösningsleverantör(CSP)-roller och icke-AAD-företagsroller. Ett enskilt företag kan ha behov av alla dessa roller.

>[!Important]
>Enskilda användare måste anges i din klientorganisation för att få åtkomst till Partnercenter. Rolltilldelningar ger ytterligare åtkomst.

## <a name="next-steps"></a>Nästa steg

- [Tilldela användarroller och behörigheter för anställda som behöver arbeta i Partnercenter](permissions-overview.md)
