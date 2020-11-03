---
title: Lägg till ytterligare klienter till ditt partner Center-konto
ms.topic: article
ms.date: 07/30/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Lär dig hur du lägger till, konsoliderar eller hanterar flera Azure AD-klienter i ditt partner Center-konto. Lär dig också om några av de orsaker du kanske vill göra det.
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: b9379ce6b27a8ef6e5d6894a0630745794e04e04
ms.sourcegitcommit: 3c45a181ef86b3a4866e97fb50efeae8714ab3f7
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 10/19/2020
ms.locfileid: "92532028"
---
# <a name="add-and-manage-multiple-tenants-in-your-partner-center-account"></a><span data-ttu-id="6c072-104">Lägga till och hantera flera klienter i ditt partner Center-konto</span><span class="sxs-lookup"><span data-stu-id="6c072-104">Add and manage multiple tenants in your Partner Center account</span></span>

<span data-ttu-id="6c072-105">**Gäller för**</span><span class="sxs-lookup"><span data-stu-id="6c072-105">**Applies to**</span></span>

- <span data-ttu-id="6c072-106">Partnercenter</span><span class="sxs-lookup"><span data-stu-id="6c072-106">Partner Center</span></span>

<span data-ttu-id="6c072-107">**Lämpliga roller**</span><span class="sxs-lookup"><span data-stu-id="6c072-107">**Appropriate roles**</span></span>

- <span data-ttu-id="6c072-108">Global administratör</span><span class="sxs-lookup"><span data-stu-id="6c072-108">Global admin</span></span>

<span data-ttu-id="6c072-109">Med den här funktionen kan du hantera flera klientorganisationer i ditt företag och konsolidera dem till ditt Partner Center-konto.</span><span class="sxs-lookup"><span data-stu-id="6c072-109">This feature allows you to manage multiple tenants for your company and to consolidate them into your Partner Center account.</span></span> <span data-ttu-id="6c072-110">Det finns många orsaker till varför du kan behöva hantera flera Azure AD-klienter i ditt partner Center-konto.</span><span class="sxs-lookup"><span data-stu-id="6c072-110">There are many reasons why you may need to manage multiple Azure AD tenants in your Partner Center account.</span></span> <span data-ttu-id="6c072-111">Exempel:</span><span class="sxs-lookup"><span data-stu-id="6c072-111">For example:</span></span>

- <span data-ttu-id="6c072-112">Företaget kan köpa ett annat företag och du vill att de anställda i det nya företaget ska kunna använda Partner Center.</span><span class="sxs-lookup"><span data-stu-id="6c072-112">Your company may purchase another company, and you want the employees in the new company to be able to use Partner Center.</span></span> <span data-ttu-id="6c072-113">Men du vill att de två företagen ska vara åtskilda.</span><span class="sxs-lookup"><span data-stu-id="6c072-113">However, you want the two companies to remain separate.</span></span> <span data-ttu-id="6c072-114">I det här fallet associerar du det nya företagets Azure AD-klient med ditt partner globala konto (PGA).</span><span class="sxs-lookup"><span data-stu-id="6c072-114">In this case, you'd associate the new company's Azure AD tenant with your Partner global account (PGA).</span></span> <span data-ttu-id="6c072-115">Den här kopplingen gör det möjligt för användare i båda företagen att arbeta i Partner Center.</span><span class="sxs-lookup"><span data-stu-id="6c072-115">This association would enable users in both companies to work in Partner Center.</span></span>

- <span data-ttu-id="6c072-116">Om du har fler än en klient för att köra företaget (t. ex. contoso.com, contoso.uk, contoso.in) kan du använda flera innehavare för att koppla ihop dem under samma PC-konto.</span><span class="sxs-lookup"><span data-stu-id="6c072-116">If you have more than one tenant to run your business (e.g. contoso.com, contoso.uk, contoso.in) you can use multi-tenancy to tie them under the same PC account.</span></span>

