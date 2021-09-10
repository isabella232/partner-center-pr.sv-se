---
title: Skapa användarkonton och tilldela roller
description: Varje medarbetare måste tilldelas en roll innan de kan komma åt Partnercenter. Lär dig hur du skapar användarkonton, tilldelar roller och anger behörigheter.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-account
ms.custom: contperf-fy21q2
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.date: 10/12/2020
ms.openlocfilehash: 71a330356b6c4b3792086f1bc2823e0e067e04ae
ms.sourcegitcommit: 1161d5bcb345e368348c535a7211f0d353c5a471
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/09/2021
ms.locfileid: "123960316"
---
# <a name="create-user-accounts"></a>Skapa användarkonton  

**Lämpliga roller:** Kontoadministratörsroller | Globala | Administratör för användarhantering

Skapa användarkonton för anställda som behöver åtkomst till Partnercenter. Dessa uppgifter måste utföras av användarhanteringsadministratören, kontoadministratören eller den globala administratören. Användaren som utför dessa uppgifter måste också tilldelas AAD Azure Active Directory rollerna (Användaradministratör) eller Global administratör. Mer information om AAD-roller finns i [Administratörsrollbehörigheter i Azure Active Directory](/azure/active-directory/users-groups-roles/directory-assign-admin-roles).

## <a name="add-a-new-user"></a>Lägga till en ny användare

1. Från ikonen **Inställningar** längst upp till höger i Partnercenter väljer **du Kontoinställningar** och sedan **Användarhantering.**

2. Välj **Lägg till användare**.

3. Ange användarens fullständiga namn och unika e-postadress.

4. Välj typ av agent och/eller den typ av administratör som du vill tilldela till användaren. Åtkomst till Partnercenter är rollbaserad, så du kan tilldela behörigheter för att anpassa användarvyn så att endast de funktioner som användaren behöver för att slutföra specifika uppgifter visas.  Om användarna vill ha en rolltilldelning kan de hitta globala administratörer att kontakta genom att gå till **Användarhantering och** filtrering på global administratör.

5. Välj **Lägg till** när du vill skapa användarkontot. Bekräfta användarens information på nästa sida.

> [!IMPORTANT]  
> Anteckna den nya användarens inloggningsinformation som visas på den här sidan. Se till att kopiera och skicka den här informationen till den nya användaren eftersom du inte kommer att kunna komma åt den igen senare. 

Användaren måste logga in på Partnercenter med sitt användarnamn och tillfälliga lösenord. När användaren loggar in på Partnercenter för första gången uppmanas de att ändra sitt lösenord.

## <a name="assign-user-roles"></a>Tilldela användarroller

Om du vill arbeta i Partnercenter måste du ha en tilldelad roll.  För närvarande omfattar roller Azure Active Directory klientroller, Molnlösningsleverantör-roller (CSP) och icke-AAD-företagsroller. Ett enskilt företag kan ha ett behov av alla dessa roller.

>[!Important]
>Enskilda användare måste anges i din klientorganisation för att få åtkomst till Partnercenter. Rolltilldelningar ger ytterligare åtkomst.

## <a name="next-steps"></a>Nästa steg

- [Tilldela användarroller och behörigheter för anställda som behöver arbeta i Partnercenter](permissions-overview.md)
