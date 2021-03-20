---
title: Skapa och hantera privata Azure Marketplace i Azure Portal
description: Lär dig mer om att skapa och hantera privata Azure Marketplace (för hands version) i Azure Portal. Med privat Azure Marketplace (för hands version) kan administratörer styra vilka lösningar från tredje part som användarna kan använda.
ms.service: marketplace-customer
ms.topic: how-to
author: msjogarrig
ms.author: jogarrig
ms.date: 02/24/2021
ms.openlocfilehash: 8cfe0e95d1655530c9bc9d24b1efe85e6432236b
ms.sourcegitcommit: e8e8362d2777d25efac3e1076af5939765ed13d0
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/20/2021
ms.locfileid: "104712774"
---
# <a name="create-and-manage-private-azure-marketplace-in-the-azure-portal"></a><span data-ttu-id="0f595-104">Skapa och hantera privata Azure Marketplace i Azure Portal</span><span class="sxs-lookup"><span data-stu-id="0f595-104">Create and manage Private Azure Marketplace in the Azure portal</span></span>

<span data-ttu-id="0f595-105">Privata Azure Marketplace låter administratörer styra vilka lösningar från tredje part som användarna kan använda.</span><span class="sxs-lookup"><span data-stu-id="0f595-105">Private Azure Marketplace lets administrators govern which third-party solutions their users can use.</span></span> <span data-ttu-id="0f595-106">Det gör det genom att låta användaren bara distribuera erbjudanden som godkänts av administratören och följa företagets principer.</span><span class="sxs-lookup"><span data-stu-id="0f595-106">It does this by allowing the user to deploy only offers that are approved by the administrator and comply with your enterprise's policies.</span></span> <span data-ttu-id="0f595-107">Med privat Azure Marketplace kan användarna söka i onlinebutiken efter kompatibla erbjudanden för köp och distribution.</span><span class="sxs-lookup"><span data-stu-id="0f595-107">With Private Azure Marketplace, users can search the online store for compliant offers to purchase and deploy.</span></span>

<span data-ttu-id="0f595-108">Som Marketplace-administratör (tilldelad roll) börjar du med en inaktive rad och en tom privat lagrings plats där du kan lägga till godkända erbjudanden och planer.</span><span class="sxs-lookup"><span data-stu-id="0f595-108">As a Marketplace admin (assigned role), you will start with a disabled and empty Private Store where you can add your approved offers and plans.</span></span> <span data-ttu-id="0f595-109">Den här artikeln beskriver hur du tilldelar den roll som krävs, skapar ett privat lager, hanterar objekt, godkänner användar förfrågningar och aktiverar privat Azure Marketplace för dina användare.</span><span class="sxs-lookup"><span data-stu-id="0f595-109">This article explains how to assign the needed role, create a private store, manage items, approve user requests, and enable Private Azure Marketplace for your users.</span></span>

> [!NOTE]
> - <span data-ttu-id="0f595-110">En privat Azure Marketplace finns på klient nivå, så alla användare under klienten ser samma granskade lista.</span><span class="sxs-lookup"><span data-stu-id="0f595-110">Private Azure Marketplace is at a tenant level, so all users under the tenant will see the same curated list.</span></span>
> - <span data-ttu-id="0f595-111">Alla Microsoft-lösningar (inklusive godkända [Linux-distributioner](/azure/virtual-machines/linux/endorsed-distros)) läggs automatiskt till i privata Azure Marketplace.</span><span class="sxs-lookup"><span data-stu-id="0f595-111">All Microsoft solutions (including [Endorsed Linux Distributions](/azure/virtual-machines/linux/endorsed-distros)) are automatically added to Private Azure Marketplace.</span></span>

## <a name="assign-the-marketplace-admin-role"></a><span data-ttu-id="0f595-112">Tilldela rollen Marketplace-administratör</span><span class="sxs-lookup"><span data-stu-id="0f595-112">Assign the Marketplace admin role</span></span>

<span data-ttu-id="0f595-113">Den globala klient organisationen måste tilldela rollen **Marketplace-administratör** till den privata Azure Marketplace-administratören som ska hantera den privata lagringen.</span><span class="sxs-lookup"><span data-stu-id="0f595-113">The tenant Global administrator must assign the **Marketplace admin** role to the Private Azure Marketplace admin who will manage the private store.</span></span>

>[!IMPORTANT]
> <span data-ttu-id="0f595-114">Åtkomst till privat Azure Marketplace-hantering är bara tillgänglig för IT-administratörer med rollen Marketplace-administratör tilldelad.</span><span class="sxs-lookup"><span data-stu-id="0f595-114">Access to Private Azure Marketplace management is only available to IT admins with the Marketplace admin role assigned.</span></span>

### <a name="prerequisites"></a><span data-ttu-id="0f595-115">Förutsättningar</span><span class="sxs-lookup"><span data-stu-id="0f595-115">Prerequisites</span></span>

<span data-ttu-id="0f595-116">Dessa krav måste vara uppfyllda innan du kan tilldela rollen Marketplace-administratör till en användare i klient omfånget:</span><span class="sxs-lookup"><span data-stu-id="0f595-116">These prerequisites are required before you can assign the Marketplace Admin role to a user on the tenant scope:</span></span>

- <span data-ttu-id="0f595-117">Du har åtkomst till en **Global administratörs** användare.</span><span class="sxs-lookup"><span data-stu-id="0f595-117">You have access to a **Global administrator** user.</span></span>
- <span data-ttu-id="0f595-118">Klienten har minst en prenumeration (kan vara av valfri typ).</span><span class="sxs-lookup"><span data-stu-id="0f595-118">The tenant has at least one subscription (can be any type).</span></span>
- <span data-ttu-id="0f595-119">Den globala administratörs användaren tilldelas rollen **deltagare** eller högre för den valda prenumerationen.</span><span class="sxs-lookup"><span data-stu-id="0f595-119">The Global administrator user is assigned the **Contributor** role or higher for the chosen subscription.</span></span>

### <a name="assign-the-marketplace-admin-role-with-access-control-iam"></a><span data-ttu-id="0f595-120">Tilldela rollen Marketplace-administratör med åtkomst kontroll (IAM)</span><span class="sxs-lookup"><span data-stu-id="0f595-120">Assign the Marketplace admin role with access control (IAM)</span></span>

