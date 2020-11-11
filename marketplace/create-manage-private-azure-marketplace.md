---
title: Skapa och hantera privat Azure Marketplace i Azure Portal
description: Lär dig mer om att skapa och hantera privata Azure Marketplace (för hands version) i Azure Portal.
ms.prod: marketplace-customer
ms.topic: article
author: msjogarrig
ms.author: jogarrig
ms.date: 09/18/2020
ms.openlocfilehash: 1333bb2c8830cec83d7b7f05890af818d5c0ce5b
ms.sourcegitcommit: 95a5afdf68d88b6be848729830dcd114e3fb0c0f
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 11/11/2020
ms.locfileid: "94487711"
---
# <a name="create-and-manage-private-azure-marketplace-preview-in-the-azure-portal"></a><span data-ttu-id="cb9a4-103">Skapa och hantera privat Azure Marketplace (för hands version) i Azure Portal</span><span class="sxs-lookup"><span data-stu-id="cb9a4-103">Create and manage Private Azure Marketplace (preview) in the Azure portal</span></span>

<span data-ttu-id="cb9a4-104">Med privat Azure Marketplace (för hands version) kan administratörer styra vilka lösningar från tredje part som användarna kan använda.</span><span class="sxs-lookup"><span data-stu-id="cb9a4-104">Private Azure Marketplace (preview) lets administrators govern which third-party solutions their users can use.</span></span> <span data-ttu-id="cb9a4-105">Det gör det genom att låta dig distribuera endast erbjudanden som du godkänner och som uppfyller företagets principer.</span><span class="sxs-lookup"><span data-stu-id="cb9a4-105">It does this by allowing you to deploy only offers that you approve and that comply with your enterprise's policies.</span></span> <span data-ttu-id="cb9a4-106">Med en privat Azure Marketplace kan användarna söka i onlinebutiken efter kompatibla erbjudanden för köp och distribution.</span><span class="sxs-lookup"><span data-stu-id="cb9a4-106">With Private Azure Marketplace, your users can search the online store for compliant offers to purchase and deploy.</span></span> 

<span data-ttu-id="cb9a4-107">Som Marketplace-administratör (tilldelad roll) börjar du med en inaktive rad och en tom privat lagrings plats där du kan lägga till godkända erbjudanden och planer.</span><span class="sxs-lookup"><span data-stu-id="cb9a4-107">As a Marketplace admin (assigned role), you will start with a disabled and empty Private Store where you can add your approved offers and plans.</span></span> <span data-ttu-id="cb9a4-108">Den här artikeln beskriver hur du skapar, hanterar och aktiverar privat Azure Marketplace för dina användare.</span><span class="sxs-lookup"><span data-stu-id="cb9a4-108">This article explains how to create, manage, and enable Private Azure Marketplace for your users.</span></span>

<span data-ttu-id="cb9a4-109">Obs!</span><span class="sxs-lookup"><span data-stu-id="cb9a4-109">Notes:</span></span>

- <span data-ttu-id="cb9a4-110">En privat Azure Marketplace finns på klient nivå, så alla användare under klienten ser samma granskade lista.</span><span class="sxs-lookup"><span data-stu-id="cb9a4-110">Private Azure Marketplace is at a tenant level, so all users under the tenant will see the same curated list.</span></span>
- <span data-ttu-id="cb9a4-111">Alla Microsoft-lösningar läggs automatiskt till i privata Azure Marketplace.</span><span class="sxs-lookup"><span data-stu-id="cb9a4-111">All Microsoft solutions are automatically added to Private Azure Marketplace.</span></span>

## <a name="assign-the-marketplace-admin-role"></a><span data-ttu-id="cb9a4-112">Tilldela rollen Marketplace-administratör</span><span class="sxs-lookup"><span data-stu-id="cb9a4-112">Assign the Marketplace admin role</span></span>

<span data-ttu-id="cb9a4-113">Den globala klient organisationen måste tilldela rollen **Marketplace-administratör** till den privata Azure Marketplace-administratören som ska hantera den privata lagringen.</span><span class="sxs-lookup"><span data-stu-id="cb9a4-113">The tenant Global administrator must assign the **Marketplace admin** role to the Private Azure Marketplace admin who will manage the private store.</span></span>

