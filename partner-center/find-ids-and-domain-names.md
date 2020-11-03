---
title: Hitta klient-ID, domän namn, användar objekt-ID
ms.topic: how-to
ms.date: 09/16/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 'Lär dig hitta ID: n i Azure Portal-en organisations Azure AD-klient-ID, domän namn eller ett särskilt användar objekt-ID. Vissa uppgifter behöver den här informationen.'
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOJULY.20
ms.openlocfilehash: 4a3695079a9d5b0b3c66b7c2eda52a31888a6660
ms.sourcegitcommit: 3158b0de261539694e37e433c763afa4067e36fb
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/17/2020
ms.locfileid: "92531461"
---
# <a name="locate-important-ids-for-a-user"></a><span data-ttu-id="77a3b-104">Hitta viktiga ID: n för en användare</span><span class="sxs-lookup"><span data-stu-id="77a3b-104">Locate important IDs for a user</span></span>

<span data-ttu-id="77a3b-105">Den här artikeln beskriver hur du använder [Azure Portal](https://portal.azure.com/) för att hitta följande information för en användare:</span><span class="sxs-lookup"><span data-stu-id="77a3b-105">This article describes how to use the [Azure portal](https://portal.azure.com/) to locate the following information for a user:</span></span>

- <span data-ttu-id="77a3b-106">Microsoft Azure Active Directory (Azure AD) klient-ID för användarens organisation eller företag</span><span class="sxs-lookup"><span data-stu-id="77a3b-106">The Microsoft Azure Active Directory (Azure AD) tenant ID of the user's organization or company</span></span>

- <span data-ttu-id="77a3b-107">Det primära domän namnet för den organisation eller det företag som är associerat med Azure AD-klienten</span><span class="sxs-lookup"><span data-stu-id="77a3b-107">The primary domain name of the organization or company associated with the Azure AD tenant</span></span>

- <span data-ttu-id="77a3b-108">Användar objektets ID</span><span class="sxs-lookup"><span data-stu-id="77a3b-108">The user object ID</span></span>

## <a name="find-the-microsoft-azure-ad-tenant-id-and-primary-domain-name"></a><span data-ttu-id="77a3b-109">Hitta Microsoft Azure AD klient-ID och primärt domän namn</span><span class="sxs-lookup"><span data-stu-id="77a3b-109">Find the Microsoft Azure AD tenant ID and primary domain name</span></span>

<span data-ttu-id="77a3b-110">Följ de här stegen för att hitta Azure AD-klient-ID: t eller det primära domän namnet inom Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="77a3b-110">Follow these steps to locate the Azure AD tenant ID or primary domain name within the Azure portal.</span></span>

> [!NOTE]
> <span data-ttu-id="77a3b-111">Klient-ID: t kan anropas med olika namn i olika program eller resurser.</span><span class="sxs-lookup"><span data-stu-id="77a3b-111">The tenant ID may be called different names in different applications or resources.</span></span> <span data-ttu-id="77a3b-112">Klient-ID: t kan till exempel kallas katalog-ID, Azure Active Directory (Azure AD)-klient, Microsoft-ID eller för vissa rapporter, även *tenantguid* .</span><span class="sxs-lookup"><span data-stu-id="77a3b-112">For example, the tenant ID may be referred to as the directory ID, the Azure Active Directory (Azure AD) tenant, Microsoft ID, or for certain reports, even the *tenantguid* .</span></span>

1. <span data-ttu-id="77a3b-113">Logga in på [Azure-portalen](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="77a3b-113">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>

2. <span data-ttu-id="77a3b-114">Välj **Azure Active Directory** på menyn.</span><span class="sxs-lookup"><span data-stu-id="77a3b-114">Select **Azure Active Directory** from the menu.</span></span>

   :::image type="content" source="images/id/1-find-id-azure-portal-home-screen.png" alt-text="Visar Azure Portal att välja alternativet Azure Active Directory på menyn.":::

3. <span data-ttu-id="77a3b-116">Sidan **Översikt över** Azure Active Directory visas.</span><span class="sxs-lookup"><span data-stu-id="77a3b-116">An Azure Active Directory **Overview** page appears.</span></span> <span data-ttu-id="77a3b-117">Du hittar Azure AD-klient-ID: t eller det primära domän namnet genom att leta efter **klient-ID-** fältet och det **primära domän** fältet.</span><span class="sxs-lookup"><span data-stu-id="77a3b-117">To find the Azure AD tenant ID or primary domain name, look for the **Tenant ID** field and the **Primary domain** field.</span></span> <span data-ttu-id="77a3b-118">Dessa fält visas i avsnittet klient information.</span><span class="sxs-lookup"><span data-stu-id="77a3b-118">These fields appear in the Tenant information section.</span></span>

   :::image type="content" source="images/id/2-find-id-azure-portal-azure-ad-overview-tenant-id-partial-screen.png" alt-text="Visar översikts sidan med två markerade fält, klient-ID och primärt domän namn.":::

4. <span data-ttu-id="77a3b-120">Du kan hitta klient-ID: t i Azure Portal på några andra sätt.</span><span class="sxs-lookup"><span data-stu-id="77a3b-120">You can find the tenant ID in the Azure portal in a few other ways.</span></span> <span data-ttu-id="77a3b-121">Välj **Azure Active Directory** på menyn.</span><span class="sxs-lookup"><span data-stu-id="77a3b-121">Select **Azure Active Directory** from the menu.</span></span> <span data-ttu-id="77a3b-122">Leta sedan upp avsnittet **Hantera** på menyn och välj **Egenskaper** .</span><span class="sxs-lookup"><span data-stu-id="77a3b-122">Then, locate the **Manage** section on the menu and select **Properties** .</span></span>

   <span data-ttu-id="77a3b-123">På sidan Egenskaper visas även användarens associerade klient-ID.</span><span class="sxs-lookup"><span data-stu-id="77a3b-123">The Properties page also displays the user's associated Tenant ID.</span></span>

   :::image type="content" source="images/id/3-find-id-azure-portal-aad-properties-tenant-id-partial.png" alt-text="Visar sidan Egenskaper med det markerade klient-ID-fältet.":::

## <a name="find-the-user-object-id"></a><span data-ttu-id="77a3b-125">Hitta användar objektets ID</span><span class="sxs-lookup"><span data-stu-id="77a3b-125">Find the user object ID</span></span>

<span data-ttu-id="77a3b-126">Det är inte alltid tillräckligt med att hitta domän namnet och klient-ID: t.</span><span class="sxs-lookup"><span data-stu-id="77a3b-126">Just finding the domain name and tenant ID may not always be enough.</span></span> <span data-ttu-id="77a3b-127">Du kan också behöva hitta det objekt-ID som tilldelats till en användare.</span><span class="sxs-lookup"><span data-stu-id="77a3b-127">You may also need to locate the specific object ID assigned to a user.</span></span> <span data-ttu-id="77a3b-128">Följ de här stegen för att hitta en användares objekt-ID i Azure Portal:</span><span class="sxs-lookup"><span data-stu-id="77a3b-128">Follow these steps to find a user's object ID in the Azure portal:</span></span>

1. <span data-ttu-id="77a3b-129">Logga in på [Azure-portalen](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="77a3b-129">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>

2. <span data-ttu-id="77a3b-130">Välj **Azure Active Directory** på menyn.</span><span class="sxs-lookup"><span data-stu-id="77a3b-130">Select **Azure Active Directory** from the menu.</span></span>

3. <span data-ttu-id="77a3b-131">Leta upp avsnittet **Hantera** på menyn och välj sedan **användare** .</span><span class="sxs-lookup"><span data-stu-id="77a3b-131">Locate the **Manage** section on the menu, then select **Users** .</span></span>

      :::image type="content" source="images/id/4-find-id-azure-portal-aad-manage-users-option.png" alt-text="Visar Azure Active Directory menyn med alternativet markerat, användare.":::

4. <span data-ttu-id="77a3b-133">På sidan användare anger du användarens namn i sökrutan.</span><span class="sxs-lookup"><span data-stu-id="77a3b-133">From the Users page, type the user's name in the search box.</span></span>

      :::image type="content" source="images/id/5-find-id-azure-portal-aad-all-users-search.png" alt-text="Visar sidan användare med sökrutan för att söka efter en speciell användare.":::

5. <span data-ttu-id="77a3b-135">Välj användarens namn där det visas i listan.</span><span class="sxs-lookup"><span data-stu-id="77a3b-135">Select the user's name where it appears on the list.</span></span>  

      :::image type="content" source="images/id/6-find-id-azure-portal-select-user-name-partial.png" alt-text="Visar användar sidan som visar en rad för den genomsökta användaren.":::

6. <span data-ttu-id="77a3b-137">Leta upp avsnittet identitet på användarens profil sida.</span><span class="sxs-lookup"><span data-stu-id="77a3b-137">Locate the Identity section on the user's Profile page.</span></span> <span data-ttu-id="77a3b-138">Fältet objekt-ID visas här med användarens unika objekt-ID.</span><span class="sxs-lookup"><span data-stu-id="77a3b-138">The Object ID field appears here with the user's unique object ID.</span></span>

      :::image type="content" source="images/id/7-find-id-azure-portal-aad-user-profile-object-id.png" alt-text="Visar sidan användar profil med avsnittet identitet och ett markerat fält för objekt-ID.":::

## <a name="next-steps"></a><span data-ttu-id="77a3b-140">Nästa steg</span><span class="sxs-lookup"><span data-stu-id="77a3b-140">Next steps</span></span>

- [<span data-ttu-id="77a3b-141">Lär dig mer om användar profiler i Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="77a3b-141">Learn more about user profiles in Azure Active Directory</span></span>](/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)
- [<span data-ttu-id="77a3b-142">Ta reda på hur partner kan se eller exportera kund information i Partner Center</span><span class="sxs-lookup"><span data-stu-id="77a3b-142">Find out how partners can see or export customer details in Partner Center</span></span>](see-your-customer-list.md)