---
title: Skapa och hantera privat Azure Marketplace i Azure Portal
description: Lär dig mer om att skapa och hantera privata Azure Marketplace (för hands version) i Azure Portal. Med privat Azure Marketplace (för hands version) kan administratörer styra vilka lösningar från tredje part som användarna kan använda.
ms.prod: marketplace-customer
ms.topic: how-to
author: msjogarrig
ms.author: jogarrig
ms.date: 12/22/2020
ms.openlocfilehash: 09f7bcb29dc619e4e31c0aa3d5c73fade5218819
ms.sourcegitcommit: 30d154cdf40aa75400be7805cd9b2685b66a1382
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 12/24/2020
ms.locfileid: "97760824"
---
# <a name="create-and-manage-private-azure-marketplace-preview-in-the-azure-portal"></a><span data-ttu-id="97cdf-104">Skapa och hantera privat Azure Marketplace (för hands version) i Azure Portal</span><span class="sxs-lookup"><span data-stu-id="97cdf-104">Create and manage Private Azure Marketplace (preview) in the Azure portal</span></span>

<span data-ttu-id="97cdf-105">Med privat Azure Marketplace (för hands version) kan administratörer styra vilka lösningar från tredje part som användarna kan använda.</span><span class="sxs-lookup"><span data-stu-id="97cdf-105">Private Azure Marketplace (preview) lets administrators govern which third-party solutions their users can use.</span></span> <span data-ttu-id="97cdf-106">Det gör det genom att låta dig distribuera endast erbjudanden som du godkänner och som uppfyller företagets principer.</span><span class="sxs-lookup"><span data-stu-id="97cdf-106">It does this by allowing you to deploy only offers that you approve and that comply with your enterprise's policies.</span></span> <span data-ttu-id="97cdf-107">Med en privat Azure Marketplace kan användarna söka i onlinebutiken efter kompatibla erbjudanden för köp och distribution.</span><span class="sxs-lookup"><span data-stu-id="97cdf-107">With Private Azure Marketplace, your users can search the online store for compliant offers to purchase and deploy.</span></span> 

<span data-ttu-id="97cdf-108">Som Marketplace-administratör (tilldelad roll) börjar du med en inaktive rad och en tom privat lagrings plats där du kan lägga till godkända erbjudanden och planer.</span><span class="sxs-lookup"><span data-stu-id="97cdf-108">As a Marketplace admin (assigned role), you will start with a disabled and empty Private Store where you can add your approved offers and plans.</span></span> <span data-ttu-id="97cdf-109">Den här artikeln beskriver hur du skapar, hanterar och aktiverar privat Azure Marketplace för dina användare.</span><span class="sxs-lookup"><span data-stu-id="97cdf-109">This article explains how to create, manage, and enable Private Azure Marketplace for your users.</span></span>

<span data-ttu-id="97cdf-110">Obs!</span><span class="sxs-lookup"><span data-stu-id="97cdf-110">Notes:</span></span>

- <span data-ttu-id="97cdf-111">En privat Azure Marketplace finns på klient nivå, så alla användare under klienten ser samma granskade lista.</span><span class="sxs-lookup"><span data-stu-id="97cdf-111">Private Azure Marketplace is at a tenant level, so all users under the tenant will see the same curated list.</span></span>
- <span data-ttu-id="97cdf-112">Alla Microsoft-lösningar läggs automatiskt till i privata Azure Marketplace.</span><span class="sxs-lookup"><span data-stu-id="97cdf-112">All Microsoft solutions are automatically added to Private Azure Marketplace.</span></span>

## <a name="assign-the-marketplace-admin-role"></a><span data-ttu-id="97cdf-113">Tilldela rollen Marketplace-administratör</span><span class="sxs-lookup"><span data-stu-id="97cdf-113">Assign the Marketplace admin role</span></span>

<span data-ttu-id="97cdf-114">Den globala klient organisationen måste tilldela rollen **Marketplace-administratör** till den privata Azure Marketplace-administratören som ska hantera den privata lagringen.</span><span class="sxs-lookup"><span data-stu-id="97cdf-114">The tenant Global administrator must assign the **Marketplace admin** role to the Private Azure Marketplace admin who will manage the private store.</span></span>

