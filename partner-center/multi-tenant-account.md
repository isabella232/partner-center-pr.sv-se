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
ms.openlocfilehash: f9852b4e1c3997b82f744555db25fe64e1afc8ad
ms.sourcegitcommit: 531151a5dbc999b8b7de478d72ea115e6d579ff1
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 01/13/2021
ms.locfileid: "98182446"
---
# <a name="add-and-manage-multiple-tenants-in-your-partner-center-account"></a><span data-ttu-id="a1331-104">Lägga till och hantera flera klienter i ditt partner Center-konto</span><span class="sxs-lookup"><span data-stu-id="a1331-104">Add and manage multiple tenants in your Partner Center account</span></span>


<span data-ttu-id="a1331-105">**Lämpliga roller**</span><span class="sxs-lookup"><span data-stu-id="a1331-105">**Appropriate roles**</span></span>

- <span data-ttu-id="a1331-106">Global administratör</span><span class="sxs-lookup"><span data-stu-id="a1331-106">Global admin</span></span>
- <span data-ttu-id="a1331-107">Kontoadministratör</span><span class="sxs-lookup"><span data-stu-id="a1331-107">Account admin</span></span>

<span data-ttu-id="a1331-108">Med den här funktionen kan du hantera flera klientorganisationer i ditt företag och konsolidera dem till ditt Partner Center-konto.</span><span class="sxs-lookup"><span data-stu-id="a1331-108">This feature allows you to manage multiple tenants for your company and to consolidate them into your Partner Center account.</span></span> <span data-ttu-id="a1331-109">Det finns många orsaker till varför du kan behöva hantera flera Azure AD-klienter i ditt partner Center-konto.</span><span class="sxs-lookup"><span data-stu-id="a1331-109">There are many reasons why you may need to manage multiple Azure AD tenants in your Partner Center account.</span></span> <span data-ttu-id="a1331-110">Exempel:</span><span class="sxs-lookup"><span data-stu-id="a1331-110">For example:</span></span>

- <span data-ttu-id="a1331-111">Företaget kan köpa ett annat företag och du vill att de anställda i det nya företaget ska kunna använda Partner Center.</span><span class="sxs-lookup"><span data-stu-id="a1331-111">Your company may purchase another company, and you want the employees in the new company to be able to use Partner Center.</span></span> <span data-ttu-id="a1331-112">Men du vill att de två företagen ska vara åtskilda.</span><span class="sxs-lookup"><span data-stu-id="a1331-112">However, you want the two companies to remain separate.</span></span> <span data-ttu-id="a1331-113">I det här fallet associerar du det nya företagets Azure AD-klient med ditt partner globala konto (PGA).</span><span class="sxs-lookup"><span data-stu-id="a1331-113">In this case, you'd associate the new company's Azure AD tenant with your Partner global account (PGA).</span></span> <span data-ttu-id="a1331-114">Den här kopplingen gör det möjligt för användare i båda företagen att arbeta i Partner Center.</span><span class="sxs-lookup"><span data-stu-id="a1331-114">This association would enable users in both companies to work in Partner Center.</span></span>

- <span data-ttu-id="a1331-115">Om du har fler än en klient för att köra företaget (t. ex. contoso.com, contoso.uk, contoso.in) kan du använda flera innehavare för att koppla ihop dem under samma PC-konto.</span><span class="sxs-lookup"><span data-stu-id="a1331-115">If you have more than one tenant to run your business (e.g. contoso.com, contoso.uk, contoso.in) you can use multi-tenancy to tie them under the same PC account.</span></span>

- <span data-ttu-id="a1331-116">Sammanslagningar och förvärv kräver att du arbetar med fler än en klient (t. ex. om contoso förvärvar Fabrikam måste du kunna använda både Constoso.com och Fabrikam.com respektive klienter).</span><span class="sxs-lookup"><span data-stu-id="a1331-116">Mergers and acquisitions requires you to work with more than one tenant (e.g. If Contoso acquires Fabrikam, you would need to be able to use both Constoso.com and Fabrikam.com respective tenants).</span></span>

- <span data-ttu-id="a1331-117">Användare från någon av klient organisationerna måste kunna:</span><span class="sxs-lookup"><span data-stu-id="a1331-117">Users from any of the tenants would need to be able to:</span></span>
    1.  <span data-ttu-id="a1331-118">Åtkomst till Partner Center för utbildning, digital hämtning, MCP-Association</span><span class="sxs-lookup"><span data-stu-id="a1331-118">Access Partner Center for training, digital downloads, MCP association</span></span>
    2.  <span data-ttu-id="a1331-119">Tilldelas Partner Center-roller som MPN-administratör, incitaments administratör osv.</span><span class="sxs-lookup"><span data-stu-id="a1331-119">Be assigned Partner Center roles like MPN Admin, Incentives Admin etc.</span></span>