>[!IMPORTANT]
> <span data-ttu-id="cb9a4-114">Åtkomst till privat Azure Marketplace-hantering är bara tillgänglig för IT-administratörer med rollen Marketplace-administratör tilldelad.</span><span class="sxs-lookup"><span data-stu-id="cb9a4-114">Access to Private Azure Marketplace management is only available to IT admins with the Marketplace admin role assigned.</span></span>

### <a name="prerequisites"></a><span data-ttu-id="cb9a4-115">Förutsättningar</span><span class="sxs-lookup"><span data-stu-id="cb9a4-115">Prerequisites</span></span>

<span data-ttu-id="cb9a4-116">Du måste uppfylla dessa krav innan du kan tilldela rollen Marketplace-administratör till en användare i klient omfånget:</span><span class="sxs-lookup"><span data-stu-id="cb9a4-116">You must meet these prerequisites before you can assign the Marketplace Admin role to a user on the tenant scope:</span></span>

- <span data-ttu-id="cb9a4-117">Du har åtkomst till en **Global administratörs** användare.</span><span class="sxs-lookup"><span data-stu-id="cb9a4-117">You have access to a **Global administrator** user.</span></span>
- <span data-ttu-id="cb9a4-118">Klienten har minst en prenumeration (kan vara av valfri typ).</span><span class="sxs-lookup"><span data-stu-id="cb9a4-118">The tenant has at least one Subscription (can be any type).</span></span>
- <span data-ttu-id="cb9a4-119">Den globala administratörs användaren tilldelas **deltagar** rollen eller högre för den prenumeration som valts i steg 2.</span><span class="sxs-lookup"><span data-stu-id="cb9a4-119">The Global administrator user is assigned the **Contributor** role or higher for the subscription chosen in step 2.</span></span>
- <span data-ttu-id="cb9a4-120">Den globala administratörs användaren har förhöjd åtkomst inställt på **Ja** (se [höjning-åtkomst-global-admin](/azure/role-based-access-control/elevate-access-global-admin)).</span><span class="sxs-lookup"><span data-stu-id="cb9a4-120">The Global administrator user has elevated access set to **Yes** (see [elevate-access-global-admin](/azure/role-based-access-control/elevate-access-global-admin)).</span></span>

### <a name="assign-the-marketplace-admin-role-with-powershell"></a><span data-ttu-id="cb9a4-121">Tilldela rollen Marketplace-administratör med PowerShell</span><span class="sxs-lookup"><span data-stu-id="cb9a4-121">Assign the Marketplace admin role with PowerShell</span></span>

<span data-ttu-id="cb9a4-122">Använd följande PowerShell-skript för att tilldela rollen Marketplace-administratör; den kräver följande parametrar:</span><span class="sxs-lookup"><span data-stu-id="cb9a4-122">Use the following PowerShell script to assign the Marketplace Admin role; it requires the following parameters:</span></span>

- <span data-ttu-id="cb9a4-123">**TenantId:** ID: t för klient organisationen i omfånget (Marketplace admin-rollen kan tilldelas i klientens omfång).</span><span class="sxs-lookup"><span data-stu-id="cb9a4-123">**TenantId:** The ID of the tenant in scope (Marketplace admin role is assignable on the tenant scope).</span></span>
- <span data-ttu-id="cb9a4-124">**SubscriptionId:** En prenumeration som den globala administratören har rollen **deltagare** eller högre tilldelad.</span><span class="sxs-lookup"><span data-stu-id="cb9a4-124">**SubscriptionId:** A subscription of which the global admin has **Contributor** role or higher assigned.</span></span>
- <span data-ttu-id="cb9a4-125">**GlobalAdminUsername:** Användar namnet för den globala administratören.</span><span class="sxs-lookup"><span data-stu-id="cb9a4-125">**GlobalAdminUsername:** The username of the global admin.</span></span>
- <span data-ttu-id="cb9a4-126">**UsernameToAssignRoleFor:** Det användar namn som Marketplace-administratörskonsolen ska tilldelas till.</span><span class="sxs-lookup"><span data-stu-id="cb9a4-126">**UsernameToAssignRoleFor:** The user name to which the Marketplace admin role will be assigned.</span></span>

