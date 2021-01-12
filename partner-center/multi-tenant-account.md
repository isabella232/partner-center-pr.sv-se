---
title: Lägg till ytterligare klienter till ditt partner Center-konto
ms.topic: article
ms.date: 01/11/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Lär dig hur du lägger till, konsoliderar eller hanterar flera Azure AD-klienter i ditt partner Center-konto. Lär dig också om några av de orsaker du kanske vill göra det.
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 22f85bda0a651559da1717ae1e5365da40d62aff
ms.sourcegitcommit: 8cb98de420f6ab5bb4cb3efc9007262c4d7d3327
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 01/12/2021
ms.locfileid: "98105564"
---
# <a name="add-and-manage-multiple-tenants-in-your-partner-center-account"></a><span data-ttu-id="aa3ef-104">Lägga till och hantera flera klienter i ditt partner Center-konto</span><span class="sxs-lookup"><span data-stu-id="aa3ef-104">Add and manage multiple tenants in your Partner Center account</span></span>


<span data-ttu-id="aa3ef-105">**Lämpliga roller**</span><span class="sxs-lookup"><span data-stu-id="aa3ef-105">**Appropriate roles**</span></span>

- <span data-ttu-id="aa3ef-106">Global administratör</span><span class="sxs-lookup"><span data-stu-id="aa3ef-106">Global admin</span></span>

<span data-ttu-id="aa3ef-107">Med den här funktionen kan du hantera flera klientorganisationer i ditt företag och konsolidera dem till ditt Partner Center-konto.</span><span class="sxs-lookup"><span data-stu-id="aa3ef-107">This feature allows you to manage multiple tenants for your company and to consolidate them into your Partner Center account.</span></span> <span data-ttu-id="aa3ef-108">Det finns många orsaker till varför du kan behöva hantera flera Azure AD-klienter i ditt partner Center-konto.</span><span class="sxs-lookup"><span data-stu-id="aa3ef-108">There are many reasons why you may need to manage multiple Azure AD tenants in your Partner Center account.</span></span> <span data-ttu-id="aa3ef-109">Till exempel:</span><span class="sxs-lookup"><span data-stu-id="aa3ef-109">For example:</span></span>

- <span data-ttu-id="aa3ef-110">Företaget kan köpa ett annat företag och du vill att de anställda i det nya företaget ska kunna använda Partner Center.</span><span class="sxs-lookup"><span data-stu-id="aa3ef-110">Your company may purchase another company, and you want the employees in the new company to be able to use Partner Center.</span></span> <span data-ttu-id="aa3ef-111">Men du vill att de två företagen ska vara åtskilda.</span><span class="sxs-lookup"><span data-stu-id="aa3ef-111">However, you want the two companies to remain separate.</span></span> <span data-ttu-id="aa3ef-112">I det här fallet associerar du det nya företagets Azure AD-klient med ditt partner globala konto (PGA).</span><span class="sxs-lookup"><span data-stu-id="aa3ef-112">In this case, you'd associate the new company's Azure AD tenant with your Partner global account (PGA).</span></span> <span data-ttu-id="aa3ef-113">Den här kopplingen gör det möjligt för användare i båda företagen att arbeta i Partner Center.</span><span class="sxs-lookup"><span data-stu-id="aa3ef-113">This association would enable users in both companies to work in Partner Center.</span></span>

- <span data-ttu-id="aa3ef-114">Om du har fler än en klient för att köra företaget (t. ex. contoso.com, contoso.uk, contoso.in) kan du använda flera innehavare för att koppla ihop dem under samma PC-konto.</span><span class="sxs-lookup"><span data-stu-id="aa3ef-114">If you have more than one tenant to run your business (e.g. contoso.com, contoso.uk, contoso.in) you can use multi-tenancy to tie them under the same PC account.</span></span>

- <span data-ttu-id="aa3ef-115">Sammanslagningar och förvärv kräver att du arbetar med fler än en klient (t. ex. om contoso förvärvar Fabrikam måste du kunna använda både Constoso.com och Fabrikam.com respektive klienter).</span><span class="sxs-lookup"><span data-stu-id="aa3ef-115">Mergers and acquisitions requires you to work with more than one tenant (e.g. If Contoso acquires Fabrikam, you would need to be able to use both Constoso.com and Fabrikam.com respective tenants).</span></span>

- <span data-ttu-id="aa3ef-116">Användare från någon av klient organisationerna måste kunna:</span><span class="sxs-lookup"><span data-stu-id="aa3ef-116">Users from any of the tenants would need to be able to:</span></span>
    1.  <span data-ttu-id="aa3ef-117">Åtkomst till Partner Center för utbildning, digital hämtning, MCP-Association</span><span class="sxs-lookup"><span data-stu-id="aa3ef-117">Access Partner Center for training, digital downloads, MCP association</span></span>
    2.  <span data-ttu-id="aa3ef-118">Tilldelas Partner Center-roller som MPN-administratör, incitaments administratör osv.</span><span class="sxs-lookup"><span data-stu-id="aa3ef-118">Be assigned Partner Center roles like MPN Admin, Incentives Admin etc.</span></span>