## <a name="add-another-azure-ad-tenant-to-your-account"></a><span data-ttu-id="a1331-120">Lägg till en annan Azure AD-klient i ditt konto</span><span class="sxs-lookup"><span data-stu-id="a1331-120">Add another Azure AD tenant to your account</span></span>

1. <span data-ttu-id="a1331-121">Logga in på [instrument panelen](https://partner.microsoft.com/dashboard)för partner Center som global administratör.</span><span class="sxs-lookup"><span data-stu-id="a1331-121">As the global admin, sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>
1. <span data-ttu-id="a1331-122">Från **inställnings** ikonen väljer du **konto inställningar** och väljer sedan **klienter**.</span><span class="sxs-lookup"><span data-stu-id="a1331-122">From the **Settings** icon, select **Account settings** and then select **Tenants**.</span></span>
 
:::image type="content" source="images/merge-accounts/multitenantNew.png" alt-text="koppla klienter"::: 

3. <span data-ttu-id="a1331-124">Välj **associera en annan AD-klient** och ange den klient som du vill koppla.</span><span class="sxs-lookup"><span data-stu-id="a1331-124">Select **Associate another AD tenant** and indicate the tenant you want to associate.</span></span>

1. <span data-ttu-id="a1331-125">Logga in på den klient som du vill associera och bekräfta associationen som global administratör.</span><span class="sxs-lookup"><span data-stu-id="a1331-125">As global admin, sign into the tenant you want to associate and confirm the association.</span></span> 

:::image type="content" source="images/merge-accounts/multitenantNew2.png" alt-text="bekräfta koppling av klienter"::: 

5. <span data-ttu-id="a1331-127">När **du har bekräftat visas ett meddelande** om detta.</span><span class="sxs-lookup"><span data-stu-id="a1331-127">After you confirm, you will see an **All set** notice.</span></span>  <span data-ttu-id="a1331-128">Välj **återgå till klient hantering** så visas den nyligen tillagda klienten i listan.</span><span class="sxs-lookup"><span data-stu-id="a1331-128">Select **Return to tenant management** and you'll see the newly added tenant listed.</span></span> 
 

>[!NOTE]
><span data-ttu-id="a1331-129">Du kan inte koppla en klient till ett konto om det redan är kopplat till ett annat Partner Center-konto.</span><span class="sxs-lookup"><span data-stu-id="a1331-129">You can't associate a tenant to an account if it is already associated to another Partner Center account.</span></span>


## <a name="remove-a-tenant-from-your-account"></a><span data-ttu-id="a1331-130">Ta bort en klient från ditt konto</span><span class="sxs-lookup"><span data-stu-id="a1331-130">Remove a tenant from your account</span></span>
 
1. <span data-ttu-id="a1331-131">Logga in på [instrument panelen](https://partner.microsoft.com/dashboard)för partner Center som global administratör.</span><span class="sxs-lookup"><span data-stu-id="a1331-131">As the global admin, sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

1. <span data-ttu-id="a1331-132">I ikonen **Inställningar** väljer du **konto inställningar** -> klienter och klickar på fliken **partner** .</span><span class="sxs-lookup"><span data-stu-id="a1331-132">From the **Settings** icon, select **Account settings** -> Tenants and click on the **Partner** tab.</span></span>
 
3. <span data-ttu-id="a1331-133">Klicka på **ta bort** för den klient som du vill koppla bort.</span><span class="sxs-lookup"><span data-stu-id="a1331-133">Click **Remove** for the tenant you want to dissociate.</span></span>

4. <span data-ttu-id="a1331-134">Att koppla från en klient organisation innebär att användare av den klienten inte längre har åtkomst till Partner Center-kontot, och detta kan påverka din kompetens.</span><span class="sxs-lookup"><span data-stu-id="a1331-134">Dissociating a tenant means that the users on that tenant will no longer have access to the Partner Center account, and this could have an impact on your competencies.</span></span> 

<span data-ttu-id="a1331-135">Knappen **ta bort** är aktive rad för alla associerade klienter, förutom den primära klienten och klienten som du för närvarande är inloggad på.</span><span class="sxs-lookup"><span data-stu-id="a1331-135">The **Remove** button is enabled for all associated tenants, except the primary tenant and the tenant which you are currently signed into.</span></span>

:::image type="content" source="images/disassociate.png" alt-text="innehavare med knappen Ta bort":::
 

## <a name="next-steps"></a><span data-ttu-id="a1331-137">Nästa steg</span><span class="sxs-lookup"><span data-stu-id="a1331-137">Next steps</span></span>

- [<span data-ttu-id="a1331-138">Lägg till användare</span><span class="sxs-lookup"><span data-stu-id="a1331-138">Add users</span></span>](create-user-accounts-and-set-permissions.md)






