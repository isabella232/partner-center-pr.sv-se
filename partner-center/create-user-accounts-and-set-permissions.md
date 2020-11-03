---
title: Skapa användar konton och tilldela roller
description: Varje medarbetare måste tilldelas en roll innan de kan komma åt Partner Center. Lär dig hur du skapar användar konton, tilldelar roller och anger behörigheter.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
ms.custom: contperfq2
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.date: 10/12/2020
ms.openlocfilehash: 41f7f68c61630daf30595e28bd5de52f5a5787c8
ms.sourcegitcommit: 940dad4527f51781f6f966e196b3aa08389613a2
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 10/13/2020
ms.locfileid: "92531852"
---
# <a name="create-user-accounts"></a><span data-ttu-id="f0558-104">Skapa användar konton</span><span class="sxs-lookup"><span data-stu-id="f0558-104">Create user accounts</span></span>  

<span data-ttu-id="f0558-105">**Lämpliga roller**</span><span class="sxs-lookup"><span data-stu-id="f0558-105">**Appropriate roles**</span></span>

- <span data-ttu-id="f0558-106">Kontoadministratör</span><span class="sxs-lookup"><span data-stu-id="f0558-106">Account admin</span></span>
- <span data-ttu-id="f0558-107">Global administratör</span><span class="sxs-lookup"><span data-stu-id="f0558-107">Global admin</span></span>
- <span data-ttu-id="f0558-108">Administratör för användar hantering</span><span class="sxs-lookup"><span data-stu-id="f0558-108">User management admin</span></span>

<span data-ttu-id="f0558-109">Skapa användar konton för medarbetare som behöver åtkomst till Partner Center.</span><span class="sxs-lookup"><span data-stu-id="f0558-109">Create user accounts for employees who need access to the Partner Center.</span></span> <span data-ttu-id="f0558-110">Dessa uppgifter måste utföras av administratör för användar hantering, konto administratör eller global administratör. Användaren som utför dessa uppgifter måste också tilldelas Azure Active Directory-roller (AAD) för användar administratör eller global administratör.</span><span class="sxs-lookup"><span data-stu-id="f0558-110">These tasks must be done by the user management admin, accounts admin, or the global admin. The user performing these tasks must also be assigned the Azure Active Directory (AAD) roles of User administrator or Global administrator.</span></span> <span data-ttu-id="f0558-111">Mer information om AAD-roller finns [i administratörs roll behörigheter i Azure Active Directory](/azure/active-directory/users-groups-roles/directory-assign-admin-roles).</span><span class="sxs-lookup"><span data-stu-id="f0558-111">For more information about AAD roles, see [Administrator role permissions in Azure Active Directory](/azure/active-directory/users-groups-roles/directory-assign-admin-roles).</span></span>

## <a name="add-a-new-user"></a><span data-ttu-id="f0558-112">Lägga till en ny användare</span><span class="sxs-lookup"><span data-stu-id="f0558-112">Add a new user</span></span>

1. <span data-ttu-id="f0558-113">Från **inställnings** ikonen längst upp till höger i Partner Center väljer du **konto inställningar** och väljer sedan **användar hantering** .</span><span class="sxs-lookup"><span data-stu-id="f0558-113">From the **Settings** icon at the top right of the Partner Center, select **Account settings** and then select **User management** .</span></span>

2. <span data-ttu-id="f0558-114">Välj **Lägg till användare** .</span><span class="sxs-lookup"><span data-stu-id="f0558-114">Select **Add user** .</span></span>

3. <span data-ttu-id="f0558-115">Ange användarens fullständiga namn och unika e-postadress.</span><span class="sxs-lookup"><span data-stu-id="f0558-115">Enter the user's full name and unique email address.</span></span>