1. <span data-ttu-id="0f595-121">Logga in på [Azure-portalen](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="0f595-121">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
1. <span data-ttu-id="0f595-122">Välj **alla tjänster** och sedan **Marketplace**.</span><span class="sxs-lookup"><span data-stu-id="0f595-122">Select **All services** and then **Marketplace**.</span></span>
1. <span data-ttu-id="0f595-123">Välj **privat Marketplace** på menyn till vänster.</span><span class="sxs-lookup"><span data-stu-id="0f595-123">Select **Private Marketplace** from the menu on the left.</span></span>

    <span data-ttu-id="0f595-124">[![Visar meny alternativet privat Marketplace på vänster sida av Marketplace.](media/private-azure/private-marketplace.png)](media/private-azure/private-marketplace-zoom.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="0f595-124">[![Shows the private marketplace menu option on the left side of the Marketplace.](media/private-azure/private-marketplace.png)](media/private-azure/private-marketplace-zoom.png#lightbox)</span></span>

1. <span data-ttu-id="0f595-125">Välj **åtkomst kontroll (IAM)** för att tilldela rollen Marketplace-administratör.</span><span class="sxs-lookup"><span data-stu-id="0f595-125">Select **Access control (IAM)** to assign the Marketplace admin role.</span></span>

    :::image type="content" source="media/private-azure/access-control-iam.png" alt-text="Visar skärmen I A M-åtkomst kontroll.":::

1. <span data-ttu-id="0f595-127">Välj **+ Lägg till** > **Lägg till rolltilldelning**.</span><span class="sxs-lookup"><span data-stu-id="0f595-127">Select **+ Add** > **Add role assignment**.</span></span>
1. <span data-ttu-id="0f595-128">Välj **Marketplace-administratör** under **roll**.</span><span class="sxs-lookup"><span data-stu-id="0f595-128">Under **Role**, choose **Marketplace Admin**.</span></span>

    :::image type="content" source="media/private-azure/iam-role-assignment.png" alt-text="Visar menyn roll tilldelning.":::

1. <span data-ttu-id="0f595-130">Välj önskad användare i list rutan och välj sedan **Slutför**.</span><span class="sxs-lookup"><span data-stu-id="0f595-130">Select the desired user from the dropdown list, then select **Done**.</span></span>

### <a name="assign-the-marketplace-admin-role-with-powershell"></a><span data-ttu-id="0f595-131">Tilldela rollen Marketplace-administratör med PowerShell</span><span class="sxs-lookup"><span data-stu-id="0f595-131">Assign the Marketplace admin role with PowerShell</span></span>

<span data-ttu-id="0f595-132">Använd följande PowerShell-skript för att tilldela rollen Marketplace-administratör; den kräver följande parametrar:</span><span class="sxs-lookup"><span data-stu-id="0f595-132">Use the following PowerShell script to assign the Marketplace Admin role; it requires the following parameters:</span></span>

- <span data-ttu-id="0f595-133">**TenantId:** ID: t för klient organisationen i omfånget (Marketplace admin-rollen kan tilldelas i klientens omfång).</span><span class="sxs-lookup"><span data-stu-id="0f595-133">**TenantId:** The ID of the tenant in scope (Marketplace admin role is assignable on the tenant scope).</span></span>
- <span data-ttu-id="0f595-134">**SubscriptionId:** En prenumeration som den globala administratören har rollen **deltagare** eller högre tilldelad.</span><span class="sxs-lookup"><span data-stu-id="0f595-134">**SubscriptionId:** A subscription of which the global admin has **Contributor** role or higher assigned.</span></span>
- <span data-ttu-id="0f595-135">**GlobalAdminUsername:** Användar namnet för den globala administratören.</span><span class="sxs-lookup"><span data-stu-id="0f595-135">**GlobalAdminUsername:** The username of the global admin.</span></span>
- <span data-ttu-id="0f595-136">**UsernameToAssignRoleFor:** Det användar namn som Marketplace-administratörskonsolen ska tilldelas till.</span><span class="sxs-lookup"><span data-stu-id="0f595-136">**UsernameToAssignRoleFor:** The user name to which the Marketplace admin role will be assigned.</span></span>

> [!NOTE]
> <span data-ttu-id="0f595-137">För gäst användare som har bjudits in till klienten kan det ta upp till 48 timmar tills deras konto är tillgängligt för att tilldela Marketplace-administratörskonsolen.</span><span class="sxs-lookup"><span data-stu-id="0f595-137">For guest users invited to the tenant, it may take up to 48 hours until their account is available for assigning the Marketplace Admin role.</span></span> <span data-ttu-id="0f595-138">Mer information finns i [Egenskaper för en Azure Active Directory B2B-samarbets användare](/azure/active-directory/b2b/user-properties).</span><span class="sxs-lookup"><span data-stu-id="0f595-138">For more information, see [Properties of an Azure Active Directory B2B collaboration user](/azure/active-directory/b2b/user-properties).</span></span>

```PowerShell
function Assign-MarketplaceAdminRole { 
[CmdletBinding()] 
param( 
[Parameter(Mandatory)] 
[string]$TenantId, 
 
[Parameter(Mandatory)] 
[string]$SubscriptionId, 

 

[Parameter(Mandatory)] 
[string]$GlobalAdminUsername, 

 

[Parameter(Mandatory)] 
[string]$UsernameToAssignRoleFor 
) 

$MarketplaceAdminRoleDefinitionName = "Marketplace Admin" 

 

Write-Output "TenantId = $TenantId" 
Write-Output "SubscriptionId = $SubscriptionId" 
Write-Output "GlobalAdminUsername = $GlobalAdminUsername" 
Write-Output "UsernameToAssignRoleFor = $UsernameToAssignRoleFor" 

 

Write-Output "$($GlobalAdminUsername) is about to assign '$($MarketplaceAdminRoleDefinitionName)' role for $($UsernameToAssignRoleFor)" 

 

$profile = Connect-AzAccount -Tenant $TenantId -SubscriptionId $SubscriptionId

 

 
if($profile -eq $null) 
{ 
Write-Error -Message "Failed to connect to tenant and/or subscription" -ErrorAction Stop 
} 
elseif($profile.Context.Account.Id -ne $GlobalAdminUsername) 
{ 
Write-Error "Connected with $($profile.Context.Account.Id) instead of with the global admin that was specified in the script parameters, which is $($GlobalAdminUsername)" 
} 
else 
{ 
Write-Output "$($GlobalAdminUsername) was connected successfully to Tenant=$($profile.Context.Tenant), Subscription=$($profile.Context.Subscription), AccountId=$($profile.Context.Account.Id), Environment=$($profile.Context.Environment)" 
} 

 

$MarketPlaceAdminRole = Get-AzRoleDefinition $MarketplaceAdminRoleDefinitionName -Scope "/providers/Microsoft.Marketplace"

 

if($MarketPlaceAdminRole -eq $null) 
{ 
Write-Error -Message "'$($MarketplaceAdminRoleDefinitionName)' role is not available" -ErrorAction Stop 
} 
else 
{ 
Write-Output -Message "'$($MarketplaceAdminRoleDefinitionName)' role is available" 
} 

 

Write-Output -Message "About to assign '$($MarketplaceAdminRoleDefinitionName)' role for $($UsernameToAssignRoleFor)..." 

New-AzRoleAssignment -SignInName $UsernameToAssignRoleFor -RoleDefinitionName $MarketplaceAdminRoleDefinitionName -Scope "/providers/Microsoft.Marketplace" 

} 

Assign-MarketplaceAdminRole 
```

<span data-ttu-id="0f595-139">Mer information om de cmdletar som finns i AZ. Portal PowerShell-modulen finns [Microsoft Azure PowerShell: portalens instrument panels-cmdletar](/powershell/module/az.portal/).</span><span class="sxs-lookup"><span data-stu-id="0f595-139">For more information about the cmdlets contained in the Az.Portal PowerShell module, see [Microsoft Azure PowerShell: Portal Dashboard cmdlets](/powershell/module/az.portal/).</span></span>

## <a name="create-private-azure-marketplace"></a><span data-ttu-id="0f595-140">Skapa en privat Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="0f595-140">Create Private Azure Marketplace</span></span>

1. <span data-ttu-id="0f595-141">Logga in på [Azure-portalen](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="0f595-141">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="0f595-142">Välj **alla tjänster** och sedan **Marketplace**.</span><span class="sxs-lookup"><span data-stu-id="0f595-142">Select **All services** and then **Marketplace**.</span></span>

   :::image type="content" source="media/private-azure/azure-portal-marketplace.png" alt-text="Visar Azure Portal huvud fönstret.":::

3. <span data-ttu-id="0f595-144">Välj **privat Marketplace** på menyn till vänster.</span><span class="sxs-lookup"><span data-stu-id="0f595-144">Select **Private Marketplace** from the menu on the left.</span></span>

4. <span data-ttu-id="0f595-145">Välj **Kom igång** för att skapa en privat Azure Marketplace (du behöver bara göra det här en gång).</span><span class="sxs-lookup"><span data-stu-id="0f595-145">Select **Get Started** to create Private Azure Marketplace (you only have to do this once).</span></span>

    :::image type="content" source="media/private-azure/private-marketplace-get-started.png" alt-text="Visar hur du väljer huvud fönstret kom igång i Azure Portal.":::

    <span data-ttu-id="0f595-147">Om den privata Azure Marketplace redan finns för den här klienten, är **Hantera Marketplace** valt som standard.</span><span class="sxs-lookup"><span data-stu-id="0f595-147">If Private Azure Marketplace already exists for this tenant, **Manage Marketplace** will be selected by default.</span></span>

5. <span data-ttu-id="0f595-148">När du är klar har du en tom och inaktive rad privat Azure Marketplace.</span><span class="sxs-lookup"><span data-stu-id="0f595-148">Once completed you will have an empty and disabled Private Azure Marketplace.</span></span>

    :::image type="content" source="media/private-azure/new-private-marketplace.png" alt-text="Visar den tomma privata Azure Marketplace-skärmen.":::

## <a name="add-items-from-gallery"></a><span data-ttu-id="0f595-150">Lägg till objekt från galleriet</span><span class="sxs-lookup"><span data-stu-id="0f595-150">Add items from gallery</span></span>

<span data-ttu-id="0f595-151">Ett objekt är en kombination av ett erbjudande och en plan.</span><span class="sxs-lookup"><span data-stu-id="0f595-151">An item is a combination of an offer and a plan.</span></span> <span data-ttu-id="0f595-152">Du kan söka efter och lägga till objekt på sidan Hantera Marketplace.</span><span class="sxs-lookup"><span data-stu-id="0f595-152">You can search for and add items on the Manage Marketplace page.</span></span>

1. <span data-ttu-id="0f595-153">Välj **Lägg till objekt**.</span><span class="sxs-lookup"><span data-stu-id="0f595-153">Select **Add items**.</span></span>

2. <span data-ttu-id="0f595-154">Bläddra i **galleriet** eller Använd Sök fältet för att hitta det objekt som du vill använda.</span><span class="sxs-lookup"><span data-stu-id="0f595-154">Browse the **Gallery** or use the search field to find the item you want.</span></span>

    <span data-ttu-id="0f595-155">[![Visar hur du bläddrar i galleriet eller använder Sök fältet.](media/private-azure/marketplace-gallery.png)](media/private-azure/marketplace-gallery-zoom.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="0f595-155">[![Shows how to browse the gallery or use the search field.](media/private-azure/marketplace-gallery.png)](media/private-azure/marketplace-gallery-zoom.png#lightbox)</span></span>

3. <span data-ttu-id="0f595-156">Som standard kommer alla aktuella planer att läggas till i listan över godkända när du lägger till ett nytt erbjudande.</span><span class="sxs-lookup"><span data-stu-id="0f595-156">As default, when adding a new offer, all current plans will be added to the approved list.</span></span> <span data-ttu-id="0f595-157">Om du vill ändra plan urvalet innan du lägger till de valda objekten väljer du den nedrullningsbara menyn i erbjudande panelen och uppdaterar de nödvändiga planerna.</span><span class="sxs-lookup"><span data-stu-id="0f595-157">To modify the plan selection before adding the selected items, select the drop-down menu in the offer’s tile and update the required plans.</span></span>

    :::image type="content" source="media/private-azure/update-plans-400.png" alt-text="Visar hur du uppdaterar nödvändiga planer.":::

4. <span data-ttu-id="0f595-159">Välj **klar** längst ned till vänster när du har gjort dina val.</span><span class="sxs-lookup"><span data-stu-id="0f595-159">Select **Done** at the bottom-left after you've made your selections.</span></span>

>[!Note]
> <span data-ttu-id="0f595-160">**Lägg till objekt** till Marketplace kommer endast att vara tillgängligt för erbjudanden som inte kommer från Microsoft.</span><span class="sxs-lookup"><span data-stu-id="0f595-160">**Add Items** to the Marketplace will be available for non-Microsoft offers only.</span></span> <span data-ttu-id="0f595-161">Microsoft-lösningar (inklusive godkända [Linux-distributioner](/azure/virtual-machines/linux/endorsed-distros)) märks som "godkända som standard" och kan inte hanteras i privat Marketplace.</span><span class="sxs-lookup"><span data-stu-id="0f595-161">Microsoft solutions (including [Endorsed Linux Distributions](/azure/virtual-machines/linux/endorsed-distros)) will be tagged as “Approved by default” and cannot be managed in Private Marketplace.</span></span>

## <a name="edit-items-plans"></a><span data-ttu-id="0f595-162">Redigera objektets planer</span><span class="sxs-lookup"><span data-stu-id="0f595-162">Edit item's plans</span></span>

<span data-ttu-id="0f595-163">Du kan redigera ett objekts planer på sidan Hantera Marketplace.</span><span class="sxs-lookup"><span data-stu-id="0f595-163">You can edit an item's plans on the Manage Marketplace page.</span></span>

1. <span data-ttu-id="0f595-164">I kolumnen **planer** granskar du de tillgängliga planerna från List menyn för det objektet.</span><span class="sxs-lookup"><span data-stu-id="0f595-164">In the **Plans** column, review the available plans from the dropdown menu for that item.</span></span>
2. <span data-ttu-id="0f595-165">Markera eller avmarkera kryss rutorna för att välja vilka planer som ska vara tillgängliga för dina användare.</span><span class="sxs-lookup"><span data-stu-id="0f595-165">Select or clear the checkboxes to choose which plans to make available to your users.</span></span>

    :::image type="content" source="media/private-azure/edit-items.png" alt-text="Visar hur du markerar eller avmarkerar kryss rutan för det begärda objektet.":::

> [!NOTE]
> <span data-ttu-id="0f595-167">Varje erbjudande måste ha minst en plan som valts för att uppdateringen ska ske.</span><span class="sxs-lookup"><span data-stu-id="0f595-167">Each offer needs at least one plan selected for the update to occur.</span></span> <span data-ttu-id="0f595-168">Ta bort alla planer som är relaterade till ett erbjudande genom att ta bort hela erbjudandet (se nästa avsnitt).</span><span class="sxs-lookup"><span data-stu-id="0f595-168">To remove all plans related to an offer, delete the entire offer (see next section).</span></span>

## <a name="delete-offers"></a><span data-ttu-id="0f595-169">Ta bort erbjudanden</span><span class="sxs-lookup"><span data-stu-id="0f595-169">Delete offers</span></span>

<span data-ttu-id="0f595-170">På sidan Hantera marknads plats markerar du kryss rutan bredvid namnet på erbjudandet (se skärmen ovan) och väljer **ta bort objekt**.</span><span class="sxs-lookup"><span data-stu-id="0f595-170">In the Manage Marketplace page, select the check box next to the offer name (see screen above) and select **Delete items**.</span></span>

## <a name="enabledisable-private-azure-marketplace"></a><span data-ttu-id="0f595-171">Aktivera/inaktivera privat Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="0f595-171">Enable/disable Private Azure Marketplace</span></span>

<span data-ttu-id="0f595-172">På sidan Hantera Marketplace visas en av dessa banderoller som visar det aktuella läget för privat Azure Marketplace:</span><span class="sxs-lookup"><span data-stu-id="0f595-172">In the Manage Marketplace page you will see one of these banners, which show the current state of Private Azure Marketplace:</span></span>

:::image type="content" source="media/private-azure/state-disable.png" alt-text="Visar banderollen &quot;inaktivera tillstånd&quot;.":::

:::image type="content" source="media/private-azure/state-enable.png" alt-text="Visar banderollen Enable State.":::

<span data-ttu-id="0f595-175">Du kan aktivera eller inaktivera privat Azure Marketplace efter behov.</span><span class="sxs-lookup"><span data-stu-id="0f595-175">You can enable or disable Private Azure Marketplace as needed.</span></span>

- <span data-ttu-id="0f595-176">Om det är inaktiverat väljer du **aktivera privat Marketplace** för att aktivera.</span><span class="sxs-lookup"><span data-stu-id="0f595-176">If disabled, select **Enable Private Marketplace** to enable.</span></span>
- <span data-ttu-id="0f595-177">Om aktive rad väljer du **Inaktivera privat Marketplace** för att inaktivera.</span><span class="sxs-lookup"><span data-stu-id="0f595-177">If enabled, select **Disable Private Marketplace** to disable.</span></span>

## <a name="private-azure-marketplace-notification-center"></a><span data-ttu-id="0f595-178">Privat meddelande Center för Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="0f595-178">Private Azure Marketplace notification center</span></span>

<span data-ttu-id="0f595-179">Notification Center består av tre typer av meddelanden och gör att Marketplace-administratören kan vidta åtgärder baserat på aviseringen:</span><span class="sxs-lookup"><span data-stu-id="0f595-179">Notification Center consists of three types of notifications and allows the Marketplace admin to take actions based on the notification:</span></span>

- <span data-ttu-id="0f595-180">Godkännande begär Anden från användare för objekt som inte finns med i listan över godkända (se [begäran om att lägga till erbjudanden eller planer](#request-to-add-offers-or-plans) nedan).</span><span class="sxs-lookup"><span data-stu-id="0f595-180">Approval requests from users for items that are not in the approved list (see [Request to add offers or plans](#request-to-add-offers-or-plans) below).</span></span>
- <span data-ttu-id="0f595-181">Nya plan meddelanden för erbjudanden som redan har en eller flera planer i listan över godkända.</span><span class="sxs-lookup"><span data-stu-id="0f595-181">New plan notifications for offers that already have one or more plans in the approved list.</span></span>
- <span data-ttu-id="0f595-182">Tog bort plan meddelanden för objekt som finns i den godkända listan men som har tagits bort från den globala Azure Marketplace.</span><span class="sxs-lookup"><span data-stu-id="0f595-182">Removed plan notifications for items that are in the approved list but were removed from the global Azure Marketplace.</span></span>

<span data-ttu-id="0f595-183">För att komma åt meddelande centret:</span><span class="sxs-lookup"><span data-stu-id="0f595-183">To access the notification center:</span></span>

1. <span data-ttu-id="0f595-184">Välj **meddelanden** på menyn på den vänstra sidan.</span><span class="sxs-lookup"><span data-stu-id="0f595-184">Select **Notifications** from the left-side menu.</span></span>

    <span data-ttu-id="0f595-185">[![Visar menyn meddelanden.](media/private-azure/marketplace-notifications-small.png)](media/private-azure/marketplace-notifications.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="0f595-185">[![Shows the Notifications menu.](media/private-azure/marketplace-notifications-small.png)](media/private-azure/marketplace-notifications.png#lightbox)</span></span>

1. <span data-ttu-id="0f595-186">Välj menyn med tre punkter för fler åtgärder.</span><span class="sxs-lookup"><span data-stu-id="0f595-186">Select the ellipsis menu for more actions.</span></span>

    :::image type="content" source="media/private-azure/notifications-more-options.png" alt-text="Visar meny resultatet fler alternativ.":::

1. <span data-ttu-id="0f595-188">För begäran om att **Visa förfrågningar** öppnar formuläret begäran om godkännande där du kan granska alla användar förfrågningar för det aktuella erbjudandet.</span><span class="sxs-lookup"><span data-stu-id="0f595-188">For plan requests, **Show requests** opens the approval request form where you can review all user requests for the specific offer.</span></span>
1. <span data-ttu-id="0f595-189">Välj **Godkänn** eller **avvisa**.</span><span class="sxs-lookup"><span data-stu-id="0f595-189">Select **Approve** or **Reject**.</span></span>

    <span data-ttu-id="0f595-190">[![Visar alternativen Godkänn och avvisa.](media/private-azure/notifications-approve-reject-small.png)](media/private-azure/notifications-approve-reject.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="0f595-190">[![Shows the approve and reject options.](media/private-azure/notifications-approve-reject-small.png)](media/private-azure/notifications-approve-reject.png#lightbox)</span></span>

1. <span data-ttu-id="0f595-191">Välj den plan som du vill godkänna på den nedrullningsbara menyn.</span><span class="sxs-lookup"><span data-stu-id="0f595-191">Select the plan to approve from the drop-down menu.</span></span>
1. <span data-ttu-id="0f595-192">Lägg till en kommentar och välj **Skicka**.</span><span class="sxs-lookup"><span data-stu-id="0f595-192">Add a comment and select **Submit**.</span></span>

## <a name="browsing-private-azure-marketplace"></a><span data-ttu-id="0f595-193">Bläddra i privat Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="0f595-193">Browsing Private Azure Marketplace</span></span>

<span data-ttu-id="0f595-194">När privat Azure Marketplace är aktiverat ser användarna vilka planer som Marketplace-administratören har godkänt.</span><span class="sxs-lookup"><span data-stu-id="0f595-194">When Private Azure Marketplace is enabled, users will see which plans the Marketplace admin has approved.</span></span>

- <span data-ttu-id="0f595-195">Ett grönt **godkänt** meddelande anger ett erbjudande för partner (inte Microsoft) som är godkänt.</span><span class="sxs-lookup"><span data-stu-id="0f595-195">A green **Approved** notice indicates a Partner (non-Microsoft) offer that is approved.</span></span>
- <span data-ttu-id="0f595-196">Ett blått **godkänt** meddelande anger ett Microsoft-erbjudande (inklusive godkända [Linux-distributioner](/azure/virtual-machines/linux/endorsed-distros)) som är godkänt.</span><span class="sxs-lookup"><span data-stu-id="0f595-196">A blue **Approved** notice indicates a Microsoft offer (including [Endorsed Linux distributions](/azure/virtual-machines/linux/endorsed-distros)) that is approved.</span></span>

<span data-ttu-id="0f595-197">Användare kan filtrera mellan erbjudanden som är och inte är godkända:</span><span class="sxs-lookup"><span data-stu-id="0f595-197">Users can filter between offers that are and are not approved:</span></span>

<span data-ttu-id="0f595-198">[![Visar filtrerings alternativet.](media/private-azure/filter-option-small.png)](media/private-azure/filter-option.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="0f595-198">[![Shows the filtering option.](media/private-azure/filter-option-small.png)](media/private-azure/filter-option.png#lightbox)</span></span>

## <a name="buy-or-deploy-in-private-azure-marketplace"></a><span data-ttu-id="0f595-199">Köp eller distribuera i privat Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="0f595-199">Buy or deploy in Private Azure Marketplace</span></span>

<span data-ttu-id="0f595-200">Även om produkt informationens sid upplevelse liknar den globala Azure Marketplace finns det tre privata Azure Marketplace-olika scenarier.</span><span class="sxs-lookup"><span data-stu-id="0f595-200">While the product details page experience is similar to the global Azure Marketplace, there are three Private Azure Marketplace specific scenarios.</span></span>

- <span data-ttu-id="0f595-201">När en användare väljer en godkänd plan aktive ras knappen **skapa** :</span><span class="sxs-lookup"><span data-stu-id="0f595-201">When a user selects an approved plan, the **Create** button is enabled:</span></span>

    <span data-ttu-id="0f595-202">[![Visar en banderoll för erbjudandet om att en plan kan skapas.](media/private-azure/button-create-enabled-small.png)](media/private-azure/button-create-enabled.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="0f595-202">[![Shows the offer banner noting a plan can be created.](media/private-azure/button-create-enabled-small.png)](media/private-azure/button-create-enabled.png#lightbox)</span></span>

- <span data-ttu-id="0f595-203">Om ett val av produkt plan inte visas på sidan produkt information men administratören har godkänt en eller flera planer, visar en banderoll vilka planer som godkänns och knappen **skapa** är aktive rad:</span><span class="sxs-lookup"><span data-stu-id="0f595-203">If a product plan selection does not appear in the product details page but the admin approved one or more plans, a banner notes which plans are approved and the **Create** button is enabled:</span></span>

    <span data-ttu-id="0f595-204">[![Visar banderollen erbjudande om att en plan kan skapas och Visa tillgängliga planer.](media/private-azure/button-create-enabled-and-plans-small.png)](media/private-azure/button-create-enabled-and-plans.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="0f595-204">[![Shows the offer banner noting that a plan can be created and showing available plans.](media/private-azure/button-create-enabled-and-plans-small.png)](media/private-azure/button-create-enabled-and-plans.png#lightbox)</span></span>

- <span data-ttu-id="0f595-205">När en användare väljer en icke godkänd plan, visar en banderoll om planen är inte godkänd och knappen **skapa** är inaktive rad.</span><span class="sxs-lookup"><span data-stu-id="0f595-205">When a user selects a non-approved plan, a banner notes the plan as not approved and the **Create** button is disabled.</span></span> <span data-ttu-id="0f595-206">Användaren kan fortfarande begära att lägga till planen i den godkända listan (se nästa avsnitt).</span><span class="sxs-lookup"><span data-stu-id="0f595-206">The user can still request to add the plan to the approved list (see next section).</span></span>

## <a name="request-to-add-offers-or-plans"></a><span data-ttu-id="0f595-207">Begäran om att lägga till erbjudanden eller planer</span><span class="sxs-lookup"><span data-stu-id="0f595-207">Request to add offers or plans</span></span>

<span data-ttu-id="0f595-208">Du kan begära att lägga till ett offentligt erbjudande eller en plan som inte är godkänd i den privata Azure Marketplace.</span><span class="sxs-lookup"><span data-stu-id="0f595-208">You can request to add a public offer or plan that is not currently approved in the Private Azure Marketplace.</span></span>

1. <span data-ttu-id="0f595-209">Välj **begär att lägga till** i banderollen för att öppna **formuläret** åtkomstbegäran.</span><span class="sxs-lookup"><span data-stu-id="0f595-209">Select **Request to add** in the banner to open the **Access request form**.</span></span>

    <span data-ttu-id="0f595-210">[![Visar banderollen med länken "begär att lägga till".](media/private-azure/request-banner-small.png)](media/private-azure/request-banner.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="0f595-210">[![Shows the banner with the 'Request to add' link.](media/private-azure/request-banner-small.png)](media/private-azure/request-banner.png#lightbox)</span></span>

    <span data-ttu-id="0f595-211">[![Visar formuläret för åtkomstbegäran för erbjudanden eller planer.](media/private-azure/access-request-form-small.png)](media/private-azure/access-request-form.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="0f595-211">[![Shows the access request form for offers or plans.](media/private-azure/access-request-form-small.png)](media/private-azure/access-request-form.png#lightbox)</span></span>

1. <span data-ttu-id="0f595-212">Välj vilka planer som ska läggas till i begäran (**alla planer** meddelar Marketplace-administratören att du inte har någon preferens för en prenumeration i ett erbjudande).</span><span class="sxs-lookup"><span data-stu-id="0f595-212">Select which plans to add to the request (**Any Plan** tells the Marketplace admin that you don't have a preference for a plan within an offer).</span></span>

1. <span data-ttu-id="0f595-213">Lägg till en **motivering** och välj **begäran** för att skicka in din begäran.</span><span class="sxs-lookup"><span data-stu-id="0f595-213">Add a **Justification** and select **Request** to submit your request.</span></span>
  
    <span data-ttu-id="0f595-214">[![Visar formuläret för åtkomstbegäran för erbjudanden eller planer med exempel poster.](media/private-azure/access-request-form-filled-small.png)](media/private-azure/access-request-form-filled.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="0f595-214">[![Shows the access request form for offers or plans with sample entries.](media/private-azure/access-request-form-filled-small.png)](media/private-azure/access-request-form-filled.png#lightbox)</span></span>

1. <span data-ttu-id="0f595-215">En indikation för en väntande begäran visas i formuläret åtkomstbegäran med ett alternativ för att **återkalla begäran**.</span><span class="sxs-lookup"><span data-stu-id="0f595-215">An indication for a pending request will appear in the Access request form with an option to **Withdraw request**.</span></span>

    <span data-ttu-id="0f595-216">[![Visar en lista över godkända eller väntande planer med länken återkalla begäran.](media/private-azure/approved-pending-plans-small.png)](media/private-azure/approved-pending-plans.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="0f595-216">[![Shows a list of approved or pending plans with Withdraw Request link.](media/private-azure/approved-pending-plans-small.png)](media/private-azure/approved-pending-plans.png#lightbox)</span></span>

> [!NOTE]
> <span data-ttu-id="0f595-217">När den har skickats skickas formuläret för godkännande förfrågning till [meddelande centret](#private-azure-marketplace-notification-center) för Marketplace-administratören för att granska begäran och vidta åtgärder.</span><span class="sxs-lookup"><span data-stu-id="0f595-217">Once submitted, the approval request form will be sent to the [Notification Center](#private-azure-marketplace-notification-center) for the Marketplace admin to review the request and take action.</span></span>

## <a name="frequently-asked-questions-faqs"></a><span data-ttu-id="0f595-218">Vanliga frågor och svar</span><span class="sxs-lookup"><span data-stu-id="0f595-218">Frequently Asked Questions (FAQs)</span></span>

#### <a name="i-am-already-blocking-marketplace-third-party-application-through-azure-policy-how-is-this-different"></a><span data-ttu-id="0f595-219">Jag blockerar redan Marketplace-program från tredje part via Azure Policy.</span><span class="sxs-lookup"><span data-stu-id="0f595-219">I am already blocking Marketplace third-party application through Azure Policy.</span></span> <span data-ttu-id="0f595-220">Hur skiljer sig detta?</span><span class="sxs-lookup"><span data-stu-id="0f595-220">How is this different?</span></span>

<span data-ttu-id="0f595-221">Det finns för närvarande två sätt att begränsa tjänster från tredje part på Marketplace:</span><span class="sxs-lookup"><span data-stu-id="0f595-221">There are currently two ways to restrict third-party services in Marketplace:</span></span>

1. <span data-ttu-id="0f595-222">I EA-portalen eller Azure Portal inaktiverar du tjänster från tredje part eller begränsar till "kostnads fri eller BYOL SKU: er".</span><span class="sxs-lookup"><span data-stu-id="0f595-222">Through EA portal or the Azure portal, disable third-party services or restrict to “Free or BYOL SKUs only”.</span></span>

    :::image type="content" source="media/private-azure/disable-services.png" alt-text="Visar hur du begränsar tjänster i Azure Portal.":::

    :::image type="content" source="media/private-azure/disable-services-other-view.png" alt-text="Visar hur du begränsar tjänster i E-portalen.":::

2. <span data-ttu-id="0f595-225">Skapa en Azure-princip för att bara tillåta vissa virtuella datorer.</span><span class="sxs-lookup"><span data-stu-id="0f595-225">Create an Azure policy to only allow specific VMs.</span></span> <span data-ttu-id="0f595-226">Mer information om hur du tillämpar principer för virtuella Windows-datorer finns i [tillämpa principer på virtuella Windows-datorer med Azure Resource Manager](/azure/virtual-machines/windows/policy).</span><span class="sxs-lookup"><span data-stu-id="0f595-226">For details on how to enforce policy to Windows VMs, see [Apply policies to Windows VMs with Azure Resource Manager](/azure/virtual-machines/windows/policy).</span></span>

<span data-ttu-id="0f595-227">Privata Azure Marketplace ger större flexibilitet när det gäller att begränsa och tillåta vissa erbjudanden och planer.</span><span class="sxs-lookup"><span data-stu-id="0f595-227">Private Azure Marketplace allows more flexibility on restricting and allowing specific offers and plans.</span></span> <span data-ttu-id="0f595-228">Det informerar slutanvändarna om tillgänglighet för distribution i Marketplace-galleriet även innan de försöker distribuera tjänster från tredje part.</span><span class="sxs-lookup"><span data-stu-id="0f595-228">It informs end users on the availability for deployment in the marketplace gallery even before they try to deploy third-party services.</span></span> <span data-ttu-id="0f595-229">Om du vill tillåta distribution av tjänster från tredje part ställer du in Azure Marketplace till på/aktiverat i EA-portalen och Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="0f595-229">To allow deployment of third-party services, set Azure Marketplace to On/Enabled in EA Portal and the Azure portal.</span></span>

- <span data-ttu-id="0f595-230">Privata Azure Marketplace kan granska partner lösningar som inte är begränsade till virtuella datorer.</span><span class="sxs-lookup"><span data-stu-id="0f595-230">Private Azure Marketplace can curate partner solutions not limited to virtual machines.</span></span>
- <span data-ttu-id="0f595-231">Privata Azure Marketplace kan granska på plannivå och kan också ange "nuvarande och framtida plan".</span><span class="sxs-lookup"><span data-stu-id="0f595-231">Private Azure Marketplace can curate at the plan level and can also set “Current and future plan”.</span></span>
- <span data-ttu-id="0f595-232">Privata Azure Marketplace kan informera slutanvändarna om vad som kan och inte kan distribueras.</span><span class="sxs-lookup"><span data-stu-id="0f595-232">Private Azure Marketplace can inform the end users up front on what can and cannot be deployed.</span></span>

#### <a name="whats-the-difference-between-a-private-offer-and-private-azure-marketplace"></a><span data-ttu-id="0f595-233">Vad är skillnaden mellan ett privat erbjudande och en privat Azure Marketplace?</span><span class="sxs-lookup"><span data-stu-id="0f595-233">What's the difference between a Private Offer and Private Azure Marketplace?</span></span>

<span data-ttu-id="0f595-234">Med ett **privat erbjudande** kan utgivare skapa planer som endast är synliga för riktade kunder.</span><span class="sxs-lookup"><span data-stu-id="0f595-234">A **Private Offer** lets publishers create plans that are only visible to targeted customers.</span></span> <span data-ttu-id="0f595-235">Detta gör det möjligt för dem att dela anpassade lösningar med förhandlad prissättning, privata villkor och specialiserade konfigurationer.</span><span class="sxs-lookup"><span data-stu-id="0f595-235">This lets them privately share customized solutions with negotiated pricing, private terms and conditions, and specialized configurations.</span></span> <span data-ttu-id="0f595-236">Mer information finns [i privata erbjudanden på den kommersiella marknaden](/azure/marketplace/private-offers).</span><span class="sxs-lookup"><span data-stu-id="0f595-236">For details, see [Private offers in the commercial marketplace](/azure/marketplace/private-offers).</span></span>

<span data-ttu-id="0f595-237">Med den **privata Azure Marketplace** i Azure Portal kan administratörer godkänna vilka lösningar från tredje part som användarna kan distribuera.</span><span class="sxs-lookup"><span data-stu-id="0f595-237">**Private Azure Marketplace** in the Azure portal lets administrators pre-approve which third-party solutions their users can deploy.</span></span> <span data-ttu-id="0f595-238">Med en privat Azure Marketplace kan användarna dra nytta av fördelarna med Azure Marketplace genom att söka efter, köpa och distribuera kompatibla erbjudanden.</span><span class="sxs-lookup"><span data-stu-id="0f595-238">With a Private Azure Marketplace, users can enjoy the benefits of Azure Marketplace by finding, buying, and deploying compliant offers.</span></span> <span data-ttu-id="0f595-239">För att hantera prenumerations privata erbjudanden i privat Marketplace måste Marketplace-administratören ha minst "Läs"-rollen för den aktuella prenumerationen.</span><span class="sxs-lookup"><span data-stu-id="0f595-239">To manage subscription-based Private Offers in Private Marketplace, the Marketplace admin must have a minimum of “read” role on the specific subscription.</span></span>

#### <a name="i-added-a-private-offer-to-the-private-azure-marketplace-why-is-it-not-showing-in-the-manage-marketplace-tab"></a><span data-ttu-id="0f595-240">Jag har lagt till ett privat erbjudande på den privata Azure Marketplace, varför visas det inte på fliken Hantera Marketplace?</span><span class="sxs-lookup"><span data-stu-id="0f595-240">I added a Private Offer to the Private Azure Marketplace, why is it not showing in the manage marketplace tab?</span></span>

<span data-ttu-id="0f595-241">Prenumerations privata erbjudanden visas bara för de listade prenumerationerna i inställningarna för privata erbjudanden.</span><span class="sxs-lookup"><span data-stu-id="0f595-241">Subscription-based Private Offers are visible only for the listed subscriptions in the Private Offer settings.</span></span> <span data-ttu-id="0f595-242">Om du vill visa det privata erbjudandet ser du till att det globala prenumerations filtret visar alla prenumerationer.</span><span class="sxs-lookup"><span data-stu-id="0f595-242">To view the Private Offer, ensure the global subscription filter is showing all the subscriptions.</span></span>

<span data-ttu-id="0f595-243">[![Visar filtret för privata marknads platser.](media/private-azure/private-marketplace-filter.png)](media/private-azure/private-marketplace-filter.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="0f595-243">[![Shows the private marketplace filter.](media/private-azure/private-marketplace-filter.png)](media/private-azure/private-marketplace-filter.png#lightbox)</span></span>

#### <a name="can-we-include-custom-images-in-private-azure-marketplace"></a><span data-ttu-id="0f595-244">Kan vi inkludera anpassade bilder i privata Azure Marketplace?</span><span class="sxs-lookup"><span data-stu-id="0f595-244">Can we include custom images in Private Azure Marketplace?</span></span>

<span data-ttu-id="0f595-245">Nej.</span><span class="sxs-lookup"><span data-stu-id="0f595-245">No.</span></span> <span data-ttu-id="0f595-246">Med privata Azure Marketplace kan IT-administratörer hantera och granska lösningar från tredje part från globala Azure Marketplace.</span><span class="sxs-lookup"><span data-stu-id="0f595-246">Private Azure Marketplace allows any IT administrator to manage and curate third-party solutions from global Azure Marketplace.</span></span> <span data-ttu-id="0f595-247">Eftersom anpassade avbildningar inte finns på globala Azure Marketplace kan IT-administratören inte välja och välja anpassade avbildningar.</span><span class="sxs-lookup"><span data-stu-id="0f595-247">Since custom images are not on global Azure Marketplace, the IT administrator cannot pick and choose your custom images.</span></span> <span data-ttu-id="0f595-248">Använd [delat avbildnings Galleri](/azure/virtual-machines/shared-image-galleries)om du vill dela anpassade avbildningar.</span><span class="sxs-lookup"><span data-stu-id="0f595-248">If you would like to share custom images, use [Shared Image Gallery](/azure/virtual-machines/shared-image-galleries).</span></span>

1. <span data-ttu-id="0f595-249">Steg-för-steg-guide skapa ett delat bild galleri (SIG) ([CLI](/azure/virtual-machines/shared-images-cli), [PowerShell](/azure/virtual-machines/shared-images-powershell)).</span><span class="sxs-lookup"><span data-stu-id="0f595-249">Step-by-step guide Create a Shared Image Gallery (SIG) ([CLI](/azure/virtual-machines/shared-images-cli), [PowerShell](/azure/virtual-machines/shared-images-powershell)).</span></span>
2. <span data-ttu-id="0f595-250">Skapa en avbildnings definition i en SIG.</span><span class="sxs-lookup"><span data-stu-id="0f595-250">Create an image definition within a SIG.</span></span> <span data-ttu-id="0f595-251">Kunden bör välja **generaliserad** för fältet OS-tillstånd.</span><span class="sxs-lookup"><span data-stu-id="0f595-251">Customer should choose **Generalized** for the OS-state field.</span></span> <span data-ttu-id="0f595-252">([CLI](/azure/virtual-machines/image-version-managed-image-cli#create-an-image-definition), [PowerShell](/azure/virtual-machines/image-version-vm-powershell#create-an-image-definition)).</span><span class="sxs-lookup"><span data-stu-id="0f595-252">([CLI](/azure/virtual-machines/image-version-managed-image-cli#create-an-image-definition), [PowerShell](/azure/virtual-machines/image-version-vm-powershell#create-an-image-definition)).</span></span>
3. <span data-ttu-id="0f595-253">Placera hanterade avbildningar i det delade bild galleriet ([CLI](/azure/virtual-machines/image-version-managed-image-cli), [PowerShell](/azure/virtual-machines/image-version-managed-image-powershell)).</span><span class="sxs-lookup"><span data-stu-id="0f595-253">Bring managed image into the Shared Image Gallery ([CLI](/azure/virtual-machines/image-version-managed-image-cli), [PowerShell](/azure/virtual-machines/image-version-managed-image-powershell)).</span></span>
4. <span data-ttu-id="0f595-254">Avbildningarna för SIG-VM finns i en prenumeration.</span><span class="sxs-lookup"><span data-stu-id="0f595-254">The SIG VM images would reside in one subscription.</span></span> <span data-ttu-id="0f595-255">Använd en app-registrering ([CLI](/azure/virtual-machines/linux/share-images-across-tenants), [PowerShell](/azure/virtual-machines/windows/share-images-across-tenants)) för att göra det tillgängligt för andra prenumerationer.</span><span class="sxs-lookup"><span data-stu-id="0f595-255">To make it available to other subscriptions, use an app registration ([CLI](/azure/virtual-machines/linux/share-images-across-tenants), [PowerShell](/azure/virtual-machines/windows/share-images-across-tenants)).</span></span>

#### <a name="why-do-i-see-some-offers-approved-by-default-even-though-the-publisher-is-not-microsoft"></a><span data-ttu-id="0f595-256">Varför visas vissa erbjudanden som har **godkänts som standard** även om utgivaren inte är Microsoft?</span><span class="sxs-lookup"><span data-stu-id="0f595-256">Why do I see some offers **Approved by default** even though the publisher is not Microsoft?</span></span>

<span data-ttu-id="0f595-257">Microsoft stöder Linux och teknik med öppen källkod i Azure.</span><span class="sxs-lookup"><span data-stu-id="0f595-257">Microsoft supports Linux and open-source technology in Azure.</span></span> <span data-ttu-id="0f595-258">Godkända [Linux-distributioner](/azure/virtual-machines/linux/endorsed-distros) stöds i Azure och priset är integrerat i virtuella datorer.</span><span class="sxs-lookup"><span data-stu-id="0f595-258">[Endorsed Linux distributions](/azure/virtual-machines/linux/endorsed-distros) are supported on Azure and the price is integrated in virtual machines.</span></span> <span data-ttu-id="0f595-259">Eftersom Azure Linux-agenten redan är förinstallerad på Azure Marketplace, behandlas det som ett Microsoft-erbjudande.</span><span class="sxs-lookup"><span data-stu-id="0f595-259">Because Azure Linux Agent is already pre-installed on Azure Marketplace, it is treated like a Microsoft offer.</span></span> <span data-ttu-id="0f595-260">Eftersom Microsoft-erbjudanden har godkänts som standard kan inte godkända Linux-distributioner hanteras i privata Azure Marketplace och godkänns som standard.</span><span class="sxs-lookup"><span data-stu-id="0f595-260">Since Microsoft offers are approved by default, endorsed Linux distributions cannot be managed in Private Azure Marketplace and are approved by default.</span></span>

## <a name="contact-support"></a><span data-ttu-id="0f595-261">Kontakta supporten</span><span class="sxs-lookup"><span data-stu-id="0f595-261">Contact support</span></span>

- <span data-ttu-id="0f595-262">Besök [Microsoft Q&A](/answers/products/)för support för Azure Marketplace.</span><span class="sxs-lookup"><span data-stu-id="0f595-262">For Azure Marketplace support, visit [Microsoft Q&A](/answers/products/).</span></span>