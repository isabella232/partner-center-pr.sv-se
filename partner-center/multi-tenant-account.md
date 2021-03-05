---
title: Lägga till klienter till ditt partner Center-konto
ms.topic: article
ms.date: 01/11/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Lär dig hur du lägger till, konsoliderar eller hanterar flera Azure AD-klienter i ditt partner Center-konto och lär dig varför du kanske vill göra det.
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 2f3094489f65b7164b4a55804047f9a4ab5f11cb
ms.sourcegitcommit: 79d2f00c352db61252e523f45abf93fe2a2742a5
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/04/2021
ms.locfileid: "102124813"
---
# <a name="add-and-manage-multiple-tenants-in-your-partner-center-account"></a><span data-ttu-id="4736d-103">Lägga till och hantera flera klienter i ditt partner Center-konto</span><span class="sxs-lookup"><span data-stu-id="4736d-103">Add and manage multiple tenants in your Partner Center account</span></span>


<span data-ttu-id="4736d-104">**Lämpliga roller**</span><span class="sxs-lookup"><span data-stu-id="4736d-104">**Appropriate roles**</span></span>

- <span data-ttu-id="4736d-105">Global administratör</span><span class="sxs-lookup"><span data-stu-id="4736d-105">Global admin</span></span>
- <span data-ttu-id="4736d-106">Kontoadministratör</span><span class="sxs-lookup"><span data-stu-id="4736d-106">Account admin</span></span>

<span data-ttu-id="4736d-107">Den här artikeln beskriver hur du konsoliderar flera Azure Active Directory (Azure AD)-klienter för företaget och sedan lägger till och hanterar dem i ditt partner Center-konto.</span><span class="sxs-lookup"><span data-stu-id="4736d-107">This article discusses how to consolidate multiple Azure Active Directory (Azure AD) tenants for your company and then add and manage them in your Partner Center account.</span></span> <span data-ttu-id="4736d-108">Det finns många skäl att göra det.</span><span class="sxs-lookup"><span data-stu-id="4736d-108">There are many reasons to do so.</span></span> <span data-ttu-id="4736d-109">Exempel:</span><span class="sxs-lookup"><span data-stu-id="4736d-109">For example:</span></span>

- <span data-ttu-id="4736d-110">Låt oss säga att ditt företag, contoso, har förvärvat ett annat företag, Fabrikam.</span><span class="sxs-lookup"><span data-stu-id="4736d-110">Let's say your company, Contoso, has acquired another company, Fabrikam.</span></span> <span data-ttu-id="4736d-111">Du vill att de två företagen ska vara åtskilda, men du vill att de nya anställda ska kunna använda Partner Center.</span><span class="sxs-lookup"><span data-stu-id="4736d-111">You want the two companies to remain separate, but you want the new employees to be able to use Partner Center.</span></span> <span data-ttu-id="4736d-112">I det här fallet associerar du det nya företagets Azure AD-klient med ditt partner globala konto (PGA).</span><span class="sxs-lookup"><span data-stu-id="4736d-112">In this case, you associate the new company's Azure AD tenant with your Partner global account (PGA).</span></span> <span data-ttu-id="4736d-113">Den här kopplingen gör det möjligt för användare i båda företagen att arbeta i Partner Center.</span><span class="sxs-lookup"><span data-stu-id="4736d-113">This association enables users in both companies to work in Partner Center.</span></span>

- <span data-ttu-id="4736d-114">Om du kör din verksamhet med fler än en klient (till exempel *contoso.com*, *contoso.uk* och *contoso.in*) kan du använda flera innehavare för att gruppera dem i samma PC-konto.</span><span class="sxs-lookup"><span data-stu-id="4736d-114">If you run your business with more than one tenant (for example, *contoso.com*, *contoso.uk*, and *contoso.in*), you can use multitenancy to group them in the same PC account.</span></span>

- <span data-ttu-id="4736d-115">Om rikt linjerna för sammanslagning och förvärv kräver att du arbetar med klienter för båda företagen, använder du både *constoso.com* -och *fabrikam.com* -klienterna.</span><span class="sxs-lookup"><span data-stu-id="4736d-115">If mergers and acquisitions guidelines require you to work with tenants of both companies, you would use both the *constoso.com* and *fabrikam.com* tenants.</span></span>

- <span data-ttu-id="4736d-116">Användare av någon av klienterna måste kunna:</span><span class="sxs-lookup"><span data-stu-id="4736d-116">Users of any of the tenants need to be able to:</span></span>
    * <span data-ttu-id="4736d-117">Få åtkomst till Partner Center för utbildning, digital hämtning eller Microsoft Certified Professional (MCP)-Association.</span><span class="sxs-lookup"><span data-stu-id="4736d-117">Access Partner Center for training, digital downloads, or Microsoft Certified Professional (MCP) association.</span></span>
    * <span data-ttu-id="4736d-118">Tilldelas Partner Center-roller som Microsoft Partner Network (MPN) admin eller incitaments administratör.</span><span class="sxs-lookup"><span data-stu-id="4736d-118">Be assigned Partner Center roles such as Microsoft Partner Network (MPN) admin or incentives admin.</span></span>

## <a name="add-an-azure-ad-tenant-to-your-account"></a><span data-ttu-id="4736d-119">Lägg till en Azure AD-klient i ditt konto</span><span class="sxs-lookup"><span data-stu-id="4736d-119">Add an Azure AD tenant to your account</span></span>