## <a name="add-another-azure-ad-tenant-to-your-account"></a><span data-ttu-id="aa3ef-119">Lägg till en annan Azure AD-klient i ditt konto</span><span class="sxs-lookup"><span data-stu-id="aa3ef-119">Add another Azure AD tenant to your account</span></span>

1. <span data-ttu-id="aa3ef-120">Logga in på [instrument panelen](https://partner.microsoft.com/dashboard)för partner Center som global administratör.</span><span class="sxs-lookup"><span data-stu-id="aa3ef-120">As the global admin, sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>
1. <span data-ttu-id="aa3ef-121">Från **inställnings** ikonen väljer du **konto inställningar** och väljer sedan **klienter**.</span><span class="sxs-lookup"><span data-stu-id="aa3ef-121">From the **Settings** icon, select **Account settings** and then select **Tenants**.</span></span>
 
:::image type="content" source="images/merge-accounts/multitenantNew.png" alt-text="koppla klienter"::: 

3. <span data-ttu-id="aa3ef-123">Välj **associera en annan AD-klient** och ange den klient som du vill koppla.</span><span class="sxs-lookup"><span data-stu-id="aa3ef-123">Select **Associate another AD tenant** and indicate the tenant you want to associate.</span></span>

1. <span data-ttu-id="aa3ef-124">Logga in på den klient som du vill associera och bekräfta associationen som global administratör.</span><span class="sxs-lookup"><span data-stu-id="aa3ef-124">As global admin, sign into the tenant you want to associate and confirm the association.</span></span> 

:::image type="content" source="images/merge-accounts/multitenantNew2.png" alt-text="bekräfta koppling av klienter"::: 

5. <span data-ttu-id="aa3ef-126">När **du har bekräftat visas ett meddelande** om detta.</span><span class="sxs-lookup"><span data-stu-id="aa3ef-126">After you confirm, you will see an **All set** notice.</span></span>  <span data-ttu-id="aa3ef-127">Välj **återgå till klient hantering** så visas den nyligen tillagda klienten i listan.</span><span class="sxs-lookup"><span data-stu-id="aa3ef-127">Select **Return to tenant management** and you'll see the newly added tenant listed.</span></span> 
 

>[!NOTE]
><span data-ttu-id="aa3ef-128">Du kan inte koppla en klient till ett konto om det redan är kopplat till ett annat Partner Center-konto.</span><span class="sxs-lookup"><span data-stu-id="aa3ef-128">You can't associate a tenant to an account if it is already associated to another Partner Center account.</span></span>


## <a name="remove-a-tenant-from-your-account"></a><span data-ttu-id="aa3ef-129">Ta bort en klient från ditt konto</span><span class="sxs-lookup"><span data-stu-id="aa3ef-129">Remove a tenant from your account</span></span>
 
1. <span data-ttu-id="aa3ef-130">Logga in på [instrument panelen](https://partner.microsoft.com/dashboard)för partner Center som global administratör.</span><span class="sxs-lookup"><span data-stu-id="aa3ef-130">As the global admin, sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

1. <span data-ttu-id="aa3ef-131">I ikonen **Inställningar** väljer du **konto inställningar** -> klienter och klickar på fliken **partner** .</span><span class="sxs-lookup"><span data-stu-id="aa3ef-131">From the **Settings** icon, select **Account settings** -> Tenants and click on the **Partner** tab.</span></span>
 
3. <span data-ttu-id="aa3ef-132">Klicka på **ta bort** för den klient som du vill koppla bort.</span><span class="sxs-lookup"><span data-stu-id="aa3ef-132">Click **Remove** for the tenant you want to dissociate.</span></span>

4. <span data-ttu-id="aa3ef-133">Att koppla från en klient organisation innebär att användare av den klienten inte längre har åtkomst till Partner Center-kontot, och detta kan påverka din kompetens.</span><span class="sxs-lookup"><span data-stu-id="aa3ef-133">Dissociating a tenant means that the users on that tenant will no longer have access to the Partner Center account, and this could have an impact on your competencies.</span></span> 

<span data-ttu-id="aa3ef-134">Knappen **ta bort** är aktive rad för alla associerade klienter, förutom den primära klienten och klienten som du för närvarande är inloggad på.</span><span class="sxs-lookup"><span data-stu-id="aa3ef-134">The **Remove** button is enabled for all associated tenants, except the primary tenant and the tenant which you are currently signed into.</span></span>

:::image type="content" source="images/disassociate.png" alt-text="innehavare med knappen Ta bort":::
 

## <a name="next-steps"></a><span data-ttu-id="aa3ef-136">Nästa steg</span><span class="sxs-lookup"><span data-stu-id="aa3ef-136">Next steps</span></span>

- [<span data-ttu-id="aa3ef-137">Lägg till användare</span><span class="sxs-lookup"><span data-stu-id="aa3ef-137">Add users</span></span>](create-user-accounts-and-set-permissions.md)