- <span data-ttu-id="6c072-117">Sammanslagningar och förvärv kräver att du arbetar med fler än en klient (t. ex. om contoso förvärvar Fabrikam måste du kunna använda både Constoso.com och Fabrikam.com respektive klienter).</span><span class="sxs-lookup"><span data-stu-id="6c072-117">Mergers and acquisitions requires you to work with more than one tenant (e.g. If Contoso acquires Fabrikam, you would need to be able to use both Constoso.com and Fabrikam.com respective tenants).</span></span>

- <span data-ttu-id="6c072-118">Användare från någon av klient organisationerna måste kunna:</span><span class="sxs-lookup"><span data-stu-id="6c072-118">Users from any of the tenants would need to be able to:</span></span>
    1.  <span data-ttu-id="6c072-119">Åtkomst till Partner Center för utbildning, digital hämtning, MCP-Association</span><span class="sxs-lookup"><span data-stu-id="6c072-119">Access Partner Center for training, digital downloads, MCP association</span></span>
    2.  <span data-ttu-id="6c072-120">Tilldelas Partner Center-roller som MPN-administratör, incitaments administratör osv.</span><span class="sxs-lookup"><span data-stu-id="6c072-120">Be assigned Partner Center roles like MPN Admin, Incentives Admin etc.</span></span>


## <a name="add-another-azure-ad-tenant-to-your-account"></a><span data-ttu-id="6c072-121">Lägg till en annan Azure AD-klient i ditt konto</span><span class="sxs-lookup"><span data-stu-id="6c072-121">Add another Azure AD tenant to your account</span></span>

1. <span data-ttu-id="6c072-122">Logga in på [instrument panelen](https://partner.microsoft.com/dashboard)för partner Center som global administratör.</span><span class="sxs-lookup"><span data-stu-id="6c072-122">As the global admin, sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>
1. <span data-ttu-id="6c072-123">Från **inställnings** ikonen väljer du **konto inställningar** och väljer sedan **klienter** .</span><span class="sxs-lookup"><span data-stu-id="6c072-123">From the **Settings** icon, select **Account settings** and then select **Tenants** .</span></span>
 
:::image type="content" source="images/merge-accounts/multitenantNew.png" alt-text="koppla klienter"::: 

3. <span data-ttu-id="6c072-125">Välj **associera en annan AD-klient** och ange den klient som du vill koppla.</span><span class="sxs-lookup"><span data-stu-id="6c072-125">Select **Associate another AD tenant** and indicate the tenant you want to associate.</span></span>

1. <span data-ttu-id="6c072-126">Logga in på den klient som du vill associera och bekräfta associationen som global administratör.</span><span class="sxs-lookup"><span data-stu-id="6c072-126">As global admin, sign into the tenant you want to associate and confirm the association.</span></span> 

:::image type="content" source="images/merge-accounts/multitenantNew2.png" alt-text="bekräfta koppling av klienter"::: 

5. <span data-ttu-id="6c072-128">När **du har bekräftat visas ett meddelande** om detta.</span><span class="sxs-lookup"><span data-stu-id="6c072-128">After you confirm, you will see an **All set** notice.</span></span>  <span data-ttu-id="6c072-129">Välj **återgå till klient organisations hantering** så visas den nyligen tillagda klienten i listan.</span><span class="sxs-lookup"><span data-stu-id="6c072-129">Select **Return to tenant management** and you will see the newly added tenant listed.</span></span> 
 

>[!NOTE]
><span data-ttu-id="6c072-130">Du kan inte koppla en klient till ett konto om det redan är kopplat till ett annat Partner Center-konto.</span><span class="sxs-lookup"><span data-stu-id="6c072-130">You can't associate a tenant to an account if it is already associated to another Partner Center account.</span></span>

 
## <a name="next-steps"></a><span data-ttu-id="6c072-131">Nästa steg</span><span class="sxs-lookup"><span data-stu-id="6c072-131">Next steps</span></span>

- [<span data-ttu-id="6c072-132">Lägg till användare</span><span class="sxs-lookup"><span data-stu-id="6c072-132">Add users</span></span>](create-user-accounts-and-set-permissions.md)
