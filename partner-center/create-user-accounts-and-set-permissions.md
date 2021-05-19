---
title: Skapa användarkonton och tilldela roller
description: Varje medarbetare måste tilldelas en roll innan de kan komma åt Partnercenter. Lär dig hur du skapar användarkonton, tilldelar roller och anger behörigheter.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
ms.custom: contperf-fy21q2
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.date: 10/12/2020
ms.openlocfilehash: 9621f0bc3283d7d3b08e2ebac62b4e5d8c95a4d4
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 05/19/2021
ms.locfileid: "110148150"
---
# <a name="create-user-accounts"></a><span data-ttu-id="23877-104">Skapa användarkonton</span><span class="sxs-lookup"><span data-stu-id="23877-104">Create user accounts</span></span>  

<span data-ttu-id="23877-105">**Lämpliga roller:** Kontoadministratörsroller | Globala | Administratör för användarhantering</span><span class="sxs-lookup"><span data-stu-id="23877-105">**Appropriate roles**: Account admin | Global admin | User management admin</span></span>

<span data-ttu-id="23877-106">Skapa användarkonton för anställda som behöver åtkomst till Partnercenter.</span><span class="sxs-lookup"><span data-stu-id="23877-106">Create user accounts for employees who need access to the Partner Center.</span></span> <span data-ttu-id="23877-107">Dessa uppgifter måste utföras av användarhanteringsadministratören, kontoadministratören eller den globala administratören. Användaren som utför dessa uppgifter måste också tilldelas AAD Azure Active Directory rollerna (Användaradministratör) eller Global administratör.</span><span class="sxs-lookup"><span data-stu-id="23877-107">These tasks must be done by the user management admin, accounts admin, or the global admin. The user performing these tasks must also be assigned the Azure Active Directory (AAD) roles of User administrator or Global administrator.</span></span> <span data-ttu-id="23877-108">Mer information om AAD-roller finns i [Administratörsrollbehörigheter i Azure Active Directory](/azure/active-directory/users-groups-roles/directory-assign-admin-roles).</span><span class="sxs-lookup"><span data-stu-id="23877-108">For more information about AAD roles, see [Administrator role permissions in Azure Active Directory](/azure/active-directory/users-groups-roles/directory-assign-admin-roles).</span></span>

## <a name="add-a-new-user"></a><span data-ttu-id="23877-109">Lägga till en ny användare</span><span class="sxs-lookup"><span data-stu-id="23877-109">Add a new user</span></span>

1. <span data-ttu-id="23877-110">Från ikonen **Inställningar** längst upp till höger i Partnercenter väljer du **Kontoinställningar** och sedan **Användarhantering.**</span><span class="sxs-lookup"><span data-stu-id="23877-110">From the **Settings** icon at the top right of the Partner Center, select **Account settings** and then select **User management**.</span></span>

2. <span data-ttu-id="23877-111">Välj **Lägg till användare**.</span><span class="sxs-lookup"><span data-stu-id="23877-111">Select **Add user**.</span></span>

3. <span data-ttu-id="23877-112">Ange användarens fullständiga namn och unika e-postadress.</span><span class="sxs-lookup"><span data-stu-id="23877-112">Enter the user's full name and unique email address.</span></span>

4. <span data-ttu-id="23877-113">Välj typ av agent och/eller den typ av administratör som du vill tilldela till användaren.</span><span class="sxs-lookup"><span data-stu-id="23877-113">Select the type of agent and/or the type of admin you want to assign to the user.</span></span> <span data-ttu-id="23877-114">Åtkomst till Partnercenter är rollbaserad, så du kan tilldela behörigheter för att anpassa användarens vy så att endast de funktioner som användaren behöver för att slutföra specifika uppgifter visas.</span><span class="sxs-lookup"><span data-stu-id="23877-114">Partner Center access is role-based, so you can assign permissions to customize the user's view to show only the features the user needs to complete specific tasks.</span></span>  <span data-ttu-id="23877-115">Om användarna vill ha en rolltilldelning kan de hitta globala administratörer att kontakta genom att gå till **Användarhantering och** filtrering på global administratör.</span><span class="sxs-lookup"><span data-stu-id="23877-115">If users want a role assignment, they can find global admins to contact by going to **User management** and filtering on global admin.</span></span>