> [!NOTE]
> <span data-ttu-id="cb9a4-127">För gäst användare som har bjudits in till klienten kan det ta upp till 48 timmar tills deras konto är tillgängligt för att tilldela Marketplace-administratörskonsolen.</span><span class="sxs-lookup"><span data-stu-id="cb9a4-127">For guest users invited to the tenant, it may take up to 48 hours until their account is available for assigning the Marketplace admin role.</span></span> <span data-ttu-id="cb9a4-128">Mer information finns i [Egenskaper för en Azure Active Directory B2B-samarbets användare](/azure/active-directory/b2b/user-properties).</span><span class="sxs-lookup"><span data-stu-id="cb9a4-128">For more information, see [Properties of an Azure Active Directory B2B collaboration user](/azure/active-directory/b2b/user-properties).</span></span>

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

$MarketPlaceAdminRole = Get-AzRoleDefinition $MarketplaceAdminRoleDefinitionName

if($MarketPlaceAdminRole -eq $null)
{
Write-Error -Message "'$($MarketplaceAdminRoleDefinitionName)' role is not available" -ErrorAction Stop
}
else
{
Write-Output -Message "'$($MarketplaceAdminRoleDefinitionName)' role is available"
}

Write-Output -Message "About to assign '$($MarketplaceAdminRoleDefinitionName)' role for $($UsernameToAssignRoleFor)..."

$elevatedAccessOnRoot = Get-AzRoleAssignment | where {$_.RoleDefinitionName -eq "User Access Administrator" -and $_.Scope -eq "/" -and $_.SignInName.Trim().ToLower() -eq $GlobalAdminUsername.Trim().ToLower() } | ft -Property SignInName

if($elevatedAccessOnRoot.Count -eq 0)
{
Write-Error -Message "$($GlobalAdminUsername) doesn't have permissions to assign '$($MarketplaceAdminRoleDefinitionName)'. Please verify it has elevated access 'On' in portal, https://docs.microsoft.com/en-us/azure/role-based-access-control/elevate-access-global-admin" -ErrorAction Stop
}
else
{
Write-Output "$GlobalAdminUsername has elevated access on root"
}

New-AzRoleAssignment -SignInName $UsernameToAssignRoleFor -RoleDefinitionName $MarketplaceAdminRoleDefinitionName -Scope "/providers/Microsoft.Marketplace"

}