>[!IMPORTANT]
> <span data-ttu-id="97cdf-115">Åtkomst till privat Azure Marketplace-hantering är bara tillgänglig för IT-administratörer med rollen Marketplace-administratör tilldelad.</span><span class="sxs-lookup"><span data-stu-id="97cdf-115">Access to Private Azure Marketplace management is only available to IT admins with the Marketplace admin role assigned.</span></span>

### <a name="prerequisites"></a><span data-ttu-id="97cdf-116">Förutsättningar</span><span class="sxs-lookup"><span data-stu-id="97cdf-116">Prerequisites</span></span>

<span data-ttu-id="97cdf-117">Du måste uppfylla dessa krav innan du kan tilldela rollen Marketplace-administratör till en användare i klient omfånget:</span><span class="sxs-lookup"><span data-stu-id="97cdf-117">You must meet these prerequisites before you can assign the Marketplace Admin role to a user on the tenant scope:</span></span>

- <span data-ttu-id="97cdf-118">Du har åtkomst till en **Global administratörs** användare.</span><span class="sxs-lookup"><span data-stu-id="97cdf-118">You have access to a **Global administrator** user.</span></span>
- <span data-ttu-id="97cdf-119">Klienten har minst en prenumeration (kan vara av valfri typ).</span><span class="sxs-lookup"><span data-stu-id="97cdf-119">The tenant has at least one subscription (can be any type).</span></span>
- <span data-ttu-id="97cdf-120">Den globala administratörs användaren tilldelas rollen **deltagare** eller högre för den valda prenumerationen.</span><span class="sxs-lookup"><span data-stu-id="97cdf-120">The Global administrator user is assigned the **Contributor** role or higher for the chosen subscription.</span></span>

### <a name="assign-the-marketplace-admin-role-with-iam"></a><span data-ttu-id="97cdf-121">Tilldela rollen Marketplace-administratör med IAM</span><span class="sxs-lookup"><span data-stu-id="97cdf-121">Assign the Marketplace admin role with IAM</span></span>