5. <span data-ttu-id="23877-116">Välj **Lägg till** när du vill skapa användarkontot.</span><span class="sxs-lookup"><span data-stu-id="23877-116">Select **Add** to create the user account.</span></span> <span data-ttu-id="23877-117">Bekräfta användarens information på nästa sida.</span><span class="sxs-lookup"><span data-stu-id="23877-117">Confirm the user's details on the next page.</span></span>

> [!IMPORTANT]  
> <span data-ttu-id="23877-118">Anteckna den nya användarens inloggningsinformation som visas på den här sidan.</span><span class="sxs-lookup"><span data-stu-id="23877-118">Make a note of the new user's sign-in information displayed on this page.</span></span> <span data-ttu-id="23877-119">Se till att kopiera och skicka den här informationen till den nya användaren eftersom du inte kan komma åt den igen senare.</span><span class="sxs-lookup"><span data-stu-id="23877-119">Be sure to copy and send this information to the new user as you will not be able to access it again later.</span></span> 

<span data-ttu-id="23877-120">Användaren måste logga in på Partnercenter med sitt användarnamn och tillfälliga lösenord.</span><span class="sxs-lookup"><span data-stu-id="23877-120">The user will need to sign in to the Partner Center with their user name and temporary password.</span></span> <span data-ttu-id="23877-121">När användaren loggar in på Partnercenter för första gången uppmanas de att ändra sitt lösenord.</span><span class="sxs-lookup"><span data-stu-id="23877-121">When the user signs in to the Partner Center for the first time, they are prompted to change their password.</span></span>

## <a name="assign-user-roles"></a><span data-ttu-id="23877-122">Tilldela användarroller</span><span class="sxs-lookup"><span data-stu-id="23877-122">Assign user roles</span></span>

<span data-ttu-id="23877-123">Om du vill arbeta i Partnercenter måste du ha en tilldelad roll.</span><span class="sxs-lookup"><span data-stu-id="23877-123">To work in the Partner Center, you must have an assigned role.</span></span>  <span data-ttu-id="23877-124">För närvarande omfattar roller Azure Active Directory klientroller, Molnlösningsleverantör-roller (CSP) och icke-AAD-företagsroller.</span><span class="sxs-lookup"><span data-stu-id="23877-124">Currently, roles include Azure Active Directory tenant roles, Cloud Solution Provider (CSP) roles, and non-AAD company roles.</span></span> <span data-ttu-id="23877-125">Ett enskilt företag kan ha behov av alla dessa roller.</span><span class="sxs-lookup"><span data-stu-id="23877-125">An individual company can have a need for all of these roles.</span></span>

>[!Important]
><span data-ttu-id="23877-126">Enskilda användare måste anges i din klientorganisation för att få åtkomst till Partnercenter.</span><span class="sxs-lookup"><span data-stu-id="23877-126">Individuals must be listed in your tenant to access Partner Center.</span></span> <span data-ttu-id="23877-127">Rolltilldelningar ger ytterligare åtkomst.</span><span class="sxs-lookup"><span data-stu-id="23877-127">Role assignments provide additional access.</span></span>

## <a name="next-steps"></a><span data-ttu-id="23877-128">Nästa steg</span><span class="sxs-lookup"><span data-stu-id="23877-128">Next steps</span></span>

- [<span data-ttu-id="23877-129">Tilldela användarroller och behörigheter för anställda som behöver arbeta i Partnercenter</span><span class="sxs-lookup"><span data-stu-id="23877-129">Assign users roles and permissions for employees needing to work in Partner Center</span></span>](permissions-overview.md)
