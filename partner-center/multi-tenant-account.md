---
title: Lägga till klienter i ditt Partnercenter-konto
ms.topic: article
ms.date: 01/11/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Lär dig hur du lägger till, konsoliderar eller hanterar flera Azure AD-klienter i ditt Partnercenter-konto och lär dig varför du kanske vill göra det.
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: caea2002b5edc2958c0af316762408e309bcf14a
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 05/19/2021
ms.locfileid: "110151210"
---
# <a name="add-and-manage-multiple-tenants-in-your-partner-center-account"></a><span data-ttu-id="59c15-103">Lägga till och hantera flera klienter i ditt Partnercenter-konto</span><span class="sxs-lookup"><span data-stu-id="59c15-103">Add and manage multiple tenants in your Partner Center account</span></span>


<span data-ttu-id="59c15-104">**Lämpliga roller:** Global | Kontoadministratör</span><span class="sxs-lookup"><span data-stu-id="59c15-104">**Appropriate roles**: Global admin | Account admin</span></span>

<span data-ttu-id="59c15-105">Den här artikeln beskriver hur du konsoliderar flera Azure Active Directory-klienter (Azure AD) för ditt företag och sedan lägger till och hanterar dem i ditt Partnercenter-konto.</span><span class="sxs-lookup"><span data-stu-id="59c15-105">This article discusses how to consolidate multiple Azure Active Directory (Azure AD) tenants for your company and then add and manage them in your Partner Center account.</span></span> <span data-ttu-id="59c15-106">Det finns många skäl att göra det.</span><span class="sxs-lookup"><span data-stu-id="59c15-106">There are many reasons to do so.</span></span> <span data-ttu-id="59c15-107">Exempel:</span><span class="sxs-lookup"><span data-stu-id="59c15-107">For example:</span></span>

- <span data-ttu-id="59c15-108">Anta att ditt företag, Contoso, har köpt ett annat företag, Fabrikam.</span><span class="sxs-lookup"><span data-stu-id="59c15-108">Let's say your company, Contoso, has acquired another company, Fabrikam.</span></span> <span data-ttu-id="59c15-109">Du vill att de två företagen ska vara åtskilda, men du vill att de nya medarbetarna ska kunna använda Partnercenter.</span><span class="sxs-lookup"><span data-stu-id="59c15-109">You want the two companies to remain separate, but you want the new employees to be able to use Partner Center.</span></span> <span data-ttu-id="59c15-110">I det här fallet associerar du det nya företagets Azure AD-klientorganisation med ditt globala partnerkonto (PGA).</span><span class="sxs-lookup"><span data-stu-id="59c15-110">In this case, you associate the new company's Azure AD tenant with your Partner global account (PGA).</span></span> <span data-ttu-id="59c15-111">Den här associationen gör det möjligt för användare i båda företagen att arbeta i Partnercenter.</span><span class="sxs-lookup"><span data-stu-id="59c15-111">This association enables users in both companies to work in Partner Center.</span></span>

- <span data-ttu-id="59c15-112">Om du driver ditt företag med fler än en klientorganisation (till exempel *contoso.com*, *contoso.uk* och *contoso.in*) kan du använda flera klientorganisationen för att gruppera dem i samma datorkonto.</span><span class="sxs-lookup"><span data-stu-id="59c15-112">If you run your business with more than one tenant (for example, *contoso.com*, *contoso.uk*, and *contoso.in*), you can use multitenancy to group them in the same PC account.</span></span>

- <span data-ttu-id="59c15-113">Om riktlinjerna för sammanslagningar och förvärv kräver att du arbetar med klienter för båda företagen använder du både constoso.com *och* *fabrikam.com* klienter.</span><span class="sxs-lookup"><span data-stu-id="59c15-113">If mergers and acquisitions guidelines require you to work with tenants of both companies, you would use both the *constoso.com* and *fabrikam.com* tenants.</span></span>

- <span data-ttu-id="59c15-114">Användare av någon av klienterna måste kunna:</span><span class="sxs-lookup"><span data-stu-id="59c15-114">Users of any of the tenants need to be able to:</span></span>
    * <span data-ttu-id="59c15-115">Få åtkomst till Partnercenter för utbildning, digitala nedladdningar eller MICROSOFT Certified Professional-association (MCP).</span><span class="sxs-lookup"><span data-stu-id="59c15-115">Access Partner Center for training, digital downloads, or Microsoft Certified Professional (MCP) association.</span></span>
    * <span data-ttu-id="59c15-116">Tilldelas Partner Center-roller som Microsoft Partner Network (MPN)-administratör eller incitamentsadministratör.</span><span class="sxs-lookup"><span data-stu-id="59c15-116">Be assigned Partner Center roles such as Microsoft Partner Network (MPN) admin or incentives admin.</span></span>

## <a name="add-an-azure-ad-tenant-to-your-account"></a><span data-ttu-id="59c15-117">Lägga till en Azure AD-klientorganisation till ditt konto</span><span class="sxs-lookup"><span data-stu-id="59c15-117">Add an Azure AD tenant to your account</span></span>