1. <span data-ttu-id="97cdf-122">Logga in på [Azure-portalen](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="97cdf-122">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
1. <span data-ttu-id="97cdf-123">Välj **alla tjänster** och sedan **Marketplace**.</span><span class="sxs-lookup"><span data-stu-id="97cdf-123">Select **All services** and then **Marketplace**.</span></span>

   :::image type="content" source="media/private-azure/azure-portal-marketplace.png" alt-text="Azure Portal huvud fönstret.":::

3. <span data-ttu-id="97cdf-125">Välj **privat Marketplace** från alternativen till vänster.</span><span class="sxs-lookup"><span data-stu-id="97cdf-125">Select **Private Marketplace** from the options on the left.</span></span>
1. <span data-ttu-id="97cdf-126">Välj **åtkomst kontroll (IAM)** för att tilldela rollen Marketplace-administratör.</span><span class="sxs-lookup"><span data-stu-id="97cdf-126">Select **Access control (IAM)** to assign the Marketplace admin role.</span></span>

    :::image type="content" source="media/private-azure/access-control-iam.png" alt-text="Skärm bilden IAM Access Control.":::

1. <span data-ttu-id="97cdf-128">Välj **+ Lägg till** > **Lägg till rolltilldelning**.</span><span class="sxs-lookup"><span data-stu-id="97cdf-128">Select **+ Add** > **Add role assignment**.</span></span>
1. <span data-ttu-id="97cdf-129">Välj **Marketplace-administratör** under **roll**.</span><span class="sxs-lookup"><span data-stu-id="97cdf-129">Under **Role**, choose **Marketplace Admin**.</span></span>

    :::image type="content" source="media/private-azure/iam-role-assignment.png" alt-text="Menyn roll tilldelning.":::

1. <span data-ttu-id="97cdf-131">Välj önskad användare i list rutan och välj sedan **Slutför**.</span><span class="sxs-lookup"><span data-stu-id="97cdf-131">Select the desired user from the dropdown list, then select **Done**.</span></span>

### <a name="assign-the-marketplace-admin-role-with-powershell"></a><span data-ttu-id="97cdf-132">Tilldela rollen Marketplace-administratör med PowerShell</span><span class="sxs-lookup"><span data-stu-id="97cdf-132">Assign the Marketplace admin role with PowerShell</span></span>

<span data-ttu-id="97cdf-133">Använd följande PowerShell-skript för att tilldela rollen Marketplace-administratör; den kräver följande parametrar:</span><span class="sxs-lookup"><span data-stu-id="97cdf-133">Use the following PowerShell script to assign the Marketplace Admin role; it requires the following parameters:</span></span>

- <span data-ttu-id="97cdf-134">**TenantId:** ID: t för klient organisationen i omfånget (Marketplace admin-rollen kan tilldelas i klientens omfång).</span><span class="sxs-lookup"><span data-stu-id="97cdf-134">**TenantId:** The ID of the tenant in scope (Marketplace admin role is assignable on the tenant scope).</span></span>
- <span data-ttu-id="97cdf-135">**SubscriptionId:** En prenumeration som den globala administratören har rollen **deltagare** eller högre tilldelad.</span><span class="sxs-lookup"><span data-stu-id="97cdf-135">**SubscriptionId:** A subscription of which the global admin has **Contributor** role or higher assigned.</span></span>
- <span data-ttu-id="97cdf-136">**GlobalAdminUsername:** Användar namnet för den globala administratören.</span><span class="sxs-lookup"><span data-stu-id="97cdf-136">**GlobalAdminUsername:** The username of the global admin.</span></span>
- <span data-ttu-id="97cdf-137">**UsernameToAssignRoleFor:** Det användar namn som Marketplace-administratörskonsolen ska tilldelas till.</span><span class="sxs-lookup"><span data-stu-id="97cdf-137">**UsernameToAssignRoleFor:** The user name to which the Marketplace admin role will be assigned.</span></span>

> [!NOTE]
> <span data-ttu-id="97cdf-138">För gäst användare som har bjudits in till klienten kan det ta upp till 48 timmar tills deras konto är tillgängligt för att tilldela Marketplace-administratörskonsolen.</span><span class="sxs-lookup"><span data-stu-id="97cdf-138">For guest users invited to the tenant, it may take up to 48 hours until their account is available for assigning the Marketplace admin role.</span></span> <span data-ttu-id="97cdf-139">Mer information finns i [Egenskaper för en Azure Active Directory B2B-samarbets användare](/azure/active-directory/b2b/user-properties).</span><span class="sxs-lookup"><span data-stu-id="97cdf-139">For more information, see [Properties of an Azure Active Directory B2B collaboration user](/azure/active-directory/b2b/user-properties).</span></span>

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

<span data-ttu-id="97cdf-140">Mer information om de cmdletar som finns i AZ. Portal PowerShell-modulen finns [Microsoft Azure PowerShell: portalens instrument panels-cmdletar](/powershell/module/az.portal/).</span><span class="sxs-lookup"><span data-stu-id="97cdf-140">For more information about the cmdlets contained in the Az.Portal PowerShell module, see [Microsoft Azure PowerShell: Portal Dashboard cmdlets](/powershell/module/az.portal/).</span></span>

## <a name="create-private-azure-marketplace"></a><span data-ttu-id="97cdf-141">Skapa en privat Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="97cdf-141">Create Private Azure Marketplace</span></span>

1. <span data-ttu-id="97cdf-142">Logga in på [Azure-portalen](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="97cdf-142">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="97cdf-143">Välj **alla tjänster** och sedan **Marketplace**.</span><span class="sxs-lookup"><span data-stu-id="97cdf-143">Select **All services** and then **Marketplace**.</span></span>

   :::image type="content" source="media/private-azure/azure-portal-marketplace.png" alt-text="Azure Portal huvud fönstret.":::

3. <span data-ttu-id="97cdf-145">Välj **privat Marketplace** från alternativen till vänster.</span><span class="sxs-lookup"><span data-stu-id="97cdf-145">Select **Private Marketplace** from the options on the left.</span></span>

    :::image type="content" source="media/private-azure/private-marketplace.png" alt-text="Välja Privat Marketplace i Azure Portal huvud fönstret.":::

4. <span data-ttu-id="97cdf-147">Välj **Kom igång** för att skapa en privat Azure Marketplace (du behöver bara göra det här en gång).</span><span class="sxs-lookup"><span data-stu-id="97cdf-147">Select **Get Started** to create Private Azure Marketplace (you only have to do this once).</span></span>

    :::image type="content" source="media/private-azure/private-marketplace-get-started.png" alt-text="Välj kom igång i Azure Portal huvud fönstret.":::

    <span data-ttu-id="97cdf-149">Om den privata Azure Marketplace redan finns för den här klienten, är **Hantera Marketplace** valt som standard.</span><span class="sxs-lookup"><span data-stu-id="97cdf-149">If Private Azure Marketplace already exists for this tenant, **Manage Marketplace** will be selected by default.</span></span>

5. <span data-ttu-id="97cdf-150">När du är klar har du en tom och inaktive rad privat Azure Marketplace.</span><span class="sxs-lookup"><span data-stu-id="97cdf-150">Once completed you will have an empty and disabled Private Azure Marketplace.</span></span>

    :::image type="content" source="media/private-azure/new-private-marketplace.png" alt-text="Den tomma privata Azure Marketplace-skärmen.":::

## <a name="add-items-from-gallery"></a><span data-ttu-id="97cdf-152">Lägg till objekt från galleriet</span><span class="sxs-lookup"><span data-stu-id="97cdf-152">Add items from gallery</span></span>

<span data-ttu-id="97cdf-153">Ett objekt är en kombination av ett erbjudande och en plan.</span><span class="sxs-lookup"><span data-stu-id="97cdf-153">An item is a combination of an offer and a plan.</span></span> <span data-ttu-id="97cdf-154">Du kan söka efter och lägga till objekt på sidan Hantera Marketplace.</span><span class="sxs-lookup"><span data-stu-id="97cdf-154">You can search for and add item in the Manage Marketplace page.</span></span>

1. <span data-ttu-id="97cdf-155">Välj **Lägg till objekt**.</span><span class="sxs-lookup"><span data-stu-id="97cdf-155">Select **Add items**.</span></span>

2. <span data-ttu-id="97cdf-156">Bläddra i **galleriet** eller Använd Sök fältet för att hitta det objekt som du vill använda.</span><span class="sxs-lookup"><span data-stu-id="97cdf-156">Browse the **Gallery** or use the search field to find the item you want.</span></span>

    :::image type="content" source="media/private-azure/marketplace-gallery.png" alt-text="Bläddra i galleriet eller Använd Sök fältet.":::

3. <span data-ttu-id="97cdf-158">Som standard kommer alla aktuella planer att läggas till i listan över tillåtna när du lägger till ett nytt erbjudande.</span><span class="sxs-lookup"><span data-stu-id="97cdf-158">As default, when adding a new offer, all current plans will be added to the allowed list.</span></span> <span data-ttu-id="97cdf-159">Om du vill ändra plan urvalet innan du lägger till de valda objekten väljer du den nedrullningsbara menyn i erbjudande panelen och uppdaterar de nödvändiga planerna.</span><span class="sxs-lookup"><span data-stu-id="97cdf-159">To modify the plan selection before adding the selected items, select the drop-down menu in the offer’s tile and update the required plans.</span></span>

    :::image type="content" source="media/private-azure/update-plans-400.png" alt-text="Uppdatera nödvändiga planer.":::

4. <span data-ttu-id="97cdf-161">Välj **klar** längst ned till vänster när du har gjort dina val.</span><span class="sxs-lookup"><span data-stu-id="97cdf-161">Select **Done** at the bottom-left after you've made your selections.</span></span>

>[!Note]
> <span data-ttu-id="97cdf-162">**Lägg till objekt** till Marketplace kommer endast att vara tillgängligt för erbjudanden som inte kommer från Microsoft.</span><span class="sxs-lookup"><span data-stu-id="97cdf-162">**Add Items** to the Marketplace will be available for non-Microsoft offers only.</span></span> <span data-ttu-id="97cdf-163">Microsoft-erbjudanden tillåts som standard.</span><span class="sxs-lookup"><span data-stu-id="97cdf-163">Microsoft offers are allowed by default.</span></span>

## <a name="edit-item-plans"></a><span data-ttu-id="97cdf-164">Redigera artikel planer</span><span class="sxs-lookup"><span data-stu-id="97cdf-164">Edit item plans</span></span>

<span data-ttu-id="97cdf-165">Du kan redigera ett objekts planer på sidan Hantera Marketplace.</span><span class="sxs-lookup"><span data-stu-id="97cdf-165">You can edit an item's plans in the Manage Marketplace page.</span></span>

1. <span data-ttu-id="97cdf-166">I kolumnen **planer** granskar du de tillgängliga planerna från List menyn för det objektet.</span><span class="sxs-lookup"><span data-stu-id="97cdf-166">In the **Plans** column, review the available plans from the dropdown menu for that item.</span></span>
2. <span data-ttu-id="97cdf-167">Markera eller avmarkera kryss rutorna för att välja vilka planer som ska vara tillgängliga för dina användare.</span><span class="sxs-lookup"><span data-stu-id="97cdf-167">Select or clear the checkboxes to choose which plans to make available to your users.</span></span>

    :::image type="content" source="media/private-azure/edit-items.png" alt-text="Markera eller avmarkera kryss rutan för det begärda objektet.":::

> [!NOTE]
> <span data-ttu-id="97cdf-169">Varje erbjudande måste ha minst en plan vald för att uppdateringen ska ske.</span><span class="sxs-lookup"><span data-stu-id="97cdf-169">Each offer needs at least one plan selected in order for the update to occur.</span></span> <span data-ttu-id="97cdf-170">Ta bort alla planer som är relaterade till ett erbjudande genom att ta bort hela erbjudandet (se nästa avsnitt).</span><span class="sxs-lookup"><span data-stu-id="97cdf-170">To remove all plans related to an offer, delete the entire offer (see next section).</span></span>

## <a name="delete-offers"></a><span data-ttu-id="97cdf-171">Ta bort erbjudanden</span><span class="sxs-lookup"><span data-stu-id="97cdf-171">Delete offers</span></span>

<span data-ttu-id="97cdf-172">På sidan Hantera marknads plats markerar du kryss rutan bredvid namnet på erbjudandet (se skärmen ovan) och väljer **ta bort objekt**.</span><span class="sxs-lookup"><span data-stu-id="97cdf-172">In the Manage Marketplace page, select the check box next to the offer name (see screen above) and select **Delete items**.</span></span>

## <a name="enabledisable-private-azure-marketplace"></a><span data-ttu-id="97cdf-173">Aktivera/inaktivera privat Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="97cdf-173">Enable/disable Private Azure Marketplace</span></span>

<span data-ttu-id="97cdf-174">På sidan Hantera Marketplace visas en av dessa banderoller som visar det aktuella läget för privat Azure Marketplace:</span><span class="sxs-lookup"><span data-stu-id="97cdf-174">In the Manage Marketplace page you will see one of these banners, which show the current state of Private Azure Marketplace:</span></span>

:::image type="content" source="media/private-azure/state-disable.png" alt-text="Inaktivera State-banderoll":::

:::image type="content" source="media/private-azure/state-enable.png" alt-text="Aktivera State-banderoll":::

<span data-ttu-id="97cdf-177">Du kan aktivera eller inaktivera privat Azure Marketplace efter behov.</span><span class="sxs-lookup"><span data-stu-id="97cdf-177">You can enable or disable Private Azure Marketplace as needed.</span></span>

- <span data-ttu-id="97cdf-178">Om det är inaktiverat väljer du **aktivera privat Marketplace** för att aktivera.</span><span class="sxs-lookup"><span data-stu-id="97cdf-178">If disabled, select **Enable Private Marketplace** to enable.</span></span>
- <span data-ttu-id="97cdf-179">Om aktive rad väljer du **Inaktivera privat Marketplace** för att inaktivera.</span><span class="sxs-lookup"><span data-stu-id="97cdf-179">If enabled, select **Disable Private Marketplace** to disable.</span></span>

## <a name="browsing-private-azure-marketplace"></a><span data-ttu-id="97cdf-180">Bläddra i privat Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="97cdf-180">Browsing Private Azure Marketplace</span></span>

<span data-ttu-id="97cdf-181">När privat Azure Marketplace är aktiverat ser användarna vilka planer som Marketplace-administratören har tillåtit.</span><span class="sxs-lookup"><span data-stu-id="97cdf-181">When Private Azure Marketplace is enabled, users will see which plans the Marketplace admin has allowed.</span></span>

- <span data-ttu-id="97cdf-182">Ett grönt **tillåtet** meddelande anger ett erbjudande för partner (inte Microsoft) som är tillåtet.</span><span class="sxs-lookup"><span data-stu-id="97cdf-182">A green **Allowed** notice indicates a Partner (non-Microsoft) offer that is allowed.</span></span>
- <span data-ttu-id="97cdf-183">Ett blått **tillåtet** meddelande indikerar ett Microsoft-erbjudande som är tillåtet.</span><span class="sxs-lookup"><span data-stu-id="97cdf-183">A blue **Allowed** notice indicates a Microsoft offer that is allowed.</span></span>

<span data-ttu-id="97cdf-184">Användare kan filtrera mellan erbjudanden som är och inte tillåtna:</span><span class="sxs-lookup"><span data-stu-id="97cdf-184">Users can filter between offers that are and are not allowed:</span></span>

:::image type="content" source="media/private-azure/filter-option.png" alt-text="Filtrerings alternativ.":::

## <a name="buy-or-deploy-in-private-azure-marketplace"></a><span data-ttu-id="97cdf-186">Köp eller distribuera i privat Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="97cdf-186">Buy or deploy in Private Azure Marketplace</span></span>

<span data-ttu-id="97cdf-187">Även om produkt informationens sid upplevelse liknar den offentliga Azure Marketplace finns det tre privata Azure Marketplace-scenarier.</span><span class="sxs-lookup"><span data-stu-id="97cdf-187">While the product details page experience is similar to the public Azure Marketplace, there are three Private Azure Marketplace specific scenarios.</span></span>

- <span data-ttu-id="97cdf-188">När en användare väljer en tillåten plan aktive ras knappen **skapa** :</span><span class="sxs-lookup"><span data-stu-id="97cdf-188">When a user selects an allowed plan, the **Create** button is enabled:</span></span>

    :::image type="content" source="media/private-azure/button-create-enabled.png" alt-text="Erbjudande banderoll med en plan kan skapas.":::

- <span data-ttu-id="97cdf-190">När en användare väljer en icke-tillåten plan, visar en banderoll om att planen inte är tillåten och knappen **skapa** är inaktive rad.</span><span class="sxs-lookup"><span data-stu-id="97cdf-190">When a user selects a non-allowed plan, a banner notes that the plan is not allowed and the **Create** button is disabled.</span></span>

   :::image type="content" source="media/private-azure/button-create-disabled.png" alt-text="Erbjudande banderollen det går inte att skapa en plan.":::

- <span data-ttu-id="97cdf-192">Om ett val av produkt plan inte visas på sidan produkt information men administratören har godkänt en eller flera planer, visar en banderoll vilka planer som är tillåtna och knappen **skapa** är aktive rad:</span><span class="sxs-lookup"><span data-stu-id="97cdf-192">If a product plan selection does not appear in the product details page but the admin approved one or more plans, a banner notes which plans are allowed and the **Create** button is enabled:</span></span>

    :::image type="content" source="media/private-azure/button-create-enabled-and-plans.png" alt-text="Erbjud banderoll som visar att en plan kan skapas och Visa tillgängliga planer.":::

## <a name="contact-support"></a><span data-ttu-id="97cdf-194">Kontakta supporten</span><span class="sxs-lookup"><span data-stu-id="97cdf-194">Contact support</span></span>

<span data-ttu-id="97cdf-195">Besök [Microsoft Q&A](/answers/products/)för support för Azure Marketplace.</span><span class="sxs-lookup"><span data-stu-id="97cdf-195">For Azure Marketplace support, visit [Microsoft Q&A](/answers/products/).</span></span> 