Assign-MarketplaceAdminRole
```

<span data-ttu-id="cb9a4-129">Mer information om de cmdletar som finns i AZ. Portal PowerShell-modulen finns [Microsoft Azure PowerShell: portalens instrument panels-cmdletar](/powershell/module/az.portal/).</span><span class="sxs-lookup"><span data-stu-id="cb9a4-129">For more information about the cmdlets contained in the Az.Portal PowerShell module, see [Microsoft Azure PowerShell: Portal Dashboard cmdlets](/powershell/module/az.portal/).</span></span>

## <a name="create-private-azure-marketplace"></a><span data-ttu-id="cb9a4-130">Skapa en privat Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="cb9a4-130">Create Private Azure Marketplace</span></span>

1. <span data-ttu-id="cb9a4-131">Logga in på [Azure Portal](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="cb9a4-131">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="cb9a4-132">Välj **alla tjänster** och sedan **Marketplace**.</span><span class="sxs-lookup"><span data-stu-id="cb9a4-132">Select **All services** and then **Marketplace**.</span></span>

   :::image type="content" source="media/private-azure/azure-portal-marketplace.png" alt-text="Azure Portal huvud fönstret.":::

3. <span data-ttu-id="cb9a4-134">Välj **privat Marketplace** från alternativen till vänster.</span><span class="sxs-lookup"><span data-stu-id="cb9a4-134">Select **Private Marketplace** from the options on the left.</span></span>

    :::image type="content" source="media/private-azure/private-marketplace.png" alt-text="Välja Privat Marketplace i Azure Portal huvud fönstret.":::

4. <span data-ttu-id="cb9a4-136">Välj **Kom igång** för att skapa en privat Azure Marketplace (du behöver bara göra det här en gång).</span><span class="sxs-lookup"><span data-stu-id="cb9a4-136">Select **Get Started** to create Private Azure Marketplace (you only have to do this once).</span></span>

    :::image type="content" source="media/private-azure/private-marketplace-get-started.png" alt-text="Välj kom igång i Azure Portal huvud fönstret.":::

    <span data-ttu-id="cb9a4-138">Om den privata Azure Marketplace redan finns för den här klienten, är **Hantera Marketplace** valt som standard.</span><span class="sxs-lookup"><span data-stu-id="cb9a4-138">If Private Azure Marketplace already exists for this tenant, **Manage Marketplace** will be selected by default.</span></span>

5. <span data-ttu-id="cb9a4-139">När du är klar har du en tom och inaktive rad privat Azure Marketplace.</span><span class="sxs-lookup"><span data-stu-id="cb9a4-139">Once completed you will have an empty and disabled Private Azure Marketplace.</span></span>

    :::image type="content" source="media/private-azure/new-private-marketplace.png" alt-text="Den tomma privata Azure Marketplace-skärmen.":::

## <a name="add-items-from-gallery"></a><span data-ttu-id="cb9a4-141">Lägg till objekt från galleriet</span><span class="sxs-lookup"><span data-stu-id="cb9a4-141">Add items from gallery</span></span>

<span data-ttu-id="cb9a4-142">Ett objekt är en kombination av ett erbjudande och en plan.</span><span class="sxs-lookup"><span data-stu-id="cb9a4-142">An item is a combination of an offer and a plan.</span></span> <span data-ttu-id="cb9a4-143">Du kan söka efter och lägga till objekt på sidan Hantera Marketplace.</span><span class="sxs-lookup"><span data-stu-id="cb9a4-143">You can search for and add item in the Manage Marketplace page.</span></span>

1. <span data-ttu-id="cb9a4-144">Välj **Lägg till objekt**.</span><span class="sxs-lookup"><span data-stu-id="cb9a4-144">Select **Add items**.</span></span>

2. <span data-ttu-id="cb9a4-145">Bläddra i **galleriet** eller Använd Sök fältet för att hitta det objekt som du vill använda.</span><span class="sxs-lookup"><span data-stu-id="cb9a4-145">Browse the **Gallery** or use the search field to find the item you want.</span></span>

    :::image type="content" source="media/private-azure/marketplace-gallery.png" alt-text="Bläddra i galleriet eller Använd Sök fältet.":::

3. <span data-ttu-id="cb9a4-147">Som standard kommer alla aktuella planer att läggas till i listan över tillåtna när du lägger till ett nytt erbjudande.</span><span class="sxs-lookup"><span data-stu-id="cb9a4-147">As default, when adding a new offer, all current plans will be added to the allowed list.</span></span> <span data-ttu-id="cb9a4-148">Om du vill ändra plan urvalet innan du lägger till de valda objekten väljer du den nedrullningsbara menyn i erbjudande panelen och uppdaterar de nödvändiga planerna.</span><span class="sxs-lookup"><span data-stu-id="cb9a4-148">To modify the plan selection before adding the selected items, select the drop-down menu in the offer’s tile and update the required plans.</span></span>

    :::image type="content" source="media/private-azure/update-plans-400.png" alt-text="Uppdatera nödvändiga planer.":::

4. <span data-ttu-id="cb9a4-150">Välj **klar** längst ned till vänster när du har gjort dina val.</span><span class="sxs-lookup"><span data-stu-id="cb9a4-150">Select **Done** at the bottom-left after you've made your selections.</span></span>

>[!Note]
> <span data-ttu-id="cb9a4-151">**Lägg till objekt** till Marketplace kommer endast att vara tillgängligt för erbjudanden som inte kommer från Microsoft.</span><span class="sxs-lookup"><span data-stu-id="cb9a4-151">**Add Items** to the Marketplace will be available for non-Microsoft offers only.</span></span> <span data-ttu-id="cb9a4-152">Microsoft-erbjudanden tillåts som standard.</span><span class="sxs-lookup"><span data-stu-id="cb9a4-152">Microsoft offers are allowed by default.</span></span>

## <a name="edit-item-plans"></a><span data-ttu-id="cb9a4-153">Redigera artikel planer</span><span class="sxs-lookup"><span data-stu-id="cb9a4-153">Edit item plans</span></span>

<span data-ttu-id="cb9a4-154">Du kan redigera ett objekts planer på sidan Hantera Marketplace.</span><span class="sxs-lookup"><span data-stu-id="cb9a4-154">You can edit an item's plans in the Manage Marketplace page.</span></span>

1. <span data-ttu-id="cb9a4-155">I kolumnen **planer** granskar du de tillgängliga planerna från List menyn för det objektet.</span><span class="sxs-lookup"><span data-stu-id="cb9a4-155">In the **Plans** column, review the available plans from the dropdown menu for that item.</span></span>
2. <span data-ttu-id="cb9a4-156">Markera eller avmarkera kryss rutorna för att välja vilka planer som ska vara tillgängliga för dina användare.</span><span class="sxs-lookup"><span data-stu-id="cb9a4-156">Select or clear the checkboxes to choose which plans to make available to your users.</span></span>

    :::image type="content" source="media/private-azure/edit-items.png" alt-text="Markera eller avmarkera kryss rutan för det begärda objektet.":::

> [!NOTE]
> <span data-ttu-id="cb9a4-158">Varje erbjudande måste ha minst en plan vald för att uppdateringen ska ske.</span><span class="sxs-lookup"><span data-stu-id="cb9a4-158">Each offer needs at least one plan selected in order for the update to occur.</span></span> <span data-ttu-id="cb9a4-159">Ta bort alla planer som är relaterade till ett erbjudande genom att ta bort hela erbjudandet (se nästa avsnitt).</span><span class="sxs-lookup"><span data-stu-id="cb9a4-159">To remove all plans related to an offer, delete the entire offer (see next section).</span></span>

## <a name="delete-offers"></a><span data-ttu-id="cb9a4-160">Ta bort erbjudanden</span><span class="sxs-lookup"><span data-stu-id="cb9a4-160">Delete offers</span></span>

<span data-ttu-id="cb9a4-161">På sidan Hantera marknads plats markerar du kryss rutan bredvid namnet på erbjudandet (se skärmen ovan) och väljer **ta bort objekt**.</span><span class="sxs-lookup"><span data-stu-id="cb9a4-161">In the Manage Marketplace page, select the check box next to the offer name (see screen above) and select **Delete items**.</span></span>

## <a name="enabledisable-private-azure-marketplace"></a><span data-ttu-id="cb9a4-162">Aktivera/inaktivera privat Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="cb9a4-162">Enable/disable Private Azure Marketplace</span></span>

<span data-ttu-id="cb9a4-163">På sidan Hantera Marketplace visas en av dessa banderoller som visar det aktuella läget för privat Azure Marketplace:</span><span class="sxs-lookup"><span data-stu-id="cb9a4-163">In the Manage Marketplace page you will see one of these banners, which show the current state of Private Azure Marketplace:</span></span>

:::image type="content" source="media/private-azure/state-disable.png" alt-text="Inaktivera State-banderoll":::

:::image type="content" source="media/private-azure/state-enable.png" alt-text="Aktivera State-banderoll":::

<span data-ttu-id="cb9a4-166">Du kan aktivera eller inaktivera privat Azure Marketplace efter behov.</span><span class="sxs-lookup"><span data-stu-id="cb9a4-166">You can enable or disable Private Azure Marketplace as needed.</span></span>

1. <span data-ttu-id="cb9a4-167">Om det är inaktiverat väljer du **aktivera privat Marketplace** för att aktivera.</span><span class="sxs-lookup"><span data-stu-id="cb9a4-167">If disabled, select **Enable Private Marketplace** to enable.</span></span>
2. <span data-ttu-id="cb9a4-168">Om aktive rad väljer du **Inaktivera privat Marketplace** för att inaktivera.</span><span class="sxs-lookup"><span data-stu-id="cb9a4-168">If enabled, select **Disable Private Marketplace** to disable.</span></span>

## <a name="browsing-private-azure-marketplace"></a><span data-ttu-id="cb9a4-169">Bläddra i privat Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="cb9a4-169">Browsing Private Azure Marketplace</span></span>

<span data-ttu-id="cb9a4-170">När privat Azure Marketplace är aktiverat ser användarna vilka planer som Marketplace-administratören har tillåtit.</span><span class="sxs-lookup"><span data-stu-id="cb9a4-170">When Private Azure Marketplace is enabled, users will see which plans the Marketplace admin has allowed.</span></span>

- <span data-ttu-id="cb9a4-171">Ett grönt **tillåtet** meddelande anger ett erbjudande för partner (inte Microsoft) som är tillåtet.</span><span class="sxs-lookup"><span data-stu-id="cb9a4-171">A green **Allowed** notice indicates a Partner (non-Microsoft) offer that is allowed.</span></span>
- <span data-ttu-id="cb9a4-172">Ett blått **tillåtet** meddelande indikerar ett Microsoft-erbjudande som är tillåtet.</span><span class="sxs-lookup"><span data-stu-id="cb9a4-172">A blue **Allowed** notice indicates a Microsoft offer that is allowed.</span></span>

<span data-ttu-id="cb9a4-173">Användare kan filtrera mellan erbjudanden som är och inte tillåtna:</span><span class="sxs-lookup"><span data-stu-id="cb9a4-173">Users can filter between offers that are and are not allowed:</span></span>

:::image type="content" source="media/private-azure/filter-option.png" alt-text="Filtrerings alternativ.":::

## <a name="buy-or-deploy-in-private-azure-marketplace"></a><span data-ttu-id="cb9a4-175">Köp eller distribuera i privat Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="cb9a4-175">Buy or deploy in Private Azure Marketplace</span></span>

<span data-ttu-id="cb9a4-176">Även om produkt informationens sid upplevelse liknar den offentliga Azure Marketplace finns det tre privata Azure Marketplace-scenarier.</span><span class="sxs-lookup"><span data-stu-id="cb9a4-176">While the product details page experience is similar to the public Azure Marketplace, there are three Private Azure Marketplace specific scenarios.</span></span>

- <span data-ttu-id="cb9a4-177">När en användare väljer en tillåten plan aktive ras knappen **skapa** :</span><span class="sxs-lookup"><span data-stu-id="cb9a4-177">When a user selects an allowed plan, the **Create** button is enabled:</span></span>

    :::image type="content" source="media/private-azure/button-create-enabled.png" alt-text="Erbjudande banderoll med en plan kan skapas.":::

- <span data-ttu-id="cb9a4-179">När en användare väljer en icke-tillåten plan, visar en banderoll om att planen inte är tillåten och knappen **skapa** är inaktive rad.</span><span class="sxs-lookup"><span data-stu-id="cb9a4-179">When a user selects a non-allowed plan, a banner notes that the plan is not allowed and the **Create** button is disabled.</span></span>

   :::image type="content" source="media/private-azure/button-create-disabled.png" alt-text="Erbjudande banderollen det går inte att skapa en plan.":::

- <span data-ttu-id="cb9a4-181">Om ett val av produkt plan inte visas på sidan produkt information men administratören har godkänt en eller flera planer, visar en banderoll vilka planer som är tillåtna och knappen **skapa** är aktive rad:</span><span class="sxs-lookup"><span data-stu-id="cb9a4-181">If a product plan selection does not appear in the product details page but the admin approved one or more plans, a banner notes which plans are allowed and the **Create** button is enabled:</span></span>

    :::image type="content" source="media/private-azure/button-create-enabled-and-plans.png" alt-text="Erbjudande banderoll som visar att en plan kan skapas och visar tillgängliga planer.":::

## <a name="contact-support"></a><span data-ttu-id="cb9a4-183">Kontakta supporten</span><span class="sxs-lookup"><span data-stu-id="cb9a4-183">Contact support</span></span>

<span data-ttu-id="cb9a4-184">Besök [Microsoft Q&A](/answers/products/)för support för Azure Marketplace.</span><span class="sxs-lookup"><span data-stu-id="cb9a4-184">For Azure Marketplace support, visit [Microsoft Q&A](/answers/products/).</span></span> 