4. <span data-ttu-id="f0558-116">Välj typ av agent och/eller vilken typ av administratör som du vill tilldela till användaren.</span><span class="sxs-lookup"><span data-stu-id="f0558-116">Select the type of agent and/or the type of admin you want to assign to the user.</span></span> <span data-ttu-id="f0558-117">Åtkomst till Partner Center är rollbaserad, så du kan tilldela behörigheter för att anpassa användarens vy så att bara de funktioner som användaren behöver för att slutföra vissa uppgifter visas.</span><span class="sxs-lookup"><span data-stu-id="f0558-117">Partner Center access is role-based, so you can assign permissions to customize the user's view to show only the features the user needs to complete specific tasks.</span></span>  <span data-ttu-id="f0558-118">Om användarna vill ha en roll tilldelning kan de hitta globala administratörer att kontakta genom att gå till **användar hantering** och filtrering på global administratör.</span><span class="sxs-lookup"><span data-stu-id="f0558-118">If users want a role assignment, they can find global admins to contact by going to **User management** and filtering on global admin.</span></span>

5. <span data-ttu-id="f0558-119">Välj **Lägg till** när du vill skapa användarkontot.</span><span class="sxs-lookup"><span data-stu-id="f0558-119">Select **Add** to create the user account.</span></span> <span data-ttu-id="f0558-120">Bekräfta användarens information på nästa sida.</span><span class="sxs-lookup"><span data-stu-id="f0558-120">Confirm the user's details on the next page.</span></span>

> [!IMPORTANT]  
> <span data-ttu-id="f0558-121">Anteckna den nya användarens inloggnings information som visas på den här sidan.</span><span class="sxs-lookup"><span data-stu-id="f0558-121">Make a note of the new user's sign-in information displayed on this page.</span></span> <span data-ttu-id="f0558-122">Se till att kopiera och skicka den här informationen till den nya användaren eftersom du inte kommer att kunna komma åt den igen senare.</span><span class="sxs-lookup"><span data-stu-id="f0558-122">Be sure to copy and send this information to the new user as you will not be able to access it again later.</span></span> 

<span data-ttu-id="f0558-123">Användaren måste logga in på Partner Center med sitt användar namn och tillfälliga lösen ord.</span><span class="sxs-lookup"><span data-stu-id="f0558-123">The user will need to sign in to the Partner Center with their user name and temporary password.</span></span> <span data-ttu-id="f0558-124">När användaren loggar in på Partner Center för första gången uppmanas de att ändra sina lösen ord.</span><span class="sxs-lookup"><span data-stu-id="f0558-124">When the user signs in to the Partner Center for the first time, they are prompted to change their password.</span></span>

## <a name="assign-user-roles"></a><span data-ttu-id="f0558-125">Tilldela användar roller</span><span class="sxs-lookup"><span data-stu-id="f0558-125">Assign user roles</span></span>

<span data-ttu-id="f0558-126">Du måste ha en tilldelad roll för att kunna arbeta i Partner Center.</span><span class="sxs-lookup"><span data-stu-id="f0558-126">To work in the Partner Center, you must have an assigned role.</span></span>  <span data-ttu-id="f0558-127">För närvarande inkluderar roller Azure Active Directory klient roller, CSP-roller (Cloud Solution Provider) och företags roller som inte är AAD-AAD.</span><span class="sxs-lookup"><span data-stu-id="f0558-127">Currently, roles include Azure Active Directory tenant roles, Cloud Solution Provider (CSP) roles, and non-AAD company roles.</span></span> <span data-ttu-id="f0558-128">Ett enskilt företag kan ha behov av alla dessa roller.</span><span class="sxs-lookup"><span data-stu-id="f0558-128">An individual company can have a need for all of these roles.</span></span>

>[!Important]
><span data-ttu-id="f0558-129">Individer måste anges i din klient organisation för att få åtkomst till Partner Center.</span><span class="sxs-lookup"><span data-stu-id="f0558-129">Individuals must be listed in your tenant to access Partner Center.</span></span> <span data-ttu-id="f0558-130">Roll tilldelningar ger ytterligare åtkomst.</span><span class="sxs-lookup"><span data-stu-id="f0558-130">Role assignments provide additional access.</span></span>

## <a name="next-steps"></a><span data-ttu-id="f0558-131">Nästa steg</span><span class="sxs-lookup"><span data-stu-id="f0558-131">Next steps</span></span>

- [<span data-ttu-id="f0558-132">Tilldela användar roller och behörigheter för medarbetare som behöver arbeta i Partner Center</span><span class="sxs-lookup"><span data-stu-id="f0558-132">Assign users roles and permissions for employees needing to work in Partner Center</span></span>](permissions-overview.md)
