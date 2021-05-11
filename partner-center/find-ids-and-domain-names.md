---
title: Hitta klientorganisations-ID, domännamn, användarobjekt-ID
ms.topic: how-to
ms.date: 11/06/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Lär dig hur du hittar ID:n i Azure Portal – en organisations Azure AD-klientorganisations-ID, domännamn eller specifikt användarobjekt-ID. Vissa uppgifter behöver den här informationen.
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOJULY.20
ms.openlocfilehash: 643b1eeb96a47ee4c438f733efe3be22234d02ff
ms.sourcegitcommit: e462f562e7f26b7d6870c22638a2a841499109d6
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 05/11/2021
ms.locfileid: "109740292"
---
# <a name="locate-important-ids-for-a-user"></a><span data-ttu-id="8749d-104">Hitta viktiga ID:er för en användare</span><span class="sxs-lookup"><span data-stu-id="8749d-104">Locate important IDs for a user</span></span>

<span data-ttu-id="8749d-105">**Lämpliga roller**</span><span class="sxs-lookup"><span data-stu-id="8749d-105">**Appropriate roles**</span></span>

- <span data-ttu-id="8749d-106">Global administratör</span><span class="sxs-lookup"><span data-stu-id="8749d-106">Global admin</span></span>

<span data-ttu-id="8749d-107">Den här artikeln beskriver hur du använder [Azure Portal](https://portal.azure.com/) för att hitta följande information för en användare:</span><span class="sxs-lookup"><span data-stu-id="8749d-107">This article describes how to use the [Azure portal](https://portal.azure.com/) to locate the following information for a user:</span></span>

- <span data-ttu-id="8749d-108">Det Microsoft Azure Active Directory (Azure AD) klientorganisations-ID:t för användarens organisation eller företag</span><span class="sxs-lookup"><span data-stu-id="8749d-108">The Microsoft Azure Active Directory (Azure AD) tenant ID of the user's organization or company</span></span>

- <span data-ttu-id="8749d-109">Det primära domännamnet för den organisation eller det företag som är associerat med Azure AD-klientorganisationen</span><span class="sxs-lookup"><span data-stu-id="8749d-109">The primary domain name of the organization or company associated with the Azure AD tenant</span></span>

- <span data-ttu-id="8749d-110">Användarobjektets ID</span><span class="sxs-lookup"><span data-stu-id="8749d-110">The user object ID</span></span>

## <a name="find-the-microsoft-azure-ad-tenant-id-and-primary-domain-name"></a><span data-ttu-id="8749d-111">Hitta Microsoft Azure AD klientorganisations-ID och primärt domännamn</span><span class="sxs-lookup"><span data-stu-id="8749d-111">Find the Microsoft Azure AD tenant ID and primary domain name</span></span>

<span data-ttu-id="8749d-112">Följ dessa steg för att hitta Azure AD-klientorganisations-ID:t eller det primära domännamnet i Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="8749d-112">Follow these steps to locate the Azure AD tenant ID or primary domain name within the Azure portal.</span></span> <span data-ttu-id="8749d-113">(Om du vill hitta ett klientorganisations-ID programmässigt kan du se [Hitta klient-ID med PowerShell eller CLI](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant#find-tenant-id-with-powershell).)</span><span class="sxs-lookup"><span data-stu-id="8749d-113">(If you'd like to find a tenant ID programmatically, see [Find tenant ID with PowerShell or CLI](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant#find-tenant-id-with-powershell).)</span></span>

> [!NOTE]
> <span data-ttu-id="8749d-114">Klientorganisations-ID:t kan kallas olika namn i olika program eller resurser.</span><span class="sxs-lookup"><span data-stu-id="8749d-114">The tenant ID may be called different names in different applications or resources.</span></span> <span data-ttu-id="8749d-115">Klientorganisations-ID:t kan till exempel kallas katalog-ID, Azure Active Directory-klientorganisation (Azure AD), Microsoft-ID eller för vissa rapporter, även *tenantguid*.</span><span class="sxs-lookup"><span data-stu-id="8749d-115">For example, the tenant ID may be referred to as the directory ID, the Azure Active Directory (Azure AD) tenant, Microsoft ID, or for certain reports, even the *tenantguid*.</span></span>

1. <span data-ttu-id="8749d-116">Logga in på [Azure-portalen](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="8749d-116">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>

2. <span data-ttu-id="8749d-117">Välj **Azure Active Directory** på menyn.</span><span class="sxs-lookup"><span data-stu-id="8749d-117">Select **Azure Active Directory** from the menu.</span></span>

   :::image type="content" source="images/id/1-find-id-azure-portal-home-screen.png" alt-text="Visar Azure Portal väljer Azure Active Directory på menyn.":::

3. <span data-ttu-id="8749d-119">En Azure Active Directory **översiktssida** visas.</span><span class="sxs-lookup"><span data-stu-id="8749d-119">An Azure Active Directory **Overview** page appears.</span></span> <span data-ttu-id="8749d-120">Om du vill hitta Azure AD-klientorganisations-ID:t eller det primära domännamnet letar du upp fältet **Klientorganisations-ID** och **fältet Primär** domän.</span><span class="sxs-lookup"><span data-stu-id="8749d-120">To find the Azure AD tenant ID or primary domain name, look for the **Tenant ID** field and the **Primary domain** field.</span></span> <span data-ttu-id="8749d-121">Dessa fält visas i avsnittet Klientinformation.</span><span class="sxs-lookup"><span data-stu-id="8749d-121">These fields appear in the Tenant information section.</span></span>

   :::image type="content" source="images/id/2-find-id-azure-portal-azure-ad-overview-tenant-id-partial-screen.png" alt-text="Visar sidan Översikt med två markerade fält, klientorganisations-ID och primärt domännamn.":::

4. <span data-ttu-id="8749d-123">Du hittar klientorganisations-ID:t i Azure Portal på några andra sätt.</span><span class="sxs-lookup"><span data-stu-id="8749d-123">You can find the tenant ID in the Azure portal in a few other ways.</span></span> <span data-ttu-id="8749d-124">Välj **Azure Active Directory** på menyn.</span><span class="sxs-lookup"><span data-stu-id="8749d-124">Select **Azure Active Directory** from the menu.</span></span> <span data-ttu-id="8749d-125">Leta sedan upp **avsnittet** Hantera på menyn och välj **Egenskaper.**</span><span class="sxs-lookup"><span data-stu-id="8749d-125">Then, locate the **Manage** section on the menu and select **Properties**.</span></span>

   <span data-ttu-id="8749d-126">Sidan Egenskaper visar också användarens associerade klientorganisations-ID.</span><span class="sxs-lookup"><span data-stu-id="8749d-126">The Properties page also displays the user's associated Tenant ID.</span></span>

   :::image type="content" source="images/id/3-find-id-azure-portal-aad-properties-tenant-id-partial.png" alt-text="Visar sidan Egenskaper med markerat fält för klientorganisations-ID.":::

## <a name="find-the-user-object-id"></a><span data-ttu-id="8749d-128">Hitta användarobjektets ID</span><span class="sxs-lookup"><span data-stu-id="8749d-128">Find the user object ID</span></span>

<span data-ttu-id="8749d-129">Att bara hitta domännamnet och klientorganisations-ID:t kanske inte alltid räcker.</span><span class="sxs-lookup"><span data-stu-id="8749d-129">Just finding the domain name and tenant ID may not always be enough.</span></span> <span data-ttu-id="8749d-130">Du kan också behöva hitta det specifika objekt-ID som tilldelats en användare.</span><span class="sxs-lookup"><span data-stu-id="8749d-130">You may also need to locate the specific object ID assigned to a user.</span></span> <span data-ttu-id="8749d-131">Följ dessa steg för att hitta en användares objekt-ID i Azure Portal:</span><span class="sxs-lookup"><span data-stu-id="8749d-131">Follow these steps to find a user's object ID in the Azure portal:</span></span>

1. <span data-ttu-id="8749d-132">Logga in på [Azure-portalen](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="8749d-132">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>

2. <span data-ttu-id="8749d-133">Välj **Azure Active Directory** på menyn.</span><span class="sxs-lookup"><span data-stu-id="8749d-133">Select **Azure Active Directory** from the menu.</span></span>

3. <span data-ttu-id="8749d-134">Leta upp **avsnittet** Hantera på menyn och välj sedan **Användare.**</span><span class="sxs-lookup"><span data-stu-id="8749d-134">Locate the **Manage** section on the menu, then select **Users**.</span></span>

      :::image type="content" source="images/id/4-find-id-azure-portal-aad-manage-users-option.png" alt-text="Visar Azure Active Directory meny med markerat alternativ Användare.":::

4. <span data-ttu-id="8749d-136">På sidan Användare skriver du användarens namn i sökrutan.</span><span class="sxs-lookup"><span data-stu-id="8749d-136">From the Users page, type the user's name in the search box.</span></span>

      :::image type="content" source="images/id/5-find-id-azure-portal-aad-all-users-search.png" alt-text="Visar sidan Användare med sökruta för att söka efter en viss användare.":::

5. <span data-ttu-id="8749d-138">Välj användarens namn där det visas i listan.</span><span class="sxs-lookup"><span data-stu-id="8749d-138">Select the user's name where it appears on the list.</span></span>  

      :::image type="content" source="images/id/6-find-id-azure-portal-select-user-name-partial.png" alt-text="Visar sidan Användare som visar en rad för den sökte användaren.":::

6. <span data-ttu-id="8749d-140">Leta upp avsnittet Identitet på användarens profilsida.</span><span class="sxs-lookup"><span data-stu-id="8749d-140">Locate the Identity section on the user's Profile page.</span></span> <span data-ttu-id="8749d-141">Fältet Objekt-ID visas här med användarens unika objekt-ID.</span><span class="sxs-lookup"><span data-stu-id="8749d-141">The Object ID field appears here with the user's unique object ID.</span></span>

      :::image type="content" source="images/id/7-find-id-azure-portal-aad-user-profile-object-id.png" alt-text="Visar sidan Användarprofil med avsnittet Identitet och ett markerat fält för Objekt-ID.":::

## <a name="next-steps"></a><span data-ttu-id="8749d-143">Nästa steg</span><span class="sxs-lookup"><span data-stu-id="8749d-143">Next steps</span></span>

- [<span data-ttu-id="8749d-144">Hitta ditt klientorganisations-ID programmatiskt med PowerShell eller CLI</span><span class="sxs-lookup"><span data-stu-id="8749d-144">Find your tenant ID programmatically with PowerShell or CLI</span></span>](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant)
- [<span data-ttu-id="8749d-145">Läs mer om användarprofiler i Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="8749d-145">Learn more about user profiles in Azure Active Directory</span></span>](/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)
- [<span data-ttu-id="8749d-146">Ta reda på hur partner kan se eller exportera kundinformation i Partnercenter</span><span class="sxs-lookup"><span data-stu-id="8749d-146">Find out how partners can see or export customer details in Partner Center</span></span>](see-your-customer-list.md)