1. <span data-ttu-id="4736d-120">Logga in som global administratör till [Microsoft Partner Center](https://partner.microsoft.com/dashboard).</span><span class="sxs-lookup"><span data-stu-id="4736d-120">Sign in as global admin to [Microsoft Partner Center](https://partner.microsoft.com/dashboard).</span></span>

1. <span data-ttu-id="4736d-121">I det övre högra hörnet väljer du **Inställningar**, sedan **konto inställningar** och väljer sedan **klienter**.</span><span class="sxs-lookup"><span data-stu-id="4736d-121">At the upper right, select **Settings**, select **Account settings**, and then select **Tenants**.</span></span>
 
   :::image type="content" source="images/merge-accounts/multitenantNew.png" alt-text="Skärm bild av knappen associera i fönstret Azure AD-profil."::: 

1. <span data-ttu-id="4736d-123">Välj **associera** och ange den klient som du vill associera.</span><span class="sxs-lookup"><span data-stu-id="4736d-123">Select **Associate**, and then indicate the tenant you want to associate.</span></span>

1. <span data-ttu-id="4736d-124">Vid prompten loggar du in som global administratör till den klient som du vill associera och väljer sedan **Bekräfta**.</span><span class="sxs-lookup"><span data-stu-id="4736d-124">At the prompt, sign in as global admin to the tenant you want to associate, and then select **Confirm**.</span></span> 

   :::image type="content" source="images/merge-accounts/multitenantNew2.png" alt-text="Skärm bild av knappen Bekräfta i fönstret Bekräfta nytt Azure AD-Association."::: 

   <span data-ttu-id="4736d-126">När du har bekräftat associationen visas ett meddelande om att **alla anges** .</span><span class="sxs-lookup"><span data-stu-id="4736d-126">After you've confirmed the association, an **All set** message is displayed.</span></span> <span data-ttu-id="4736d-127">Om du vill visa den nyligen tillagda klienten väljer du **återgå till klient organisations hantering**.</span><span class="sxs-lookup"><span data-stu-id="4736d-127">To view the newly added tenant, select **Return to tenant management**.</span></span> 
 
>[!NOTE]
><span data-ttu-id="4736d-128">Du kan inte associera en klient med ett konto om det redan är kopplat till ett annat Partner Center-konto.</span><span class="sxs-lookup"><span data-stu-id="4736d-128">You can't associate a tenant with an account if it's already associated with another Partner Center account.</span></span>


## <a name="remove-a-tenant-from-your-account"></a><span data-ttu-id="4736d-129">Ta bort en klient från ditt konto</span><span class="sxs-lookup"><span data-stu-id="4736d-129">Remove a tenant from your account</span></span>
 
1. <span data-ttu-id="4736d-130">Logga in som global administratör till [Microsoft Partner Center](https://partner.microsoft.com/dashboard).</span><span class="sxs-lookup"><span data-stu-id="4736d-130">Sign in as global admin to [Microsoft Partner Center](https://partner.microsoft.com/dashboard).</span></span>

1. <span data-ttu-id="4736d-131">Klicka på ikonen **Inställningar** längst upp till höger och välj sedan **konto inställningar**.</span><span class="sxs-lookup"><span data-stu-id="4736d-131">At the upper right, select the **Settings** icon, and then select **Account settings**.</span></span>

1. <span data-ttu-id="4736d-132">Välj **innehavare** i det vänstra fönstret.</span><span class="sxs-lookup"><span data-stu-id="4736d-132">On the left pane, select **Tenants**.</span></span> <span data-ttu-id="4736d-133">Under **Hantera Azure AD-klienter** väljer du fliken **partner** .</span><span class="sxs-lookup"><span data-stu-id="4736d-133">Under **Manage Azure AD tenants**, select the **Partner** tab.</span></span>
 
1. <span data-ttu-id="4736d-134">Välj **ta bort** bredvid den klient vars Association du vill ta bort.</span><span class="sxs-lookup"><span data-stu-id="4736d-134">Select **Remove** next to the tenant whose association you want to remove.</span></span>

   :::image type="content" source="images/disassociate.png" alt-text="Skärm bild av de aktuella klient kopplingarna och deras borttagnings länkar.":::

   <span data-ttu-id="4736d-136">Som du ser i föregående skärm bild är **ta bort** länkar aktiverade för alla associerade klienter, förutom den primära klienten och klienten som du för närvarande är inloggad på.</span><span class="sxs-lookup"><span data-stu-id="4736d-136">As shown in the preceding screenshot, the **Remove** links are enabled for all associated tenants, except for the primary tenant and the tenant that you're currently signed in to.</span></span> 

   > [!NOTE]   
   > <span data-ttu-id="4736d-137">När du tar bort en klient har användarna på den innehavaren inte längre åtkomst till Partner Center-kontot, och borttagningen kan påverka din kompetens.</span><span class="sxs-lookup"><span data-stu-id="4736d-137">When you remove a tenant, the users on that tenant no longer have access to the Partner Center account, and the removal might have an impact on your competencies.</span></span> 

## <a name="next-steps"></a><span data-ttu-id="4736d-138">Nästa steg</span><span class="sxs-lookup"><span data-stu-id="4736d-138">Next steps</span></span>

- [<span data-ttu-id="4736d-139">Skapa användarkonton</span><span class="sxs-lookup"><span data-stu-id="4736d-139">Create user accounts</span></span>](create-user-accounts-and-set-permissions.md)