1. <span data-ttu-id="59c15-118">Logga in som global administratör på [Microsoft Partner Center.](https://partner.microsoft.com/dashboard)</span><span class="sxs-lookup"><span data-stu-id="59c15-118">Sign in as global admin to [Microsoft Partner Center](https://partner.microsoft.com/dashboard).</span></span>

1. <span data-ttu-id="59c15-119">Längst upp till höger väljer **du Inställningar,** **Kontoinställningar** och sedan **Klienter.**</span><span class="sxs-lookup"><span data-stu-id="59c15-119">At the upper right, select **Settings**, select **Account settings**, and then select **Tenants**.</span></span>
 
   :::image type="content" source="images/merge-accounts/multitenantNew.png" alt-text="Skärmbild av knappen Associera i fönstret Azure AD-profil."::: 

1. <span data-ttu-id="59c15-121">Välj **Associera** och ange sedan den klientorganisation som du vill associera.</span><span class="sxs-lookup"><span data-stu-id="59c15-121">Select **Associate**, and then indicate the tenant you want to associate.</span></span>

1. <span data-ttu-id="59c15-122">Logga in som global administratör till den klientorganisation som du vill associera med i prompten och välj sedan **Bekräfta.**</span><span class="sxs-lookup"><span data-stu-id="59c15-122">At the prompt, sign in as global admin to the tenant you want to associate, and then select **Confirm**.</span></span> 

   :::image type="content" source="images/merge-accounts/multitenantNew2.png" alt-text="Skärmbild av knappen Bekräfta i fönstret Bekräfta ny Azure AD-association."::: 

   <span data-ttu-id="59c15-124">När du har bekräftat associationen visas **meddelandet All set** (Allt angett).</span><span class="sxs-lookup"><span data-stu-id="59c15-124">After you've confirmed the association, an **All set** message is displayed.</span></span> <span data-ttu-id="59c15-125">Om du vill visa den nyligen tillagda klienten väljer **du Återgå till klienthantering.**</span><span class="sxs-lookup"><span data-stu-id="59c15-125">To view the newly added tenant, select **Return to tenant management**.</span></span> 
 
>[!NOTE]
><span data-ttu-id="59c15-126">Du kan inte associera en klientorganisation med ett konto om den redan är associerad med ett annat Partnercenter-konto.</span><span class="sxs-lookup"><span data-stu-id="59c15-126">You can't associate a tenant with an account if it's already associated with another Partner Center account.</span></span>


## <a name="remove-a-tenant-from-your-account"></a><span data-ttu-id="59c15-127">Ta bort en klientorganisation från ditt konto</span><span class="sxs-lookup"><span data-stu-id="59c15-127">Remove a tenant from your account</span></span>
 
1. <span data-ttu-id="59c15-128">Logga in som global administratör på [Microsoft Partner Center.](https://partner.microsoft.com/dashboard)</span><span class="sxs-lookup"><span data-stu-id="59c15-128">Sign in as global admin to [Microsoft Partner Center](https://partner.microsoft.com/dashboard).</span></span>

1. <span data-ttu-id="59c15-129">Längst upp till höger väljer du **ikonen** Inställningar och sedan **Kontoinställningar.**</span><span class="sxs-lookup"><span data-stu-id="59c15-129">At the upper right, select the **Settings** icon, and then select **Account settings**.</span></span>

1. <span data-ttu-id="59c15-130">I den vänstra rutan väljer **du Klienter.**</span><span class="sxs-lookup"><span data-stu-id="59c15-130">On the left pane, select **Tenants**.</span></span> <span data-ttu-id="59c15-131">Under **Hantera Azure AD-klienter** väljer du **fliken** Partner.</span><span class="sxs-lookup"><span data-stu-id="59c15-131">Under **Manage Azure AD tenants**, select the **Partner** tab.</span></span>
 
1. <span data-ttu-id="59c15-132">Välj **Ta** bort bredvid den klientorganisation vars association du vill ta bort.</span><span class="sxs-lookup"><span data-stu-id="59c15-132">Select **Remove** next to the tenant whose association you want to remove.</span></span>

   :::image type="content" source="images/disassociate.png" alt-text="Skärmbild av de aktuella klientorganisationsassociationer och deras Ta bort länkar.":::

   <span data-ttu-id="59c15-134">Som du ser i föregående  skärmbild är länkarna Ta bort aktiverade för alla associerade klienter, förutom den primära klientorganisationen och den klientorganisation som du för närvarande är inloggad på.</span><span class="sxs-lookup"><span data-stu-id="59c15-134">As shown in the preceding screenshot, the **Remove** links are enabled for all associated tenants, except for the primary tenant and the tenant that you're currently signed in to.</span></span> 

   > [!NOTE]   
   > <span data-ttu-id="59c15-135">När du tar bort en klientorganisation har användarna i den klientorganisationen inte längre åtkomst till Partnercenter-kontot och borttagningen kan påverka dina kompetenser.</span><span class="sxs-lookup"><span data-stu-id="59c15-135">When you remove a tenant, the users on that tenant no longer have access to the Partner Center account, and the removal might have an impact on your competencies.</span></span> 

## <a name="next-steps"></a><span data-ttu-id="59c15-136">Nästa steg</span><span class="sxs-lookup"><span data-stu-id="59c15-136">Next steps</span></span>

- [<span data-ttu-id="59c15-137">Skapa användarkonton</span><span class="sxs-lookup"><span data-stu-id="59c15-137">Create user accounts</span></span>](create-user-accounts-and-set-permissions.md)






